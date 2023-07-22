# Comparing `tmp/pls-5.4.0.tar.gz` & `tmp/pls-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pls-5.4.0.tar", max compression
+gzip compressed data, was "pls-6.0.0.tar", max compression
```

## Comparing `pls-5.4.0.tar` & `pls-6.0.0.tar`

### file list

```diff
@@ -1,73 +1,76 @@
--rw-r--r--   0        0        0    35149 2022-02-12 12:47:32.607294 pls-5.4.0/LICENSE
--rw-r--r--   0        0        0     3019 2022-08-11 10:25:09.154177 pls-5.4.0/README.md
--rw-r--r--   0        0        0      858 2022-08-11 15:34:48.103463 pls-5.4.0/pyproject.toml
--rw-r--r--   0        0        0       94 2022-06-03 11:01:41.819668 pls-5.4.0/src/pls/__init__.py
--rw-r--r--   0        0        0        0 2022-02-25 20:29:00.406121 pls-5.4.0/src/pls/config/__init__.py
--rw-r--r--   0        0        0     4842 2022-07-17 20:08:37.459980 pls-5.4.0/src/pls/config/constants.py
--rw-r--r--   0        0        0     3417 2022-07-04 08:24:45.791671 pls-5.4.0/src/pls/config/files.py
--rw-r--r--   0        0        0     1513 2022-03-25 22:12:48.899583 pls-5.4.0/src/pls/config/icons.py
--rw-r--r--   0        0        0     4635 2022-04-06 20:44:41.250029 pls-5.4.0/src/pls/config/prefs.py
--rw-r--r--   0        0        0     3815 2022-07-04 08:19:08.522971 pls-5.4.0/src/pls/config/specs.py
--rw-r--r--   0        0        0        0 2022-02-12 12:47:33.111168 pls-5.4.0/src/pls/data/__init__.py
--rw-r--r--   0        0        0     1052 2022-07-17 20:14:16.803313 pls-5.4.0/src/pls/data/constants.yml
--rw-r--r--   0        0        0      714 2022-07-17 19:53:27.695494 pls-5.4.0/src/pls/data/emoji_icons.yml
--rw-r--r--   0        0        0     1315 2022-07-17 19:53:31.750908 pls-5.4.0/src/pls/data/nerd_icons.yml
--rw-r--r--   0        0        0     2696 2022-07-04 04:57:05.677035 pls-5.4.0/src/pls/data/node_specs.yml
--rw-r--r--   0        0        0      449 2022-04-04 10:10:02.971566 pls-5.4.0/src/pls/data/prefs.yml
--rw-r--r--   0        0        0     8140 2022-04-04 10:18:14.908998 pls-5.4.0/src/pls/data/schema/pls_config.yml
--rw-r--r--   0        0        0      362 2022-02-14 12:05:40.861053 pls-5.4.0/src/pls/data/solarized.yml
--rw-r--r--   0        0        0     1144 2022-07-04 06:35:14.936049 pls-5.4.0/src/pls/data/utils.py
--rw-r--r--   0        0        0        0 2022-02-12 12:47:33.105430 pls-5.4.0/src/pls/enums/__init__.py
--rw-r--r--   0        0        0      391 2022-03-25 21:11:39.701518 pls-5.4.0/src/pls/enums/base.py
--rw-r--r--   0        0        0      482 2022-02-12 12:47:33.106585 pls-5.4.0/src/pls/enums/icon_type.py
--rw-r--r--   0        0        0     2991 2022-07-17 20:09:54.774750 pls-5.4.0/src/pls/enums/node_type.py
--rw-r--r--   0        0        0     1523 2022-03-25 21:11:40.911349 pls-5.4.0/src/pls/enums/unit_system.py
--rw-r--r--   0        0        0     2723 2022-03-27 11:15:14.862535 pls-5.4.0/src/pls/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-12 12:47:33.110524 pls-5.4.0/src/pls/fs/__init__.py
--rw-r--r--   0        0        0     4170 2022-08-11 15:34:37.883205 pls-5.4.0/src/pls/fs/git.py
--rw-r--r--   0        0        0     2261 2022-05-23 15:02:18.824289 pls-5.4.0/src/pls/fs/list.py
--rw-r--r--   0        0        0     6058 2022-04-05 12:27:50.495911 pls-5.4.0/src/pls/fs/stats.py
--rw-r--r--   0        0        0        0 2022-03-19 09:30:43.601860 pls-5.4.0/src/pls/globals/__init__.py
--rw-r--r--   0        0        0      143 2022-04-06 20:44:41.250164 pls-5.4.0/src/pls/globals/args.py
--rw-r--r--   0        0        0      410 2022-04-24 07:59:35.412154 pls-5.4.0/src/pls/globals/console.py
--rw-r--r--   0        0        0     3544 2022-07-04 08:24:45.791837 pls-5.4.0/src/pls/globals/state.py
--rw-r--r--   0        0        0        0 2022-03-25 21:11:41.098788 pls-5.4.0/src/pls/log/__init__.py
--rw-r--r--   0        0        0     1060 2022-03-27 20:20:52.677779 pls-5.4.0/src/pls/log/config.py
--rwxr-xr-x   0        0        0     5001 2022-07-17 20:01:42.110375 pls-5.4.0/src/pls/main.py
--rw-r--r--   0        0        0        0 2022-02-12 12:47:33.107615 pls-5.4.0/src/pls/models/__init__.py
--rw-r--r--   0        0        0     2249 2022-04-07 20:58:03.944476 pls-5.4.0/src/pls/models/base_node.py
--rw-r--r--   0        0        0     1651 2022-04-10 22:59:48.177589 pls-5.4.0/src/pls/models/column_spec.py
--rw-r--r--   0        0        0        0 2022-02-19 08:22:26.288583 pls-5.4.0/src/pls/models/mixins/__init__.py
--rw-r--r--   0        0        0     1646 2022-03-29 09:28:36.835863 pls-5.4.0/src/pls/models/mixins/git.py
--rw-r--r--   0        0        0     1545 2022-04-07 20:58:03.944974 pls-5.4.0/src/pls/models/mixins/imp.py
--rw-r--r--   0        0        0     2473 2022-04-05 12:27:50.461966 pls-5.4.0/src/pls/models/mixins/stat.py
--rw-r--r--   0        0        0     4500 2022-04-11 00:20:02.793256 pls-5.4.0/src/pls/models/mixins/tree.py
--rw-r--r--   0        0        0     2862 2022-04-23 12:29:52.099015 pls-5.4.0/src/pls/models/mixins/type.py
--rw-r--r--   0        0        0     7657 2022-07-17 20:09:54.774809 pls-5.4.0/src/pls/models/node.py
--rw-r--r--   0        0        0     2340 2022-07-04 08:19:08.523140 pls-5.4.0/src/pls/models/node_spec.py
--rw-r--r--   0        0        0        0 2022-02-15 07:24:41.439608 pls-5.4.0/src/pls/output/__init__.py
--rw-r--r--   0        0        0        0 2022-04-10 12:25:23.271011 pls-5.4.0/src/pls/output/columns/__init__.py
--rw-r--r--   0        0        0     1020 2022-04-11 00:20:08.285813 pls-5.4.0/src/pls/output/columns/all_columns.py
--rw-r--r--   0        0        0     1669 2022-04-10 23:01:41.399670 pls-5.4.0/src/pls/output/columns/detail_columns.py
--rw-r--r--   0        0        0     1993 2022-04-10 12:24:05.240171 pls-5.4.0/src/pls/output/columns_printer.py
--rw-r--r--   0        0        0     2333 2022-05-23 15:02:18.824758 pls-5.4.0/src/pls/output/printers.py
--rw-r--r--   0        0        0     1369 2022-03-27 20:32:57.265913 pls-5.4.0/src/pls/output/solarized.py
--rw-r--r--   0        0        0     4179 2022-05-23 14:22:24.546861 pls-5.4.0/src/pls/output/table_printer.py
--rw-r--r--   0        0        0     2413 2022-06-03 11:34:42.818513 pls-5.4.0/src/pls/output/update.py
--rw-r--r--   0        0        0        0 2022-03-29 12:16:25.052032 pls-5.4.0/src/pls/parser/__init__.py
--rw-r--r--   0        0        0     2819 2022-04-03 07:53:06.614770 pls-5.4.0/src/pls/parser/actions.py
--rw-r--r--   0        0        0        0 2022-03-29 12:16:30.800565 pls-5.4.0/src/pls/parser/args/__init__.py
--rw-r--r--   0        0        0     1315 2022-03-29 12:16:25.052281 pls-5.4.0/src/pls/parser/args/dev.py
--rw-r--r--   0        0        0     1295 2022-04-01 19:56:10.306682 pls-5.4.0/src/pls/parser/args/filter.py
--rw-r--r--   0        0        0     1395 2022-04-10 12:26:29.762986 pls-5.4.0/src/pls/parser/args/info.py
--rw-r--r--   0        0        0      641 2022-06-03 11:01:11.386244 pls-5.4.0/src/pls/parser/args/meta.py
--rw-r--r--   0        0        0     1119 2022-07-04 04:56:10.578126 pls-5.4.0/src/pls/parser/args/pos.py
--rw-r--r--   0        0        0     1201 2022-04-01 19:56:19.421452 pls-5.4.0/src/pls/parser/args/pres.py
--rw-r--r--   0        0        0      916 2022-04-10 22:13:27.503004 pls-5.4.0/src/pls/parser/args/sort.py
--rw-r--r--   0        0        0     5935 2022-05-23 15:42:14.389337 pls-5.4.0/src/pls/parser/base.py
--rw-r--r--   0        0        0     1264 2022-06-03 11:01:00.867027 pls-5.4.0/src/pls/parser/parser.py
--rw-r--r--   0        0        0      618 2022-04-03 07:21:52.169968 pls-5.4.0/src/pls/parser/validation.py
--rw-r--r--   0        0        0        0 2022-03-26 22:34:53.745710 pls-5.4.0/src/pls/utils/__init__.py
--rw-r--r--   0        0        0      411 2022-03-29 12:39:35.165674 pls-5.4.0/src/pls/utils/strip_fmt.py
--rw-r--r--   0        0        0     4191 2022-08-11 15:35:29.791093 pls-5.4.0/setup.py
--rw-r--r--   0        0        0     3805 2022-08-11 15:35:29.791311 pls-5.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-16 11:16:40.002261 pls-6.0.0/LICENSE
+-rw-r--r--   0        0        0     3019 2023-07-16 11:16:40.002972 pls-6.0.0/README.md
+-rw-r--r--   0        0        0      879 2023-07-22 01:19:32.435817 pls-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-07-16 11:16:40.020955 pls-6.0.0/src/pls/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.021026 pls-6.0.0/src/pls/config/__init__.py
+-rw-r--r--   0        0        0     5104 2023-07-16 11:16:47.017618 pls-6.0.0/src/pls/config/constants.py
+-rw-r--r--   0        0        0     3490 2023-07-22 01:17:16.808153 pls-6.0.0/src/pls/config/files.py
+-rw-r--r--   0        0        0     1617 2023-07-16 11:16:40.021848 pls-6.0.0/src/pls/config/icons.py
+-rw-r--r--   0        0        0     4739 2023-07-16 11:16:40.021966 pls-6.0.0/src/pls/config/prefs.py
+-rw-r--r--   0        0        0     3919 2023-07-16 11:16:40.022082 pls-6.0.0/src/pls/config/specs.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.022150 pls-6.0.0/src/pls/data/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-16 11:16:40.022437 pls-6.0.0/src/pls/data/constants.yml
+-rw-r--r--   0        0        0      735 2023-07-16 11:16:40.022540 pls-6.0.0/src/pls/data/emoji_icons.yml
+-rw-r--r--   0        0        0     1352 2023-07-16 11:16:47.017809 pls-6.0.0/src/pls/data/nerd_icons.yml
+-rw-r--r--   0        0        0     2731 2023-07-16 11:16:40.022978 pls-6.0.0/src/pls/data/node_specs.yml
+-rw-r--r--   0        0        0      449 2023-07-16 11:16:40.023154 pls-6.0.0/src/pls/data/prefs.yml
+-rw-r--r--   0        0        0     8140 2023-07-16 11:16:40.023295 pls-6.0.0/src/pls/data/schema/pls_config.yml
+-rw-r--r--   0        0        0      362 2023-07-16 11:16:40.023388 pls-6.0.0/src/pls/data/solarized.yml
+-rw-r--r--   0        0        0     1144 2023-07-16 11:16:40.023489 pls-6.0.0/src/pls/data/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.023541 pls-6.0.0/src/pls/enums/__init__.py
+-rw-r--r--   0        0        0      391 2023-07-16 11:16:40.023858 pls-6.0.0/src/pls/enums/base.py
+-rw-r--r--   0        0        0      482 2023-07-16 11:16:40.023951 pls-6.0.0/src/pls/enums/icon_type.py
+-rw-r--r--   0        0        0     1911 2023-07-16 11:16:40.024052 pls-6.0.0/src/pls/enums/node_type.py
+-rw-r--r--   0        0        0     1702 2023-07-16 11:16:40.024156 pls-6.0.0/src/pls/enums/unit_system.py
+-rw-r--r--   0        0        0     2723 2023-07-16 11:16:40.024322 pls-6.0.0/src/pls/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.024389 pls-6.0.0/src/pls/fs/__init__.py
+-rw-r--r--   0        0        0     4218 2023-07-22 01:17:16.808463 pls-6.0.0/src/pls/fs/git.py
+-rw-r--r--   0        0        0     2419 2023-07-22 01:17:16.808760 pls-6.0.0/src/pls/fs/list.py
+-rw-r--r--   0        0        0     5150 2023-07-16 11:16:40.024830 pls-6.0.0/src/pls/fs/stats.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.024886 pls-6.0.0/src/pls/globals/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-16 11:16:40.025009 pls-6.0.0/src/pls/globals/args.py
+-rw-r--r--   0        0        0      501 2023-07-16 11:16:40.025096 pls-6.0.0/src/pls/globals/console.py
+-rw-r--r--   0        0        0     3499 2023-07-16 11:16:40.025203 pls-6.0.0/src/pls/globals/state.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.025255 pls-6.0.0/src/pls/log/__init__.py
+-rw-r--r--   0        0        0     1060 2023-07-16 11:16:40.025369 pls-6.0.0/src/pls/log/config.py
+-rwxr-xr-x   0        0        0     5573 2023-07-17 08:09:30.472634 pls-6.0.0/src/pls/main.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.025774 pls-6.0.0/src/pls/models/__init__.py
+-rw-r--r--   0        0        0     1651 2023-07-16 11:16:40.025888 pls-6.0.0/src/pls/models/column_spec.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.025941 pls-6.0.0/src/pls/models/composables/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-17 08:09:30.472995 pls-6.0.0/src/pls/models/composables/children.py
+-rw-r--r--   0        0        0     1633 2023-07-16 11:16:40.026250 pls-6.0.0/src/pls/models/composables/collapse.py
+-rw-r--r--   0        0        0     1662 2023-07-16 11:16:40.026343 pls-6.0.0/src/pls/models/composables/git.py
+-rw-r--r--   0        0        0     2104 2023-07-16 11:16:40.026439 pls-6.0.0/src/pls/models/composables/imp.py
+-rw-r--r--   0        0        0     1513 2023-07-16 11:16:40.026566 pls-6.0.0/src/pls/models/composables/name.py
+-rw-r--r--   0        0        0     1405 2023-07-17 08:09:30.473115 pls-6.0.0/src/pls/models/composables/spec.py
+-rw-r--r--   0        0        0     2805 2023-07-22 01:17:16.809044 pls-6.0.0/src/pls/models/composables/stat.py
+-rw-r--r--   0        0        0     5853 2023-07-16 11:16:47.018014 pls-6.0.0/src/pls/models/composables/type.py
+-rw-r--r--   0        0        0     1495 2023-07-16 11:16:40.027170 pls-6.0.0/src/pls/models/format_rules.py
+-rw-r--r--   0        0        0     6120 2023-07-22 01:17:16.809320 pls-6.0.0/src/pls/models/node.py
+-rw-r--r--   0        0        0     2307 2023-07-16 11:16:47.018350 pls-6.0.0/src/pls/models/node_spec.py
+-rw-r--r--   0        0        0     3922 2023-07-17 08:09:30.473542 pls-6.0.0/src/pls/models/tree.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.027877 pls-6.0.0/src/pls/output/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.027938 pls-6.0.0/src/pls/output/columns/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-16 11:16:40.028049 pls-6.0.0/src/pls/output/columns/all_columns.py
+-rw-r--r--   0        0        0     1669 2023-07-16 11:16:40.028152 pls-6.0.0/src/pls/output/columns/detail_columns.py
+-rw-r--r--   0        0        0     1993 2023-07-16 11:16:40.028260 pls-6.0.0/src/pls/output/columns_printer.py
+-rw-r--r--   0        0        0     2333 2023-07-16 11:16:40.028352 pls-6.0.0/src/pls/output/printers.py
+-rw-r--r--   0        0        0     1369 2023-07-16 11:16:40.028439 pls-6.0.0/src/pls/output/solarized.py
+-rw-r--r--   0        0        0     3673 2023-07-16 11:16:40.028612 pls-6.0.0/src/pls/output/table_printer.py
+-rw-r--r--   0        0        0     2523 2023-07-16 11:16:40.028716 pls-6.0.0/src/pls/output/update.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.028771 pls-6.0.0/src/pls/parser/__init__.py
+-rw-r--r--   0        0        0     3804 2023-07-16 11:16:40.028881 pls-6.0.0/src/pls/parser/actions.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.028946 pls-6.0.0/src/pls/parser/args/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-16 11:16:40.029071 pls-6.0.0/src/pls/parser/args/dev.py
+-rw-r--r--   0        0        0     1213 2023-07-16 11:16:40.029179 pls-6.0.0/src/pls/parser/args/filter.py
+-rw-r--r--   0        0        0     1341 2023-07-16 11:16:40.029282 pls-6.0.0/src/pls/parser/args/info.py
+-rw-r--r--   0        0        0      576 2023-07-16 11:16:40.029374 pls-6.0.0/src/pls/parser/args/meta.py
+-rw-r--r--   0        0        0     1119 2023-07-16 11:16:40.029468 pls-6.0.0/src/pls/parser/args/pos.py
+-rw-r--r--   0        0        0     1292 2023-07-16 11:16:40.029565 pls-6.0.0/src/pls/parser/args/pres.py
+-rw-r--r--   0        0        0      916 2023-07-16 11:16:40.029665 pls-6.0.0/src/pls/parser/args/sort.py
+-rw-r--r--   0        0        0     5933 2023-07-16 11:16:47.018529 pls-6.0.0/src/pls/parser/base.py
+-rw-r--r--   0        0        0     1347 2023-07-16 11:16:40.029968 pls-6.0.0/src/pls/parser/parser.py
+-rw-r--r--   0        0        0     1275 2023-07-16 11:16:40.030059 pls-6.0.0/src/pls/parser/validation.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:16:40.030118 pls-6.0.0/src/pls/utils/__init__.py
+-rw-r--r--   0        0        0      411 2023-07-16 11:16:40.030229 pls-6.0.0/src/pls/utils/strip_fmt.py
+-rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 pls-6.0.0/PKG-INFO
```

### Comparing `pls-5.4.0/LICENSE` & `pls-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/README.md` & `pls-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/pyproject.toml` & `pls-6.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pls"
 description = "`pls` is a prettier and powerful `ls` for the pros."
-version = "5.4.0"
+version = "6.0.0"
 
 authors = ["Dhruv Bhanushali"]
 
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 homepage = "https://dhruvkb.github.io/pls"
@@ -19,22 +19,23 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^6.0"
 rich = "^12.5.1"
 requests = "^2.27.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.20.0"
+pre-commit = "^3.3.3"
 ipython = "^8.4.0"
 pytest = "^7.1.2"
 pytest-lazy-fixture = "^0.6.3"
 freezegun = "^1.2.1"
 jsonschema = "^4.9.0"
 requests = "^2.27.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
+GitPython = "^3.1.27"
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pls-5.4.0/src/pls/config/constants.py` & `pls-6.0.0/src/pls/config/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 Do not import variables from this module, always import the module directly and use its
 variables with a dot ``.`` notation.
 """
 
 from __future__ import annotations
 
+import copy
+from functools import lru_cache
 from pathlib import Path
 from typing import Any, Optional
 
 from pls.data.utils import load_yml_file
 from pls.exceptions import ConfigException, ConstException
 
 
 class NestedDict(dict):
     """
     Extends ``dict`` to add support for deep-merge and lookup functionality.
     """
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.lookup = lru_cache(maxsize=None)(self._lookup)
+
     @staticmethod
     def _deep_merge(
         a: dict, b: dict, overwrite: bool = False, path: Optional[list[str]] = None
     ):
         """
         Deep-merge dict ``b`` into dict ``a``. This function mutates ``a`` as a side
         effect and therefore does not return any value. Nested lists are union-ed and
@@ -60,15 +67,15 @@
 
         :param other: the incoming dictionary, left unchanged
         :param overwrite: whether to write the conflicting keys with value in ``other``
         """
 
         self._deep_merge(self, other, overwrite)
 
-    def lookup(self, *path: str, default: Any = None) -> Any:
+    def _lookup(self, *path: str, default: Any = "~UNSET~") -> Any:
         """
         Lookup the given path in the dictionary by traversing the fragments. This
         assumes that the dictionary contains only contains plain data types. Use
         integers for looking up values in lists. Note that a lookup resulting in
         ``None`` is considered a passing lookup and will not return the default value.
 
         :param path: the path to the data point inside the dictionary
@@ -80,22 +87,21 @@
         obj = self
 
         for fragment in path:
             try:
                 if (isinstance(obj, list)) or isinstance(obj, dict):
                     obj = obj[fragment]
                     continue
-                else:
-                    raise ConstException
+                raise ConstException
             except (KeyError, IndexError, TypeError, ConstException) as exc:
                 # ``KeyError`` when ``fragment`` not in ``obj`` dict
                 # ``IndexError`` when ``fragment`` not in ``obj`` list
                 # ``TypeError`` when ``fragment`` not ``int`` in ``obj`` list
                 # ``ConstException`` when traversal not possible
-                if default is not None:
+                if default != "~UNSET~":
                     return default
 
                 path_str = ".".join([str(fragment) for fragment in path])
                 raise ConstException(f"Cannot find `{path_str}` in dict.") from exc
 
         return obj
 
@@ -108,15 +114,16 @@
     :param conf_paths: the list of config files from which to import constants
     :return: the mapping of icon name to icon glyph
     """
 
     consts: NestedDict = NestedDict()
 
     for conf_path in reversed(conf_paths):
-        conf = load_yml_file(conf_path)
+        # Use a copy to prevent ``load_yml_file`` cache from being polluted.
+        conf = copy.deepcopy(load_yml_file(conf_path))
 
         consts_val = conf.get("constants", {})
         if not consts_val:
             continue
         if not isinstance(consts_val, dict):
             raise ConfigException("[italic]`constants`[/] must be a dictionary.")
         consts.deep_merge(consts_val, overwrite=True)
```

### Comparing `pls-5.4.0/src/pls/config/files.py` & `pls-6.0.0/src/pls/config/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,18 @@
     """
     Check if the given path points to an existing file.
 
     :param path: the path to check for validity
     :return: ``True`` if the path is an existing file, ``False`` otherwise
     """
 
-    is_valid = path.exists() and path.is_file()
+    try:
+        is_valid = path.exists() and path.is_file()
+    except (OSError, PermissionError):
+        return False
     logger.debug(f'{path}: {"valid" if is_valid else "invalid"}')
     return is_valid
 
 
 def get_cwd_conf(curr_dir: Path) -> Optional[Path]:
     """
     Get the path to the ``pls`` config in the current directory itself.
```

### Comparing `pls-5.4.0/src/pls/config/icons.py` & `pls-6.0.0/src/pls/config/icons.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Do not import variables from this module, always import the module directly and use its
 variables with a dot ``.`` notation.
 """
 
 from __future__ import annotations
 
+import copy
 from pathlib import Path
 
 from pls.data.utils import load_yml_file
 from pls.exceptions import ConfigException
 
 
 def get_icons(conf_paths: list[Path]) -> tuple[dict[str, str], dict[str, str]]:
@@ -21,15 +22,16 @@
     :return: the mapping of icon name to icon glyph
     """
 
     nerd: dict[str, str] = {}
     emoji: dict[str, str] = {}
 
     for conf_path in reversed(conf_paths):
-        conf = load_yml_file(conf_path)
+        # Use a copy to prevent ``load_yml_file`` cache from being polluted.
+        conf = copy.deepcopy(load_yml_file(conf_path))
 
         nerd_val = conf.get("nerd_icons", {})
         if nerd_val:
             if not isinstance(nerd_val, dict):
                 raise ConfigException("[italic]`nerd_icons`[/] must be a dictionary.")
             nerd.update(nerd_val)
```

### Comparing `pls-5.4.0/src/pls/config/prefs.py` & `pls-6.0.0/src/pls/config/prefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This module must be synchronised with ``pls.args`` due to the overlapping nature of
 CLI args and config-based preferences.
 """
 
 from __future__ import annotations
 
 import argparse
+import copy
 import logging
 import re
 from enum import Enum
 from pathlib import Path
 from typing import Type, Union
 
 from pls.data.utils import load_yml_file
@@ -124,15 +125,16 @@
     """
 
     preferences: dict = {}
     if not isinstance(conf_paths, list):
         conf_paths = [conf_paths]
 
     for conf_path in reversed(conf_paths):
-        conf = load_yml_file(conf_path)
+        # Use a copy to prevent ``load_yml_file`` cache from being polluted.
+        conf = copy.deepcopy(load_yml_file(conf_path))
 
         pref_val = conf.get("prefs", {})
         if not pref_val:
             continue
         if not isinstance(pref_val, dict):
             raise ConfigException("[italic]`prefs`[/] must be a dictionary.")
         preferences.update(pref_val)
```

### Comparing `pls-5.4.0/src/pls/config/specs.py` & `pls-6.0.0/src/pls/config/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Do not import variables from this module, always import the module directly and use its
 variables with a dot ``.`` notation.
 """
 
 from __future__ import annotations
 
+import copy
 import logging
 from pathlib import Path
 
 from pls.data.utils import load_yml_file
 from pls.exceptions import SpecException
 from pls.models.node_spec import NodeSpec
 
@@ -99,15 +100,16 @@
     :param conf_paths: the list of config files from which to import spec POPOs
     :return: the list of all node specs for all languages
     """
 
     entries = []
 
     for conf_path in conf_paths:
-        conf = load_yml_file(conf_path)
+        # Use a copy to prevent ``load_yml_file`` cache from being polluted.
+        conf = copy.deepcopy(load_yml_file(conf_path))
         entries.extend(conf.get("node_specs", []))
 
     return [NodeSpec(**spec) for entry in entries for spec in massage_specs(entry)]
 
 
 node_specs: list[NodeSpec]
 """the list of all node specs for all types of nodes"""
```

### Comparing `pls-5.4.0/src/pls/data/emoji_icons.yml` & `pls-6.0.0/src/pls/data/emoji_icons.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   audio:      "🔈"
   broom:      "🧹"
   config:     "⚙️"
   css:        "🎨"
   docker:     "🐳"
   folder:     "📁"
   git:        "⏪"
+  github:     "🐙"
   html:       "🔗"
   image:      "🖼"
   javascript: "🟨"
   json:       "🤝"
   license:    "⚖️"
   lock:       "🔒"
   markdown:   "📄"
```

### Comparing `pls-5.4.0/src/pls/data/node_specs.yml` & `pls-6.0.0/src/pls/data/node_specs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
   - name: .DS_Store
     icon: apple
     importance: -2
 
   - name: .gitignore
     icon: git
+  - name: .github
+    icon: github
 
   - name: [justfile, Makefile, Rakefile]
     icon: runner
 
   - name: [pyproject.toml, Pipfile, setup.py, setup.cfg]
     icon: package
   - name: [poetry.lock, Pipfile.lock]
```

### Comparing `pls-5.4.0/src/pls/data/schema/pls_config.yml` & `pls-6.0.0/src/pls/data/schema/pls_config.yml`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/data/utils.py` & `pls-6.0.0/src/pls/data/utils.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/enums/unit_system.py` & `pls-6.0.0/src/pls/enums/unit_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 from __future__ import annotations
 
 import logging
 from enum import auto
+from functools import cached_property
 
 from pls.enums.base import AutoEnum
 
 
 logger = logging.getLogger(__name__)
 
 
 class UnitSystem(AutoEnum):
     """
-    Bytes can be converted to higher units in two ways:
-
-    - the decimal system where powers of 10 (factor: 10^3) are used
-    - the binary system where powers of 2 (factor: 2^10) are used
-    - no system where higher units are not used
-
-    This enum lists these possibilities.
-    """
-
-    BINARY = auto()
-    DECIMAL = auto()
-    NONE = auto()
-
-
-def get_base_and_pad_and_units(us: UnitSystem) -> tuple[int, int, list[str]]:
-    """
-    Get the base factor i.e. the ratio between any two successive orders of
-    magnitude and the units corresponding to each multiplication of the base
-    factor.
-
-    :param us: the unit system in use
-    :return: the base factor and the list of units
+    This enum lists the different unit systems in which measurements can be represented,
+    also including an option to not use any unit system at all.
     """
 
-    logger.debug(f"Unit system: {us}")
-    units = [
-        "K",  # kibi | kilo
-        "M",  # mebi | mega
-        "G",  # gibi | giga
-        "T",  # tebi | tera
-        "P",  # pebi | peta
-        "E",  # exbi | exa
-        "Z",  # zebi | zetta
-        "Y",  # yobi | yotta
-    ]
-
-    if us == UnitSystem.DECIMAL:
-        base = pow(10, 3)
-        pad = 2  # units will be 2 chars e.g. KB, GB
-        units = ["", *units]
-    else:  # us == UnitSystem.BINARY (default)
-        base = pow(2, 10)
-        pad = 3  # units will be 3 chars e.g. KiB, GiB
-        units = ["", *map(lambda i: f"{i}i", units)]
-    return base, pad, units
+    BINARY = auto()  # powers of 2 (steps of 2^10) are used
+    DECIMAL = auto()  # powers of 10 (steps of 10^3) are used
+    NONE = auto()  # no higher units
+
+    @cached_property
+    def base_pad_units(self) -> tuple[int, int, list[str]]:
+        """
+        Get the base factor i.e. the ratio between any two successive orders of
+        magnitude and the units corresponding to each multiplication of the base
+        factor.
+
+        :return: the base factor, length of each unit string and the list of units
+        """
+
+        if self == UnitSystem.NONE:
+            return 1, 0, [""]
+
+        logger.debug(f"Unit system: {self}")
+        units = [
+            "K",  # kibi | kilo
+            "M",  # mebi | mega
+            "G",  # gibi | giga
+            "T",  # tebi | tera
+            "P",  # pebi | peta
+            "E",  # exbi | exa
+            "Z",  # zebi | zetta
+            "Y",  # yobi | yotta
+        ]
+
+        if self == UnitSystem.DECIMAL:
+            base = pow(10, 3)
+            pad = 2  # units will be 2 chars e.g. KB, GB
+            units = ["", *units]
+        else:  # self == UnitSystem.BINARY (default)
+            base = pow(2, 10)
+            pad = 3  # units will be 3 chars e.g. KiB, GiB
+            units = ["", *map(lambda i: f"{i}i", units)]
+        return base, pad, units
```

### Comparing `pls-5.4.0/src/pls/exceptions.py` & `pls-6.0.0/src/pls/exceptions.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/fs/git.py` & `pls-6.0.0/src/pls/fs/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 
-def formatted_status(status: str) -> str:
+def formatted_status(status: Optional[str]) -> str:
     """
     Get the given Git status formatted using Rich console markup. Expects the
     two-letter Git status as returned by git-status with the ``--porcelain``
     flag.
 
     :param status: the status to format
     :return: the formatted Git status
     """
 
-    if status == "  ":
-        return status
+    if status is None:
+        return "  "
 
     format_map: dict[str, str] = {
         "D": "red",  # deleted
         "M": "yellow",  # modified
         "R": "yellow",  # renamed
         "A": "green",  # added
         "!": "dim",  # ignored
@@ -72,15 +72,15 @@
     try:
         proc = exec_git(
             ["rev-parse", "--show-toplevel"],
             cwd=working_dir,
         )
         root_path = Path(proc.stdout.rstrip())
         return root_path
-    except (subprocess.CalledProcessError, FileNotFoundError):
+    except (subprocess.CalledProcessError, FileNotFoundError, PermissionError):
         return None
 
 
 def _split_git_output(stdout: str) -> list[str]:
     """
     Split the output of Git status with the ``--porcelain`` and ``-z`` flags. The
     NUL character ``\0`` is used as the separator. Renamed files need to be handled
@@ -104,44 +104,44 @@
 
 
 def get_git_statuses(git_root: Path) -> dict[Path, str]:
     """
     Identify the Git statuses for all files in the working directory. To get the
     Git statues, this uses following two commands::
 
-        git status --porcelain=1 -z --untracked-files --ignored
-        git status --porcelain=1 -z --untracked-files=normal --ignored=matching
+        git status --porcelain -z --untracked-files
+        git status --porcelain -z --untracked-files=normal --ignored=matching
 
     Refer to the `git-status command documentation
     <https://git-scm.com/docs/git-status>`_ for more info.
 
     :param git_root: the root directory of the Git repository
     :return: the mapping of paths to their Git statues
     """
 
     status_map: dict[Path, str] = {}
 
     status_lines: set[str] = set()
     try:
-        status_args = ["status", "--porcelain=1", "-z"]
+        status_args = ["status", "--porcelain", "-z"]
 
         proc = exec_git(
             [*status_args, "--untracked-files"],
             cwd=git_root,
         )
         if proc.stdout:
             status_lines.update(_split_git_output(proc.stdout.rstrip()))
 
         proc = exec_git(
-            [*status_args, "--untracked-files=normal"],
+            [*status_args, "--untracked-files=normal", "--ignored=matching"],
             cwd=git_root,
         )
         if proc.stdout:
             status_lines.update(_split_git_output(proc.stdout.rstrip()))
-    except (subprocess.CalledProcessError, FileNotFoundError):
+    except (subprocess.CalledProcessError, FileNotFoundError, PermissionError):
         return status_map
 
     for line in status_lines:
         status = line[0:2]
         path = Path(line[3:].strip())
 
         status_map[path] = status
```

### Comparing `pls-5.4.0/src/pls/fs/list.py` & `pls-6.0.0/src/pls/fs/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,37 +42,41 @@
     Get a list of all directories and files in the given directory.
 
     :return: the list of directories and files inside the given directory
     """
 
     if arg_path.is_dir():
         parent_path = arg_path
-        all_nodes = os.listdir(arg_path)
+        try:
+            all_nodes = os.listdir(arg_path)
+        except (OSError, PermissionError):
+            console.console.print(
+                f"Permission denied for [repr.path]{arg_path}[/].",
+                highlight=False,
+            )
+            return {}, []
     else:
         parent_path = arg_path.parent
         all_nodes = [arg_path.name]
 
-    node_map = {}
-    node_list = []
-
     if not all_nodes:
         console.console.print(
             f"There are no files or folders in [repr.path]{arg_path}[/].",
             highlight=False,
         )
-    else:
-        node_map = {
-            node: Node(name=node, path=parent_path.joinpath(node))
-            for node in all_nodes
-            if passes_name_filters(node)
-        }
-        node_list = list(node_map.values())
+        return {}, []
 
-        sort_fields = args.args.sort
-        for field in reversed(sort_fields):
-            item = field.rstrip("-")
-            node_list.sort(
-                key=lambda node: node.sort_keys[item],
-                reverse=field.endswith("-"),
-            )
+    node_map = {
+        node: Node(name=node, path=parent_path.joinpath(node))
+        for node in all_nodes
+        if passes_name_filters(node)
+    }
+    node_list = list(node_map.values())
+    sort_fields = args.args.sort
+    for field in reversed(sort_fields):
+        item = field.rstrip("-")
+        node_list.sort(
+            key=lambda node: node.sort_keys[item],
+            reverse=field.endswith("-"),
+        )
 
     return node_map, node_list
```

### Comparing `pls-5.4.0/src/pls/fs/stats.py` & `pls-6.0.0/src/pls/fs/stats.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,202 +1,162 @@
 from __future__ import annotations
 
 import datetime
 import logging
-import os
-from itertools import cycle
-from stat import S_ISDIR
-from typing import Literal, Optional
-
-from pls.enums.unit_system import UnitSystem, get_base_and_pad_and_units
+from functools import lru_cache
+from stat import filemode
+from typing import Optional
+
+from pls.config import constants
+from pls.enums.node_type import NodeType
+from pls.enums.unit_system import UnitSystem
 from pls.globals import args, state
+from pls.models.format_rules import FormatRules
 
 
 logger = logging.getLogger(__name__)
 
 
-def _get_format_pair(rules: list[str]) -> tuple[str, str]:
-    """
-    Get the format pair to mark up the console output for the given rules.
-
-    :param rules: the set of formatting directives to apply on the text
-    :return: the pair of format strings to place on either side of the text
-    """
-
-    if not rules:
-        return "", ""
-    left = " ".join(rules)
-    return f"[{left}]", "[/]"
-
-
-def get_formatted_links(stat: os.stat_result) -> str:
+@lru_cache(maxsize=None)
+def get_formatted_links(node_type: NodeType, st_nlink: int) -> str:
     """
     Get the number of hard links pointing to the file. This is usually higher
     than 1 for directories (as all files and folders within in it counted) but
     usually exactly 1 for files.
 
-    :param stat: the stat results of the node
+    :param node_type: the type of the node
+    :param st_nlink: the number of links retrieved from the ``stat`` call
     :return: the number of links of a file
     """
 
-    st_nlink = stat.st_nlink
-
     nlink = str(st_nlink)
-    if not S_ISDIR(stat.st_mode) and st_nlink > 1:
+    if node_type != NodeType.DIR and st_nlink > 1:
         nlink = f"[yellow]{nlink}[/]"
     return nlink
 
 
-def get_formatted_perms(stat: os.stat_result) -> str:
+@lru_cache(maxsize=None)
+def get_formatted_perms(st_mode: int) -> str:
     """
     Get the permission text for the node in the form of a triplet of 'rwx'
     strings. Uses ``st_mode`` from the stat results.
 
-    :param stat: the stat results of the node
+    :param st_mode: the file mode retrieved from the ``stat`` call
     :return: the text to render as the permissions of the node
     """
 
-    st_mode = stat.st_mode
+    perm = filemode(st_mode)[1:]  # drop the first letter, i.e. type char
+    perm = f"{perm[:3]} {perm[3:6]} {perm[6:]}"
 
-    perms = ["r", "w", "x"]
-    specials = ["s", "s", "t"]
-    color_map = {
-        "r": "yellow",
-        "w": "red",
-        "x": "green",
-        "t": "magenta",
-        "s": "magenta",
-    }
-    perm_sets: list[list[str]] = [["-" for _ in range(3)] for _ in range(3)]
-
-    text_rep = format(st_mode, "012b")[-12:]
-
-    for index, (bit, perm) in enumerate(zip(text_rep[3:], cycle(perms))):
-        if int(bit):
-            perm_sets[int(index / 3)][index % 3] = perm
-    for index, (bit, spl) in enumerate(zip(text_rep[:3], specials)):
-        if int(bit):
-            perm_sets[index][2] = spl if perm_sets[index][2] == "x" else spl.upper()
-
-    return " ".join(
-        "".join(
-            f"[{color}]{perm}[/]"
-            if (color := color_map.get(perm.lower(), ""))
-            else perm
-            for perm in perm_set
-        )
-        for perm_set in perm_sets
-    )
+    formatted_perm = ""
+    for char in perm:
+        color = constants.constants.lookup("permission_styles", char, default="dim")
+        formatted_perm += f"[{color}]{char}[/]"
 
+    return formatted_perm
 
-def get_formatted_user(stat: os.stat_result) -> Optional[str]:
+
+@lru_cache(maxsize=None)
+def get_formatted_user(st_uid: int) -> Optional[str]:
     """
     Get the name of the user that owns the node. This requires a ``passwd``
     lookup for the user ID found in the node stats. Uses ``st_uid`` from the
     stat results.
 
-    :param stat: the stat results of the node
+    :param st_uid: the user ID retrieved from the ``stat`` call
     :return: the name of the user who owns the node, ``None`` on Windows
     """
 
     try:
         from pwd import getpwuid
 
-        uid = stat.st_uid
-        format_rules = []
+        format_rules = FormatRules()
         try:
-            pw_name = getpwuid(stat.st_uid).pw_name
+            pw_name = getpwuid(st_uid).pw_name
         except KeyError:  # user does not exist anymore
-            pw_name = str(uid)
+            pw_name = str(st_uid)
             format_rules.append("red")
 
-        if uid != state.state.uid:
+        if st_uid != state.state.uid:
             format_rules.append("dim")
 
-        left, right = _get_format_pair(format_rules)
-        return f"{left}{pw_name}{right}"
+        return format_rules.format_text(pw_name)
     except ModuleNotFoundError:  # on non-POSIX systems like Windows
         return None
 
 
-def get_formatted_group(stat: os.stat_result) -> Optional[str]:
+@lru_cache(maxsize=None)
+def get_formatted_group(st_gid: int) -> Optional[str]:
     """
     Get the name of the group that owns the node. This requires a group database
     lookup for the group ID found in the node stats. Uses ``st_gid`` from the
     stat results.
 
-    :param stat: the stat results of the node
+    :param st_gid: the group ID retrieved from the ``stat`` call
     :return: the name of the group that owns the node, ``None`` on Windows
     """
 
     try:
         from grp import getgrgid
 
-        gid = stat.st_gid
-        format_rules = []
+        format_rules = FormatRules()
         try:
-            gr_name = getgrgid(stat.st_gid).gr_name
+            gr_name = getgrgid(st_gid).gr_name
         except KeyError:  # group does not exist anymore
-            gr_name = str(gid)
+            gr_name = str(st_gid)
             format_rules.append("red")
 
-        if gid not in state.state.gids:
+        if st_gid not in state.state.gids:
             format_rules.append("dim")
 
-        left, right = _get_format_pair(format_rules)
-        return f"{left}{gr_name}{right}"
+        return format_rules.format_text(gr_name)
     except ModuleNotFoundError:  # on non-POSIX systems like Windows
         return None
 
 
-def get_formatted_size(stat: os.stat_result) -> str:
+def get_formatted_size(node_type: NodeType, st_size: int) -> str:
     """
     Get the human-readable size of the node in the form of a number followed by
     a compound unit of a byte. Uses ``st_size`` from the stat results.
 
-    :param stat: the stat results of the node
+    :param node_type: the type of the node
+    :param st_size: the size of the file retrieved from the ``stat`` call
     :return: the size of the node as a human-readable value
     """
 
-    st_size = stat.st_size
-
-    if S_ISDIR(stat.st_mode):
+    if node_type == NodeType.DIR:
         return "[dim]-[/dim]"
 
     if args.args.units == UnitSystem.NONE:
         return f"{st_size}[dim]B[/]"
 
-    base, pad, units = get_base_and_pad_and_units(args.args.units)
+    unit_system = args.args.units or UnitSystem.BINARY
+    base, pad, units = unit_system.base_pad_units
     logger.debug(f"Base: {base}")
     logger.debug(f"Pad: {pad}")
     logger.debug(f"Units: {units}")
     for index, unit in reversed(list(enumerate(units))):
         order_of_magnitude = base**index
         if st_size >= order_of_magnitude:
             magnitude = round(st_size / order_of_magnitude)  # Pop! Pop!
             unit = f"{unit}B".rjust(pad, " ")
 
             return f"{magnitude}[dim]{unit}[/]"
     return f"{st_size}  [dim]B[/]"
 
 
-def get_formatted_time(
-    stat: os.stat_result,
-    attr_name: Literal["st_birthtime", "st_ctime", "st_mtime", "st_atime"],
-) -> str:
+def get_formatted_time(st_time: Optional[int]) -> str:
     """
     Get the given UNIX timestamp as a formatted human/machine-readable date time
     value. The formatting can be controlled via CLI arguments. The name of the
     stat result attribute to use is passed via argument.
 
-    :param stat: the stat results of the node
-    :param attr_name: the name of the UNIX timestamp attribute to use
+    :param st_time: the timestamp retrieved from the ``stat`` call
     :return: the readable date time value for the timestamp
     """
 
-    st_time = getattr(stat, attr_name, None)
     if st_time is None:
         return ""
 
     dt = datetime.datetime.fromtimestamp(st_time)
     fmt = args.args.time_fmt
     return dt.strftime(fmt)
```

### Comparing `pls-5.4.0/src/pls/globals/state.py` & `pls-6.0.0/src/pls/globals/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,13 +115,12 @@
 
         :param node: the file or directory being listed
         """
 
         directory = node if node.is_dir() else node.parent
         self.git_root = get_git_root(directory)
         if self.git_root is not None:
-            assert self.git_root is not None
             self.git_status_map = get_git_statuses(self.git_root)
 
 
 state: State
 """the global state of the application"""
```

### Comparing `pls-5.4.0/src/pls/log/config.py` & `pls-6.0.0/src/pls/log/config.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/main.py` & `pls-6.0.0/src/pls/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pls.config import constants, icons, prefs, specs
 from pls.config.files import find_configs
 from pls.data.utils import internal_yml_path
 from pls.fs.list import read_input
 from pls.globals import args, console, state
 from pls.log.config import configure_log_level
 from pls.output.printers import BasePrinter
-from pls.output.update import check_update
 from pls.parser.parser import parser
 from pls.parser.validation import validate_args
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -101,32 +100,60 @@
             *conf_files,
             internal_yml_path("node_specs.yml"),
         ]
     )
     logger.debug(f"Node specs count: {len(specs.node_specs)}")
 
 
+def treerender(node, child_list, show_header: bool):
+    """
+    Required subprocess to populate and render a Live Tree output
+    """
+
+    from rich.live import Live
+
+    from pls.output.table_printer import TablePrinter
+
+    printer = TablePrinter(node, child_list)
+
+    with Live(
+        printer.table,
+        vertical_overflow="visible",
+        refresh_per_second=20,
+    ):
+
+        def populate_callback(_):
+            printer.tabulate_node(_)
+
+        for child in child_list:
+            child.populate_tree(specs.node_specs, populate_callback=populate_callback)
+
+
 def main_unit(node: Path, show_header: bool = False):
     """
     This function is the job of main, extracted outside the loop.
 
     :param node: the node being described in this iteration
     :param show_header: whether to show the name of the working node before the output
     """
 
     child_map, child_list = read_input(node)
 
     # If there are no children in node, move on.
     if not child_list:
         return
 
+    if args.args.tree:
+        return treerender(node=node, child_list=child_list, show_header=show_header)
+
     for child in child_list:
-        child.match_specs(specs.node_specs)
+        child.spec_comp.match(specs.node_specs)
+
         if args.args.collapse:
-            child.find_main(child_map)
+            child.collapse_comp.find_main(child_map)
     if args.args.collapse:
         for child in child_list:
             if child.is_sub:
                 continue
             child.set_sub_pre_shapes()
 
     PrinterClass: Type[BasePrinter]
@@ -160,17 +187,14 @@
         node_specific_init(node, cli_prefs)
 
         main_unit(node, show_header)
 
         if index != node_counts - 1:
             console.console.print()  # Separate outputs using blank lines.
 
-    if not (os.getenv("PLS_NO_UPDATE_CHECK") or os.getenv("CI")):
-        check_update()
-
 
 def dev():
     os.environ.setdefault("PLS_LOG_LEVEL", "DEBUG")  # Show detailed logs
 
     main()
```

### Comparing `pls-5.4.0/src/pls/models/base_node.py` & `pls-6.0.0/src/pls/models/composables/spec.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,41 @@
 from __future__ import annotations
 
-from functools import cached_property
 from typing import TYPE_CHECKING
 
-from rich.markup import escape
+from pls.models.node_spec import NodeSpec
 
 
 if TYPE_CHECKING:
-    from pathlib import Path
     from typing import Any
 
-    from pls.models.node_spec import NodeSpec
+    from pls.models.node import Node
 
 
-class BaseNode:
+class SpecComp:
     """
-    Acts as the final node in the MRO for the ``__init__`` calls.
+    Adds functionality related to matching and extracting information from the specs.
     """
 
-    def __init__(self, name: str, path: Path):
-        self.name = escape(name)
-        self.path = path
+    def __init__(self, node: Node):
+        self.node = node
 
-        self.specs: list[NodeSpec] = []  # matched in ``match_specs``
+        self.specs: list[NodeSpec] = []  # matched in ``match``
 
-    @cached_property
-    def pure_name(self) -> str:
-        """the name of the node with the leading dot stripped"""
-
-        if self.name.startswith("."):
-            return self.name.replace(".", "", 1)
-        else:
-            return self.name
-
-    @cached_property
-    def canonical_name(self) -> str:
-        """the case-normalised pure name of the node"""
-
-        return self.pure_name.lower()
-
-    @cached_property
-    def extension(self) -> str:
-        """the extension of the node, i.e. the portion after the last dot"""
-
-        return self.name.split(".")[-1] if "." in self.name else ""
-
-    @property
-    def is_visible(self) -> bool:
-        """whether the node deserves to be rendered to the screen"""
-
-        return True
-
-    def match_specs(self, specs: list[NodeSpec]):
+    def match(self, specs: list[NodeSpec]):
         """
         Find all spec matching this node from a list of all possible specs and
         store them in the ``specs`` attribute.
 
         :param specs: the list of all specs
         """
 
-        self.specs = [spec for spec in specs if spec.match(self)]
+        self.specs = [spec for spec in specs if spec.match(self.node)]
 
-    def spec_attr(self, attr: str, coalesce: bool = False) -> Any:
+    def attr(self, attr: str, coalesce: bool = False) -> Any:
         """
         Get the requested attribute from the first matching spec to provide it.
 
         :param attr: the requested attribute
         :param coalesce: whether to group attrs from all specs and return a list
         :return: the value of the attribute if found, ``None`` otherwise
         """
```

### Comparing `pls-5.4.0/src/pls/models/column_spec.py` & `pls-6.0.0/src/pls/models/column_spec.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/models/mixins/git.py` & `pls-6.0.0/src/pls/models/composables/git.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 from pls.fs.git import formatted_status
 from pls.globals import state
-from pls.models.base_node import BaseNode
+from pls.models.format_rules import FormatRules
 
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Optional
 
+    from pls.models.node import Node
 
-class GitMixin(BaseNode):
+
+class GitComp:
     """
-    Adds functionality related to Git status for objects that are Git-tracked.
+    Adds functionality related to the Git status for nodes that are Git tracked. This
+    only applies to files as folders cannot be Git tracked.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, node: Node):
+        self.node = node
 
         self.path_wrt_git: Optional[Path] = None
-        self.git_status: str = "  "
+        self.git_status: Optional[str] = None
 
         if state.state.git_root is not None:
             try:
-                self.path_wrt_git = self.path.relative_to(state.state.git_root)
-                self.git_status = state.state.git_status_map.get(
-                    self.path_wrt_git, "  "
+                self.path_wrt_git = node.path.absolute().relative_to(
+                    state.state.git_root
                 )
+                self.git_status = state.state.git_status_map.get(self.path_wrt_git)
             except ValueError:
                 # This is dest node for absolute symlink to file outside Git repo.
                 pass
 
     @cached_property
-    def git_cells(self) -> dict[str, str]:
+    def cells(self) -> dict[str, str]:
         """mapping of detail keys to the corresponding formatted Git-status"""
 
         if state.state.git_root is None:
             return {}
 
         cells = {"git": formatted_status(self.git_status)}
         return cells
 
     @cached_property
-    def git_format_rules(self) -> tuple[list[str], list[str]]:
+    def format_rules(self) -> FormatRules:
         """the formatting associated with a node's Git status"""
 
-        fmt_rules: list[str] = []
-        txt_fmt_rules: list[str] = []
+        fmt_rules = FormatRules()
 
         if self.git_status == "!!":  # Git-ignored node
             fmt_rules.append("dim")
 
-        return fmt_rules, txt_fmt_rules
+        return fmt_rules
```

### Comparing `pls-5.4.0/src/pls/models/mixins/tree.py` & `pls-6.0.0/src/pls/models/tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic, Optional, TypeVar, cast
+from typing import TYPE_CHECKING
 
 from pls.config import constants
 from pls.globals import args
-from pls.models.base_node import BaseNode
 
 
 if TYPE_CHECKING:
-    from pls.models.node import Node
+    from typing import Callable, Optional
 
-    T = TypeVar("T", bound=Node)
-else:
-    T = TypeVar("T")
+    from pls.models.node_spec import NodeSpec
 
 
-class TreeMixin(Generic[T], BaseNode):
+class Tree:
     """
-    This mixin provides functionality associated with rendering trees.
+    This class provides functionality associated with rendering trees. It should be
+    inherited by any class that behaves as a tree.
     """
 
+    @staticmethod
+    def link(parent: Tree, *children: Tree):
+        """
+        Link a parent node with any number of children nodes.
+
+        :param parent: the parent node to which the children are being linked
+        :param children: the children to each of which the parent is being linked
+        """
+
+        for child in children:
+            child.parent = parent
+            parent.children.append(child)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.children: list[T] = []
-        self.parent: Optional[T] = None
+        self.children: list[Tree] = []
+        self.parent: Optional[Tree] = None
 
         self.pre_shapes: list[str] = []
         self.last_shape: str = ""
 
     @property
     def is_sub(self) -> bool:  # TODO: Use TypeGuards
         """whether the node is a sub node of another"""
 
         return self.parent is not None
 
     @property
-    def is_visible(self) -> bool:
-        """whether the node deserves to be rendered to the screen"""
-
-        is_tree_visible = not self.is_sub or args.args.collapse <= 1
-        return is_tree_visible and super().is_visible
-
-    @property
     def tree_prefix(self) -> str:
         """the complete string to draw the tree lines before the node name"""
 
         tree_chars = "".join([*self.pre_shapes, self.last_shape])
         if args.args.align:
             tree_chars = f" {tree_chars}"
         return tree_chars
@@ -59,19 +63,19 @@
         :param end_shape: the box-drawing characters for the last node
         :param not_end_shape: the box-drawing characters for other nodes
         :return: ``end_shape`` if the node is last, ``not_end_shape`` otherwise
         """
 
         if not self.is_sub:
             return ""
-
         assert self.parent is not None
+
         siblings = self.parent.children
 
-        is_last = siblings.index(cast(T, self)) == len(siblings) - 1
+        is_last = siblings.index(self) == len(siblings) - 1
         if is_last:
             return end_shape
 
         return not_end_shape
 
     def _get_pre_shape(self) -> str:
         """
@@ -80,18 +84,21 @@
         ancestors.
 
         Can either be ``"  "`` or ``"| "``.
 
         :return: the set of box-drawing characters before the node's own
         """
 
-        return self.get_shape(
+        shape = self.get_shape(
             constants.constants.lookup("tree", "space_space", default=""),
             constants.constants.lookup("tree", "pipe_space", default=""),
         )
+        if shape and args.args.align:
+            shape = f"{shape} "
+        return shape
 
     def _get_last_shape(self) -> str:
         """
         Get the box-drawing characters to render before the node itself. The
         last shape is the box drawing characters pertaining to itself.
 
         Can either be ``"└ "`` or ``"├ "``.
@@ -111,31 +118,13 @@
 
         pre_shapes = [*self.pre_shapes, self._get_pre_shape()]
         for sub_node in self.children:
             sub_node.pre_shapes.extend(pre_shapes)
             sub_node.set_sub_pre_shapes()
             sub_node.last_shape = sub_node._get_last_shape()
 
-    def find_main(self, node_map: dict[str, T]):
-        """
-        Find the main node of this node from the mapping of node names and
-        corresponding ``Node`` instances. If the spec specifies ``collapse`` and
-        the main node exists, register this node as a sub-node of the main one.
-
-        :param node_map: the mapping of names and ``Node`` instances
-        """
-
-        collapses = self.spec_attr("collapse", coalesce=True)
-        if not collapses:
-            return
-
-        for collapse in collapses:
-            if "extension" in collapse:
-                extension = collapse["extension"]
-                name = self.name.replace(self.extension, extension)
-            else:  # "name" in collapse:
-                name = collapse["name"]
-
-            if (node := node_map.get(name)) is not None and node.is_visible:
-                node_map[name].children.append(cast(T, self))
-                self.parent = node
-                break
+    def populate_tree(
+        self,
+        specs: list[NodeSpec],
+        populate_callback: Callable = lambda _: None,
+    ):
+        raise NotImplementedError
```

### Comparing `pls-5.4.0/src/pls/models/node_spec.py` & `pls-6.0.0/src/pls/models/node_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
-    from pls.models.base_node import BaseNode
+    from pls.models.node import Node
 
 
 class NodeSpec:
     """
     A spec describes the nature of a class of FS nodes that determine its
     presentation. This model stores attributes pertaining to a single spec. Make
     sure to massage spec entries using :py:func:`pls.data.config.massage_specs`
@@ -54,27 +54,26 @@
             return f"*.{self.extension}"
         if self.pattern:
             return f"/{self.pattern.pattern}/"
         if self.glob:
             return f"<{self.glob}>"
         return "[No ID]"
 
-    def match(self, node: BaseNode) -> bool:
+    def match(self, node: Node) -> bool:
         """
         Check whether the given node matches this spec. The criterion for
         evaluating a match is based on whether the spec defines the name,
         regular expression, glob pattern or extension.
 
         :param node: the node to compare against the spec for a match
         :return: ``True`` if the node matches this entry, ``False`` otherwise
         """
 
         if self.name:
             return self.name == node.name
-        elif self.pattern:
+        if self.pattern:
             return self.pattern.match(node.name) is not None
-        elif self.glob:
+        if self.glob:
             return node.path.match(self.glob)
-        elif self.extension:
-            return self.extension == node.extension
-        else:
-            return False
+        if self.extension:
+            return self.extension == node.name_comp.ext
+        return False
```

### Comparing `pls-5.4.0/src/pls/output/columns/all_columns.py` & `pls-6.0.0/src/pls/output/columns/all_columns.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/output/columns/detail_columns.py` & `pls-6.0.0/src/pls/output/columns/detail_columns.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/output/columns_printer.py` & `pls-6.0.0/src/pls/output/columns_printer.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/output/printers.py` & `pls-6.0.0/src/pls/output/printers.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/output/solarized.py` & `pls-6.0.0/src/pls/output/solarized.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/output/table_printer.py` & `pls-6.0.0/src/pls/output/table_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,36 +19,14 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.cols: list[ColumnSpec] = self._get_cols()
         self.table = self._get_table()
 
     @staticmethod
-    def _column_chosen(spec: ColumnSpec) -> bool:
-        """
-        Determine whether the given column name has been asked for in the details.
-
-        :param spec: the specification of the column to check
-        :return: ``True`` if the column is to be shown, ``False`` otherwise
-        """
-
-        default_details = [
-            "type",
-            "perms",
-            "user",
-            "group",
-        ]
-
-        return (
-            spec.key in args.args.details
-            or "all" in args.args.details
-            or (spec.key in default_details and "std" in args.args.details)
-        )
-
-    @staticmethod
     def _filter_groups(
         all_col_groups: list[list[str]],
         extra_cond: Callable[[ColumnSpec], bool] = lambda _: True,
     ) -> list[list[ColumnSpec]]:
         """
         Given a group of column groups, filter out all unavailable columns.
 
@@ -74,15 +52,15 @@
         """
 
         detail_col_groups, required_col_groups = column_groups
         selected_col_groups = []
         if args.args.details:
             selected_col_groups.extend(
                 TablePrinter._filter_groups(
-                    detail_col_groups, TablePrinter._column_chosen
+                    detail_col_groups, lambda spec: spec.key in args.args.details
                 )
             )
         selected_col_groups.extend(TablePrinter._filter_groups(required_col_groups))
 
         flattened_cols = []
         for index, col_group in enumerate(selected_col_groups):
             # Skip groups with zero chosen columns.
@@ -104,15 +82,15 @@
         :return: a Rich table
         """
 
         table = Table(
             padding=(0, 1, 0, 0),
             box=None,
             show_header=bool(args.args.details),
-            header_style="underline",
+            header_style="underline bold",
         )
         for col in self.cols:
             table.add_column(col.name, **col.attrs)
         return table
 
     def tabulate_node(self, node: Node):
         """
@@ -122,16 +100,18 @@
         :param node: the node to insert into the table
         """
 
         data = node.table_row
         if data is not None:
             cells = [data.get(col.key, col.value or "") for col in self.cols]
             self.table.add_row(*cells)
-            for sub_node in node.children:
-                self.tabulate_node(sub_node)
+            if not args.args.tree:
+                for sub_node in node.children:
+                    if isinstance(sub_node, Node):
+                        self.tabulate_node(sub_node)
 
     def print_output(self):
         for node in self.all_nodes:
             # Sub-nodes are not tabulated with the rest of the top-level nodes.
             if node.is_sub:
                 continue
             self.tabulate_node(node)
```

### Comparing `pls-5.4.0/src/pls/output/update.py` & `pls-6.0.0/src/pls/output/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,22 @@
     """
 
     res = requests.get(f"https://pypi.org/pypi/{__pkg__}/json", timeout=0.5)
     package_info = res.json()
     return package_info["info"]["version"]
 
 
+def print_version():
+    """
+    Print the current version to the console.
+    """
+
+    console.console.print(f"[red bold]pls[/] [blue]{__version__}[/]")
+
+
 def check_update():
     """
     Compare the current version to the latest and show an upgrade message if a newer
     version has been published.
     """
 
     try:
@@ -75,13 +83,12 @@
         upgrade_color_map: dict[UpgradeType, str] = {
             "major": "red",
             "minor": "yellow",
             "patch": "green",
         }
         message_color = upgrade_color_map[diff]
 
-        console.console.print()  # blank line
         console.console.print(
             f"A new [bold {message_color}]{diff}[/] version is available: "
             f"[blue]{latest_version}[/]. "
             "Please upgrade."
         )
```

### Comparing `pls-5.4.0/src/pls/parser/actions.py` & `pls-6.0.0/src/pls/parser/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import argparse
 import logging
+import os
+
+from pls.globals import console
+from pls.output.update import check_update, print_version
 
 
 logger = logging.getLogger(__name__)
 
 
 class BooleanOptionalAction(argparse.Action):
     """
@@ -77,7 +81,35 @@
         if values is not None:  # ``values`` can be 0
             setattr(namespace, self.dest, values)
         else:
             count = getattr(namespace, self.dest, None)
             if count is None:
                 count = 0
             setattr(namespace, self.dest, count + 1)
+
+
+class VersionUpdateAction(argparse.Action):
+    """
+    Combines the behaviour of the built inCheck if there are any new versions of
+    ``pls`` available on PyPI.
+    """
+
+    def __init__(self, *args, **kwargs):
+        kwargs.pop("nargs", None)
+
+        super().__init__(*args, **kwargs, nargs=0)
+
+    def __call__(self, parser, *args, **kwargs):
+        console.console = console.get_console()
+
+        print_version()
+        if not (os.getenv("PLS_NO_UPDATE_CHECK") or os.getenv("CI")):
+            check_update()
+
+        parser.exit()
+
+
+def register_actions(parser: argparse.ArgumentParser):
+    parser.register("action", "boolean_optional", BooleanOptionalAction)
+    parser.register("action", "collect_or_clear", CollectOrClearAction)
+    parser.register("action", "store_or_count", StoreOrCountAction)
+    parser.register("action", "version_update", VersionUpdateAction)
```

### Comparing `pls-5.4.0/src/pls/parser/args/dev.py` & `pls-6.0.0/src/pls/parser/args/dev.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/parser/args/filter.py` & `pls-6.0.0/src/pls/parser/args/filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import argparse
 import re
 
-from pls.parser.actions import BooleanOptionalAction, StoreOrCountAction
-
 
 def add_args(parser: argparse.ArgumentParser):
     """
     Add arguments for filtering to the given parser.
 
     :param parser: the parser to which to add the arguments
     """
 
     filtering = parser.add_argument_group(
         title="filtering",
         description="arguments used for filtering nodes in the output",
     )
     filtering.add_argument(
         *["-a", "--all"],
-        action=StoreOrCountAction,
+        action="store_or_count",
         help="increasingly show low-importance files that would otherwise be hidden",
     )
     filtering.add_argument(
         "--dirs",
-        action=BooleanOptionalAction,
+        action="boolean_optional",
         help="[underline]show[/]/[magenta]hide[/] directories in the output",
     )
     filtering.add_argument(
         "--files",
-        action=BooleanOptionalAction,
+        action="boolean_optional",
         help="[underline]show[/]/[magenta]hide[/] files in the output",
     )
     filtering.add_argument(
         *["-e", "--exclude"],
         type=lambda val: re.compile(val),
         help="do not show nodes that match the given regular expression",
     )
```

### Comparing `pls-5.4.0/src/pls/parser/args/info.py` & `pls-6.0.0/src/pls/parser/args/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 
 from pls.enums.unit_system import UnitSystem
 from pls.output.columns.detail_columns import detail_column_specs
-from pls.parser.actions import CollectOrClearAction
 
 
 detail_choices = list(detail_column_specs.keys()) + [
     "none",  # means no details
     "std",  # means the default set of details
     "all",  # means all details
 ]
@@ -22,15 +21,15 @@
     info = parser.add_argument_group(
         title="info",
         description="arguments for toggling and customising details for nodes",
     )
     info.add_argument(
         *["-d", "--details"],
         metavar="FIELD",
-        action=CollectOrClearAction,
+        action="collect_or_clear",
         nargs=argparse.OPTIONAL,
         const="std",  # when there is a --details flag without value, see ``nargs``
         help="the data points to show for each node in the output",
         choices=detail_choices,
     )
     info.add_argument(
         *["-u", "--units"],
```

### Comparing `pls-5.4.0/src/pls/parser/args/meta.py` & `pls-6.0.0/src/pls/parser/args/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import argparse
 
-from pls import __version__
-
 
 def add_args(parser: argparse.ArgumentParser):
     """
     Add meta arguments to the given parser.
 
     :param parser: the parser to which to add the arguments
     """
@@ -17,11 +15,10 @@
     meta.add_argument(
         *["-h", "--help"],
         action="help",
         help="show this help message and exit",
     )
     meta.add_argument(
         *["-v", "--version"],
-        action="version",
-        version=f"%(prog)s {__version__}",
+        action="version_update",
         help="show the version of the codebase",
     )
```

### Comparing `pls-5.4.0/src/pls/parser/args/pos.py` & `pls-6.0.0/src/pls/parser/args/pos.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/parser/args/pres.py` & `pls-6.0.0/src/pls/parser/args/pres.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import argparse
 
 from pls.enums.icon_type import IconType
-from pls.parser.actions import BooleanOptionalAction, StoreOrCountAction
 
 
 def add_args(parser: argparse.ArgumentParser):
     """
     Add arguments for presentation to the given parser.
 
     :param parser: the parser to which to add the arguments
@@ -20,20 +19,25 @@
         metavar="TYPE",
         type=IconType,
         choices=list(IconType),
         help="the type of icons to show with the files",
     )
     presentation.add_argument(
         "--align",
-        action=BooleanOptionalAction,
+        action="boolean_optional",
         help="[underline]do[/]/[magenta]don't[/] align names based on leading dots",
     )
     presentation.add_argument(
         "--multi-cols",
-        action=BooleanOptionalAction,
+        action="boolean_optional",
         help="render output in multiple/[magenta][underline]single[/][/] columns",
     )
     presentation.add_argument(
         *["-c", "--collapse"],
-        action=StoreOrCountAction,
+        action="store_or_count",
         help="collapse autogenerated files behind their sources",
     )
+    presentation.add_argument(
+        "--tree",
+        action="boolean_optional",
+        help="do/[magenta][underline]don't[/][/] expand directories recursively",
+    )
```

### Comparing `pls-5.4.0/src/pls/parser/args/sort.py` & `pls-6.0.0/src/pls/parser/args/sort.py`

 * *Files identical despite different names*

### Comparing `pls-5.4.0/src/pls/parser/base.py` & `pls-6.0.0/src/pls/parser/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Overrides ``_format_args`` to bridge the version difference between Python
         versions and return consistent output for the 'nodes' positional argument.
         """
 
         if action.nargs == argparse.ZERO_OR_MORE:
             get_metavar = self._metavar_formatter(action, default_metavar)
             metavar = get_metavar(1)
-            return "[%s ...]" % metavar
+            return f"[{metavar} ...]"
         return super()._format_args(action, default_metavar)
 
     def _format_usage(self, *args, **kwargs) -> str:
         """
         Use Rich's ``escape`` function to ensure that all the square brackets in the
         usage text are printed to the screen.
         """
```

### Comparing `pls-5.4.0/src/pls/parser/parser.py` & `pls-6.0.0/src/pls/parser/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pls import __pkg__
+from pls.parser.actions import register_actions
 from pls.parser.args import dev, filter, info, meta, pos, pres, sort
 from pls.parser.base import PlsFormatter, PlsParser
 
 
 def _get_core_parser() -> PlsParser:
     """
     Get an empty argument parser for ``pls``. This parser has no arguments or argument
@@ -31,14 +32,16 @@
     Get the parser with all arguments configured on it.
 
     :return: the complete ``pls`` argument parser
     """
 
     core_parser = _get_core_parser()
 
+    register_actions(core_parser)
+
     arg_modules = [pos, meta, pres, info, sort, filter, dev]
     for arg_module in arg_modules:
         adder = getattr(arg_module, "add_args")
         adder(core_parser)
 
     return core_parser
```

### Comparing `pls-5.4.0/setup.py` & `pls-6.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pls
+Version: 6.0.0
+Summary: `pls` is a prettier and powerful `ls` for the pros.
+Home-page: https://dhruvkb.github.io/pls
+License: GPL-3.0-or-later
+Author: Dhruv Bhanushali
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Project-URL: Documentation, https://dhruvkb.github.io/pls
+Project-URL: Repository, https://github.com/dhruvkb/pls
+Description-Content-Type: text/markdown
+
+<h1 align="center">
+  <img height="128px" src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/pls.svg"/>
+
+  <p align="center">
+    <a href="https://www.python.org">
+      <img src="https://img.shields.io/pypi/pyversions/pls" alt="Python versions"/>
+    </a>
+    <a href="https://github.com/dhruvkb/pls/blob/main/LICENSE">
+      <img src="https://img.shields.io/github/license/dhruvkb/pls" alt="GPL-3.0"/>
+    </a>
+    <a href="https://pypi.org/project/pls/">
+      <img src="https://img.shields.io/static/v1?label=supported%20OS&message=posix,%20win&color=informational" alt="Platforms"/>
+    </a>
+    <a href="https://github.com/dhruvkb/pls/actions/workflows/ci.yml">
+      <img src="https://github.com/dhruvkb/pls/actions/workflows/ci.yml/badge.svg" alt="CI status"/>
+    </a>
+    <a href="https://github.com/dhruvkb/pls">
+      <img src="https://tokei.rs/b1/github/dhruvkb/pls" alt="LoC"/>
+    </a>
+  </p>
+</h1>
+
+<p align="center">
+  <strong>Links:</strong>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/pls/">
+    <img src="https://img.shields.io/pypi/v/pls" alt="pls on PyPI"/>
+  </a>
+  <a href="https://dhruvkb.github.io/pls/">
+    <img src="https://img.shields.io/static/v1?label=docs&message=dhruvkb/pls:docs&color=informational" alt="Docs"/>
+  </a>
+</p>
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/demo.png" alt="Demo of `pls`"/>
+  <img src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/help.png" alt="Help of `pls`"/>
+</p>
+
+`pls` is a prettier and powerful `ls` for the pros.
+
+The "p" stands for
+- pretty (the output from `pls` surely looks better)
+- powerful (`pls` has lots of features and endless customisation)
+- programmer (`pls` is geared towards developers)
+- professional (`pls` can be extensively tweaked by the pros)
+- Python (`pls` is written in Python!)
+
+Just pick whichever helps you remember the command name.
+
+It works in a manner similar to `ls`, in  that it lists directories and files in
+a given directory, but it adds many more
+[developer-friendly features](https://dhruvkb.github.io/pls/features).
+
+> ⚠️ Note that `pls` is not a replacement for `ls`. `ls` is a tried, tested and
+trusted command with lots of features. `pls`, on the other hand, is a simple
+tool for people who just want to see the contents of their directories.
+
+## Documentation
+
+We have some very beautiful [documentation](https://dhruvkb.github.io/pls) over
+on our GitHub pages site. These docs are built from the
+[`docs` branch](https://github.com/dhruvkb/pls/tree/docs) in the same
+repository, and contributions to the docs are most welcome.
+
+The docs contain information on almost everything, including but not limited to
+the following:
+
+- [installation and updates](https://dhruvkb.github.io/pls/get_started/installation)
+- [features and CLI options](https://dhruvkb.github.io/pls/features)
+- [reference](https://dhruvkb.github.io/pls/reference)
+- [contribution](https://dhruvkb.github.io/pls/contribution)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pls',
- 'pls.config',
- 'pls.data',
- 'pls.enums',
- 'pls.fs',
- 'pls.globals',
- 'pls.log',
- 'pls.models',
- 'pls.models.mixins',
- 'pls.output',
- 'pls.output.columns',
- 'pls.parser',
- 'pls.parser.args',
- 'pls.utils']
-
-package_data = \
-{'': ['*'], 'pls.data': ['schema/*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0', 'requests>=2.27.1,<3.0.0', 'rich>=12.5.1,<13.0.0']
-
-entry_points = \
-{'console_scripts': ['pls = pls.main:main', 'pls-dev = pls.main:dev']}
-
-setup_kwargs = {
-    'name': 'pls',
-    'version': '5.4.0',
-    'description': '`pls` is a prettier and powerful `ls` for the pros.',
-    'long_description': '<h1 align="center">\n  <img height="128px" src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/pls.svg"/>\n\n  <p align="center">\n    <a href="https://www.python.org">\n      <img src="https://img.shields.io/pypi/pyversions/pls" alt="Python versions"/>\n    </a>\n    <a href="https://github.com/dhruvkb/pls/blob/main/LICENSE">\n      <img src="https://img.shields.io/github/license/dhruvkb/pls" alt="GPL-3.0"/>\n    </a>\n    <a href="https://pypi.org/project/pls/">\n      <img src="https://img.shields.io/static/v1?label=supported%20OS&message=posix,%20win&color=informational" alt="Platforms"/>\n    </a>\n    <a href="https://github.com/dhruvkb/pls/actions/workflows/ci.yml">\n      <img src="https://github.com/dhruvkb/pls/actions/workflows/ci.yml/badge.svg" alt="CI status"/>\n    </a>\n    <a href="https://github.com/dhruvkb/pls">\n      <img src="https://tokei.rs/b1/github/dhruvkb/pls" alt="LoC"/>\n    </a>\n  </p>\n</h1>\n\n<p align="center">\n  <strong>Links:</strong>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/pls/">\n    <img src="https://img.shields.io/pypi/v/pls" alt="pls on PyPI"/>\n  </a>\n  <a href="https://dhruvkb.github.io/pls/">\n    <img src="https://img.shields.io/static/v1?label=docs&message=dhruvkb/pls:docs&color=informational" alt="Docs"/>\n  </a>\n</p>\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/demo.png" alt="Demo of `pls`"/>\n  <img src="https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/help.png" alt="Help of `pls`"/>\n</p>\n\n`pls` is a prettier and powerful `ls` for the pros.\n\nThe "p" stands for\n- pretty (the output from `pls` surely looks better)\n- powerful (`pls` has lots of features and endless customisation)\n- programmer (`pls` is geared towards developers)\n- professional (`pls` can be extensively tweaked by the pros)\n- Python (`pls` is written in Python!)\n\nJust pick whichever helps you remember the command name.\n\nIt works in a manner similar to `ls`, in  that it lists directories and files in\na given directory, but it adds many more\n[developer-friendly features](https://dhruvkb.github.io/pls/features).\n\n> ⚠️ Note that `pls` is not a replacement for `ls`. `ls` is a tried, tested and\ntrusted command with lots of features. `pls`, on the other hand, is a simple\ntool for people who just want to see the contents of their directories.\n\n## Documentation\n\nWe have some very beautiful [documentation](https://dhruvkb.github.io/pls) over\non our GitHub pages site. These docs are built from the\n[`docs` branch](https://github.com/dhruvkb/pls/tree/docs) in the same\nrepository, and contributions to the docs are most welcome.\n\nThe docs contain information on almost everything, including but not limited to\nthe following:\n\n- [installation and updates](https://dhruvkb.github.io/pls/get_started/installation)\n- [features and CLI options](https://dhruvkb.github.io/pls/features)\n- [reference](https://dhruvkb.github.io/pls/reference)\n- [contribution](https://dhruvkb.github.io/pls/contribution)\n',
-    'author': 'Dhruv Bhanushali',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://dhruvkb.github.io/pls',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,44 +1,37 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['pls', 'pls.config', 'pls.data', 'pls.enums', 'pls.fs',
-'pls.globals', 'pls.log', 'pls.models', 'pls.models.mixins', 'pls.output',
-'pls.output.columns', 'pls.parser', 'pls.parser.args', 'pls.utils']
-package_data = \ {'': ['*'], 'pls.data': ['schema/*']} install_requires = \
-['PyYAML>=6.0,<7.0', 'requests>=2.27.1,<3.0.0', 'rich>=12.5.1,<13.0.0']
-entry_points = \ {'console_scripts': ['pls = pls.main:main', 'pls-dev =
-pls.main:dev']} setup_kwargs = { 'name': 'pls', 'version': '5.4.0',
-'description': '`pls` is a prettier and powerful `ls` for the pros.',
-'long_description': '
- ****** \n [https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/
-pls.svg]\n\n\n \n_[Python_versions]\n\n \n_[GPL-3.0]\n\n \n_[Platforms]\n\n \n_
-                     [CI_status]\n\n \n_[LoC]\n\n\n ******
-\n\n
-                                  \n Links:\n
-\n
-                     \n \n_[pls_on_PyPI]\n\n \n_[Docs]\n\n
-\n\n
-                    \n [Demo of `pls`]\n [Help of `pls`]\n
-\n\n`pls` is a prettier and powerful `ls` for the pros.\n\nThe "p" stands
-for\n- pretty (the output from `pls` surely looks better)\n- powerful (`pls`
-has lots of features and endless customisation)\n- programmer (`pls` is geared
-towards developers)\n- professional (`pls` can be extensively tweaked by the
-pros)\n- Python (`pls` is written in Python!)\n\nJust pick whichever helps you
-remember the command name.\n\nIt works in a manner similar to `ls`, in that it
-lists directories and files in\na given directory, but it adds many more\n
-[developer-friendly features](https://dhruvkb.github.io/pls/features).\n\n>
-â ï¸ Note that `pls` is not a replacement for `ls`. `ls` is a tried, tested
-and\ntrusted command with lots of features. `pls`, on the other hand, is a
-simple\ntool for people who just want to see the contents of their
-directories.\n\n## Documentation\n\nWe have some very beautiful [documentation]
-(https://dhruvkb.github.io/pls) over\non our GitHub pages site. These docs are
-built from the\n[`docs` branch](https://github.com/dhruvkb/pls/tree/docs) in
-the same\nrepository, and contributions to the docs are most welcome.\n\nThe
-docs contain information on almost everything, including but not limited
-to\nthe following:\n\n- [installation and updates](https://dhruvkb.github.io/
-pls/get_started/installation)\n- [features and CLI options](https://
-dhruvkb.github.io/pls/features)\n- [reference](https://dhruvkb.github.io/pls/
-reference)\n- [contribution](https://dhruvkb.github.io/pls/contribution)\n',
-'author': 'Dhruv Bhanushali', 'author_email': None, 'maintainer': None,
-'maintainer_email': None, 'url': 'https://dhruvkb.github.io/pls',
-'package_dir': package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: pls Version: 6.0.0 Summary: `pls` is a prettier and
+powerful `ls` for the pros. Home-page: https://dhruvkb.github.io/pls License:
+GPL-3.0-or-later Author: Dhruv Bhanushali Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later
+(GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: rich
+(>=12.5.1,<13.0.0) Project-URL: Documentation, https://dhruvkb.github.io/pls
+Project-URL: Repository, https://github.com/dhruvkb/pls Description-Content-
+Type: text/markdown
+   ****** [https://raw.githubusercontent.com/dhruvkb/pls/main/readme_assets/
+   pls.svg][Python_versions] [GPL-3.0] [Platforms] [CI_status] [LoC] ******
+                                    Links:
+                             [pls_on_PyPI] [Docs]
+                        [Demo of `pls`] [Help of `pls`]
+`pls` is a prettier and powerful `ls` for the pros. The "p" stands for - pretty
+(the output from `pls` surely looks better) - powerful (`pls` has lots of
+features and endless customisation) - programmer (`pls` is geared towards
+developers) - professional (`pls` can be extensively tweaked by the pros) -
+Python (`pls` is written in Python!) Just pick whichever helps you remember the
+command name. It works in a manner similar to `ls`, in that it lists
+directories and files in a given directory, but it adds many more [developer-
+friendly features](https://dhruvkb.github.io/pls/features). > â ï¸ Note that
+`pls` is not a replacement for `ls`. `ls` is a tried, tested and trusted
+command with lots of features. `pls`, on the other hand, is a simple tool for
+people who just want to see the contents of their directories. ## Documentation
+We have some very beautiful [documentation](https://dhruvkb.github.io/pls) over
+on our GitHub pages site. These docs are built from the [`docs` branch](https:/
+/github.com/dhruvkb/pls/tree/docs) in the same repository, and contributions to
+the docs are most welcome. The docs contain information on almost everything,
+including but not limited to the following: - [installation and updates](https:
+//dhruvkb.github.io/pls/get_started/installation) - [features and CLI options]
+(https://dhruvkb.github.io/pls/features) - [reference](https://
+dhruvkb.github.io/pls/reference) - [contribution](https://dhruvkb.github.io/
+pls/contribution)
```

