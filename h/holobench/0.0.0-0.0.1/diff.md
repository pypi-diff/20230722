# Comparing `tmp/holobench-0.0.0.tar.gz` & `tmp/holobench-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-0.0.0.tar` & `holobench-0.0.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0      346 2023-07-22 11:01:59.628200 holobench-0.0.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1395 2023-07-22 11:01:59.628200 holobench-0.0.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.0/.gitignore
--rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.0/.pylintrc
--rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      713 2023-07-22 09:13:13.899071 holobench-0.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.0/LICENSE
--rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.0/README.md
--rw-r--r--   0        0        0      789 2023-07-22 11:02:06.336212 holobench-0.0.0/bencher/__init__.py
--rw-r--r--   0        0        0    25862 2023-07-22 09:13:13.899071 holobench-0.0.0/bencher/bench_cfg.py
--rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.0/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.0/bencher/bench_vars.py
--rw-r--r--   0        0        0    27767 2023-07-22 09:34:45.468154 holobench-0.0.0/bencher/bencher.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.0/bencher/example/__init__.py
--rw-r--r--   0        0        0     4168 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_float2D_scatter.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_float3D_cone.py
--rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_floats.py
--rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     4101 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/example/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/example/example_interactive.py
--rw-r--r--   0        0        0     2415 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_kwargs.py
--rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_persistent.py
--rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.0/bencher/example/example_plot_library.py
--rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.0/bencher/example/example_template.py
--rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.0/bencher/example/example_vector.py
--rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/example/example_workflow.py
--rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/example/hv_bool_bug.py
--rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.0/bencher/plotting/plot_collection.py
--rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plot_library.py
--rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plot_types.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/plots/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/plots/catplot.py
--rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.0/bencher/plotting/plots/heatmap.py
--rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plots/hv_interactive.py
--rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plots/lineplot.py
--rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.0/bencher/plotting/plots/plot_base.py
--rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/plots/scatterplot.py
--rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plots/surface.py
--rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/plotting/plots/tables.py
--rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting/plots/volume.py
--rw-r--r--   0        0        0    10787 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plotting_functions.py
--rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.0/bencher/plt_cfg.py
--rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.0/bencher/utils.py
--rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.0/dependencies.yaml
--rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.0/package.xml
--rw-r--r--   0        0        0     1519 2023-07-22 11:16:30.847502 holobench-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.0/resource/bencher
--rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.0/setup.cfg
--rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.0/setup.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.0/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.0/test/plots/__init__.py
--rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.0/test/plots/test_catplot.py
--rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.0/test/plots/test_plots_common.py
--rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.0/test/plots/test_tables.py
--rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.0/test/test_bench_examples.py
--rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_bencher.py
--rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_combinations.py
--rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_plot_collection.py
--rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_plot_filter.py
--rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_plot_library.py
--rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_sample_cache.py
--rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_sweep_vars.py
--rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_utils.py
--rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.0/test/test_vars.py
--rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 holobench-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-07-22 11:01:59.628200 holobench-0.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1395 2023-07-22 11:01:59.628200 holobench-0.0.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.1/.gitignore
+-rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.1/.pylintrc
+-rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      713 2023-07-22 09:13:13.899071 holobench-0.0.1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.1/README.md
+-rw-r--r--   0        0        0      789 2023-07-22 11:20:01.088575 holobench-0.0.1/bencher/__init__.py
+-rw-r--r--   0        0        0    25862 2023-07-22 09:13:13.899071 holobench-0.0.1/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.1/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.1/bencher/bench_vars.py
+-rw-r--r--   0        0        0    27767 2023-07-22 09:34:45.468154 holobench-0.0.1/bencher/bencher.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.1/bencher/example/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_float2D_scatter.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_float3D_cone.py
+-rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     4101 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/example/example_holosweep.py
+-rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/example/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/example/example_interactive.py
+-rw-r--r--   0        0        0     2415 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_kwargs.py
+-rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_persistent.py
+-rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.1/bencher/example/example_plot_library.py
+-rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.1/bencher/example/example_template.py
+-rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.1/bencher/example/example_vector.py
+-rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/example/hv_bool_bug.py
+-rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.1/bencher/plotting/plot_collection.py
+-rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plot_library.py
+-rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plot_types.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/plots/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/plots/catplot.py
+-rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.1/bencher/plotting/plots/heatmap.py
+-rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plots/hv_interactive.py
+-rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plots/lineplot.py
+-rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.1/bencher/plotting/plots/plot_base.py
+-rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/plots/scatterplot.py
+-rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plots/surface.py
+-rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/plotting/plots/tables.py
+-rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting/plots/volume.py
+-rw-r--r--   0        0        0    10787 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plotting_functions.py
+-rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.1/bencher/plt_cfg.py
+-rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.1/bencher/utils.py
+-rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.1/dependencies.yaml
+-rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.1/package.xml
+-rw-r--r--   0        0        0     1531 2023-07-22 11:19:40.792470 holobench-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.1/resource/bencher
+-rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.1/setup.cfg
+-rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.1/setup.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.1/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.1/test/plots/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.1/test/plots/test_catplot.py
+-rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.1/test/plots/test_plots_common.py
+-rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.1/test/plots/test_tables.py
+-rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.1/test/test_bench_examples.py
+-rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_bencher.py
+-rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_combinations.py
+-rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_plot_collection.py
+-rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_plot_filter.py
+-rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_plot_library.py
+-rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_sample_cache.py
+-rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_sweep_vars.py
+-rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_utils.py
+-rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.1/test/test_vars.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 holobench-0.0.1/PKG-INFO
```

### Comparing `holobench-0.0.0/.devcontainer/devcontainer.json` & `holobench-0.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/.github/workflows/ci.yml` & `holobench-0.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/.gitignore` & `holobench-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/.vscode/tasks.json` & `holobench-0.0.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/LICENSE` & `holobench-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/README.md` & `holobench-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/__init__.py` & `holobench-0.0.1/bencher/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 
 from .bencher import Bench, BenchCfg, BenchRunCfg
 from .plt_cfg import BenchPlotter, PltCfgBase
 from .example.benchmark_data import ExampleBenchCfgIn, ExampleBenchCfgOut, bench_function
 from .bench_plot_server import BenchPlotServer
 from .bench_vars import (
     IntSweep,
```

### Comparing `holobench-0.0.0/bencher/bench_cfg.py` & `holobench-0.0.1/bencher/bench_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/bench_plot_server.py` & `holobench-0.0.1/bencher/bench_plot_server.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/bench_vars.py` & `holobench-0.0.1/bencher/bench_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/bencher.py` & `holobench-0.0.1/bencher/bencher.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/benchmark_data.py` & `holobench-0.0.1/bencher/example/benchmark_data.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_categorical.py` & `holobench-0.0.1/bencher/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_custom_sweep.py` & `holobench-0.0.1/bencher/example/example_custom_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_float2D_scatter.py` & `holobench-0.0.1/bencher/example/example_float2D_scatter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_float3D.py` & `holobench-0.0.1/bencher/example/example_float3D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_float3D_cone.py` & `holobench-0.0.1/bencher/example/example_float3D_cone.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_float_cat.py` & `holobench-0.0.1/bencher/example/example_float_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_floats.py` & `holobench-0.0.1/bencher/example/example_floats.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_floats2D.py` & `holobench-0.0.1/bencher/example/example_floats2D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_holosweep.py` & `holobench-0.0.1/bencher/example/example_holosweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_hvplot_explorer.py` & `holobench-0.0.1/bencher/example/example_hvplot_explorer.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_interactive.py` & `holobench-0.0.1/bencher/example/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_kwargs.py` & `holobench-0.0.1/bencher/example/example_kwargs.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_pareto.py` & `holobench-0.0.1/bencher/example/example_pareto.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_persistent.py` & `holobench-0.0.1/bencher/example/example_persistent.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_plot_library.py` & `holobench-0.0.1/bencher/example/example_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_sample_cache.py` & `holobench-0.0.1/bencher/example/example_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_sample_cache_context.py` & `holobench-0.0.1/bencher/example/example_sample_cache_context.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_simple.py` & `holobench-0.0.1/bencher/example/example_simple.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_simple_bool.py` & `holobench-0.0.1/bencher/example/example_simple_bool.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_simple_cat.py` & `holobench-0.0.1/bencher/example/example_simple_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_simple_float.py` & `holobench-0.0.1/bencher/example/example_simple_float.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_template.py` & `holobench-0.0.1/bencher/example/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_time_event.py` & `holobench-0.0.1/bencher/example/example_time_event.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_vector.py` & `holobench-0.0.1/bencher/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/example_workflow.py` & `holobench-0.0.1/bencher/example/example_workflow.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/example/hv_bool_bug.py` & `holobench-0.0.1/bencher/example/hv_bool_bug.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/optuna_conversions.py` & `holobench-0.0.1/bencher/optuna_conversions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plot_collection.py` & `holobench-0.0.1/bencher/plotting/plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plot_filter.py` & `holobench-0.0.1/bencher/plotting/plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plot_library.py` & `holobench-0.0.1/bencher/plotting/plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plot_types.py` & `holobench-0.0.1/bencher/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/catplot.py` & `holobench-0.0.1/bencher/plotting/plots/catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/heatmap.py` & `holobench-0.0.1/bencher/plotting/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/hv_interactive.py` & `holobench-0.0.1/bencher/plotting/plots/hv_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/lineplot.py` & `holobench-0.0.1/bencher/plotting/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/plot_base.py` & `holobench-0.0.1/bencher/plotting/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/scatterplot.py` & `holobench-0.0.1/bencher/plotting/plots/scatterplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/surface.py` & `holobench-0.0.1/bencher/plotting/plots/surface.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/tables.py` & `holobench-0.0.1/bencher/plotting/plots/tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting/plots/volume.py` & `holobench-0.0.1/bencher/plotting/plots/volume.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plotting_functions.py` & `holobench-0.0.1/bencher/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/plt_cfg.py` & `holobench-0.0.1/bencher/plt_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/bencher/utils.py` & `holobench-0.0.1/bencher/utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/package.xml` & `holobench-0.0.1/package.xml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/pyproject.toml` & `holobench-0.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 dependencies = [
   "holoviews[reccomended]==1.16.2",
   "hvplot==0.8.4",
   "diskcache",
   "optuna",
   "xarray",
+  "plotly",
   "sortedcontainers",
   "pandas==2.0.1",
   "strenum",
   "seaborn==0.12.2",
   "scikit-learn",
   "str2bool"
 ]
```

### Comparing `holobench-0.0.0/setup.py` & `holobench-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/plots/test_catplot.py` & `holobench-0.0.1/test/plots/test_catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/plots/test_plots_common.py` & `holobench-0.0.1/test/plots/test_plots_common.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/plots/test_tables.py` & `holobench-0.0.1/test/plots/test_tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_bench_examples.py` & `holobench-0.0.1/test/test_bench_examples.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_bencher.py` & `holobench-0.0.1/test/test_bencher.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_combinations.py` & `holobench-0.0.1/test/test_combinations.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_plot_collection.py` & `holobench-0.0.1/test/test_plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_plot_filter.py` & `holobench-0.0.1/test/test_plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_plot_library.py` & `holobench-0.0.1/test/test_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_sample_cache.py` & `holobench-0.0.1/test/test_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_sweep_vars.py` & `holobench-0.0.1/test/test_sweep_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_utils.py` & `holobench-0.0.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/test/test_vars.py` & `holobench-0.0.1/test/test_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.0/PKG-INFO` & `holobench-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: holoviews[reccomended]==1.16.2
 Requires-Dist: hvplot==0.8.4
 Requires-Dist: diskcache
 Requires-Dist: optuna
 Requires-Dist: xarray
+Requires-Dist: plotly
 Requires-Dist: sortedcontainers
 Requires-Dist: pandas==2.0.1
 Requires-Dist: strenum
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: scikit-learn
 Requires-Dist: str2bool
 Requires-Dist: black==23.3.0 ; extra == "test"
```

