# Comparing `tmp/nonebot_plugin_l4d2_server-0.6.0.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.6.0.tar` & `nonebot_plugin_l4d2_server-0.6.0.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0    35149 2023-07-16 09:49:04.006732 nonebot_plugin_l4d2_server-0.6.0/LICENSE
--rw-r--r--   0        0        0     5644 2023-07-16 09:49:04.006732 nonebot_plugin_l4d2_server-0.6.0/README.md
--rw-r--r--   0        0        0    19094 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-16 09:49:04.010732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     7067 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
--rw-r--r--   0        0        0     6135 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     9076 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     2054 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      369 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3574 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3363 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1344 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     3273 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1832 2023-07-16 09:49:04.014732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4211 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4174 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      665 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9492 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1083 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     4019 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1421 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7593 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     1296 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1294 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py
--rw-r--r--   0        0        0    12634 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     5211 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
--rw-r--r--   0        0        0     1587 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1337 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1551 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4067 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9345 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5979 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0     3220 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1219 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0      669 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     7725 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8521 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14963 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1695 2023-07-16 09:49:04.018732 nonebot_plugin_l4d2_server-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-22 11:39:30.920580 nonebot_plugin_l4d2_server-0.6.0.1/LICENSE
+-rw-r--r--   0        0        0     5749 2023-07-22 11:39:30.920580 nonebot_plugin_l4d2_server-0.6.0.1/README.md
+-rw-r--r--   0        0        0    18984 2023-07-22 11:39:30.924581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-22 11:39:30.924581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     7067 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
+-rw-r--r--   0        0        0     6135 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     9076 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     2971 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     2054 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      369 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3576 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      449 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3364 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1345 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     3275 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1831 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4179 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4176 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      665 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9413 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1084 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     4018 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1422 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7526 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     1297 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1294 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py
+-rw-r--r--   0        0        0    12635 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     5233 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
+-rw-r--r--   0        0        0     1588 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1339 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1569 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4067 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1186 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9326 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5975 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0     1017 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1219 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0      764 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     7291 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     9286 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    15415 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     3492 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py
+-rw-r--r--   0        0        0     1648 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/LICENSE` & `nonebot_plugin_l4d2_server-0.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/README.md` & `nonebot_plugin_l4d2_server-0.6.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,21 @@
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 顶置公告
 
-0.6.0更新了适配器，初步实现了v11,v12,kook的适配，以及qq频道的部分适配
+多适配器版本请查看[分支](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/tree/nb_adapter)
 
 文档暂时没时间更新ozr
 
+网页端管理端 `https://{ip}:{port}/l4d2`
+网页用户端 `https://{ip}:{port}/l4d2/user`
+
 ## 安装
 
 以下方法任选其一：
 
         nb plugin install nonebot-plugin-l4d2-server
         pip install nonebot-plugin-l4d2-server
         pipx install nonebot-plugin-l4d2-server
@@ -115,23 +118,21 @@
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 3
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 | 驴头 | 驴头服 | lvt | 4
 | 迷茫 | 迷茫 | 迷茫 | 10
 | 尸鬼 | 尸鬼狂潮 | ❀几❀ | 13
 
-
 ## To do
 
 - [ ] 帮助图片
 - [ ] 网页控制台查看服务器地图
 - [ ] 网页控制台启动和关闭服务器
 - [ ] 网页控制台管理封禁用户
 
-
 ## 其他
 
 - 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 - 如果本插件对你有帮助，不要忘了点个Star~
 - 本项目仅供学习使用，请勿用于商业用途
 - [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
-## é¡¶ç½®å¬å
-0.6.0æ´æ°äºééå¨ï¼åæ­¥å®ç°äºv11,v12,kookçééï¼ä»¥åqqé¢éçé¨åéé
-ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin
-install nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx
-install nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
+## é¡¶ç½®å¬å å¤ééå¨çæ¬è¯·æ¥ç[åæ¯](https://github.com/Agnes4m/
+nonebot_plugin_l4d2_server/tree/nb_adapter) ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr
+ç½é¡µç«¯ç®¡çç«¯ `https://{ip}:{port}/l4d2` ç½é¡µç¨æ·ç«¯ `https://{ip}:
+{port}/l4d2/user` ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin install
+nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx install
+nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server.git ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
 //github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
 l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
 ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml # éç½®æä»¶
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,67 +15,63 @@
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 from nonebot import require
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 require("nonebot_plugin_txt2img")
-require("nonebot_plugin_saa")
-from .l4d2_web import web, webUI
-
-from typing import Tuple, Union, List
-from time import sleep
 import time
+from time import sleep
+from typing import List, Tuple, Union
 
+from nonebot import get_driver, require
 from nonebot.matcher import Matcher
+from nonebot.params import Arg, ArgPlainText, CommandArg, Keyword, RegexGroup
 from nonebot.typing import T_State
-from nonebot.params import CommandArg, ArgPlainText, RegexGroup, Arg
-from nonebot import get_driver, require
-from typing import Annotated
-from nonebot.params import Keyword
 
-from .l4d2_utils.config import *
-from .l4d2_utils.utils import *
-from .l4d2_utils.command import *
-from .l4d2_image.steam import url_to_byte, url_to_byte_name
 from .l4d2_anne.server import updata_anne_server
 from .l4d2_data import sq_L4D2
-from .l4d2_push import *
-from .l4d2_image.vtfs import img_to_vtf
-from .l4d2_file import updown_l4d2_vpk, all_zip_to_one
+from .l4d2_file import all_zip_to_one, updown_l4d2_vpk
 from .l4d2_file.input_json import *
-from .l4d2_utils.txt_to_img import mode_txt_to_img
+from .l4d2_image.steam import url_to_byte, url_to_byte_name
+from .l4d2_image.vtfs import img_to_vtf
+from .l4d2_push import *
+from .l4d2_queries.qqgroup import add_ip, del_ip, get_number_url, show_ip
 from .l4d2_queries.utils import queries_server
-from .l4d2_queries.qqgroup import add_ip,show_ip,del_ip,get_number_url
+from .l4d2_utils.command import *
+from .l4d2_utils.config import *
+from .l4d2_utils.txt_to_img import mode_txt_to_img
+from .l4d2_utils.utils import *
+from .l4d2_web import web, webUI
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 from nonebot.plugin import PluginMetadata
 
 driver = get_driver()
 
 __version__ = "0.6.0"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
-    description="适配V11,v12,kook,qq频道的多平台nonebot2插件",
+    description="可用于管理求生之路查服和本地管理",
     usage="群内对有关求生之路的查询和操作",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
-    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~kaiheila"},
+    supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 
 """相当于启动就检查数据库"""
 
 
 @up.handle()
-async def _(matcher: Matcher, event: NoticeEvent_):
+async def _(matcher: Matcher, event: NoticeEvent):
     args = event.dict()
     if args["notice_type"] != "offline_file":
         matcher.set_arg("txt", args)  # type: ignore
         return
     l4_file_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
     map_path = Path(l4_file_path, vpk_path)  # type: ignore
     # 检查下载路径是否存在
@@ -156,19 +152,19 @@
     map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
     name_vpk = get_vpk(map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ""
     msg = mes_list(msg, name_vpk).replace(" ", "")
 
-    await mode_txt_to_img(mes, msg).send()
+    await matcher.finish(mode_txt_to_img(mes, msg))
 
 
 @del_vpk.handle()
-async def _(matcher: Matcher, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num", args)
 
 
 @del_vpk.got("num", prompt="你要删除第几个序号的地图(阿拉伯数字)")
 async def _(matcher: Matcher, tag: str = ArgPlainText("num")):
@@ -193,15 +189,15 @@
         if map_name:
             await matcher.finish("改名成功\n原名:" + map_name + "\n新名称:" + rename)
     except ValueError:
         await matcher.finish("参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称")
 
 
 @anne_player.handle()
-async def _(matcher: Matcher, event: MessageEvent, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     name = args.extract_plain_text()
     name = name.strip()
     at = await get_message_at(event.json())
     usr_id = at_to_usrid(at)
     if not usr_id:
         usr_id = event.user_id
     # 没有参数则从db里找数据
@@ -209,15 +205,15 @@
     if isinstance(msg, str):
         await matcher.finish(msg)
     elif isinstance(msg, bytes):
         await matcher.finish(MessageSegment.image(msg))
 
 
 @anne_bind.handle()
-async def _(matcher: Matcher, event: MessageEvent, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     tag = args.extract_plain_text()
     tag = tag.strip()
     if tag == "" or tag.isspace():
         await matcher.finish("虚空绑定?")
     usr_id = str(event.user_id)
     nickname = event.sender.card or event.sender.nickname
     if not nickname:
@@ -229,32 +225,32 @@
 @del_bind.handle()
 async def _(matcher: Matcher, event: MessageEvent):
     usr_id = event.user_id
     await matcher.finish(name_exist(str(usr_id)))
 
 
 @rcon_to_server.handle()
-async def _(matcher: Matcher, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("command", args)
 
 
 @rcon_to_server.got("command", prompt="请输入向服务器发送的指令")
 async def _(matcher: Matcher, tag: str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     try:
-        await mode_txt_to_img("服务器返回", msg).send()
+        await matcher.finish(mode_txt_to_img("服务器返回", msg))
     except:
         await matcher.finish(msg, reply_message=True)
 
 
 @check_path.handle()
-async def _(matcher: Matcher, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg.startswith("切换"):
         msg_number = int("".join(msg.replace("切换", " ").split()))
         if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
             await matcher.send("没有这个序号的路径呐")
         else:
             l4_config.l4_number = msg_number - 1
@@ -282,26 +278,26 @@
         await matcher.finish()
     ip_list = split_maohao(one_msg)
     msg = await queries_server(ip_list)
     await str_to_picstr(msg, matcher, keyword)
 
 
 @add_queries.handle()
-async def _(matcher: Matcher, event: GroupMessageEvent, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, event: GroupMessageEvent, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg) == 0:
         await matcher.finish("请在该指令后加入参数，例如【114.51.49.19:1810】")
     [host, port] = split_maohao(msg)
     group_id = event.group_id
     msg = await add_ip(group_id, host, port)
     await matcher.finish(msg)
 
 
 @del_queries.handle()
-async def _(event: GroupMessageEvent, matcher: Matcher, args: Message_ = CommandArg()):
+async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if not msg.isdigit():
         await matcher.finish("请输入正确的序号数字")
     group_id = event.group_id
     msg = await del_ip(group_id, msg)
     await matcher.finish(msg)
 
@@ -315,22 +311,22 @@
     if isinstance(msg, str):
         await matcher.finish(msg)
     else:
         await matcher.finish(MessageSegment.image(msg))
 
 
 @join_server.handle()
-async def _(args: Message_ = CommandArg()):
+async def _(args: Message = CommandArg()):
     msg = args.extract_plain_text()
     url = await get_number_url(msg)
     await join_server.finish(url)
 
 
 @up_workshop.handle()
-async def _(matcher: Matcher, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("ip", args)
 
 
 @up_workshop.got("ip", prompt="请输入创意工坊网址或者物品id")
 async def _(matcher: Matcher, state: T_State, tag: str = ArgPlainText("ip")):
@@ -338,25 +334,25 @@
     msg = await workshop_msg(tag)
     if not msg:
         await matcher.finish("没有这个物品捏")
     elif isinstance(msg, dict):
         pic = await url_to_byte(msg["图片地址"])
         if not pic:
             return
-        message:str = ''
+        message: str = ""
         for item, value in msg.items():
-            if item in ["图片地址", "下载地址", "细节"] or not isinstance(item,str):
+            if item in ["图片地址", "下载地址", "细节"] or not isinstance(item, str):
                 continue
-            message +=  item + ":" + value + "\n"
+            message += item + ":" + value + "\n"
         state["dic"] = msg
-        await MessageFactory([Image(pic),Text(message)]).send()
+        await matcher.finish(MessageSegment.image(pic) + (message))
     elif isinstance(msg, list):
         lenge = len(msg)
-        pic = await url_to_byte(msg[0]["图片地址"]) # type: ignore
-        message:str = f"有{lenge}个文件\n"
+        pic = await url_to_byte(msg[0]["图片地址"])  # type: ignore
+        message: str = f"有{lenge}个文件\n"
         ones = []
         for one in msg:
             for item, value in one.items():
                 if item in ["图片地址", "下载地址", "细节"]:
                     continue
                 message += f"{item}:{value}\n"
             ones.append(one)
@@ -387,25 +383,25 @@
                 await all_zip_to_one(data_file_list)
                 await upload_file(bot, event, data_file, file_name)
     else:
         await matcher.finish("已取消上传")
 
 
 @updata.handle()
-async def _(matcher: Matcher, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     """更新"""
     anne_ip_dict = await updata_anne_server()
     if not anne_ip_dict:
         await matcher.finish("网络开小差了捏")
     server_number = len(anne_ip_dict["云"])
     await matcher.finish(f"更新成功\n一共更新了{server_number}个电信anne服ip")
 
 
 @vtf_make.handle()
-async def _(matcher: Matcher, state: T_State, args: Message_ = CommandArg()):
+async def _(matcher: Matcher, state: T_State, args: Message = CommandArg()):
     msg: str = args.extract_plain_text()
     if msg not in ["拉伸", "填充", "覆盖", ""]:
         await matcher.finish("错误的图片处理方式")
     if msg == "":
         msg = "拉伸"
     state["way"] = msg
     logger.info("方式", msg)
@@ -437,31 +433,31 @@
         "left4dead2/addons/sourcemod/plugins",
     )
     name_smx = get_vpk(smx_path, file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ""
     msg = mes_list(msg, name_smx).replace(" ", "")
-    await mode_txt_to_img(mes, msg).send()
+    await matcher.finish(mode_txt_to_img(mes, msg))
 
 
 # @search_api.handle()
-# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message_ = CommandArg()):
+# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
 #     msg:str = args.extract_plain_text()
 #     # if msg.startswith('代码'):
 #         # 建图代码返回三方图信息
 #     data = await seach_map(msg,l4_config.l4_master[0],l4_config.l4_key)
 #     # else:
 #     if type(data) == str:
 #         await matcher.finish(data)
 #     else:
 #         state['maps'] = data
 #         await matcher.send(await map_dict_to_str(data))
 @help_.handle()
-async def _(matcher:Matcher):
+async def _(matcher: Matcher):
     msg = [
         "=====求生机器人帮助=====",
         "1、电信服战绩查询【求生anne[id/steamid/@]】",
         "2、电信服绑定【求生绑定[id/steamid]】",
         "3、电信服状态查询【云xx】" "4、创意工坊下载【创意工坊下载[物品id/链接]】",
         "5、指定ip查询【求生ip[ip]】(可以是域名)",
         "6、求生喷漆制作【求生喷漆】",
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from nonebot.log import logger
+from typing import List
 
 import pandas as pd
-from typing import List
+from nonebot.log import logger
 
-from .analysis import df_to_guoguanlv
-from ..l4d2_utils.seach import *
 from ..l4d2_data.players import L4D2Player
 from ..l4d2_image import out_png
+from ..l4d2_utils.seach import *
+from .analysis import df_to_guoguanlv
 
 # from .anne_telecom import ANNE_API
 
 
 s = L4D2Player()
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from .startand import SAVE_MAP, NUMBER_MAP
 import pandas as pd
 
+from .startand import NUMBER_MAP, SAVE_MAP
+
 
 async def df_to_guoguanlv(df: pd.DataFrame):
     """分析救援关过图率"""
     data = df[df["游戏模式"] == "AnneHappy药役"]
     other = df[df["游戏模式"].isin(["牛牛冲刺", "单人装逼"])]
     all_map = len(data["地图"])
     other_map = len(other["地图"])
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # from ..l4d2_image.steam import url_to_byte
 # from bs4 import BeautifulSoup
 # from typing import List
 
 # 暂时废弃
 # class ANNE_API:
-    
+
 #     async def __init__(
 #         self,
 #         STEAMID:str,
 #         tag:str
 #     ):
 #         self.STEAMID = STEAMID
 #         if tag == '中':
 #             msg1 = await self.anne_msg()
 #         elif tag == '长':
 #             msg1 = await self.anne_msg()
 #             msg1.update(await self.anne_map())
-        
-    
+
+
 #     async def anne_msg(self):
 #         """个人资料表"""
 #         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={self.STEAMID}')
 #         data_bs = BeautifulSoup(data_bytes, 'html.parser')
 #         data_fom = data_bs.find_all('table')
 #         n = 0
 #         data_dict = {}
@@ -43,15 +43,15 @@
 #         # 获取一言
 #         message = data_fom.select("html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span")
 #         msg_list = []
 #         for i in message:
 #             msg_list.append(i.text)
 #         data_list[0].update({"一言":msg_list})
 #         return data_list
-        
+
 #     async def anne_map(self):
 #         """个人地图表"""
 #         data_dict = {}
 #         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/timedmaps.php?steamid={self.STEAMID}')
 #         data_bs = BeautifulSoup(data_bytes, 'html.parser')
 #         tbody = data_bs.select('tbody')
 #         for tr in tbody:
@@ -68,9 +68,9 @@
 #                 else:
 #                     if title in data_dict:
 #                         data_dict[title].append(data_text)
 #                     else:
 #                         data_dict[title] = [data_text]
 #             if special_amount and refresh_interval:
 #                 data_dict['刷特时间'] = special_amount + refresh_interval
-                
-#         return data_dict
+
+#         return data_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import httpx
-from bs4 import BeautifulSoup
-import json
 import asyncio
-from typing import Dict, List, Set, Union, Tuple
+import json
 from pathlib import Path
+from typing import Dict, List, Set, Tuple, Union
 
+import httpx
+from bs4 import BeautifulSoup
 from nonebot.log import logger
-from ..l4d2_utils.config import CONFIG_PATH, anne_url, ANNE_IP, headers
 
 from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
+from ..l4d2_utils.config import ANNE_IP, CONFIG_PATH, anne_url, headers
 
 # 储存anne服务器ip
 anne_url = "https://sb.trygek.com/"
 # ANNE_IP = {}
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
 }
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import sqlite3
+
+from nonebot.log import logger
+
 from ..l4d2_utils.config import (
     DATASQLITE,
-    table_data,
+    L4d2_BOOLEAN,
+    L4d2_INTEGER,
     L4d2_players_tag,
     L4d2_server_tag,
-    L4d2_INTEGER,
     L4d2_TEXT,
-    L4d2_BOOLEAN,
+    table_data,
     tables_columns,
 )
-import sqlite3
-from nonebot.log import logger
 
 
 class L4D2DataSqlite:
     """连接数据库和断开数据库，以及一些检查函数"""
 
     def __init__(self):
         """连接数据库"""
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from ..l4d2_utils.config import DATASQLITE
 import sqlite3
-from typing import Union, Tuple, Optional, List
+from typing import List, Optional, Tuple, Union
+
+from ..l4d2_utils.config import DATASQLITE
 
 
 class L4D2Player:
     """数据库L4D2_Player表的操作"""
 
     def __init__(self):
         """连接数据库"""
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from ..l4d2_utils.config import DATASQLITE
 import sqlite3
 
+from ..l4d2_utils.config import DATASQLITE
+
 
 class L4D2Server:
     """数据库L4D2_server表的操作"""
 
     def __init__(self):
         """连接数据库"""
         self.datasqlite_path = DATASQLITE
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import io
+import os
+import sys
 from pathlib import Path
-from zipfile import ZipFile
 from time import sleep
-import sys
-import os
-import io
-from typing import List, Callable
+from typing import Callable, List
+from zipfile import ZipFile
 
-from ..l4d2_utils.utils import get_file, get_vpk
-from ..l4d2_utils.config import systems
-from nonebot.log import logger
-from rarfile import RarFile
 import rarfile
+from nonebot.log import logger
 from pyunpack import Archive
+from rarfile import RarFile
+
+from ..l4d2_utils.config import systems
+from ..l4d2_utils.utils import get_file, get_vpk
 
 
 async def updown_l4d2_vpk(map_paths: Path, name: str, url: str):
     """从url下载压缩包并解压到位置"""
     original_vpk_files = get_vpk(map_paths)
     down_file = Path(map_paths, name)
     if await get_file(url, down_file) == None:
@@ -28,19 +29,20 @@
     extracted_vpk_files = get_vpk(map_paths)
     # 获取新增vpk文件的list
     vpk_files = list(set(extracted_vpk_files) - set(original_vpk_files))
     return vpk_files
 
 
 import zipfile
-import rarfile
-from pyunpack import Archive
 from pathlib import Path
 from typing import Dict
 
+import rarfile
+from pyunpack import Archive
+
 SUPPORTED_EXTENSIONS = (".zip", ".7z", ".rar")
 
 
 def unzip_zipfile(down_file: Path, down_path: Path):
     """解压zip文件"""
     with support_gbk(zipfile.ZipFile(down_file, "r")) as z:
         z.extractall(down_path)
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from nonebot import on_notice
-from nonebot.adapters.onebot.v11 import NoticeEvent
-from pathlib import Path
-import httpx
-
 import json
+from pathlib import Path
 
+import httpx
+from nonebot import on_notice
+from nonebot.adapters.onebot.v11 import NoticeEvent
 
 upload = on_notice(priority=1)
 
 
 @upload.handle()
 async def _(event: NoticeEvent):
     try:
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from bs4 import BeautifulSoup
+from typing import List, Optional
+
 import jinja2
+from bs4 import BeautifulSoup
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
-from typing import List, Optional
-
 
 # from .htmlimg import dict_to_dict_img
 # from ..l4d2_anne.anne_telecom import ANNE_API
-from ..l4d2_utils.config import TEXT_PATH
+from ..l4d2_utils.config import TEXT_PATH, l4_config
 from .download import get_head_by_user_id_and_save
 from .send_image_tool import convert_img
 
-from ..l4d2_utils.config import l4_config
-
 template_path = TEXT_PATH / "template"
 
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import httpx
-from nonebot.log import logger
 import asyncio
 import hashlib
+import io
 import os
 import random
+
+import httpx
+from nonebot.log import logger
 from PIL import Image, ImageDraw
 from PIL.Image import Image as ImageS
-import io
+
 from ..l4d2_utils.config import PLAYERSDATA, TEXT_PATH
 
 # from .steam import web_player
 
 
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from io import BytesIO
-from pathlib import Path
-from base64 import b64encode
-from typing import Union, overload
-from typing import Union, Tuple, Optional
 import math
 import random
-
-import aiofiles
-from PIL import Image
-from httpx import get
 import sys
+from base64 import b64encode
+from io import BytesIO
 from pathlib import Path
-from typing import overload
+from typing import Optional, Tuple, Union, overload
 
+import aiofiles
+from httpx import get
+from PIL import Image
 
 MAIN_PATH = Path() / "data" / "GenshinUID"
 sys.path.append(str(MAIN_PATH))
 CONFIG_PATH = MAIN_PATH / "config.json"
 RESOURCE_PATH = MAIN_PATH / "resource"
 WIKI_PATH = MAIN_PATH / "wiki"
 CU_BG_PATH = MAIN_PATH / "bg"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from PIL import Image, ImageDraw, ImageFont
-from typing import List
 from pathlib import Path
+from typing import List
+
+from PIL import Image, ImageDraw, ImageFont
 
 # 半透明素材
 half_whitel_image_path = Path(__file__).parent.parent.joinpath("data/img/white.png")
 half_whitel_image = Image.open(half_whitel_image_path)
 
 
 async def one_server_img(msg: dict):
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # from PIL import Image
-import httpx
-import aiohttp
-
 # from bs4 import BeautifulSoup
 from typing import List, Optional
 from urllib.parse import unquote
 
+import aiohttp
+import httpx
 
 # async def web_player(url) -> Image :
 #     """steam个人资料获取头像"""
 #     data = BeautifulSoup(await url_for_byte(url), 'html.parser')
 #     print(data)
 #     head = data.find("div", class_="playerAvatarAutoSizeInner")
 #     img_elements = head.find_all("img")
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from PIL import Image
-from nonebot.log import logger
 from io import BytesIO
 
+from nonebot.log import logger
+from PIL import Image
+
 # import sys
 # sys.modules["srctools._cy_vtf_readwrite"] = None
 from srctools.vtf import VTF, ImageFormats
 
 
 async def img_to_vtf(pic_byte: bytes, tag) -> BytesIO:
     pic = BytesIO(pic_byte)
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from pathlib import Path
 import re
+from pathlib import Path
+from typing import Any, Dict, Optional, Union
+
 import a2s
-from typing import Dict, Union, Optional, Any
 
 try:
     import ujson as json
 except:
     import json
 
+from nonebot import get_bot, get_driver, on_command, require
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, Message, MessageSegment
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.log import logger
-from nonebot import get_driver, on_command, get_bot
-from nonebot import require
-from nonebot.permission import SUPERUSER
-from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import  MessageSegment
-from nonebot.adapters.onebot.v11.permission import (
-    GROUP_ADMIN,
-    GROUP_OWNER,
-)
+from nonebot.params import CommandArg
+from nonebot.permission import SUPERUSER
+
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
-from ..l4d2_utils.rule import MessageFactory,Image,Text,GroupEvent_,Message_
-from ..l4d2_utils.command import get_ip_to_mes
-from ..l4d2_utils.utils import extract_last_digit, split_maohao,get_group_id
 from ..l4d2_queries.utils import json_server_to_tag_dict, queries_dict
+from ..l4d2_utils.command import get_ip_to_mes
 from ..l4d2_utils.config import l4_config
+from ..l4d2_utils.utils import extract_last_digit, split_maohao
 
 driver = get_driver()
 sch_json = Path("data/L4D2/scheduler.json")
 if not sch_json.exists():
     with sch_json.open("w") as f:
         json.dump({}, f, ensure_ascii=False)
 
@@ -45,42 +42,42 @@
     aliases={"求生定时删除"},
     priority=30,
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
 )
 
 
 @add_rss.handle()
-async def _(event: GroupEvent_, matcher: Matcher, args: Message_ = CommandArg()):
-    group_id = get_group_id(event)
+async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
+    group_id = event.group_id
     if not group_id:
         return
     msg = args.extract_plain_text()
     command, message = await extract_last_digit(msg)
     push_msg = await get_ip_to_mes(msg=message, command=command)
     if not push_msg:
         return
     if push_msg in ["服务器无响应", None]:
         await matcher.finish("无响应的服务器，请检查")
     else:
         return_msg = await add_or_update_data(group_id, msg)
         if isinstance(push_msg, bytes):
-            await MessageFactory([Image(push_msg)]).send()
-        elif isinstance(push_msg, MessageFactory):
-            await push_msg.send()
+            await matcher.finish(MessageSegment.image(push_msg))
+        elif isinstance(push_msg, Message | MessageSegment):
+            await matcher.finish(push_msg)
         else:
             await matcher.send(push_msg)
         if return_msg == "add":
             await matcher.send(f"已添加群定时任务【{msg}】{l4_config.l4_push_times}次")
         elif return_msg in ["update", "change"]:
             await matcher.send(f"已更新群定时任务【{msg}】{l4_config.l4_push_times}次")
 
 
 @del_rss.handle()
-async def _(event: GroupEvent_, matcher: Matcher):
-    group_id = get_group_id(event)
+async def _(event: GroupMessageEvent, matcher: Matcher):
+    group_id = event.group_id
     if not group_id:
         return
     await add_or_update_data(group_id, "", ad_mode="del")
     await matcher.finish("已删除群定时任务")
 
 
 async def add_or_update_data(group_i: int, some_str: str = "", ad_mode: str = "add"):
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import List, Tuple, Dict
-from .localIP import Group_All_HOST, ALL_HOST
+from typing import Dict, List, Tuple
+
 from ..l4d2_utils.utils import split_maohao
+from .localIP import ALL_HOST, Group_All_HOST
 from .qqgroup import qq_ip_querie
 
 
 async def get_group_ip_to_msg(command: str, text: str = ""):
     """输出群组ip"""
     if not text:
         group_tag_list: List[str] = Group_All_HOST[command]
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import asyncio
+import random
+from typing import Any, Dict, List, Tuple, Union
+
+from nonebot.log import logger
+
 from ..l4d2_data.serverip import L4D2Server
 from ..l4d2_image import server_ip_pic
+from ..l4d2_utils.message import KAILAO, PRISON, QUEREN
+from ..l4d2_utils.utils import split_maohao
+from .localIP import ALL_HOST
 from .utils import (
-    queries,
+    msg_ip_to_list,
     player_queries,
-    queries_dict,
     player_queries_anne_dict,
-    msg_ip_to_list,
+    queries,
+    queries_dict,
 )
-from nonebot.log import logger
-import random
-import asyncio
-from ..l4d2_utils.utils import split_maohao
-from ..l4d2_utils.message import PRISON, QUEREN, KAILAO
-from .localIP import ALL_HOST
-from typing import List, Dict, Any, Tuple, Union
 
 try:
     import ujson as json
 except:
     import json
 si = L4D2Server()
 errors = (
@@ -97,15 +99,15 @@
                 )
             except ValueError:
                 continue  # 处理异常情况
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
         # msg_list.sort(key=lambda x: x["number"])
-        send_list =  sorted(msg_list, key=lambda x: int(x["number"]))
+        send_list = sorted(msg_list, key=lambda x: int(x["number"]))
         result = {"msg_list": send_list}
 
     else:
         result: Dict[str, List[Dict[str, Any]]] = {}
     return result
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_queries/utils.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
-import struct
-import a2s
 import random
-from pydantic import BaseModel
+import struct
 from typing import List
+
+import a2s
 from nonebot.log import logger
+from pydantic import BaseModel
+
 from ..l4d2_utils.config import l4_config
 from ..l4d2_utils.txt_to_img import mode_txt_to_img
 from ..l4d2_utils.utils import split_maohao
 from .localIP import ALL_HOST
 
 
 class GROUP_MSG(BaseModel):
@@ -44,17 +46,19 @@
     return msgs
 
 
 async def get_anne_server_ip(ip, ismsg: bool = False):
     """输出查询ip和ping"""
     host, port = split_maohao(ip)
     data = await queries_server([host, port])
-    
+
     if l4_config.l4_image:
-        data = mode_txt_to_img(data.split("\n")[0],data.replace(data.split("\n")[0],f"\nconnect {ip}"))
+        data = mode_txt_to_img(
+            data.split("\n")[0], data.replace(data.split("\n")[0], f"\nconnect {ip}")
+        )
     else:
         data += f"\nconnect {ip}"
     return data
 
 
 async def json_server_to_tag_dict(key: str, msg: str):
     """
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
+
+from rcon.source.async_rcon import close, communicate
 from rcon.source.proto import Packet, Type
-from rcon.source.async_rcon import communicate, close
 
 
 async def main(host):
     host = "43.142.178.212"
     port = 40003
     password = "1145149191810"
     encoding = "utf-8"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from rcon.source import rcon
 import asyncio
 from pathlib import Path
-from ..l4d2_utils.config import l4_config, CHECK_FILE
+
+from rcon.source import rcon
+
+from ..l4d2_utils.config import CHECK_FILE, l4_config
 
 
 async def rcon_server(PASSWORD: str, msg: str):
     # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
     # return response
     try:
         response = await asyncio.wait_for(
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from typing import Dict, List, Union
+
 import httpx
-from typing import Dict,List,Union
 from nonebot.log import logger
 
 try:
     import ujson as json
 except:
     import json
 
@@ -17,39 +18,39 @@
         return await primary_map(i)
     else:
         return await only_map(i)
 
 
 async def api_get_json(msg: str):
     url_serach = "https://db.steamworkshopdownloader.io/prod/api/details/file"
-    data:Dict[str,str] = {msg: ''}
+    data: Dict[str, str] = {msg: ""}
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
     }
     data_msg = httpx.post(url=url_serach, headers=headers, data=data).content.decode(
         "utf-8"
     )
     logger.info(data_msg)
     out = {}
     data_msg = data_msg[1:-1]
-    datas:Dict[str,str] = json.loads(data_msg)
+    datas: Dict[str, str] = json.loads(data_msg)
     return datas
 
 
-async def only_map(i: Dict[str,str]):
+async def only_map(i: Dict[str, str]):
     """单地图下载"""
-    out:Dict[str,str] = {}
+    out: Dict[str, str] = {}
     out["名字"] = i["title"]
     out["游戏"] = i["app_name"]
     out["下载地址"] = i["file_url"]
     out["图片地址"] = i["preview_url"]
     out["细节"] = i["file_description"]
     return out
 
 
-async def primary_map(i:Dict[str,List[Dict[str,str]]]):
+async def primary_map(i: Dict[str, List[Dict[str, str]]]):
     """主地图返回多地图参数"""
-    map_list:List[Union[Dict[str,List[Dict[str,str]]],Dict[str,str]]] = []
+    map_list: List[Union[Dict[str, List[Dict[str, str]]], Dict[str, str]]] = []
     map_list.append(i)
     for one in i["children"]:
         map_list.append(await api_get_json(one["publishedfileid"]))
     return map_list
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any, Tuple
 
+from nonebot import get_bot, get_driver, on_command, on_regex
+from nonebot.adapters.onebot.v11 import Bot, MessageEvent, MessageSegment
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import RegexGroup
 from nonebot.permission import SUPERUSER
-from nonebot import get_bot, on_regex, get_driver, on_command
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, MessageSegment
 
-from ..l4d2_utils.utils import register_menu
 from ..l4d2_utils.rule import FullCommand
+from ..l4d2_utils.utils import register_menu
 from .draw_update_log import draw_update_log_img
-from .restart import restart_message, restart_genshinuid
+from .restart import restart_genshinuid, restart_message
 
 l4d_restart = on_command("l4重启", rule=FullCommand())
 get_update_log = on_command("l4更新记录", rule=FullCommand())
 l4d_update = on_regex(
     r"^(l4)(强行)?(强制)?(更新)$",
     block=True,
 )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import Union
 
+from .update import update_from_git
+
 # from PIL import Image, ImageDraw
 
-from .update import update_from_git
 
 # from ..l4d2_image.image import convert_img
 # from ..l4d2_image.image import get_color_bg
 # from ..utils.genshin_fonts.genshin_fonts import genshin_font_origin
 
 R_PATH = Path(__file__).parent
 TEXT_PATH = R_PATH / "texture2d"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
-import sys
 import json
-import time
+import os
 import platform
 import subprocess
+import sys
+import time
 from pathlib import Path
 
 # from ..utils.db_operation.db_operation import config_check
 
 bot_start = Path().cwd() / "bot.py"
 restart_sh_path = Path().cwd() / "gs_restart.sh"
 update_log_path = Path(__file__).parent / "update_log.json"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import List, Union
 
 import git
-from nonebot.log import logger
 from git.exc import GitCommandError
+from nonebot.log import logger
 
 
 async def update_from_git(
     level: int = 0,
     repo_path: Union[str, Path, None] = None,
     log_config: dict = {
         "key": "✨🐛🎨⚡🍱♻️",
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-import re
 import asyncio
-from typing import Type, List, Tuple
+import re
 from time import sleep
+from typing import List, Tuple, Type
 
-from nonebot import on_notice, on_command, on_regex, on_keyword
-from nonebot.params import CommandArg, RawCommand, CommandStart
+from nonebot import on_command, on_keyword, on_notice, on_regex
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import (
-    GroupMessageEvent
-)
+from nonebot.params import CommandArg, CommandStart, RawCommand
 
-
-from ..l4d2_anne.server import server_key, ANNE_IP, group_key
-from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
-from .config import *
-from ..l4d2_queries.qqgroup import split_maohao, get_tan_jian, qq_ip_queries_pic
+from ..l4d2_anne.server import ANNE_IP, group_key, server_key
+from ..l4d2_image.one import one_server_img
 from ..l4d2_queries import get_group_ip_to_msg
-
+from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
+from ..l4d2_queries.qqgroup import get_tan_jian, qq_ip_queries_pic, split_maohao
 from ..l4d2_queries.utils import get_anne_server_ip, json_server_to_tag_dict
+from .config import *
+from .rule import *
+from .txt_to_img import mode_txt_to_img
 
 # from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
 from .utils import *
-from .txt_to_img import mode_txt_to_img
-from ..l4d2_image.one import one_server_img
-from .rule import *
-
 
 help_ = on_command("l4_help", aliases={"求生帮助"}, priority=20, block=True)
 
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
@@ -98,16 +93,14 @@
 # 下载内容
 up_workshop = on_command(
     "workshop", aliases={"创意工坊下载", "求生创意工坊"}, priority=20, block=True
 )
 vtf_make = on_command("vtf_make", aliases={"求生喷漆"}, priority=20, block=True)
 
 
-
-
 matchers: Dict[str, List[Type[Matcher]]] = {}
 
 
 async def get_des_ip():
     """初始化"""
     global ALL_HOST
     global ANNE_IP
@@ -158,50 +151,49 @@
 
 async def get_read_ip(ip_anne_list: List[Tuple[str, str, str]]):
     get_ip = on_command("云", aliases=server_key(), priority=50, block=True)
 
     @get_ip.handle()
     async def _(
         matcher: Matcher,
-        event: Event_,
+        event: MessageEvent,
         start: str = CommandStart(),
         command: str = RawCommand(),
-        args: Message_ = CommandArg(),
+        args: Message = CommandArg(),
     ):
         if start:
             command = command.replace(start, "")
         if command == "anne":
             command = "云"
         msg: str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
         if not push_msg:
             return
-        if isinstance(push_msg,MessageFactory):
+        if isinstance(push_msg, Message):
             logger.info("构造")
             try:
-                await push_msg.finish()
+                await matcher.finish(push_msg)
             except Exception as E:
                 logger.warning(E)
                 return
         elif isinstance(push_msg, bytes):
             logger.info("直接发送图片")
-            send_msg = Image(push_msg)
+            send_msg = MessageSegment.image(push_msg)
         elif msg and type(push_msg) == list:
             logger.info("更加构造函数")
-            send_msg = MessageFactory([Image(push_msg[0]), Text(push_msg[-1])])
+            send_msg = Message(MessageSegment.image(push_msg[0]) + push_msg[-1])
         elif msg and isinstance(push_msg, str):
-            send_msg = MessageFactory(push_msg)
+            send_msg = push_msg
         else:
             logger.info("出错了")
             return
         logger.info(type(send_msg))
         if not send_msg:
             logger.warning("没有")
-        await send_msg.send()
-        await matcher.finish()
+        await matcher.finish(send_msg)
 
 
 async def get_ip_to_mes(msg: str, command: str = ""):
     if not msg:
         # 以图片输出全部当前
         igr = False
         # if command in gamemode_list:
@@ -245,40 +237,40 @@
     get_grou_ip = on_command("anne", aliases=group_key(), priority=80, block=True)
 
     @get_grou_ip.handle()
     async def _(
         matcher: Matcher,
         start: str = CommandStart(),
         command: str = RawCommand(),
-        args: Message_ = CommandArg(),
+        args: Message = CommandArg(),
     ):
         if start:
             command = command.replace(start, "")
         msg: str = args.extract_plain_text()
         push_msg = await get_group_ip_to_msg(msg, command)
         if isinstance(push_msg, bytes):
-            send_msg = MessageFactory(Image(push_msg))
+            send_msg = MessageSegment.image(push_msg)
         elif msg and type(push_msg) == list:
-            send_msg = MessageFactory([Image(push_msg[0]), Text(push_msg[-1])])
+            send_msg = Message(MessageSegment.image(push_msg[0]) + push_msg[-1])
         elif msg and isinstance(push_msg, str):
             await str_to_picstr(push_msg, matcher)
 
 
-# tests = on_command("测试1")     
+# tests = on_command("测试1")
 
 # @tests.handle()
 # async def _(event: Event,arg:Message=CommandArg()):
 #     logger.info(event)
 #     logger.info(arg.extract_plain_text())
 
 
 async def init():
     global matchers
     # print('启动辣')
-    from ..l4d2_update import l4d_restart, l4d_update, get_update_log, driver
+    from ..l4d2_update import driver, get_update_log, l4d_restart, l4d_update
 
     await get_des_ip()
 
 
 @driver.on_startup
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-from pathlib import Path
-from typing import List, Dict, Any
-
 import platform
+from pathlib import Path
+from typing import Any, Dict, List
 
-from ruamel import yaml
-from pydantic import BaseModel, Field
-
-
-from nonebot.permission import SUPERUSER
 from nonebot import get_driver
-from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
-
+from nonebot.log import logger
+from nonebot.permission import SUPERUSER
+from pydantic import BaseModel, Field
+from ruamel import yaml
 
 file_format = (".vpk", ".zip", ".7z", "rar")
 # 权限
 
 driver = get_driver()
 COMMAND_START = list(driver.config.command_start)
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bs4 import BeautifulSoup
 import httpx
+from bs4 import BeautifulSoup
 
 
 def anne_search(name: str):
     """输入名字返回列表["""
     url = "https://sb.trygek.com/l4d_stats/ranking/search.php"
     data = {"search": name}
     headers = {"Content-Type": "application/x-www-form-urlencoded"}
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent
-from nonebot.log import logger
-from nonebot.matcher import Matcher
-import httpx
+import json
 import os
+import tempfile
 from pathlib import Path
-from typing import List, Dict, Union, Optional
-from .config import *
-from ..l4d2_anne import write_player, del_player, anne_message
-from ..l4d2_server.rcon import read_server_cfg_rcon, rcon_server
-from ..l4d2_server.workshop import workshop_to_dict
+from typing import Dict, List, Optional, Union
+
+import httpx
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
+from nonebot.log import logger
+from nonebot.matcher import Matcher
+
+from ..l4d2_anne import anne_message, del_player, write_player
 from ..l4d2_image.steam import url_to_byte
+from ..l4d2_server.rcon import rcon_server, read_server_cfg_rcon
+from ..l4d2_server.workshop import workshop_to_dict
+from .config import *
 from .rule import *
 from .txt_to_img import mode_txt_to_img
-import tempfile
-import json
 
 
 async def get_file(url: str, down_file: Path):
     """
     下载指定Url到指定位置
     """
     try:
@@ -224,17 +226,17 @@
     """判断图片输出还是正常输出"""
     if l4_config.l4_image:
         lines = push_msg.splitlines()
         first_str = lines[0]
         last_str = lines[-1]
         push_msg = "\n".join(lines[1:-1])
         if l4_config.l4_connect:
-            await mode_txt_to_img(first_str, push_msg,last_str).send()
+            await matcher.finish(mode_txt_to_img(first_str, push_msg, last_str))
         else:
-            await mode_txt_to_img(first_str, push_msg).send()
+            await matcher.finish(mode_txt_to_img(first_str, push_msg))
     else:
         if l4_config.l4_connect or keyword == "connect":
             await matcher.send(push_msg)
         else:
             await matcher.send("\n".join(push_msg.splitlines()[1:-2]))
 
 
@@ -246,21 +248,7 @@
         msgs: List[str] = msg.split("：")
     elif msg.replace(".", "").isdigit():
         msgs: List[str] = [msg, "20715"]
     else:
         msgs = []
     mse = [msgs[0], msgs[-1]]
     return mse
-
-def get_group_id(event: GroupEvent_) -> Optional[int]:
-    if isinstance(event, (V11GroupMessageEvent, V12GroupMessageEvent)):
-        group_id = event.group_id
-    elif isinstance(event, kaiheilaChannelMessageEvent):
-        group_id = int(event.group_id)
-    elif isinstance(event, qqguidChannelEvent):
-        if event.id:
-            group_id = event.id
-        else:
-            group_id = None
-    else:
-        group_id =  None
-    return group_id
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import datetime
-from typing import Optional, Union
+from pathlib import Path
+from typing import Optional
 
-from fastapi import FastAPI
-from fastapi import Header, HTTPException, Depends
-from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
+from fastapi import Depends, FastAPI, Header, HTTPException
+from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from jose import jwt
-from jose.exceptions import JWTError, ExpiredSignatureError
-from nonebot import get_bot, get_app
-
-from pathlib import Path
+from jose.exceptions import ExpiredSignatureError, JWTError
+from nonebot import get_adapter, get_app, get_driver, logger
+from nonebot.adapters.onebot.v11 import Adapter
 
-from nonebot import get_driver, logger
+from ..l4d2_queries.qqgroup import qq_ip_querie
 from ..l4d2_utils.config import *
 from ..l4d2_utils.utils import split_maohao
-from ..l4d2_queries.qqgroup import qq_ip_querie
 
 CONFIG_PATH = Path() / "data" / "L4D2" / "l4d2.yml"
 
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 
-from .webUI import login_page, admin_app
+from .webUI import admin_app, login_page
+from .webUI_s import user_app
 
 requestAdaptor = """
 requestAdaptor(api) {
     api.headers["token"] = localStorage.getItem("token");
     return api;
 },
 """
@@ -94,15 +93,19 @@
     @app.get(
         "/l4d2/api/get_group_list",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_group_list_api():
         try:
-            group_list = await get_bot().get_group_list()
+            bots = get_adapter(Adapter).bots
+            if len(bots) == 0:
+                return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+            bot = list(bots.values())[0]
+            group_list = await bot.get_group_list()
             group_list = [
                 {
                     "label": f'{group["group_name"]}({group["group_id"]})',
                     "value": group["group_id"],
                 }
                 for group in group_list
             ]
@@ -123,15 +126,18 @@
     @app.get(
         "/l4d2/api/l4d2_global_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_l4d2_global_config():
         try:
-            bot = get_bot()
+            bots = get_adapter(Adapter).bots
+            if len(bots) == 0:
+                return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+            bot = list(bots.values())[0]
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
                 members = await bot.get_group_member_list(group_id=group["group_id"])
                 member_list.extend(
                     [
                         {
@@ -145,14 +151,15 @@
             config["member_list"] = member_list
             config["l4_styles"] = ["standard", "black"]
 
             return config
         except ValueError:
             return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
+    @app.get("/l4d2/api/user/get_query_contexts", response_class=JSONResponse)
     @app.get(
         "/l4d2/api/get_query_contexts",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_query_context():
         try:
@@ -164,14 +171,15 @@
                 for d in v:
                     host, port = split_maohao(d["ip"])
                     ip_lists.append((d["id"], ip_list, host, port))
             data_dict = await qq_ip_querie(ip_lists)
             if not data_dict:
                 return {"status": -100, "msg": "返回失败，请确保有可用的服务器ip"}
             data_list = data_dict["msg_list"]
+            # logger.info(data_list)
             return {
                 "status": 0,
                 "msg": "ok",
                 "data": {
                     "items": data_list,
                     "total": len(data_list),
                 },
@@ -237,7 +245,14 @@
     async def admin_page_app():
         return admin_app.render(
             site_title="l4d2-l4d2 后台管理",
             theme="ang",
             requestAdaptor=requestAdaptor,
             responseAdaptor=responseAdaptor,
         )
+
+    @app.get("/l4d2/user", response_class=HTMLResponse)
+    async def user_page_app():
+        return user_app.render(
+            site_title="l4d2服务器查询",
+            theme="ang",
+        )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from amis import ActionType, TableCRUD, TableColumn
-from amis import PageSchema, Switch, InputNumber, InputTag, Action, App
 from amis import (
-    Form,
-    InputText,
-    InputPassword,
+    Action,
+    ActionType,
+    Alert,
+    AmisAPI,
+    App,
     DisplayModeEnum,
+    Flex,
+    Form,
     Horizontal,
-    Remark,
     Html,
+    InputNumber,
+    InputPassword,
+    InputTag,
+    InputText,
+    LevelEnum,
     Page,
-    AmisAPI,
+    PageSchema,
+    Remark,
+    Select,
+    Switch,
+    TableColumn,
+    TableCRUD,
+    Tpl,
     Wrapper,
 )
-from amis import LevelEnum, Select, Alert, Tpl, Flex
-
 
 from ..l4d2_utils.config import NICKNAME
 
 logo = Html(
     html="""
 <p align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
-        <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
+        <img src="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
          width="256" height="256" alt="l4d2-server">
     </a>
 </p>
 <h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
 <div align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
     Github仓库</a>
@@ -101,14 +111,22 @@
         ),
         InputText(
             label="字体",
             name="l4_font",
             value="${l4_font}",
             labelRemark=Remark(shape="circle", content="机器人返回图片中文字的字体。"),
         ),
+        Switch(
+            label="是否图片发送单服务器查询",
+            name="l4_image",
+            value="${l4_image}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="开启时，会查询单服务器会使用图片，避免长信息风控"),
+        ),
         Select(
             label="图片风格",
             name="l4_style",
             value="${l4_style}",
             source="${l4_styles}",
             labelRemark=Remark(shape="circle", content="仅仅是批量查询的风格"),
         ),
@@ -343,15 +361,16 @@
             confirmText="加入steam://connect/" + "${ip}",
             url="steam://connect/" + "${ip}",
             # url= "http://"+'${ip}',
             blank=True,
         ),
     ],
     columns=[
-        TableColumn(label="服主", name="master", searchable=True),
+        TableColumn(label="服主", name="tag", searchable=True),
+        TableColumn(label="序号", name="number", searchable=True),
         TableColumn(label="名称", name="name", searchable=True),
         TableColumn(label="地图", name="map_", searchable=True),
         TableColumn(label="玩家", name="rank_players", searchable=True),
         TableColumn(label="延迟", name="ping", searchable=True),
         TableColumn(label="IP 地址", name="ip", searchable=True),
     ],
 )
@@ -396,14 +415,15 @@
         ],
     ),
 )
 
 database_page = PageSchema(
     label="数据库", icon="fa fa-database", children=[server_page, query_page]
 )  # type: ignore
+
 config_page = PageSchema(
     url="/configs",
     isDefaultPage=True,
     icon="fa fa-wrench",
     label="配置",
     schema=Page(
         title="配置",
@@ -421,12 +441,12 @@
 )
 header = Flex(
     className="w-full", justify="flex-end", alignItems="flex-end", items=[github_logo]
 )
 
 admin_app = App(
     brandName="L4d2-Server",
-    logo="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png",
+    logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png",
     header=header,
     pages=[{"children": [config_page, database_page]}],
     footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',
 )
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-from amis import ActionType, TableCRUD, TableColumn from amis import
-PageSchema, Switch, InputNumber, InputTag, Action, App from amis import ( Form,
-InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page,
-AmisAPI, Wrapper, ) from amis import LevelEnum, Select, Alert, Tpl, Flex from
-..l4d2_utils.config import NICKNAME logo = Html( html="""
+from amis import ( Action, ActionType, Alert, AmisAPI, App, DisplayModeEnum,
+Flex, Form, Horizontal, Html, InputNumber, InputPassword, InputTag, InputText,
+LevelEnum, Page, PageSchema, Remark, Select, Switch, TableColumn, TableCRUD,
+Tpl, Wrapper, ) from ..l4d2_utils.config import NICKNAME logo = Html( html="""
                                  [l4d2-server]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
 """ ) login_api = AmisAPI( url="/l4d2/api/login", method="post", adaptor=""" if
 (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
@@ -31,16 +30,20 @@
 labelRemark=Remark(shape="circle",
 content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
 ( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
 {web_secret_key}", labelRemark=Remark(shape="circle",
 content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputText
 ( label="å­ä½", name="l4_font", value="${l4_font}", labelRemark=Remark
 (shape="circle", content="æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã"), ),
-Select( label="å¾çé£æ ¼", name="l4_style", value="${l4_style}", source="$
-{l4_styles}", labelRemark=Remark(shape="circle",
+Switch( label="æ¯å¦å¾çåéåæå¡å¨æ¥è¯¢", name="l4_image", value="$
+{l4_image}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
+(shape="circle",
+content="å¼å¯æ¶ï¼ä¼æ¥è¯¢åæå¡å¨ä¼ä½¿ç¨å¾çï¼é¿åé¿ä¿¡æ¯é£æ§"),
+), Select( label="å¾çé£æ ¼", name="l4_style", value="${l4_style}",
+source="${l4_styles}", labelRemark=Remark(shape="circle",
 content="ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼"), ), Switch
 ( label="æ¯å¦ä¼åä¸ä¼ å°å¾", name="l4_only", value="${l4_only}",
 onText="å¼å¯", offText="å³é­", labelRemark=Remark(shape="circle",
 content="å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤"),
 ), Switch( label="æ¯å¦æ¾ç¤ºconnect", name="l4_connect", value="$
 {l4_connect}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
 (shape="circle",
@@ -123,40 +126,40 @@
 content="è¿ç¨æå¡å¨çç»å½å¯ç "), ), ], actions=[ Action
 (label="ä¿å­", level=LevelEnum.success, type="submit"), Action
 (label="éç½®", level=LevelEnum.warning, type="reset"), ], ) query_table =
 TableCRUD( mode="table", title="", syncLocation=False, api="/l4d2/api/
 get_query_contexts", interval=60000, itemActions=[ ActionType.Url
 ( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad", confirmText="å å¥steam://
 connect/" + "${ip}", url="steam://connect/" + "${ip}", # url= "http://"+'$
-{ip}', blank=True, ), ], columns=[ TableColumn(label="æä¸»", name="master",
-searchable=True), TableColumn(label="åç§°", name="name", searchable=True),
-TableColumn(label="å°å¾", name="map_", searchable=True), TableColumn
-(label="ç©å®¶", name="rank_players", searchable=True), TableColumn
-(label="å»¶è¿", name="ping", searchable=True), TableColumn(label="IP å°å",
-name="ip", searchable=True), ], ) server_page = PageSchema( url="/messages",
-icon="fa fa-comment", label="æ¬å°æå¡å¨ç®¡ç", schema=Page
-( title="æ¬å°æå¡å¨ç®¡ç", interval=120000, initApi="/l4d2/api/
-get_l4d2_messages", body=[ Alert( level=LevelEnum.info, className="white-space-
-pre-wrap", body=(f"æ­¤æ°æ®åºè®°å½äº
-{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n" f"Â· åè½ææªå®å"),
-), server_control, server_ditail, ], ), ) query_page = PageSchema( url="/
-contexts", icon="fa fa-comments", label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page
-( title="è¿ç¨æå¡å¨æ¥è¯¢", body=[ Alert( level=LevelEnum.info,
-className="white-space-pre-wrap", body=( f"æ­¤æ°æ®åºè®°å½äº
-{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
+{ip}', blank=True, ), ], columns=[ TableColumn(label="æä¸»", name="tag",
+searchable=True), TableColumn(label="åºå·", name="number", searchable=True),
+TableColumn(label="åç§°", name="name", searchable=True), TableColumn
+(label="å°å¾", name="map_", searchable=True), TableColumn(label="ç©å®¶",
+name="rank_players", searchable=True), TableColumn(label="å»¶è¿", name="ping",
+searchable=True), TableColumn(label="IP å°å", name="ip", searchable=True),
+], ) server_page = PageSchema( url="/messages", icon="fa fa-comment",
+label="æ¬å°æå¡å¨ç®¡ç", schema=Page( title="æ¬å°æå¡å¨ç®¡ç",
+interval=120000, initApi="/l4d2/api/get_l4d2_messages", body=[ Alert
+( level=LevelEnum.info, className="white-space-pre-wrap", body=
+(f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n"
+f"Â· åè½ææªå®å"), ), server_control, server_ditail, ], ), ) query_page
+= PageSchema( url="/contexts", icon="fa fa-comments",
+label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢",
+body=[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
+( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
 f"Â· åè½ææªå®å" ), ), query_table, ], ), ) database_page = PageSchema
 ( label="æ°æ®åº", icon="fa fa-database", children=[server_page, query_page]
 ) # type: ignore config_page = PageSchema( url="/configs", isDefaultPage=True,
 icon="fa fa-wrench", label="éç½®", schema=Page( title="éç½®", initApi="/
 l4d2/api/get_group_list", body=[global_config_form, group_select,
 group_config_form], ), ) l4d2_page = PageSchema( label="æ±çä¹è·¯", icon="fa
 fa-wechat (alias)", children=[config_page, database_page] ) # type: ignore
 github_logo = Tpl( className="w-full", tpl='
 ', ) header = Flex( className="w-full", justify="flex-end", alignItems="flex-
 end", items=[github_logo] ) admin_app = App( brandName="L4d2-Server",
-logo="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/
-main/image/logo.png", header=header, pages=[{"children": [config_page,
-database_page]}], footer='
+logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/
+nonebot_plugin_l4d2_server/main/image/logo.png", header=header, pages=[
+{"children": [config_page, database_page]}], footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
 ', )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/pyproject.toml` & `nonebot_plugin_l4d2_server-0.6.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.6.0"
+version = "0.6.0.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -20,19 +20,18 @@
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = ">=2.2.1"
 nonebot-plugin-htmlrender = "^0.2.0.3"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
-nonebot-plugin-send-anything-anywhere = "0.2.7"
+nonebot-adapter-onebot = "^2.2.3"
 asyncio = ">=3.4.3"
 aiohttp = "^3.8.4"
 jinja2 = ">=3.0.0"
 srctools="^2.3.9"
 bs4 = "0.0.1"
 httpx = ">=0.22.0"
 rcon = "^2.1.0"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0/PKG-INFO` & `nonebot_plugin_l4d2_server-0.6.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.6.0
+Version: 0.6.0.1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -21,17 +21,16 @@
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: jinja2 (>=3.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (==0.2.7)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
@@ -78,18 +77,21 @@
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
 ## 顶置公告
 
-0.6.0更新了适配器，初步实现了v11,v12,kook的适配，以及qq频道的部分适配
+多适配器版本请查看[分支](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/tree/nb_adapter)
 
 文档暂时没时间更新ozr
 
+网页端管理端 `https://{ip}:{port}/l4d2`
+网页用户端 `https://{ip}:{port}/l4d2/user`
+
 ## 安装
 
 以下方法任选其一：
 
         nb plugin install nonebot-plugin-l4d2-server
         pip install nonebot-plugin-l4d2-server
         pipx install nonebot-plugin-l4d2-server
@@ -161,23 +163,21 @@
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 3
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 | 驴头 | 驴头服 | lvt | 4
 | 迷茫 | 迷茫 | 迷茫 | 10
 | 尸鬼 | 尸鬼狂潮 | ❀几❀ | 13
 
-
 ## To do
 
 - [ ] 帮助图片
 - [ ] 网页控制台查看服务器地图
 - [ ] 网页控制台启动和关闭服务器
 - [ ] 网页控制台管理封禁用户
 
-
 ## 其他
 
 - 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 - 如果本插件对你有帮助，不要忘了点个Star~
 - 本项目仅供学习使用，请勿用于商业用途
 - [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0 Summary:
-L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0.1
+Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
 asyncio (>=3.4.3) Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist: bs4
 (==0.0.1) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx (>=0.22.0)
-Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist:
-nonebot-plugin-send-anything-anywhere (==0.2.7) Requires-Dist: nonebot2
-(>=2.0.0,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.4.0,<10.0.0)
-Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0)
-Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
-Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
-(>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
-Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
-Content-Type: text/markdown
+Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
+nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
+patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.4.0,<10.0.0) Requires-Dist:
+python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0) Requires-Dist:
+pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0) Requires-Dist:
+rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-
+Dist: srctools (>=2.3.9,<3.0.0) Project-URL: Repository, https://github.com/
+Agnes4m/nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
-## é¡¶ç½®å¬å
-0.6.0æ´æ°äºééå¨ï¼åæ­¥å®ç°äºv11,v12,kookçééï¼ä»¥åqqé¢éçé¨åéé
-ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin
-install nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx
-install nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
+## é¡¶ç½®å¬å å¤ééå¨çæ¬è¯·æ¥ç[åæ¯](https://github.com/Agnes4m/
+nonebot_plugin_l4d2_server/tree/nb_adapter) ææ¡£ææ¶æ²¡æ¶é´æ´æ°ozr
+ç½é¡µç«¯ç®¡çç«¯ `https://{ip}:{port}/l4d2` ç½é¡µç¨æ·ç«¯ `https://{ip}:
+{port}/l4d2/user` ## å®è£ ä»¥ä¸æ¹æ³ä»»éå¶ä¸ï¼ nb plugin install
+nonebot-plugin-l4d2-server pip install nonebot-plugin-l4d2-server pipx install
+nonebot-plugin-l4d2-server git clone https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server.git ## ä¸»è¦åè½ - æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
 //github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
 l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
 ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml # éç½®æä»¶
```

