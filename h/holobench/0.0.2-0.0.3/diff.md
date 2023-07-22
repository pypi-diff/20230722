# Comparing `tmp/holobench-0.0.2.tar.gz` & `tmp/holobench-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holobench-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "holobench-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `holobench-0.0.2.tar` & `holobench-0.0.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0      346 2023-07-22 11:01:59.628200 holobench-0.0.2/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1395 2023-07-22 11:01:59.628200 holobench-0.0.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.2/.gitignore
--rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.2/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.2/.pylintrc
--rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      713 2023-07-22 09:13:13.899071 holobench-0.0.2/.vscode/tasks.json
--rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.2/LICENSE
--rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.2/README.md
--rw-r--r--   0        0        0      789 2023-07-22 11:22:18.553301 holobench-0.0.2/bencher/__init__.py
--rw-r--r--   0        0        0    25862 2023-07-22 09:13:13.899071 holobench-0.0.2/bencher/bench_cfg.py
--rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.2/bencher/bench_plot_server.py
--rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.2/bencher/bench_vars.py
--rw-r--r--   0        0        0    27767 2023-07-22 09:34:45.468154 holobench-0.0.2/bencher/bencher.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.2/bencher/example/__init__.py
--rw-r--r--   0        0        0     4168 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/benchmark_data.py
--rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_categorical.py
--rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_custom_sweep.py
--rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_float2D_scatter.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_float3D.py
--rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_float3D_cone.py
--rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_float_cat.py
--rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_floats.py
--rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_floats2D.py
--rw-r--r--   0        0        0     4101 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/example/example_holosweep.py
--rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/example/example_hvplot_explorer.py
--rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/example/example_interactive.py
--rw-r--r--   0        0        0     2415 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_kwargs.py
--rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_pareto.py
--rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_persistent.py
--rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.2/bencher/example/example_plot_library.py
--rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_sample_cache.py
--rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_sample_cache_context.py
--rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_simple.py
--rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/example/example_simple_bool.py
--rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_simple_cat.py
--rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_simple_float.py
--rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.2/bencher/example/example_template.py
--rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_time_event.py
--rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.2/bencher/example/example_vector.py
--rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/example/example_workflow.py
--rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/example/hv_bool_bug.py
--rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/optuna_conversions.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/__init__.py
--rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.2/bencher/plotting/plot_collection.py
--rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/plot_filter.py
--rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plot_library.py
--rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plot_types.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/plots/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/plots/catplot.py
--rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.2/bencher/plotting/plots/heatmap.py
--rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plots/hv_interactive.py
--rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plots/lineplot.py
--rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.2/bencher/plotting/plots/plot_base.py
--rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/plots/scatterplot.py
--rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plots/surface.py
--rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/plotting/plots/tables.py
--rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting/plots/volume.py
--rw-r--r--   0        0        0    10787 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plotting_functions.py
--rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.2/bencher/plt_cfg.py
--rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.2/bencher/utils.py
--rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.2/dependencies.yaml
--rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.2/package.xml
--rw-r--r--   0        0        0     1527 2023-07-22 11:24:05.129873 holobench-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.2/resource/bencher
--rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.2/setup.cfg
--rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.2/setup.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.2/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.2/test/plots/__init__.py
--rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.2/test/plots/test_catplot.py
--rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.2/test/plots/test_plots_common.py
--rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.2/test/plots/test_tables.py
--rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.2/test/test_bench_examples.py
--rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_bencher.py
--rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_combinations.py
--rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_plot_collection.py
--rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_plot_filter.py
--rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_plot_library.py
--rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_sample_cache.py
--rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_sweep_vars.py
--rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_utils.py
--rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.2/test/test_vars.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 holobench-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-07-22 13:16:20.755958 holobench-0.0.3/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1394 2023-07-22 12:02:54.862576 holobench-0.0.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2023-07-16 12:36:45.474978 holobench-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1264 2023-07-16 12:36:45.474978 holobench-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3208 2023-07-20 18:29:05.424632 holobench-0.0.3/.gitignore
+-rw-r--r--   0        0        0      381 2023-07-16 12:36:45.474978 holobench-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      209 2023-07-16 12:36:45.474978 holobench-0.0.3/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      379 2023-07-16 12:36:45.474978 holobench-0.0.3/.pylintrc
+-rw-r--r--   0        0        0      187 2023-07-16 12:36:45.474978 holobench-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      885 2023-07-22 13:25:18.062797 holobench-0.0.3/.vscode/tasks.json
+-rw-r--r--   0        0        0     1065 2023-07-16 12:36:45.474978 holobench-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2720 2023-07-16 12:36:45.474978 holobench-0.0.3/README.md
+-rw-r--r--   0        0        0      789 2023-07-22 12:02:54.862576 holobench-0.0.3/bencher/__init__.py
+-rw-r--r--   0        0        0    25862 2023-07-22 09:13:13.899071 holobench-0.0.3/bencher/bench_cfg.py
+-rw-r--r--   0        0        0     3858 2023-07-16 12:36:45.474978 holobench-0.0.3/bencher/bench_plot_server.py
+-rw-r--r--   0        0        0    24828 2023-07-22 09:13:13.899071 holobench-0.0.3/bencher/bench_vars.py
+-rw-r--r--   0        0        0    27651 2023-07-22 13:21:30.469629 holobench-0.0.3/bencher/bencher.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.474978 holobench-0.0.3/bencher/example/__init__.py
+-rw-r--r--   0        0        0     4187 2023-07-22 13:22:35.729968 holobench-0.0.3/bencher/example/benchmark_data.py
+-rw-r--r--   0        0        0     3745 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_categorical.py
+-rw-r--r--   0        0        0     1901 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_custom_sweep.py
+-rw-r--r--   0        0        0     3197 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_float2D_scatter.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_float3D.py
+-rw-r--r--   0        0        0     2817 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_float3D_cone.py
+-rw-r--r--   0        0        0     3562 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_float_cat.py
+-rw-r--r--   0        0        0     4348 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_floats.py
+-rw-r--r--   0        0        0     4018 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_floats2D.py
+-rw-r--r--   0        0        0     4101 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/example/example_holosweep.py
+-rw-r--r--   0        0        0     1805 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/example/example_hvplot_explorer.py
+-rw-r--r--   0        0        0     2619 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/example/example_interactive.py
+-rw-r--r--   0        0        0     2416 2023-07-22 12:02:54.862576 holobench-0.0.3/bencher/example/example_kwargs.py
+-rw-r--r--   0        0        0     2431 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_pareto.py
+-rw-r--r--   0        0        0     3438 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_persistent.py
+-rw-r--r--   0        0        0     2540 2023-07-20 18:29:05.428632 holobench-0.0.3/bencher/example/example_plot_library.py
+-rw-r--r--   0        0        0     4027 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_sample_cache.py
+-rw-r--r--   0        0        0     3716 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_sample_cache_context.py
+-rw-r--r--   0        0        0    11711 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_simple.py
+-rw-r--r--   0        0        0     1525 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/example/example_simple_bool.py
+-rw-r--r--   0        0        0     1473 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_simple_cat.py
+-rw-r--r--   0        0        0     1393 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_simple_float.py
+-rw-r--r--   0        0        0     1172 2023-07-20 18:29:05.428632 holobench-0.0.3/bencher/example/example_template.py
+-rw-r--r--   0        0        0     1951 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_time_event.py
+-rw-r--r--   0        0        0     2990 2023-07-20 19:07:32.744938 holobench-0.0.3/bencher/example/example_vector.py
+-rw-r--r--   0        0        0     6718 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/example/example_workflow.py
+-rw-r--r--   0        0        0     2261 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/example/hv_bool_bug.py
+-rw-r--r--   0        0        0    10946 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/optuna_conversions.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/__init__.py
+-rw-r--r--   0        0        0     5436 2023-07-20 18:29:05.428632 holobench-0.0.3/bencher/plotting/plot_collection.py
+-rw-r--r--   0        0        0     4705 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/plot_filter.py
+-rw-r--r--   0        0        0     3579 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plot_library.py
+-rw-r--r--   0        0        0     1197 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plot_types.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/plots/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/plots/catplot.py
+-rw-r--r--   0        0        0     3754 2023-07-20 18:29:05.428632 holobench-0.0.3/bencher/plotting/plots/heatmap.py
+-rw-r--r--   0        0        0     3821 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plots/hv_interactive.py
+-rw-r--r--   0        0        0     6359 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plots/lineplot.py
+-rw-r--r--   0        0        0      618 2023-07-20 18:29:05.432632 holobench-0.0.3/bencher/plotting/plots/plot_base.py
+-rw-r--r--   0        0        0     1616 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/plots/scatterplot.py
+-rw-r--r--   0        0        0     3830 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plots/surface.py
+-rw-r--r--   0        0        0     1194 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/plotting/plots/tables.py
+-rw-r--r--   0        0        0     5971 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting/plots/volume.py
+-rw-r--r--   0        0        0    10787 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plotting_functions.py
+-rw-r--r--   0        0        0    14109 2023-07-22 09:13:13.903071 holobench-0.0.3/bencher/plt_cfg.py
+-rw-r--r--   0        0        0     2339 2023-07-16 12:36:45.478978 holobench-0.0.3/bencher/utils.py
+-rw-r--r--   0        0        0      423 2023-07-16 12:36:45.478978 holobench-0.0.3/dependencies.yaml
+-rw-r--r--   0        0        0     1045 2023-07-16 12:36:45.478978 holobench-0.0.3/package.xml
+-rw-r--r--   0        0        0     1548 2023-07-22 13:18:43.192741 holobench-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-07-20 18:29:05.432632 holobench-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.3/resource/bencher
+-rw-r--r--   0        0        0       83 2023-07-16 12:36:45.478978 holobench-0.0.3/setup.cfg
+-rw-r--r--   0        0        0      628 2023-07-16 12:36:45.478978 holobench-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:36:45.478978 holobench-0.0.3/test/plots/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-16 12:36:45.478978 holobench-0.0.3/test/plots/test_catplot.py
+-rw-r--r--   0        0        0     1330 2023-07-16 12:36:45.478978 holobench-0.0.3/test/plots/test_plots_common.py
+-rw-r--r--   0        0        0     1089 2023-07-16 12:36:45.478978 holobench-0.0.3/test/plots/test_tables.py
+-rw-r--r--   0        0        0     3497 2023-07-20 19:19:06.224197 holobench-0.0.3/test/test_bench_examples.py
+-rw-r--r--   0        0        0    16047 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_bencher.py
+-rw-r--r--   0        0        0     6150 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_combinations.py
+-rw-r--r--   0        0        0     3534 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_plot_collection.py
+-rw-r--r--   0        0        0     2772 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_plot_filter.py
+-rw-r--r--   0        0        0     1788 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_plot_library.py
+-rw-r--r--   0        0        0     5671 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_sample_cache.py
+-rw-r--r--   0        0        0     1972 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_sweep_vars.py
+-rw-r--r--   0        0        0     1207 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_utils.py
+-rw-r--r--   0        0        0     2439 2023-07-16 12:36:45.478978 holobench-0.0.3/test/test_vars.py
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 holobench-0.0.3/PKG-INFO
```

### Comparing `holobench-0.0.2/.devcontainer/devcontainer.json` & `holobench-0.0.3/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 	"build": {
 		"dockerfile": "Dockerfile",
 		"context": ".."
 	},
 	"customizations": {
 		"vscode": {
 			"extensions": [
-				"mhutchie.git-graph",
 				"ms-python.python",
+				"ms-python.vscode-pylance",
 				"ms-python.pylint",
 				"njpwerner.autodocstring",
 				"charliermarsh.ruff",
-				"formulahendry.code-runner"
+				"mhutchie.git-graph"
 			]
 		}
 	},
 	// "onCreateCommand": "pre-commit install-hooks"
 }
```

### Comparing `holobench-0.0.2/.github/workflows/ci.yml` & `holobench-0.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/.gitignore` & `holobench-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/.vscode/tasks.json` & `holobench-0.0.3/.vscode/tasks.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'tasks'": "{insert: [(1, OrderedDict([('label', 'flit install'), ('type', 'shell'), ('command', "*

 * *            "'flit install')])), (2, OrderedDict([('label', 'flit publish'), ('type', 'shell'), "*

 * *            "('command', 'flit publish')]))]}"}*

```diff
@@ -2,14 +2,24 @@
     "tasks": [
         {
             "command": "ruff . --fix && black .",
             "label": "autoformat",
             "type": "shell"
         },
         {
+            "command": "flit install",
+            "label": "flit install",
+            "type": "shell"
+        },
+        {
+            "command": "flit publish",
+            "label": "flit publish",
+            "type": "shell"
+        },
+        {
             "command": "mkdir ${workspaceFolder}/.vscode/cfg/;echo ${file} > $_/active_file.cfg; echo Setting the current file: ${file} as the active file.",
             "group": {
                 "isDefault": "True",
                 "kind": "test"
             },
             "label": "sa: Set Active File",
             "problemMatcher": [],
```

### Comparing `holobench-0.0.2/LICENSE` & `holobench-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/README.md` & `holobench-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/__init__.py` & `holobench-0.0.3/bencher/__init__.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/bench_cfg.py` & `holobench-0.0.3/bencher/bench_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/bench_plot_server.py` & `holobench-0.0.3/bencher/bench_plot_server.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/bench_vars.py` & `holobench-0.0.3/bencher/bench_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/bencher.py` & `holobench-0.0.3/bencher/bencher.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,69 +32,69 @@
 
 for handler in logging.root.handlers:
     handler.setFormatter(formatter)
 
 
 def set_xarray_multidim(data_array: xr.DataArray, index_tuple, value: float) -> xr.DataArray:
     """This is terrible, I need to do this in a better way, but [] does not like *args syntax and the () version of the set function doesn't either"""
-    match len(index_tuple):
-        case 1:
-            data_array[index_tuple[0]] = value
-        case 2:
-            data_array[index_tuple[0], index_tuple[1]] = value
-        case 3:
-            data_array[index_tuple[0], index_tuple[1], index_tuple[2]] = value
-        case 4:
-            data_array[index_tuple[0], index_tuple[1], index_tuple[2], index_tuple[3]] = value
-        case 5:
-            data_array[
-                index_tuple[0], index_tuple[1], index_tuple[2], index_tuple[3], index_tuple[4]
-            ] = value
-        case 6:
-            data_array[
-                index_tuple[0],
-                index_tuple[1],
-                index_tuple[2],
-                index_tuple[3],
-                index_tuple[4],
-                index_tuple[5],
-            ] = value
-        case 7:
-            data_array[
-                index_tuple[0],
-                index_tuple[1],
-                index_tuple[2],
-                index_tuple[3],
-                index_tuple[4],
-                index_tuple[5],
-                index_tuple[6],
-            ] = value
-        case 8:
-            data_array[
-                index_tuple[0],
-                index_tuple[1],
-                index_tuple[2],
-                index_tuple[3],
-                index_tuple[4],
-                index_tuple[5],
-                index_tuple[6],
-                index_tuple[7],
-            ] = value
-        case 9:
-            data_array[
-                index_tuple[0],
-                index_tuple[1],
-                index_tuple[2],
-                index_tuple[3],
-                index_tuple[4],
-                index_tuple[5],
-                index_tuple[6],
-                index_tuple[7],
-                index_tuple[8],
-            ] = value
+    tup_len = len(index_tuple)
+    if tup_len == 1:
+        data_array[index_tuple[0]] = value
+    elif tup_len == 2:
+        data_array[index_tuple[0], index_tuple[1]] = value
+    elif tup_len == 3:
+        data_array[index_tuple[0], index_tuple[1], index_tuple[2]] = value
+    elif tup_len == 4:
+        data_array[index_tuple[0], index_tuple[1], index_tuple[2], index_tuple[3]] = value
+    elif tup_len == 5:
+        data_array[
+            index_tuple[0], index_tuple[1], index_tuple[2], index_tuple[3], index_tuple[4]
+        ] = value
+    elif tup_len == 6:
+        data_array[
+            index_tuple[0],
+            index_tuple[1],
+            index_tuple[2],
+            index_tuple[3],
+            index_tuple[4],
+            index_tuple[5],
+        ] = value
+    elif tup_len == 7:
+        data_array[
+            index_tuple[0],
+            index_tuple[1],
+            index_tuple[2],
+            index_tuple[3],
+            index_tuple[4],
+            index_tuple[5],
+            index_tuple[6],
+        ] = value
+    elif tup_len == 8:
+        data_array[
+            index_tuple[0],
+            index_tuple[1],
+            index_tuple[2],
+            index_tuple[3],
+            index_tuple[4],
+            index_tuple[5],
+            index_tuple[6],
+            index_tuple[7],
+        ] = value
+    elif tup_len == 9:
+        data_array[
+            index_tuple[0],
+            index_tuple[1],
+            index_tuple[2],
+            index_tuple[3],
+            index_tuple[4],
+            index_tuple[5],
+            index_tuple[6],
+            index_tuple[7],
+            index_tuple[8],
+        ] = value
     return data_array
 
 
 class Bench(BenchPlotServer):
     def __init__(
         self,
         bench_name: str = None,
```

### Comparing `holobench-0.0.2/bencher/example/benchmark_data.py` & `holobench-0.0.3/bencher/example/benchmark_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,22 +61,20 @@
 
     Returns:
         float: a noisy float value
     """
 
     noise = 0.0
     if config.noisy:
-        match config.noise_distribution:
-            case NoiseDistribution.uniform:
-                noise = random.uniform(0, config.sigma)
-            case NoiseDistribution.gaussian:
-                noise = random.gauss(0, config.sigma)
-            case NoiseDistribution.lognorm:
-                noise = random.lognormvariate(0, config.sigma)
-
+        if config.noise_distribution == NoiseDistribution.uniform:
+            noise = random.uniform(0, config.sigma)
+        elif config.noise_distribution == NoiseDistribution.gaussian:
+            noise = random.gauss(0, config.sigma)
+        elif config.noise_distribution == NoiseDistribution.lognorm:
+            noise = random.lognormvariate(0, config.sigma)
     return noise
 
 
 class ExampleBenchCfgIn(NoiseCfg):
     """A class for representing a set of configuration options for the example worker. This class inherits from NoiseCfg so it also stores all its values as well."""
 
     theta = FloatSweep(default=0, bounds=[0, math.pi], doc="Input angle", units="rad", samples=30)
```

### Comparing `holobench-0.0.2/bencher/example/example_categorical.py` & `holobench-0.0.3/bencher/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_custom_sweep.py` & `holobench-0.0.3/bencher/example/example_custom_sweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_float2D_scatter.py` & `holobench-0.0.3/bencher/example/example_float2D_scatter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_float3D.py` & `holobench-0.0.3/bencher/example/example_float3D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_float3D_cone.py` & `holobench-0.0.3/bencher/example/example_float3D_cone.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_float_cat.py` & `holobench-0.0.3/bencher/example/example_float_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_floats.py` & `holobench-0.0.3/bencher/example/example_floats.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_floats2D.py` & `holobench-0.0.3/bencher/example/example_floats2D.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_holosweep.py` & `holobench-0.0.3/bencher/example/example_holosweep.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_hvplot_explorer.py` & `holobench-0.0.3/bencher/example/example_hvplot_explorer.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_interactive.py` & `holobench-0.0.3/bencher/example/example_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_kwargs.py` & `holobench-0.0.3/bencher/example/example_kwargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def bench_function(
     theta: float = 0,
     offset: float = 0,
     scale: float = 1.0,
     trig_func: str = "sin",
-    **kwargs  # pylint: disable=unused-argument
+    **kwargs,  # pylint: disable=unused-argument
 ) -> dict:
     """All the other examples use classes and parameters to define the inputs and outputs to the function. However it makes the code less flexible when integrating with other systems, so this example shows a more basic interface that accepts and returns dictionaries.  The classes still need to be defined however because that is how the sweep and plotting settings are calcuated"""
     output = {}
 
     if trig_func == "sin":
         output["voltage"] = offset + math.sin(theta) * scale
     elif trig_func == "cos":
```

### Comparing `holobench-0.0.2/bencher/example/example_pareto.py` & `holobench-0.0.3/bencher/example/example_pareto.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_persistent.py` & `holobench-0.0.3/bencher/example/example_persistent.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_plot_library.py` & `holobench-0.0.3/bencher/example/example_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_sample_cache.py` & `holobench-0.0.3/bencher/example/example_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_sample_cache_context.py` & `holobench-0.0.3/bencher/example/example_sample_cache_context.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_simple.py` & `holobench-0.0.3/bencher/example/example_simple.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_simple_bool.py` & `holobench-0.0.3/bencher/example/example_simple_bool.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_simple_cat.py` & `holobench-0.0.3/bencher/example/example_simple_cat.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_simple_float.py` & `holobench-0.0.3/bencher/example/example_simple_float.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_template.py` & `holobench-0.0.3/bencher/example/example_template.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_time_event.py` & `holobench-0.0.3/bencher/example/example_time_event.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_vector.py` & `holobench-0.0.3/bencher/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/example_workflow.py` & `holobench-0.0.3/bencher/example/example_workflow.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/example/hv_bool_bug.py` & `holobench-0.0.3/bencher/example/hv_bool_bug.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/optuna_conversions.py` & `holobench-0.0.3/bencher/optuna_conversions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plot_collection.py` & `holobench-0.0.3/bencher/plotting/plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plot_filter.py` & `holobench-0.0.3/bencher/plotting/plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plot_library.py` & `holobench-0.0.3/bencher/plotting/plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plot_types.py` & `holobench-0.0.3/bencher/plotting/plot_types.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/catplot.py` & `holobench-0.0.3/bencher/plotting/plots/catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/heatmap.py` & `holobench-0.0.3/bencher/plotting/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/hv_interactive.py` & `holobench-0.0.3/bencher/plotting/plots/hv_interactive.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/lineplot.py` & `holobench-0.0.3/bencher/plotting/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/plot_base.py` & `holobench-0.0.3/bencher/plotting/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/scatterplot.py` & `holobench-0.0.3/bencher/plotting/plots/scatterplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/surface.py` & `holobench-0.0.3/bencher/plotting/plots/surface.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/tables.py` & `holobench-0.0.3/bencher/plotting/plots/tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting/plots/volume.py` & `holobench-0.0.3/bencher/plotting/plots/volume.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plotting_functions.py` & `holobench-0.0.3/bencher/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/plt_cfg.py` & `holobench-0.0.3/bencher/plt_cfg.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/bencher/utils.py` & `holobench-0.0.3/bencher/utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/package.xml` & `holobench-0.0.3/package.xml`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/pyproject.toml` & `holobench-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name =  "holobench"
+version = "0.0.3"
+
 authors = [
     {name = "Austin Gregg-Smith", email = "blooop@gmail.com"},
 ]
 description = "A package for benchmarking the performance of arbitrary functions"
 readme = "README.md"
 
-requires-python = ">=3.10"
-version = "0.0.2"
+requires-python = ">=3.8"
 
 dependencies = [
   "holoviews[reccomended]==1.16.2",
   "hvplot==0.8.4",
   "diskcache",
   "optuna",
   "xarray",
@@ -30,15 +31,16 @@
     "check-manifest==0.49",
     "pre-commit==2.21.0",
     "pylint==2.17.4",
     "pytest-cov==4.1.0",
     "pytest-mock<3.10.2",
     "pytest-runner",
     "pytest==7.4.0",
-    "hypothesis==6.82.0"
+    "hypothesis==6.82.0",
+    "ruff==0.0.280"
 ]
 
 [project.urls]
 Source = "https://github.com/blooop/bencher"
 Home = "https://github.com/blooop/bencher"
```

### Comparing `holobench-0.0.2/setup.py` & `holobench-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/plots/test_catplot.py` & `holobench-0.0.3/test/plots/test_catplot.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/plots/test_plots_common.py` & `holobench-0.0.3/test/plots/test_plots_common.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/plots/test_tables.py` & `holobench-0.0.3/test/plots/test_tables.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_bench_examples.py` & `holobench-0.0.3/test/test_bench_examples.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_bencher.py` & `holobench-0.0.3/test/test_bencher.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_combinations.py` & `holobench-0.0.3/test/test_combinations.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_plot_collection.py` & `holobench-0.0.3/test/test_plot_collection.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_plot_filter.py` & `holobench-0.0.3/test/test_plot_filter.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_plot_library.py` & `holobench-0.0.3/test/test_plot_library.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_sample_cache.py` & `holobench-0.0.3/test/test_sample_cache.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_sweep_vars.py` & `holobench-0.0.3/test/test_sweep_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_utils.py` & `holobench-0.0.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/test/test_vars.py` & `holobench-0.0.3/test/test_vars.py`

 * *Files identical despite different names*

### Comparing `holobench-0.0.2/PKG-INFO` & `holobench-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: holobench
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for benchmarking the performance of arbitrary functions
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: holoviews[reccomended]==1.16.2
 Requires-Dist: hvplot==0.8.4
 Requires-Dist: diskcache
 Requires-Dist: optuna
 Requires-Dist: xarray
 Requires-Dist: plotly
@@ -22,14 +22,15 @@
 Requires-Dist: pre-commit==2.21.0 ; extra == "test"
 Requires-Dist: pylint==2.17.4 ; extra == "test"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "test"
 Requires-Dist: pytest-mock<3.10.2 ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
 Requires-Dist: pytest==7.4.0 ; extra == "test"
 Requires-Dist: hypothesis==6.82.0 ; extra == "test"
+Requires-Dist: ruff==0.0.280 ; extra == "test"
 Project-URL: Home, https://github.com/blooop/bencher
 Project-URL: Source, https://github.com/blooop/bencher
 Provides-Extra: test
 
 # Bencher
 
 ## Continuous Integration Status
```

