# Comparing `tmp/np_workflows-1.5.5.tar.gz` & `tmp/np_workflows-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_workflows-1.5.5.tar", last modified: Wed Jul 19 00:52:36 2023, max compression
+gzip compressed data, was "np_workflows-1.6.0.tar", last modified: Fri Jul 21 23:41:30 2023, max compression
```

## Comparing `np_workflows-1.5.5.tar` & `np_workflows-1.6.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0     1614 2023-06-30 17:48:35.853909 np_workflows-1.5.5/README.md
--rw-r--r--   0        0        0     2561 2023-07-19 00:52:36.978217 np_workflows-1.5.5/pyproject.toml
--rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.5.5/src/np_workflows/__init__.py
--rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.5.5/src/np_workflows/assets/images/logo_np_hab.png
--rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.5.5/src/np_workflows/assets/images/logo_np_vis.png
--rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.5.5/src/np_workflows/experiments/__init__.py
--rw-r--r--   0        0        0      148 2023-05-18 23:17:52.356257 np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/__init__.py
--rw-r--r--   0        0        0     2737 2023-06-08 01:15:00.774997 np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py
--rw-r--r--   0        0        0     4401 2023-05-11 18:20:25.162316 np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py
--rw-r--r--   0        0        0     7621 2023-06-05 04:11:33.975384 np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py
--rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-18 01:58:07.942705 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py
--rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_00.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.949928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_01.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_02.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_03.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_04.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_05.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_06.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.919928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_07.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.889928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_08.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_09.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.859928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_10.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.839929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_11.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.829929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_12.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_13.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.799929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_14.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.789932 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_15.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.769930 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_16.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.759930 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_17.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.749930 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_18.stim
--rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/flash_250ms.stim
--rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim
--rw-r--r--   0        0        0      340 2023-03-08 20:59:00.949928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/old_stim.stim
--rw-r--r--   0        0        0      334 2023-03-08 20:59:00.959929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed.stim
--rw-r--r--   0        0        0      345 2023-03-08 20:59:00.979929 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_1st.stim
--rw-r--r--   0        0        0      346 2023-03-08 20:59:00.969928 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_2nd.stim
--rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
--rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
--rw-r--r--   0        0        0     9220 2023-05-18 02:12:21.002654 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
--rw-r--r--   0        0        0     2684 2023-06-08 00:43:09.047204 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
--rw-r--r--   0        0        0     8693 2023-05-24 16:37:52.954146 np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
--rw-r--r--   0        0        0      200 2023-05-19 23:52:58.915202 np_workflows-1.5.5/src/np_workflows/experiments/templeton/__init__.py
--rw-r--r--   0        0        0    12631 2023-07-19 00:25:39.284891 np_workflows-1.5.5/src/np_workflows/experiments/templeton/main_templeton_pilot.py
--rw-r--r--   0        0        0     1779 2023-05-19 23:56:16.341090 np_workflows-1.5.5/src/np_workflows/experiments/templeton/templeton_stim_config.py
--rw-r--r--   0        0        0     2750 2023-07-19 00:00:36.269446 np_workflows-1.5.5/src/np_workflows/experiments/templeton/templeton_widgets.py
--rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.5.5/src/np_workflows/shared/__init__.py
--rw-r--r--   0        0        0    18321 2023-07-13 02:06:35.161196 np_workflows-1.5.5/src/np_workflows/shared/base_experiments.py
--rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.5/src/np_workflows/shared/camstim_scripts/flash_250ms.stim
--rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.5/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim
--rw-r--r--   0        0        0     6258 2023-05-04 01:03:37.729885 np_workflows-1.5.5/src/np_workflows/shared/npxc.py
--rw-r--r--   0        0        0    25914 2023-06-08 00:33:50.617758 np_workflows-1.5.5/src/np_workflows/shared/widgets.py
--rw-r--r--   0        0        0   753021 2023-04-14 19:17:10.939361 np_workflows-1.5.5/tests/logs/debug.log
--rw-r--r--   0        0        0   361698 2023-04-14 19:17:10.939361 np_workflows-1.5.5/tests/logs/warning.log
--rw-r--r--   0        0        0      508 2023-03-17 23:19:28.833208 np_workflows-1.5.5/tests/model_sandbox.py
--rw-r--r--   0        0        0    34554 2023-07-11 18:40:27.336659 np_workflows-1.5.5/tests/widget_sandbox.ipynb
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 np_workflows-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1614 2023-06-30 17:48:35.853909 np_workflows-1.6.0/README.md
+-rw-r--r--   0        0        0     2561 2023-07-21 23:41:30.955131 np_workflows-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.6.0/src/np_workflows/__init__.py
+-rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.6.0/src/np_workflows/assets/images/logo_np_hab.png
+-rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.6.0/src/np_workflows/assets/images/logo_np_vis.png
+-rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.6.0/src/np_workflows/experiments/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-18 23:17:52.356257 np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/__init__.py
+-rw-r--r--   0        0        0     2737 2023-06-08 01:15:00.774997 np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py
+-rw-r--r--   0        0        0     4401 2023-05-11 18:20:25.162316 np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py
+-rw-r--r--   0        0        0     7621 2023-06-05 04:11:33.975384 np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py
+-rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-18 01:58:07.942705 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py
+-rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_00.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.949928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_01.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_02.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_03.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_04.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_05.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_06.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.919928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_07.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.889928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_08.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_09.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.859928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_10.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.839929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_11.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.829929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_12.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_13.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.799929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_14.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.789932 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_15.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.769930 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_16.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.759930 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_17.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.749930 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_18.stim
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0      340 2023-03-08 20:59:00.949928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/old_stim.stim
+-rw-r--r--   0        0        0      334 2023-03-08 20:59:00.959929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed.stim
+-rw-r--r--   0        0        0      345 2023-03-08 20:59:00.979929 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_1st.stim
+-rw-r--r--   0        0        0      346 2023-03-08 20:59:00.969928 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_2nd.stim
+-rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
+-rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
+-rw-r--r--   0        0        0     9220 2023-05-18 02:12:21.002654 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
+-rw-r--r--   0        0        0     2684 2023-06-08 00:43:09.047204 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
+-rw-r--r--   0        0        0     8693 2023-05-24 16:37:52.954146 np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
+-rw-r--r--   0        0        0      200 2023-05-19 23:52:58.915202 np_workflows-1.6.0/src/np_workflows/experiments/templeton/__init__.py
+-rw-r--r--   0        0        0     4382 2023-07-21 23:36:50.366998 np_workflows-1.6.0/src/np_workflows/experiments/templeton/main_templeton_pilot.py
+-rw-r--r--   0        0        0     2750 2023-07-19 00:00:36.269446 np_workflows-1.6.0/src/np_workflows/experiments/templeton/templeton_widgets.py
+-rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.6.0/src/np_workflows/shared/__init__.py
+-rw-r--r--   0        0        0    28198 2023-07-21 23:40:15.307485 np_workflows-1.6.0/src/np_workflows/shared/base_experiments.py
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.6.0/src/np_workflows/shared/camstim_scripts/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.6.0/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0     6876 2023-07-21 23:37:20.672906 np_workflows-1.6.0/src/np_workflows/shared/npxc.py
+-rw-r--r--   0        0        0    25914 2023-06-08 00:33:50.617758 np_workflows-1.6.0/src/np_workflows/shared/widgets.py
+-rw-r--r--   0        0        0   753021 2023-04-14 19:17:10.939361 np_workflows-1.6.0/tests/logs/debug.log
+-rw-r--r--   0        0        0   361698 2023-04-14 19:17:10.939361 np_workflows-1.6.0/tests/logs/warning.log
+-rw-r--r--   0        0        0      508 2023-03-17 23:19:28.833208 np_workflows-1.6.0/tests/model_sandbox.py
+-rw-r--r--   0        0        0    34554 2023-07-11 18:40:27.336659 np_workflows-1.6.0/tests/widget_sandbox.ipynb
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 np_workflows-1.6.0/PKG-INFO
```

### Comparing `np_workflows-1.5.5/README.md` & `np_workflows-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/pyproject.toml` & `np_workflows-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "np-workflows"
-version = "1.5.5"
+version = "1.6.0"
 description = "Ecephys and behavior workflows for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 readme = "README.md"
 requires-python = "==3.11.*"
 dependencies = [
-    "np-services>=0.1.47",
+    "np-services>=0.1.53",
     "np-session>=0.6.5",
     "np-config >=0.4.20",
     "np-probe-targets >= 0.0.11",
     "np-datajoint",
     "ipywidgets >=7",
     "pydantic >=1, < 2",
     "jupyterlab >= 3.6",
```

### Comparing `np_workflows-1.5.5/src/np_workflows/assets/images/logo_np_hab.png` & `np_workflows-1.6.0/src/np_workflows/assets/images/logo_np_hab.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/assets/images/logo_np_vis.png` & `np_workflows-1.6.0/src/np_workflows/assets/images/logo_np_vis.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py` & `np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py` & `np_workflows-1.6.0/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py` & `np_workflows-1.6.0/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/experiments/templeton/templeton_widgets.py` & `np_workflows-1.6.0/src/np_workflows/experiments/templeton/templeton_widgets.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/shared/base_experiments.py` & `np_workflows-1.6.0/src/np_workflows/shared/base_experiments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import abc
 import configparser
 import contextlib
+import enum
 import functools
-import getpass
 import pathlib
 import re
 import shutil
 import time
-from typing import Any, ClassVar, Iterable, Literal, Optional, Protocol, Sequence, Type, Union
+from typing import Any, ClassVar, Iterable, Literal, Optional, Protocol, Type
 
-import fabric 
+import fabric
 import ipylab
-
 import np_config
 import np_logging
-import np_session
 import np_services
-import np_workflows.shared.npxc as npxc
+import np_session
 from np_services import (
-    Service,
-    TestError,
-    Configurable,
+    Finalizable,
     Initializable,
-    Testable,
     Pretestable,
+    Service,
+    Shutdownable,
     Startable,
-    Verifiable,
     Stoppable,
-    Finalizable,
+    Testable,
     Validatable,
-    Shutdownable,
+    Verifiable,
 )
 
+import np_workflows.shared.npxc as npxc
 
 logger = np_logging.getLogger(__name__)
 
 class WithSessionInfo(Protocol):
     @property
     def session(self) -> np_session.Session: ...
     @property
@@ -49,15 +46,25 @@
 class WithSession(abc.ABC):
     
     default_session_subclass: ClassVar[Type[np_session.Session]] = np_session.PipelineSession
     default_session_type: Literal['ephys', 'hab'] = 'ephys'
     
     services: tuple[Service, ...] = ()
     "All services. Devices, databases, etc."
+    
+    workflow: enum.Enum = enum.Enum('BaseWithSessionWorkflow', ('BASECLASS')).BASECLASS # type: ignore
+    """Enum for workflow type, e.g. PRETEST, HAB_AUD, HAB_VIS, EPHYS_ etc."""
 
+    def log(self, message: str, weblog_name: Optional[str] = None) -> None:
+        logger.info(message)
+        if not weblog_name:
+            weblog_name = self.workflow.name
+        with contextlib.suppress(AttributeError):
+            np_logging.web(f'{weblog_name.lower()}_{self.mouse}').info(message)
+    
     @property
     @abc.abstractmethod
     def recorders(self) -> tuple[Startable | Stoppable, ...]:
         """Services that record data. These are started and stopped as a group."""
         return NotImplemented
     
     def __init__(self, 
@@ -285,16 +292,44 @@
         # TODO use the following to export to html (shows input to widgets and
         # output of cells)
         #! currently can't be run automatically as save as path dialog opens 
         # app.commands.execute('notebook:export-to-format', {
         #     'format': 'html',
         #     # 'download': 'false',
         #     # 'path': 'c:/users/svc_neuropix/documents/github/np_notebooks/task_trained_network/ttn_pilot.html',
-        # })       
+        # })   
+            
+    @functools.cached_property
+    def system_camstim_params(self) -> dict[str, Any]:
+        """Try to load defaults from camstim config file on the Stim computer.
         
+        May encounter permission error if not running as svc_neuropix.
+        """
+        with contextlib.suppress(OSError):
+            parser = configparser.RawConfigParser()
+            parser.read(
+                (self.rig.paths["Camstim"].parent / "config" / "stim.cfg").as_posix()
+            )
+
+            camstim_default_config = {}
+            for section in parser.sections():
+                camstim_default_config[section] = {}
+                for k, v in parser[section].items():
+                    try:
+                        value = eval(
+                            v
+                        )  # this removes comments in config and converts values to expected datatype
+                    except:
+                        continue
+                    else:
+                        camstim_default_config[section][k] = value
+            return camstim_default_config
+        logger.warning("Could not load camstim defaults from config file on Stim computer.")
+        return {}
+    
 class PipelineExperiment(WithSession):
     @property
     def platform_json(self) -> np_session.PlatformJson:
         self.session.platform_json.update('rig_id', str(self.rig))
         return self.session.platform_json
     
     def start_recording(self, *recorders: Startable) -> None:
@@ -385,42 +420,223 @@
         for ephys_folder in np_services.OpenEphys.data_files:
             with contextlib.suppress(Exception):
                 with ssh:
                     ssh.run(
                     f'robocopy "{ephys_folder}" "{self.session.npexp_path / ephys_folder.name}" /j /s /xo' 
                     # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
                     )
-    
-    @functools.cached_property
-    def system_camstim_params(self) -> dict[str, Any]:
-        """Try to load defaults from camstim config file on the Stim computer.
-        
-        May encounter permission error if not running as svc_neuropix.
-        """
-        with contextlib.suppress(OSError):
-            parser = configparser.RawConfigParser()
-            parser.read(
-                (self.rig.paths["Camstim"].parent / "config" / "stim.cfg").as_posix()
-            )
-
-            camstim_default_config = {}
-            for section in parser.sections():
-                camstim_default_config[section] = {}
-                for k, v in parser[section].items():
-                    try:
-                        value = eval(
-                            v
-                        )  # this removes comments in config and converts values to expected datatype
-                    except:
-                        continue
-                    else:
-                        camstim_default_config[section][k] = value
-            return camstim_default_config
-        logger.warning("Could not load camstim defaults from config file on Stim computer.")
-        return {}
 
 class PipelineEphys(PipelineExperiment):
     default_session_type = 'ephys'
 
-
 class PipelineHab(PipelineExperiment):
     default_session_type = 'hab'
+
+
+class DynamicRoutingExperiment(WithSession):
+    
+    default_session_subclass: Type[np_session.Session]
+    
+    workflow: enum.Enum
+    
+    @property
+    @abc.abstractmethod
+    def is_pretest(self) -> bool:
+        return NotImplemented
+    
+    @property
+    @abc.abstractmethod
+    def is_hab(self) -> bool:
+        return NotImplemented
+    
+    @property
+    @abc.abstractmethod
+    def task_name(self) -> str:
+        """For sending to runTask.py and controlling implementation details of the task."""
+        return NotImplemented
+            
+    services = (
+        np_services.Sync,
+        np_services.VideoMVR,
+        np_services.ImageMVR,
+        np_services.OpenEphys, 
+        np_services.NewScaleCoordinateRecorder,
+        np_services.ScriptCamstim, 
+        np_services.MouseDirector,
+        )
+    
+    stims = (np_services.ScriptCamstim,)
+    
+    @property
+    def recorders(self) -> tuple[Service, ...]:
+        """Services to be started before stimuli run, and stopped after. Session-dependent."""
+        if self.is_hab:
+            return (np_services.Sync, np_services.VideoMVR)
+        return (np_services.Sync, np_services.VideoMVR, np_services.OpenEphys)
+    
+    @property
+    def hdf5_dir(self) -> pathlib.Path:
+        return pathlib.Path('//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/Data') /  str(self.mouse)
+    
+    @property
+    def task_params(self) -> dict[str, str]:
+        """For sending to runTask.py"""
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = str(self.mouse),
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/DynamicRouting1.py',
+                taskVersion = self.task_name,
+        )
+        
+    @property
+    def spontaneous_params(self) -> dict[str, str]:
+        """For sending to runTask.py"""
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = str(self.mouse) if not self.is_pretest else 'test',
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/TaskControl.py',
+                taskVersion = 'spontaneous',
+        )
+        
+    @property
+    def spontaneous_rewards_params(self) -> dict[str, str]:
+        """For sending to runTask.py"""
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = str(self.mouse) if not self.is_pretest else 'test',
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/TaskControl.py',
+                taskVersion = 'spontaneous rewards',
+                # rewardSound = "device",
+        )
+        
+    @property
+    def optotagging_params(self) -> dict[str, str]:
+        """For sending to runTask.py"""
+        locs_root = pathlib.Path("//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/OptoGui/optolocs")
+        locs = sorted(tuple(locs_root.glob(f"optolocs_{self.mouse.id}_{str(self.rig).replace('.', '')}_*")), reverse=True)[0]
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = str(self.mouse) if not self.is_pretest else 'test',
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/TaskControl.py',
+                taskVersion = 'optotagging',
+                optoTaggingLocs = locs.as_posix(),
+        )
+
+    @property
+    def mapping_params(self: WithSessionInfo) -> dict[str, str]:
+        """For sending to runTask.py"""
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = str(self.mouse),
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/RFMapping.py'
+            )
+
+    @property
+    def sound_test_params(self) -> dict[str, str]:
+        """For sending to runTask.py"""
+        return dict(
+                rigName = str(self.rig).replace('.',''),
+                subjectName = 'sound',
+                taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/TaskControl.py',
+                taskVersion = 'sound test',
+        )
+        
+    def run_script(self, stim: Literal['sound_test', 'mapping', 'task', 'optotagging', 'spontaneous', 'spontaneous_rewards']) -> None:
+        np_services.ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/runTask.py'
+        np_services.ScriptCamstim.params = getattr(self, f'{stim.replace(" ", "_")}_params')
+
+        self.log(f"{stim} started")
+
+        np_services.ScriptCamstim.start()
+
+        while not np_services.ScriptCamstim.is_ready_to_start():
+            time.sleep(1)
+            
+        self.log(f"{stim} complete")
+
+        np_services.ScriptCamstim.finalize()
+        
+    run_mapping = functools.partialmethod(run_script, 'mapping')
+    run_sound_test = functools.partialmethod(run_script, 'sound_test')
+    run_optotagging = functools.partialmethod(run_script, 'optotagging')
+    run_spontaneous = functools.partialmethod(run_script, 'spontaneous')
+    run_spontaneous_rewards = functools.partialmethod(run_script, 'spontaneous_rewards')
+    
+    def run_task(self) -> None:
+        self.update_state()
+        self.run_script('task')    
+        
+    def update_state(self) -> None:
+        "Persist useful but non-essential info."
+        self.mouse.state['last_session'] = self.session.id
+        self.mouse.state['last_workflow'] = str(self.workflow.name)
+        self.mouse.state['last_task'] = str(self.task_name)
+        
+    def initialize_and_test_services(self) -> None:
+        """Configure, initialize (ie. reset), then test all services."""
+        
+        np_services.ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/runTask.py'
+        np_services.ScriptCamstim.data_root = self.hdf5_dir
+
+        np_services.MouseDirector.user = self.user.id
+        np_services.MouseDirector.mouse = self.mouse.id
+
+        np_services.OpenEphys.folder = self.session.folder
+
+        np_services.NewScaleCoordinateRecorder.log_root = self.session.npexp_path
+
+        self.configure_services()
+
+        super().initialize_and_test_services()
+
+    def copy_ephys(self) -> None:
+        # copy ephys       
+        password = np_config.fetch('/logins')['svc_neuropix']['password']
+        ssh = fabric.Connection(host=np_services.OpenEphys.host, user='svc_neuropix', connect_kwargs=dict(password=password))
+        for ephys_folder in np_services.OpenEphys.data_files:
+            if isinstance(self.session, np_session.TempletonPilotSession):
+                ephys_folder = next(ephys_folder.glob('Record Node*'))
+            with ssh:
+                ssh.run(
+                f'robocopy "{ephys_folder}" "{self.session.npexp_path / ephys_folder.name}" /j /s /xo' 
+                # /j unbuffered, /s incl non-empty subdirs, /xo exclude src files older than dest
+                )
+                
+    def copy_data_files(self) -> None:
+        """Copy files from raw data storage to session folder for all services
+        except Open Ephys."""
+        for service in self.services:
+            if service == self.imager:
+                # copy vimba files:
+                for file in np_services.get_files_created_between(
+                    path=np_services.config_from_zk()['ImageVimba']['data'],
+                    start=self.imager.initialization,
+                ): 
+                    shutil.copy2(file, self.session.npexp_path)
+                    npxc.validate_or_overwrite(self.session.npexp_path / file.name, file)
+            if service is np_services.ScriptCamstim:
+                np_services.ScriptCamstim.data_root = self.hdf5_dir
+            match service.__name__:
+                case "np_services.open_ephys":
+                    continue # copy ephys after other files
+                case _:
+                    files: Iterable[pathlib.Path] = service.data_files or service.get_latest_data('*')
+                    if not files:
+                        continue
+                    files = set(files)
+                    print(files)
+                    for file in files:
+                        shutil.copy2(file, self.session.npexp_path)
+                        npxc.validate_or_overwrite(self.session.npexp_path / file.name, file)
+    
+    #TODO move this to a dedicated np_service class instead of using ScriptCamstim
+    def run_stim_desktop_theme_script(self, selection: str) -> None:     
+        np_services.ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/ben/change_desktop.py'
+        np_services.ScriptCamstim.params = {'selection': selection}
+        np_services.ScriptCamstim.start()
+        while not np_services.ScriptCamstim.is_ready_to_start():
+            time.sleep(0.1)
+
+    set_grey_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'grey')
+    set_dark_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'dark')
+    reset_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'reset')
+
```

### Comparing `np_workflows-1.5.5/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim` & `np_workflows-1.6.0/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/src/np_workflows/shared/npxc.py` & `np_workflows-1.6.0/src/np_workflows/shared/npxc.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import datetime
 import inspect
 import pathlib
 import shutil
 import sys
 import time
 from typing import Any, Generator, Sequence, Type
+import zlib
 
 import fabric
 import np_config
 import np_logging
 import np_session
 from np_services import Initializable, Testable, TestError, Finalizable, Service
 from np_services import Sync, VideoMVR, ImageMVR, Cam3d, ScriptCamstim, OpenEphys  
@@ -166,8 +167,21 @@
     toggle_tb.send(None)
     def show_tracebacks():
         toggle_tb.send(False)
     def hide_tracebacks():
         toggle_tb.send(True)
         
 def now() -> str:
-    return np_services.utils.normalize_time(time.time())
+    return np_services.utils.normalize_time(time.time())
+
+def validate_or_overwrite(validate: str | pathlib.Path, src: str | pathlib.Path):
+    "Checksum validate against `src`, (over)write `validate` as `src` if different."
+    validate, src = pathlib.Path(validate), pathlib.Path(src)
+    def copy():
+        logger.debug("Copying %s to %s", src, validate)
+        shutil.copy2(src, validate)
+    while (
+        validate.exists() == False
+        or (v := zlib.crc32(validate.read_bytes())) != (c := zlib.crc32(pathlib.Path(src).read_bytes()))
+        ):
+        copy()
+    logger.debug("Validated %s CRC32: %08X", validate, (v & 0xFFFFFFFF) )
```

### Comparing `np_workflows-1.5.5/src/np_workflows/shared/widgets.py` & `np_workflows-1.6.0/src/np_workflows/shared/widgets.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/tests/logs/debug.log` & `np_workflows-1.6.0/tests/logs/debug.log`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/tests/logs/warning.log` & `np_workflows-1.6.0/tests/logs/warning.log`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/tests/widget_sandbox.ipynb` & `np_workflows-1.6.0/tests/widget_sandbox.ipynb`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.5/PKG-INFO` & `np_workflows-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: np-workflows
-Version: 1.5.5
+Version: 1.6.0
 Summary: Ecephys and behavior workflows for the Mindscope Neuropixels team.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Repository, https://github.com/AllenInstitute/np_workflows
 Project-URL: Issues, https://github.com/AllenInstitute/np_workflows/issues
 Requires-Python: ==3.11.*
-Requires-Dist: np-services>=0.1.47
+Requires-Dist: np-services>=0.1.53
 Requires-Dist: np-session>=0.6.5
 Requires-Dist: np-config>=0.4.20
 Requires-Dist: np-probe-targets>=0.0.11
 Requires-Dist: np-datajoint
 Requires-Dist: ipywidgets>=7
 Requires-Dist: pydantic<2,>=1
 Requires-Dist: jupyterlab>=3.6
```

