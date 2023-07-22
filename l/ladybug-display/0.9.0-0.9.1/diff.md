# Comparing `tmp/ladybug-display-0.9.0.tar.gz` & `tmp/ladybug-display-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-display-0.9.0.tar", last modified: Tue Jan 10 01:12:30 2023, max compression
+gzip compressed data, was "dist/ladybug-display-0.9.1.tar", last modified: Mon May 15 19:29:19 2023, max compression
```

## Comparing `ladybug-display-0.9.0.tar` & `ladybug-display-0.9.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/_extend_ladybug.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/altnumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/dictutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/extension/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/hourlyplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/monthlychart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/psychchart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/raddome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/radrose.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/skydome.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/sunpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/windprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/extension/windrose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry2d/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/cone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/polyface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/geometry3d/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    64826 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/ladybug_display/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/ladybug_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 01:12:30.000000 ladybug-display-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/arc2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/arc3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/cone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/cylinder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/face3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/line2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/line3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/mesh2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/mesh3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/plane_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/point2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/point3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyface3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polygon2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyline2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/polyline3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/ray2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/ray3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/sphere_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/vector2d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/vector3d_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-01-10 01:11:25.000000 ladybug-display-0.9.0/tests/visualization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/_extend_ladybug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/altnumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/dictutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/hourlyplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/monthlychart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/psychchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/raddome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/radrose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/skydome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/sunpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/windprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/extension/windrose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry2d/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/polyface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/geometry3d/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64843 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/ladybug_display/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/ladybug_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:29:19.000000 ladybug-display-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/arc2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/arc3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/cone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/cylinder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/face3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/line2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/line3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/mesh2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/mesh3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/plane_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/point2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/point3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/polyface3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/polygon2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/polyline2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/polyline3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/ray2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/ray3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/sphere_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/vector2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/vector3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-15 19:28:20.000000 ladybug-display-0.9.1/tests/visualization_test.py
```

### Comparing `ladybug-display-0.9.0/.github/workflows/ci.yaml` & `ladybug-display-0.9.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/LICENSE` & `ladybug-display-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/PKG-INFO` & `ladybug-display-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ladybug-display
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library that assigns basic display attributes to ladybug-geometry objects (color, line weight, line type, etc).
 Home-page: https://github.com/ladybug-tools/ladybug-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -60,9 +59,7 @@
 ```
 
 4. Generate Documentation:
 ```console
 sphinx-apidoc -f -e -d 4 -o ./docs ./ladybug_display
 sphinx-build -b html ./docs ./docs/_build/docs
 ```
-
-
```

### Comparing `ladybug-display-0.9.0/README.md` & `ladybug-display-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/dev-requirements.txt` & `ladybug-display-0.9.1/dev-requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 coverage==5.5
 coveralls==1.7.0;python_version<'3.0'
 coveralls==2.2.0;python_version>='3.6'
 pytest==4.6.9;python_version<'3.0'
 pytest==6.2.4;python_version>='3.6'
 pytest-cov==2.12.0
 Sphinx==1.8.5;python_version<'3.0'
-Sphinx==3.3.1;python_version>='3.6'
+Sphinx==5.3.0;python_version>='3.6'
 docutils==0.17;python_version>='3.6'
-sphinx-bootstrap-theme==0.7.1
+sphinx-bootstrap-theme==0.8.1
 sphinxcontrib-fulltoc==1.2.0
 sphinxcontrib-websupport==1.1.2;python_version<'3.0'
 sphinxcontrib-websupport==1.2.4;python_version>='3.6'
-sphinx-click==2.7.1
+sphinx-click==4.4.0
 twine==1.13.0;python_version<'3.0'
 twine==3.4.1;python_version>='3.6'
-wheel==0.36.2
+wheel==0.38.1
 setuptools==44.1.0;python_version<'3.0'
-setuptools==57.0.0;python_version>='3.6'
+setuptools==65.5.1;python_version>='3.6'
 importlib-metadata==2.0.0;python_version<'3.0'
-importlib-metadata==4.3.1;python_version>='3.6'
+importlib-metadata==4.8.0;python_version>='3.6'
 jinja2==3.0.3;python_version>='3.6'
 markupsafe==2.0.1;python_version>='3.6'
```

### Comparing `ladybug-display-0.9.0/docs/_templates/layout.html` & `ladybug-display-0.9.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/docs/conf.py` & `ladybug-display-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/_base.py` & `ladybug-display-0.9.1/ladybug_display/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/_extend_ladybug.py` & `ladybug-display-0.9.1/ladybug_display/_extend_ladybug.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/altnumber.py` & `ladybug-display-0.9.1/ladybug_display/altnumber.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/dictutil.py` & `ladybug-display-0.9.1/ladybug_display/dictutil.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/compass.py` & `ladybug-display-0.9.1/ladybug_display/extension/compass.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/hourlyplot.py` & `ladybug-display-0.9.1/ladybug_display/extension/hourlyplot.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/monthlychart.py` & `ladybug-display-0.9.1/ladybug_display/extension/monthlychart.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/psychchart.py` & `ladybug-display-0.9.1/ladybug_display/extension/psychchart.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/raddome.py` & `ladybug-display-0.9.1/ladybug_display/extension/raddome.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/radrose.py` & `ladybug-display-0.9.1/ladybug_display/extension/radrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/skydome.py` & `ladybug-display-0.9.1/ladybug_display/extension/skydome.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/sunpath.py` & `ladybug-display-0.9.1/ladybug_display/extension/sunpath.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/windprofile.py` & `ladybug-display-0.9.1/ladybug_display/extension/windprofile.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/extension/windrose.py` & `ladybug-display-0.9.1/ladybug_display/extension/windrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/_base.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/arc.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/arc.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/line.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/line.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/mesh.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/mesh.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/point.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/point.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/polygon.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/polygon.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/polyline.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/polyline.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/ray.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/ray.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry2d/vector.py` & `ladybug-display-0.9.1/ladybug_display/geometry2d/vector.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/__init__.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/_base.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/_base.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/arc.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/arc.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/cone.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/cone.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/cylinder.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/cylinder.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/face.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/face.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/line.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/line.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/mesh.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/mesh.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/plane.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/plane.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/point.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/point.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/polyface.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/polyface.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/polyline.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/polyline.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/ray.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/ray.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/sphere.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/sphere.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/text.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/text.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/geometry3d/vector.py` & `ladybug-display-0.9.1/ladybug_display/geometry3d/vector.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/typing.py` & `ladybug-display-0.9.1/ladybug_display/typing.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/ladybug_display/visualization.py` & `ladybug-display-0.9.1/ladybug_display/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,16 @@
     def active_data(self):
         """Get or set an integer for the index of data set that is actively displaying.
         """
         return self._active_data
 
     @active_data.setter
     def active_data(self, value):
-        self._active_data = int_in_range(value, 0, len(self._data_sets), 'active_data')
+        self._active_data = int_in_range(
+            value, 0, len(self._data_sets) - 1, 'active_data')
 
     @property
     def display_mode(self):
         """Get or set text to indicate the display mode."""
         return self._display_mode
 
     @display_mode.setter
```

### Comparing `ladybug-display-0.9.0/ladybug_display.egg-info/PKG-INFO` & `ladybug-display-0.9.1/ladybug_display.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ladybug-display
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library that assigns basic display attributes to ladybug-geometry objects (color, line weight, line type, etc).
 Home-page: https://github.com/ladybug-tools/ladybug-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -60,9 +59,7 @@
 ```
 
 4. Generate Documentation:
 ```console
 sphinx-apidoc -f -e -d 4 -o ./docs ./ladybug_display
 sphinx-build -b html ./docs ./docs/_build/docs
 ```
-
-
```

### Comparing `ladybug-display-0.9.0/ladybug_display.egg-info/SOURCES.txt` & `ladybug-display-0.9.1/ladybug_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/setup.py` & `ladybug-display-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/arc2d_test.py` & `ladybug-display-0.9.1/tests/arc2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/arc3d_test.py` & `ladybug-display-0.9.1/tests/arc3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/cone_test.py` & `ladybug-display-0.9.1/tests/cone_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/cylinder_test.py` & `ladybug-display-0.9.1/tests/cylinder_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/face3d_test.py` & `ladybug-display-0.9.1/tests/face3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/line2d_test.py` & `ladybug-display-0.9.1/tests/line2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/line3d_test.py` & `ladybug-display-0.9.1/tests/line3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/mesh2d_test.py` & `ladybug-display-0.9.1/tests/mesh2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/mesh3d_test.py` & `ladybug-display-0.9.1/tests/mesh3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/plane_test.py` & `ladybug-display-0.9.1/tests/plane_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/point2d_test.py` & `ladybug-display-0.9.1/tests/point2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/point3d_test.py` & `ladybug-display-0.9.1/tests/point3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/polyface3d_test.py` & `ladybug-display-0.9.1/tests/polyface3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/polygon2d_test.py` & `ladybug-display-0.9.1/tests/polygon2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/polyline2d_test.py` & `ladybug-display-0.9.1/tests/polyline2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/polyline3d_test.py` & `ladybug-display-0.9.1/tests/polyline3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/ray2d_test.py` & `ladybug-display-0.9.1/tests/ray2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/ray3d_test.py` & `ladybug-display-0.9.1/tests/ray3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/sphere_test.py` & `ladybug-display-0.9.1/tests/sphere_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/vector2d_test.py` & `ladybug-display-0.9.1/tests/vector2d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/vector3d_test.py` & `ladybug-display-0.9.1/tests/vector3d_test.py`

 * *Files identical despite different names*

### Comparing `ladybug-display-0.9.0/tests/visualization_test.py` & `ladybug-display-0.9.1/tests/visualization_test.py`

 * *Files identical despite different names*

