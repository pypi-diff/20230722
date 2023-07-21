# Comparing `tmp/dsspy-2.2.7.tar.gz` & `tmp/dsspy-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyDSS/PyDSS/dist/.tmp-iiu0lz3s/dsspy-2.2.7.tar", last modified: Mon Jun 12 21:40:42 2023, max compression
+gzip compressed data, was "/home/runner/work/PyDSS/PyDSS/dist/.tmp-krmgk6bg/dsspy-2.2.8.tar", last modified: Fri Jul 21 22:57:44 2023, max compression
```

## Comparing `dsspy-2.2.7.tar` & `dsspy-2.2.8.tar`

### file list

```diff
@@ -1,217 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-12 21:40:29.000000 dsspy-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 21:40:42.000000 dsspy-2.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/Extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/Extensions/MonteCarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/Extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3014 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/NetworkModifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/ProfileManager/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/ProfileInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/base_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/ProfileManager/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/hooks/MongoDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ProfileManager/hooks/h5.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/ResultData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/SolveMode.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/api/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/api/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/api/src/app/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/DataWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/HDF5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/JSON_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/Tester.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/arrow_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/app/pydss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/api/src/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/web/create_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/web/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/api/src/web/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/add_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/create_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/edit_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/pydss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/cli/run_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dataset_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/defaults/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/ExportMode-byClass.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/ExportMode-byElement.toml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/Exports.toml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/Subscriptions.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/ExportLists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/defaults/Monte_Carlo/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/Monte_Carlo/MonteCarloSettings.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/Monte_Carlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/plots.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/FaultController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/GenController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/MotorStall.toml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/PvController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/SocketController.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/StorageController.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyControllerList/xfmrController.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/FrequencySweep.toml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/Histogram.toml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/NetworkGraph.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/Table.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/ThreeDim.toml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/TimeSeries.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/Topology.toml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/VoltageDistance.toml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/XY.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/defaults/pyPlotList/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssBus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssCircuit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6380 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssElement.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssElementFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    30519 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssObjectBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/dssTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/element_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/element_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/export_list_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/get_snapshot_timepoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/helics_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    44407 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/modes/Dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/modes/QSTS.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/modes/Snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/modes/solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/naerm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/node_voltage_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyContrReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyControllers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/FaultController.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/GenController.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/HybridController.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/MotorStall.py
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/PvController.py
--rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/Settings/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/SocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/StorageController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/ThermostaticLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/Controllers/xfmrController.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/pyController.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyControllers/pyControllerAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyDSS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyLogger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlotReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyPlots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/FrequencySweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/Histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/NetworkGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/ThreeDim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/Topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/VoltageDistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/XY.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/Plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/pyPlotAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPlots/pyPlots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
--rw-r--r--   0 runner    (1001) docker     (123)    20893 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/pyPostprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyPostprocessor/pyPostprocessAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pyResults.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pydss_fs_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30773 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pydss_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    38195 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/pydss_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/capacitor_change_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/feeder_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/pv_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/reg_control_tap_number_change_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/thermal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/reports/voltage_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/simulation_input_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/storage_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/thermal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/unitDefinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/PyDSS/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/dss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/pydss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/timing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-06-12 21:40:29.000000 dsspy-2.2.7/PyDSS/value_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 21:40:42.000000 dsspy-2.2.7/dsspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:40:42.000000 dsspy-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-12 21:40:29.000000 dsspy-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:40:42.000000 dsspy-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_auto_snapshot_time_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_custom_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_dataset_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_element_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_export_list_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_independent_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_opendss_export_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_opendss_export_powers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_pv_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_pydss_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_pydss_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-12 21:40:29.000000 dsspy-2.2.7/tests/test_space_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-21 22:57:35.000000 dsspy-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 22:57:44.000000 dsspy-2.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/Extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/Extensions/MonteCarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/Extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3014 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/NetworkModifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/ProfileManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/ProfileInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/base_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ProfileManager/hooks/h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/ResultData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/SolveMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/DataWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/HDF5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/JSON_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/Tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/arrow_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/app/pydss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/api/src/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/create_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/api/src/web/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/apps/data_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/add_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/create_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/edit_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/pydss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/cli/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dataset_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byClass.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byElement.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/Exports.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/Subscriptions.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/ExportLists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/MonteCarloSettings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/Monte_Carlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/plots.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/FaultController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/GenController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/MotorStall.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/SocketController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/StorageController.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyControllerList/xfmrController.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/FrequencySweep.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Histogram.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/NetworkGraph.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Table.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/ThreeDim.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/TimeSeries.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/Topology.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/VoltageDistance.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/XY.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/defaults/pyPlotList/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssBus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssCircuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6380 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssElementFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30519 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssObjectBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/dssTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/element_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/element_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/export_list_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/get_snapshot_timepoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/helics_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44407 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/Dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/QSTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/Snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/modes/solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/naerm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/node_voltage_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyContrReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/FaultController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/GenController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/HybridController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/MotorStall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24135 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/SocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/StorageController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/ThermostaticLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/Controllers/xfmrController.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/pyController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyControllers/pyControllerAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyDSS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyLogger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlotReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPlots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/FrequencySweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/NetworkGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/ThreeDim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/Topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/VoltageDistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/XY.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/Plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/pyPlotAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPlots/pyPlots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20893 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocessAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pyResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_fs_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30773 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38195 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/pydss_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/capacitor_change_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/feeder_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/pv_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/reg_control_tap_number_change_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/thermal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/reports/voltage_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/simulation_input_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/storage_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/thermal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/unitDefinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/PyDSS/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/dss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/pydss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/timing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-07-21 22:57:35.000000 dsspy-2.2.8/PyDSS/value_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 22:57:44.000000 dsspy-2.2.8/dsspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:57:44.000000 dsspy-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-21 22:57:35.000000 dsspy-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:57:44.000000 dsspy-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_auto_snapshot_time_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_custom_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_dataset_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_element_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_export_list_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_independent_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_opendss_export_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_opendss_export_powers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pv_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pydss_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_pydss_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 22:57:35.000000 dsspy-2.2.8/tests/test_space_estimation.py
```

### Comparing `dsspy-2.2.7/LICENSE` & `dsspy-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PKG-INFO` & `dsspy-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsspy
-Version: 2.2.7
+Version: 2.2.8
 Summary: A high-level python interface for OpenDSS
 Home-page: http://www.github.com/nrel/pydss
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `dsspy-2.2.7/PyDSS/Extensions/MonteCarlo.py` & `dsspy-2.2.8/PyDSS/Extensions/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/NetworkModifier.py` & `dsspy-2.2.8/PyDSS/NetworkModifier.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/ProfileManager/ProfileInterface.py` & `dsspy-2.2.8/PyDSS/ProfileManager/ProfileInterface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/ProfileManager/base_definitions.py` & `dsspy-2.2.8/PyDSS/ProfileManager/base_definitions.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/ProfileManager/hooks/MongoDB.py` & `dsspy-2.2.8/PyDSS/ProfileManager/hooks/MongoDB.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/ProfileManager/hooks/h5.py` & `dsspy-2.2.8/PyDSS/ProfileManager/hooks/h5.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/ResultData.py` & `dsspy-2.2.8/PyDSS/ResultData.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/SolveMode.py` & `dsspy-2.2.8/PyDSS/SolveMode.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/server.py` & `dsspy-2.2.8/PyDSS/api/server.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/DataWriter.py` & `dsspy-2.2.8/PyDSS/api/src/app/DataWriter.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/HDF5.py` & `dsspy-2.2.8/PyDSS/api/src/app/HDF5.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/JSON_writer.py` & `dsspy-2.2.8/PyDSS/api/src/app/JSON_writer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/Tester.py` & `dsspy-2.2.8/PyDSS/api/src/app/Tester.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/arrow_writer.py` & `dsspy-2.2.8/PyDSS/api/src/app/arrow_writer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/app/pydss.py` & `dsspy-2.2.8/PyDSS/api/src/app/pydss.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/web/handler.py` & `dsspy-2.2.8/PyDSS/api/src/web/handler.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/api/src/web/parser.py` & `dsspy-2.2.8/PyDSS/api/src/web/parser.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/add_post_process.py` & `dsspy-2.2.8/PyDSS/cli/add_post_process.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/controllers.py` & `dsspy-2.2.8/PyDSS/cli/controllers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/convert.py` & `dsspy-2.2.8/PyDSS/cli/convert.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/create_project.py` & `dsspy-2.2.8/PyDSS/cli/create_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/edit_scenario.py` & `dsspy-2.2.8/PyDSS/cli/edit_scenario.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/export.py` & `dsspy-2.2.8/PyDSS/cli/export.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/extract.py` & `dsspy-2.2.8/PyDSS/cli/extract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/pydss.py` & `dsspy-2.2.8/PyDSS/cli/pydss.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/reports.py` & `dsspy-2.2.8/PyDSS/cli/reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/run.py` & `dsspy-2.2.8/PyDSS/cli/run.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/cli/run_server.py` & `dsspy-2.2.8/PyDSS/cli/run_server.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/common.py` & `dsspy-2.2.8/PyDSS/common.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/config_data.py` & `dsspy-2.2.8/PyDSS/config_data.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/controllers.py` & `dsspy-2.2.8/PyDSS/controllers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dataset_buffer.py` & `dsspy-2.2.8/PyDSS/dataset_buffer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/defaults/ExportLists/ExportMode-byClass.toml` & `dsspy-2.2.8/PyDSS/defaults/ExportLists/ExportMode-byClass.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/defaults/ExportLists/Exports.toml` & `dsspy-2.2.8/PyDSS/defaults/ExportLists/Exports.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/defaults/plots.toml` & `dsspy-2.2.8/PyDSS/defaults/plots.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml` & `dsspy-2.2.8/PyDSS/defaults/pyControllerList/PvVoltageRideThru.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/defaults/pyControllerList/StorageController.toml` & `dsspy-2.2.8/PyDSS/defaults/pyControllerList/StorageController.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssBus.py` & `dsspy-2.2.8/PyDSS/dssBus.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssCircuit.py` & `dsspy-2.2.8/PyDSS/dssCircuit.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssElement.py` & `dsspy-2.2.8/PyDSS/dssElement.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssInstance.py` & `dsspy-2.2.8/PyDSS/dssInstance.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssObjectBase.py` & `dsspy-2.2.8/PyDSS/dssObjectBase.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/dssTransformer.py` & `dsspy-2.2.8/PyDSS/dssTransformer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/element_fields.py` & `dsspy-2.2.8/PyDSS/element_fields.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/element_options.py` & `dsspy-2.2.8/PyDSS/element_options.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/exceptions.py` & `dsspy-2.2.8/PyDSS/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/export_list_reader.py` & `dsspy-2.2.8/PyDSS/export_list_reader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/get_snapshot_timepoints.py` & `dsspy-2.2.8/PyDSS/get_snapshot_timepoints.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/helics_interface.py` & `dsspy-2.2.8/PyDSS/helics_interface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/loggers.py` & `dsspy-2.2.8/PyDSS/loggers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/metrics.py` & `dsspy-2.2.8/PyDSS/metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/modes/Dynamic.py` & `dsspy-2.2.8/PyDSS/modes/Dynamic.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/modes/QSTS.py` & `dsspy-2.2.8/PyDSS/modes/QSTS.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/modes/Snapshot.py` & `dsspy-2.2.8/PyDSS/modes/Snapshot.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/modes/solver_base.py` & `dsspy-2.2.8/PyDSS/modes/solver_base.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/naerm.py` & `dsspy-2.2.8/PyDSS/naerm.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/node_voltage_metrics.py` & `dsspy-2.2.8/PyDSS/node_voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyContrReader.py` & `dsspy-2.2.8/PyDSS/pyContrReader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/FaultController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/FaultController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/GenController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/GenController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/HybridController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/HybridController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/MotorStall.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/MotorStall.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/PvController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/PvVoltageRideThru.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/Settings/PvControllers.toml`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/SocketController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/SocketController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/StorageController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/StorageController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/ThermostaticLoad.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/ThermostaticLoad.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/Controllers/xfmrController.py` & `dsspy-2.2.8/PyDSS/pyControllers/Controllers/xfmrController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyControllers/pyController.py` & `dsspy-2.2.8/PyDSS/pyControllers/pyController.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyDSS.py` & `dsspy-2.2.8/PyDSS/pyDSS.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyLogger.py` & `dsspy-2.2.8/PyDSS/pyLogger.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlotReader.py` & `dsspy-2.2.8/PyDSS/pyPlotReader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/FrequencySweep.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/FrequencySweep.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/Histogram.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/Histogram.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/NetworkGraph.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/NetworkGraph.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/Table.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/Table.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/ThreeDim.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/ThreeDim.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/TimeSeries.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/Topology.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/Topology.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/VoltageDistance.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/VoltageDistance.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/Plots/XY.py` & `dsspy-2.2.8/PyDSS/pyPlots/Plots/XY.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/pyPlotAbstract.py` & `dsspy-2.2.8/PyDSS/pyPlots/pyPlotAbstract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPlots/pyPlots.py` & `dsspy-2.2.8/PyDSS/pyPlots/pyPlots.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/EdLiFoControl.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/PostprocessScripts/Utilidata_Interface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/pyPostprocess.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocess.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyPostprocessor/pyPostprocessAbstract.py` & `dsspy-2.2.8/PyDSS/pyPostprocessor/pyPostprocessAbstract.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pyResults.py` & `dsspy-2.2.8/PyDSS/pyResults.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pydss_fs_interface.py` & `dsspy-2.2.8/PyDSS/pydss_fs_interface.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pydss_project.py` & `dsspy-2.2.8/PyDSS/pydss_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/pydss_results.py` & `dsspy-2.2.8/PyDSS/pydss_results.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/registry.py` & `dsspy-2.2.8/PyDSS/registry.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/capacitor_change_count.py` & `dsspy-2.2.8/PyDSS/reports/capacitor_change_count.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/feeder_losses.py` & `dsspy-2.2.8/PyDSS/reports/feeder_losses.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/pv_reports.py` & `dsspy-2.2.8/PyDSS/reports/pv_reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/reg_control_tap_number_change_count.py` & `dsspy-2.2.8/PyDSS/reports/reg_control_tap_number_change_count.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/reports.py` & `dsspy-2.2.8/PyDSS/reports/reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/thermal_metrics.py` & `dsspy-2.2.8/PyDSS/reports/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/reports/voltage_metrics.py` & `dsspy-2.2.8/PyDSS/reports/voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/simulation_input_models.py` & `dsspy-2.2.8/PyDSS/simulation_input_models.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/storage_filters.py` & `dsspy-2.2.8/PyDSS/storage_filters.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/thermal_metrics.py` & `dsspy-2.2.8/PyDSS/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/unitDefinations.py` & `dsspy-2.2.8/PyDSS/unitDefinations.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/dataframe_utils.py` & `dsspy-2.2.8/PyDSS/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/dss_utils.py` & `dsspy-2.2.8/PyDSS/utils/dss_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/pydss_utils.py` & `dsspy-2.2.8/PyDSS/utils/pydss_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/simulation_utils.py` & `dsspy-2.2.8/PyDSS/utils/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/timing_utils.py` & `dsspy-2.2.8/PyDSS/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/utils/utils.py` & `dsspy-2.2.8/PyDSS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/PyDSS/value_storage.py` & `dsspy-2.2.8/PyDSS/value_storage.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/dsspy.egg-info/PKG-INFO` & `dsspy-2.2.8/dsspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsspy
-Version: 2.2.7
+Version: 2.2.8
 Summary: A high-level python interface for OpenDSS
 Home-page: http://www.github.com/nrel/pydss
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `dsspy-2.2.7/dsspy.egg-info/SOURCES.txt` & `dsspy-2.2.8/dsspy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 PyDSS/api/src/app/__init__.py
 PyDSS/api/src/app/arrow_writer.py
 PyDSS/api/src/app/pydss.py
 PyDSS/api/src/web/__init__.py
 PyDSS/api/src/web/create_schema.py
 PyDSS/api/src/web/handler.py
 PyDSS/api/src/web/parser.py
+PyDSS/apps/__init__.py
+PyDSS/apps/data_viewer.py
 PyDSS/cli/__init__.py
 PyDSS/cli/add_post_process.py
 PyDSS/cli/controllers.py
 PyDSS/cli/convert.py
 PyDSS/cli/create_project.py
 PyDSS/cli/edit_scenario.py
 PyDSS/cli/export.py
```

### Comparing `dsspy-2.2.7/setup.py` & `dsspy-2.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/common.py` & `dsspy-2.2.8/tests/common.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_auto_snapshot_time_point.py` & `dsspy-2.2.8/tests/test_auto_snapshot_time_point.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_custom_exports.py` & `dsspy-2.2.8/tests/test_custom_exports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_dataset_buffer.py` & `dsspy-2.2.8/tests/test_dataset_buffer.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_export_list_reader.py` & `dsspy-2.2.8/tests/test_export_list_reader.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_metrics.py` & `dsspy-2.2.8/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_opendss_export_overloads.py` & `dsspy-2.2.8/tests/test_opendss_export_overloads.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_opendss_export_powers.py` & `dsspy-2.2.8/tests/test_opendss_export_powers.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_pv_reports.py` & `dsspy-2.2.8/tests/test_pv_reports.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_pydss_examples.py` & `dsspy-2.2.8/tests/test_pydss_examples.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_pydss_project.py` & `dsspy-2.2.8/tests/test_pydss_project.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_registry.py` & `dsspy-2.2.8/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `dsspy-2.2.7/tests/test_space_estimation.py` & `dsspy-2.2.8/tests/test_space_estimation.py`

 * *Files identical despite different names*

