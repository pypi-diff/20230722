# Comparing `tmp/pollination-annual-daylight-enhanced.full-0.0.2.tar.gz` & `tmp/pollination-annual-daylight-enhanced.full-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollination-annual-daylight-enhanced.full-0.0.2.tar", last modified: Tue Jun 27 15:01:07 2023, max compression
+gzip compressed data, was "pollination-annual-daylight-enhanced.full-0.0.3.tar", last modified: Sat Jul 22 08:11:19 2023, max compression
```

## Comparing `pollination-annual-daylight-enhanced.full-0.0.2.tar` & `pollination-annual-daylight-enhanced.full-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/pollination/annual_daylight_enhanced/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination/annual_daylight_enhanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination/annual_daylight_enhanced/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 15:01:07.000000 pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:01:07.578683 pollination-annual-daylight-enhanced.full-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 15:00:08.000000 pollination-annual-daylight-enhanced.full-0.0.2/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.476868 pollination-annual-daylight-enhanced.full-0.0.3/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/pollination/annual_daylight_enhanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination/annual_daylight_enhanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination/annual_daylight_enhanced/_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination/annual_daylight_enhanced/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 08:11:19.000000 pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 08:11:19.484867 pollination-annual-daylight-enhanced.full-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:11:19.480867 pollination-annual-daylight-enhanced.full-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-22 08:10:34.000000 pollination-annual-daylight-enhanced.full-0.0.3/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/.github/workflows/ci.yaml` & `pollination-annual-daylight-enhanced.full-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/.github/workflows/tests.yaml` & `pollination-annual-daylight-enhanced.full-0.0.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/LICENSE` & `pollination-annual-daylight-enhanced.full-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/PKG-INFO` & `pollination-annual-daylight-enhanced.full-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-enhanced.full
-Version: 0.0.2
+Version: 0.0.3
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-enhanced
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/README.md` & `pollination-annual-daylight-enhanced.full-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/pollination/annual_daylight_enhanced/entry.py` & `pollination-annual-daylight-enhanced.full-0.0.3/pollination/annual_daylight_enhanced/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from pollination_dsl.dag import Inputs, DAG, task, Outputs
 from dataclasses import dataclass
 from pollination.two_phase_daylight_coefficient import TwoPhaseDaylightCoefficientEntryPoint
-from pollination.honeybee_radiance_postprocess.post_process import AnnualDaylightMetrics
-from pollination.honeybee_display.translate import ModelToVis
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.wea import wea_input_timestep_check
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
 from pollination.alias.inputs.schedule import schedule_csv_input
+from pollination.alias.inputs.postprocess import grid_metrics_input
 from pollination.alias.outputs.daylight import daylight_autonomy_results, \
     continuous_daylight_autonomy_results, \
-    udi_results, udi_lower_results, udi_upper_results
+    udi_results, udi_lower_results, udi_upper_results, grid_metrics_results
+
+from ._post_process import AnnualDaylightPostProcess
 
 
 @dataclass
 class AnnualDaylightEntryPoint(DAG):
     """Annual daylight entry point."""
 
     # inputs
@@ -91,63 +92,69 @@
         'threshold. The default is -t 300 -lt 100 -ut 3000. The order of the keys is '
         'not important and you can include one or all of them. For instance if you only '
         'want to change the upper threshold to 2000 lux you should use -ut 2000 as '
         'the input.', default='-t 300 -lt 100 -ut 3000',
         alias=daylight_thresholds_input
     )
 
+    grid_metrics = Inputs.file(
+        description='A JSON file with additional custom metrics to calculate.',
+        extensions=['json'], optional=True, alias=grid_metrics_input
+    )
+
     @task(
         template=TwoPhaseDaylightCoefficientEntryPoint
     )
     def run_two_phase_daylight_coefficient(
             self, north=north, cpu_count=cpu_count, min_sensor_count=min_sensor_count,
             radiance_parameters=radiance_parameters, grid_filter=grid_filter,
             model=model, wea=wea
     ):
         pass
 
     @task(
-        template=AnnualDaylightMetrics,
+        template=AnnualDaylightPostProcess,
         needs=[run_two_phase_daylight_coefficient]
     )
-    def calculate_annual_metrics(
-        self, folder='results',
-        schedule=schedule, thresholds=thresholds
+    def annual_metrics_postprocess(
+        self, model=model, results='results', grids_info='results/grids_info.json',
+        schedule=schedule, thresholds=thresholds, grid_metrics=grid_metrics
     ):
         return [
             {
-                'from': AnnualDaylightMetrics()._outputs.annual_metrics,
+                'from': AnnualDaylightPostProcess()._outputs.metrics,
                 'to': 'metrics'
-            }
-        ]
-
-    @task(template=ModelToVis, needs=[calculate_annual_metrics])
-    def create_vsf(
-        self, model=model, grid_data='metrics', active_grid_data='udi',
-        output_format='vsf'
-    ):
-        return [
+            },
             {
-                'from': ModelToVis()._outputs.output_file,
+                'from': AnnualDaylightPostProcess()._outputs.grid_summary,
+                'to': 'grid_summary.csv'
+            },
+            {
+                'from': AnnualDaylightPostProcess()._outputs.visualization,
                 'to': 'visualization.vsf'
             }
         ]
 
     visualization = Outputs.file(
         source='visualization.vsf',
         description='Annual daylight result visualization in VisualizationSet format.'
     )
 
+    metrics = Outputs.folder(
+        source='metrics', description='Annual metrics folder.'
+    )
+
     results = Outputs.folder(
         source='results', description='Folder with raw result files (.ill) that '
         'contain illuminance matrices for each sensor at each timestep of the analysis.'
     )
 
-    metrics = Outputs.folder(
-        source='metrics', description='Annual metrics folder.'
+    grid_summary = Outputs.file(
+        source='grid_summary.csv', description='Grid summary of metrics.',
+        alias=grid_metrics_results
     )
 
     da = Outputs.folder(
         source='metrics/da', description='Daylight autonomy results.',
         alias=daylight_autonomy_results
     )
```

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/PKG-INFO` & `pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-enhanced.full
-Version: 0.0.2
+Version: 0.0.3
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-enhanced
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/pollination_annual_daylight_enhanced.full.egg-info/SOURCES.txt` & `pollination-annual-daylight-enhanced.full-0.0.3/pollination_annual_daylight_enhanced.full.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/tests.yaml
 pollination/annual_daylight_enhanced/__init__.py
+pollination/annual_daylight_enhanced/_post_process.py
 pollination/annual_daylight_enhanced/entry.py
 pollination_annual_daylight_enhanced.full.egg-info/PKG-INFO
 pollination_annual_daylight_enhanced.full.egg-info/SOURCES.txt
 pollination_annual_daylight_enhanced.full.egg-info/dependency_links.txt
 pollination_annual_daylight_enhanced.full.egg-info/not-zip-safe
 pollination_annual_daylight_enhanced.full.egg-info/requires.txt
 pollination_annual_daylight_enhanced.full.egg-info/top_level.txt
```

### Comparing `pollination-annual-daylight-enhanced.full-0.0.2/setup.py` & `pollination-annual-daylight-enhanced.full-0.0.3/setup.py`

 * *Files identical despite different names*

