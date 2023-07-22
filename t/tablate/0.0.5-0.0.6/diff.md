# Comparing `tmp/tablate-0.0.5.tar.gz` & `tmp/tablate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablate-0.0.5.tar", last modified: Thu Jul 20 21:58:05 2023, max compression
+gzip compressed data, was "tablate-0.0.6.tar", last modified: Sat Jul 22 12:55:58 2023, max compression
```

## Comparing `tablate-0.0.5.tar` & `tablate-0.0.6.tar`

### file list

```diff
@@ -1,100 +1,136 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.972311 tablate-0.0.5/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.5/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 21:58:05.972311 tablate-0.0.5/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 tablate-0.0.5/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-20 21:58:00.000000 tablate-0.0.5/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-20 21:58:05.972311 tablate-0.0.5/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.959311 tablate-0.0.5/tablate/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      117 2023-07-19 10:35:23.000000 tablate-0.0.5/tablate/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.961311 tablate-0.0.5/tablate/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    10270 2023-07-20 21:18:19.000000 tablate-0.0.5/tablate/api/Tablate.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.5/tablate/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.962311 tablate-0.0.5/tablate/characters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.5/tablate/characters/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.5/tablate/characters/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.5/tablate/characters/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.962311 tablate-0.0.5/tablate/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.5/tablate/helpers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/calcs/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.5/tablate/helpers/calcs/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-19 21:31:48.000000 tablate-0.0.5/tablate/helpers/calcs/calc_column_percent.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.5/tablate/helpers/calcs/calc_column_widths.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.5/tablate/helpers/calcs/get_row_colspan.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-19 22:13:11.000000 tablate-0.0.5/tablate/helpers/calcs/random_string.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/checkers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.5/tablate/helpers/checkers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.5/tablate/helpers/checkers/is_last_element.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/formatters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.5/tablate/helpers/formatters/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.964311 tablate-0.0.5/tablate/helpers/formatters/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.5/tablate/helpers/formatters/console/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.5/tablate/helpers/formatters/console/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      539 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/formatters/console/row_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3160 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/formatters/console/row_divider.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.964311 tablate-0.0.5/tablate/helpers/formatters/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.5/tablate/helpers/formatters/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/element/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:39.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/row.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:34.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/style/border/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:38.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:51.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_bottom.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:46:57.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_right.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_style.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      211 2023-07-20 10:49:54.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/selector.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.966311 tablate-0.0.5/tablate/helpers/formatters/html/style/text/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:34.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/alignment.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/multiline.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:48:28.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/overflow.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:12:25.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/padding.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.966311 tablate-0.0.5/tablate/helpers/renderers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.5/tablate/helpers/renderers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.967311 tablate-0.0.5/tablate/helpers/renderers/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.5/tablate/helpers/renderers/console/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.968311 tablate-0.0.5/tablate/helpers/renderers/console/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2113 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2530 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_frame_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3869 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1936 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      800 2023-07-20 14:55:25.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2320 2023-07-20 14:45:23.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      777 2023-07-20 14:55:25.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.969311 tablate-0.0.5/tablate/helpers/renderers/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.5/tablate/helpers/renderers/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.970311 tablate-0.0.5/tablate/helpers/renderers/html/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      277 2023-07-19 20:38:22.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1375 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_body.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1023 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_head.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:50:17.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      760 2023-07-20 10:18:01.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1157 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.970311 tablate-0.0.5/tablate/helpers/validators/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.5/tablate/helpers/validators/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.971311 tablate-0.0.5/tablate/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 00:45:20.000000 tablate-0.0.5/tablate/tests/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       14 2023-07-20 14:52:15.000000 tablate-0.0.5/tablate/tests/blah.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3528 2023-07-20 14:50:58.000000 tablate-0.0.5/tablate/tests/test_decs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8057 2023-07-20 00:01:38.000000 tablate-0.0.5/tablate/tests/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       67 2023-07-19 10:35:23.000000 tablate-0.0.5/tablate/tests/test_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-20 21:47:24.000000 tablate-0.0.5/tablate/tests/test_text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.971311 tablate-0.0.5/tablate/type/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.5/tablate/type/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2473 2023-07-20 09:49:58.000000 tablate-0.0.5/tablate/type/dict_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1281 2023-07-20 21:47:24.000000 tablate-0.0.5/tablate/type/dict_input.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      538 2023-07-20 13:47:58.000000 tablate-0.0.5/tablate/type/dict_options.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.5/tablate/type/primitives.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.960311 tablate-0.0.5/tablate.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3173 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.573204 tablate-0.0.6/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.6/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      509 2023-07-22 12:55:58.572204 tablate-0.0.6/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:33:05.000000 tablate-0.0.6/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      583 2023-07-22 12:54:43.000000 tablate-0.0.6/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-22 12:55:58.573204 tablate-0.0.6/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.556204 tablate-0.0.6/tablate/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      117 2023-07-19 10:35:23.000000 tablate-0.0.6/tablate/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.557204 tablate-0.0.6/tablate/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     9502 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/Tablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.6/tablate/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.557204 tablate-0.0.6/tablate/api/classes/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 01:25:25.000000 tablate-0.0.6/tablate/api/classes/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.558204 tablate-0.0.6/tablate/api/classes/modules/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:16:24.000000 tablate-0.0.6/tablate/api/classes/modules/Grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:16:19.000000 tablate-0.0.6/tablate/api/classes/modules/Table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:16:13.000000 tablate-0.0.6/tablate/api/classes/modules/Text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.6/tablate/api/classes/modules/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.558204 tablate-0.0.6/tablate/api/classes/options/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.6/tablate/api/classes/options/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.558204 tablate-0.0.6/tablate/api/classes/options/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.6/tablate/api/classes/options/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.559204 tablate-0.0.6/tablate/api/classes/options/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4480 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/StyleCss.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.6/tablate/api/classes/options/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.559204 tablate-0.0.6/tablate/api/classes/options/html/style/mixins/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      508 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/mixins/AddStyleMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      519 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/mixins/ClassNameMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 01:07:40.000000 tablate-0.0.6/tablate/api/classes/options/html/style/mixins/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.559204 tablate-0.0.6/tablate/api/classes/options/html/style/subclasses/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2430 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/subclasses/ElementStyle.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      591 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/subclasses/TableStyle.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      682 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/subclasses/TextStyle.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.6/tablate/api/classes/options/html/style/subclasses/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.560204 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 15:13:12.000000 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      231 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/base_names.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2285 2023-07-22 08:57:04.000000 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/css_factory.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      880 2023-07-22 08:57:04.000000 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/selectors.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      885 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/api/classes/options/html/style/utilities/style_dict.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.560204 tablate-0.0.6/tablate/api/functions/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.6/tablate/api/functions/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:16:43.000000 tablate-0.0.6/tablate/api/functions/concat.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.562204 tablate-0.0.6/tablate/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.6/tablate/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.6/tablate/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.6/tablate/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.6/tablate/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.6/tablate/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.6/tablate/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.562204 tablate-0.0.6/tablate/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.6/tablate/helpers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.563204 tablate-0.0.6/tablate/helpers/calcs/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.6/tablate/helpers/calcs/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      769 2023-07-21 00:44:07.000000 tablate-0.0.6/tablate/helpers/calcs/calc_column_percent.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.6/tablate/helpers/calcs/calc_column_widths.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.6/tablate/helpers/calcs/get_row_colspan.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-19 22:13:11.000000 tablate-0.0.6/tablate/helpers/calcs/random_string.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.563204 tablate-0.0.6/tablate/helpers/checkers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.6/tablate/helpers/checkers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.6/tablate/helpers/checkers/is_last_element.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.564204 tablate-0.0.6/tablate/helpers/formatters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.6/tablate/helpers/formatters/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.565204 tablate-0.0.6/tablate/helpers/formatters/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.6/tablate/helpers/formatters/console/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.6/tablate/helpers/formatters/console/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      539 2023-07-20 09:59:11.000000 tablate-0.0.6/tablate/helpers/formatters/console/row_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3160 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/formatters/console/row_divider.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.565204 tablate-0.0.6/tablate/helpers/formatters/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.6/tablate/helpers/formatters/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.565204 tablate-0.0.6/tablate/helpers/formatters/html/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.6/tablate/helpers/formatters/html/element/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      721 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/formatters/html/element/column.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      490 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/formatters/html/element/frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      115 2023-07-22 11:20:40.000000 tablate-0.0.6/tablate/helpers/formatters/html/element/row.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      279 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/formatters/html/element/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.566204 tablate-0.0.6/tablate/helpers/formatters/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/border_style.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.566204 tablate-0.0.6/tablate/helpers/formatters/html/style/elements/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:02:02.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/elements/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      710 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/elements/column_style.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      515 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/elements/frame_style.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      764 2023-07-22 12:24:01.000000 tablate-0.0.6/tablate/helpers/formatters/html/style/elements/text_style.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.567204 tablate-0.0.6/tablate/helpers/renderers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.6/tablate/helpers/renderers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.567204 tablate-0.0.6/tablate/helpers/renderers/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.6/tablate/helpers/renderers/console/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.568204 tablate-0.0.6/tablate/helpers/renderers/console/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.6/tablate/helpers/renderers/console/frames/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2113 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/frames/render_console_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2530 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/frames/render_console_frame_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3869 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/frames/render_string_frame_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1936 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/frames/render_string_frame_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      765 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/render_console.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      800 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/render_console_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2320 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/render_console_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      777 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/console/render_console_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.569204 tablate-0.0.6/tablate/helpers/renderers/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.6/tablate/helpers/renderers/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.569204 tablate-0.0.6/tablate/helpers/renderers/html/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3028 2023-07-22 12:45:12.000000 tablate-0.0.6/tablate/helpers/renderers/html/frames/render_html_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6154 2023-07-22 12:23:41.000000 tablate-0.0.6/tablate/helpers/renderers/html/frames/render_html_table_body.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2536 2023-07-22 12:50:37.000000 tablate-0.0.6/tablate/helpers/renderers/html/frames/render_html_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1267 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/html/render_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.6/tablate/helpers/renderers/html/render_html_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1696 2023-07-22 12:48:53.000000 tablate-0.0.6/tablate/helpers/renderers/html/render_html_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1779 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/helpers/renderers/html/render_html_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.569204 tablate-0.0.6/tablate/helpers/validators/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.6/tablate/helpers/validators/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.570204 tablate-0.0.6/tablate/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 00:41:48.000000 tablate-0.0.6/tablate/tests/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.571204 tablate-0.0.6/tablate/tests/playpen/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:20:57.000000 tablate-0.0.6/tablate/tests/playpen/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      335 2023-07-21 12:33:50.000000 tablate-0.0.6/tablate/tests/playpen/class.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      516 2023-07-22 01:36:08.000000 tablate-0.0.6/tablate/tests/playpen/class_0.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      170 2023-07-21 11:38:53.000000 tablate-0.0.6/tablate/tests/playpen/class_1.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      171 2023-07-21 10:41:14.000000 tablate-0.0.6/tablate/tests/playpen/class_2.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3569 2023-07-22 12:51:12.000000 tablate-0.0.6/tablate/tests/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8057 2023-07-20 00:01:38.000000 tablate-0.0.6/tablate/tests/test_objs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 05:05:56.000000 tablate-0.0.6/tablate/tests/test_out_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.6/tablate/tests/test_out_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      955 2023-07-22 04:54:36.000000 tablate-0.0.6/tablate/tests/test_styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.572204 tablate-0.0.6/tablate/type/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.6/tablate/type/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.6/tablate/type/primitives.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2385 2023-07-22 10:49:03.000000 tablate-0.0.6/tablate/type/type_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      156 2023-07-22 12:45:12.000000 tablate-0.0.6/tablate/type/type_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      626 2023-07-20 23:50:14.000000 tablate-0.0.6/tablate/type/type_input.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      714 2023-07-22 01:36:07.000000 tablate-0.0.6/tablate/type/type_options.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1024 2023-07-22 08:41:42.000000 tablate-0.0.6/tablate/type/type_style.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:55:58.557204 tablate-0.0.6/tablate.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      509 2023-07-22 12:55:58.000000 tablate-0.0.6/tablate.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4411 2023-07-22 12:55:58.000000 tablate-0.0.6/tablate.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-22 12:55:58.000000 tablate-0.0.6/tablate.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-22 12:55:58.000000 tablate-0.0.6/tablate.egg-info/top_level.txt
```

### Comparing `tablate-0.0.5/LICENCE` & `tablate-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/pyproject.toml` & `tablate-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablate"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII plain text table renderer."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-
 [project.urls]
-"Homepage" = "https://gitlab.com/guydewinton/textframe"
-"Bug Tracker" = "https://gitlab.com/guydewinton/textframe/issues"
+"Homepage" = "https://gitlab.com/guydewinton/tablate"
+"Bug Tracker" = "https://gitlab.com/guydewinton/tablate/issues"
```

### Comparing `tablate-0.0.5/tablate/api/Tablate.py` & `tablate-0.0.6/tablate/api/Tablate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 import copy
 import shutil
 from typing import List, Dict, Optional, Union
 
-from tablate.helpers.calcs.calc_column_percent import calc_column_percent
 from tablate.helpers.calcs.calc_column_widths import calc_column_widths
-from tablate.helpers.calcs.random_string import random_string
-from tablate.helpers.renderers.console.render_console_foot import render_console_foot
-from tablate.helpers.renderers.console.render_console_frames import render_console_frames
-from tablate.helpers.renderers.console.render_console_head import render_console_head
-from tablate.helpers.renderers.html.render_html_head import render_html_head
-from tablate.type.dict_frame import TextFrameDict, GridFrameDict, TableRowsFrameDict, \
+from tablate.helpers.renderers.console.render_console import render_console
+from tablate.helpers.renderers.html.render_html import render_html
+from tablate.type.type_frame import TextFrameDict, GridFrameDict, TableRowsFrameDict, \
     TableHeadColumnFrameDict, TableRowsColumnFrameDict, TableHeadFrameDict, FrameDictList
-from tablate.type.dict_options import Options
-from tablate.type.dict_input import GridInputColumnDict, TableInputColumnDict
+from tablate.type.type_options import Options
+from tablate.type.type_input import GridInputColumnDict, TableInputColumnDict
 from tablate.type.primitives import Border, BaseDivider, TextAlignment, ColumnDivider, HeaderAlignment, \
     HeaderColumnDivider
 
 
 class Tablate:
 
     # todo: maybe allow align/padding/frame_divider defaults in constructor??
     # todo: allow frame names (will make TextFrame iPython friendly) -- also constructor options `show_frame_names` & `frame_name_align`
     # todo: allow cell level definition of padding/v_line/trunc_value in `add_` constructor objects??? => a lot of fuss and complication for marginal use... v_lines might be useful...
 
     # todo: text styles / colours
 
+    # todo: css injector class / closure to remove all the messy += statements
+    # todo: create options class... (make everything betterer??? maybe... maybe not...)
+
     def __init__(self,
                  border_style: Border = "thick",
                  frame_padding: int = 1, # todo: allow padding definition for all sides => int: all sides, string: css style ('0' or '0 0' or '0 0 0 0') // dict: {"top", "bottom", "left", "right"} // three input methods
                  frame_divider: BaseDivider = "thick",
                  frame_width: int = None,
                  html_px_size: int = 6,
                  html_text_size: int = 12,
                  html_frame_width: str = "100%",
-                 html_css_injection: str = ""):
+                 html_css_injection: str = "") -> None:
 
         self._options: Options = {
             "common": {
                 "border_style": border_style,
                 "frame_padding": frame_padding,
                 "frame_divider": frame_divider,
                 "frame_width": frame_width if frame_width else shutil.get_terminal_size((120 + (frame_padding * 2), 0))[
                                                                    0] - (frame_padding * 2)
             },
             "html": {
                 "px_size": html_px_size,
                 "text_size": html_text_size,
                 "width": html_frame_width,
-                "css": html_css_injection,
             }
         }
 
         self._frame_list: FrameDictList = []
 
-
     def add_text_frame(self,
                        text: Union[str, int, float],
                        multiline: bool = True,
                        max_lines: Optional[int] = None,
                        text_align: TextAlignment = "left",
                        text_padding: int = 1,
                        frame_base_divider: BaseDivider = "thick",
-                       trunc_value: str = "..."):
+                       trunc_value: str = "...") -> None:
 
         text_frame_dict: TextFrameDict = {
             "type": "text",
             "column_list": [{"width": self._options["common"]["frame_width"] - 2, "divider": "blank"}],
             "string": text,
             "base_divider": frame_base_divider,
             "max_lines": max_lines,
@@ -80,15 +77,15 @@
     def add_grid_frame(self,
                        columns: List[Union[str, GridInputColumnDict]],
                        column_padding: int = 1,
                        column_divider: ColumnDivider = "thin",
                        frame_base_divider: BaseDivider = "thick",
                        multiline: bool = True,
                        max_lines: int = None,
-                       trunc_value: str = "..."):
+                       trunc_value: str = "...") -> None:
 
         columns = copy.deepcopy(columns)
 
         grid_column_list = []
 
         for grid_column_item in columns:
             if type(grid_column_item) == str:
@@ -133,15 +130,15 @@
                         header_base_divider: BaseDivider = "thick",
                         multiline: bool = False,
                         max_lines: int = None,
                         multiline_header: bool = False,
                         max_lines_header: int = None,
                         hide_header: bool = False,
                         head_trunc_value: str = ".",
-                        row_trunc_value: str = "..."):
+                        row_trunc_value: str = "...") -> None:
 
         columns = copy.deepcopy(columns)
         rows = copy.deepcopy(rows)
 
         columns = calc_column_widths(columns=columns, frame_width=self._options["common"]["frame_width"], column_padding=column_padding)
 
         header_column_list = []
@@ -199,35 +196,23 @@
             "base_divider": frame_base_divider,
             "max_lines": max_lines,
             "multiline": multiline
         }
 
         self._frame_list.append(rows_frame_dict)
 
-    def to_string(self):
-        return_string = ""
-        if len(self._frame_list) > 0:
-            return_string += render_console_head(frame_list=self._frame_list, options=self._options)
-            return_string += render_console_frames(frame_list=self._frame_list, options=self._options)
-            return_string += render_console_foot(frame_list=self._frame_list, options=self._options)
-        return return_string
+    def to_string(self) -> str:
+        return render_console(frame_list=self._frame_list, options=self._options)
 
-    def print(self):
+    def print(self) -> None:
         print(self.to_string())
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.to_string()
 
-    def to_html(self):
-        self._options["html"]["uid"] = random_string(6)
-        frame_list, self._options["html"]["column_widths"] = calc_column_percent(frame_list=self._frame_list,
-                                                                                 frame_width=self._options["common"]["frame_width"])
-
-        return_html = ""
-
-        return_html += render_html_head(options=self._options)
-
+    def to_html(self) -> str:
+        return render_html(frame_list=self._frame_list, options=self._options)
 
-    def _repr_html_(self):
+    def _repr_html_(self) -> str:
         return self.to_html()
```

### Comparing `tablate-0.0.5/tablate/characters/matrix_cross.py` & `tablate-0.0.6/tablate/characters/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/characters/matrix_side.py` & `tablate-0.0.6/tablate/characters/matrix_side.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/helpers/calcs/calc_column_widths.py` & `tablate-0.0.6/tablate/helpers/calcs/calc_column_widths.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/helpers/calcs/get_row_colspan.py` & `tablate-0.0.6/tablate/helpers/calcs/get_row_colspan.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/helpers/formatters/console/cell_string.py` & `tablate-0.0.6/tablate/helpers/formatters/console/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/helpers/formatters/console/row_border.py` & `tablate-0.0.6/tablate/helpers/formatters/console/row_border.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/helpers/formatters/console/row_divider.py` & `tablate-0.0.6/tablate/helpers/formatters/console/row_divider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
 from tablate.characters.line_h import h_line
 from tablate.characters.matrix_cross import cross_matrix
-from tablate.type.dict_options import Options
+from tablate.type.type_options import Options
 from tablate.type.primitives import BaseDivider
 
 
 def row_divider(column_list_top: list, column_list_bottom: list, divider: BaseDivider) -> str:
 
     """
     :param divider: BorderType
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_columns.py` & `tablate-0.0.6/tablate/helpers/renderers/console/frames/render_console_columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from tablate.characters.line_v import v_line
 from tablate.helpers.checkers.is_last_element import is_last_element
 from tablate.helpers.formatters.console.cell_string import cell_string_multi_line, cell_string_single_line
 from tablate.helpers.formatters.console.row_border import row_border
-from tablate.type.dict_frame import BaseFrameDict
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import BaseFrameDict
+from tablate.type.type_options import Options
 from tablate.type.primitives import Border
 
 
 def column_console_multiline(formatted_columns_array: List[List[str]], frame_dict: BaseFrameDict, options: Options):
 
     frame_padding = options["common"]["frame_padding"]
     frame_border = options["common"]["border_style"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_frame_grid.py` & `tablate-0.0.6/tablate/helpers/renderers/console/frames/render_console_frame_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from tablate.characters.line_v import v_line
 from tablate.helpers.checkers.is_last_element import is_last_element
 from tablate.helpers.formatters.console.cell_string import cell_string_single_line, cell_string_multi_line
 from tablate.helpers.renderers.console.frames.render_console_columns import column_console_multiline
 from tablate.helpers.formatters.console.row_border import row_border
-from tablate.type.dict_frame import GridFrameDict
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import GridFrameDict
+from tablate.type.type_options import Options
 from tablate.type.primitives import Border
 
 
 def render_console_single_line_grid(grid_frame_dict: GridFrameDict, options: Options):
 
     frame_padding = options["common"]["frame_padding"]
     frame_border = options["common"]["border_style"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_table.py` & `tablate-0.0.6/tablate/helpers/renderers/console/frames/render_string_frame_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tablate.characters.line_v import v_line
 from tablate.helpers.checkers.is_last_element import is_last_element
 from tablate.helpers.formatters.console.cell_string import cell_string_single_line, cell_string_multi_line
 from tablate.helpers.renderers.console.frames.render_console_columns import column_console_multiline
 from tablate.helpers.formatters.console.row_divider import row_divider
 from tablate.helpers.formatters.console.row_border import row_border
-from tablate.type.dict_frame import TableRowsFrameDict
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import TableRowsFrameDict
+from tablate.type.type_options import Options
 from tablate.type.primitives import Border
 
 
 def render_console_table_frame(table_frame_dict: TableRowsFrameDict, options: Options) -> str:
 
     frame_padding = options["common"]["frame_padding"]
     frame_border = options["common"]["border_style"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_text.py` & `tablate-0.0.6/tablate/helpers/renderers/console/frames/render_string_frame_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tablate.helpers.formatters.console.cell_string import cell_string_multi_line, cell_string_single_line
 from tablate.helpers.formatters.console.row_border import row_border
-from tablate.type.dict_frame import TextFrameDict
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import TextFrameDict
+from tablate.type.type_options import Options
 from tablate.type.primitives import Border
 
 
 def render_console_text_frame(text_frame_dict: TextFrameDict, options: Options) -> str:
 
     frame_padding = options["common"]["frame_padding"]
     frame_border = options["common"]["border_style"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/render_console_foot.py` & `tablate-0.0.6/tablate/helpers/renderers/console/render_console_foot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tablate.characters.corners import bottom_left, bottom_right
 from tablate.helpers.formatters.console.row_divider import row_divider
-from tablate.type.dict_frame import FrameDictList
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import FrameDictList
+from tablate.type.type_options import Options
 
 
 def render_console_foot(frame_list: FrameDictList, options: Options) -> str:
 
     return_string = ""
 
     frame_padding = options["common"]["frame_padding"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/render_console_frames.py` & `tablate-0.0.6/tablate/helpers/renderers/console/render_console_frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from tablate.helpers.checkers.is_last_element import is_last_element
 from tablate.helpers.formatters.console.row_divider import row_divider
 from tablate.helpers.formatters.console.row_border import row_border
 from tablate.helpers.renderers.console.frames.render_console_frame_grid import render_console_single_line_grid, \
     render_console_multi_line_grid
 from tablate.helpers.renderers.console.frames.render_string_frame_table import render_console_table_frame
 from tablate.helpers.renderers.console.frames.render_string_frame_text import render_console_text_frame
-from tablate.type.dict_frame import FrameDictList
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import FrameDictList
+from tablate.type.type_options import Options
 
 
 def render_console_frames(frame_list: FrameDictList, options: Options) -> str:
 
     return_string = ""
 
     frame_padding = options["common"]["frame_padding"]
```

### Comparing `tablate-0.0.5/tablate/helpers/renderers/console/render_console_head.py` & `tablate-0.0.6/tablate/helpers/renderers/console/render_console_head.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tablate.characters.corners import top_left, top_right
 from tablate.helpers.formatters.console.row_divider import row_divider
-from tablate.type.dict_frame import FrameDictList
-from tablate.type.dict_options import Options
+from tablate.type.type_frame import FrameDictList
+from tablate.type.type_options import Options
 
 
 def render_console_head(frame_list: FrameDictList, options: Options) -> str:
 
     return_string = ""
 
     frame_border = options["common"]["border_style"]
```

### Comparing `tablate-0.0.5/tablate/tests/test_decs.py` & `tablate-0.0.6/tablate/tests/test_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tablate as tf
-from tablate.tests.test_defs import column_list1, row_list1, column_list2a, row_list2, column_list2b, column_list2c, \
+from tablate.tests.test_objs import column_list1, row_list1, column_list2a, row_list2, column_list2b, column_list2c, \
     column_list3, column_list4, column_list5, really_long_string
 
-new_frame = tf.Tablate(border_style="thin", frame_padding=6)
+# new_frame = tf.Tablate(border_style="thin", frame_padding=6)
+new_frame = tf.Tablate()
+
 
 new_frame.add_table_frame(column_list1, row_list1)
 
 new_frame.add_table_frame(column_list1, row_list1, multiline=True)
 new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=3)
 new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=6)
 new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=100)
@@ -20,20 +22,20 @@
 
 new_frame.add_text_frame("Default text")
 
 new_frame.add_text_frame(really_long_string)
 new_frame.add_text_frame(really_long_string, multiline=True)
 
 new_frame.add_text_frame(really_long_string, multiline=False)
-new_frame.add_text_frame(really_long_string, max_lines=6)
+new_frame.add_text_frame(really_long_string, max_lines=3)
 
-new_frame.add_text_frame(really_long_string, multiline=True, max_lines=6)
+new_frame.add_text_frame(really_long_string, multiline=True, max_lines=3)
 new_frame.add_text_frame(really_long_string, multiline=True, max_lines=100)
 
-new_frame.add_text_frame(really_long_string, multiline=False, max_lines=6)
+new_frame.add_text_frame(really_long_string, multiline=False, max_lines=3)
 new_frame.add_text_frame(really_long_string, multiline=False, max_lines=100)
 
 new_frame.add_text_frame("Example text frame with left indentation", multiline=False,text_align="left", max_lines=100)
 new_frame.add_text_frame("Example text frame with center indentation", multiline=False,text_align="center")
 new_frame.add_text_frame("Example text frame with right indentation", multiline=False,text_align="right")
 
 new_frame.add_text_frame(666)
@@ -53,15 +55,15 @@
 new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thin", row_line_divider="thin", header_base_divider="thin", header_column_divider="double", frame_base_divider="thick")
 new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thick", row_line_divider="thick", header_base_divider="thick", header_column_divider="double", frame_base_divider="thin")
 
 new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="double", row_line_divider="double", header_base_divider="double", header_column_divider="double", frame_base_divider="none")
 new_frame.add_table_frame(column_list2c, row_list2)
 
 new_frame.add_grid_frame(column_list3, max_lines=1)
+new_frame.add_grid_frame(column_list4, max_lines=6)
 new_frame.add_grid_frame(column_list4, max_lines=100)
-new_frame.add_grid_frame(column_list4)
 new_frame.add_grid_frame(column_list5)
 
 some_set = {1,2,3}
 some_set.add(1)
 
 some_set.add(4)
```

### Comparing `tablate-0.0.5/tablate/tests/test_defs.py` & `tablate-0.0.6/tablate/tests/test_objs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.5/tablate/type/dict_frame.py` & `tablate-0.0.6/tablate/type/type_frame.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,80 @@
 from typing import Literal, TypedDict, Union, List, Dict, Generic, TypeVar
 
 from tablate.type.primitives import TextAlignment, BaseDivider, ColumnDivider
 
 ########################################################################################################################
-### FrameDicts #########################################################################################################
+# FrameDicts ###########################################################################################################
 ########################################################################################################################
 
 
 T = TypeVar('T')
 
+class BaseColumnDict(TypedDict):
+    width: Union[int, str]
+    divider: BaseDivider
+
+
 class BaseFrameDict(TypedDict, Generic[T]):
     column_list: List[T]
     base_divider: BaseDivider
     max_lines: Union[int, None]
     multiline: bool
 
-### Text FrameDict #####################################################################################################
+# Text FrameDict #######################################################################################################
+
+
+class TextBoxColumnDict(BaseColumnDict):
+    pass
 
-class TextBoxColumnDict(TypedDict):
-    width: Union[int, str]
-    divider: BaseDivider
 
 class TextFrameDict(BaseFrameDict[TextBoxColumnDict]):
     type: Literal["text"]
     string: Union[str, int, float]
     align: TextAlignment
     padding: int
     trunc_value: str
 
 
-### Grid FrameDict #####################################################################################################
+# Grid FrameDict #######################################################################################################
 
 
-class GridColumnFrameDict(TypedDict):
-    width: Union[int, str]
-    divider: BaseDivider
+class GridColumnFrameDict(BaseColumnDict):
     string: Union[str, int, float]
     align: TextAlignment
     padding: int
     trunc_value: str
 
+
 class GridFrameDict(BaseFrameDict[GridColumnFrameDict]):
     type: Literal["grid"]
 
 
-### Table FrameDict ####################################################################################################
+# Table FrameDict ######################################################################################################
 
-class TableHeadColumnFrameDict(TypedDict):
-    width: Union[int, str]
-    divider: ColumnDivider
+class TableHeadColumnFrameDict(BaseColumnDict):
     string: Union[str, int, float]
     align: TextAlignment
     padding: int
     trunc_value: str
 
+
 class TableHeadFrameDict(BaseFrameDict[GridColumnFrameDict]):
     type: Literal["table-head"]
 
-class TableRowsColumnFrameDict(TypedDict):
-    width: Union[int, str]
-    divider: BaseDivider
+
+class TableRowsColumnFrameDict(BaseColumnDict):
     key: str
     align: TextAlignment
     padding: int
     trunc_value: str
 
+
 class TableRowsFrameDict(BaseFrameDict[GridColumnFrameDict]):
     type: Literal["table-body"]
     table_row_list: List[Dict[str, Union[str, int, float]]]
     row_line_divider: BaseDivider
 
 
-### FrameDict List #####################################################################################################
+# FrameDict List #######################################################################################################
 
 FrameDictList = List[Union[TextFrameDict, GridFrameDict, TableHeadFrameDict, TableRowsFrameDict]]
```

### Comparing `tablate-0.0.5/tablate/type/dict_options.py` & `tablate-0.0.6/tablate/type/type_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from typing import TypedDict, Union, NotRequired, List
 
+from tablate.api.classes.options.html.style.StyleCss import StyleCss
 from tablate.type.primitives import Border, BaseDivider
 
 
 class CommonOptions(TypedDict):
     border_style: Border
     frame_padding: int
     frame_divider: BaseDivider
     frame_width: int
 
+
 class ConsoleOptions(TypedDict):
     pass
 
+
+class CssDict(TypedDict):
+    head: NotRequired[str]
+    foot: NotRequired[str]
+
+
 class HtmlOptions(TypedDict):
     px_size: int
     text_size: int
     width: Union[int, str]
-    css: str
+    css: NotRequired[StyleCss]
     uid: NotRequired[str]
-    column_widths: NotRequired[List[int]]
+    column_baselines: NotRequired[List[int]]
+
 
 class Options(TypedDict):
     common: CommonOptions
-    html: HtmlOptions
+    html: HtmlOptions
```

