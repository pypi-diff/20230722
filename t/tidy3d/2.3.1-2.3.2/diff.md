# Comparing `tmp/tidy3d-2.3.1.tar.gz` & `tmp/tidy3d-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.3.1.tar", last modified: Fri Jul 14 19:13:34 2023, max compression
+gzip compressed data, was "tidy3d-2.3.2.tar", last modified: Sat Jul 22 16:50:36 2023, max compression
```

## Comparing `tidy3d-2.3.1.tar` & `tidy3d-2.3.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-14 19:13:15.000000 tidy3d-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 19:13:15.000000 tidy3d-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-14 19:13:34.001042 tidy3d-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-14 19:13:15.000000 tidy3d-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 19:13:15.000000 tidy3d-2.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:13:34.001042 tidy3d-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-14 19:13:15.000000 tidy3d-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    35660 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    54875 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47180 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21275 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    84194 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   147649 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)   124300 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   121570 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33009 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62878 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29109 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30578 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-22 16:50:20.000000 tidy3d-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-22 16:50:20.000000 tidy3d-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-22 16:50:36.368388 tidy3d-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-22 16:50:20.000000 tidy3d-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-22 16:50:20.000000 tidy3d-2.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:50:36.368388 tidy3d-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-22 16:50:20.000000 tidy3d-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35660 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54875 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47180 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21275 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84194 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147649 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124301 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33009 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62878 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29109 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30578 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.3.1/LICENSE` & `tidy3d-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/PKG-INFO` & `tidy3d-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.1
+Version: 2.3.2
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.1/README.md` & `tidy3d-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/setup.py` & `tidy3d-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.3.2/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/_test_local/_test_data_performance.py` & `tidy3d-2.3.2/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/_test_local/_test_fit_web.py` & `tidy3d-2.3.2/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.3.2/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/_test_local/_test_web.py` & `tidy3d-2.3.2/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_IO.py` & `tidy3d-2.3.2/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_apodization.py` & `tidy3d-2.3.2/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_base.py` & `tidy3d-2.3.2/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_boundaries.py` & `tidy3d-2.3.2/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_custom.py` & `tidy3d-2.3.2/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_field_projection.py` & `tidy3d-2.3.2/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_geometry.py` & `tidy3d-2.3.2/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_grid.py` & `tidy3d-2.3.2/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_grid_spec.py` & `tidy3d-2.3.2/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_medium.py` & `tidy3d-2.3.2/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_meshgenerate.py` & `tidy3d-2.3.2/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_mode.py` & `tidy3d-2.3.2/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_monitor.py` & `tidy3d-2.3.2/tests/test_components/test_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,32 +115,42 @@
     M = td.FieldProjectionAngleMonitor(
         size=(2, 2, 2), theta=[1], phi=[0], name="f", freqs=[2e12], exclude_surfaces=["x-", "y+"]
     ).projection_surfaces
     assert len(M) == 4
 
 
 def test_fieldproj_surfaces_in_simulaiton():
-    # test error if a projection surfaces is outside the simulation domain
-    M = td.FieldProjectionAngleMonitor(size=(1, 3, 3), theta=[1], phi=[0], name="f", freqs=[2e12])
+    # test error if all projection surfaces are outside the simulation domain
+    M = td.FieldProjectionAngleMonitor(size=(3, 3, 3), theta=[1], phi=[0], name="f", freqs=[2e12])
     with pytest.raises(pydantic.ValidationError):
         sim = td.Simulation(
             size=(2, 2, 2),
             run_time=1e-12,
             monitors=[M],
             grid_spec=td.GridSpec.uniform(0.1),
         )
-    # no error when outside surfaces are excluded
-    M = M.updated_copy(exclude_surfaces=["y-", "y+", "z-", "z+"])
+    # no error when some surfaces are in
+    M = M.updated_copy(size=(1, 3, 3))
     sim = td.Simulation(
         size=(2, 2, 2),
         run_time=1e-12,
         monitors=[M],
         grid_spec=td.GridSpec.uniform(0.1),
     )
 
+    # error when the surfaces that are in are excluded
+    M = M.updated_copy(exclude_surfaces=["x-", "x+"])
+    with pytest.raises(pydantic.ValidationError):
+        sim = td.Simulation(
+            size=(2, 2, 2),
+            run_time=1e-12,
+            monitors=[M],
+            grid_spec=td.GridSpec.uniform(0.1),
+        )
+
 
 def test_fieldproj_kspace_range():
     # make sure ux, uy are in [-1, 1] for k-space projection monitors
     with pytest.raises(pydantic.ValidationError):
         M = td.FieldProjectionKSpaceMonitor(
             size=(2, 0, 2), ux=[0.1, 2], uy=[0], name="f", freqs=[2e12], proj_axis=1
         )
```

### Comparing `tidy3d-2.3.1/tests/test_components/test_sidewall.py` & `tidy3d-2.3.2/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_simulation.py` & `tidy3d-2.3.2/tests/test_components/test_simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_source.py` & `tidy3d-2.3.2/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_types.py` & `tidy3d-2.3.2/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_components/test_viz.py` & `tidy3d-2.3.2/tests/test_components/test_viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_data/test_data_arrays.py` & `tidy3d-2.3.2/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_data/test_monitor_data.py` & `tidy3d-2.3.2/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_data/test_sim_data.py` & `tidy3d-2.3.2/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_package/test_config.py` & `tidy3d-2.3.2/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_package/test_log.py` & `tidy3d-2.3.2/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_package/test_make_script.py` & `tidy3d-2.3.2/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_package/test_material_library.py` & `tidy3d-2.3.2/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_package/test_parametric_variants.py` & `tidy3d-2.3.2/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_adjoint.py` & `tidy3d-2.3.2/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.3.2/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.3.2/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.3.2/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_polyslab.py` & `tidy3d-2.3.2/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.3.2/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_plugins/test_waveguide.py` & `tidy3d-2.3.2/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_cli.py` & `tidy3d-2.3.2/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_material_fitter.py` & `tidy3d-2.3.2/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.3.2/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.3.2/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.3.2/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/test_web/test_webapi.py` & `tidy3d-2.3.2/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tests/utils.py` & `tidy3d-2.3.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/__init__.py` & `tidy3d-2.3.2/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/__main__.py` & `tidy3d-2.3.2/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/apodization.py` & `tidy3d-2.3.2/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/base.py` & `tidy3d-2.3.2/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/boundary.py` & `tidy3d-2.3.2/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/data/data_array.py` & `tidy3d-2.3.2/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/data/dataset.py` & `tidy3d-2.3.2/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/data/monitor_data.py` & `tidy3d-2.3.2/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/data/sim_data.py` & `tidy3d-2.3.2/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/field_projection.py` & `tidy3d-2.3.2/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/geometry.py` & `tidy3d-2.3.2/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/grid/grid.py` & `tidy3d-2.3.2/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.3.2/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/grid/mesher.py` & `tidy3d-2.3.2/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/medium.py` & `tidy3d-2.3.2/tidy3d/components/medium.py`

 * *Files 0% similar despite different names*

```diff
@@ -1178,15 +1178,15 @@
         def make_grid(scalar_field: Union[ScalarFieldDataArray, SpatialDataArray]) -> Grid:
             """Make a grid for a single dataset."""
 
             def make_bound_coords(coords: np.ndarray, pt_min: float, pt_max: float) -> List[float]:
                 """Convert user supplied coords into boundary coords to use in :class:`.Grid`."""
 
                 # get coordinates of the bondaries halfway between user-supplied data
-                coord_bounds = (coords[1:] + coords[:1]) / 2.0
+                coord_bounds = (coords[1:] + coords[:-1]) / 2.0
 
                 # res-set coord boundaries that lie outside geometry bounds to the boundary (0 vol.)
                 coord_bounds[coord_bounds <= pt_min] = pt_min
                 coord_bounds[coord_bounds >= pt_max] = pt_max
 
                 # add the geometry bounds in explicitly
                 return [pt_min] + coord_bounds.tolist() + [pt_max]
```

### Comparing `tidy3d-2.3.1/tidy3d/components/mode.py` & `tidy3d-2.3.2/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/monitor.py` & `tidy3d-2.3.2/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/simulation.py` & `tidy3d-2.3.2/tidy3d/components/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -663,21 +663,19 @@
             return val
 
         sim_center = values.get("center")
         sim_size = values.get("size")
         sim_box = Box(size=sim_size, center=sim_center)
 
         for mnt in (mnt for mnt in val if isinstance(mnt, SurfaceIntegrationMonitor)):
-            for surface in mnt.integration_surfaces:
-                if not sim_box.intersects(surface):
-                    raise SetupError(
-                        f"Integration surface '{surface.name}' of monitor "
-                        f"'{mnt.name}' is outside of the simulation bounds. Modify monitor "
-                        "geometry or use 'exclude_surfaces' to exclude that surface."
-                    )
+            if not any(sim_box.intersects(surf) for surf in mnt.integration_surfaces):
+                raise SetupError(
+                    f"All integration surfaces of monitor '{mnt.name}' are outside of the "
+                    "simulation bounds."
+                )
 
         return val
 
     @pydantic.validator("monitors", always=True)
     def _projection_monitors_distance(cls, val, values):
         """Warn if the projection distance is large for exact projections."""
```

### Comparing `tidy3d-2.3.1/tidy3d/components/source.py` & `tidy3d-2.3.2/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/structure.py` & `tidy3d-2.3.2/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/transformation.py` & `tidy3d-2.3.2/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/types.py` & `tidy3d-2.3.2/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/validators.py` & `tidy3d-2.3.2/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/components/viz.py` & `tidy3d-2.3.2/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/config.py` & `tidy3d-2.3.2/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/constants.py` & `tidy3d-2.3.2/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/exceptions.py` & `tidy3d-2.3.2/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/log.py` & `tidy3d-2.3.2/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/material_library/material_library.py` & `tidy3d-2.3.2/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/material_library/material_reference.py` & `tidy3d-2.3.2/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.3.2/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
         adjoint_sources = []
         for amp, direction, freq, mode_index in zip(amps, directions, freqs, mode_indices):
 
             # TODO: figure out where this factor comes from
             k0 = 2 * np.pi * freq / C_0
             grad_const = k0 / 4 / ETA_0
             src_amp = grad_const * amp
+            if direction == "-":
+                src_amp *= -1
 
             src_direction = self.flip_direction(str(direction))
 
             adj_mode_src = ModeSource(
                 size=self.monitor.size,
                 center=self.monitor.center,
                 source_time=self.make_source_time(amp_complex=src_amp, freq=freq, fwidth=fwidth),
```

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.3.2/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.3.2/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/dispersion/web.py` & `tidy3d-2.3.2/tidy3d/plugins/dispersion/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.3.2/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.3.2/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/mode/solver.py` & `tidy3d-2.3.2/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.3.2/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/mode/web.py` & `tidy3d-2.3.2/tidy3d/plugins/mode/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.3.2/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.3.2/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.3.2/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.3.2/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/updater.py` & `tidy3d-2.3.2/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/asynchronous.py` & `tidy3d-2.3.2/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/cacert.pem` & `tidy3d-2.3.2/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/cli/app.py` & `tidy3d-2.3.2/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/cli/migrate.py` & `tidy3d-2.3.2/tidy3d/web/cli/migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 "workings of Tidy3D will remain the same.",
                 type=bool,
                 default=True,
             )
             if is_migrate:
                 headers = {"Application": "TIDY3D"}
                 resp = requests.get(
-                    f"{Env.current.auth_api_endpoint}/auth",
+                    f"{Env.current.web_api_endpoint}/auth",
                     headers=headers,
                     auth=(email, password),
                 )
                 if resp.status_code != 200:
                     click.echo(f"Migrate to api key failed: {resp.text}")
                     return False
                 else:
```

### Comparing `tidy3d-2.3.1/tidy3d/web/container.py` & `tidy3d-2.3.2/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/environment.py` & `tidy3d-2.3.2/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/http_management.py` & `tidy3d-2.3.2/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/httputils.py` & `tidy3d-2.3.2/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/material_fitter.py` & `tidy3d-2.3.2/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/material_libray.py` & `tidy3d-2.3.2/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/s3utils.py` & `tidy3d-2.3.2/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/simulation_task.py` & `tidy3d-2.3.2/tidy3d/web/simulation_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/task.py` & `tidy3d-2.3.2/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/types.py` & `tidy3d-2.3.2/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d/web/webapi.py` & `tidy3d-2.3.2/tidy3d/web/webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.3.2/tidy3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.1
+Version: 2.3.2
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.1/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.3.2/tidy3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.1/tidy3d.egg-info/requires.txt` & `tidy3d-2.3.2/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

