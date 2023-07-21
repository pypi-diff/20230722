# Comparing `tmp/py4cytoscape-1.7.0.tar.gz` & `tmp/py4cytoscape-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\py4cytoscape-1.7.0.tar", last modified: Sun Mar 12 22:44:13 2023, max compression
+gzip compressed data, was "dist\py4cytoscape-1.8.0.tar", last modified: Fri Jul 21 22:48:09 2023, max compression
```

## Comparing `py4cytoscape-1.7.0.tar` & `py4cytoscape-1.8.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 22:44:13.844484 py4cytoscape-1.7.0/
--rw-rw-rw-   0        0        0     1246 2022-05-06 19:31:46.000000 py4cytoscape-1.7.0/LICENSE.rst
--rw-rw-rw-   0        0        0     4590 2023-03-12 22:44:13.836125 py4cytoscape-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3623 2022-06-28 23:23:26.000000 py4cytoscape-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 22:44:13.293399 py4cytoscape-1.7.0/py4cytoscape/
--rw-rw-rw-   0        0        0     3236 2022-05-31 18:08:35.000000 py4cytoscape-1.7.0/py4cytoscape/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/_version.py
--rw-rw-rw-   0        0        0    55157 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/annotations.py
--rw-rw-rw-   0        0        0    14409 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/apps.py
--rw-rw-rw-   0        0        0     6023 2022-06-28 23:01:09.000000 py4cytoscape-1.7.0/py4cytoscape/collections.py
--rw-rw-rw-   0        0        0    36092 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/commands.py
--rw-rw-rw-   0        0        0    10870 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/cy_ndex.py
--rw-rw-rw-   0        0        0     7445 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/cytoscape_system.py
--rw-rw-rw-   0        0        0     2432 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/decorators.py
--rw-rw-rw-   0        0        0     2253 2022-08-04 01:45:05.000000 py4cytoscape-1.7.0/py4cytoscape/exceptions.py
--rw-rw-rw-   0        0        0    24751 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/filters.py
--rw-rw-rw-   0        0        0    23244 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/groups.py
--rw-rw-rw-   0        0        0    17514 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/layouts.py
--rw-rw-rw-   0        0        0    43692 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/network_selection.py
--rw-rw-rw-   0        0        0    24738 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/network_views.py
--rw-rw-rw-   0        0        0    76003 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/networks.py
--rw-rw-rw-   0        0        0     8037 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/notebook.py
--rw-rw-rw-   0        0        0     8278 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_logger.py
--rw-rw-rw-   0        0        0     1722 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_logger_settings.py
--rw-rw-rw-   0        0        0    12422 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_notebook.py
--rw-rw-rw-   0        0        0     9437 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_sandbox.py
--rw-rw-rw-   0        0        0     2554 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_tuning.py
--rw-rw-rw-   0        0        0    37018 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_utils.py
--rw-rw-rw-   0        0        0    30142 2022-06-28 23:01:09.000000 py4cytoscape-1.7.0/py4cytoscape/sandbox.py
--rw-rw-rw-   0        0        0     7672 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/session.py
--rw-rw-rw-   0        0        0    87327 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/style_auto_mappings.py
--rw-rw-rw-   0        0        0   129440 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/style_bypasses.py
--rw-rw-rw-   0        0        0    79317 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/style_defaults.py
--rw-rw-rw-   0        0        0     9753 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/style_dependencies.py
--rw-rw-rw-   0        0        0   113755 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/style_mappings.py
--rw-rw-rw-   0        0        0    36763 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/py4cytoscape/style_values.py
--rw-rw-rw-   0        0        0     4538 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/style_visual_props.py
--rw-rw-rw-   0        0        0    21750 2022-06-28 23:01:09.000000 py4cytoscape-1.7.0/py4cytoscape/styles.py
--rw-rw-rw-   0        0        0    33276 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/tables.py
--rw-rw-rw-   0        0        0    25082 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/py4cytoscape/tools.py
--rw-rw-rw-   0        0        0     7223 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/py4cytoscape/user_interface.py
-drwxrwxrwx   0        0        0        0 2023-03-12 22:44:13.331148 py4cytoscape-1.7.0/py4cytoscape.egg-info/
--rw-rw-rw-   0        0        0     4590 2023-03-12 22:44:12.000000 py4cytoscape-1.7.0/py4cytoscape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1924 2023-03-12 22:44:12.000000 py4cytoscape-1.7.0/py4cytoscape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 22:44:12.000000 py4cytoscape-1.7.0/py4cytoscape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-03-12 22:44:12.000000 py4cytoscape-1.7.0/py4cytoscape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-12 22:44:12.000000 py4cytoscape-1.7.0/py4cytoscape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 22:44:13.844484 py4cytoscape-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1846 2023-03-12 20:47:02.000000 py4cytoscape-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-12 22:44:13.836125 py4cytoscape-1.7.0/tests/
--rw-rw-rw-   0        0        0    79567 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_annotations.py
--rw-rw-rw-   0        0        0    12858 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/tests/test_apps.py
--rw-rw-rw-   0        0        0     4984 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_collections.py
--rw-rw-rw-   0        0        0    16881 2022-12-12 23:41:03.000000 py4cytoscape-1.7.0/tests/test_commands.py
--rw-rw-rw-   0        0        0    10351 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_cy_ndex.py
--rw-rw-rw-   0        0        0     3699 2022-12-13 00:57:26.000000 py4cytoscape-1.7.0/tests/test_cytoscape_system.py
--rw-rw-rw-   0        0        0    23679 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_filters.py
--rw-rw-rw-   0        0        0    39638 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_groups.py
--rw-rw-rw-   0        0        0    11922 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_layouts.py
--rw-rw-rw-   0        0        0    35958 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_network_selection.py
--rw-rw-rw-   0        0        0    24884 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_network_views.py
--rw-rw-rw-   0        0        0    74860 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/tests/test_networks.py
--rw-rw-rw-   0        0        0    16112 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_py4cytoscape_utils.py
--rw-rw-rw-   0        0        0    28298 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_sandbox.py
--rw-rw-rw-   0        0        0    12465 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_sanity.py
--rw-rw-rw-   0        0        0     5797 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_session.py
--rw-rw-rw-   0        0        0   105285 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_style_auto_mappings.py
--rw-rw-rw-   0        0        0    33958 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_style_bypasses.py
--rw-rw-rw-   0        0        0    67593 2023-01-12 21:13:45.000000 py4cytoscape-1.7.0/tests/test_style_defaults.py
--rw-rw-rw-   0        0        0     6845 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_style_dependencies.py
--rw-rw-rw-   0        0        0    91607 2023-01-14 20:02:19.000000 py4cytoscape-1.7.0/tests/test_style_mappings.py
--rw-rw-rw-   0        0        0    11072 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_style_values.py
--rw-rw-rw-   0        0        0    21240 2022-06-28 23:01:09.000000 py4cytoscape-1.7.0/tests/test_styles.py
--rw-rw-rw-   0        0        0    24470 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/tests/test_tables.py
--rw-rw-rw-   0        0        0    24118 2023-03-12 20:47:31.000000 py4cytoscape-1.7.0/tests/test_tools.py
--rw-rw-rw-   0        0        0     3507 2022-05-26 20:54:04.000000 py4cytoscape-1.7.0/tests/test_user_interface.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:48:09.769872 py4cytoscape-1.8.0/
+-rw-rw-rw-   0        0        0     1246 2022-05-06 19:31:46.000000 py4cytoscape-1.8.0/LICENSE.rst
+-rw-rw-rw-   0        0        0     4590 2023-07-21 22:48:09.768015 py4cytoscape-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3623 2022-06-28 23:23:26.000000 py4cytoscape-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 22:48:09.109974 py4cytoscape-1.8.0/py4cytoscape/
+-rw-rw-rw-   0        0        0     3236 2022-05-31 18:08:35.000000 py4cytoscape-1.8.0/py4cytoscape/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-03-12 23:10:35.000000 py4cytoscape-1.8.0/py4cytoscape/_version.py
+-rw-rw-rw-   0        0        0    55157 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/py4cytoscape/annotations.py
+-rw-rw-rw-   0        0        0    14409 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/apps.py
+-rw-rw-rw-   0        0        0     6023 2022-06-28 23:01:09.000000 py4cytoscape-1.8.0/py4cytoscape/collections.py
+-rw-rw-rw-   0        0        0    36092 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/commands.py
+-rw-rw-rw-   0        0        0    10870 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/cy_ndex.py
+-rw-rw-rw-   0        0        0     7445 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/cytoscape_system.py
+-rw-rw-rw-   0        0        0     2432 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/decorators.py
+-rw-rw-rw-   0        0        0     2253 2022-08-04 01:45:05.000000 py4cytoscape-1.8.0/py4cytoscape/exceptions.py
+-rw-rw-rw-   0        0        0    24751 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/filters.py
+-rw-rw-rw-   0        0        0    23244 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/py4cytoscape/groups.py
+-rw-rw-rw-   0        0        0    17514 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/layouts.py
+-rw-rw-rw-   0        0        0    43692 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/py4cytoscape/network_selection.py
+-rw-rw-rw-   0        0        0    24738 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/network_views.py
+-rw-rw-rw-   0        0        0    75996 2023-07-20 00:03:49.000000 py4cytoscape-1.8.0/py4cytoscape/networks.py
+-rw-rw-rw-   0        0        0     8037 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/notebook.py
+-rw-rw-rw-   0        0        0     8278 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_logger.py
+-rw-rw-rw-   0        0        0     1722 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_logger_settings.py
+-rw-rw-rw-   0        0        0    12422 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_notebook.py
+-rw-rw-rw-   0        0        0     9437 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_sandbox.py
+-rw-rw-rw-   0        0        0     2554 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_tuning.py
+-rw-rw-rw-   0        0        0    37018 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_utils.py
+-rw-rw-rw-   0        0        0    30142 2022-06-28 23:01:09.000000 py4cytoscape-1.8.0/py4cytoscape/sandbox.py
+-rw-rw-rw-   0        0        0     7672 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/session.py
+-rw-rw-rw-   0        0        0    87327 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/style_auto_mappings.py
+-rw-rw-rw-   0        0        0   132274 2023-07-21 18:06:26.000000 py4cytoscape-1.8.0/py4cytoscape/style_bypasses.py
+-rw-rw-rw-   0        0        0    79398 2023-06-12 22:37:32.000000 py4cytoscape-1.8.0/py4cytoscape/style_defaults.py
+-rw-rw-rw-   0        0        0     9753 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/style_dependencies.py
+-rw-rw-rw-   0        0        0   113755 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/style_mappings.py
+-rw-rw-rw-   0        0        0    36763 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/py4cytoscape/style_values.py
+-rw-rw-rw-   0        0        0     4538 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/style_visual_props.py
+-rw-rw-rw-   0        0        0    21750 2022-06-28 23:01:09.000000 py4cytoscape-1.8.0/py4cytoscape/styles.py
+-rw-rw-rw-   0        0        0    33320 2023-06-28 22:41:24.000000 py4cytoscape-1.8.0/py4cytoscape/tables.py
+-rw-rw-rw-   0        0        0    25082 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/py4cytoscape/tools.py
+-rw-rw-rw-   0        0        0     7223 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/py4cytoscape/user_interface.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:48:09.166075 py4cytoscape-1.8.0/py4cytoscape.egg-info/
+-rw-rw-rw-   0        0        0     4590 2023-07-21 22:48:07.000000 py4cytoscape-1.8.0/py4cytoscape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1924 2023-07-21 22:48:07.000000 py4cytoscape-1.8.0/py4cytoscape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 22:48:07.000000 py4cytoscape-1.8.0/py4cytoscape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-21 22:48:07.000000 py4cytoscape-1.8.0/py4cytoscape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 22:48:07.000000 py4cytoscape-1.8.0/py4cytoscape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 22:48:09.769872 py4cytoscape-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-07-20 00:03:49.000000 py4cytoscape-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:48:09.765015 py4cytoscape-1.8.0/tests/
+-rw-rw-rw-   0        0        0    79567 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_annotations.py
+-rw-rw-rw-   0        0        0    12963 2023-03-19 22:15:58.000000 py4cytoscape-1.8.0/tests/test_apps.py
+-rw-rw-rw-   0        0        0     4984 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_collections.py
+-rw-rw-rw-   0        0        0    17129 2023-04-11 20:16:51.000000 py4cytoscape-1.8.0/tests/test_commands.py
+-rw-rw-rw-   0        0        0    10351 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_cy_ndex.py
+-rw-rw-rw-   0        0        0     3699 2022-12-13 00:57:26.000000 py4cytoscape-1.8.0/tests/test_cytoscape_system.py
+-rw-rw-rw-   0        0        0    23679 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_filters.py
+-rw-rw-rw-   0        0        0    39638 2023-04-12 20:00:43.000000 py4cytoscape-1.8.0/tests/test_groups.py
+-rw-rw-rw-   0        0        0    11922 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_layouts.py
+-rw-rw-rw-   0        0        0    35958 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_network_selection.py
+-rw-rw-rw-   0        0        0    24884 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_network_views.py
+-rw-rw-rw-   0        0        0    74860 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/tests/test_networks.py
+-rw-rw-rw-   0        0        0    16112 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_py4cytoscape_utils.py
+-rw-rw-rw-   0        0        0    28298 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_sandbox.py
+-rw-rw-rw-   0        0        0    12465 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_sanity.py
+-rw-rw-rw-   0        0        0     5797 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_session.py
+-rw-rw-rw-   0        0        0   105285 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_style_auto_mappings.py
+-rw-rw-rw-   0        0        0    33958 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_style_bypasses.py
+-rw-rw-rw-   0        0        0    67593 2023-01-12 21:13:45.000000 py4cytoscape-1.8.0/tests/test_style_defaults.py
+-rw-rw-rw-   0        0        0     6845 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_style_dependencies.py
+-rw-rw-rw-   0        0        0    91607 2023-01-14 20:02:19.000000 py4cytoscape-1.8.0/tests/test_style_mappings.py
+-rw-rw-rw-   0        0        0    11072 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_style_values.py
+-rw-rw-rw-   0        0        0    21240 2022-06-28 23:01:09.000000 py4cytoscape-1.8.0/tests/test_styles.py
+-rw-rw-rw-   0        0        0    25475 2023-07-01 00:17:55.000000 py4cytoscape-1.8.0/tests/test_tables.py
+-rw-rw-rw-   0        0        0    24118 2023-03-12 20:47:31.000000 py4cytoscape-1.8.0/tests/test_tools.py
+-rw-rw-rw-   0        0        0     3507 2022-05-26 20:54:04.000000 py4cytoscape-1.8.0/tests/test_user_interface.py
```

### Comparing `py4cytoscape-1.7.0/LICENSE.rst` & `py4cytoscape-1.8.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/PKG-INFO` & `py4cytoscape-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4cytoscape
-Version: 1.7.0
+Version: 1.8.0
 Summary: Cytoscape Automation API
 Home-page: https://github.com/cytoscape/py4cytoscape
 Author: Barry Demchak
 Author-email: bdemchak@ucsd.edu
 Maintainer: Barry Demchak
 Maintainer-email: bdemchak@ucsd.edu
 License: MIT License
```

### Comparing `py4cytoscape-1.7.0/README.md` & `py4cytoscape-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/__init__.py` & `py4cytoscape-1.8.0/py4cytoscape/__init__.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/_version.py` & `py4cytoscape-1.8.0/py4cytoscape/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 # This is the official version of this library. Change it here, and the build and documentation
 # should pick it up automatically.
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 # This reflects the reference API this module meets
-_automation_api_version = '1.7.0'
+_automation_api_version = '1.8.0'
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape/annotations.py` & `py4cytoscape-1.8.0/py4cytoscape/annotations.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/apps.py` & `py4cytoscape-1.8.0/py4cytoscape/apps.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/collections.py` & `py4cytoscape-1.8.0/py4cytoscape/collections.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/commands.py` & `py4cytoscape-1.8.0/py4cytoscape/commands.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/cy_ndex.py` & `py4cytoscape-1.8.0/py4cytoscape/cy_ndex.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/cytoscape_system.py` & `py4cytoscape-1.8.0/py4cytoscape/cytoscape_system.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/decorators.py` & `py4cytoscape-1.8.0/py4cytoscape/decorators.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/exceptions.py` & `py4cytoscape-1.8.0/py4cytoscape/exceptions.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/filters.py` & `py4cytoscape-1.8.0/py4cytoscape/filters.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/groups.py` & `py4cytoscape-1.8.0/py4cytoscape/groups.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/layouts.py` & `py4cytoscape-1.8.0/py4cytoscape/layouts.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/network_selection.py` & `py4cytoscape-1.8.0/py4cytoscape/network_selection.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/network_views.py` & `py4cytoscape-1.8.0/py4cytoscape/network_views.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/networks.py` & `py4cytoscape-1.8.0/py4cytoscape/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1416,15 +1416,15 @@
     if not {'source', 'target'} <= set(cyedges.columns):
         src_trg = parse_edges(cyedges['name'])
         cyedges['source'] = [x[0] for x in src_trg]
         cyedges['target'] = [x[2] for x in src_trg]
 
     # set up iGraph vertices ... first create vertex by naming it, then pile on attributes
     # Tutorial: https://igraph.org/python/doc/tutorial/tutorial.html
-    # Source: https://github.com/igraph/python-igraph/blob/master/src/igraph/__init__.py
+    # Source: https://github.com/igraph/igraph/blob/master/src/igraph/__init__.py
     g = ig.Graph(directed=True)
 
     # add all nodes and their attributes
     g.add_vertices(list(cynodes['name']))
     for col in cynodes.columns:
         if not col in ['name', 'SUID']: g.vs[col] = list(cynodes[col])
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape/notebook.py` & `py4cytoscape-1.8.0/py4cytoscape/notebook.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_logger.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_logger.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_logger_settings.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_logger_settings.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_notebook.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_notebook.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_sandbox.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_sandbox.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_tuning.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_tuning.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/py4cytoscape_utils.py` & `py4cytoscape-1.8.0/py4cytoscape/py4cytoscape_utils.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/sandbox.py` & `py4cytoscape-1.8.0/py4cytoscape/sandbox.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/session.py` & `py4cytoscape-1.8.0/py4cytoscape/session.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_auto_mappings.py` & `py4cytoscape-1.8.0/py4cytoscape/style_auto_mappings.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_bypasses.py` & `py4cytoscape-1.8.0/py4cytoscape/style_bypasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,30 @@
     elif visual_property in NODE_SHAPE_PROPERTIES:
         new_values = verify_node_shapes(new_values, styles.get_node_shapes(base_url=base_url))
     elif visual_property in NODE_VISIBLE_PROPERTIES:
         new_values = verify_bools(new_values)
     elif visual_property in NODE_LABEL_PROPERTIES | NODE_TOOLTIP_PROPERTIES | NODE_FONT_FACE_PROPERTIES:
         new_values = verify_strs(new_values)
     else:
-        show_error(f'Warning: setting unknown node bypass property "{visual_property}"')
+        # There are a bunch of properties that we can validate when we're next in a major development.
+        # It takes a lot to test these validations, so we don't take this lightly. The NODE properties
+        # we're not validating are: NODE, NODE_BORDER_STROKE, NODE_CUSTOMGRAPHICS_SIZE_1..9, NODE_CUSTOMPAINT_1..9,
+        # NODE_DEPTH, NODE_LABEL_BACKGROUND_COLOR, NODE_LABEL_BACKGROUND_SHAPE, NODE_LABEL_BACKGROUND_TRANSPARENCY,
+        # NODE_LABEL_FONT_FACE, NODE_LABEL_POSITION, NODE_LABEL_ROTATION, NODE_LABEL_WIDTH,
+        # NODE_NESTED_NETWORK_IMAGE_VISIBLE, NODE_PAINT, NODE_SELECTED_PAINT, NODE_X_LOCATION, NODE_Y_LOCATION,
+        # NODE_Z_LOCATION
+        # So, the validation we *do* do should be considered an early convenience, as it's incomplete. Of course, if
+        # a value isn't acceptable to CyREST, an error will be generated by CyREST. So, the above validation is
+        # somewhat redundant. The major exception is with color properties, which should be passed to CyREST as
+        # hex values (e.g., 0x123456). Color validation converts color words (e.g., RED) to hex values, so
+        # the caller must pass unvalidated color properties (e.g., NODE_LABEL_BACKGROUND_COLOR) as only hex values.
+        # Given this, we're removing the warning we were giving for unvalidated properties, as it's more of a
+        # worry for users than it's worth:
+        # show_error(f'Warning: setting unknown node bypass property "{visual_property}"')
+        pass
 
     # there can be more than one node.SUID per node.name!
     # 'node.SUIDs' and 'new.values' must have the same length
     # TODO: Should we allow a scalar for a new_value, or do we assume a list?
     if len(new_values) == 1: new_values = new_values * len(node_suids)
 
     if len(new_values) != len(node_suids):
@@ -305,15 +320,29 @@
     elif visual_property in EDGE_ARROW_STYLE_PROPERTIES:
         new_values = verify_edge_shapes(new_values, styles.get_arrow_shapes(base_url=base_url), 'arrow shape', 'get_arrow_shapes')
     elif visual_property in EDGE_VISIBLE_PROPERTIES:
         new_values = verify_bools(new_values)
     elif visual_property in EDGE_LABEL_PROPERTIES | EDGE_TOOLTIP_PROPERTIES | EDGE_FONT_FACE_PROPERTIES:
         new_values = verify_strs(new_values)
     else:
-        show_error(f'Warning: setting unknown edge bypass property "{visual_property}"')
+        # There are a bunch of properties that we can validate when we're next in a major development.
+        # It takes a lot to test these validations, so we don't take this lightly. The EDGE properties
+        # we're not validating are: EDGE, EDGE_BEND, EDGE_CURVED, EDGE_LABEL_AUTOROTATE, EDGE_LABEL_BACKGROUND_COLOR,
+        # EDGE_LABEL_BACKGROUND_SHAPE, EDGE_LABEL_BACKGROUND_TRANSPARENCY, EDGE_LABEL_FONT_SIZE, EDGE_LABEL_POSITION,
+        # EDGE_LABEL_ROTATION, EDGE_LABEL_WIDTH, EDGE_PAINT, EDGE_SELECTED, EDGE_SOURCE_ARROW_SIZE, EDGE_STACKING,
+        # EDGE_STACKING_DENSITY, EDGE_TARGET_ARROW_SELECTED_PAINT, EDGE_TARGET_ARROW_SIZE, EDGE_WIDTH, EDGE_Z_ORDER
+        # So, the validation we *do* do should be considered an early convenience, as it's incomplete. Of course, if
+        # a value isn't acceptable to CyREST, an error will be generated by CyREST. So, the above validation is
+        # somewhat redundant. The major exception is with color properties, which should be passed to CyREST as
+        # hex values (e.g., 0x123456). Color validation converts color words (e.g., RED) to hex values, so
+        # the caller must pass unvalidated color properties (e.g., EDGE_LABEL_BACKGROUND_COLOR) as only hex values.
+        # Given this, we're removing the warning we were giving for unvalidated properties, as it's more of a
+        # worry for users than it's worth:
+        # show_error(f'Warning: setting unknown edge bypass property "{visual_property}"')
+        pass
 
     # there can be more than one edge.SUID per edge.name!
     # 'edge.SUIDs' and 'new.values' must have the same length
     # TODO: Should we allow a scalar for a new_value, or do we assume a list?
     if len(new_values) == 1: new_values = new_values * len(edge_suids)
 
     if len(new_values) != len(edge_suids):
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_defaults.py` & `py4cytoscape-1.8.0/py4cytoscape/style_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         narrate(f'style_name not specified, so updating "default" style.')
 
     # process visual property, including common alternatives for vp names :)
     def_list = [{'visualProperty': normalize_prop_name(prop), 'value': val} for prop, val in defaults.items()]
 
     # Verify values and adjust them if necessary
     for prop in def_list:
-        prop['value'] = _validate_prop_value(prop['visualProperty'], prop['value'])
+        prop['value'] = _validate_prop_value(prop['visualProperty'], prop['value'], base_url)
 
     res = commands.cyrest_put(f'styles/{style_name}/defaults', body=def_list, base_url=base_url,
                               require_json=False)
     return res
 
 
 @cy_log
@@ -158,15 +158,15 @@
     """
     if style_name is None:
         style_name = 'default'
         narrate(f'style_name not specified, so updating "default" style.')
 
     style_string['visualProperty'] = normalize_prop_name(style_string['visualProperty'])
     # Verify value and adjust it if necessary
-    style_string['value'] = _validate_prop_value(style_string['visualProperty'], style_string['value'])
+    style_string['value'] = _validate_prop_value(style_string['visualProperty'], style_string['value'], base_url)
 
     # TODO: Should the property name be mapped like in update_style_defaults?
     res = commands.cyrest_put(f'styles/{style_name}/defaults', body=[style_string], base_url=base_url,
                               require_json=False)
     time.sleep(
         MODEL_PROPAGATION_SECS)  # wait for attributes to be applied ... it looks like Cytoscape returns before this is complete [BUG]
     return res
@@ -1797,15 +1797,15 @@
         >>> set_background_color_default('red')
         ''
     """
     style = {'visualProperty': 'NETWORK_BACKGROUND_PAINT', 'value': new_color}
     res = set_visual_property_default(style, style_name, base_url=base_url)
     return res
 
-def _validate_prop_value(prop, prop_val):
+def _validate_prop_value(prop, prop_val, base_url):
     # Check property value to make sure it fits syntax
 
     def none_check(value):
         if value is None:
             raise CyError(f'Property "{prop}" cannot be None. It must be a scalar.',
                       caller=sys._getframe(4).f_code.co_name)
         return value
@@ -1817,19 +1817,19 @@
     if prop in COLOR_PROPERTIES:
         return verify_hex_colors(none_check(prop_val))
     elif prop in DIMENSION_PROPERTIES:
         return verify_dimensions(DIMENSION_PROPERTIES[prop], none_check(prop_val))
     elif prop in OPACITY_PROPERTIES:
         return verify_opacities(none_check(prop_val))
     elif prop in SHAPE_PROPERTIES:
-        return verify_node_shapes(none_check(prop_val), styles.get_node_shapes())
+        return verify_node_shapes(none_check(prop_val), styles.get_node_shapes(base_url=base_url))
     elif prop in LINE_STYLE_PROPERTIES:
-        return verify_edge_shapes(none_check(prop_val), styles.get_line_styles(), 'line style', 'get_line_style')
+        return verify_edge_shapes(none_check(prop_val), styles.get_line_styles(base_url=base_url), 'line style', 'get_line_style')
     elif prop in ARROW_STYLE_PROPERTIES:
-        return verify_edge_shapes(none_check(prop_val), styles.get_arrow_shapes(), 'arrow style', 'get_arrow_shapes')
+        return verify_edge_shapes(none_check(prop_val), styles.get_arrow_shapes(base_url=base_url), 'arrow style', 'get_arrow_shapes')
     elif prop in VISIBLE_PROPERTIES:
         return verify_bools(none_check(prop_val))
     elif prop in LABEL_PROPERTIES | TOOLTIP_PROPERTIES | FONT_FACE_PROPERTIES:
         return verify_strs(none_check(prop_val))
     elif prop in CUSTOM_GRAPHICS_PROPERTIES:
         return prop_val
     else:
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_dependencies.py` & `py4cytoscape-1.8.0/py4cytoscape/style_dependencies.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_mappings.py` & `py4cytoscape-1.8.0/py4cytoscape/style_mappings.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_values.py` & `py4cytoscape-1.8.0/py4cytoscape/style_values.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/style_visual_props.py` & `py4cytoscape-1.8.0/py4cytoscape/style_visual_props.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/styles.py` & `py4cytoscape-1.8.0/py4cytoscape/styles.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/tables.py` & `py4cytoscape-1.8.0/py4cytoscape/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,15 @@
         detail_logger.debug(f'data_subset: {data_subset}')
         raise CyError(f'Provided table key column "{table_key_column}" and data key column "{data_key_column}" do not contain any matches')
 
     # look for elements that are lists (instead of scalars) and turn them into comma-separated strings.
     # Note that CyREST doesn't accept lists or create columns of type list, but comma-separated strings is
     # the best we can do for the user at this time.
     for col in data_subset.columns:
-        col_val = [','.join(val) if isinstance(val, list) else val for val in data_subset[col]]
+        col_val = [','.join([str(list_element)   for list_element in val]) if isinstance(val, list) else val   for val in data_subset[col]]
         data_subset[col] = col_val
 
     # TODO: Find out whether "factors" are an issue in Python, and why factors could be troublesome in R
     # TODO: Verify that this gives the right answer for list of str, int, etc
 
     data_list = _df_to_attr_dict_list(data_subset)  # convert DataFrame to dicts that are easy to convert to JSON
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape/tools.py` & `py4cytoscape-1.8.0/py4cytoscape/tools.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape/user_interface.py` & `py4cytoscape-1.8.0/py4cytoscape/user_interface.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/py4cytoscape.egg-info/PKG-INFO` & `py4cytoscape-1.8.0/py4cytoscape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4cytoscape
-Version: 1.7.0
+Version: 1.8.0
 Summary: Cytoscape Automation API
 Home-page: https://github.com/cytoscape/py4cytoscape
 Author: Barry Demchak
 Author-email: bdemchak@ucsd.edu
 Maintainer: Barry Demchak
 Maintainer-email: bdemchak@ucsd.edu
 License: MIT License
```

### Comparing `py4cytoscape-1.7.0/py4cytoscape.egg-info/SOURCES.txt` & `py4cytoscape-1.8.0/py4cytoscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/setup.py` & `py4cytoscape-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     packages=setuptools.find_packages( exclude=['docker*'] ),
     include_package_data=True,
     setup_requires=['Cython','numpy'],
     install_requires=[
         'pandas',
         'networkx',
         'requests',
-        'python-igraph',
+        'igraph',
         'colorbrewer',
         'chardet',
         'decorator',
         'backoff',
         'colour'
     ],
     classifiers=[
```

### Comparing `py4cytoscape-1.7.0/tests/test_annotations.py` & `py4cytoscape-1.8.0/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_apps.py` & `py4cytoscape-1.8.0/tests/test_apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,28 +102,28 @@
         self.assertIn(APP_NAME, [app['appName'] for app in get_disabled_apps()])
 
         # Verify that the app can be enabled and that it doesn't show up on the disabled list after that
         self.assertDictEqual(enable_app(APP_NAME), {'appName': APP_NAME})
         self.assertSetEqual({app['appName'] for app in get_disabled_apps()}, pre_disabled_app_names)
 
         # Verify that enabling the app again doesn't have any effect
-        self.assertDictEqual(enable_app(APP_NAME), {'appName': APP_NAME})
+        self.assertDictEqual(enable_app(APP_NAME), {'error': f"App '{APP_NAME}' is not disabled"})
         self.assertSetEqual({app['appName'] for app in get_disabled_apps()}, pre_disabled_app_names)
 
         # Uninstall the app just to be clean
         self.assertDictEqual(uninstall_app(APP_NAME), {'appName': APP_NAME})
 
         # Verify that enabling and disabling a non-existent app is caught
-        self.assertDictEqual(enable_app(BAD_APP_NAME), {'appName': BAD_APP_NAME})
+        self.assertDictEqual(enable_app(BAD_APP_NAME), {'error': f"Can't find app '{BAD_APP_NAME}'"})
         self.assertNotIn(BAD_APP_NAME, [app['appName'] for app in get_disabled_apps()])
-        self.assertDictEqual(disable_app(BAD_APP_NAME), {'appName': BAD_APP_NAME})
+        self.assertDictEqual(disable_app(BAD_APP_NAME), {'error': f"Can't find app '{BAD_APP_NAME}'"})
         self.assertNotIn(BAD_APP_NAME, [app['appName'] for app in get_disabled_apps()])
-        self.assertDictEqual(enable_app(EMPTY_APP_NAME), {'appName': EMPTY_APP_NAME})
+        self.assertDictEqual(enable_app(EMPTY_APP_NAME), {'error': f"Can't find app '{EMPTY_APP_NAME}'"})
         self.assertNotIn(EMPTY_APP_NAME, [app['appName'] for app in get_disabled_apps()])
-        self.assertDictEqual(disable_app(EMPTY_APP_NAME), {'appName': EMPTY_APP_NAME})
+        self.assertDictEqual(disable_app(EMPTY_APP_NAME), {'error': f"Can't find app '{EMPTY_APP_NAME}'"})
         self.assertNotIn(EMPTY_APP_NAME, [app['appName'] for app in get_disabled_apps()])
 
     
     @print_entry_exit
     def test_install_uninstall_app(self):
         # Initialization
         APP_NAME = 'boundaryLayout'  # Some app that's unlikely to be already installed
```

### Comparing `py4cytoscape-1.7.0/tests/test_collections.py` & `py4cytoscape-1.8.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_commands.py` & `py4cytoscape-1.8.0/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     def tearDown(self):
         pass
 
     @print_entry_exit
     def test_cyrest_api(self):
         self.assertTrue(cyrest_api())
 
+        time.sleep(10) # This is tricky ... it seems like bad things happen if cyrest_api doesn't wait until completion
+
     @print_entry_exit
     def test_cyrest_delete(self):
         # Initialization
         load_test_session()
 
         # Verify that deleting a view returns a non-JSON result
         self.assertEqual(len(get_network_views()), 1)
@@ -137,14 +139,16 @@
         self.assertRaises(RequestException, cyrest_post, 'networks/views/currentNetworkView',
                           body={'networkViewSUID': view}, base_url='http://yahoo.com')
 
     @print_entry_exit
     def test_commands_api(self):
         self.assertTrue(commands_api())
 
+        time.sleep(10) # This is tricky ... it seems like bad things happen if commands_api doesn't wait until completion
+
     @print_entry_exit
     def test_commands_get(self):
         # Verify the expected return from common commands
         self._check_cy_result(commands_get('command sleep duration=5'), [])
         self._check_cy_result(commands_get(''),
                               ['Available namespaces:', 'analyzer', 'apps', 'command', 'cybrowser', 'cychart',
                                'diffusion', 'edge', 'filter', 'group', 'idmapper', 'layout', 'network', 'node',
```

### Comparing `py4cytoscape-1.7.0/tests/test_cy_ndex.py` & `py4cytoscape-1.8.0/tests/test_cy_ndex.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_cytoscape_system.py` & `py4cytoscape-1.8.0/tests/test_cytoscape_system.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_filters.py` & `py4cytoscape-1.8.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_groups.py` & `py4cytoscape-1.8.0/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_layouts.py` & `py4cytoscape-1.8.0/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_network_selection.py` & `py4cytoscape-1.8.0/tests/test_network_selection.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_network_views.py` & `py4cytoscape-1.8.0/tests/test_network_views.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_networks.py` & `py4cytoscape-1.8.0/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_py4cytoscape_utils.py` & `py4cytoscape-1.8.0/tests/test_py4cytoscape_utils.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_sandbox.py` & `py4cytoscape-1.8.0/tests/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_sanity.py` & `py4cytoscape-1.8.0/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_session.py` & `py4cytoscape-1.8.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_auto_mappings.py` & `py4cytoscape-1.8.0/tests/test_style_auto_mappings.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_bypasses.py` & `py4cytoscape-1.8.0/tests/test_style_bypasses.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_defaults.py` & `py4cytoscape-1.8.0/tests/test_style_defaults.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_dependencies.py` & `py4cytoscape-1.8.0/tests/test_style_dependencies.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_mappings.py` & `py4cytoscape-1.8.0/tests/test_style_mappings.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_style_values.py` & `py4cytoscape-1.8.0/tests/test_style_values.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_styles.py` & `py4cytoscape-1.8.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_tables.py` & `py4cytoscape-1.8.0/tests/test_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -316,34 +316,44 @@
 
         # Verify that newcol_val column and derived were added, and that derived has values only for the newcol nodes
         check_values_added(column_names_string_keyed, 'name', test_data_string_keyed, 'id_e', 'newcol_e', table='edge')
 
         # Verify that adding a column with a null works properly, and that adding columns of different types does, too
         # While we're at it, eyeball the running time to see that it's not crazy slow
         test_data_suid_name = get_table_columns(columns=['SUID', 'name'])
-        test_data_suid_name['IntCol'] = test_data_suid_name['SUID']
-        test_data_suid_name['StrCol'] = test_data_suid_name['SUID']
-        test_data_suid_name['FloatCol'] = test_data_suid_name['SUID']
+        suid_list = test_data_suid_name['SUID']
+        test_data_suid_name['IntCol'] = suid_list
+        test_data_suid_name['StrCol'] = suid_list
+        test_data_suid_name['FloatCol'] = suid_list
         test_data_suid_name = test_data_suid_name.astype({'IntCol': np.int64, 'StrCol': np.str_, 'FloatCol': np.float_})
+        test_data_suid_name['ListIntCol'] = [[int(suid), int(suid), int(suid)]   for suid in suid_list]
+        test_data_suid_name['ListFloatCol'] = [[float(suid), float(suid), float(suid)]   for suid in suid_list]
+        test_data_suid_name['ListStrCol'] = [[str(suid), str(suid), str(suid)]   for suid in suid_list]
+        test_data_suid_name['ListBoolCol'] = [[True, False, True]   for suid in suid_list]
         suid_YBL079W = test_data_suid_name.index[test_data_suid_name.name == 'YBL079W'][0]
         del test_data_suid_name['name']
-        test_data_suid_name.at[suid_YBL079W, 'FloatCol'] = np.nan # used to be set_value, but it was deprecated
-#        test_data_suid_name.set_value(suid_YBL079W, 'FloatCol', np.nan)
+        test_data_suid_name.at[suid_YBL079W, 'FloatCol'] = np.nan
+        test_data_suid_name.at[suid_YBL079W, 'ListFloatCol'] = [np.nan, 1.23, np.nan]
         res = load_table_data(test_data_suid_name, data_key_column='SUID', table_key_column='SUID')
         self.assertEqual(res, 'Success: Data loaded in defaultnode table')
         # Make sure that Cytoscape got all of the column types and values right, including the NAN
-        t = get_table_columns(columns=['SUID', 'IntCol', 'StrCol', 'FloatCol'])
-        for suid, intcol, strcol, floatcol in zip(t['SUID'], t['IntCol'], t['StrCol'], t['FloatCol']):
+        t = get_table_columns(columns=['SUID', 'IntCol', 'StrCol', 'FloatCol', 'ListIntCol', 'ListFloatCol', 'ListStrCol', 'ListBoolCol'])
+        for suid, intcol, strcol, floatcol, list_int_col, list_float_col, list_str_col, list_bool_col in zip(t['SUID'], t['IntCol'], t['StrCol'], t['FloatCol'], t['ListIntCol'], t['ListFloatCol'], t['ListStrCol'], t['ListBoolCol']):
             str_suid = str(suid)
             self.assertEqual(str_suid, str(intcol))
             self.assertEqual(str_suid, strcol)
+            self.assertEqual(','.join([str(int(suid)), str(int(suid)), str(int(suid))]), list_int_col)
+            self.assertEqual(','.join([str(suid), str(suid), str(suid)]), list_str_col)
+            self.assertEqual('True,False,True', list_bool_col)
             if suid == suid_YBL079W:
                 self.assertTrue(np.isnan(floatcol))
+                self.assertEqual(list_float_col, 'nan,1.23,nan')
             else:
                 self.assertEqual(str_suid, str(int(floatcol)))
+                self.assertEqual(','.join([str(float(suid)), str(float(suid)), str(float(suid))]), list_float_col)
 
         data = get_table_columns()
         self.assertRaises(CyError, load_table_data, data, table='bogus')
         self.assertRaises(CyError, load_table_data, data, namespace='bogus')
         self.assertRaises(CyError, load_table_data, data, network='bogus')
```

### Comparing `py4cytoscape-1.7.0/tests/test_tools.py` & `py4cytoscape-1.8.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `py4cytoscape-1.7.0/tests/test_user_interface.py` & `py4cytoscape-1.8.0/tests/test_user_interface.py`

 * *Files identical despite different names*

