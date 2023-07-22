# Comparing `tmp/TXM_Sandbox-0.2.3.tar.gz` & `tmp/TXM_Sandbox-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TXM_Sandbox-0.2.3.tar", last modified: Tue Nov  1 12:02:23 2022, max compression
+gzip compressed data, was "TXM_Sandbox-0.2.4.tar", last modified: Sat Jul 22 04:20:03 2023, max compression
```

## Comparing `TXM_Sandbox-0.2.3.tar` & `TXM_Sandbox-0.2.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.449906 TXM_Sandbox-0.2.3/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     1070 2022-10-01 04:14:05.000000 TXM_Sandbox-0.2.3/LICENSE
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      147 2022-10-01 04:14:26.000000 TXM_Sandbox-0.2.3/MANIFEST.in
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      268 2022-11-01 12:02:23.449906 TXM_Sandbox-0.2.3/PKG-INFO
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     1601 2022-10-01 04:14:37.000000 TXM_Sandbox-0.2.3/README.md
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    13782 2022-10-30 14:13:42.000000 TXM_Sandbox-0.2.3/TXM_GUI2.ipynb
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.441907 TXM_Sandbox-0.2.3/TXM_Sandbox/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      181 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/__init__.py
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.443906 TXM_Sandbox-0.2.3/TXM_Sandbox/config/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     5092 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)       45 2022-10-30 14:12:11.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      497 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      500 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      616 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.443906 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     3757 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/config_dict.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    41092 2022-10-31 02:49:15.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      755 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      583 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/xanes_analysis_dict.py
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.444907 TXM_Sandbox-0.2.3/TXM_Sandbox/external/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/external/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      253 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/external/user_io.py
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.446906 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    32500 2022-11-01 02:56:31.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    74120 2022-10-28 02:49:38.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    79227 2022-10-31 03:03:44.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/gui_components.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    36872 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    15639 2022-10-19 23:44:48.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/main_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      795 2022-10-23 19:45:27.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/misc_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)   167020 2022-10-25 05:40:00.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)   197422 2022-10-03 16:45:10.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)   198632 2022-10-03 16:44:03.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    96600 2022-10-31 12:12:38.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)   207086 2022-10-31 04:27:31.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes_fitting_gui.py
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.447907 TXM_Sandbox-0.2.3/TXM_Sandbox/tmp/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/tmp/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)       69 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/tmp/readme.txt
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.448907 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/__init__.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    16483 2022-10-27 05:08:09.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/io.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    14410 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xiao      (1001) xiao      (1001)     3114 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/misc.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     1439 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/plotlib.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    85268 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/reg_algs.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    41053 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    36738 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     2342 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    23436 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_math.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     6083 2022-10-09 19:32:18.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)    76955 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     3266 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_spectra_filters.py
-drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2022-11-01 12:02:23.442906 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      268 2022-11-01 12:02:23.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/PKG-INFO
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     1684 2022-11-01 12:02:23.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/SOURCES.txt
--rw-rw-r--   0 xiao      (1001) xiao      (1001)        1 2022-11-01 12:02:23.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/dependency_links.txt
--rw-rw-r--   0 xiao      (1001) xiao      (1001)        1 2022-10-30 14:56:54.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/not-zip-safe
--rw-rw-r--   0 xiao      (1001) xiao      (1001)      177 2022-11-01 12:02:23.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/requires.txt
--rw-rw-r--   0 xiao      (1001) xiao      (1001)       12 2022-11-01 12:02:23.000000 TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/top_level.txt
--rw-rw-r--   0 xiao      (1001) xiao      (1001)       38 2022-11-01 12:02:23.449906 TXM_Sandbox-0.2.3/setup.cfg
--rw-rw-r--   0 xiao      (1001) xiao      (1001)     1148 2022-11-01 12:01:55.000000 TXM_Sandbox-0.2.3/setup.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.227200 TXM_Sandbox-0.2.4/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     1070 2022-10-01 04:14:05.000000 TXM_Sandbox-0.2.4/LICENSE
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      147 2022-10-01 04:14:26.000000 TXM_Sandbox-0.2.4/MANIFEST.in
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      268 2023-07-22 04:20:03.227200 TXM_Sandbox-0.2.4/PKG-INFO
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     1601 2022-10-01 04:14:37.000000 TXM_Sandbox-0.2.4/README.md
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    13610 2023-07-21 23:35:51.000000 TXM_Sandbox-0.2.4/TXM_GUI2.ipynb
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.206200 TXM_Sandbox-0.2.4/TXM_Sandbox/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      181 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/__init__.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.208200 TXM_Sandbox-0.2.4/TXM_Sandbox/config/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     5092 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)       45 2023-07-22 02:50:00.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      497 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      500 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      616 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.210200 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     3757 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    41092 2022-10-31 02:49:15.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      755 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      583 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/xanes_analysis_dict.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.211200 TXM_Sandbox-0.2.4/TXM_Sandbox/external/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/external/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      253 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/external/user_io.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.219200 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    32500 2022-11-01 02:56:31.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    74120 2022-10-28 02:49:38.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    79227 2022-10-31 03:03:44.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/gui_components.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    36752 2023-07-21 03:16:57.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    15639 2022-10-19 23:44:48.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/main_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      795 2022-10-23 19:45:27.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)   167412 2023-07-21 23:46:06.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)   197422 2022-10-03 16:45:10.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)   198632 2022-10-03 16:44:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    96600 2022-10-31 12:12:38.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)   207086 2022-10-31 04:27:31.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes_fitting_gui.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.221200 TXM_Sandbox-0.2.4/TXM_Sandbox/tmp/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/tmp/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)       69 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/tmp/readme.txt
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.227200 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      107 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/__init__.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    16458 2023-07-21 23:43:49.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/io.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    14410 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xiao      (1001) xiao      (1001)     3114 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/misc.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     1439 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/plotlib.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    85268 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    41510 2023-07-21 23:45:17.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    36738 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     2342 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    23436 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     6083 2022-10-09 19:32:18.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)    76955 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     3266 2022-10-01 03:53:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_spectra_filters.py
+drwxrwxr-x   0 xiao      (1001) xiao      (1001)        0 2023-07-22 04:20:03.207200 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      268 2023-07-22 04:20:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/PKG-INFO
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     1694 2023-07-22 04:20:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)        1 2023-07-22 04:20:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)        1 2022-10-30 14:56:54.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/not-zip-safe
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)      177 2023-07-22 04:20:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/requires.txt
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)       12 2023-07-22 04:20:03.000000 TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/top_level.txt
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)       38 2023-07-22 04:20:03.228200 TXM_Sandbox-0.2.4/setup.cfg
+-rw-rw-r--   0 xiao      (1001) xiao      (1001)     1157 2023-07-21 02:50:52.000000 TXM_Sandbox-0.2.4/setup.py
```

### Comparing `TXM_Sandbox-0.2.3/LICENSE` & `TXM_Sandbox-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/README.md` & `TXM_Sandbox-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_GUI2.ipynb` & `TXM_Sandbox-0.2.4/TXM_GUI2.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977444334215168%*

 * *Differences: {"'cells'": "{1: {'outputs': {1: {'data': {'application/vnd.jupyter.widget-view+json': "*

 * *            "{'model_id': 'b2e6e32311164e3eaad05f9e8d0ac989'}}}, 2: {'text': {delete: [2, 1]}}}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.6'}}"}*

```diff
@@ -55,32 +55,30 @@
                         "WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations\n",
                         "WARNING: All illegal access operations will be denied in a future release\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "65e64398455b4f0fad5d3030ecf8322c",
+                            "model_id": "b2e6e32311164e3eaad05f9e8d0ac989",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Tab(children=(Tab(children=(VBox(children=(VBox(children=(HBox(children=(HTML(value=\"<span style='color:red; f\u2026"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "WARNING: Qt: Session management error: None of the authentication protocols specified are supported\n",
-                        "Warning: Could not get charToByteConverterClass![java.lang.Enum.toString] Warning: Could not get charToByteConverterClass!\n",
-                        "[java.lang.Enum.toString] \n"
+                        "WARNING: Qt: Session management error: None of the authentication protocols specified are supported\n"
                     ]
                 }
             ],
             "source": [
                 "%gui qt\n",
                 "from TXM_Sandbox.gui import main_gui as txmg\n",
                 "gui = txmg.txm_gui(fiji_path='/home/xiao/software/Fiji.app', form_sz=[750, 1000])\n",
@@ -459,13 +457,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5"
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/config/XANES2D_GUI_config.json` & `TXM_Sandbox-0.2.4/TXM_Sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json` & `TXM_Sandbox-0.2.4/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/config_dict.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/customized_struct_dict.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/sklearn_opt_dict.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/dicts/xanes_analysis_dict.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/conv_data_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/gen_algn_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/gui_components.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/io_config_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/io_config_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,23 +379,23 @@
     def io_optn_chbx_chg(self, a):
         self.boxes_logics()
 
     def io_cfm_btn_clk(self, a):
         save_io_config(self)
         with open(self.global_h.io_data_struc_tomo_cfg_file, 'r') as f:
             self.global_h.io_tomo_cfg = json.load(f)
-            self.global_h.tomo_recon_gui.tomo_raw_fn_temp = self.global_h.io_tomo_cfg['structured_h5_reader']['tomo_raw_fn_template']
+            self.global_h.tomo_recon_gui.tomo_raw_fn_temp = self.global_h.io_tomo_cfg['tomo_raw_fn_template']
         with open(self.global_h.io_data_struc_xanes2D_cfg_file, 'r') as f:
             self.global_h.io_xanes2D_cfg = json.load(f)
-            self.global_h.xanes2D_gui.xanes2D_raw_fn_temp = self.global_h.io_xanes2D_cfg['structured_h5_reader']['xanes2D_raw_fn_template']
+            self.global_h.xanes2D_gui.xanes2D_raw_fn_temp = self.global_h.io_xanes2D_cfg['xanes2D_raw_fn_template']
         with open(self.global_h.io_data_struc_xanes3D_cfg_file, 'r') as f:
             self.global_h.io_xanes3D_cfg = json.load(f)
-            self.global_h.xanes3D_gui.xanes3D_raw_fn_temp = self.global_h.io_xanes3D_cfg['structured_h5_reader']['tomo_raw_fn_template']
-            self.global_h.xanes3D_gui.xanes3D_recon_dir_temp = self.global_h.io_xanes3D_cfg['structured_h5_reader']['xanes3D_recon_dir_template']
-            self.global_h.xanes3D_gui.xanes3D_recon_fn_temp = self.global_h.io_xanes3D_cfg['structured_h5_reader']['xanes3D_recon_fn_template']
+            self.global_h.xanes3D_gui.xanes3D_raw_fn_temp = self.global_h.io_xanes3D_cfg['tomo_raw_fn_template']
+            self.global_h.xanes3D_gui.xanes3D_recon_dir_temp = self.global_h.io_xanes3D_cfg['xanes3D_recon_dir_template']
+            self.global_h.xanes3D_gui.xanes3D_recon_fn_temp = self.global_h.io_xanes3D_cfg['xanes3D_recon_fn_template']
 
     def io_spec_tomo_rdr_btn_clk(self, a):
         if len(a.files[0]) != 0:
             self.hs['IOSpecTomoRdr text'].value = a.files[0]        
             save_io_config(self)
             with open(self.global_h.io_data_struc_tomo_cfg_file, 'r') as f:
                 self.global_h.io_tomo_cfg = json.load(f)
```

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/main_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/misc_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/tomo_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/tomo_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3099,27 +3099,36 @@
         self.recon_finish = -1
         self.boxes_logic()
         self.tomo_compound_logic()
 
     def AutoRefFn_btn_clk(self, a):
         if len(a.files[0]) != 0:
             self.tomo_wedge_ang_auto_det_ref_fn = a.files[0]
+            self.set_rec_dict_from_rec_params()
+            cfg = deepcopy(self.tomo_recon_param_dict)
+            cfg["file_params"][
+                "wedge_ang_auto_det_ref_fn"
+            ] = self.tomo_wedge_ang_auto_det_ref_fn
+            cfg["file_params"]["reader"] = self.reader
+            cfg["file_params"]["info_reader"] = data_info(tomo_h5_info)
+            cfg["recon_config"]["use_ds"] = (
+                True if self.tomo_use_downsample == 1 else False
+            )
             self.wedge_eva_data, flat, dark, _ = read_data(
                 self.reader,
                 self.tomo_wedge_ang_auto_det_ref_fn,
-                self.global_h.io_tomo_cfg,
+                cfg,
                 sli_start=self.tomo_sli_s,
                 sli_end=self.tomo_sli_e,
                 col_start=self.tomo_wedge_auto_ref_col_s,
                 col_end=self.tomo_wedge_auto_ref_col_e,
                 ds_use=self.tomo_use_downsample,
                 ds_level=self.tomo_ds_ratio,
                 mean_axis=2,
             )
-            print(self.wedge_eva_data.shape, flat.shape, dark.shape)
             self.hs["AutoRefSli sldr"].value = 0
             self.hs["AutoRefSli sldr"].max = self.wedge_eva_data.shape[1] - 1
         else:
             self.tomo_wedge_ang_auto_det_ref_fn = None
         self.tomo_data_configured = False
         self.recon_finish = -1
         self.boxes_logic()
```

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes2D_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes3D_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes_analysis_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/gui/xanes_fitting_gui.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/io.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
              for dtype='eng'
     Returns:
         ndarray
     """
     sli = sli_interpreter(sli)
     with h5py.File(fn, 'r') as f:
         if dtype == 'data':
-            # print(sli)
             return np.squeeze(f[cfg['structured_h5_reader']
                                 ['io_data_structure']['data_path']])[sli]
         elif dtype == 'flat':
             return np.squeeze(f[cfg['structured_h5_reader']
                                 ['io_data_structure']['flat_path']])[sli]
         elif dtype == 'dark':
             return np.squeeze(f[cfg['structured_h5_reader']
```

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/lineshapes.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/misc.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/plotlib.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/reg_algs.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/tomo_recon_tools.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/tomo_recon_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     return:
         dictionary,
         the bad angle list for each slice in the slice range [sli_start, sli_end]
     """
     sli_start = int(sli_start)
 
-    img_shape = dim_info(fn, dtype='data', cfg=cfg)
+    img_shape = dim_info(fn, dtype='data', cfg=cfg["file_params"]["io_confg"])
     if sli_end is None:
         sli_end = img_shape[1]
     elif sli_end > img_shape[1]:
         print('sli_end exceeds the maximum allowed range...')
         return None
     else:
         sli_end = int(sli_end)
@@ -148,15 +148,14 @@
                              fake_flat_val=1e4, fake_dark_val=100,
                              ds_use=ds_use, ds_level=ds_level, mean_axis=2)
     bad_angs = tem < thres
     return bad_angs
 
 
 def get_file(raw_data_top_dir, scan_id, cfg, recon_top_dir=None):
-    print(cfg['tomo_raw_fn_template'].format(scan_id))
     data_file = glob.glob(os.path.join(raw_data_top_dir, cfg['tomo_raw_fn_template'].format(scan_id)))
 
     if data_file is []:
         return None
 
     if recon_top_dir is None:
         output_file = os.path.join(raw_data_top_dir,
@@ -258,24 +257,30 @@
     return: tuple of ndarray, or None
         return data, white, dark, theta if succeeds; otherwise None
     """
     if flat_name is None:
         flat_name = fn
     if dark_name is None:
         dark_name = fn
+       
+    data_dim = cfg["file_params"]["info_reader"](
+        fn, dtype="data", cfg=cfg["file_params"]["io_confg"]
+    )
 
-    theta = reader(fn, dtype='theta', sli=[None], cfg=cfg).astype(np.float32)
+    theta = reader(fn, dtype='theta', sli=[None], cfg=cfg["file_params"]["io_confg"]).astype(np.float32)
     idx = rm_redundant(theta)
     theta = theta[idx]
+    if data_dim[0] > theta.shape[0]:
+        idx = np.concatenate((idx, np.zeros(data_dim[0] - theta.shape[0], dtype=bool)))
 
     if mean_axis is None:
         if ds_use:
             data = data_down_sampling(reader(fn, dtype='data',
                                              sli=[None, [sli_start, sli_end], [col_start, col_end]],
-                                             cfg=cfg), [1, ds_level, ds_level]).astype(np.float32)[idx]
+                                             cfg=cfg["file_params"]["io_confg"]), [1, ds_level, ds_level]).astype(np.float32)[idx]
 
             if use_fake_flat:
                 if fake_flat_roi is None:
                     white = data_down_sampling(fake_flat_val * np.ones([8, data.shape[1], data.shape[2]]),
                                                [1, ds_level, ds_level]).astype(np.float32)
                 else:
                     white = data_down_sampling((data[:, fake_flat_roi[0]:fake_flat_roi[1],
@@ -288,74 +293,74 @@
                     [1, ds_level, ds_level]).astype(np.float32)
 
             if use_fake_dark:
                 dark = data_down_sampling(fake_dark_val * np.ones([8, data.shape[1], data.shape[2]]),
                                           [1, ds_level, ds_level]).astype(np.float32)
             else:
                 dark = data_down_sampling(
-                    reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg),
+                    reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]),
                     [1, ds_level, ds_level]).astype(np.float32)
         else:
-            data = reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg).astype(
+            data = reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]).astype(
                 np.float32)[idx]
 
             if use_fake_flat:
                 if fake_flat_roi is None:
                     white = fake_flat_val * np.ones([8, data.shape[1], data.shape[2]], dtype=np.float32)
                 else:
                     white = data[:, fake_flat_roi[0]:fake_flat_roi[1],
                                  fake_flat_roi[2]:fake_flat_roi[3]].mean(axis=(1, 2), keepdims=True) * \
                             np.ones([1, data.shape[1], data.shape[2]], dtype=np.float32)
             else:
                 white = reader(flat_name, dtype='flat', sli=[None, [sli_start, sli_end], [col_start, col_end]],
-                               cfg=cfg).astype(np.float32)
+                               cfg=cfg["file_params"]["io_confg"]).astype(np.float32)
 
             if use_fake_dark:
                 dark = fake_dark_val * np.ones([8, data.shape[1], data.shape[2]], dtype=np.float32)
             else:
                 dark = reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]],
-                              cfg=cfg).astype(np.float32)
+                              cfg=cfg["file_params"]["io_confg"]).astype(np.float32)
     else:
         if ds_use:
             data = data_down_sampling(
-                reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg),
+                reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]),
                 [1, ds_level, ds_level]).astype(np.float32)[idx]
             if use_fake_flat:
                 white = data_down_sampling(fake_flat_val * np.ones([data.shape[1], data.shape[2]]),
                                            [ds_level, ds_level]).astype(np.float32)
             else:
                 white = data_down_sampling(
-                    reader(flat_name, dtype='flat', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg),
+                    reader(flat_name, dtype='flat', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]),
                     [1, ds_level, ds_level]).mean(axis=0).astype(np.float32)
 
             if use_fake_dark:
                 dark = data_down_sampling(fake_dark_val * np.ones([data.shape[1], data.shape[2]]),
                                           [ds_level, ds_level]).astype(np.float32)
             else:
                 dark = data_down_sampling(
-                    reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg),
+                    reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]),
                     [1, ds_level, ds_level]).mean(axis=0).astype(np.float32)
             data[:] = (data - dark[np.newaxis, :]) / (white[np.newaxis, :] - dark[np.newaxis, :])[:]
             data[np.isinf(data)] = 0
             data[np.isnan(data)] = 0
             data = data.mean(axis=mean_axis).astype(np.float32)
         else:
-            data = reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg).astype(
+            data = reader(fn, dtype='data', sli=[None, [sli_start, sli_end], [col_start, col_end]], cfg=cfg["file_params"]["io_confg"]).astype(
                 np.float32)[idx]
             if use_fake_flat:
                 white = fake_flat_val * np.ones([data.shape[1], data.shape[2]], dtype=np.float32)
             else:
                 white = reader(flat_name, dtype='flat', sli=[None, [sli_start, sli_end], [col_start, col_end]],
-                               cfg=cfg).mean(axis=0).astype(np.float32)
+                               cfg=cfg["file_params"]["io_confg"]).mean(axis=0).astype(np.float32)
 
             if use_fake_dark:
                 dark = fake_dark_val * np.ones([data.shape[1], data.shape[2]], dtype=np.float32)
             else:
                 dark = reader(dark_name, dtype='dark', sli=[None, [sli_start, sli_end], [col_start, col_end]],
-                              cfg=cfg).mean(axis=0).astype(np.float32)
+                              cfg=cfg["file_params"]["io_confg"]).mean(axis=0).astype(np.float32)
             data[:] = (data - dark[np.newaxis, :]) / (white[np.newaxis, :] - dark[np.newaxis, :])[:]
             data[np.isinf(data)] = 0
             data[np.isnan(data)] = 0
             data = data.mean(axis=mean_axis).astype(np.float32)
     gc.collect()
     return data, white, dark, theta
 
@@ -446,15 +451,15 @@
         file_alt_flat_fn = None
     if not rec_use_alt_dark:
         file_alt_dark_fn = None
 
     if rec_type == 'Trial Cent':
         file_raw_fn, file_recon_template = get_file(file_raw_data_top_dir, data_scan_id, file_cfg)
 
-        data, white, dark, theta = read_data(reader, file_raw_fn, file_cfg,
+        data, white, dark, theta = read_data(reader, file_raw_fn, kwargs,
                                              sli_start=data_sli_s, sli_end=data_sli_s + 20,
                                              col_start=data_col_s, col_end=data_col_e,
                                              flat_name=file_alt_flat_fn, dark_name=file_alt_dark_fn,
                                              use_fake_flat=rec_use_fake_flat, use_fake_dark=rec_use_fake_dark,
                                              fake_flat_val=data_fake_flat_val, fake_dark_val=data_fake_dark_val,
                                              ds_use=rec_use_ds, ds_level=data_ds_level)
         theta = theta * np.pi / 180.0
@@ -470,25 +475,24 @@
 
         if is_wedge:
             if rec_use_wedge_ang_auto_det:
                 print('wedge_ref_file: ', file_wedge_ang_auto_det_ref_fn)
                 bad_angs = get_dim_ang_range_range_sli(dim_info,
                                                        reader,
                                                        file_wedge_ang_auto_det_ref_fn,
-                                                       file_cfg,
+                                                       kwargs,
                                                        sli_start=data_sli_s,
                                                        sli_end=data_sli_s + 20,
                                                        col_start=data_wedge_col_s, col_end=data_wedge_col_e,
                                                        ds_use=rec_use_ds, ds_level=data_ds_level,
                                                        thres=data_wedge_ang_auto_det_thres)
             else:
                 bad_angs = np.zeros([data.shape[0], data.shape[1]], dtype=bool)
                 bad_angs[data_wedge_missing_s:data_wedge_missing_e, :] = True
             data[:] = sort_wedge(data, bad_angs, 0, 20, padval=1)[:]
-            print(data.shape)
             if rec_use_debug:
                 save_debug(file_debug_top_dir, '1-wedge_data.tiff', data)
 
         if rec_use_debug:
             save_debug(file_debug_top_dir, '2-norm_data.tiff', data)
 
         if 0 != len(flt_param_dict.keys()):
@@ -530,33 +534,32 @@
                     fo.write(str(k) + ': ' + str(v) + '\n\n')
         return 0
     else:
         state = 1
         if is_wedge:
             if rec_use_wedge_ang_auto_det:
                 bad_angs = get_dim_ang_range_range_sli(dim_info, reader, file_wedge_ang_auto_det_ref_fn,
-                                                       file_cfg, sli_start=0,
+                                                       kwargs, sli_start=0,
                                                        sli_end=None, col_start=data_wedge_col_s,
                                                        col_end=data_wedge_col_e,
                                                        ds_use=rec_use_ds, ds_level=data_ds_level,
                                                        thres=data_wedge_ang_auto_det_thres)
             else:
                 bad_angs = np.zeros([data.shape[0], data.shape[1]])
                 bad_angs[data_wedge_missing_s:data_wedge_missing_e, :] = 1
 
         file_raw_fn, file_recon_template = get_file(file_raw_data_top_dir, data_scan_id, file_cfg,
                                                     recon_top_dir=file_recon_top_dir)
-        print(file_raw_fn, file_recon_template)
         dim = dim_info(file_raw_fn, dtype='data', cfg=file_cfg)
 
         if data_chunk_sz >= (data_sli_e - data_sli_s):
             data_chunk_sz = (data_sli_e - data_sli_s)
             num_chunk = 1
         else:
-            num_chunk = np.int((data_sli_e - data_sli_s) / (data_chunk_sz - 2 * data_margin)) + 1
+            num_chunk = int((data_sli_e - data_sli_s) / (data_chunk_sz - 2 * data_margin)) + 1
 
         for ii in range(num_chunk):
             try:
                 if ii == 0:
                     sli_start = data_sli_s
                     sli_end = data_sli_s + data_chunk_sz
                 else:
@@ -568,15 +571,15 @@
                         sli_end = dim[1]
 
                 if (sli_end - sli_start) <= data_margin:
                     print('skip')
                     break
                 else:
                     data, white, dark, theta = read_data(reader,
-                                                         file_raw_fn, file_cfg,
+                                                         file_raw_fn, kwargs,
                                                          sli_start=sli_start, sli_end=sli_end,
                                                          col_start=data_col_s, col_end=data_col_e,
                                                          flat_name=file_alt_flat_fn, dark_name=file_alt_dark_fn,
                                                          use_fake_flat=rec_use_fake_flat,
                                                          use_fake_dark=rec_use_fake_dark,
                                                          fake_flat_val=data_fake_flat_val,
                                                          fake_dark_val=data_fake_dark_val,
```

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_analysis.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_image_utils.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_math.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_post_analysis.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_regtools.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox/utils/xanes_spectra_filters.py` & `TXM_Sandbox-0.2.4/TXM_Sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `TXM_Sandbox-0.2.3/TXM_Sandbox.egg-info/SOURCES.txt` & `TXM_Sandbox-0.2.4/TXM_Sandbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 TXM_GUI2.ipynb
+setup.cfg
 setup.py
 TXM_Sandbox/__init__.py
 TXM_Sandbox.egg-info/PKG-INFO
 TXM_Sandbox.egg-info/SOURCES.txt
 TXM_Sandbox.egg-info/dependency_links.txt
 TXM_Sandbox.egg-info/not-zip-safe
 TXM_Sandbox.egg-info/requires.txt
```

### Comparing `TXM_Sandbox-0.2.3/setup.py` & `TXM_Sandbox-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jul 16 22:20:14 2020
 
-@author: xiao
+@author: Xianghui Xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='TXM_Sandbox',
-      version='0.2.3',
+      version='0.2.4',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

