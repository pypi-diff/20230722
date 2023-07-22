# Comparing `tmp/openslide-python-1.2.0.tar.gz` & `tmp/openslide-python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openslide-python-1.2.0.tar", last modified: Sat Jun 18 02:30:17 2022, max compression
+gzip compressed data, was "openslide-python-1.3.0.tar", last modified: Sat Jul 22 06:33:12 2023, max compression
```

## Comparing `openslide-python-1.2.0.tar` & `openslide-python-1.3.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.530655 openslide-python-1.2.0/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3340 2022-06-18 02:22:54.000000 openslide-python-1.2.0/CHANGELOG.md
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      536 2018-05-05 17:20:40.000000 openslide-python-1.2.0/LICENSE.txt
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      150 2022-06-17 04:52:35.000000 openslide-python-1.2.0/MANIFEST.in
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3501 2022-06-18 02:30:17.529655 openslide-python-1.2.0/PKG-INFO
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2265 2022-06-17 04:52:35.000000 openslide-python-1.2.0/README.md
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.513655 openslide-python-1.2.0/doc/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     8492 2022-06-17 04:43:15.000000 openslide-python-1.2.0/doc/conf.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    14405 2022-06-17 04:43:15.000000 openslide-python-1.2.0/doc/index.rst
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2724 2022-06-17 04:43:15.000000 openslide-python-1.2.0/doc/jekyll_fix.py
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.510655 openslide-python-1.2.0/examples/
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.515655 openslide-python-1.2.0/examples/deepzoom/
--rwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)     8416 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/deepzoom_multiserver.py
--rwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)     6679 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/deepzoom_server.py
--rwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)    11826 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/deepzoom_tile.py
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.517655 openslide-python-1.2.0/examples/deepzoom/static/
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.526655 openslide-python-1.2.0/examples/deepzoom/static/images/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1085 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2184 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2225 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1309 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1062 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/home_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2091 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/home_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2138 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/home_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1258 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/home_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1918 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/next_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2358 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/next_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2411 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/next_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2027 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/next_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1933 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/previous_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2361 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/previous_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2413 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/previous_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2029 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/previous_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1731 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2094 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2036 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1779 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1800 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2158 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2039 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1812 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1060 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2116 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2159 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1262 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      977 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_grouphover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1926 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_hover.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1997 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_pressed.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1153 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_rest.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)   235341 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/jquery.js
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    23862 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/openseadragon-scalebar.js
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)   906910 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/static/openseadragon.js
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.527655 openslide-python-1.2.0/examples/deepzoom/templates/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      753 2014-02-15 06:43:28.000000 openslide-python-1.2.0/examples/deepzoom/templates/files.html
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1458 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/templates/slide-fullpage.html
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     4038 2022-06-17 04:43:15.000000 openslide-python-1.2.0/examples/deepzoom/templates/slide-multipane.html
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    26530 2012-06-09 02:07:17.000000 openslide-python-1.2.0/lgpl-2.1.txt
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.527655 openslide-python-1.2.0/openslide/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    14862 2022-06-17 04:43:15.000000 openslide-python-1.2.0/openslide/__init__.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3243 2022-06-17 04:43:15.000000 openslide-python-1.2.0/openslide/_convert.c
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      961 2022-06-18 02:22:54.000000 openslide-python-1.2.0/openslide/_version.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    10027 2022-06-17 04:43:15.000000 openslide-python-1.2.0/openslide/deepzoom.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)    10852 2022-06-17 04:43:15.000000 openslide-python-1.2.0/openslide/lowlevel.py
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.528655 openslide-python-1.2.0/openslide_python.egg-info/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3501 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/PKG-INFO
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2690 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/SOURCES.txt
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)        1 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/dependency_links.txt
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)        7 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/requires.txt
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)       10 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/top_level.txt
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)        1 2022-06-18 02:30:17.000000 openslide-python-1.2.0/openslide_python.egg-info/zip-safe
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)       38 2022-06-18 02:30:17.530655 openslide-python-1.2.0/setup.cfg
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1859 2022-06-17 04:43:15.000000 openslide-python-1.2.0/setup.py
-drwxrwxr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2022-06-18 02:30:17.529655 openslide-python-1.2.0/tests/
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2056 2022-06-17 04:43:15.000000 openslide-python-1.2.0/tests/__init__.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      204 2018-04-09 06:21:42.000000 openslide-python-1.2.0/tests/boxes.png
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3580 2018-04-09 06:21:42.000000 openslide-python-1.2.0/tests/boxes.tiff
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2651 2018-04-09 06:21:42.000000 openslide-python-1.2.0/tests/small.svs
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1171 2022-06-17 04:43:15.000000 openslide-python-1.2.0/tests/test_base.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     3285 2022-06-17 04:43:15.000000 openslide-python-1.2.0/tests/test_deepzoom.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     4134 2022-06-17 04:43:15.000000 openslide-python-1.2.0/tests/test_imageslide.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     7874 2022-06-17 04:43:15.000000 openslide-python-1.2.0/tests/test_openslide.py
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     1020 2018-04-09 06:21:42.000000 openslide-python-1.2.0/tests/unopenable.tiff
--rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)     2651 2018-04-09 06:21:42.000000 openslide-python-1.2.0/tests/unreadable.svs
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.970921 openslide-python-1.3.0/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     4017 2023-07-22 06:20:34.000000 openslide-python-1.3.0/CHANGELOG.md
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    26530 2023-07-18 18:01:43.000000 openslide-python-1.3.0/COPYING.LESSER
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      161 2023-07-22 05:15:40.000000 openslide-python-1.3.0/MANIFEST.in
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     3789 2023-07-22 06:33:12.970921 openslide-python-1.3.0/PKG-INFO
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2569 2023-07-22 05:22:33.000000 openslide-python-1.3.0/README.md
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.963921 openslide-python-1.3.0/doc/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     8492 2023-07-22 05:15:40.000000 openslide-python-1.3.0/doc/conf.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    16673 2023-07-22 06:20:34.000000 openslide-python-1.3.0/doc/index.rst
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     3111 2023-07-18 17:59:07.000000 openslide-python-1.3.0/doc/jekyll_fix.py
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.962921 openslide-python-1.3.0/examples/
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.964921 openslide-python-1.3.0/examples/deepzoom/
+-rwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)    11853 2023-07-22 05:15:40.000000 openslide-python-1.3.0/examples/deepzoom/deepzoom_multiserver.py
+-rwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)     9915 2023-07-22 05:15:40.000000 openslide-python-1.3.0/examples/deepzoom/deepzoom_server.py
+-rwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)    14912 2023-07-22 05:15:40.000000 openslide-python-1.3.0/examples/deepzoom/deepzoom_tile.py
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.964921 openslide-python-1.3.0/examples/deepzoom/static/
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.967921 openslide-python-1.3.0/examples/deepzoom/static/images/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1085 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2184 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2225 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1309 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1062 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/home_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2091 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/home_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2138 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/home_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1258 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/home_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1918 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/next_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2358 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/next_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2411 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/next_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2027 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/next_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1933 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/previous_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2361 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/previous_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2413 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/previous_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2029 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/previous_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1731 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2094 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2036 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1779 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1800 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2158 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2039 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1812 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1060 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2116 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2159 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1262 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      977 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_grouphover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1926 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_hover.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1997 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_pressed.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1153 2023-05-25 20:54:36.000000 openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_rest.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)   231697 2023-07-18 18:01:43.000000 openslide-python-1.3.0/examples/deepzoom/static/jquery.js
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    23862 2022-08-08 06:37:49.000000 openslide-python-1.3.0/examples/deepzoom/static/openseadragon-scalebar.js
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)   963905 2023-07-22 05:15:40.000000 openslide-python-1.3.0/examples/deepzoom/static/openseadragon.js
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.968921 openslide-python-1.3.0/examples/deepzoom/templates/
+-rw-rw-r--   0 bgilbert  (1000) bgilbert  (1000)      753 2014-02-15 06:43:28.000000 openslide-python-1.3.0/examples/deepzoom/templates/files.html
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1458 2022-08-08 06:37:49.000000 openslide-python-1.3.0/examples/deepzoom/templates/slide-fullpage.html
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     4038 2022-08-08 06:37:49.000000 openslide-python-1.3.0/examples/deepzoom/templates/slide-multipane.html
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.968921 openslide-python-1.3.0/openslide/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    16199 2023-07-22 05:15:40.000000 openslide-python-1.3.0/openslide/__init__.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     3243 2022-08-08 06:37:49.000000 openslide-python-1.3.0/openslide/_convert.c
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      961 2023-07-22 06:20:34.000000 openslide-python-1.3.0/openslide/_version.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    10186 2023-07-22 05:15:40.000000 openslide-python-1.3.0/openslide/deepzoom.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)    12830 2023-07-22 05:15:40.000000 openslide-python-1.3.0/openslide/lowlevel.py
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.969921 openslide-python-1.3.0/openslide_python.egg-info/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     3789 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/PKG-INFO
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2820 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/SOURCES.txt
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)        1 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/dependency_links.txt
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)        7 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/requires.txt
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)       10 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/top_level.txt
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)        1 2023-07-22 06:33:12.000000 openslide-python-1.3.0/openslide_python.egg-info/zip-safe
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      230 2023-07-18 18:01:43.000000 openslide-python-1.3.0/pytest.ini
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)       38 2023-07-22 06:33:12.970921 openslide-python-1.3.0/setup.cfg
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1860 2023-07-20 04:46:52.000000 openslide-python-1.3.0/setup.py
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.969921 openslide-python-1.3.0/tests/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1359 2023-07-20 04:46:52.000000 openslide-python-1.3.0/tests/common.py
+drwxr-xr-x   0 bgilbert  (1000) bgilbert  (1000)        0 2023-07-22 06:33:12.970921 openslide-python-1.3.0/tests/fixtures/
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      204 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/fixtures/boxes-no-icc.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)      589 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/fixtures/boxes.png
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     7696 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/fixtures/boxes.tiff
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     5502 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/fixtures/boxes_0.dcm
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     5658 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/fixtures/boxes_1.dcm
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2651 2023-07-18 18:01:43.000000 openslide-python-1.3.0/tests/fixtures/small.svs
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1020 2023-07-18 18:01:43.000000 openslide-python-1.3.0/tests/fixtures/unopenable.tiff
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     2651 2023-07-18 18:01:43.000000 openslide-python-1.3.0/tests/fixtures/unreadable.svs
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     1789 2023-07-18 18:01:43.000000 openslide-python-1.3.0/tests/test_base.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     3558 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/test_deepzoom.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     4972 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/test_imageslide.py
+-rw-r--r--   0 bgilbert  (1000) bgilbert  (1000)     9554 2023-07-22 05:15:40.000000 openslide-python-1.3.0/tests/test_openslide.py
```

### Comparing `openslide-python-1.2.0/CHANGELOG.md` & `openslide-python-1.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Notable Changes in OpenSlide Python
 
+## Version 1.3.0, 2023-07-22
+
+* Support new soname in OpenSlide &ge; 4.0.0
+* Drop support for Python 3.7
+* Expose color management profiles where available
+* Notate available OpenSlide functions in low-level API
+* docs: Update OpenSlide 3.5.0 references to 4.0.0
+* docs: Consolidate license information
+* docs: Drop support for building with Sphinx &lt; 1.6
+* examples: Fix startup failure with Flask &ge; 2.3.0
+* examples: Transform to sRGB (with absolute colorimetric intent) by default
+* examples: Update OpenSeadragon to 4.1.0
+* examples: Correctly import `openslide` on Windows if `OPENSLIDE_PATH` not set
+* tests: Fix `pytest` of installed package from source directory
+
 ## Version 1.2.0, 2022-06-17
 
 * Drop support for Python &lt; 3.7
 * Support cache customization with OpenSlide 3.5.0
 * Improve pixel read performance
 * Clarify exception raised on Windows or macOS when OpenSlide can't be found
 * Raise `OpenSlideVersionError` when an operation requires a newer OpenSlide
```

### Comparing `openslide-python-1.2.0/PKG-INFO` & `openslide-python-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: openslide-python
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python interface to OpenSlide
 Home-page: https://openslide.org/
 Maintainer: OpenSlide project
 Maintainer-email: openslide-users@lists.andrew.cmu.edu
 License: GNU Lesser General Public License, version 2.1
 Keywords: openslide whole-slide image virtual slide library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: COPYING.LESSER
 
 # OpenSlide Python
 
 OpenSlide Python is a Python interface to the OpenSlide library.
 
 [OpenSlide] is a C library that provides a simple interface for reading
 whole-slide images, also known as virtual slides, which are high-resolution
@@ -38,39 +37,41 @@
 libraries, which are designed for images that can be comfortably
 uncompressed into RAM.  Whole-slide images are typically multi-resolution;
 OpenSlide allows reading a small amount of image data at the resolution
 closest to a desired zoom level.
 
 OpenSlide can read virtual slides in several formats:
 
-* [Aperio][]: (`.svs`, `.tif`)
-* [Hamamatsu][]: (`.ndpi`, `.vms`, `.vmu`)
-* [Leica][]: (`.scn`)
-* [MIRAX][]: (`.mrxs`)
-* [Philips][]: (`.tiff`)
-* [Sakura][]: (`.svslide`)
-* [Trestle][]: (`.tif`)
-* [Ventana][]: (`.bif`, `.tif`)
-* [Generic tiled TIFF][]: (`.tif`)
+* [Aperio][] (`.svs`, `.tif`)
+* [DICOM][] (`.dcm`)
+* [Hamamatsu][] (`.ndpi`, `.vms`, `.vmu`)
+* [Leica][] (`.scn`)
+* [MIRAX][] (`.mrxs`)
+* [Philips][] (`.tiff`)
+* [Sakura][] (`.svslide`)
+* [Trestle][] (`.tif`)
+* [Ventana][] (`.bif`, `.tif`)
+* [Generic tiled TIFF][] (`.tif`)
 
 [OpenSlide]: https://openslide.org/
 [Aperio]: https://openslide.org/formats/aperio/
+[DICOM]: https://openslide.org/formats/dicom/
 [Hamamatsu]: https://openslide.org/formats/hamamatsu/
 [Leica]: https://openslide.org/formats/leica/
 [MIRAX]: https://openslide.org/formats/mirax/
 [Philips]: https://openslide.org/formats/philips/
 [Sakura]: https://openslide.org/formats/sakura/
 [Trestle]: https://openslide.org/formats/trestle/
 [Ventana]: https://openslide.org/formats/ventana/
 [Generic tiled TIFF]: https://openslide.org/formats/generic-tiff/
 
 
 ## Requirements
 
-* Python &ge; 3.7
+* Python &ge; 3.8
 * OpenSlide &ge; 3.4.0
 * Pillow
 
 
 ## Installation
 
 OpenSlide Python requires [OpenSlide].  For instructions on installing both
@@ -79,19 +80,22 @@
 
 [installing]: https://openslide.org/api/python/#installing
 
 
 ## More Information
 
 - [API documentation](https://openslide.org/api/python/)
-- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md)
+- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md#notable-changes-in-openslide-python)
 - [Website][OpenSlide]
 - [GitHub](https://github.com/openslide/openslide-python)
-- [Sample data](http://openslide.cs.cmu.edu/download/openslide-testdata/)
+- [Sample data](https://openslide.cs.cmu.edu/download/openslide-testdata/)
 
 
 ## License
 
 OpenSlide Python is released under the terms of the [GNU Lesser General
-Public License, version 2.1](https://raw.github.com/openslide/openslide-python/main/lgpl-2.1.txt).
-
+Public License, version 2.1](https://openslide.org/license/).
 
+OpenSlide Python is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
+License for more details.
```

### Comparing `openslide-python-1.2.0/README.md` & `openslide-python-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -9,39 +9,41 @@
 libraries, which are designed for images that can be comfortably
 uncompressed into RAM.  Whole-slide images are typically multi-resolution;
 OpenSlide allows reading a small amount of image data at the resolution
 closest to a desired zoom level.
 
 OpenSlide can read virtual slides in several formats:
 
-* [Aperio][]: (`.svs`, `.tif`)
-* [Hamamatsu][]: (`.ndpi`, `.vms`, `.vmu`)
-* [Leica][]: (`.scn`)
-* [MIRAX][]: (`.mrxs`)
-* [Philips][]: (`.tiff`)
-* [Sakura][]: (`.svslide`)
-* [Trestle][]: (`.tif`)
-* [Ventana][]: (`.bif`, `.tif`)
-* [Generic tiled TIFF][]: (`.tif`)
+* [Aperio][] (`.svs`, `.tif`)
+* [DICOM][] (`.dcm`)
+* [Hamamatsu][] (`.ndpi`, `.vms`, `.vmu`)
+* [Leica][] (`.scn`)
+* [MIRAX][] (`.mrxs`)
+* [Philips][] (`.tiff`)
+* [Sakura][] (`.svslide`)
+* [Trestle][] (`.tif`)
+* [Ventana][] (`.bif`, `.tif`)
+* [Generic tiled TIFF][] (`.tif`)
 
 [OpenSlide]: https://openslide.org/
 [Aperio]: https://openslide.org/formats/aperio/
+[DICOM]: https://openslide.org/formats/dicom/
 [Hamamatsu]: https://openslide.org/formats/hamamatsu/
 [Leica]: https://openslide.org/formats/leica/
 [MIRAX]: https://openslide.org/formats/mirax/
 [Philips]: https://openslide.org/formats/philips/
 [Sakura]: https://openslide.org/formats/sakura/
 [Trestle]: https://openslide.org/formats/trestle/
 [Ventana]: https://openslide.org/formats/ventana/
 [Generic tiled TIFF]: https://openslide.org/formats/generic-tiff/
 
 
 ## Requirements
 
-* Python &ge; 3.7
+* Python &ge; 3.8
 * OpenSlide &ge; 3.4.0
 * Pillow
 
 
 ## Installation
 
 OpenSlide Python requires [OpenSlide].  For instructions on installing both
@@ -50,17 +52,22 @@
 
 [installing]: https://openslide.org/api/python/#installing
 
 
 ## More Information
 
 - [API documentation](https://openslide.org/api/python/)
-- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md)
+- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md#notable-changes-in-openslide-python)
 - [Website][OpenSlide]
 - [GitHub](https://github.com/openslide/openslide-python)
-- [Sample data](http://openslide.cs.cmu.edu/download/openslide-testdata/)
+- [Sample data](https://openslide.cs.cmu.edu/download/openslide-testdata/)
 
 
 ## License
 
 OpenSlide Python is released under the terms of the [GNU Lesser General
-Public License, version 2.1](https://raw.github.com/openslide/openslide-python/main/lgpl-2.1.txt).
+Public License, version 2.1](https://openslide.org/license/).
+
+OpenSlide Python is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
+License for more details.
```

### Comparing `openslide-python-1.2.0/doc/conf.py` & `openslide-python-1.3.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'OpenSlide Python'
-copyright = '2010-2022 Carnegie Mellon University and others'
+copyright = '2010-2023 Carnegie Mellon University and others'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 import _version  # noqa: E402  module-level-import-not-at-top-of-file
```

### Comparing `openslide-python-1.2.0/doc/index.rst` & `openslide-python-1.3.0/doc/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -12,37 +12,39 @@
 uncompressed into RAM.  Whole-slide images are typically multi-resolution;
 OpenSlide allows reading a small amount of image data at the resolution
 closest to a desired zoom level.
 
 OpenSlide can read virtual slides in several formats:
 
 * Aperio_ (``.svs``, ``.tif``)
+* DICOM_ (``.dcm``)
 * Hamamatsu_ (``.ndpi``, ``.vms``, ``.vmu``)
 * Leica_ (``.scn``)
 * MIRAX_ (``.mrxs``)
 * Philips_ (``.tiff``)
 * Sakura_ (``.svslide``)
 * Trestle_ (``.tif``)
 * Ventana_ (``.bif``, ``.tif``)
 * `Generic tiled TIFF`_ (``.tif``)
 
 OpenSlide Python is released under the terms of the `GNU Lesser General
 Public License, version 2.1`_.
 
 .. _OpenSlide: https://openslide.org/
 .. _Aperio: https://openslide.org/formats/aperio/
+.. _DICOM: https://openslide.org/formats/dicom/
 .. _Hamamatsu: https://openslide.org/formats/hamamatsu/
 .. _Leica: https://openslide.org/formats/leica/
 .. _MIRAX: https://openslide.org/formats/mirax/
 .. _Philips: https://openslide.org/formats/philips/
 .. _Sakura: https://openslide.org/formats/sakura/
 .. _Trestle: https://openslide.org/formats/trestle/
 .. _Ventana: https://openslide.org/formats/ventana/
 .. _`Generic tiled TIFF`: https://openslide.org/formats/generic-tiff/
-.. _`GNU Lesser General Public License, version 2.1`: https://raw.github.com/openslide/openslide-python/main/lgpl-2.1.txt
+.. _`GNU Lesser General Public License, version 2.1`: https://openslide.org/license/
 
 
 Installing
 ==========
 
 OpenSlide Python requires OpenSlide_, which must be installed separately.
 
@@ -59,23 +61,20 @@
 ``with os.add_dll_directory()`` statement::
 
     # The path can also be read from a config file, etc.
     OPENSLIDE_PATH = r'c:\path\to\openslide-win64\bin'
 
     import os
     if hasattr(os, 'add_dll_directory'):
-        # Python >= 3.8 on Windows
+        # Windows
         with os.add_dll_directory(OPENSLIDE_PATH):
             import openslide
     else:
         import openslide
 
-This won't work with Python 3.7 or earlier; you'll need to add the OpenSlide
-``bin`` directory to your ``PATH`` instead.
-
 .. _install: https://openslide.org/download/#distribution-packages
 .. _Anaconda: https://anaconda.org/
 .. _MacPorts: https://www.macports.org/
 .. _pip: https://pip.pypa.io/en/stable/
 .. _source: https://openslide.org/download/#source
 .. _`Windows binaries`: https://openslide.org/download/#windows-binaries
 
@@ -147,14 +146,20 @@
 
       Images, such as label or macro images, which are associated with this
       slide.  This is a :class:`~collections.abc.Mapping` from image
       name to RGBA :class:`Image <PIL.Image.Image>`.
 
       Unlike in the C interface, these images are not premultiplied.
 
+   .. attribute:: color_profile
+
+      The embedded :ref:`color profile <color-management>` for this slide,
+      as a Pillow :class:`~PIL.ImageCms.ImageCmsProfile`, or :obj:`None` if
+      not available.
+
    .. method:: read_region(location, level, size)
 
       Return an RGBA :class:`Image <PIL.Image.Image>` containing the
       contents of the specified region.
 
       Unlike in the C interface, the image data is not premultiplied.
 
@@ -180,34 +185,86 @@
    .. method:: set_cache(cache)
 
       Use the specified :class:`OpenSlideCache` to store recently decoded
       slide tiles.  By default, the :class:`OpenSlide` has a private cache
       with a default size.
 
       :param OpenSlideCache cache: a cache object
-      :raises OpenSlideVersionError: if OpenSlide is older than version 3.5.0
+      :raises OpenSlideVersionError: if OpenSlide is older than version 4.0.0
 
    .. method:: close()
 
       Close the OpenSlide object.
 
 
+.. _color-management:
+
+Color management
+----------------
+
+Every slide region, associated image, thumbnail, and Deep Zoom tile produced
+by OpenSlide Python includes a reference to an ICC color profile whenever a
+profile is available for the underlying pixel data.  Profiles are stored as
+a :class:`bytes` object in
+:attr:`Image.info <PIL.Image.Image.info>`:attr:`['icc_profile']`.  If no
+profile is available, the :attr:`icc_profile` dictionary key is absent.
+
+To include the profile in an image file when saving the image to disk::
+
+    image.save(filename, icc_profile=image.info.get('icc_profile'))
+
+To perform color conversions using the profile, import it into
+:mod:`ImageCms <PIL.ImageCms>`.  For example, to convert an image in-place
+to a synthesized sRGB profile, using absolute colorimetric rendering::
+
+    from io import BytesIO
+    from PIL import ImageCms
+
+    fromProfile = ImageCms.getOpenProfile(BytesIO(image.info['icc_profile']))
+    toProfile = ImageCms.createProfile('sRGB')
+    ImageCms.profileToProfile(
+        image, fromProfile, toProfile,
+        ImageCms.Intent.ABSOLUTE_COLORIMETRIC, 'RGBA', True, 0
+    )
+
+Absolute colorimetric rendering `maximizes the comparability`_ of images
+produced by different scanners.  When converting Deep Zoom tiles, use
+``'RGB'`` instead of ``'RGBA'``.
+
+All pyramid regions in a slide have the same profile, but each associated
+image can have its own profile.  As a convenience, the former is also
+available as :attr:`OpenSlide.color_profile`, already parsed into an
+:class:`~PIL.ImageCms.ImageCmsProfile` object.  You can save processing time
+by building an :class:`~PIL.ImageCms.ImageCmsTransform` for the slide and
+reusing it for multiple slide regions::
+
+    toProfile = ImageCms.createProfile('sRGB')
+    transform = ImageCms.buildTransform(
+        slide.color_profile, toProfile, 'RGBA', 'RGBA',
+        ImageCms.Intent.ABSOLUTE_COLORIMETRIC, 0
+    )
+    # for each region image:
+    ImageCms.applyTransform(image, transform, True)
+
+.. _maximizes the comparability: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4478790/
+
+
 Caching
 -------
 
 .. class:: OpenSlideCache(capacity)
 
    An in-memory tile cache.
 
    Tile caches can be attached to one or more :class:`OpenSlide` objects
    with :meth:`OpenSlide.set_cache` to cache recently-decoded tiles.  By
    default, each :class:`OpenSlide` has its own cache with a default size.
 
    :param int capacity: the cache capacity in bytes
-   :raises OpenSlideVersionError: if OpenSlide is older than version 3.5.0
+   :raises OpenSlideVersionError: if OpenSlide is older than version 4.0.0
 
 
 .. _standard-properties:
 
 Standard properties
 -------------------
 
@@ -285,16 +342,18 @@
 
 .. exception:: OpenSlideVersionError
 
    This version of OpenSlide does not support the requested functionality.
    Subclass of :exc:`OpenSlideError`.
 
 
-Wrapping a PIL Image
-====================
+.. _wrapping-a-pil-image:
+
+Wrapping a Pillow Image
+=======================
 
 .. class:: ImageSlide(file)
 
    A wrapper around an :class:`Image <PIL.Image.Image>` object that
    provides an :class:`OpenSlide`-compatible API.
 
    :param file: a filename or :class:`Image <PIL.Image.Image>` object
@@ -317,15 +376,15 @@
 .. module:: openslide.deepzoom
 
 OpenSlide Python provides functionality for generating individual
 `Deep Zoom`_ tiles from slide objects.  This is useful for displaying
 whole-slide images in a web browser without converting the entire slide to
 Deep Zoom or a similar format.
 
-.. _`Deep Zoom`: http://msdn.microsoft.com/en-us/library/cc645050%28VS.95%29.aspx
+.. _`Deep Zoom`: https://docs.microsoft.com/en-us/previous-versions/windows/silverlight/dotnet-windows-silverlight/cc645050(v=vs.95)
 
 .. class:: DeepZoomGenerator(osr, tile_size=254, overlap=1, limit_bounds=False)
 
    A Deep Zoom generator that wraps an
    :class:`OpenSlide <openslide.OpenSlide>` or
    :class:`ImageSlide <openslide.ImageSlide>` object.
```

### Comparing `openslide-python-1.2.0/doc/jekyll_fix.py` & `openslide-python-1.3.0/doc/jekyll_fix.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,65 +13,72 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
-# Sphinx hardcodes that certain output directories have names starting with
+# Sphinx hardcodes that certain output paths have names starting with
 # an underscore.
 # Jekyll hardcodes that filenames starting with an underscore are not
 # deployed to the website.
-# Rename Sphinx output directories to drop the underscore.
+# Rename Sphinx output paths to drop the underscore.
 
 import os
 
+from sphinx.util import logging
 from sphinx.util.console import bold
 
 DIRS = {
     '_static': 'static',
     '_sources': 'sources',
 }
+FILES = {
+    # Added in Sphinx 5.0.0, scheduled to be removed in Sphinx 6
+    'static/_sphinx_javascript_frameworks_compat.js': 'static/sphinx_javascript_frameworks_compat.js',  # noqa: E501
+}
 REWRITE_EXTENSIONS = {'.html', '.js'}
 
 
-def remove_directory_underscores(app, exception):
+def remove_path_underscores(app, exception):
     if exception:
         return
     # Get logger
-    try:
-        from sphinx.util import logging
-
-        logger = logging.getLogger(__name__)
-    except (ImportError, AttributeError):
-        # Sphinx < 1.6
-        logger = app
-    logger.info(bold('fixing directory names... '), nonl=True)
+    logger = logging.getLogger(__name__)
+    logger.info(bold('fixing pathnames... '), nonl=True)
     # Rewrite references in HTML/JS files
     for dirpath, _, filenames in os.walk(app.outdir):
         for filename in filenames:
             _, ext = os.path.splitext(filename)
             if ext in REWRITE_EXTENSIONS:
                 path = os.path.join(dirpath, filename)
                 with open(path, encoding='utf-8') as fh:
                     contents = fh.read()
                 for old, new in DIRS.items():
                     contents = contents.replace(old + '/', new + '/')
+                for old, new in FILES.items():
+                    contents = contents.replace(old, new)
                 with open(path, 'w', encoding='utf-8') as fh:
                     fh.write(contents)
     # Move directory contents
     for old, new in DIRS.items():
         olddir = os.path.join(app.outdir, old)
         newdir = os.path.join(app.outdir, new)
         if not os.path.exists(newdir):
             os.mkdir(newdir)
         if os.path.isdir(olddir):
             for filename in os.listdir(olddir):
                 oldfile = os.path.join(olddir, filename)
                 newfile = os.path.join(newdir, filename)
                 os.rename(oldfile, newfile)
             os.rmdir(olddir)
+    # Move files
+    for old, new in FILES.items():
+        oldfile = os.path.join(app.outdir, old)
+        newfile = os.path.join(app.outdir, new)
+        if os.path.isfile(oldfile):
+            os.rename(oldfile, newfile)
     logger.info('done')
 
 
 def setup(app):
-    app.connect('build-finished', remove_directory_underscores)
+    app.connect('build-finished', remove_path_underscores)
```

### Comparing `openslide-python-1.2.0/examples/deepzoom/deepzoom_multiserver.py` & `openslide-python-1.3.0/examples/deepzoom/deepzoom_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #
-# deepzoom_multiserver - Example web application for viewing multiple slides
+# deepzoom_server - Example web application for serving whole-slide images
 #
 # Copyright (c) 2010-2015 Carnegie Mellon University
-# Copyright (c) 2021-2022 Benjamin Gilbert
+# Copyright (c) 2023      Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -15,268 +15,302 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
-from collections import OrderedDict
+from argparse import ArgumentParser
+import base64
 from io import BytesIO
-from optparse import OptionParser
 import os
-from threading import Lock
+import re
+from unicodedata import normalize
+import zlib
 
+from PIL import ImageCms
 from flask import Flask, abort, make_response, render_template, url_for
 
 if os.name == 'nt':
     _dll_path = os.getenv('OPENSLIDE_PATH')
     if _dll_path is not None:
-        if hasattr(os, 'add_dll_directory'):
-            # Python >= 3.8
-            with os.add_dll_directory(_dll_path):
-                import openslide
-        else:
-            # Python < 3.8
-            _orig_path = os.environ.get('PATH', '')
-            os.environ['PATH'] = _orig_path + ';' + _dll_path
+        with os.add_dll_directory(_dll_path):
             import openslide
-
-            os.environ['PATH'] = _orig_path
+    else:
+        import openslide
 else:
     import openslide
 
-from openslide import OpenSlide, OpenSlideCache, OpenSlideError, OpenSlideVersionError
+from openslide import ImageSlide, open_slide
 from openslide.deepzoom import DeepZoomGenerator
 
-SLIDE_DIR = '.'
-SLIDE_CACHE_SIZE = 10
-SLIDE_TILE_CACHE_MB = 128
-DEEPZOOM_FORMAT = 'jpeg'
-DEEPZOOM_TILE_SIZE = 254
-DEEPZOOM_OVERLAP = 1
-DEEPZOOM_LIMIT_BOUNDS = True
-DEEPZOOM_TILE_QUALITY = 75
-
-app = Flask(__name__)
-app.config.from_object(__name__)
-app.config.from_envvar('DEEPZOOM_MULTISERVER_SETTINGS', silent=True)
-
-
-class _SlideCache:
-    def __init__(self, cache_size, tile_cache_mb, dz_opts):
-        self.cache_size = cache_size
-        self.dz_opts = dz_opts
-        self._lock = Lock()
-        self._cache = OrderedDict()
-        # Share a single tile cache among all slide handles, if supported
-        try:
-            self._tile_cache = OpenSlideCache(tile_cache_mb * 1024 * 1024)
-        except OpenSlideVersionError:
-            self._tile_cache = None
-
-    def get(self, path):
-        with self._lock:
-            if path in self._cache:
-                # Move to end of LRU
-                slide = self._cache.pop(path)
-                self._cache[path] = slide
-                return slide
-
-        osr = OpenSlide(path)
-        if self._tile_cache is not None:
-            osr.set_cache(self._tile_cache)
-        slide = DeepZoomGenerator(osr, **self.dz_opts)
-        try:
-            mpp_x = osr.properties[openslide.PROPERTY_NAME_MPP_X]
-            mpp_y = osr.properties[openslide.PROPERTY_NAME_MPP_Y]
-            slide.mpp = (float(mpp_x) + float(mpp_y)) / 2
-        except (KeyError, ValueError):
-            slide.mpp = 0
-
-        with self._lock:
-            if path not in self._cache:
-                if len(self._cache) == self.cache_size:
-                    self._cache.popitem(last=False)
-                self._cache[path] = slide
-        return slide
-
-
-class _Directory:
-    def __init__(self, basedir, relpath=''):
-        self.name = os.path.basename(relpath)
-        self.children = []
-        for name in sorted(os.listdir(os.path.join(basedir, relpath))):
-            cur_relpath = os.path.join(relpath, name)
-            cur_path = os.path.join(basedir, cur_relpath)
-            if os.path.isdir(cur_path):
-                cur_dir = _Directory(basedir, cur_relpath)
-                if cur_dir.children:
-                    self.children.append(cur_dir)
-            elif OpenSlide.detect_format(cur_path):
-                self.children.append(_SlideFile(cur_relpath))
-
-
-class _SlideFile:
-    def __init__(self, relpath):
-        self.name = os.path.basename(relpath)
-        self.url_path = relpath
-
-
-@app.before_first_request
-def _setup():
-    app.basedir = os.path.abspath(app.config['SLIDE_DIR'])
+SLIDE_NAME = 'slide'
+
+# Optimized sRGB v2 profile, CC0-1.0 license
+# https://github.com/saucecontrol/Compact-ICC-Profiles/blob/bdd84663/profiles/sRGB-v2-micro.icc
+# ImageCms.createProfile() generates a v4 profile and Firefox has problems
+# with those: https://littlecms.com/blog/2020/09/09/browser-check/
+SRGB_PROFILE_BYTES = zlib.decompress(
+    base64.b64decode(
+        'eNpjYGA8kZOcW8wkwMCQm1dSFOTupBARGaXA/oiBmUGEgZOBj0E2Mbm4wDfYLYQBCIoT'
+        'y4uTS4pyGFDAt2sMjCD6sm5GYl7K3IkMtg4NG2wdSnQa5y1V6mPADzhTUouTgfQHII5P'
+        'LigqYWBg5AGyecpLCkBsCSBbpAjoKCBbB8ROh7AdQOwkCDsErCYkyBnIzgCyE9KR2ElI'
+        'bKhdIMBaCvQsskNKUitKQLSzswEDKAwgop9DwH5jFDuJEMtfwMBg8YmBgbkfIZY0jYFh'
+        'eycDg8QthJgKUB1/KwPDtiPJpUVlUGu0gLiG4QfjHKZS5maWk2x+HEJcEjxJfF8Ez4t8'
+        'k8iS0VNwVlmjmaVXZ/zacrP9NbdwX7OQshjxFNmcttKwut4OnUlmc1Yv79l0e9/MU8ev'
+        'pz4p//jz/38AR4Nk5Q=='
+    )
+)
+SRGB_PROFILE = ImageCms.getOpenProfile(BytesIO(SRGB_PROFILE_BYTES))
+
+
+def create_app(config=None, config_file=None):
+    # Create and configure app
+    app = Flask(__name__)
+    app.config.from_mapping(
+        DEEPZOOM_SLIDE=None,
+        DEEPZOOM_FORMAT='jpeg',
+        DEEPZOOM_TILE_SIZE=254,
+        DEEPZOOM_OVERLAP=1,
+        DEEPZOOM_LIMIT_BOUNDS=True,
+        DEEPZOOM_TILE_QUALITY=75,
+        DEEPZOOM_COLOR_MODE='absolute-colorimetric',
+    )
+    app.config.from_envvar('DEEPZOOM_TILER_SETTINGS', silent=True)
+    if config_file is not None:
+        app.config.from_pyfile(config_file)
+    if config is not None:
+        app.config.from_mapping(config)
+
+    # Open slide
+    slidefile = app.config['DEEPZOOM_SLIDE']
+    if slidefile is None:
+        raise ValueError('No slide file specified')
     config_map = {
         'DEEPZOOM_TILE_SIZE': 'tile_size',
         'DEEPZOOM_OVERLAP': 'overlap',
         'DEEPZOOM_LIMIT_BOUNDS': 'limit_bounds',
     }
     opts = {v: app.config[k] for k, v in config_map.items()}
-    app.cache = _SlideCache(
-        app.config['SLIDE_CACHE_SIZE'], app.config['SLIDE_TILE_CACHE_MB'], opts
-    )
-
-
-def _get_slide(path):
-    path = os.path.abspath(os.path.join(app.basedir, path))
-    if not path.startswith(app.basedir + os.path.sep):
-        # Directory traversal
-        abort(404)
-    if not os.path.exists(path):
-        abort(404)
+    slide = open_slide(slidefile)
+    app.slides = {SLIDE_NAME: DeepZoomGenerator(slide, **opts)}
+    app.transforms = {
+        SLIDE_NAME: get_transform(slide, app.config['DEEPZOOM_COLOR_MODE'])
+    }
+    app.associated_images = []
+    app.slide_properties = slide.properties
+    for name, image in slide.associated_images.items():
+        app.associated_images.append(name)
+        slug = slugify(name)
+        image_slide = ImageSlide(image)
+        app.slides[slug] = DeepZoomGenerator(image_slide, **opts)
+        app.transforms[slug] = get_transform(
+            image_slide, app.config['DEEPZOOM_COLOR_MODE']
+        )
     try:
-        slide = app.cache.get(path)
-        slide.filename = os.path.basename(path)
-        return slide
-    except OpenSlideError:
-        abort(404)
-
-
-@app.route('/')
-def index():
-    return render_template('files.html', root_dir=_Directory(app.basedir))
-
-
-@app.route('/<path:path>')
-def slide(path):
-    slide = _get_slide(path)
-    slide_url = url_for('dzi', path=path)
-    return render_template(
-        'slide-fullpage.html',
-        slide_url=slide_url,
-        slide_filename=slide.filename,
-        slide_mpp=slide.mpp,
-    )
-
+        mpp_x = slide.properties[openslide.PROPERTY_NAME_MPP_X]
+        mpp_y = slide.properties[openslide.PROPERTY_NAME_MPP_Y]
+        app.slide_mpp = (float(mpp_x) + float(mpp_y)) / 2
+    except (KeyError, ValueError):
+        app.slide_mpp = 0
+
+    # Set up routes
+    @app.route('/')
+    def index():
+        slide_url = url_for('dzi', slug=SLIDE_NAME)
+        associated_urls = {
+            name: url_for('dzi', slug=slugify(name)) for name in app.associated_images
+        }
+        return render_template(
+            'slide-multipane.html',
+            slide_url=slide_url,
+            associated=associated_urls,
+            properties=app.slide_properties,
+            slide_mpp=app.slide_mpp,
+        )
+
+    @app.route('/<slug>.dzi')
+    def dzi(slug):
+        format = app.config['DEEPZOOM_FORMAT']
+        try:
+            resp = make_response(app.slides[slug].get_dzi(format))
+            resp.mimetype = 'application/xml'
+            return resp
+        except KeyError:
+            # Unknown slug
+            abort(404)
+
+    @app.route('/<slug>_files/<int:level>/<int:col>_<int:row>.<format>')
+    def tile(slug, level, col, row, format):
+        format = format.lower()
+        if format != 'jpeg' and format != 'png':
+            # Not supported by Deep Zoom
+            abort(404)
+        try:
+            tile = app.slides[slug].get_tile(level, (col, row))
+        except KeyError:
+            # Unknown slug
+            abort(404)
+        except ValueError:
+            # Invalid level or coordinates
+            abort(404)
+        app.transforms[slug](tile)
+        buf = BytesIO()
+        tile.save(
+            buf,
+            format,
+            quality=app.config['DEEPZOOM_TILE_QUALITY'],
+            icc_profile=tile.info.get('icc_profile'),
+        )
+        resp = make_response(buf.getvalue())
+        resp.mimetype = 'image/%s' % format
+        return resp
+
+    return app
+
+
+def slugify(text):
+    text = normalize('NFKD', text.lower()).encode('ascii', 'ignore').decode()
+    return re.sub('[^a-z0-9]+', '-', text)
+
+
+def get_transform(image, mode):
+    if image.color_profile is None:
+        return lambda img: None
+    if mode == 'ignore':
+        # drop ICC profile from tiles
+        return lambda img: img.info.pop('icc_profile')
+    elif mode == 'embed':
+        # embed ICC profile in tiles
+        return lambda img: None
+    elif mode == 'absolute-colorimetric':
+        intent = ImageCms.Intent.ABSOLUTE_COLORIMETRIC
+    elif mode == 'relative-colorimetric':
+        intent = ImageCms.Intent.RELATIVE_COLORIMETRIC
+    elif mode == 'perceptual':
+        intent = ImageCms.Intent.PERCEPTUAL
+    elif mode == 'saturation':
+        intent = ImageCms.Intent.SATURATION
+    else:
+        raise ValueError(f'Unknown color mode {mode}')
+    transform = ImageCms.buildTransform(
+        image.color_profile,
+        SRGB_PROFILE,
+        'RGB',
+        'RGB',
+        intent,
+        0,
+    )
+
+    def xfrm(img):
+        ImageCms.applyTransform(img, transform, True)
+        # Some browsers assume we intend the display's color space if we don't
+        # embed the profile.  Pillow's serialization is larger, so use ours.
+        img.info['icc_profile'] = SRGB_PROFILE_BYTES
 
-@app.route('/<path:path>.dzi')
-def dzi(path):
-    slide = _get_slide(path)
-    format = app.config['DEEPZOOM_FORMAT']
-    resp = make_response(slide.get_dzi(format))
-    resp.mimetype = 'application/xml'
-    return resp
-
-
-@app.route('/<path:path>_files/<int:level>/<int:col>_<int:row>.<format>')
-def tile(path, level, col, row, format):
-    slide = _get_slide(path)
-    format = format.lower()
-    if format != 'jpeg' and format != 'png':
-        # Not supported by Deep Zoom
-        abort(404)
-    try:
-        tile = slide.get_tile(level, (col, row))
-    except ValueError:
-        # Invalid level or coordinates
-        abort(404)
-    buf = BytesIO()
-    tile.save(buf, format, quality=app.config['DEEPZOOM_TILE_QUALITY'])
-    resp = make_response(buf.getvalue())
-    resp.mimetype = 'image/%s' % format
-    return resp
+    return xfrm
 
 
 if __name__ == '__main__':
-    parser = OptionParser(usage='Usage: %prog [options] [slide-directory]')
-    parser.add_option(
+    parser = ArgumentParser(usage='%(prog)s [options] [SLIDE]')
+    parser.add_argument(
         '-B',
         '--ignore-bounds',
         dest='DEEPZOOM_LIMIT_BOUNDS',
         default=True,
         action='store_false',
         help='display entire scan area',
     )
-    parser.add_option(
+    parser.add_argument(
+        '--color-mode',
+        dest='DEEPZOOM_COLOR_MODE',
+        choices=[
+            'absolute-colorimetric',
+            'perceptual',
+            'relative-colorimetric',
+            'saturation',
+            'embed',
+            'ignore',
+        ],
+        default='absolute-colorimetric',
+        help=(
+            'convert tiles to sRGB using specified rendering intent, or '
+            'embed original ICC profile, or ignore ICC profile (compat) '
+            '[absolute-colorimetric]'
+        ),
+    )
+    parser.add_argument(
         '-c', '--config', metavar='FILE', dest='config', help='config file'
     )
-    parser.add_option(
+    parser.add_argument(
         '-d',
         '--debug',
         dest='DEBUG',
         action='store_true',
         help='run in debugging mode (insecure)',
     )
-    parser.add_option(
+    parser.add_argument(
         '-e',
         '--overlap',
         metavar='PIXELS',
         dest='DEEPZOOM_OVERLAP',
-        type='int',
+        type=int,
         help='overlap of adjacent tiles [1]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-f',
         '--format',
         metavar='{jpeg|png}',
         dest='DEEPZOOM_FORMAT',
         help='image format for tiles [jpeg]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-l',
         '--listen',
         metavar='ADDRESS',
         dest='host',
         default='127.0.0.1',
         help='address to listen on [127.0.0.1]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-p',
         '--port',
         metavar='PORT',
         dest='port',
-        type='int',
+        type=int,
         default=5000,
         help='port to listen on [5000]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-Q',
         '--quality',
         metavar='QUALITY',
         dest='DEEPZOOM_TILE_QUALITY',
-        type='int',
+        type=int,
         help='JPEG compression quality [75]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-s',
         '--size',
         metavar='PIXELS',
         dest='DEEPZOOM_TILE_SIZE',
-        type='int',
+        type=int,
         help='tile size [254]',
     )
+    parser.add_argument(
+        'DEEPZOOM_SLIDE',
+        metavar='SLIDE',
+        nargs='?',
+        help='slide file',
+    )
+
+    args = parser.parse_args()
+    config = {}
+    config_file = args.config
+    # Set only those settings specified on the command line
+    for k in dir(args):
+        v = getattr(args, k)
+        if not k.startswith('_') and v is not None:
+            config[k] = v
+    app = create_app(config, config_file)
 
-    (opts, args) = parser.parse_args()
-    # Load config file if specified
-    if opts.config is not None:
-        app.config.from_pyfile(opts.config)
-    # Overwrite only those settings specified on the command line
-    for k in dir(opts):
-        if not k.startswith('_') and getattr(opts, k) is None:
-            delattr(opts, k)
-    app.config.from_object(opts)
-    # Set slide directory
-    try:
-        app.config['SLIDE_DIR'] = args[0]
-    except IndexError:
-        pass
-
-    app.run(host=opts.host, port=opts.port, threaded=True)
+    app.run(host=args.host, port=args.port, threaded=True)
```

### Comparing `openslide-python-1.2.0/examples/deepzoom/deepzoom_tile.py` & `openslide-python-1.3.0/examples/deepzoom/deepzoom_multiserver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #
-# deepzoom_tile - Convert whole-slide images to Deep Zoom format
+# deepzoom_multiserver - Example web application for viewing multiple slides
 #
 # Copyright (c) 2010-2015 Carnegie Mellon University
-# Copyright (c) 2022      Benjamin Gilbert
+# Copyright (c) 2021-2023 Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -15,350 +15,354 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
-"""An example program to generate a Deep Zoom directory tree from a slide."""
-
-import json
-from multiprocessing import JoinableQueue, Process
-from optparse import OptionParser
+from argparse import ArgumentParser
+import base64
+from collections import OrderedDict
+from io import BytesIO
 import os
-import re
-import shutil
-import sys
-from unicodedata import normalize
+from threading import Lock
+import zlib
+
+from PIL import ImageCms
+from flask import Flask, abort, make_response, render_template, url_for
 
 if os.name == 'nt':
     _dll_path = os.getenv('OPENSLIDE_PATH')
     if _dll_path is not None:
-        if hasattr(os, 'add_dll_directory'):
-            # Python >= 3.8
-            with os.add_dll_directory(_dll_path):
-                import openslide
-        else:
-            # Python < 3.8
-            _orig_path = os.environ.get('PATH', '')
-            os.environ['PATH'] = _orig_path + ';' + _dll_path
+        with os.add_dll_directory(_dll_path):
             import openslide
-
-            os.environ['PATH'] = _orig_path
+    else:
+        import openslide
 else:
     import openslide
 
-from openslide import ImageSlide, open_slide
+from openslide import OpenSlide, OpenSlideCache, OpenSlideError, OpenSlideVersionError
 from openslide.deepzoom import DeepZoomGenerator
 
-VIEWER_SLIDE_NAME = 'slide'
+# Optimized sRGB v2 profile, CC0-1.0 license
+# https://github.com/saucecontrol/Compact-ICC-Profiles/blob/bdd84663/profiles/sRGB-v2-micro.icc
+# ImageCms.createProfile() generates a v4 profile and Firefox has problems
+# with those: https://littlecms.com/blog/2020/09/09/browser-check/
+SRGB_PROFILE_BYTES = zlib.decompress(
+    base64.b64decode(
+        'eNpjYGA8kZOcW8wkwMCQm1dSFOTupBARGaXA/oiBmUGEgZOBj0E2Mbm4wDfYLYQBCIoT'
+        'y4uTS4pyGFDAt2sMjCD6sm5GYl7K3IkMtg4NG2wdSnQa5y1V6mPADzhTUouTgfQHII5P'
+        'LigqYWBg5AGyecpLCkBsCSBbpAjoKCBbB8ROh7AdQOwkCDsErCYkyBnIzgCyE9KR2ElI'
+        'bKhdIMBaCvQsskNKUitKQLSzswEDKAwgop9DwH5jFDuJEMtfwMBg8YmBgbkfIZY0jYFh'
+        'eycDg8QthJgKUB1/KwPDtiPJpUVlUGu0gLiG4QfjHKZS5maWk2x+HEJcEjxJfF8Ez4t8'
+        'k8iS0VNwVlmjmaVXZ/zacrP9NbdwX7OQshjxFNmcttKwut4OnUlmc1Yv79l0e9/MU8ev'
+        'pz4p//jz/38AR4Nk5Q=='
+    )
+)
+SRGB_PROFILE = ImageCms.getOpenProfile(BytesIO(SRGB_PROFILE_BYTES))
 
 
-class TileWorker(Process):
-    """A child process that generates and writes tiles."""
+def create_app(config=None, config_file=None):
+    # Create and configure app
+    app = Flask(__name__)
+    app.config.from_mapping(
+        SLIDE_DIR='.',
+        SLIDE_CACHE_SIZE=10,
+        SLIDE_TILE_CACHE_MB=128,
+        DEEPZOOM_FORMAT='jpeg',
+        DEEPZOOM_TILE_SIZE=254,
+        DEEPZOOM_OVERLAP=1,
+        DEEPZOOM_LIMIT_BOUNDS=True,
+        DEEPZOOM_TILE_QUALITY=75,
+        DEEPZOOM_COLOR_MODE='absolute-colorimetric',
+    )
+    app.config.from_envvar('DEEPZOOM_MULTISERVER_SETTINGS', silent=True)
+    if config_file is not None:
+        app.config.from_pyfile(config_file)
+    if config is not None:
+        app.config.from_mapping(config)
+
+    # Set up cache
+    app.basedir = os.path.abspath(app.config['SLIDE_DIR'])
+    config_map = {
+        'DEEPZOOM_TILE_SIZE': 'tile_size',
+        'DEEPZOOM_OVERLAP': 'overlap',
+        'DEEPZOOM_LIMIT_BOUNDS': 'limit_bounds',
+    }
+    opts = {v: app.config[k] for k, v in config_map.items()}
+    app.cache = _SlideCache(
+        app.config['SLIDE_CACHE_SIZE'],
+        app.config['SLIDE_TILE_CACHE_MB'],
+        opts,
+        app.config['DEEPZOOM_COLOR_MODE'],
+    )
 
-    def __init__(self, queue, slidepath, tile_size, overlap, limit_bounds, quality):
-        Process.__init__(self, name='TileWorker')
-        self.daemon = True
-        self._queue = queue
-        self._slidepath = slidepath
-        self._tile_size = tile_size
-        self._overlap = overlap
-        self._limit_bounds = limit_bounds
-        self._quality = quality
-        self._slide = None
-
-    def run(self):
-        self._slide = open_slide(self._slidepath)
-        last_associated = None
-        dz = self._get_dz()
-        while True:
-            data = self._queue.get()
-            if data is None:
-                self._queue.task_done()
-                break
-            associated, level, address, outfile = data
-            if last_associated != associated:
-                dz = self._get_dz(associated)
-                last_associated = associated
-            tile = dz.get_tile(level, address)
-            tile.save(outfile, quality=self._quality)
-            self._queue.task_done()
-
-    def _get_dz(self, associated=None):
-        if associated is not None:
-            image = ImageSlide(self._slide.associated_images[associated])
-        else:
-            image = self._slide
-        return DeepZoomGenerator(
-            image, self._tile_size, self._overlap, limit_bounds=self._limit_bounds
+    # Helper functions
+    def get_slide(path):
+        path = os.path.abspath(os.path.join(app.basedir, path))
+        if not path.startswith(app.basedir + os.path.sep):
+            # Directory traversal
+            abort(404)
+        if not os.path.exists(path):
+            abort(404)
+        try:
+            slide = app.cache.get(path)
+            slide.filename = os.path.basename(path)
+            return slide
+        except OpenSlideError:
+            abort(404)
+
+    # Set up routes
+    @app.route('/')
+    def index():
+        return render_template('files.html', root_dir=_Directory(app.basedir))
+
+    @app.route('/<path:path>')
+    def slide(path):
+        slide = get_slide(path)
+        slide_url = url_for('dzi', path=path)
+        return render_template(
+            'slide-fullpage.html',
+            slide_url=slide_url,
+            slide_filename=slide.filename,
+            slide_mpp=slide.mpp,
         )
 
-
-class DeepZoomImageTiler:
-    """Handles generation of tiles and metadata for a single image."""
-
-    def __init__(self, dz, basename, format, associated, queue):
-        self._dz = dz
-        self._basename = basename
-        self._format = format
-        self._associated = associated
-        self._queue = queue
-        self._processed = 0
-
-    def run(self):
-        self._write_tiles()
-        self._write_dzi()
-
-    def _write_tiles(self):
-        for level in range(self._dz.level_count):
-            tiledir = os.path.join("%s_files" % self._basename, str(level))
-            if not os.path.exists(tiledir):
-                os.makedirs(tiledir)
-            cols, rows = self._dz.level_tiles[level]
-            for row in range(rows):
-                for col in range(cols):
-                    tilename = os.path.join(
-                        tiledir, '%d_%d.%s' % (col, row, self._format)
-                    )
-                    if not os.path.exists(tilename):
-                        self._queue.put((self._associated, level, (col, row), tilename))
-                    self._tile_done()
-
-    def _tile_done(self):
-        self._processed += 1
-        count, total = self._processed, self._dz.tile_count
-        if count % 100 == 0 or count == total:
-            print(
-                "Tiling %s: wrote %d/%d tiles"
-                % (self._associated or 'slide', count, total),
-                end='\r',
-                file=sys.stderr,
-            )
-            if count == total:
-                print(file=sys.stderr)
-
-    def _write_dzi(self):
-        with open('%s.dzi' % self._basename, 'w') as fh:
-            fh.write(self.get_dzi())
-
-    def get_dzi(self):
-        return self._dz.get_dzi(self._format)
-
-
-class DeepZoomStaticTiler:
-    """Handles generation of tiles and metadata for all images in a slide."""
-
-    def __init__(
-        self,
-        slidepath,
-        basename,
-        format,
-        tile_size,
-        overlap,
-        limit_bounds,
-        quality,
-        workers,
-        with_viewer,
-    ):
-        if with_viewer:
-            # Check extra dependency before doing a bunch of work
-            import jinja2  # noqa: F401  module-imported-but-unused
-        self._slide = open_slide(slidepath)
-        self._basename = basename
-        self._format = format
-        self._tile_size = tile_size
-        self._overlap = overlap
-        self._limit_bounds = limit_bounds
-        self._queue = JoinableQueue(2 * workers)
-        self._workers = workers
-        self._with_viewer = with_viewer
-        self._dzi_data = {}
-        for _i in range(workers):
-            TileWorker(
-                self._queue, slidepath, tile_size, overlap, limit_bounds, quality
-            ).start()
-
-    def run(self):
-        self._run_image()
-        if self._with_viewer:
-            for name in self._slide.associated_images:
-                self._run_image(name)
-            self._write_html()
-            self._write_static()
-        self._shutdown()
-
-    def _run_image(self, associated=None):
-        """Run a single image from self._slide."""
-        if associated is None:
-            image = self._slide
-            if self._with_viewer:
-                basename = os.path.join(self._basename, VIEWER_SLIDE_NAME)
-            else:
-                basename = self._basename
-        else:
-            image = ImageSlide(self._slide.associated_images[associated])
-            basename = os.path.join(self._basename, self._slugify(associated))
-        dz = DeepZoomGenerator(
-            image, self._tile_size, self._overlap, limit_bounds=self._limit_bounds
+    @app.route('/<path:path>.dzi')
+    def dzi(path):
+        slide = get_slide(path)
+        format = app.config['DEEPZOOM_FORMAT']
+        resp = make_response(slide.get_dzi(format))
+        resp.mimetype = 'application/xml'
+        return resp
+
+    @app.route('/<path:path>_files/<int:level>/<int:col>_<int:row>.<format>')
+    def tile(path, level, col, row, format):
+        slide = get_slide(path)
+        format = format.lower()
+        if format != 'jpeg' and format != 'png':
+            # Not supported by Deep Zoom
+            abort(404)
+        try:
+            tile = slide.get_tile(level, (col, row))
+        except ValueError:
+            # Invalid level or coordinates
+            abort(404)
+        slide.transform(tile)
+        buf = BytesIO()
+        tile.save(
+            buf,
+            format,
+            quality=app.config['DEEPZOOM_TILE_QUALITY'],
+            icc_profile=tile.info.get('icc_profile'),
         )
-        tiler = DeepZoomImageTiler(dz, basename, self._format, associated, self._queue)
-        tiler.run()
-        self._dzi_data[self._url_for(associated)] = tiler.get_dzi()
-
-    def _url_for(self, associated):
-        if associated is None:
-            base = VIEWER_SLIDE_NAME
-        else:
-            base = self._slugify(associated)
-        return '%s.dzi' % base
+        resp = make_response(buf.getvalue())
+        resp.mimetype = 'image/%s' % format
+        return resp
+
+    return app
 
-    def _write_html(self):
-        import jinja2
 
-        # https://docs.python.org/3/reference/import.html#main-spec
-        if __spec__ is not None:
-            # We're running from a module (e.g. "python -m deepzoom_tile")
-            # so load templates from the containing package.
-            loader = jinja2.PackageLoader('__main__')
-        else:
-            # We're not running from a module (e.g. "python deepzoom_tile.py")
-            # so PackageLoader('__main__') doesn't work in jinja2 3.x.
-            # Load templates directly from the filesystem.
-            loader = jinja2.FileSystemLoader(
-                os.path.join(os.path.dirname(__file__), 'templates')
-            )
-        env = jinja2.Environment(loader=loader, autoescape=True)
-        template = env.get_template('slide-multipane.html')
-        associated_urls = {n: self._url_for(n) for n in self._slide.associated_images}
+class _SlideCache:
+    def __init__(self, cache_size, tile_cache_mb, dz_opts, color_mode):
+        self.cache_size = cache_size
+        self.dz_opts = dz_opts
+        self.color_mode = color_mode
+        self._lock = Lock()
+        self._cache = OrderedDict()
+        # Share a single tile cache among all slide handles, if supported
         try:
-            mpp_x = self._slide.properties[openslide.PROPERTY_NAME_MPP_X]
-            mpp_y = self._slide.properties[openslide.PROPERTY_NAME_MPP_Y]
-            mpp = (float(mpp_x) + float(mpp_y)) / 2
+            self._tile_cache = OpenSlideCache(tile_cache_mb * 1024 * 1024)
+        except OpenSlideVersionError:
+            self._tile_cache = None
+
+    def get(self, path):
+        with self._lock:
+            if path in self._cache:
+                # Move to end of LRU
+                slide = self._cache.pop(path)
+                self._cache[path] = slide
+                return slide
+
+        osr = OpenSlide(path)
+        if self._tile_cache is not None:
+            osr.set_cache(self._tile_cache)
+        slide = DeepZoomGenerator(osr, **self.dz_opts)
+        try:
+            mpp_x = osr.properties[openslide.PROPERTY_NAME_MPP_X]
+            mpp_y = osr.properties[openslide.PROPERTY_NAME_MPP_Y]
+            slide.mpp = (float(mpp_x) + float(mpp_y)) / 2
         except (KeyError, ValueError):
-            mpp = 0
-        # Embed the dzi metadata in the HTML to work around Chrome's
-        # refusal to allow XmlHttpRequest from file:///, even when
-        # the originating page is also a file:///
-        data = template.render(
-            slide_url=self._url_for(None),
-            slide_mpp=mpp,
-            associated=associated_urls,
-            properties=self._slide.properties,
-            dzi_data=json.dumps(self._dzi_data),
+            slide.mpp = 0
+        slide.transform = self._get_transform(osr)
+
+        with self._lock:
+            if path not in self._cache:
+                if len(self._cache) == self.cache_size:
+                    self._cache.popitem(last=False)
+                self._cache[path] = slide
+        return slide
+
+    def _get_transform(self, image):
+        if image.color_profile is None:
+            return lambda img: None
+        mode = self.color_mode
+        if mode == 'ignore':
+            # drop ICC profile from tiles
+            return lambda img: img.info.pop('icc_profile')
+        elif mode == 'embed':
+            # embed ICC profile in tiles
+            return lambda img: None
+        elif mode == 'absolute-colorimetric':
+            intent = ImageCms.Intent.ABSOLUTE_COLORIMETRIC
+        elif mode == 'relative-colorimetric':
+            intent = ImageCms.Intent.RELATIVE_COLORIMETRIC
+        elif mode == 'perceptual':
+            intent = ImageCms.Intent.PERCEPTUAL
+        elif mode == 'saturation':
+            intent = ImageCms.Intent.SATURATION
+        else:
+            raise ValueError(f'Unknown color mode {mode}')
+        transform = ImageCms.buildTransform(
+            image.color_profile,
+            SRGB_PROFILE,
+            'RGB',
+            'RGB',
+            intent,
+            0,
         )
-        with open(os.path.join(self._basename, 'index.html'), 'w') as fh:
-            fh.write(data)
 
-    def _write_static(self):
-        basesrc = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static')
-        basedst = os.path.join(self._basename, 'static')
-        self._copydir(basesrc, basedst)
-        self._copydir(os.path.join(basesrc, 'images'), os.path.join(basedst, 'images'))
-
-    def _copydir(self, src, dest):
-        if not os.path.exists(dest):
-            os.makedirs(dest)
-        for name in os.listdir(src):
-            srcpath = os.path.join(src, name)
-            if os.path.isfile(srcpath):
-                shutil.copy(srcpath, os.path.join(dest, name))
-
-    @classmethod
-    def _slugify(cls, text):
-        text = normalize('NFKD', text.lower()).encode('ascii', 'ignore').decode()
-        return re.sub('[^a-z0-9]+', '_', text)
-
-    def _shutdown(self):
-        for _i in range(self._workers):
-            self._queue.put(None)
-        self._queue.join()
+        def xfrm(img):
+            ImageCms.applyTransform(img, transform, True)
+            # Some browsers assume we intend the display's color space if we
+            # don't embed the profile.  Pillow's serialization is larger, so
+            # use ours.
+            img.info['icc_profile'] = SRGB_PROFILE_BYTES
+
+        return xfrm
+
+
+class _Directory:
+    def __init__(self, basedir, relpath=''):
+        self.name = os.path.basename(relpath)
+        self.children = []
+        for name in sorted(os.listdir(os.path.join(basedir, relpath))):
+            cur_relpath = os.path.join(relpath, name)
+            cur_path = os.path.join(basedir, cur_relpath)
+            if os.path.isdir(cur_path):
+                cur_dir = _Directory(basedir, cur_relpath)
+                if cur_dir.children:
+                    self.children.append(cur_dir)
+            elif OpenSlide.detect_format(cur_path):
+                self.children.append(_SlideFile(cur_relpath))
+
+
+class _SlideFile:
+    def __init__(self, relpath):
+        self.name = os.path.basename(relpath)
+        self.url_path = relpath
 
 
 if __name__ == '__main__':
-    parser = OptionParser(usage='Usage: %prog [options] <slide>')
-    parser.add_option(
+    parser = ArgumentParser(usage='%(prog)s [options] [SLIDE-DIRECTORY]')
+    parser.add_argument(
         '-B',
         '--ignore-bounds',
-        dest='limit_bounds',
+        dest='DEEPZOOM_LIMIT_BOUNDS',
         default=True,
         action='store_false',
         help='display entire scan area',
     )
-    parser.add_option(
+    parser.add_argument(
+        '--color-mode',
+        dest='DEEPZOOM_COLOR_MODE',
+        choices=[
+            'absolute-colorimetric',
+            'perceptual',
+            'relative-colorimetric',
+            'saturation',
+            'embed',
+            'ignore',
+        ],
+        default='absolute-colorimetric',
+        help=(
+            'convert tiles to sRGB using specified rendering intent, or '
+            'embed original ICC profile, or ignore ICC profile (compat) '
+            '[absolute-colorimetric]'
+        ),
+    )
+    parser.add_argument(
+        '-c', '--config', metavar='FILE', dest='config', help='config file'
+    )
+    parser.add_argument(
+        '-d',
+        '--debug',
+        dest='DEBUG',
+        action='store_true',
+        help='run in debugging mode (insecure)',
+    )
+    parser.add_argument(
         '-e',
         '--overlap',
         metavar='PIXELS',
-        dest='overlap',
-        type='int',
-        default=1,
+        dest='DEEPZOOM_OVERLAP',
+        type=int,
         help='overlap of adjacent tiles [1]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-f',
         '--format',
         metavar='{jpeg|png}',
-        dest='format',
-        default='jpeg',
+        dest='DEEPZOOM_FORMAT',
         help='image format for tiles [jpeg]',
     )
-    parser.add_option(
-        '-j',
-        '--jobs',
-        metavar='COUNT',
-        dest='workers',
-        type='int',
-        default=4,
-        help='number of worker processes to start [4]',
-    )
-    parser.add_option(
-        '-o',
-        '--output',
-        metavar='NAME',
-        dest='basename',
-        help='base name of output file',
+    parser.add_argument(
+        '-l',
+        '--listen',
+        metavar='ADDRESS',
+        dest='host',
+        default='127.0.0.1',
+        help='address to listen on [127.0.0.1]',
+    )
+    parser.add_argument(
+        '-p',
+        '--port',
+        metavar='PORT',
+        dest='port',
+        type=int,
+        default=5000,
+        help='port to listen on [5000]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-Q',
         '--quality',
         metavar='QUALITY',
-        dest='quality',
-        type='int',
-        default=90,
-        help='JPEG compression quality [90]',
-    )
-    parser.add_option(
-        '-r',
-        '--viewer',
-        dest='with_viewer',
-        action='store_true',
-        help='generate directory tree with HTML viewer',
+        dest='DEEPZOOM_TILE_QUALITY',
+        type=int,
+        help='JPEG compression quality [75]',
     )
-    parser.add_option(
+    parser.add_argument(
         '-s',
         '--size',
         metavar='PIXELS',
-        dest='tile_size',
-        type='int',
-        default=254,
+        dest='DEEPZOOM_TILE_SIZE',
+        type=int,
         help='tile size [254]',
     )
+    parser.add_argument(
+        'SLIDE_DIR',
+        metavar='SLIDE-DIRECTORY',
+        nargs='?',
+        help='slide directory',
+    )
+
+    args = parser.parse_args()
+    config = {}
+    config_file = args.config
+    # Set only those settings specified on the command line
+    for k in dir(args):
+        v = getattr(args, k)
+        if not k.startswith('_') and v is not None:
+            config[k] = v
+    app = create_app(config, config_file)
 
-    (opts, args) = parser.parse_args()
-    try:
-        slidepath = args[0]
-    except IndexError:
-        parser.error('Missing slide argument')
-    if opts.basename is None:
-        opts.basename = os.path.splitext(os.path.basename(slidepath))[0]
-
-    DeepZoomStaticTiler(
-        slidepath,
-        opts.basename,
-        opts.format,
-        opts.tile_size,
-        opts.overlap,
-        opts.limit_bounds,
-        opts.quality,
-        opts.workers,
-        opts.with_viewer,
-    ).run()
+    app.run(host=args.host, port=args.port, threaded=True)
```

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/fullpage_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/fullpage_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/home_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/home_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/home_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/home_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/home_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/home_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/home_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/home_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/next_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/next_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/next_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/next_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/next_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/next_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/next_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/next_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/previous_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/previous_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/previous_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/previous_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/previous_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/previous_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/previous_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/previous_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateleft_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateleft_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/rotateright_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/rotateright_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomin_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomin_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_grouphover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_grouphover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_hover.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_hover.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_pressed.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_pressed.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/images/zoomout_rest.png` & `openslide-python-1.3.0/examples/deepzoom/static/images/zoomout_rest.png`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/jquery.js` & `openslide-python-1.3.0/examples/deepzoom/static/jquery.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,30 @@
 /*!
- * jQuery JavaScript Library v3.6.0 -ajax,-ajax/jsonp,-ajax/load,-ajax/script,-ajax/var/location,-ajax/var/nonce,-ajax/var/rquery,-ajax/xhr,-manipulation/_evalUrl,-deprecated/ajax-event-alias,-effects,-effects/Tween,-effects/animatedSelector
+ * jQuery JavaScript Library v3.7.0 -ajax,-ajax/jsonp,-ajax/load,-ajax/script,-ajax/var/location,-ajax/var/nonce,-ajax/var/rquery,-ajax/xhr,-manipulation/_evalUrl,-deprecated/ajax-event-alias,-effects,-effects/animatedSelector,-effects/Tween
  * https://jquery.com/
  *
- * Includes Sizzle.js
- * https://sizzlejs.com/
- *
  * Copyright OpenJS Foundation and other contributors
  * Released under the MIT license
  * https://jquery.org/license
  *
- * Date: 2021-03-02T17:08Z
+ * Date: 2023-05-11T18:29Z
  */
 (function(global, factory) {
 
     "use strict";
 
     if (typeof module === "object" && typeof module.exports === "object") {
 
         // For CommonJS and CommonJS-like environments where a proper `window`
         // is present, execute the factory and get jQuery.
         // For environments that do not have a `window` with a `document`
         // (such as Node.js), expose a factory as module.exports.
         // This accentuates the need for the creation of a real `window`.
         // e.g. var jQuery = require("jquery")(window);
-        // See ticket #14549 for more info.
+        // See ticket trac-14549 for more info.
         module.exports = global.document ?
             factory(global, true) :
             function(w) {
                 if (!w.document) {
                     throw new Error("jQuery requires a window with a document");
                 }
                 return factory(w);
@@ -146,16 +143,17 @@
     }
     /* global Symbol */
     // Defining this global in .eslintrc.json would create a danger of using the global
     // unguarded in another place, it seems safer to define global only for this module
 
 
 
-    var
-        version = "3.6.0 -ajax,-ajax/jsonp,-ajax/load,-ajax/script,-ajax/var/location,-ajax/var/nonce,-ajax/var/rquery,-ajax/xhr,-manipulation/_evalUrl,-deprecated/ajax-event-alias,-effects,-effects/Tween,-effects/animatedSelector",
+    var version = "3.7.0 -ajax,-ajax/jsonp,-ajax/load,-ajax/script,-ajax/var/location,-ajax/var/nonce,-ajax/var/rquery,-ajax/xhr,-manipulation/_evalUrl,-deprecated/ajax-event-alias,-effects,-effects/animatedSelector,-effects/Tween",
+
+        rhtmlSuffix = /HTML$/i,
 
         // Define a local copy of jQuery
         jQuery = function(selector, context) {
 
             // The jQuery object is actually just the init constructor 'enhanced'
             // Need init if jQuery is called (just allow error to be thrown if not included)
             return new jQuery.fn.init(selector, context);
@@ -395,14 +393,41 @@
                     }
                 }
             }
 
             return obj;
         },
 
+
+        // Retrieve the text value of an array of DOM nodes
+        text: function(elem) {
+            var node,
+                ret = "",
+                i = 0,
+                nodeType = elem.nodeType;
+
+            if (!nodeType) {
+
+                // If no nodeType, this is expected to be an array
+                while ((node = elem[i++])) {
+
+                    // Do not traverse comment nodes
+                    ret += jQuery.text(node);
+                }
+            } else if (nodeType === 1 || nodeType === 9 || nodeType === 11) {
+                return elem.textContent;
+            } else if (nodeType === 3 || nodeType === 4) {
+                return elem.nodeValue;
+            }
+
+            // Do not include comment or processing instruction nodes
+
+            return ret;
+        },
+
         // results is for internal usage only
         makeArray: function(arr, results) {
             var ret = results || [];
 
             if (arr != null) {
                 if (isArrayLike(Object(arr))) {
                     jQuery.merge(ret,
@@ -416,14 +441,23 @@
             return ret;
         },
 
         inArray: function(elem, arr, i) {
             return arr == null ? -1 : indexOf.call(arr, elem, i);
         },
 
+        isXMLDoc: function(elem) {
+            var namespace = elem && elem.namespaceURI,
+                docElem = elem && (elem.ownerDocument || elem).documentElement;
+
+            // Assume HTML when documentElement doesn't yet exist, such as inside
+            // document fragments.
+            return !rhtmlSuffix.test(namespace || docElem && docElem.nodeName || "HTML");
+        },
+
         // Support: Android <=4.0 only, PhantomJS 1 only
         // push.apply(_, arraylike) throws on ancient WebKit
         merge: function(first, second) {
             var len = +second.length,
                 j = 0,
                 i = first.length;
 
@@ -517,2510 +551,2194 @@
         if (isFunction(obj) || isWindow(obj)) {
             return false;
         }
 
         return type === "array" || length === 0 ||
             typeof length === "number" && length > 0 && (length - 1) in obj;
     }
-    var Sizzle =
-        /*!
-         * Sizzle CSS Selector Engine v2.3.6
-         * https://sizzlejs.com/
-         *
-         * Copyright JS Foundation and other contributors
-         * Released under the MIT license
-         * https://js.foundation/
-         *
-         * Date: 2021-02-16
-         */
-        (function(window) {
-            var i,
-                support,
-                Expr,
-                getText,
-                isXML,
-                tokenize,
-                compile,
-                select,
-                outermostContext,
-                sortInput,
-                hasDuplicate,
-
-                // Local document vars
-                setDocument,
-                document,
-                docElem,
-                documentIsHTML,
-                rbuggyQSA,
-                rbuggyMatches,
-                matches,
-                contains,
-
-                // Instance-specific data
-                expando = "sizzle" + 1 * new Date(),
-                preferredDoc = window.document,
-                dirruns = 0,
-                done = 0,
-                classCache = createCache(),
-                tokenCache = createCache(),
-                compilerCache = createCache(),
-                nonnativeSelectorCache = createCache(),
-                sortOrder = function(a, b) {
-                    if (a === b) {
-                        hasDuplicate = true;
-                    }
-                    return 0;
-                },
 
-                // Instance methods
-                hasOwn = ({}).hasOwnProperty,
-                arr = [],
-                pop = arr.pop,
-                pushNative = arr.push,
-                push = arr.push,
-                slice = arr.slice,
-
-                // Use a stripped-down indexOf as it's faster than native
-                // https://jsperf.com/thor-indexof-vs-for/5
-                indexOf = function(list, elem) {
-                    var i = 0,
-                        len = list.length;
-                    for (; i < len; i++) {
-                        if (list[i] === elem) {
-                            return i;
-                        }
-                    }
-                    return -1;
-                },
-
-                booleans = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|" +
-                "ismap|loop|multiple|open|readonly|required|scoped",
 
-                // Regular expressions
+    function nodeName(elem, name) {
 
-                // http://www.w3.org/TR/css3-selectors/#whitespace
-                whitespace = "[\\x20\\t\\r\\n\\f]",
+        return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
 
-                // https://www.w3.org/TR/css-syntax-3/#ident-token-diagram
-                identifier = "(?:\\\\[\\da-fA-F]{1,6}" + whitespace +
-                "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
-
-                // Attribute selectors: http://www.w3.org/TR/selectors/#attribute-selectors
-                attributes = "\\[" + whitespace + "*(" + identifier + ")(?:" + whitespace +
-
-                // Operator (capture 2)
-                "*([*^$|!~]?=)" + whitespace +
-
-                // "Attribute values must be CSS identifiers [capture 5]
-                // or strings [capture 3 or capture 4]"
-                "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + identifier + "))|)" +
-                whitespace + "*\\]",
-
-                pseudos = ":(" + identifier + ")(?:\\((" +
-
-                // To reduce the number of selectors needing tokenize in the preFilter, prefer arguments:
-                // 1. quoted (capture 3; capture 4 or capture 5)
-                "('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|" +
-
-                // 2. simple (capture 6)
-                "((?:\\\\.|[^\\\\()[\\]]|" + attributes + ")*)|" +
-
-                // 3. anything else (capture 2)
-                ".*" +
-                ")\\)|)",
-
-                // Leading and non-escaped trailing whitespace, capturing some non-whitespace characters preceding the latter
-                rwhitespace = new RegExp(whitespace + "+", "g"),
-                rtrim = new RegExp("^" + whitespace + "+|((?:^|[^\\\\])(?:\\\\.)*)" +
-                    whitespace + "+$", "g"),
-
-                rcomma = new RegExp("^" + whitespace + "*," + whitespace + "*"),
-                rcombinators = new RegExp("^" + whitespace + "*([>+~]|" + whitespace + ")" + whitespace +
-                    "*"),
-                rdescend = new RegExp(whitespace + "|>"),
-
-                rpseudo = new RegExp(pseudos),
-                ridentifier = new RegExp("^" + identifier + "$"),
-
-                matchExpr = {
-                    "ID": new RegExp("^#(" + identifier + ")"),
-                    "CLASS": new RegExp("^\\.(" + identifier + ")"),
-                    "TAG": new RegExp("^(" + identifier + "|[*])"),
-                    "ATTR": new RegExp("^" + attributes),
-                    "PSEUDO": new RegExp("^" + pseudos),
-                    "CHILD": new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" +
-                        whitespace + "*(even|odd|(([+-]|)(\\d*)n|)" + whitespace + "*(?:([+-]|)" +
-                        whitespace + "*(\\d+)|))" + whitespace + "*\\)|)", "i"),
-                    "bool": new RegExp("^(?:" + booleans + ")$", "i"),
-
-                    // For use in libraries implementing .is()
-                    // We use this for POS matching in `select`
-                    "needsContext": new RegExp("^" + whitespace +
-                        "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + whitespace +
-                        "*((?:-\\d)?\\d*)" + whitespace + "*\\)|)(?=[^-]|$)", "i")
-                },
+    }
+    var pop = arr.pop;
 
-                rhtml = /HTML$/i,
-                rinputs = /^(?:input|select|textarea|button)$/i,
-                rheader = /^h\d$/i,
-
-                rnative = /^[^{]+\{\s*\[native \w/,
-
-                // Easily-parseable/retrievable ID or TAG or CLASS selectors
-                rquickExpr = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-
-                rsibling = /[+~]/,
-
-                // CSS escapes
-                // http://www.w3.org/TR/CSS21/syndata.html#escaped-characters
-                runescape = new RegExp("\\\\[\\da-fA-F]{1,6}" + whitespace + "?|\\\\([^\\r\\n\\f])", "g"),
-                funescape = function(escape, nonHex) {
-                    var high = "0x" + escape.slice(1) - 0x10000;
-
-                    return nonHex ?
-
-                        // Strip the backslash prefix from a non-hex escape sequence
-                        nonHex :
-
-                        // Replace a hexadecimal escape sequence with the encoded Unicode code point
-                        // Support: IE <=11+
-                        // For values outside the Basic Multilingual Plane (BMP), manually construct a
-                        // surrogate pair
-                        high < 0 ?
-                        String.fromCharCode(high + 0x10000) :
-                        String.fromCharCode(high >> 10 | 0xD800, high & 0x3FF | 0xDC00);
-                },
 
-                // CSS string/identifier serialization
-                // https://drafts.csswg.org/cssom/#common-serializing-idioms
-                rcssescape = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
-                fcssescape = function(ch, asCodePoint) {
-                    if (asCodePoint) {
+    var sort = arr.sort;
 
-                        // U+0000 NULL becomes U+FFFD REPLACEMENT CHARACTER
-                        if (ch === "\0") {
-                            return "\uFFFD";
-                        }
 
-                        // Control characters and (dependent upon position) numbers get escaped as code points
-                        return ch.slice(0, -1) + "\\" +
-                            ch.charCodeAt(ch.length - 1).toString(16) + " ";
-                    }
+    var splice = arr.splice;
 
-                    // Other potentially-special ASCII characters get backslash-escaped
-                    return "\\" + ch;
-                },
 
-                // Used for iframes
-                // See setDocument()
-                // Removing the function wrapper causes a "Permission Denied"
-                // error in IE
-                unloadHandler = function() {
-                    setDocument();
-                },
+    var whitespace = "[\\x20\\t\\r\\n\\f]";
 
-                inDisabledFieldset = addCombinator(
-                    function(elem) {
-                        return elem.disabled === true && elem.nodeName.toLowerCase() === "fieldset";
-                    }, {
-                        dir: "parentNode",
-                        next: "legend"
-                    }
-                );
 
-            // Optimize for push.apply( _, NodeList )
-            try {
-                push.apply(
-                    (arr = slice.call(preferredDoc.childNodes)),
-                    preferredDoc.childNodes
-                );
+    var rtrimCSS = new RegExp(
+        "^" + whitespace + "+|((?:^|[^\\\\])(?:\\\\.)*)" + whitespace + "+$",
+        "g"
+    );
 
-                // Support: Android<4.0
-                // Detect silently failing push.apply
-                // eslint-disable-next-line no-unused-expressions
-                arr[preferredDoc.childNodes.length].nodeType;
-            } catch (e) {
-                push = {
-                    apply: arr.length ?
 
-                        // Leverage slice if possible
-                        function(target, els) {
-                            pushNative.apply(target, slice.call(els));
-                        } :
 
-                        // Support: IE<9
-                        // Otherwise append directly
-                        function(target, els) {
-                            var j = target.length,
-                                i = 0;
-
-                            // Can't trust NodeList.length
-                            while ((target[j++] = els[i++])) {}
-                            target.length = j - 1;
-                        }
-                };
-            }
 
-            function Sizzle(selector, context, results, seed) {
-                var m, i, elem, nid, match, groups, newSelector,
-                    newContext = context && context.ownerDocument,
+    // Note: an element does not contain itself
+    jQuery.contains = function(a, b) {
+        var bup = b && b.parentNode;
+
+        return a === bup || !!(bup && bup.nodeType === 1 && (
+
+            // Support: IE 9 - 11+
+            // IE doesn't have `contains` on SVG.
+            a.contains ?
+            a.contains(bup) :
+            a.compareDocumentPosition && a.compareDocumentPosition(bup) & 16
+        ));
+    };
 
-                    // nodeType defaults to 9, since context defaults to document
-                    nodeType = context ? context.nodeType : 9;
 
-                results = results || [];
 
-                // Return early from calls with invalid selector or context
-                if (typeof selector !== "string" || !selector ||
-                    nodeType !== 1 && nodeType !== 9 && nodeType !== 11) {
 
-                    return results;
-                }
+    // CSS string/identifier serialization
+    // https://drafts.csswg.org/cssom/#common-serializing-idioms
+    var rcssescape = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\x80-\uFFFF\w-]/g;
 
-                // Try to shortcut find operations (as opposed to filters) in HTML documents
-                if (!seed) {
-                    setDocument(context);
-                    context = context || document;
+    function fcssescape(ch, asCodePoint) {
+        if (asCodePoint) {
 
-                    if (documentIsHTML) {
+            // U+0000 NULL becomes U+FFFD REPLACEMENT CHARACTER
+            if (ch === "\0") {
+                return "\uFFFD";
+            }
 
-                        // If the selector is sufficiently simple, try using a "get*By*" DOM method
-                        // (excepting DocumentFragment context, where the methods don't exist)
-                        if (nodeType !== 11 && (match = rquickExpr.exec(selector))) {
+            // Control characters and (dependent upon position) numbers get escaped as code points
+            return ch.slice(0, -1) + "\\" + ch.charCodeAt(ch.length - 1).toString(16) + " ";
+        }
 
-                            // ID selector
-                            if ((m = match[1])) {
+        // Other potentially-special ASCII characters get backslash-escaped
+        return "\\" + ch;
+    }
 
-                                // Document context
-                                if (nodeType === 9) {
-                                    if ((elem = context.getElementById(m))) {
+    jQuery.escapeSelector = function(sel) {
+        return (sel + "").replace(rcssescape, fcssescape);
+    };
 
-                                        // Support: IE, Opera, Webkit
-                                        // TODO: identify versions
-                                        // getElementById can match elements by name instead of ID
-                                        if (elem.id === m) {
-                                            results.push(elem);
-                                            return results;
-                                        }
-                                    } else {
-                                        return results;
-                                    }
 
-                                    // Element context
-                                } else {
 
-                                    // Support: IE, Opera, Webkit
-                                    // TODO: identify versions
-                                    // getElementById can match elements by name instead of ID
-                                    if (newContext && (elem = newContext.getElementById(m)) &&
-                                        contains(context, elem) &&
-                                        elem.id === m) {
 
-                                        results.push(elem);
-                                        return results;
-                                    }
-                                }
+    var preferredDoc = document,
+        pushNative = push;
 
-                                // Type selector
-                            } else if (match[2]) {
-                                push.apply(results, context.getElementsByTagName(selector));
-                                return results;
+    (function() {
 
-                                // Class selector
-                            } else if ((m = match[3]) && support.getElementsByClassName &&
-                                context.getElementsByClassName) {
+        var i,
+            Expr,
+            outermostContext,
+            sortInput,
+            hasDuplicate,
+            push = pushNative,
+
+            // Local document vars
+            document,
+            documentElement,
+            documentIsHTML,
+            rbuggyQSA,
+            matches,
+
+            // Instance-specific data
+            expando = jQuery.expando,
+            dirruns = 0,
+            done = 0,
+            classCache = createCache(),
+            tokenCache = createCache(),
+            compilerCache = createCache(),
+            nonnativeSelectorCache = createCache(),
+            sortOrder = function(a, b) {
+                if (a === b) {
+                    hasDuplicate = true;
+                }
+                return 0;
+            },
 
-                                push.apply(results, context.getElementsByClassName(m));
-                                return results;
-                            }
-                        }
+            booleans = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|" +
+            "loop|multiple|open|readonly|required|scoped",
 
-                        // Take advantage of querySelectorAll
-                        if (support.qsa &&
-                            !nonnativeSelectorCache[selector + " "] &&
-                            (!rbuggyQSA || !rbuggyQSA.test(selector)) &&
-
-                            // Support: IE 8 only
-                            // Exclude object elements
-                            (nodeType !== 1 || context.nodeName.toLowerCase() !== "object")) {
-
-                            newSelector = selector;
-                            newContext = context;
-
-                            // qSA considers elements outside a scoping root when evaluating child or
-                            // descendant combinators, which is not what we want.
-                            // In such cases, we work around the behavior by prefixing every selector in the
-                            // list with an ID selector referencing the scope context.
-                            // The technique has to be used as well when a leading combinator is used
-                            // as such selectors are not recognized by querySelectorAll.
-                            // Thanks to Andrew Dupont for this technique.
-                            if (nodeType === 1 &&
-                                (rdescend.test(selector) || rcombinators.test(selector))) {
-
-                                // Expand context for sibling selectors
-                                newContext = rsibling.test(selector) && testContext(context.parentNode) ||
-                                    context;
-
-                                // We can use :scope instead of the ID hack if the browser
-                                // supports it & if we're not changing the context.
-                                if (newContext !== context || !support.scope) {
-
-                                    // Capture the context ID, setting it first if necessary
-                                    if ((nid = context.getAttribute("id"))) {
-                                        nid = nid.replace(rcssescape, fcssescape);
-                                    } else {
-                                        context.setAttribute("id", (nid = expando));
-                                    }
-                                }
+            // Regular expressions
 
-                                // Prefix every selector in the list
-                                groups = tokenize(selector);
-                                i = groups.length;
-                                while (i--) {
-                                    groups[i] = (nid ? "#" + nid : ":scope") + " " +
-                                        toSelector(groups[i]);
-                                }
-                                newSelector = groups.join(",");
-                            }
+            // https://www.w3.org/TR/css-syntax-3/#ident-token-diagram
+            identifier = "(?:\\\\[\\da-fA-F]{1,6}" + whitespace +
+            "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
+
+            // Attribute selectors: https://www.w3.org/TR/selectors/#attribute-selectors
+            attributes = "\\[" + whitespace + "*(" + identifier + ")(?:" + whitespace +
+
+            // Operator (capture 2)
+            "*([*^$|!~]?=)" + whitespace +
+
+            // "Attribute values must be CSS identifiers [capture 5] or strings [capture 3 or capture 4]"
+            "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + identifier + "))|)" +
+            whitespace + "*\\]",
+
+            pseudos = ":(" + identifier + ")(?:\\((" +
+
+            // To reduce the number of selectors needing tokenize in the preFilter, prefer arguments:
+            // 1. quoted (capture 3; capture 4 or capture 5)
+            "('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|" +
+
+            // 2. simple (capture 6)
+            "((?:\\\\.|[^\\\\()[\\]]|" + attributes + ")*)|" +
+
+            // 3. anything else (capture 2)
+            ".*" +
+            ")\\)|)",
+
+            // Leading and non-escaped trailing whitespace, capturing some non-whitespace characters preceding the latter
+            rwhitespace = new RegExp(whitespace + "+", "g"),
+
+            rcomma = new RegExp("^" + whitespace + "*," + whitespace + "*"),
+            rleadingCombinator = new RegExp("^" + whitespace + "*([>+~]|" + whitespace + ")" +
+                whitespace + "*"),
+            rdescend = new RegExp(whitespace + "|>"),
+
+            rpseudo = new RegExp(pseudos),
+            ridentifier = new RegExp("^" + identifier + "$"),
+
+            matchExpr = {
+                ID: new RegExp("^#(" + identifier + ")"),
+                CLASS: new RegExp("^\\.(" + identifier + ")"),
+                TAG: new RegExp("^(" + identifier + "|[*])"),
+                ATTR: new RegExp("^" + attributes),
+                PSEUDO: new RegExp("^" + pseudos),
+                CHILD: new RegExp(
+                    "^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" +
+                    whitespace + "*(even|odd|(([+-]|)(\\d*)n|)" + whitespace + "*(?:([+-]|)" +
+                    whitespace + "*(\\d+)|))" + whitespace + "*\\)|)", "i"),
+                bool: new RegExp("^(?:" + booleans + ")$", "i"),
+
+                // For use in libraries implementing .is()
+                // We use this for POS matching in `select`
+                needsContext: new RegExp("^" + whitespace +
+                    "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + whitespace +
+                    "*((?:-\\d)?\\d*)" + whitespace + "*\\)|)(?=[^-]|$)", "i")
+            },
 
-                            try {
-                                push.apply(results,
-                                    newContext.querySelectorAll(newSelector)
-                                );
-                                return results;
-                            } catch (qsaError) {
-                                nonnativeSelectorCache(selector, true);
-                            } finally {
-                                if (nid === expando) {
-                                    context.removeAttribute("id");
-                                }
-                            }
-                        }
-                    }
-                }
+            rinputs = /^(?:input|select|textarea|button)$/i,
+            rheader = /^h\d$/i,
 
-                // All others
-                return select(selector.replace(rtrim, "$1"), context, results, seed);
-            }
+            // Easily-parseable/retrievable ID or TAG or CLASS selectors
+            rquickExpr = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
 
-            /**
-             * Create key-value caches of limited size
-             * @returns {function(string, object)} Returns the Object data after storing it on itself with
-             *	property name the (space-suffixed) string and (if the cache is larger than Expr.cacheLength)
-             *	deleting the oldest entry
-             */
-            function createCache() {
-                var keys = [];
+            rsibling = /[+~]/,
 
-                function cache(key, value) {
+            // CSS escapes
+            // https://www.w3.org/TR/CSS21/syndata.html#escaped-characters
+            runescape = new RegExp("\\\\[\\da-fA-F]{1,6}" + whitespace +
+                "?|\\\\([^\\r\\n\\f])", "g"),
+            funescape = function(escape, nonHex) {
+                var high = "0x" + escape.slice(1) - 0x10000;
+
+                if (nonHex) {
+
+                    // Strip the backslash prefix from a non-hex escape sequence
+                    return nonHex;
+                }
+
+                // Replace a hexadecimal escape sequence with the encoded Unicode code point
+                // Support: IE <=11+
+                // For values outside the Basic Multilingual Plane (BMP), manually construct a
+                // surrogate pair
+                return high < 0 ?
+                    String.fromCharCode(high + 0x10000) :
+                    String.fromCharCode(high >> 10 | 0xD800, high & 0x3FF | 0xDC00);
+            },
 
-                    // Use (key + " ") to avoid collision with native prototype properties (see Issue #157)
-                    if (keys.push(key + " ") > Expr.cacheLength) {
+            // Used for iframes; see `setDocument`.
+            // Support: IE 9 - 11+, Edge 12 - 18+
+            // Removing the function wrapper causes a "Permission Denied"
+            // error in IE/Edge.
+            unloadHandler = function() {
+                setDocument();
+            },
 
-                        // Only keep the most recent entries
-                        delete cache[keys.shift()];
-                    }
-                    return (cache[key + " "] = value);
+            inDisabledFieldset = addCombinator(
+                function(elem) {
+                    return elem.disabled === true && nodeName(elem, "fieldset");
+                }, {
+                    dir: "parentNode",
+                    next: "legend"
                 }
-                return cache;
-            }
+            );
 
-            /**
-             * Mark a function for special use by Sizzle
-             * @param {Function} fn The function to mark
-             */
-            function markFunction(fn) {
-                fn[expando] = true;
-                return fn;
-            }
+        // Support: IE <=9 only
+        // Accessing document.activeElement can throw unexpectedly
+        // https://bugs.jquery.com/ticket/13393
+        function safeActiveElement() {
+            try {
+                return document.activeElement;
+            } catch (err) {}
+        }
 
-            /**
-             * Support testing using an element
-             * @param {Function} fn Passed the created element and returns a boolean result
-             */
-            function assert(fn) {
-                var el = document.createElement("fieldset");
+        // Optimize for push.apply( _, NodeList )
+        try {
+            push.apply(
+                (arr = slice.call(preferredDoc.childNodes)),
+                preferredDoc.childNodes
+            );
 
-                try {
-                    return !!fn(el);
-                } catch (e) {
-                    return false;
-                } finally {
+            // Support: Android <=4.0
+            // Detect silently failing push.apply
+            // eslint-disable-next-line no-unused-expressions
+            arr[preferredDoc.childNodes.length].nodeType;
+        } catch (e) {
+            push = {
+                apply: function(target, els) {
+                    pushNative.apply(target, slice.call(els));
+                },
+                call: function(target) {
+                    pushNative.apply(target, slice.call(arguments, 1));
+                }
+            };
+        }
 
-                    // Remove from its parent by default
-                    if (el.parentNode) {
-                        el.parentNode.removeChild(el);
-                    }
+        function find(selector, context, results, seed) {
+            var m, i, elem, nid, match, groups, newSelector,
+                newContext = context && context.ownerDocument,
+
+                // nodeType defaults to 9, since context defaults to document
+                nodeType = context ? context.nodeType : 9;
+
+            results = results || [];
+
+            // Return early from calls with invalid selector or context
+            if (typeof selector !== "string" || !selector ||
+                nodeType !== 1 && nodeType !== 9 && nodeType !== 11) {
 
-                    // release memory in IE
-                    el = null;
-                }
+                return results;
             }
 
-            /**
-             * Adds the same handler for all of the specified attrs
-             * @param {String} attrs Pipe-separated list of attributes
-             * @param {Function} handler The method that will be applied
-             */
-            function addHandle(attrs, handler) {
-                var arr = attrs.split("|"),
-                    i = arr.length;
+            // Try to shortcut find operations (as opposed to filters) in HTML documents
+            if (!seed) {
+                setDocument(context);
+                context = context || document;
 
-                while (i--) {
-                    Expr.attrHandle[arr[i]] = handler;
-                }
-            }
+                if (documentIsHTML) {
 
-            /**
-             * Checks document order of two siblings
-             * @param {Element} a
-             * @param {Element} b
-             * @returns {Number} Returns less than 0 if a precedes b, greater than 0 if a follows b
-             */
-            function siblingCheck(a, b) {
-                var cur = b && a,
-                    diff = cur && a.nodeType === 1 && b.nodeType === 1 &&
-                    a.sourceIndex - b.sourceIndex;
+                    // If the selector is sufficiently simple, try using a "get*By*" DOM method
+                    // (excepting DocumentFragment context, where the methods don't exist)
+                    if (nodeType !== 11 && (match = rquickExpr.exec(selector))) {
 
-                // Use IE sourceIndex if available on both nodes
-                if (diff) {
-                    return diff;
-                }
+                        // ID selector
+                        if ((m = match[1])) {
 
-                // Check if b follows a
-                if (cur) {
-                    while ((cur = cur.nextSibling)) {
-                        if (cur === b) {
-                            return -1;
-                        }
-                    }
-                }
+                            // Document context
+                            if (nodeType === 9) {
+                                if ((elem = context.getElementById(m))) {
 
-                return a ? 1 : -1;
-            }
+                                    // Support: IE 9 only
+                                    // getElementById can match elements by name instead of ID
+                                    if (elem.id === m) {
+                                        push.call(results, elem);
+                                        return results;
+                                    }
+                                } else {
+                                    return results;
+                                }
 
-            /**
-             * Returns a function to use in pseudos for input types
-             * @param {String} type
-             */
-            function createInputPseudo(type) {
-                return function(elem) {
-                    var name = elem.nodeName.toLowerCase();
-                    return name === "input" && elem.type === type;
-                };
-            }
+                                // Element context
+                            } else {
 
-            /**
-             * Returns a function to use in pseudos for buttons
-             * @param {String} type
-             */
-            function createButtonPseudo(type) {
-                return function(elem) {
-                    var name = elem.nodeName.toLowerCase();
-                    return (name === "input" || name === "button") && elem.type === type;
-                };
-            }
+                                // Support: IE 9 only
+                                // getElementById can match elements by name instead of ID
+                                if (newContext && (elem = newContext.getElementById(m)) &&
+                                    find.contains(context, elem) &&
+                                    elem.id === m) {
 
-            /**
-             * Returns a function to use in pseudos for :enabled/:disabled
-             * @param {Boolean} disabled true for :disabled; false for :enabled
-             */
-            function createDisabledPseudo(disabled) {
-
-                // Known :disabled false positives: fieldset[disabled] > legend:nth-of-type(n+2) :can-disable
-                return function(elem) {
-
-                    // Only certain elements can match :enabled or :disabled
-                    // https://html.spec.whatwg.org/multipage/scripting.html#selector-enabled
-                    // https://html.spec.whatwg.org/multipage/scripting.html#selector-disabled
-                    if ("form" in elem) {
-
-                        // Check for inherited disabledness on relevant non-disabled elements:
-                        // * listed form-associated elements in a disabled fieldset
-                        //   https://html.spec.whatwg.org/multipage/forms.html#category-listed
-                        //   https://html.spec.whatwg.org/multipage/forms.html#concept-fe-disabled
-                        // * option elements in a disabled optgroup
-                        //   https://html.spec.whatwg.org/multipage/forms.html#concept-option-disabled
-                        // All such elements have a "form" property.
-                        if (elem.parentNode && elem.disabled === false) {
-
-                            // Option elements defer to a parent optgroup if present
-                            if ("label" in elem) {
-                                if ("label" in elem.parentNode) {
-                                    return elem.parentNode.disabled === disabled;
-                                } else {
-                                    return elem.disabled === disabled;
+                                    push.call(results, elem);
+                                    return results;
                                 }
                             }
 
-                            // Support: IE 6 - 11
-                            // Use the isDisabled shortcut property to check for disabled fieldset ancestors
-                            return elem.isDisabled === disabled ||
+                            // Type selector
+                        } else if (match[2]) {
+                            push.apply(results, context.getElementsByTagName(selector));
+                            return results;
 
-                                // Where there is no isDisabled, check manually
-                                /* jshint -W018 */
-                                elem.isDisabled !== !disabled &&
-                                inDisabledFieldset(elem) === disabled;
+                            // Class selector
+                        } else if ((m = match[3]) && context.getElementsByClassName) {
+                            push.apply(results, context.getElementsByClassName(m));
+                            return results;
                         }
+                    }
 
-                        return elem.disabled === disabled;
+                    // Take advantage of querySelectorAll
+                    if (!nonnativeSelectorCache[selector + " "] &&
+                        (!rbuggyQSA || !rbuggyQSA.test(selector))) {
+
+                        newSelector = selector;
+                        newContext = context;
+
+                        // qSA considers elements outside a scoping root when evaluating child or
+                        // descendant combinators, which is not what we want.
+                        // In such cases, we work around the behavior by prefixing every selector in the
+                        // list with an ID selector referencing the scope context.
+                        // The technique has to be used as well when a leading combinator is used
+                        // as such selectors are not recognized by querySelectorAll.
+                        // Thanks to Andrew Dupont for this technique.
+                        if (nodeType === 1 &&
+                            (rdescend.test(selector) || rleadingCombinator.test(selector))) {
+
+                            // Expand context for sibling selectors
+                            newContext = rsibling.test(selector) && testContext(context.parentNode) ||
+                                context;
 
-                        // Try to winnow out elements that can't be disabled before trusting the disabled property.
-                        // Some victims get caught in our net (label, legend, menu, track), but it shouldn't
-                        // even exist on them, let alone have a boolean value.
-                    } else if ("label" in elem) {
-                        return elem.disabled === disabled;
-                    }
+                            // We can use :scope instead of the ID hack if the browser
+                            // supports it & if we're not changing the context.
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when
+                            // strict-comparing two documents; shallow comparisons work.
+                            // eslint-disable-next-line eqeqeq
+                            if (newContext != context || !support.scope) {
 
-                    // Remaining elements are neither :enabled nor :disabled
-                    return false;
-                };
-            }
+                                // Capture the context ID, setting it first if necessary
+                                if ((nid = context.getAttribute("id"))) {
+                                    nid = jQuery.escapeSelector(nid);
+                                } else {
+                                    context.setAttribute("id", (nid = expando));
+                                }
+                            }
 
-            /**
-             * Returns a function to use in pseudos for positionals
-             * @param {Function} fn
-             */
-            function createPositionalPseudo(fn) {
-                return markFunction(function(argument) {
-                    argument = +argument;
-                    return markFunction(function(seed, matches) {
-                        var j,
-                            matchIndexes = fn([], seed.length, argument),
-                            i = matchIndexes.length;
+                            // Prefix every selector in the list
+                            groups = tokenize(selector);
+                            i = groups.length;
+                            while (i--) {
+                                groups[i] = (nid ? "#" + nid : ":scope") + " " +
+                                    toSelector(groups[i]);
+                            }
+                            newSelector = groups.join(",");
+                        }
 
-                        // Match elements found at the specified indexes
-                        while (i--) {
-                            if (seed[(j = matchIndexes[i])]) {
-                                seed[j] = !(matches[j] = seed[j]);
+                        try {
+                            push.apply(results,
+                                newContext.querySelectorAll(newSelector)
+                            );
+                            return results;
+                        } catch (qsaError) {
+                            nonnativeSelectorCache(selector, true);
+                        } finally {
+                            if (nid === expando) {
+                                context.removeAttribute("id");
                             }
                         }
-                    });
-                });
+                    }
+                }
             }
 
-            /**
-             * Checks a node for validity as a Sizzle context
-             * @param {Element|Object=} context
-             * @returns {Element|Object|Boolean} The input node if acceptable, otherwise a falsy value
-             */
-            function testContext(context) {
-                return context && typeof context.getElementsByTagName !== "undefined" && context;
-            }
-
-            // Expose support vars for convenience
-            support = Sizzle.support = {};
-
-            /**
-             * Detects XML nodes
-             * @param {Element|Object} elem An element or a document
-             * @returns {Boolean} True iff elem is a non-HTML XML node
-             */
-            isXML = Sizzle.isXML = function(elem) {
-                var namespace = elem && elem.namespaceURI,
-                    docElem = elem && (elem.ownerDocument || elem).documentElement;
-
-                // Support: IE <=8
-                // Assume HTML when documentElement doesn't yet exist, such as inside loading iframes
-                // https://bugs.jquery.com/ticket/4833
-                return !rhtml.test(namespace || docElem && docElem.nodeName || "HTML");
-            };
-
-            /**
-             * Sets document-related variables once based on the current document
-             * @param {Element|Object} [doc] An element or document object to use to set the document
-             * @returns {Object} Returns the current document
-             */
-            setDocument = Sizzle.setDocument = function(node) {
-                var hasCompare, subWindow,
-                    doc = node ? node.ownerDocument || node : preferredDoc;
+            // All others
+            return select(selector.replace(rtrimCSS, "$1"), context, results, seed);
+        }
 
-                // Return early if doc is invalid or already selected
-                // Support: IE 11+, Edge 17 - 18+
-                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                // two documents; shallow comparisons work.
-                // eslint-disable-next-line eqeqeq
-                if (doc == document || doc.nodeType !== 9 || !doc.documentElement) {
-                    return document;
-                }
+        /**
+         * Create key-value caches of limited size
+         * @returns {function(string, object)} Returns the Object data after storing it on itself with
+         *	property name the (space-suffixed) string and (if the cache is larger than Expr.cacheLength)
+         *	deleting the oldest entry
+         */
+        function createCache() {
+            var keys = [];
 
-                // Update global variables
-                document = doc;
-                docElem = document.documentElement;
-                documentIsHTML = !isXML(document);
+            function cache(key, value) {
 
-                // Support: IE 9 - 11+, Edge 12 - 18+
-                // Accessing iframe documents after unload throws "permission denied" errors (jQuery #13936)
-                // Support: IE 11+, Edge 17 - 18+
-                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                // two documents; shallow comparisons work.
-                // eslint-disable-next-line eqeqeq
-                if (preferredDoc != document &&
-                    (subWindow = document.defaultView) && subWindow.top !== subWindow) {
+                // Use (key + " ") to avoid collision with native prototype properties
+                // (see https://github.com/jquery/sizzle/issues/157)
+                if (keys.push(key + " ") > Expr.cacheLength) {
 
-                    // Support: IE 11, Edge
-                    if (subWindow.addEventListener) {
-                        subWindow.addEventListener("unload", unloadHandler, false);
-
-                        // Support: IE 9 - 10 only
-                    } else if (subWindow.attachEvent) {
-                        subWindow.attachEvent("onunload", unloadHandler);
-                    }
+                    // Only keep the most recent entries
+                    delete cache[keys.shift()];
                 }
+                return (cache[key + " "] = value);
+            }
+            return cache;
+        }
 
-                // Support: IE 8 - 11+, Edge 12 - 18+, Chrome <=16 - 25 only, Firefox <=3.6 - 31 only,
-                // Safari 4 - 5 only, Opera <=11.6 - 12.x only
-                // IE/Edge & older browsers don't support the :scope pseudo-class.
-                // Support: Safari 6.0 only
-                // Safari 6.0 supports :scope but it's an alias of :root there.
-                support.scope = assert(function(el) {
-                    docElem.appendChild(el).appendChild(document.createElement("div"));
-                    return typeof el.querySelectorAll !== "undefined" &&
-                        !el.querySelectorAll(":scope fieldset div").length;
-                });
-
-                /* Attributes
-                ---------------------------------------------------------------------- */
-
-                // Support: IE<8
-                // Verify that getAttribute really returns attributes and not properties
-                // (excepting IE8 booleans)
-                support.attributes = assert(function(el) {
-                    el.className = "i";
-                    return !el.getAttribute("className");
-                });
+        /**
+         * Mark a function for special use by jQuery selector module
+         * @param {Function} fn The function to mark
+         */
+        function markFunction(fn) {
+            fn[expando] = true;
+            return fn;
+        }
 
-                /* getElement(s)By*
-                ---------------------------------------------------------------------- */
+        /**
+         * Support testing using an element
+         * @param {Function} fn Passed the created element and returns a boolean result
+         */
+        function assert(fn) {
+            var el = document.createElement("fieldset");
 
-                // Check if getElementsByTagName("*") returns only elements
-                support.getElementsByTagName = assert(function(el) {
-                    el.appendChild(document.createComment(""));
-                    return !el.getElementsByTagName("*").length;
-                });
+            try {
+                return !!fn(el);
+            } catch (e) {
+                return false;
+            } finally {
 
-                // Support: IE<9
-                support.getElementsByClassName = rnative.test(document.getElementsByClassName);
+                // Remove from its parent by default
+                if (el.parentNode) {
+                    el.parentNode.removeChild(el);
+                }
 
-                // Support: IE<10
-                // Check if getElementById returns elements by name
-                // The broken getElementById methods don't pick up programmatically-set names,
-                // so use a roundabout getElementsByName test
-                support.getById = assert(function(el) {
-                    docElem.appendChild(el).id = expando;
-                    return !document.getElementsByName || !document.getElementsByName(expando).length;
-                });
+                // release memory in IE
+                el = null;
+            }
+        }
 
-                // ID filter and find
-                if (support.getById) {
-                    Expr.filter["ID"] = function(id) {
-                        var attrId = id.replace(runescape, funescape);
-                        return function(elem) {
-                            return elem.getAttribute("id") === attrId;
-                        };
-                    };
-                    Expr.find["ID"] = function(id, context) {
-                        if (typeof context.getElementById !== "undefined" && documentIsHTML) {
-                            var elem = context.getElementById(id);
-                            return elem ? [elem] : [];
-                        }
-                    };
-                } else {
-                    Expr.filter["ID"] = function(id) {
-                        var attrId = id.replace(runescape, funescape);
-                        return function(elem) {
-                            var node = typeof elem.getAttributeNode !== "undefined" &&
-                                elem.getAttributeNode("id");
-                            return node && node.value === attrId;
-                        };
-                    };
+        /**
+         * Returns a function to use in pseudos for input types
+         * @param {String} type
+         */
+        function createInputPseudo(type) {
+            return function(elem) {
+                return nodeName(elem, "input") && elem.type === type;
+            };
+        }
 
-                    // Support: IE 6 - 7 only
-                    // getElementById is not reliable as a find shortcut
-                    Expr.find["ID"] = function(id, context) {
-                        if (typeof context.getElementById !== "undefined" && documentIsHTML) {
-                            var node, i, elems,
-                                elem = context.getElementById(id);
+        /**
+         * Returns a function to use in pseudos for buttons
+         * @param {String} type
+         */
+        function createButtonPseudo(type) {
+            return function(elem) {
+                return (nodeName(elem, "input") || nodeName(elem, "button")) &&
+                    elem.type === type;
+            };
+        }
 
-                            if (elem) {
+        /**
+         * Returns a function to use in pseudos for :enabled/:disabled
+         * @param {Boolean} disabled true for :disabled; false for :enabled
+         */
+        function createDisabledPseudo(disabled) {
 
-                                // Verify the id attribute
-                                node = elem.getAttributeNode("id");
-                                if (node && node.value === id) {
-                                    return [elem];
-                                }
+            // Known :disabled false positives: fieldset[disabled] > legend:nth-of-type(n+2) :can-disable
+            return function(elem) {
 
-                                // Fall back on getElementsByName
-                                elems = context.getElementsByName(id);
-                                i = 0;
-                                while ((elem = elems[i++])) {
-                                    node = elem.getAttributeNode("id");
-                                    if (node && node.value === id) {
-                                        return [elem];
-                                    }
-                                }
+                // Only certain elements can match :enabled or :disabled
+                // https://html.spec.whatwg.org/multipage/scripting.html#selector-enabled
+                // https://html.spec.whatwg.org/multipage/scripting.html#selector-disabled
+                if ("form" in elem) {
+
+                    // Check for inherited disabledness on relevant non-disabled elements:
+                    // * listed form-associated elements in a disabled fieldset
+                    //   https://html.spec.whatwg.org/multipage/forms.html#category-listed
+                    //   https://html.spec.whatwg.org/multipage/forms.html#concept-fe-disabled
+                    // * option elements in a disabled optgroup
+                    //   https://html.spec.whatwg.org/multipage/forms.html#concept-option-disabled
+                    // All such elements have a "form" property.
+                    if (elem.parentNode && elem.disabled === false) {
+
+                        // Option elements defer to a parent optgroup if present
+                        if ("label" in elem) {
+                            if ("label" in elem.parentNode) {
+                                return elem.parentNode.disabled === disabled;
+                            } else {
+                                return elem.disabled === disabled;
                             }
-
-                            return [];
                         }
-                    };
-                }
-
-                // Tag
-                Expr.find["TAG"] = support.getElementsByTagName ?
-                    function(tag, context) {
-                        if (typeof context.getElementsByTagName !== "undefined") {
-                            return context.getElementsByTagName(tag);
-
-                            // DocumentFragment nodes don't have gEBTN
-                        } else if (support.qsa) {
-                            return context.querySelectorAll(tag);
-                        }
-                    } :
-
-                    function(tag, context) {
-                        var elem,
-                            tmp = [],
-                            i = 0,
-
-                            // By happy coincidence, a (broken) gEBTN appears on DocumentFragment nodes too
-                            results = context.getElementsByTagName(tag);
-
-                        // Filter out possible comments
-                        if (tag === "*") {
-                            while ((elem = results[i++])) {
-                                if (elem.nodeType === 1) {
-                                    tmp.push(elem);
-                                }
-                            }
 
-                            return tmp;
-                        }
-                        return results;
-                    };
+                        // Support: IE 6 - 11+
+                        // Use the isDisabled shortcut property to check for disabled fieldset ancestors
+                        return elem.isDisabled === disabled ||
 
-                // Class
-                Expr.find["CLASS"] = support.getElementsByClassName && function(className, context) {
-                    if (typeof context.getElementsByClassName !== "undefined" && documentIsHTML) {
-                        return context.getElementsByClassName(className);
+                            // Where there is no isDisabled, check manually
+                            elem.isDisabled !== !disabled &&
+                            inDisabledFieldset(elem) === disabled;
                     }
-                };
-
-                /* QSA/matchesSelector
-                ---------------------------------------------------------------------- */
-
-                // QSA and matchesSelector support
 
-                // matchesSelector(:active) reports false when true (IE9/Opera 11.5)
-                rbuggyMatches = [];
+                    return elem.disabled === disabled;
 
-                // qSa(:focus) reports false when true (Chrome 21)
-                // We allow this because of a bug in IE8/9 that throws an error
-                // whenever `document.activeElement` is accessed on an iframe
-                // So, we allow :focus to pass through QSA all the time to avoid the IE error
-                // See https://bugs.jquery.com/ticket/13378
-                rbuggyQSA = [];
-
-                if ((support.qsa = rnative.test(document.querySelectorAll))) {
-
-                    // Build QSA regex
-                    // Regex strategy adopted from Diego Perini
-                    assert(function(el) {
-
-                        var input;
-
-                        // Select is set to empty string on purpose
-                        // This is to test IE's treatment of not explicitly
-                        // setting a boolean content attribute,
-                        // since its presence should be enough
-                        // https://bugs.jquery.com/ticket/12359
-                        docElem.appendChild(el).innerHTML = "<a id='" + expando + "'></a>" +
-                            "<select id='" + expando + "-\r\\' msallowcapture=''>" +
-                            "<option selected=''></option></select>";
-
-                        // Support: IE8, Opera 11-12.16
-                        // Nothing should be selected when empty strings follow ^= or $= or *=
-                        // The test attribute must be unknown in Opera but "safe" for WinRT
-                        // https://msdn.microsoft.com/en-us/library/ie/hh465388.aspx#attribute_section
-                        if (el.querySelectorAll("[msallowcapture^='']").length) {
-                            rbuggyQSA.push("[*^$]=" + whitespace + "*(?:''|\"\")");
-                        }
-
-                        // Support: IE8
-                        // Boolean attributes and "value" are not treated correctly
-                        if (!el.querySelectorAll("[selected]").length) {
-                            rbuggyQSA.push("\\[" + whitespace + "*(?:value|" + booleans + ")");
-                        }
-
-                        // Support: Chrome<29, Android<4.4, Safari<7.0+, iOS<7.0+, PhantomJS<1.9.8+
-                        if (!el.querySelectorAll("[id~=" + expando + "-]").length) {
-                            rbuggyQSA.push("~=");
-                        }
-
-                        // Support: IE 11+, Edge 15 - 18+
-                        // IE 11/Edge don't find elements on a `[name='']` query in some cases.
-                        // Adding a temporary attribute to the document before the selection works
-                        // around the issue.
-                        // Interestingly, IE 10 & older don't seem to have the issue.
-                        input = document.createElement("input");
-                        input.setAttribute("name", "");
-                        el.appendChild(input);
-                        if (!el.querySelectorAll("[name='']").length) {
-                            rbuggyQSA.push("\\[" + whitespace + "*name" + whitespace + "*=" +
-                                whitespace + "*(?:''|\"\")");
-                        }
-
-                        // Webkit/Opera - :checked should return selected option elements
-                        // http://www.w3.org/TR/2011/REC-css3-selectors-20110929/#checked
-                        // IE8 throws error here and will not see later tests
-                        if (!el.querySelectorAll(":checked").length) {
-                            rbuggyQSA.push(":checked");
-                        }
-
-                        // Support: Safari 8+, iOS 8+
-                        // https://bugs.webkit.org/show_bug.cgi?id=136851
-                        // In-page `selector#id sibling-combinator selector` fails
-                        if (!el.querySelectorAll("a#" + expando + "+*").length) {
-                            rbuggyQSA.push(".#.+[+~]");
-                        }
-
-                        // Support: Firefox <=3.6 - 5 only
-                        // Old Firefox doesn't throw on a badly-escaped identifier.
-                        el.querySelectorAll("\\\f");
-                        rbuggyQSA.push("[\\r\\n\\f]");
-                    });
-
-                    assert(function(el) {
-                        el.innerHTML = "<a href='' disabled='disabled'></a>" +
-                            "<select disabled='disabled'><option/></select>";
-
-                        // Support: Windows 8 Native Apps
-                        // The type and name attributes are restricted during .innerHTML assignment
-                        var input = document.createElement("input");
-                        input.setAttribute("type", "hidden");
-                        el.appendChild(input).setAttribute("name", "D");
-
-                        // Support: IE8
-                        // Enforce case-sensitivity of name attribute
-                        if (el.querySelectorAll("[name=d]").length) {
-                            rbuggyQSA.push("name" + whitespace + "*[*^$|!~]?=");
-                        }
-
-                        // FF 3.5 - :enabled/:disabled and hidden elements (hidden elements are still enabled)
-                        // IE8 throws error here and will not see later tests
-                        if (el.querySelectorAll(":enabled").length !== 2) {
-                            rbuggyQSA.push(":enabled", ":disabled");
-                        }
-
-                        // Support: IE9-11+
-                        // IE's :disabled selector does not pick up the children of disabled fieldsets
-                        docElem.appendChild(el).disabled = true;
-                        if (el.querySelectorAll(":disabled").length !== 2) {
-                            rbuggyQSA.push(":enabled", ":disabled");
-                        }
-
-                        // Support: Opera 10 - 11 only
-                        // Opera 10-11 does not throw on post-comma invalid pseudos
-                        el.querySelectorAll("*,:x");
-                        rbuggyQSA.push(",.*:");
-                    });
+                    // Try to winnow out elements that can't be disabled before trusting the disabled property.
+                    // Some victims get caught in our net (label, legend, menu, track), but it shouldn't
+                    // even exist on them, let alone have a boolean value.
+                } else if ("label" in elem) {
+                    return elem.disabled === disabled;
                 }
 
-                if ((support.matchesSelector = rnative.test((matches = docElem.matches ||
-                        docElem.webkitMatchesSelector ||
-                        docElem.mozMatchesSelector ||
-                        docElem.oMatchesSelector ||
-                        docElem.msMatchesSelector)))) {
-
-                    assert(function(el) {
-
-                        // Check to see if it's possible to do matchesSelector
-                        // on a disconnected node (IE 9)
-                        support.disconnectedMatch = matches.call(el, "*");
-
-                        // This should fail with an exception
-                        // Gecko does not error, returns false instead
-                        matches.call(el, "[s!='']:x");
-                        rbuggyMatches.push("!=", pseudos);
-                    });
-                }
+                // Remaining elements are neither :enabled nor :disabled
+                return false;
+            };
+        }
 
-                rbuggyQSA = rbuggyQSA.length && new RegExp(rbuggyQSA.join("|"));
-                rbuggyMatches = rbuggyMatches.length && new RegExp(rbuggyMatches.join("|"));
+        /**
+         * Returns a function to use in pseudos for positionals
+         * @param {Function} fn
+         */
+        function createPositionalPseudo(fn) {
+            return markFunction(function(argument) {
+                argument = +argument;
+                return markFunction(function(seed, matches) {
+                    var j,
+                        matchIndexes = fn([], seed.length, argument),
+                        i = matchIndexes.length;
 
-                /* Contains
-                ---------------------------------------------------------------------- */
-                hasCompare = rnative.test(docElem.compareDocumentPosition);
-
-                // Element contains another
-                // Purposefully self-exclusive
-                // As in, an element does not contain itself
-                contains = hasCompare || rnative.test(docElem.contains) ?
-                    function(a, b) {
-                        var adown = a.nodeType === 9 ? a.documentElement : a,
-                            bup = b && b.parentNode;
-                        return a === bup || !!(bup && bup.nodeType === 1 && (
-                            adown.contains ?
-                            adown.contains(bup) :
-                            a.compareDocumentPosition && a.compareDocumentPosition(bup) & 16
-                        ));
-                    } :
-                    function(a, b) {
-                        if (b) {
-                            while ((b = b.parentNode)) {
-                                if (b === a) {
-                                    return true;
-                                }
-                            }
+                    // Match elements found at the specified indexes
+                    while (i--) {
+                        if (seed[(j = matchIndexes[i])]) {
+                            seed[j] = !(matches[j] = seed[j]);
                         }
-                        return false;
-                    };
-
-                /* Sorting
-                ---------------------------------------------------------------------- */
+                    }
+                });
+            });
+        }
 
-                // Document order sorting
-                sortOrder = hasCompare ?
-                    function(a, b) {
+        /**
+         * Checks a node for validity as a jQuery selector context
+         * @param {Element|Object=} context
+         * @returns {Element|Object|Boolean} The input node if acceptable, otherwise a falsy value
+         */
+        function testContext(context) {
+            return context && typeof context.getElementsByTagName !== "undefined" && context;
+        }
 
-                        // Flag for duplicate removal
-                        if (a === b) {
-                            hasDuplicate = true;
-                            return 0;
-                        }
+        /**
+         * Sets document-related variables once based on the current document
+         * @param {Element|Object} [node] An element or document object to use to set the document
+         * @returns {Object} Returns the current document
+         */
+        function setDocument(node) {
+            var subWindow,
+                doc = node ? node.ownerDocument || node : preferredDoc;
+
+            // Return early if doc is invalid or already selected
+            // Support: IE 11+, Edge 17 - 18+
+            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+            // two documents; shallow comparisons work.
+            // eslint-disable-next-line eqeqeq
+            if (doc == document || doc.nodeType !== 9 || !doc.documentElement) {
+                return document;
+            }
 
-                        // Sort on method existence if only one input has compareDocumentPosition
-                        var compare = !a.compareDocumentPosition - !b.compareDocumentPosition;
-                        if (compare) {
-                            return compare;
-                        }
+            // Update global variables
+            document = doc;
+            documentElement = document.documentElement;
+            documentIsHTML = !jQuery.isXMLDoc(document);
+
+            // Support: iOS 7 only, IE 9 - 11+
+            // Older browsers didn't support unprefixed `matches`.
+            matches = documentElement.matches ||
+                documentElement.webkitMatchesSelector ||
+                documentElement.msMatchesSelector;
+
+            // Support: IE 9 - 11+, Edge 12 - 18+
+            // Accessing iframe documents after unload throws "permission denied" errors (see trac-13936)
+            // Support: IE 11+, Edge 17 - 18+
+            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+            // two documents; shallow comparisons work.
+            // eslint-disable-next-line eqeqeq
+            if (preferredDoc != document &&
+                (subWindow = document.defaultView) && subWindow.top !== subWindow) {
 
-                        // Calculate position if both inputs belong to the same document
-                        // Support: IE 11+, Edge 17 - 18+
-                        // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                        // two documents; shallow comparisons work.
-                        // eslint-disable-next-line eqeqeq
-                        compare = (a.ownerDocument || a) == (b.ownerDocument || b) ?
-                            a.compareDocumentPosition(b) :
-
-                            // Otherwise we know they are disconnected
-                            1;
+                // Support: IE 9 - 11+, Edge 12 - 18+
+                subWindow.addEventListener("unload", unloadHandler);
+            }
 
-                        // Disconnected nodes
-                        if (compare & 1 ||
-                            (!support.sortDetached && b.compareDocumentPosition(a) === compare)) {
+            // Support: IE <10
+            // Check if getElementById returns elements by name
+            // The broken getElementById methods don't pick up programmatically-set names,
+            // so use a roundabout getElementsByName test
+            support.getById = assert(function(el) {
+                documentElement.appendChild(el).id = jQuery.expando;
+                return !document.getElementsByName ||
+                    !document.getElementsByName(jQuery.expando).length;
+            });
 
-                            // Choose the first element that is related to our preferred document
-                            // Support: IE 11+, Edge 17 - 18+
-                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                            // two documents; shallow comparisons work.
-                            // eslint-disable-next-line eqeqeq
-                            if (a == document || a.ownerDocument == preferredDoc &&
-                                contains(preferredDoc, a)) {
-                                return -1;
-                            }
+            // Support: IE 9 only
+            // Check to see if it's possible to do matchesSelector
+            // on a disconnected node.
+            support.disconnectedMatch = assert(function(el) {
+                return matches.call(el, "*");
+            });
 
-                            // Support: IE 11+, Edge 17 - 18+
-                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                            // two documents; shallow comparisons work.
-                            // eslint-disable-next-line eqeqeq
-                            if (b == document || b.ownerDocument == preferredDoc &&
-                                contains(preferredDoc, b)) {
-                                return 1;
-                            }
+            // Support: IE 9 - 11+, Edge 12 - 18+
+            // IE/Edge don't support the :scope pseudo-class.
+            support.scope = assert(function() {
+                return document.querySelectorAll(":scope");
+            });
 
-                            // Maintain original order
-                            return sortInput ?
-                                (indexOf(sortInput, a) - indexOf(sortInput, b)) :
-                                0;
-                        }
-
-                        return compare & 4 ? -1 : 1;
-                    } :
-                    function(a, b) {
-
-                        // Exit early if the nodes are identical
-                        if (a === b) {
-                            hasDuplicate = true;
-                            return 0;
-                        }
-
-                        var cur,
-                            i = 0,
-                            aup = a.parentNode,
-                            bup = b.parentNode,
-                            ap = [a],
-                            bp = [b];
+            // Support: Chrome 105 - 111 only, Safari 15.4 - 16.3 only
+            // Make sure the `:has()` argument is parsed unforgivingly.
+            // We include `*` in the test to detect buggy implementations that are
+            // _selectively_ forgiving (specifically when the list includes at least
+            // one valid selector).
+            // Note that we treat complete lack of support for `:has()` as if it were
+            // spec-compliant support, which is fine because use of `:has()` in such
+            // environments will fail in the qSA path and fall back to jQuery traversal
+            // anyway.
+            support.cssHas = assert(function() {
+                try {
+                    document.querySelector(":has(*,:jqfake)");
+                    return false;
+                } catch (e) {
+                    return true;
+                }
+            });
 
-                        // Parentless nodes are either documents or disconnected
-                        if (!aup || !bup) {
+            // ID filter and find
+            if (support.getById) {
+                Expr.filter.ID = function(id) {
+                    var attrId = id.replace(runescape, funescape);
+                    return function(elem) {
+                        return elem.getAttribute("id") === attrId;
+                    };
+                };
+                Expr.find.ID = function(id, context) {
+                    if (typeof context.getElementById !== "undefined" && documentIsHTML) {
+                        var elem = context.getElementById(id);
+                        return elem ? [elem] : [];
+                    }
+                };
+            } else {
+                Expr.filter.ID = function(id) {
+                    var attrId = id.replace(runescape, funescape);
+                    return function(elem) {
+                        var node = typeof elem.getAttributeNode !== "undefined" &&
+                            elem.getAttributeNode("id");
+                        return node && node.value === attrId;
+                    };
+                };
 
-                            // Support: IE 11+, Edge 17 - 18+
-                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                            // two documents; shallow comparisons work.
-                            /* eslint-disable eqeqeq */
-                            return a == document ? -1 :
-                                b == document ? 1 :
-                                /* eslint-enable eqeqeq */
-                                aup ? -1 :
-                                bup ? 1 :
-                                sortInput ?
-                                (indexOf(sortInput, a) - indexOf(sortInput, b)) :
-                                0;
+                // Support: IE 6 - 7 only
+                // getElementById is not reliable as a find shortcut
+                Expr.find.ID = function(id, context) {
+                    if (typeof context.getElementById !== "undefined" && documentIsHTML) {
+                        var node, i, elems,
+                            elem = context.getElementById(id);
 
-                            // If the nodes are siblings, we can do a quick check
-                        } else if (aup === bup) {
-                            return siblingCheck(a, b);
-                        }
+                        if (elem) {
 
-                        // Otherwise we need full lists of their ancestors for comparison
-                        cur = a;
-                        while ((cur = cur.parentNode)) {
-                            ap.unshift(cur);
-                        }
-                        cur = b;
-                        while ((cur = cur.parentNode)) {
-                            bp.unshift(cur);
-                        }
+                            // Verify the id attribute
+                            node = elem.getAttributeNode("id");
+                            if (node && node.value === id) {
+                                return [elem];
+                            }
 
-                        // Walk down the tree looking for a discrepancy
-                        while (ap[i] === bp[i]) {
-                            i++;
+                            // Fall back on getElementsByName
+                            elems = context.getElementsByName(id);
+                            i = 0;
+                            while ((elem = elems[i++])) {
+                                node = elem.getAttributeNode("id");
+                                if (node && node.value === id) {
+                                    return [elem];
+                                }
+                            }
                         }
 
-                        return i ?
-
-                            // Do a sibling check if the nodes have a common ancestor
-                            siblingCheck(ap[i], bp[i]) :
+                        return [];
+                    }
+                };
+            }
 
-                            // Otherwise nodes in our document sort first
-                            // Support: IE 11+, Edge 17 - 18+
-                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                            // two documents; shallow comparisons work.
-                            /* eslint-disable eqeqeq */
-                            ap[i] == preferredDoc ? -1 :
-                            bp[i] == preferredDoc ? 1 :
-                            /* eslint-enable eqeqeq */
-                            0;
-                    };
+            // Tag
+            Expr.find.TAG = function(tag, context) {
+                if (typeof context.getElementsByTagName !== "undefined") {
+                    return context.getElementsByTagName(tag);
 
-                return document;
+                    // DocumentFragment nodes don't have gEBTN
+                } else {
+                    return context.querySelectorAll(tag);
+                }
             };
 
-            Sizzle.matches = function(expr, elements) {
-                return Sizzle(expr, null, null, elements);
+            // Class
+            Expr.find.CLASS = function(className, context) {
+                if (typeof context.getElementsByClassName !== "undefined" && documentIsHTML) {
+                    return context.getElementsByClassName(className);
+                }
             };
 
-            Sizzle.matchesSelector = function(elem, expr) {
-                setDocument(elem);
+            /* QSA/matchesSelector
+            ---------------------------------------------------------------------- */
 
-                if (support.matchesSelector && documentIsHTML &&
-                    !nonnativeSelectorCache[expr + " "] &&
-                    (!rbuggyMatches || !rbuggyMatches.test(expr)) &&
-                    (!rbuggyQSA || !rbuggyQSA.test(expr))) {
+            // QSA and matchesSelector support
 
-                    try {
-                        var ret = matches.call(elem, expr);
+            rbuggyQSA = [];
 
-                        // IE 9's matchesSelector returns false on disconnected nodes
-                        if (ret || support.disconnectedMatch ||
-
-                            // As well, disconnected nodes are said to be in a document
-                            // fragment in IE 9
-                            elem.document && elem.document.nodeType !== 11) {
-                            return ret;
-                        }
-                    } catch (e) {
-                        nonnativeSelectorCache(expr, true);
-                    }
+            // Build QSA regex
+            // Regex strategy adopted from Diego Perini
+            assert(function(el) {
+
+                var input;
+
+                documentElement.appendChild(el).innerHTML =
+                    "<a id='" + expando + "' href='' disabled='disabled'></a>" +
+                    "<select id='" + expando + "-\r\\' disabled='disabled'>" +
+                    "<option selected=''></option></select>";
+
+                // Support: iOS <=7 - 8 only
+                // Boolean attributes and "value" are not treated correctly in some XML documents
+                if (!el.querySelectorAll("[selected]").length) {
+                    rbuggyQSA.push("\\[" + whitespace + "*(?:value|" + booleans + ")");
+                }
+
+                // Support: iOS <=7 - 8 only
+                if (!el.querySelectorAll("[id~=" + expando + "-]").length) {
+                    rbuggyQSA.push("~=");
+                }
+
+                // Support: iOS 8 only
+                // https://bugs.webkit.org/show_bug.cgi?id=136851
+                // In-page `selector#id sibling-combinator selector` fails
+                if (!el.querySelectorAll("a#" + expando + "+*").length) {
+                    rbuggyQSA.push(".#.+[+~]");
+                }
+
+                // Support: Chrome <=105+, Firefox <=104+, Safari <=15.4+
+                // In some of the document kinds, these selectors wouldn't work natively.
+                // This is probably OK but for backwards compatibility we want to maintain
+                // handling them through jQuery traversal in jQuery 3.x.
+                if (!el.querySelectorAll(":checked").length) {
+                    rbuggyQSA.push(":checked");
+                }
+
+                // Support: Windows 8 Native Apps
+                // The type and name attributes are restricted during .innerHTML assignment
+                input = document.createElement("input");
+                input.setAttribute("type", "hidden");
+                el.appendChild(input).setAttribute("name", "D");
+
+                // Support: IE 9 - 11+
+                // IE's :disabled selector does not pick up the children of disabled fieldsets
+                // Support: Chrome <=105+, Firefox <=104+, Safari <=15.4+
+                // In some of the document kinds, these selectors wouldn't work natively.
+                // This is probably OK but for backwards compatibility we want to maintain
+                // handling them through jQuery traversal in jQuery 3.x.
+                documentElement.appendChild(el).disabled = true;
+                if (el.querySelectorAll(":disabled").length !== 2) {
+                    rbuggyQSA.push(":enabled", ":disabled");
+                }
+
+                // Support: IE 11+, Edge 15 - 18+
+                // IE 11/Edge don't find elements on a `[name='']` query in some cases.
+                // Adding a temporary attribute to the document before the selection works
+                // around the issue.
+                // Interestingly, IE 10 & older don't seem to have the issue.
+                input = document.createElement("input");
+                input.setAttribute("name", "");
+                el.appendChild(input);
+                if (!el.querySelectorAll("[name='']").length) {
+                    rbuggyQSA.push("\\[" + whitespace + "*name" + whitespace + "*=" +
+                        whitespace + "*(?:''|\"\")");
                 }
+            });
 
-                return Sizzle(expr, document, null, [elem]).length > 0;
-            };
+            if (!support.cssHas) {
 
-            Sizzle.contains = function(context, elem) {
+                // Support: Chrome 105 - 110+, Safari 15.4 - 16.3+
+                // Our regular `try-catch` mechanism fails to detect natively-unsupported
+                // pseudo-classes inside `:has()` (such as `:has(:contains("Foo"))`)
+                // in browsers that parse the `:has()` argument as a forgiving selector list.
+                // https://drafts.csswg.org/selectors/#relational now requires the argument
+                // to be parsed unforgivingly, but browsers have not yet fully adjusted.
+                rbuggyQSA.push(":has");
+            }
 
-                // Set document vars if needed
-                // Support: IE 11+, Edge 17 - 18+
-                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                // two documents; shallow comparisons work.
-                // eslint-disable-next-line eqeqeq
-                if ((context.ownerDocument || context) != document) {
-                    setDocument(context);
+            rbuggyQSA = rbuggyQSA.length && new RegExp(rbuggyQSA.join("|"));
+
+            /* Sorting
+            ---------------------------------------------------------------------- */
+
+            // Document order sorting
+            sortOrder = function(a, b) {
+
+                // Flag for duplicate removal
+                if (a === b) {
+                    hasDuplicate = true;
+                    return 0;
                 }
-                return contains(context, elem);
-            };
 
-            Sizzle.attr = function(elem, name) {
+                // Sort on method existence if only one input has compareDocumentPosition
+                var compare = !a.compareDocumentPosition - !b.compareDocumentPosition;
+                if (compare) {
+                    return compare;
+                }
 
-                // Set document vars if needed
+                // Calculate position if both inputs belong to the same document
                 // Support: IE 11+, Edge 17 - 18+
                 // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
                 // two documents; shallow comparisons work.
                 // eslint-disable-next-line eqeqeq
-                if ((elem.ownerDocument || elem) != document) {
-                    setDocument(elem);
-                }
+                compare = (a.ownerDocument || a) == (b.ownerDocument || b) ?
+                    a.compareDocumentPosition(b) :
 
-                var fn = Expr.attrHandle[name.toLowerCase()],
+                    // Otherwise we know they are disconnected
+                    1;
 
-                    // Don't get fooled by Object.prototype properties (jQuery #13807)
-                    val = fn && hasOwn.call(Expr.attrHandle, name.toLowerCase()) ?
-                    fn(elem, name, !documentIsHTML) :
-                    undefined;
-
-                return val !== undefined ?
-                    val :
-                    support.attributes || !documentIsHTML ?
-                    elem.getAttribute(name) :
-                    (val = elem.getAttributeNode(name)) && val.specified ?
-                    val.value :
-                    null;
-            };
+                // Disconnected nodes
+                if (compare & 1 ||
+                    (!support.sortDetached && b.compareDocumentPosition(a) === compare)) {
+
+                    // Choose the first element that is related to our preferred document
+                    // Support: IE 11+, Edge 17 - 18+
+                    // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                    // two documents; shallow comparisons work.
+                    // eslint-disable-next-line eqeqeq
+                    if (a === document || a.ownerDocument == preferredDoc &&
+                        find.contains(preferredDoc, a)) {
+                        return -1;
+                    }
+
+                    // Support: IE 11+, Edge 17 - 18+
+                    // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                    // two documents; shallow comparisons work.
+                    // eslint-disable-next-line eqeqeq
+                    if (b === document || b.ownerDocument == preferredDoc &&
+                        find.contains(preferredDoc, b)) {
+                        return 1;
+                    }
+
+                    // Maintain original order
+                    return sortInput ?
+                        (indexOf.call(sortInput, a) - indexOf.call(sortInput, b)) :
+                        0;
+                }
 
-            Sizzle.escape = function(sel) {
-                return (sel + "").replace(rcssescape, fcssescape);
+                return compare & 4 ? -1 : 1;
             };
 
-            Sizzle.error = function(msg) {
-                throw new Error("Syntax error, unrecognized expression: " + msg);
-            };
+            return document;
+        }
 
-            /**
-             * Document sorting and removing duplicates
-             * @param {ArrayLike} results
-             */
-            Sizzle.uniqueSort = function(results) {
-                var elem,
-                    duplicates = [],
-                    j = 0,
-                    i = 0;
+        find.matches = function(expr, elements) {
+            return find(expr, null, null, elements);
+        };
 
-                // Unless we *know* we can detect duplicates, assume their presence
-                hasDuplicate = !support.detectDuplicates;
-                sortInput = !support.sortStable && results.slice(0);
-                results.sort(sortOrder);
-
-                if (hasDuplicate) {
-                    while ((elem = results[i++])) {
-                        if (elem === results[i]) {
-                            j = duplicates.push(i);
-                        }
-                    }
-                    while (j--) {
-                        results.splice(duplicates[j], 1);
-                    }
-                }
+        find.matchesSelector = function(elem, expr) {
+            setDocument(elem);
 
-                // Clear input after sorting to release objects
-                // See https://github.com/jquery/sizzle/pull/225
-                sortInput = null;
+            if (documentIsHTML &&
+                !nonnativeSelectorCache[expr + " "] &&
+                (!rbuggyQSA || !rbuggyQSA.test(expr))) {
 
-                return results;
-            };
+                try {
+                    var ret = matches.call(elem, expr);
 
-            /**
-             * Utility function for retrieving the text value of an array of DOM nodes
-             * @param {Array|Element} elem
-             */
-            getText = Sizzle.getText = function(elem) {
-                var node,
-                    ret = "",
-                    i = 0,
-                    nodeType = elem.nodeType;
+                    // IE 9's matchesSelector returns false on disconnected nodes
+                    if (ret || support.disconnectedMatch ||
 
-                if (!nodeType) {
+                        // As well, disconnected nodes are said to be in a document
+                        // fragment in IE 9
+                        elem.document && elem.document.nodeType !== 11) {
+                        return ret;
+                    }
+                } catch (e) {
+                    nonnativeSelectorCache(expr, true);
+                }
+            }
 
-                    // If no nodeType, this is expected to be an array
-                    while ((node = elem[i++])) {
+            return find(expr, document, null, [elem]).length > 0;
+        };
 
-                        // Do not traverse comment nodes
-                        ret += getText(node);
-                    }
-                } else if (nodeType === 1 || nodeType === 9 || nodeType === 11) {
+        find.contains = function(context, elem) {
 
-                    // Use textContent for elements
-                    // innerText usage removed for consistency of new lines (jQuery #11153)
-                    if (typeof elem.textContent === "string") {
-                        return elem.textContent;
-                    } else {
+            // Set document vars if needed
+            // Support: IE 11+, Edge 17 - 18+
+            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+            // two documents; shallow comparisons work.
+            // eslint-disable-next-line eqeqeq
+            if ((context.ownerDocument || context) != document) {
+                setDocument(context);
+            }
+            return jQuery.contains(context, elem);
+        };
 
-                        // Traverse its children
-                        for (elem = elem.firstChild; elem; elem = elem.nextSibling) {
-                            ret += getText(elem);
-                        }
-                    }
-                } else if (nodeType === 3 || nodeType === 4) {
-                    return elem.nodeValue;
-                }
 
-                // Do not include comment or processing instruction nodes
+        find.attr = function(elem, name) {
 
-                return ret;
-            };
+            // Set document vars if needed
+            // Support: IE 11+, Edge 17 - 18+
+            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+            // two documents; shallow comparisons work.
+            // eslint-disable-next-line eqeqeq
+            if ((elem.ownerDocument || elem) != document) {
+                setDocument(elem);
+            }
 
-            Expr = Sizzle.selectors = {
+            var fn = Expr.attrHandle[name.toLowerCase()],
 
-                // Can be adjusted by the user
-                cacheLength: 50,
+                // Don't get fooled by Object.prototype properties (see trac-13807)
+                val = fn && hasOwn.call(Expr.attrHandle, name.toLowerCase()) ?
+                fn(elem, name, !documentIsHTML) :
+                undefined;
 
-                createPseudo: markFunction,
+            if (val !== undefined) {
+                return val;
+            }
 
-                match: matchExpr,
+            return elem.getAttribute(name);
+        };
 
-                attrHandle: {},
+        find.error = function(msg) {
+            throw new Error("Syntax error, unrecognized expression: " + msg);
+        };
 
-                find: {},
+        /**
+         * Document sorting and removing duplicates
+         * @param {ArrayLike} results
+         */
+        jQuery.uniqueSort = function(results) {
+            var elem,
+                duplicates = [],
+                j = 0,
+                i = 0;
 
-                relative: {
-                    ">": {
-                        dir: "parentNode",
-                        first: true
-                    },
-                    " ": {
-                        dir: "parentNode"
-                    },
-                    "+": {
-                        dir: "previousSibling",
-                        first: true
-                    },
-                    "~": {
-                        dir: "previousSibling"
+            // Unless we *know* we can detect duplicates, assume their presence
+            //
+            // Support: Android <=4.0+
+            // Testing for detecting duplicates is unpredictable so instead assume we can't
+            // depend on duplicate detection in all browsers without a stable sort.
+            hasDuplicate = !support.sortStable;
+            sortInput = !support.sortStable && slice.call(results, 0);
+            sort.call(results, sortOrder);
+
+            if (hasDuplicate) {
+                while ((elem = results[i++])) {
+                    if (elem === results[i]) {
+                        j = duplicates.push(i);
                     }
-                },
+                }
+                while (j--) {
+                    splice.call(results, duplicates[j], 1);
+                }
+            }
 
-                preFilter: {
-                    "ATTR": function(match) {
-                        match[1] = match[1].replace(runescape, funescape);
+            // Clear input after sorting to release objects
+            // See https://github.com/jquery/sizzle/pull/225
+            sortInput = null;
 
-                        // Move the given value to match[3] whether quoted or unquoted
-                        match[3] = (match[3] || match[4] ||
-                            match[5] || "").replace(runescape, funescape);
+            return results;
+        };
 
-                        if (match[2] === "~=") {
-                            match[3] = " " + match[3] + " ";
-                        }
+        jQuery.fn.uniqueSort = function() {
+            return this.pushStack(jQuery.uniqueSort(slice.apply(this)));
+        };
 
-                        return match.slice(0, 4);
-                    },
+        Expr = jQuery.expr = {
 
-                    "CHILD": function(match) {
+            // Can be adjusted by the user
+            cacheLength: 50,
 
-                        /* matches from matchExpr["CHILD"]
-                        	1 type (only|nth|...)
-                        	2 what (child|of-type)
-                        	3 argument (even|odd|\d*|\d*n([+-]\d+)?|...)
-                        	4 xn-component of xn+y argument ([+-]?\d*n|)
-                        	5 sign of xn-component
-                        	6 x of xn-component
-                        	7 sign of y-component
-                        	8 y of y-component
-                        */
-                        match[1] = match[1].toLowerCase();
-
-                        if (match[1].slice(0, 3) === "nth") {
-
-                            // nth-* requires argument
-                            if (!match[3]) {
-                                Sizzle.error(match[0]);
-                            }
+            createPseudo: markFunction,
 
-                            // numeric x and y parameters for Expr.filter.CHILD
-                            // remember that false/true cast respectively to 0/1
-                            match[4] = +(match[4] ?
-                                match[5] + (match[6] || 1) :
-                                2 * (match[3] === "even" || match[3] === "odd"));
-                            match[5] = +((match[7] + match[8]) || match[3] === "odd");
-
-                            // other types prohibit arguments
-                        } else if (match[3]) {
-                            Sizzle.error(match[0]);
-                        }
+            match: matchExpr,
 
-                        return match;
-                    },
+            attrHandle: {},
 
-                    "PSEUDO": function(match) {
-                        var excess,
-                            unquoted = !match[6] && match[2];
+            find: {},
 
-                        if (matchExpr["CHILD"].test(match[0])) {
-                            return null;
-                        }
+            relative: {
+                ">": {
+                    dir: "parentNode",
+                    first: true
+                },
+                " ": {
+                    dir: "parentNode"
+                },
+                "+": {
+                    dir: "previousSibling",
+                    first: true
+                },
+                "~": {
+                    dir: "previousSibling"
+                }
+            },
+
+            preFilter: {
+                ATTR: function(match) {
+                    match[1] = match[1].replace(runescape, funescape);
 
-                        // Accept quoted arguments as-is
-                        if (match[3]) {
-                            match[2] = match[4] || match[5] || "";
+                    // Move the given value to match[3] whether quoted or unquoted
+                    match[3] = (match[3] || match[4] || match[5] || "")
+                        .replace(runescape, funescape);
 
-                            // Strip excess characters from unquoted arguments
-                        } else if (unquoted && rpseudo.test(unquoted) &&
+                    if (match[2] === "~=") {
+                        match[3] = " " + match[3] + " ";
+                    }
 
-                            // Get excess from tokenize (recursively)
-                            (excess = tokenize(unquoted, true)) &&
+                    return match.slice(0, 4);
+                },
 
-                            // advance to the next closing parenthesis
-                            (excess = unquoted.indexOf(")", unquoted.length - excess) - unquoted.length)) {
+                CHILD: function(match) {
 
-                            // excess is a negative index
-                            match[0] = match[0].slice(0, excess);
-                            match[2] = unquoted.slice(0, excess);
-                        }
+                    /* matches from matchExpr["CHILD"]
+                    	1 type (only|nth|...)
+                    	2 what (child|of-type)
+                    	3 argument (even|odd|\d*|\d*n([+-]\d+)?|...)
+                    	4 xn-component of xn+y argument ([+-]?\d*n|)
+                    	5 sign of xn-component
+                    	6 x of xn-component
+                    	7 sign of y-component
+                    	8 y of y-component
+                    */
+                    match[1] = match[1].toLowerCase();
+
+                    if (match[1].slice(0, 3) === "nth") {
+
+                        // nth-* requires argument
+                        if (!match[3]) {
+                            find.error(match[0]);
+                        }
+
+                        // numeric x and y parameters for Expr.filter.CHILD
+                        // remember that false/true cast respectively to 0/1
+                        match[4] = +(match[4] ?
+                            match[5] + (match[6] || 1) :
+                            2 * (match[3] === "even" || match[3] === "odd")
+                        );
+                        match[5] = +((match[7] + match[8]) || match[3] === "odd");
 
-                        // Return only captures needed by the pseudo filter method (type and argument)
-                        return match.slice(0, 3);
+                        // other types prohibit arguments
+                    } else if (match[3]) {
+                        find.error(match[0]);
                     }
+
+                    return match;
                 },
 
-                filter: {
+                PSEUDO: function(match) {
+                    var excess,
+                        unquoted = !match[6] && match[2];
 
-                    "TAG": function(nodeNameSelector) {
-                        var nodeName = nodeNameSelector.replace(runescape, funescape).toLowerCase();
-                        return nodeNameSelector === "*" ?
-                            function() {
-                                return true;
-                            } :
-                            function(elem) {
-                                return elem.nodeName && elem.nodeName.toLowerCase() === nodeName;
-                            };
-                    },
+                    if (matchExpr.CHILD.test(match[0])) {
+                        return null;
+                    }
 
-                    "CLASS": function(className) {
-                        var pattern = classCache[className + " "];
+                    // Accept quoted arguments as-is
+                    if (match[3]) {
+                        match[2] = match[4] || match[5] || "";
 
-                        return pattern ||
-                            (pattern = new RegExp("(^|" + whitespace +
-                                ")" + className + "(" + whitespace + "|$)")) && classCache(
-                                className,
-                                function(elem) {
-                                    return pattern.test(
-                                        typeof elem.className === "string" && elem.className ||
-                                        typeof elem.getAttribute !== "undefined" &&
-                                        elem.getAttribute("class") ||
-                                        ""
-                                    );
-                                });
-                    },
+                        // Strip excess characters from unquoted arguments
+                    } else if (unquoted && rpseudo.test(unquoted) &&
 
-                    "ATTR": function(name, operator, check) {
-                        return function(elem) {
-                            var result = Sizzle.attr(elem, name);
+                        // Get excess from tokenize (recursively)
+                        (excess = tokenize(unquoted, true)) &&
 
-                            if (result == null) {
-                                return operator === "!=";
-                            }
-                            if (!operator) {
-                                return true;
-                            }
+                        // advance to the next closing parenthesis
+                        (excess = unquoted.indexOf(")", unquoted.length - excess) - unquoted.length)) {
 
-                            result += "";
+                        // excess is a negative index
+                        match[0] = match[0].slice(0, excess);
+                        match[2] = unquoted.slice(0, excess);
+                    }
 
-                            /* eslint-disable max-len */
+                    // Return only captures needed by the pseudo filter method (type and argument)
+                    return match.slice(0, 3);
+                }
+            },
 
-                            return operator === "=" ? result === check :
-                                operator === "!=" ? result !== check :
-                                operator === "^=" ? check && result.indexOf(check) === 0 :
-                                operator === "*=" ? check && result.indexOf(check) > -1 :
-                                operator === "$=" ? check && result.slice(-check.length) === check :
-                                operator === "~=" ? (" " + result.replace(rwhitespace, " ") + " ").indexOf(check) > -1 :
-                                operator === "|=" ? result === check || result.slice(0, check.length + 1) === check + "-" :
-                                false;
-                            /* eslint-enable max-len */
+            filter: {
 
+                TAG: function(nodeNameSelector) {
+                    var expectedNodeName = nodeNameSelector.replace(runescape, funescape).toLowerCase();
+                    return nodeNameSelector === "*" ?
+                        function() {
+                            return true;
+                        } :
+                        function(elem) {
+                            return nodeName(elem, expectedNodeName);
                         };
-                    },
-
-                    "CHILD": function(type, what, _argument, first, last) {
-                        var simple = type.slice(0, 3) !== "nth",
-                            forward = type.slice(-4) !== "last",
-                            ofType = what === "of-type";
+                },
 
-                        return first === 1 && last === 0 ?
+                CLASS: function(className) {
+                    var pattern = classCache[className + " "];
 
-                            // Shortcut for :nth-*(n)
-                            function(elem) {
-                                return !!elem.parentNode;
-                            } :
+                    return pattern ||
+                        (pattern = new RegExp("(^|" + whitespace + ")" + className +
+                            "(" + whitespace + "|$)")) &&
+                        classCache(className, function(elem) {
+                            return pattern.test(
+                                typeof elem.className === "string" && elem.className ||
+                                typeof elem.getAttribute !== "undefined" &&
+                                elem.getAttribute("class") ||
+                                ""
+                            );
+                        });
+                },
 
-                            function(elem, _context, xml) {
-                                var cache, uniqueCache, outerCache, node, nodeIndex, start,
-                                    dir = simple !== forward ? "nextSibling" : "previousSibling",
-                                    parent = elem.parentNode,
-                                    name = ofType && elem.nodeName.toLowerCase(),
-                                    useCache = !xml && !ofType,
-                                    diff = false;
-
-                                if (parent) {
-
-                                    // :(first|last|only)-(child|of-type)
-                                    if (simple) {
-                                        while (dir) {
-                                            node = elem;
-                                            while ((node = node[dir])) {
-                                                if (ofType ?
-                                                    node.nodeName.toLowerCase() === name :
-                                                    node.nodeType === 1) {
+                ATTR: function(name, operator, check) {
+                    return function(elem) {
+                        var result = find.attr(elem, name);
 
-                                                    return false;
-                                                }
-                                            }
+                        if (result == null) {
+                            return operator === "!=";
+                        }
+                        if (!operator) {
+                            return true;
+                        }
 
-                                            // Reverse direction for :only-* (if we haven't yet done so)
-                                            start = dir = type === "only" && !start && "nextSibling";
-                                        }
-                                        return true;
-                                    }
+                        result += "";
 
-                                    start = [forward ? parent.firstChild : parent.lastChild];
+                        if (operator === "=") {
+                            return result === check;
+                        }
+                        if (operator === "!=") {
+                            return result !== check;
+                        }
+                        if (operator === "^=") {
+                            return check && result.indexOf(check) === 0;
+                        }
+                        if (operator === "*=") {
+                            return check && result.indexOf(check) > -1;
+                        }
+                        if (operator === "$=") {
+                            return check && result.slice(-check.length) === check;
+                        }
+                        if (operator === "~=") {
+                            return (" " + result.replace(rwhitespace, " ") + " ")
+                                .indexOf(check) > -1;
+                        }
+                        if (operator === "|=") {
+                            return result === check || result.slice(0, check.length + 1) === check + "-";
+                        }
 
-                                    // non-xml :nth-child(...) stores cache data on `parent`
-                                    if (forward && useCache) {
+                        return false;
+                    };
+                },
 
-                                        // Seek `elem` from a previously-cached index
+                CHILD: function(type, what, _argument, first, last) {
+                    var simple = type.slice(0, 3) !== "nth",
+                        forward = type.slice(-4) !== "last",
+                        ofType = what === "of-type";
+
+                    return first === 1 && last === 0 ?
+
+                        // Shortcut for :nth-*(n)
+                        function(elem) {
+                            return !!elem.parentNode;
+                        } :
 
-                                        // ...in a gzip-friendly way
-                                        node = parent;
-                                        outerCache = node[expando] || (node[expando] = {});
+                        function(elem, _context, xml) {
+                            var cache, outerCache, node, nodeIndex, start,
+                                dir = simple !== forward ? "nextSibling" : "previousSibling",
+                                parent = elem.parentNode,
+                                name = ofType && elem.nodeName.toLowerCase(),
+                                useCache = !xml && !ofType,
+                                diff = false;
+
+                            if (parent) {
+
+                                // :(first|last|only)-(child|of-type)
+                                if (simple) {
+                                    while (dir) {
+                                        node = elem;
+                                        while ((node = node[dir])) {
+                                            if (ofType ?
+                                                nodeName(node, name) :
+                                                node.nodeType === 1) {
 
-                                        // Support: IE <9 only
-                                        // Defend against cloned attroperties (jQuery gh-1709)
-                                        uniqueCache = outerCache[node.uniqueID] ||
-                                            (outerCache[node.uniqueID] = {});
+                                                return false;
+                                            }
+                                        }
 
-                                        cache = uniqueCache[type] || [];
-                                        nodeIndex = cache[0] === dirruns && cache[1];
-                                        diff = nodeIndex && cache[2];
-                                        node = nodeIndex && parent.childNodes[nodeIndex];
+                                        // Reverse direction for :only-* (if we haven't yet done so)
+                                        start = dir = type === "only" && !start && "nextSibling";
+                                    }
+                                    return true;
+                                }
 
-                                        while ((node = ++nodeIndex && node && node[dir] ||
+                                start = [forward ? parent.firstChild : parent.lastChild];
 
-                                                // Fallback to seeking `elem` from the start
-                                                (diff = nodeIndex = 0) || start.pop())) {
+                                // non-xml :nth-child(...) stores cache data on `parent`
+                                if (forward && useCache) {
 
-                                            // When found, cache indexes on `parent` and break
-                                            if (node.nodeType === 1 && ++diff && node === elem) {
-                                                uniqueCache[type] = [dirruns, nodeIndex, diff];
-                                                break;
-                                            }
+                                    // Seek `elem` from a previously-cached index
+                                    outerCache = parent[expando] || (parent[expando] = {});
+                                    cache = outerCache[type] || [];
+                                    nodeIndex = cache[0] === dirruns && cache[1];
+                                    diff = nodeIndex && cache[2];
+                                    node = nodeIndex && parent.childNodes[nodeIndex];
+
+                                    while ((node = ++nodeIndex && node && node[dir] ||
+
+                                            // Fallback to seeking `elem` from the start
+                                            (diff = nodeIndex = 0) || start.pop())) {
+
+                                        // When found, cache indexes on `parent` and break
+                                        if (node.nodeType === 1 && ++diff && node === elem) {
+                                            outerCache[type] = [dirruns, nodeIndex, diff];
+                                            break;
                                         }
+                                    }
 
-                                    } else {
+                                } else {
 
-                                        // Use previously-cached element index if available
-                                        if (useCache) {
+                                    // Use previously-cached element index if available
+                                    if (useCache) {
+                                        outerCache = elem[expando] || (elem[expando] = {});
+                                        cache = outerCache[type] || [];
+                                        nodeIndex = cache[0] === dirruns && cache[1];
+                                        diff = nodeIndex;
+                                    }
 
-                                            // ...in a gzip-friendly way
-                                            node = elem;
-                                            outerCache = node[expando] || (node[expando] = {});
-
-                                            // Support: IE <9 only
-                                            // Defend against cloned attroperties (jQuery gh-1709)
-                                            uniqueCache = outerCache[node.uniqueID] ||
-                                                (outerCache[node.uniqueID] = {});
-
-                                            cache = uniqueCache[type] || [];
-                                            nodeIndex = cache[0] === dirruns && cache[1];
-                                            diff = nodeIndex;
-                                        }
+                                    // xml :nth-child(...)
+                                    // or :nth-last-child(...) or :nth(-last)?-of-type(...)
+                                    if (diff === false) {
+
+                                        // Use the same loop as above to seek `elem` from the start
+                                        while ((node = ++nodeIndex && node && node[dir] ||
+                                                (diff = nodeIndex = 0) || start.pop())) {
 
-                                        // xml :nth-child(...)
-                                        // or :nth-last-child(...) or :nth(-last)?-of-type(...)
-                                        if (diff === false) {
-
-                                            // Use the same loop as above to seek `elem` from the start
-                                            while ((node = ++nodeIndex && node && node[dir] ||
-                                                    (diff = nodeIndex = 0) || start.pop())) {
-
-                                                if ((ofType ?
-                                                        node.nodeName.toLowerCase() === name :
-                                                        node.nodeType === 1) &&
-                                                    ++diff) {
-
-                                                    // Cache the index of each encountered element
-                                                    if (useCache) {
-                                                        outerCache = node[expando] ||
-                                                            (node[expando] = {});
-
-                                                        // Support: IE <9 only
-                                                        // Defend against cloned attroperties (jQuery gh-1709)
-                                                        uniqueCache = outerCache[node.uniqueID] ||
-                                                            (outerCache[node.uniqueID] = {});
-
-                                                        uniqueCache[type] = [dirruns, diff];
-                                                    }
-
-                                                    if (node === elem) {
-                                                        break;
-                                                    }
+                                            if ((ofType ?
+                                                    nodeName(node, name) :
+                                                    node.nodeType === 1) &&
+                                                ++diff) {
+
+                                                // Cache the index of each encountered element
+                                                if (useCache) {
+                                                    outerCache = node[expando] ||
+                                                        (node[expando] = {});
+                                                    outerCache[type] = [dirruns, diff];
+                                                }
+
+                                                if (node === elem) {
+                                                    break;
                                                 }
                                             }
                                         }
                                     }
-
-                                    // Incorporate the offset, then check against cycle size
-                                    diff -= last;
-                                    return diff === first || (diff % first === 0 && diff / first >= 0);
                                 }
-                            };
-                    },
-
-                    "PSEUDO": function(pseudo, argument) {
-
-                        // pseudo-class names are case-insensitive
-                        // http://www.w3.org/TR/selectors/#pseudo-classes
-                        // Prioritize by case sensitivity in case custom pseudos are added with uppercase letters
-                        // Remember that setFilters inherits from pseudos
-                        var args,
-                            fn = Expr.pseudos[pseudo] || Expr.setFilters[pseudo.toLowerCase()] ||
-                            Sizzle.error("unsupported pseudo: " + pseudo);
-
-                        // The user may use createPseudo to indicate that
-                        // arguments are needed to create the filter function
-                        // just as Sizzle does
-                        if (fn[expando]) {
-                            return fn(argument);
-                        }
-
-                        // But maintain support for old signatures
-                        if (fn.length > 1) {
-                            args = [pseudo, pseudo, "", argument];
-                            return Expr.setFilters.hasOwnProperty(pseudo.toLowerCase()) ?
-                                markFunction(function(seed, matches) {
-                                    var idx,
-                                        matched = fn(seed, argument),
-                                        i = matched.length;
-                                    while (i--) {
-                                        idx = indexOf(seed, matched[i]);
-                                        seed[idx] = !(matches[idx] = matched[i]);
-                                    }
-                                }) :
-                                function(elem) {
-                                    return fn(elem, 0, args);
-                                };
-                        }
 
-                        return fn;
-                    }
+                                // Incorporate the offset, then check against cycle size
+                                diff -= last;
+                                return diff === first || (diff % first === 0 && diff / first >= 0);
+                            }
+                        };
                 },
 
-                pseudos: {
-
-                    // Potentially complex pseudos
-                    "not": markFunction(function(selector) {
+                PSEUDO: function(pseudo, argument) {
 
-                        // Trim the selector passed to compile
-                        // to avoid treating leading and trailing
-                        // spaces as combinators
-                        var input = [],
-                            results = [],
-                            matcher = compile(selector.replace(rtrim, "$1"));
-
-                        return matcher[expando] ?
-                            markFunction(function(seed, matches, _context, xml) {
-                                var elem,
-                                    unmatched = matcher(seed, null, xml, []),
-                                    i = seed.length;
-
-                                // Match elements unmatched by `matcher`
+                    // pseudo-class names are case-insensitive
+                    // https://www.w3.org/TR/selectors/#pseudo-classes
+                    // Prioritize by case sensitivity in case custom pseudos are added with uppercase letters
+                    // Remember that setFilters inherits from pseudos
+                    var args,
+                        fn = Expr.pseudos[pseudo] || Expr.setFilters[pseudo.toLowerCase()] ||
+                        find.error("unsupported pseudo: " + pseudo);
+
+                    // The user may use createPseudo to indicate that
+                    // arguments are needed to create the filter function
+                    // just as jQuery does
+                    if (fn[expando]) {
+                        return fn(argument);
+                    }
+
+                    // But maintain support for old signatures
+                    if (fn.length > 1) {
+                        args = [pseudo, pseudo, "", argument];
+                        return Expr.setFilters.hasOwnProperty(pseudo.toLowerCase()) ?
+                            markFunction(function(seed, matches) {
+                                var idx,
+                                    matched = fn(seed, argument),
+                                    i = matched.length;
                                 while (i--) {
-                                    if ((elem = unmatched[i])) {
-                                        seed[i] = !(matches[i] = elem);
-                                    }
+                                    idx = indexOf.call(seed, matched[i]);
+                                    seed[idx] = !(matches[idx] = matched[i]);
                                 }
                             }) :
-                            function(elem, _context, xml) {
-                                input[0] = elem;
-                                matcher(input, null, xml, results);
-
-                                // Don't keep the element (issue #299)
-                                input[0] = null;
-                                return !results.pop();
+                            function(elem) {
+                                return fn(elem, 0, args);
                             };
-                    }),
+                    }
 
-                    "has": markFunction(function(selector) {
-                        return function(elem) {
-                            return Sizzle(selector, elem).length > 0;
-                        };
-                    }),
+                    return fn;
+                }
+            },
 
-                    "contains": markFunction(function(text) {
-                        text = text.replace(runescape, funescape);
-                        return function(elem) {
-                            return (elem.textContent || getText(elem)).indexOf(text) > -1;
-                        };
-                    }),
+            pseudos: {
+
+                // Potentially complex pseudos
+                not: markFunction(function(selector) {
 
-                    // "Whether an element is represented by a :lang() selector
-                    // is based solely on the element's language value
-                    // being equal to the identifier C,
-                    // or beginning with the identifier C immediately followed by "-".
-                    // The matching of C against the element's language value is performed case-insensitively.
-                    // The identifier C does not have to be a valid language name."
-                    // http://www.w3.org/TR/selectors/#lang-pseudo
-                    "lang": markFunction(function(lang) {
-
-                        // lang value must be a valid identifier
-                        if (!ridentifier.test(lang || "")) {
-                            Sizzle.error("unsupported lang: " + lang);
-                        }
-                        lang = lang.replace(runescape, funescape).toLowerCase();
-                        return function(elem) {
-                            var elemLang;
-                            do {
-                                if ((elemLang = documentIsHTML ?
-                                        elem.lang :
-                                        elem.getAttribute("xml:lang") || elem.getAttribute("lang"))) {
+                    // Trim the selector passed to compile
+                    // to avoid treating leading and trailing
+                    // spaces as combinators
+                    var input = [],
+                        results = [],
+                        matcher = compile(selector.replace(rtrimCSS, "$1"));
+
+                    return matcher[expando] ?
+                        markFunction(function(seed, matches, _context, xml) {
+                            var elem,
+                                unmatched = matcher(seed, null, xml, []),
+                                i = seed.length;
 
-                                    elemLang = elemLang.toLowerCase();
-                                    return elemLang === lang || elemLang.indexOf(lang + "-") === 0;
+                            // Match elements unmatched by `matcher`
+                            while (i--) {
+                                if ((elem = unmatched[i])) {
+                                    seed[i] = !(matches[i] = elem);
                                 }
-                            } while ((elem = elem.parentNode) && elem.nodeType === 1);
-                            return false;
+                            }
+                        }) :
+                        function(elem, _context, xml) {
+                            input[0] = elem;
+                            matcher(input, null, xml, results);
+
+                            // Don't keep the element
+                            // (see https://github.com/jquery/sizzle/issues/299)
+                            input[0] = null;
+                            return !results.pop();
                         };
-                    }),
+                }),
 
-                    // Miscellaneous
-                    "target": function(elem) {
-                        var hash = window.location && window.location.hash;
-                        return hash && hash.slice(1) === elem.id;
-                    },
+                has: markFunction(function(selector) {
+                    return function(elem) {
+                        return find(selector, elem).length > 0;
+                    };
+                }),
 
-                    "root": function(elem) {
-                        return elem === docElem;
-                    },
+                contains: markFunction(function(text) {
+                    text = text.replace(runescape, funescape);
+                    return function(elem) {
+                        return (elem.textContent || jQuery.text(elem)).indexOf(text) > -1;
+                    };
+                }),
 
-                    "focus": function(elem) {
-                        return elem === document.activeElement &&
-                            (!document.hasFocus || document.hasFocus()) &&
-                            !!(elem.type || elem.href || ~elem.tabIndex);
-                    },
+                // "Whether an element is represented by a :lang() selector
+                // is based solely on the element's language value
+                // being equal to the identifier C,
+                // or beginning with the identifier C immediately followed by "-".
+                // The matching of C against the element's language value is performed case-insensitively.
+                // The identifier C does not have to be a valid language name."
+                // https://www.w3.org/TR/selectors/#lang-pseudo
+                lang: markFunction(function(lang) {
+
+                    // lang value must be a valid identifier
+                    if (!ridentifier.test(lang || "")) {
+                        find.error("unsupported lang: " + lang);
+                    }
+                    lang = lang.replace(runescape, funescape).toLowerCase();
+                    return function(elem) {
+                        var elemLang;
+                        do {
+                            if ((elemLang = documentIsHTML ?
+                                    elem.lang :
+                                    elem.getAttribute("xml:lang") || elem.getAttribute("lang"))) {
 
-                    // Boolean properties
-                    "enabled": createDisabledPseudo(false),
-                    "disabled": createDisabledPseudo(true),
-
-                    "checked": function(elem) {
-
-                        // In CSS3, :checked should return both checked and selected elements
-                        // http://www.w3.org/TR/2011/REC-css3-selectors-20110929/#checked
-                        var nodeName = elem.nodeName.toLowerCase();
-                        return (nodeName === "input" && !!elem.checked) ||
-                            (nodeName === "option" && !!elem.selected);
-                    },
+                                elemLang = elemLang.toLowerCase();
+                                return elemLang === lang || elemLang.indexOf(lang + "-") === 0;
+                            }
+                        } while ((elem = elem.parentNode) && elem.nodeType === 1);
+                        return false;
+                    };
+                }),
 
-                    "selected": function(elem) {
+                // Miscellaneous
+                target: function(elem) {
+                    var hash = window.location && window.location.hash;
+                    return hash && hash.slice(1) === elem.id;
+                },
 
-                        // Accessing this property makes selected-by-default
-                        // options in Safari work properly
-                        if (elem.parentNode) {
-                            // eslint-disable-next-line no-unused-expressions
-                            elem.parentNode.selectedIndex;
-                        }
+                root: function(elem) {
+                    return elem === documentElement;
+                },
 
-                        return elem.selected === true;
-                    },
+                focus: function(elem) {
+                    return elem === safeActiveElement() &&
+                        document.hasFocus() &&
+                        !!(elem.type || elem.href || ~elem.tabIndex);
+                },
 
-                    // Contents
-                    "empty": function(elem) {
+                // Boolean properties
+                enabled: createDisabledPseudo(false),
+                disabled: createDisabledPseudo(true),
+
+                checked: function(elem) {
+
+                    // In CSS3, :checked should return both checked and selected elements
+                    // https://www.w3.org/TR/2011/REC-css3-selectors-20110929/#checked
+                    return (nodeName(elem, "input") && !!elem.checked) ||
+                        (nodeName(elem, "option") && !!elem.selected);
+                },
 
-                        // http://www.w3.org/TR/selectors/#empty-pseudo
-                        // :empty is negated by element (1) or content nodes (text: 3; cdata: 4; entity ref: 5),
-                        //   but not by others (comment: 8; processing instruction: 7; etc.)
-                        // nodeType < 6 works because attributes (2) do not appear as children
-                        for (elem = elem.firstChild; elem; elem = elem.nextSibling) {
-                            if (elem.nodeType < 6) {
-                                return false;
-                            }
+                selected: function(elem) {
+
+                    // Support: IE <=11+
+                    // Accessing the selectedIndex property
+                    // forces the browser to treat the default option as
+                    // selected when in an optgroup.
+                    if (elem.parentNode) {
+                        // eslint-disable-next-line no-unused-expressions
+                        elem.parentNode.selectedIndex;
+                    }
+
+                    return elem.selected === true;
+                },
+
+                // Contents
+                empty: function(elem) {
+
+                    // https://www.w3.org/TR/selectors/#empty-pseudo
+                    // :empty is negated by element (1) or content nodes (text: 3; cdata: 4; entity ref: 5),
+                    //   but not by others (comment: 8; processing instruction: 7; etc.)
+                    // nodeType < 6 works because attributes (2) do not appear as children
+                    for (elem = elem.firstChild; elem; elem = elem.nextSibling) {
+                        if (elem.nodeType < 6) {
+                            return false;
                         }
-                        return true;
-                    },
+                    }
+                    return true;
+                },
 
-                    "parent": function(elem) {
-                        return !Expr.pseudos["empty"](elem);
-                    },
+                parent: function(elem) {
+                    return !Expr.pseudos.empty(elem);
+                },
 
-                    // Element/input types
-                    "header": function(elem) {
-                        return rheader.test(elem.nodeName);
-                    },
+                // Element/input types
+                header: function(elem) {
+                    return rheader.test(elem.nodeName);
+                },
 
-                    "input": function(elem) {
-                        return rinputs.test(elem.nodeName);
-                    },
+                input: function(elem) {
+                    return rinputs.test(elem.nodeName);
+                },
 
-                    "button": function(elem) {
-                        var name = elem.nodeName.toLowerCase();
-                        return name === "input" && elem.type === "button" || name === "button";
-                    },
+                button: function(elem) {
+                    return nodeName(elem, "input") && elem.type === "button" ||
+                        nodeName(elem, "button");
+                },
 
-                    "text": function(elem) {
-                        var attr;
-                        return elem.nodeName.toLowerCase() === "input" &&
-                            elem.type === "text" &&
-
-                            // Support: IE<8
-                            // New HTML5 attribute values (e.g., "search") appear with elem.type === "text"
-                            ((attr = elem.getAttribute("type")) == null ||
-                                attr.toLowerCase() === "text");
-                    },
+                text: function(elem) {
+                    var attr;
+                    return nodeName(elem, "input") && elem.type === "text" &&
+
+                        // Support: IE <10 only
+                        // New HTML5 attribute values (e.g., "search") appear
+                        // with elem.type === "text"
+                        ((attr = elem.getAttribute("type")) == null ||
+                            attr.toLowerCase() === "text");
+                },
 
-                    // Position-in-collection
-                    "first": createPositionalPseudo(function() {
-                        return [0];
-                    }),
-
-                    "last": createPositionalPseudo(function(_matchIndexes, length) {
-                        return [length - 1];
-                    }),
-
-                    "eq": createPositionalPseudo(function(_matchIndexes, length, argument) {
-                        return [argument < 0 ? argument + length : argument];
-                    }),
-
-                    "even": createPositionalPseudo(function(matchIndexes, length) {
-                        var i = 0;
-                        for (; i < length; i += 2) {
-                            matchIndexes.push(i);
-                        }
-                        return matchIndexes;
-                    }),
-
-                    "odd": createPositionalPseudo(function(matchIndexes, length) {
-                        var i = 1;
-                        for (; i < length; i += 2) {
-                            matchIndexes.push(i);
-                        }
-                        return matchIndexes;
-                    }),
-
-                    "lt": createPositionalPseudo(function(matchIndexes, length, argument) {
-                        var i = argument < 0 ?
-                            argument + length :
-                            argument > length ?
-                            length :
-                            argument;
-                        for (; --i >= 0;) {
-                            matchIndexes.push(i);
-                        }
-                        return matchIndexes;
-                    }),
-
-                    "gt": createPositionalPseudo(function(matchIndexes, length, argument) {
-                        var i = argument < 0 ? argument + length : argument;
-                        for (; ++i < length;) {
-                            matchIndexes.push(i);
-                        }
-                        return matchIndexes;
-                    })
-                }
-            };
+                // Position-in-collection
+                first: createPositionalPseudo(function() {
+                    return [0];
+                }),
+
+                last: createPositionalPseudo(function(_matchIndexes, length) {
+                    return [length - 1];
+                }),
+
+                eq: createPositionalPseudo(function(_matchIndexes, length, argument) {
+                    return [argument < 0 ? argument + length : argument];
+                }),
+
+                even: createPositionalPseudo(function(matchIndexes, length) {
+                    var i = 0;
+                    for (; i < length; i += 2) {
+                        matchIndexes.push(i);
+                    }
+                    return matchIndexes;
+                }),
+
+                odd: createPositionalPseudo(function(matchIndexes, length) {
+                    var i = 1;
+                    for (; i < length; i += 2) {
+                        matchIndexes.push(i);
+                    }
+                    return matchIndexes;
+                }),
+
+                lt: createPositionalPseudo(function(matchIndexes, length, argument) {
+                    var i;
+
+                    if (argument < 0) {
+                        i = argument + length;
+                    } else if (argument > length) {
+                        i = length;
+                    } else {
+                        i = argument;
+                    }
 
-            Expr.pseudos["nth"] = Expr.pseudos["eq"];
+                    for (; --i >= 0;) {
+                        matchIndexes.push(i);
+                    }
+                    return matchIndexes;
+                }),
 
-            // Add button/input type pseudos
-            for (i in {
-                    radio: true,
-                    checkbox: true,
-                    file: true,
-                    password: true,
-                    image: true
-                }) {
-                Expr.pseudos[i] = createInputPseudo(i);
-            }
-            for (i in {
-                    submit: true,
-                    reset: true
-                }) {
-                Expr.pseudos[i] = createButtonPseudo(i);
+                gt: createPositionalPseudo(function(matchIndexes, length, argument) {
+                    var i = argument < 0 ? argument + length : argument;
+                    for (; ++i < length;) {
+                        matchIndexes.push(i);
+                    }
+                    return matchIndexes;
+                })
             }
+        };
 
-            // Easy API for creating new setFilters
-            function setFilters() {}
-            setFilters.prototype = Expr.filters = Expr.pseudos;
-            Expr.setFilters = new setFilters();
+        Expr.pseudos.nth = Expr.pseudos.eq;
 
-            tokenize = Sizzle.tokenize = function(selector, parseOnly) {
-                var matched, match, tokens, type,
-                    soFar, groups, preFilters,
-                    cached = tokenCache[selector + " "];
+        // Add button/input type pseudos
+        for (i in {
+                radio: true,
+                checkbox: true,
+                file: true,
+                password: true,
+                image: true
+            }) {
+            Expr.pseudos[i] = createInputPseudo(i);
+        }
+        for (i in {
+                submit: true,
+                reset: true
+            }) {
+            Expr.pseudos[i] = createButtonPseudo(i);
+        }
 
-                if (cached) {
-                    return parseOnly ? 0 : cached.slice(0);
-                }
+        // Easy API for creating new setFilters
+        function setFilters() {}
+        setFilters.prototype = Expr.filters = Expr.pseudos;
+        Expr.setFilters = new setFilters();
 
-                soFar = selector;
-                groups = [];
-                preFilters = Expr.preFilter;
+        function tokenize(selector, parseOnly) {
+            var matched, match, tokens, type,
+                soFar, groups, preFilters,
+                cached = tokenCache[selector + " "];
 
-                while (soFar) {
+            if (cached) {
+                return parseOnly ? 0 : cached.slice(0);
+            }
 
-                    // Comma and first run
-                    if (!matched || (match = rcomma.exec(soFar))) {
-                        if (match) {
+            soFar = selector;
+            groups = [];
+            preFilters = Expr.preFilter;
 
-                            // Don't consume trailing commas as valid
-                            soFar = soFar.slice(match[0].length) || soFar;
-                        }
-                        groups.push((tokens = []));
+            while (soFar) {
+
+                // Comma and first run
+                if (!matched || (match = rcomma.exec(soFar))) {
+                    if (match) {
+
+                        // Don't consume trailing commas as valid
+                        soFar = soFar.slice(match[0].length) || soFar;
                     }
+                    groups.push((tokens = []));
+                }
 
-                    matched = false;
+                matched = false;
+
+                // Combinators
+                if ((match = rleadingCombinator.exec(soFar))) {
+                    matched = match.shift();
+                    tokens.push({
+                        value: matched,
+
+                        // Cast descendant combinators to space
+                        type: match[0].replace(rtrimCSS, " ")
+                    });
+                    soFar = soFar.slice(matched.length);
+                }
 
-                    // Combinators
-                    if ((match = rcombinators.exec(soFar))) {
+                // Filters
+                for (type in Expr.filter) {
+                    if ((match = matchExpr[type].exec(soFar)) && (!preFilters[type] ||
+                            (match = preFilters[type](match)))) {
                         matched = match.shift();
                         tokens.push({
                             value: matched,
-
-                            // Cast descendant combinators to space
-                            type: match[0].replace(rtrim, " ")
+                            type: type,
+                            matches: match
                         });
                         soFar = soFar.slice(matched.length);
                     }
+                }
 
-                    // Filters
-                    for (type in Expr.filter) {
-                        if ((match = matchExpr[type].exec(soFar)) && (!preFilters[type] ||
-                                (match = preFilters[type](match)))) {
-                            matched = match.shift();
-                            tokens.push({
-                                value: matched,
-                                type: type,
-                                matches: match
-                            });
-                            soFar = soFar.slice(matched.length);
-                        }
-                    }
-
-                    if (!matched) {
-                        break;
-                    }
+                if (!matched) {
+                    break;
                 }
+            }
 
-                // Return the length of the invalid excess
-                // if we're just parsing
-                // Otherwise, throw an error or return tokens
-                return parseOnly ?
-                    soFar.length :
-                    soFar ?
-                    Sizzle.error(selector) :
+            // Return the length of the invalid excess
+            // if we're just parsing
+            // Otherwise, throw an error or return tokens
+            if (parseOnly) {
+                return soFar.length;
+            }
 
-                    // Cache the tokens
-                    tokenCache(selector, groups).slice(0);
-            };
+            return soFar ?
+                find.error(selector) :
 
-            function toSelector(tokens) {
-                var i = 0,
-                    len = tokens.length,
-                    selector = "";
-                for (; i < len; i++) {
-                    selector += tokens[i].value;
-                }
-                return selector;
+                // Cache the tokens
+                tokenCache(selector, groups).slice(0);
+        }
+
+        function toSelector(tokens) {
+            var i = 0,
+                len = tokens.length,
+                selector = "";
+            for (; i < len; i++) {
+                selector += tokens[i].value;
             }
+            return selector;
+        }
+
+        function addCombinator(matcher, combinator, base) {
+            var dir = combinator.dir,
+                skip = combinator.next,
+                key = skip || dir,
+                checkNonElements = base && key === "parentNode",
+                doneName = done++;
+
+            return combinator.first ?
 
-            function addCombinator(matcher, combinator, base) {
-                var dir = combinator.dir,
-                    skip = combinator.next,
-                    key = skip || dir,
-                    checkNonElements = base && key === "parentNode",
-                    doneName = done++;
+                // Check against closest ancestor/preceding element
+                function(elem, context, xml) {
+                    while ((elem = elem[dir])) {
+                        if (elem.nodeType === 1 || checkNonElements) {
+                            return matcher(elem, context, xml);
+                        }
+                    }
+                    return false;
+                } :
 
-                return combinator.first ?
+                // Check against all ancestor/preceding elements
+                function(elem, context, xml) {
+                    var oldCache, outerCache,
+                        newCache = [dirruns, doneName];
 
-                    // Check against closest ancestor/preceding element
-                    function(elem, context, xml) {
+                    // We can't set arbitrary data on XML nodes, so they don't benefit from combinator caching
+                    if (xml) {
                         while ((elem = elem[dir])) {
                             if (elem.nodeType === 1 || checkNonElements) {
-                                return matcher(elem, context, xml);
+                                if (matcher(elem, context, xml)) {
+                                    return true;
+                                }
                             }
                         }
-                        return false;
-                    } :
+                    } else {
+                        while ((elem = elem[dir])) {
+                            if (elem.nodeType === 1 || checkNonElements) {
+                                outerCache = elem[expando] || (elem[expando] = {});
 
-                    // Check against all ancestor/preceding elements
-                    function(elem, context, xml) {
-                        var oldCache, uniqueCache, outerCache,
-                            newCache = [dirruns, doneName];
-
-                        // We can't set arbitrary data on XML nodes, so they don't benefit from combinator caching
-                        if (xml) {
-                            while ((elem = elem[dir])) {
-                                if (elem.nodeType === 1 || checkNonElements) {
-                                    if (matcher(elem, context, xml)) {
-                                        return true;
-                                    }
-                                }
-                            }
-                        } else {
-                            while ((elem = elem[dir])) {
-                                if (elem.nodeType === 1 || checkNonElements) {
-                                    outerCache = elem[expando] || (elem[expando] = {});
-
-                                    // Support: IE <9 only
-                                    // Defend against cloned attroperties (jQuery gh-1709)
-                                    uniqueCache = outerCache[elem.uniqueID] ||
-                                        (outerCache[elem.uniqueID] = {});
-
-                                    if (skip && skip === elem.nodeName.toLowerCase()) {
-                                        elem = elem[dir] || elem;
-                                    } else if ((oldCache = uniqueCache[key]) &&
-                                        oldCache[0] === dirruns && oldCache[1] === doneName) {
+                                if (skip && nodeName(elem, skip)) {
+                                    elem = elem[dir] || elem;
+                                } else if ((oldCache = outerCache[key]) &&
+                                    oldCache[0] === dirruns && oldCache[1] === doneName) {
 
-                                        // Assign to newCache so results back-propagate to previous elements
-                                        return (newCache[2] = oldCache[2]);
-                                    } else {
+                                    // Assign to newCache so results back-propagate to previous elements
+                                    return (newCache[2] = oldCache[2]);
+                                } else {
 
-                                        // Reuse newcache so results back-propagate to previous elements
-                                        uniqueCache[key] = newCache;
+                                    // Reuse newcache so results back-propagate to previous elements
+                                    outerCache[key] = newCache;
 
-                                        // A match means we're done; a fail means we have to keep checking
-                                        if ((newCache[2] = matcher(elem, context, xml))) {
-                                            return true;
-                                        }
+                                    // A match means we're done; a fail means we have to keep checking
+                                    if ((newCache[2] = matcher(elem, context, xml))) {
+                                        return true;
                                     }
                                 }
                             }
                         }
-                        return false;
-                    };
-            }
+                    }
+                    return false;
+                };
+        }
 
-            function elementMatcher(matchers) {
-                return matchers.length > 1 ?
-                    function(elem, context, xml) {
-                        var i = matchers.length;
-                        while (i--) {
-                            if (!matchers[i](elem, context, xml)) {
-                                return false;
-                            }
+        function elementMatcher(matchers) {
+            return matchers.length > 1 ?
+                function(elem, context, xml) {
+                    var i = matchers.length;
+                    while (i--) {
+                        if (!matchers[i](elem, context, xml)) {
+                            return false;
                         }
-                        return true;
-                    } :
-                    matchers[0];
-            }
+                    }
+                    return true;
+                } :
+                matchers[0];
+        }
 
-            function multipleContexts(selector, contexts, results) {
-                var i = 0,
-                    len = contexts.length;
-                for (; i < len; i++) {
-                    Sizzle(selector, contexts[i], results);
-                }
-                return results;
+        function multipleContexts(selector, contexts, results) {
+            var i = 0,
+                len = contexts.length;
+            for (; i < len; i++) {
+                find(selector, contexts[i], results);
             }
+            return results;
+        }
 
-            function condense(unmatched, map, filter, context, xml) {
-                var elem,
-                    newUnmatched = [],
-                    i = 0,
-                    len = unmatched.length,
-                    mapped = map != null;
+        function condense(unmatched, map, filter, context, xml) {
+            var elem,
+                newUnmatched = [],
+                i = 0,
+                len = unmatched.length,
+                mapped = map != null;
 
-                for (; i < len; i++) {
-                    if ((elem = unmatched[i])) {
-                        if (!filter || filter(elem, context, xml)) {
-                            newUnmatched.push(elem);
-                            if (mapped) {
-                                map.push(i);
-                            }
+            for (; i < len; i++) {
+                if ((elem = unmatched[i])) {
+                    if (!filter || filter(elem, context, xml)) {
+                        newUnmatched.push(elem);
+                        if (mapped) {
+                            map.push(i);
                         }
                     }
                 }
+            }
+
+            return newUnmatched;
+        }
 
-                return newUnmatched;
+        function setMatcher(preFilter, selector, matcher, postFilter, postFinder, postSelector) {
+            if (postFilter && !postFilter[expando]) {
+                postFilter = setMatcher(postFilter);
             }
+            if (postFinder && !postFinder[expando]) {
+                postFinder = setMatcher(postFinder, postSelector);
+            }
+            return markFunction(function(seed, results, context, xml) {
+                var temp, i, elem, matcherOut,
+                    preMap = [],
+                    postMap = [],
+                    preexisting = results.length,
+
+                    // Get initial elements from seed or context
+                    elems = seed ||
+                    multipleContexts(selector || "*",
+                        context.nodeType ? [context] : context, []),
 
-            function setMatcher(preFilter, selector, matcher, postFilter, postFinder, postSelector) {
-                if (postFilter && !postFilter[expando]) {
-                    postFilter = setMatcher(postFilter);
-                }
-                if (postFinder && !postFinder[expando]) {
-                    postFinder = setMatcher(postFinder, postSelector);
-                }
-                return markFunction(function(seed, results, context, xml) {
-                    var temp, i, elem,
-                        preMap = [],
-                        postMap = [],
-                        preexisting = results.length,
-
-                        // Get initial elements from seed or context
-                        elems = seed || multipleContexts(
-                            selector || "*",
-                            context.nodeType ? [context] : context,
-                            []
-                        ),
-
-                        // Prefilter to get matcher input, preserving a map for seed-results synchronization
-                        matcherIn = preFilter && (seed || !selector) ?
-                        condense(elems, preMap, preFilter, context, xml) :
-                        elems,
+                    // Prefilter to get matcher input, preserving a map for seed-results synchronization
+                    matcherIn = preFilter && (seed || !selector) ?
+                    condense(elems, preMap, preFilter, context, xml) :
+                    elems;
 
-                        matcherOut = matcher ?
+                if (matcher) {
 
-                        // If we have a postFinder, or filtered seed, or non-seed postFilter or preexisting results,
-                        postFinder || (seed ? preFilter : preexisting || postFilter) ?
+                    // If we have a postFinder, or filtered seed, or non-seed postFilter
+                    // or preexisting results,
+                    matcherOut = postFinder || (seed ? preFilter : preexisting || postFilter) ?
 
                         // ...intermediate processing is necessary
                         [] :
 
                         // ...otherwise use results directly
-                        results :
-                        matcherIn;
+                        results;
 
                     // Find primary matches
-                    if (matcher) {
-                        matcher(matcherIn, matcherOut, context, xml);
-                    }
+                    matcher(matcherIn, matcherOut, context, xml);
+                } else {
+                    matcherOut = matcherIn;
+                }
 
-                    // Apply postFilter
-                    if (postFilter) {
-                        temp = condense(matcherOut, postMap);
-                        postFilter(temp, [], context, xml);
+                // Apply postFilter
+                if (postFilter) {
+                    temp = condense(matcherOut, postMap);
+                    postFilter(temp, [], context, xml);
 
-                        // Un-match failing elements by moving them back to matcherIn
-                        i = temp.length;
-                        while (i--) {
-                            if ((elem = temp[i])) {
-                                matcherOut[postMap[i]] = !(matcherIn[postMap[i]] = elem);
-                            }
+                    // Un-match failing elements by moving them back to matcherIn
+                    i = temp.length;
+                    while (i--) {
+                        if ((elem = temp[i])) {
+                            matcherOut[postMap[i]] = !(matcherIn[postMap[i]] = elem);
                         }
                     }
+                }
 
-                    if (seed) {
-                        if (postFinder || preFilter) {
-                            if (postFinder) {
-
-                                // Get the final matcherOut by condensing this intermediate into postFinder contexts
-                                temp = [];
-                                i = matcherOut.length;
-                                while (i--) {
-                                    if ((elem = matcherOut[i])) {
-
-                                        // Restore matcherIn since elem is not yet a final match
-                                        temp.push((matcherIn[i] = elem));
-                                    }
-                                }
-                                postFinder(null, (matcherOut = []), temp, xml);
-                            }
+                if (seed) {
+                    if (postFinder || preFilter) {
+                        if (postFinder) {
 
-                            // Move matched elements from seed to results to keep them synchronized
+                            // Get the final matcherOut by condensing this intermediate into postFinder contexts
+                            temp = [];
                             i = matcherOut.length;
                             while (i--) {
-                                if ((elem = matcherOut[i]) &&
-                                    (temp = postFinder ? indexOf(seed, elem) : preMap[i]) > -1) {
+                                if ((elem = matcherOut[i])) {
 
-                                    seed[temp] = !(results[temp] = elem);
+                                    // Restore matcherIn since elem is not yet a final match
+                                    temp.push((matcherIn[i] = elem));
                                 }
                             }
+                            postFinder(null, (matcherOut = []), temp, xml);
                         }
 
-                        // Add elements to results, through postFinder if defined
-                    } else {
-                        matcherOut = condense(
-                            matcherOut === results ?
-                            matcherOut.splice(preexisting, matcherOut.length) :
-                            matcherOut
-                        );
-                        if (postFinder) {
-                            postFinder(null, results, matcherOut, xml);
-                        } else {
-                            push.apply(results, matcherOut);
+                        // Move matched elements from seed to results to keep them synchronized
+                        i = matcherOut.length;
+                        while (i--) {
+                            if ((elem = matcherOut[i]) &&
+                                (temp = postFinder ? indexOf.call(seed, elem) : preMap[i]) > -1) {
+
+                                seed[temp] = !(results[temp] = elem);
+                            }
                         }
                     }
-                });
-            }
 
-            function matcherFromTokens(tokens) {
-                var checkContext, matcher, j,
-                    len = tokens.length,
-                    leadingRelative = Expr.relative[tokens[0].type],
-                    implicitRelative = leadingRelative || Expr.relative[" "],
-                    i = leadingRelative ? 1 : 0,
-
-                    // The foundational matcher ensures that elements are reachable from top-level context(s)
-                    matchContext = addCombinator(function(elem) {
-                        return elem === checkContext;
-                    }, implicitRelative, true),
-                    matchAnyContext = addCombinator(function(elem) {
-                        return indexOf(checkContext, elem) > -1;
-                    }, implicitRelative, true),
-                    matchers = [function(elem, context, xml) {
-                        var ret = (!leadingRelative && (xml || context !== outermostContext)) || (
-                            (checkContext = context).nodeType ?
-                            matchContext(elem, context, xml) :
-                            matchAnyContext(elem, context, xml));
+                    // Add elements to results, through postFinder if defined
+                } else {
+                    matcherOut = condense(
+                        matcherOut === results ?
+                        matcherOut.splice(preexisting, matcherOut.length) :
+                        matcherOut
+                    );
+                    if (postFinder) {
+                        postFinder(null, results, matcherOut, xml);
+                    } else {
+                        push.apply(results, matcherOut);
+                    }
+                }
+            });
+        }
 
-                        // Avoid hanging onto element (issue #299)
-                        checkContext = null;
-                        return ret;
-                    }];
+        function matcherFromTokens(tokens) {
+            var checkContext, matcher, j,
+                len = tokens.length,
+                leadingRelative = Expr.relative[tokens[0].type],
+                implicitRelative = leadingRelative || Expr.relative[" "],
+                i = leadingRelative ? 1 : 0,
+
+                // The foundational matcher ensures that elements are reachable from top-level context(s)
+                matchContext = addCombinator(function(elem) {
+                    return elem === checkContext;
+                }, implicitRelative, true),
+                matchAnyContext = addCombinator(function(elem) {
+                    return indexOf.call(checkContext, elem) > -1;
+                }, implicitRelative, true),
+                matchers = [function(elem, context, xml) {
+
+                    // Support: IE 11+, Edge 17 - 18+
+                    // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                    // two documents; shallow comparisons work.
+                    // eslint-disable-next-line eqeqeq
+                    var ret = (!leadingRelative && (xml || context != outermostContext)) || (
+                        (checkContext = context).nodeType ?
+                        matchContext(elem, context, xml) :
+                        matchAnyContext(elem, context, xml));
+
+                    // Avoid hanging onto element
+                    // (see https://github.com/jquery/sizzle/issues/299)
+                    checkContext = null;
+                    return ret;
+                }];
 
-                for (; i < len; i++) {
-                    if ((matcher = Expr.relative[tokens[i].type])) {
-                        matchers = [addCombinator(elementMatcher(matchers), matcher)];
-                    } else {
-                        matcher = Expr.filter[tokens[i].type].apply(null, tokens[i].matches);
+            for (; i < len; i++) {
+                if ((matcher = Expr.relative[tokens[i].type])) {
+                    matchers = [addCombinator(elementMatcher(matchers), matcher)];
+                } else {
+                    matcher = Expr.filter[tokens[i].type].apply(null, tokens[i].matches);
 
-                        // Return special upon seeing a positional matcher
-                        if (matcher[expando]) {
+                    // Return special upon seeing a positional matcher
+                    if (matcher[expando]) {
 
-                            // Find the next relative operator (if any) for proper handling
-                            j = ++i;
-                            for (; j < len; j++) {
-                                if (Expr.relative[tokens[j].type]) {
-                                    break;
-                                }
+                        // Find the next relative operator (if any) for proper handling
+                        j = ++i;
+                        for (; j < len; j++) {
+                            if (Expr.relative[tokens[j].type]) {
+                                break;
                             }
-                            return setMatcher(
-                                i > 1 && elementMatcher(matchers),
-                                i > 1 && toSelector(
-
-                                    // If the preceding token was a descendant combinator, insert an implicit any-element `*`
-                                    tokens
-                                    .slice(0, i - 1)
-                                    .concat({
-                                        value: tokens[i - 2].type === " " ? "*" : ""
-                                    })
-                                ).replace(rtrim, "$1"),
-                                matcher,
-                                i < j && matcherFromTokens(tokens.slice(i, j)),
-                                j < len && matcherFromTokens((tokens = tokens.slice(j))),
-                                j < len && toSelector(tokens)
-                            );
                         }
-                        matchers.push(matcher);
+                        return setMatcher(
+                            i > 1 && elementMatcher(matchers),
+                            i > 1 && toSelector(
+
+                                // If the preceding token was a descendant combinator, insert an implicit any-element `*`
+                                tokens.slice(0, i - 1)
+                                .concat({
+                                    value: tokens[i - 2].type === " " ? "*" : ""
+                                })
+                            ).replace(rtrimCSS, "$1"),
+                            matcher,
+                            i < j && matcherFromTokens(tokens.slice(i, j)),
+                            j < len && matcherFromTokens((tokens = tokens.slice(j))),
+                            j < len && toSelector(tokens)
+                        );
                     }
+                    matchers.push(matcher);
                 }
-
-                return elementMatcher(matchers);
             }
 
-            function matcherFromGroupMatchers(elementMatchers, setMatchers) {
-                var bySet = setMatchers.length > 0,
-                    byElement = elementMatchers.length > 0,
-                    superMatcher = function(seed, context, xml, results, outermost) {
-                        var elem, j, matcher,
-                            matchedCount = 0,
-                            i = "0",
-                            unmatched = seed && [],
-                            setMatched = [],
-                            contextBackup = outermostContext,
+            return elementMatcher(matchers);
+        }
+
+        function matcherFromGroupMatchers(elementMatchers, setMatchers) {
+            var bySet = setMatchers.length > 0,
+                byElement = elementMatchers.length > 0,
+                superMatcher = function(seed, context, xml, results, outermost) {
+                    var elem, j, matcher,
+                        matchedCount = 0,
+                        i = "0",
+                        unmatched = seed && [],
+                        setMatched = [],
+                        contextBackup = outermostContext,
+
+                        // We must always have either seed elements or outermost context
+                        elems = seed || byElement && Expr.find.TAG("*", outermost),
 
-                            // We must always have either seed elements or outermost context
-                            elems = seed || byElement && Expr.find["TAG"]("*", outermost),
+                        // Use integer dirruns iff this is the outermost matcher
+                        dirrunsUnique = (dirruns += contextBackup == null ? 1 : Math.random() || 0.1),
+                        len = elems.length;
 
-                            // Use integer dirruns iff this is the outermost matcher
-                            dirrunsUnique = (dirruns += contextBackup == null ? 1 : Math.random() || 0.1),
-                            len = elems.length;
+                    if (outermost) {
 
-                        if (outermost) {
+                        // Support: IE 11+, Edge 17 - 18+
+                        // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                        // two documents; shallow comparisons work.
+                        // eslint-disable-next-line eqeqeq
+                        outermostContext = context == document || context || outermost;
+                    }
+
+                    // Add elements passing elementMatchers directly to results
+                    // Support: iOS <=7 - 9 only
+                    // Tolerate NodeList properties (IE: "length"; Safari: <number>) matching
+                    // elements by id. (see trac-14142)
+                    for (; i !== len && (elem = elems[i]) != null; i++) {
+                        if (byElement && elem) {
+                            j = 0;
 
                             // Support: IE 11+, Edge 17 - 18+
                             // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
                             // two documents; shallow comparisons work.
                             // eslint-disable-next-line eqeqeq
-                            outermostContext = context == document || context || outermost;
-                        }
-
-                        // Add elements passing elementMatchers directly to results
-                        // Support: IE<9, Safari
-                        // Tolerate NodeList properties (IE: "length"; Safari: <number>) matching elements by id
-                        for (; i !== len && (elem = elems[i]) != null; i++) {
-                            if (byElement && elem) {
-                                j = 0;
-
-                                // Support: IE 11+, Edge 17 - 18+
-                                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
-                                // two documents; shallow comparisons work.
-                                // eslint-disable-next-line eqeqeq
-                                if (!context && elem.ownerDocument != document) {
-                                    setDocument(elem);
-                                    xml = !documentIsHTML;
-                                }
-                                while ((matcher = elementMatchers[j++])) {
-                                    if (matcher(elem, context || document, xml)) {
-                                        results.push(elem);
-                                        break;
-                                    }
-                                }
-                                if (outermost) {
-                                    dirruns = dirrunsUnique;
+                            if (!context && elem.ownerDocument != document) {
+                                setDocument(elem);
+                                xml = !documentIsHTML;
+                            }
+                            while ((matcher = elementMatchers[j++])) {
+                                if (matcher(elem, context || document, xml)) {
+                                    push.call(results, elem);
+                                    break;
                                 }
                             }
-
-                            // Track unmatched elements for set filters
-                            if (bySet) {
-
-                                // They will have gone through all possible matchers
-                                if ((elem = !matcher && elem)) {
-                                    matchedCount--;
-                                }
-
-                                // Lengthen the array for every element, matched or not
-                                if (seed) {
-                                    unmatched.push(elem);
-                                }
+                            if (outermost) {
+                                dirruns = dirrunsUnique;
                             }
                         }
 
-                        // `i` is now the count of elements visited above, and adding it to `matchedCount`
-                        // makes the latter nonnegative.
-                        matchedCount += i;
-
-                        // Apply set filters to unmatched elements
-                        // NOTE: This can be skipped if there are no unmatched elements (i.e., `matchedCount`
-                        // equals `i`), unless we didn't visit _any_ elements in the above loop because we have
-                        // no element matchers and no seed.
-                        // Incrementing an initially-string "0" `i` allows `i` to remain a string only in that
-                        // case, which will result in a "00" `matchedCount` that differs from `i` but is also
-                        // numerically zero.
-                        if (bySet && i !== matchedCount) {
-                            j = 0;
-                            while ((matcher = setMatchers[j++])) {
-                                matcher(unmatched, setMatched, context, xml);
-                            }
-
-                            if (seed) {
+                        // Track unmatched elements for set filters
+                        if (bySet) {
 
-                                // Reintegrate element matches to eliminate the need for sorting
-                                if (matchedCount > 0) {
-                                    while (i--) {
-                                        if (!(unmatched[i] || setMatched[i])) {
-                                            setMatched[i] = pop.call(results);
-                                        }
-                                    }
-                                }
-
-                                // Discard index placeholder values to get only actual matches
-                                setMatched = condense(setMatched);
+                            // They will have gone through all possible matchers
+                            if ((elem = !matcher && elem)) {
+                                matchedCount--;
                             }
 
-                            // Add matches to results
-                            push.apply(results, setMatched);
-
-                            // Seedless set matches succeeding multiple successful matchers stipulate sorting
-                            if (outermost && !seed && setMatched.length > 0 &&
-                                (matchedCount + setMatchers.length) > 1) {
-
-                                Sizzle.uniqueSort(results);
+                            // Lengthen the array for every element, matched or not
+                            if (seed) {
+                                unmatched.push(elem);
                             }
                         }
+                    }
 
-                        // Override manipulation of globals by nested matchers
-                        if (outermost) {
-                            dirruns = dirrunsUnique;
-                            outermostContext = contextBackup;
-                        }
+                    // `i` is now the count of elements visited above, and adding it to `matchedCount`
+                    // makes the latter nonnegative.
+                    matchedCount += i;
 
-                        return unmatched;
-                    };
-
-                return bySet ?
-                    markFunction(superMatcher) :
-                    superMatcher;
-            }
+                    // Apply set filters to unmatched elements
+                    // NOTE: This can be skipped if there are no unmatched elements (i.e., `matchedCount`
+                    // equals `i`), unless we didn't visit _any_ elements in the above loop because we have
+                    // no element matchers and no seed.
+                    // Incrementing an initially-string "0" `i` allows `i` to remain a string only in that
+                    // case, which will result in a "00" `matchedCount` that differs from `i` but is also
+                    // numerically zero.
+                    if (bySet && i !== matchedCount) {
+                        j = 0;
+                        while ((matcher = setMatchers[j++])) {
+                            matcher(unmatched, setMatched, context, xml);
+                        }
 
-            compile = Sizzle.compile = function(selector, match /* Internal Use Only */ ) {
-                var i,
-                    setMatchers = [],
-                    elementMatchers = [],
-                    cached = compilerCache[selector + " "];
+                        if (seed) {
 
-                if (!cached) {
+                            // Reintegrate element matches to eliminate the need for sorting
+                            if (matchedCount > 0) {
+                                while (i--) {
+                                    if (!(unmatched[i] || setMatched[i])) {
+                                        setMatched[i] = pop.call(results);
+                                    }
+                                }
+                            }
 
-                    // Generate a function of recursive functions that can be used to check each element
-                    if (!match) {
-                        match = tokenize(selector);
-                    }
-                    i = match.length;
-                    while (i--) {
-                        cached = matcherFromTokens(match[i]);
-                        if (cached[expando]) {
-                            setMatchers.push(cached);
-                        } else {
-                            elementMatchers.push(cached);
+                            // Discard index placeholder values to get only actual matches
+                            setMatched = condense(setMatched);
                         }
-                    }
 
-                    // Cache the compiled function
-                    cached = compilerCache(
-                        selector,
-                        matcherFromGroupMatchers(elementMatchers, setMatchers)
-                    );
+                        // Add matches to results
+                        push.apply(results, setMatched);
 
-                    // Save selector and tokenization
-                    cached.selector = selector;
-                }
-                return cached;
-            };
+                        // Seedless set matches succeeding multiple successful matchers stipulate sorting
+                        if (outermost && !seed && setMatched.length > 0 &&
+                            (matchedCount + setMatchers.length) > 1) {
 
-            /**
-             * A low-level selection function that works with Sizzle's compiled
-             *  selector functions
-             * @param {String|Function} selector A selector or a pre-compiled
-             *  selector function built with Sizzle.compile
-             * @param {Element} context
-             * @param {Array} [results]
-             * @param {Array} [seed] A set of elements to match against
-             */
-            select = Sizzle.select = function(selector, context, results, seed) {
-                var i, tokens, token, type, find,
-                    compiled = typeof selector === "function" && selector,
-                    match = !seed && tokenize((selector = compiled.selector || selector));
-
-                results = results || [];
-
-                // Try to minimize operations if there is only one selector in the list and no seed
-                // (the latter of which guarantees us context)
-                if (match.length === 1) {
-
-                    // Reduce context if the leading compound selector is an ID
-                    tokens = match[0] = match[0].slice(0);
-                    if (tokens.length > 2 && (token = tokens[0]).type === "ID" &&
-                        context.nodeType === 9 && documentIsHTML && Expr.relative[tokens[1].type]) {
-
-                        context = (Expr.find["ID"](token.matches[0]
-                            .replace(runescape, funescape), context) || [])[0];
-                        if (!context) {
-                            return results;
-
-                            // Precompiled matchers will still verify ancestry, so step up a level
-                        } else if (compiled) {
-                            context = context.parentNode;
+                            jQuery.uniqueSort(results);
                         }
+                    }
 
-                        selector = selector.slice(tokens.shift().value.length);
+                    // Override manipulation of globals by nested matchers
+                    if (outermost) {
+                        dirruns = dirrunsUnique;
+                        outermostContext = contextBackup;
                     }
 
-                    // Fetch a seed set for right-to-left matching
-                    i = matchExpr["needsContext"].test(selector) ? 0 : tokens.length;
-                    while (i--) {
-                        token = tokens[i];
+                    return unmatched;
+                };
 
-                        // Abort if we hit a combinator
-                        if (Expr.relative[(type = token.type)]) {
-                            break;
-                        }
-                        if ((find = Expr.find[type])) {
+            return bySet ?
+                markFunction(superMatcher) :
+                superMatcher;
+        }
 
-                            // Search, expanding context for leading sibling combinators
-                            if ((seed = find(
-                                    token.matches[0].replace(runescape, funescape),
-                                    rsibling.test(tokens[0].type) && testContext(context.parentNode) ||
-                                    context
-                                ))) {
-
-                                // If seed is empty or no tokens remain, we can return early
-                                tokens.splice(i, 1);
-                                selector = seed.length && toSelector(tokens);
-                                if (!selector) {
-                                    push.apply(results, seed);
-                                    return results;
-                                }
+        function compile(selector, match /* Internal Use Only */ ) {
+            var i,
+                setMatchers = [],
+                elementMatchers = [],
+                cached = compilerCache[selector + " "];
 
-                                break;
-                            }
-                        }
+            if (!cached) {
+
+                // Generate a function of recursive functions that can be used to check each element
+                if (!match) {
+                    match = tokenize(selector);
+                }
+                i = match.length;
+                while (i--) {
+                    cached = matcherFromTokens(match[i]);
+                    if (cached[expando]) {
+                        setMatchers.push(cached);
+                    } else {
+                        elementMatchers.push(cached);
                     }
                 }
 
-                // Compile and execute a filtering function if one is not provided
-                // Provide `match` to avoid retokenization if we modified the selector above
-                (compiled || compile(selector, match))(
-                    seed,
-                    context,
-                    !documentIsHTML,
-                    results,
-                    !context || rsibling.test(selector) && testContext(context.parentNode) || context
-                );
-                return results;
-            };
+                // Cache the compiled function
+                cached = compilerCache(selector,
+                    matcherFromGroupMatchers(elementMatchers, setMatchers));
 
-            // One-time assignments
-
-            // Sort stability
-            support.sortStable = expando.split("").sort(sortOrder).join("") === expando;
+                // Save selector and tokenization
+                cached.selector = selector;
+            }
+            return cached;
+        }
 
-            // Support: Chrome 14-35+
-            // Always assume duplicates if they aren't passed to the comparison function
-            support.detectDuplicates = !!hasDuplicate;
+        /**
+         * A low-level selection function that works with jQuery's compiled
+         *  selector functions
+         * @param {String|Function} selector A selector or a pre-compiled
+         *  selector function built with jQuery selector compile
+         * @param {Element} context
+         * @param {Array} [results]
+         * @param {Array} [seed] A set of elements to match against
+         */
+        function select(selector, context, results, seed) {
+            var i, tokens, token, type, find,
+                compiled = typeof selector === "function" && selector,
+                match = !seed && tokenize((selector = compiled.selector || selector));
+
+            results = results || [];
+
+            // Try to minimize operations if there is only one selector in the list and no seed
+            // (the latter of which guarantees us context)
+            if (match.length === 1) {
+
+                // Reduce context if the leading compound selector is an ID
+                tokens = match[0] = match[0].slice(0);
+                if (tokens.length > 2 && (token = tokens[0]).type === "ID" &&
+                    context.nodeType === 9 && documentIsHTML && Expr.relative[tokens[1].type]) {
+
+                    context = (Expr.find.ID(
+                        token.matches[0].replace(runescape, funescape),
+                        context
+                    ) || [])[0];
+                    if (!context) {
+                        return results;
 
-            // Initialize against the default document
-            setDocument();
+                        // Precompiled matchers will still verify ancestry, so step up a level
+                    } else if (compiled) {
+                        context = context.parentNode;
+                    }
 
-            // Support: Webkit<537.32 - Safari 6.0.3/Chrome 25 (fixed in Chrome 27)
-            // Detached nodes confoundingly follow *each other*
-            support.sortDetached = assert(function(el) {
+                    selector = selector.slice(tokens.shift().value.length);
+                }
 
-                // Should return 1, but returns 4 (following)
-                return el.compareDocumentPosition(document.createElement("fieldset")) & 1;
-            });
+                // Fetch a seed set for right-to-left matching
+                i = matchExpr.needsContext.test(selector) ? 0 : tokens.length;
+                while (i--) {
+                    token = tokens[i];
 
-            // Support: IE<8
-            // Prevent attribute/property "interpolation"
-            // https://msdn.microsoft.com/en-us/library/ms536429%28VS.85%29.aspx
-            if (!assert(function(el) {
-                    el.innerHTML = "<a href='#'></a>";
-                    return el.firstChild.getAttribute("href") === "#";
-                })) {
-                addHandle("type|href|height|width", function(elem, name, isXML) {
-                    if (!isXML) {
-                        return elem.getAttribute(name, name.toLowerCase() === "type" ? 1 : 2);
+                    // Abort if we hit a combinator
+                    if (Expr.relative[(type = token.type)]) {
+                        break;
                     }
-                });
-            }
+                    if ((find = Expr.find[type])) {
 
-            // Support: IE<9
-            // Use defaultValue in place of getAttribute("value")
-            if (!support.attributes || !assert(function(el) {
-                    el.innerHTML = "<input/>";
-                    el.firstChild.setAttribute("value", "");
-                    return el.firstChild.getAttribute("value") === "";
-                })) {
-                addHandle("value", function(elem, _name, isXML) {
-                    if (!isXML && elem.nodeName.toLowerCase() === "input") {
-                        return elem.defaultValue;
-                    }
-                });
-            }
+                        // Search, expanding context for leading sibling combinators
+                        if ((seed = find(
+                                token.matches[0].replace(runescape, funescape),
+                                rsibling.test(tokens[0].type) &&
+                                testContext(context.parentNode) || context
+                            ))) {
+
+                            // If seed is empty or no tokens remain, we can return early
+                            tokens.splice(i, 1);
+                            selector = seed.length && toSelector(tokens);
+                            if (!selector) {
+                                push.apply(results, seed);
+                                return results;
+                            }
 
-            // Support: IE<9
-            // Use getAttributeNode to fetch booleans when getAttribute lies
-            if (!assert(function(el) {
-                    return el.getAttribute("disabled") == null;
-                })) {
-                addHandle(booleans, function(elem, name, isXML) {
-                    var val;
-                    if (!isXML) {
-                        return elem[name] === true ? name.toLowerCase() :
-                            (val = elem.getAttributeNode(name)) && val.specified ?
-                            val.value :
-                            null;
+                            break;
+                        }
                     }
-                });
+                }
             }
 
-            return Sizzle;
+            // Compile and execute a filtering function if one is not provided
+            // Provide `match` to avoid retokenization if we modified the selector above
+            (compiled || compile(selector, match))(
+                seed,
+                context,
+                !documentIsHTML,
+                results,
+                !context || rsibling.test(selector) && testContext(context.parentNode) || context
+            );
+            return results;
+        }
 
-        })(window);
+        // One-time assignments
 
+        // Support: Android <=4.0 - 4.1+
+        // Sort stability
+        support.sortStable = expando.split("").sort(sortOrder).join("") === expando;
 
+        // Initialize against the default document
+        setDocument();
 
-    jQuery.find = Sizzle;
-    jQuery.expr = Sizzle.selectors;
+        // Support: Android <=4.0 - 4.1+
+        // Detached nodes confoundingly follow *each other*
+        support.sortDetached = assert(function(el) {
 
-    // Deprecated
-    jQuery.expr[":"] = jQuery.expr.pseudos;
-    jQuery.uniqueSort = jQuery.unique = Sizzle.uniqueSort;
-    jQuery.text = Sizzle.getText;
-    jQuery.isXMLDoc = Sizzle.isXML;
-    jQuery.contains = Sizzle.contains;
-    jQuery.escapeSelector = Sizzle.escape;
+            // Should return 1, but returns 4 (following)
+            return el.compareDocumentPosition(document.createElement("fieldset")) & 1;
+        });
 
+        jQuery.find = find;
 
+        // Deprecated
+        jQuery.expr[":"] = jQuery.expr.pseudos;
+        jQuery.unique = jQuery.uniqueSort;
+
+        // These have always been private, but they used to be documented
+        // as part of Sizzle so let's maintain them in the 3.x line
+        // for backwards compatibility purposes.
+        find.compile = compile;
+        find.select = select;
+        find.setDocument = setDocument;
+
+        find.escape = jQuery.escapeSelector;
+        find.getText = jQuery.text;
+        find.isXML = jQuery.isXMLDoc;
+        find.selectors = jQuery.expr;
+        find.support = jQuery.support;
+        find.uniqueSort = jQuery.uniqueSort;
+
+        /* eslint-enable */
+
+    })();
 
 
     var dir = function(elem, dir, until) {
         var matched = [],
             truncate = until !== undefined;
 
         while ((elem = elem[dir]) && elem.nodeType !== 9) {
@@ -3046,21 +2764,14 @@
 
         return matched;
     };
 
 
     var rneedsContext = jQuery.expr.match.needsContext;
 
-
-
-    function nodeName(elem, name) {
-
-        return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
-
-    }
     var rsingleTag = (/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i);
 
 
 
     // Implement the identical functionality for filter and not
     function winnow(elements, qualifier, not) {
         if (isFunction(qualifier)) {
@@ -3151,16 +2862,16 @@
     // Initialize a jQuery object
 
 
     // A central reference to the root jQuery(document)
     var rootjQuery,
 
         // A simple way to check for HTML strings
-        // Prioritize #id over <tag> to avoid XSS via location.hash (#9521)
-        // Strict HTML recognition (#11290: must start with <)
+        // Prioritize #id over <tag> to avoid XSS via location.hash (trac-9521)
+        // Strict HTML recognition (trac-11290: must start with <)
         // Shortcut simple #id case for speed
         rquickExpr = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/,
 
         init = jQuery.fn.init = function(selector, context, root) {
             var match, elem;
 
             // HANDLE: $(""), $(null), $(undefined), $(false)
@@ -3303,15 +3014,15 @@
                 for (; i < l; i++) {
                     for (cur = this[i]; cur && cur !== context; cur = cur.parentNode) {
 
                         // Always skip document fragments
                         if (cur.nodeType < 11 && (targets ?
                                 targets.index(cur) > -1 :
 
-                                // Don't pass non-elements to Sizzle
+                                // Don't pass non-elements to jQuery#find
                                 cur.nodeType === 1 &&
                                 jQuery.find.matchesSelector(cur, selectors))) {
 
                             matched.push(cur);
                             break;
                         }
                     }
@@ -3863,15 +3574,15 @@
                                     function() {
                                         try {
                                             mightThrow();
                                         } catch (e) {
 
                                             if (jQuery.Deferred.exceptionHook) {
                                                 jQuery.Deferred.exceptionHook(e,
-                                                    process.stackTrace);
+                                                    process.error);
                                             }
 
                                             // Support: Promises/A+ section 2.3.3.3.4.1
                                             // https://promisesaplus.com/#point-61
                                             // Ignore post-resolution exceptions
                                             if (depth + 1 >= maxDepth) {
 
@@ -3891,18 +3602,25 @@
                                 // https://promisesaplus.com/#point-57
                                 // Re-resolve promises immediately to dodge false rejection from
                                 // subsequent errors
                                 if (depth) {
                                     process();
                                 } else {
 
-                                    // Call an optional hook to record the stack, in case of exception
+                                    // Call an optional hook to record the error, in case of exception
                                     // since it's otherwise lost when execution goes async
-                                    if (jQuery.Deferred.getStackHook) {
-                                        process.stackTrace = jQuery.Deferred.getStackHook();
+                                    if (jQuery.Deferred.getErrorHook) {
+                                        process.error = jQuery.Deferred.getErrorHook();
+
+                                        // The deprecated alias of the above. While the name suggests
+                                        // returning the stack, not an error instance, jQuery just passes
+                                        // it directly to `console.warn` so both will work; an instance
+                                        // just better cooperates with source maps.
+                                    } else if (jQuery.Deferred.getStackHook) {
+                                        process.error = jQuery.Deferred.getStackHook();
                                     }
                                     window.setTimeout(process);
                                 }
                             };
                         }
 
                         return jQuery.Deferred(function(newDefer) {
@@ -4069,20 +3787,24 @@
     });
 
 
     // These usually indicate a programmer mistake during development,
     // warn about them ASAP rather than swallowing them by default.
     var rerrorNames = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
 
-    jQuery.Deferred.exceptionHook = function(error, stack) {
+    // If `jQuery.Deferred.getErrorHook` is defined, `asyncError` is an error
+    // captured before the async barrier to get the original error cause
+    // which may otherwise be hidden.
+    jQuery.Deferred.exceptionHook = function(error, asyncError) {
 
         // Support: IE 8 - 9 only
         // Console exists when dev tools are open, which can happen at any time
         if (window.console && window.console.warn && error && rerrorNames.test(error.name)) {
-            window.console.warn("jQuery.Deferred exception: " + error.message, error.stack, stack);
+            window.console.warn("jQuery.Deferred exception: " + error.message,
+                error.stack, asyncError);
         }
     };
 
 
 
 
     jQuery.readyException = function(error) {
@@ -4114,15 +3836,15 @@
 
     jQuery.extend({
 
         // Is the DOM ready to be used? Set to true once it occurs.
         isReady: false,
 
         // A counter to track how many items to wait for before
-        // the ready event fires. See #6781
+        // the ready event fires. See trac-6781
         readyWait: 1,
 
         // Handle when the DOM is ready
         ready: function(wait) {
 
             // Abort if there are pending holds or we're already ready
             if (wait === true ? --jQuery.readyWait : jQuery.isReady) {
@@ -4242,15 +3964,15 @@
     // Used by camelCase as callback to replace()
     function fcamelCase(_all, letter) {
         return letter.toUpperCase();
     }
 
     // Convert dashed to camelCase; used by the css and data modules
     // Support: IE <=9 - 11, Edge 12 - 15
-    // Microsoft forgot to hump their vendor prefix (#9572)
+    // Microsoft forgot to hump their vendor prefix (trac-9572)
     function camelCase(string) {
         return string.replace(rmsPrefix, "ms-").replace(rdashAlpha, fcamelCase);
     }
     var acceptData = function(owner) {
 
         // Accepts only:
         //  - Node
@@ -4278,15 +4000,15 @@
             var value = owner[this.expando];
 
             // If not, create one
             if (!value) {
                 value = {};
 
                 // We can accept data for non-element nodes in modern browsers,
-                // but we should not, see #8335.
+                // but we should not, see trac-8335.
                 // Always return an empty object.
                 if (acceptData(owner)) {
 
                     // If it is a node unlikely to be stringify-ed or looped over
                     // use plain assignment
                     if (owner.nodeType) {
                         owner[this.expando] = value;
@@ -4516,15 +4238,15 @@
                     data = dataUser.get(elem);
 
                     if (elem.nodeType === 1 && !dataPriv.get(elem, "hasDataAttrs")) {
                         i = attrs.length;
                         while (i--) {
 
                             // Support: IE 11 only
-                            // The attrs elements can be null (#14894)
+                            // The attrs elements can be null (trac-14894)
                             if (attrs[i]) {
                                 name = attrs[i].name;
                                 if (name.indexOf("data-") === 0) {
                                     name = camelCase(name.slice(5));
                                     dataAttr(elem, name, data[name]);
                                 }
                             }
@@ -4941,17 +4663,17 @@
 
     (function() {
         var fragment = document.createDocumentFragment(),
             div = fragment.appendChild(document.createElement("div")),
             input = document.createElement("input");
 
         // Support: Android 4.0 - 4.3 only
-        // Check state lost if the name is set (#11217)
+        // Check state lost if the name is set (trac-11217)
         // Support: Windows Web Apps (WWA)
-        // `name` and `type` must use .setAttribute for WWA (#14901)
+        // `name` and `type` must use .setAttribute for WWA (trac-14901)
         input.setAttribute("type", "radio");
         input.setAttribute("checked", "checked");
         input.setAttribute("name", "t");
 
         div.appendChild(input);
 
         // Support: Android <=4.1 only
@@ -4967,15 +4689,15 @@
         // IE <=9 replaces <option> tags with their contents when inserted outside of
         // the select element.
         div.innerHTML = "<option></option>";
         support.option = !!div.lastChild;
     })();
 
 
-    // We have to close these tags to support XHTML (#13200)
+    // We have to close these tags to support XHTML (trac-13200)
     var wrapMap = {
 
         // XHTML parsers do not magically insert elements in the
         // same way that tag soup parsers do. So we cannot shorten
         // this by omitting <tbody> or other required elements.
         thead: [1, "<table>", "</table>"],
         col: [2, "<table><colgroup>", "</colgroup></table>"],
@@ -4993,15 +4715,15 @@
         wrapMap.optgroup = wrapMap.option = [1, "<select multiple='multiple'>", "</select>"];
     }
 
 
     function getAll(context, tag) {
 
         // Support: IE <=9 - 11 only
-        // Use typeof to avoid zero-argument method invocation on host objects (#15151)
+        // Use typeof to avoid zero-argument method invocation on host objects (trac-15151)
         var ret;
 
         if (typeof context.getElementsByTagName !== "undefined") {
             ret = context.getElementsByTagName(tag || "*");
 
         } else if (typeof context.querySelectorAll !== "undefined") {
             ret = context.querySelectorAll(tag || "*");
@@ -5076,15 +4798,15 @@
                     // Support: Android <=4.0 only, PhantomJS 1 only
                     // push.apply(_, arraylike) throws on ancient WebKit
                     jQuery.merge(nodes, tmp.childNodes);
 
                     // Remember the top-level container
                     tmp = fragment.firstChild;
 
-                    // Ensure the created nodes are orphaned (#12392)
+                    // Ensure the created nodes are orphaned (trac-12392)
                     tmp.textContent = "";
                 }
             }
         }
 
         // Remove wrapper from fragment
         fragment.textContent = "";
@@ -5131,33 +4853,14 @@
         return true;
     }
 
     function returnFalse() {
         return false;
     }
 
-    // Support: IE <=9 - 11+
-    // focus() and blur() are asynchronous, except when they are no-op.
-    // So expect focus to be synchronous when the element is already active,
-    // and blur to be synchronous when the element is not already active.
-    // (focus and blur are always synchronous in other supported browsers,
-    // this just defines when we can count on it).
-    function expectSync(elem, type) {
-        return (elem === safeActiveElement()) === (type === "focus");
-    }
-
-    // Support: IE <=9 only
-    // Accessing document.activeElement can throw unexpectedly
-    // https://bugs.jquery.com/ticket/13393
-    function safeActiveElement() {
-        try {
-            return document.activeElement;
-        } catch (err) {}
-    }
-
     function on(elem, types, selector, data, fn, one) {
         var origFn, type;
 
         // Types can be a map of types/handlers
         if (typeof types === "object") {
 
             // ( types-Object, selector, data )
@@ -5497,23 +5200,23 @@
                 // https://www.w3.org/TR/DOM-Level-3-Events/#event-type-click
                 // Support: IE 11 only
                 // ...but not arrow key "clicks" of radio inputs, which can have `button` -1 (gh-2343)
                 !(event.type === "click" && event.button >= 1)) {
 
                 for (; cur !== this; cur = cur.parentNode || this) {
 
-                    // Don't check non-elements (#13208)
-                    // Don't process clicks on disabled elements (#6911, #8165, #11382, #11764)
+                    // Don't check non-elements (trac-13208)
+                    // Don't process clicks on disabled elements (trac-6911, trac-8165, trac-11382, trac-11764)
                     if (cur.nodeType === 1 && !(event.type === "click" && cur.disabled === true)) {
                         matchedHandlers = [];
                         matchedSelectors = {};
                         for (i = 0; i < delegateCount; i++) {
                             handleObj = handlers[i];
 
-                            // Don't conflict with Object.prototype properties (#13203)
+                            // Don't conflict with Object.prototype properties (trac-13203)
                             sel = handleObj.selector + " ";
 
                             if (matchedSelectors[sel] === undefined) {
                                 matchedSelectors[sel] = handleObj.needsContext ?
                                     jQuery(sel, this).index(cur) > -1 :
                                     jQuery.find(sel, this, null, [cur]).length;
                             }
@@ -5592,15 +5295,15 @@
                     var el = this || data;
 
                     // Claim the first handler
                     if (rcheckableType.test(el.type) &&
                         el.click && nodeName(el, "input")) {
 
                         // dataPriv.set( el, "click", ... )
-                        leverageNative(el, "click", returnTrue);
+                        leverageNative(el, "click", true);
                     }
 
                     // Return false to allow normal processing in the caller
                     return false;
                 },
                 trigger: function(data) {
 
@@ -5643,98 +5346,88 @@
         }
     };
 
     // Ensure the presence of an event listener that handles manually-triggered
     // synthetic events by interrupting progress until reinvoked in response to
     // *native* events that it fires directly, ensuring that state changes have
     // already occurred before other listeners are invoked.
-    function leverageNative(el, type, expectSync) {
+    function leverageNative(el, type, isSetup) {
 
-        // Missing expectSync indicates a trigger call, which must force setup through jQuery.event.add
-        if (!expectSync) {
+        // Missing `isSetup` indicates a trigger call, which must force setup through jQuery.event.add
+        if (!isSetup) {
             if (dataPriv.get(el, type) === undefined) {
                 jQuery.event.add(el, type, returnTrue);
             }
             return;
         }
 
         // Register the controller as a special universal handler for all event namespaces
         dataPriv.set(el, type, false);
         jQuery.event.add(el, type, {
             namespace: false,
             handler: function(event) {
-                var notAsync, result,
+                var result,
                     saved = dataPriv.get(this, type);
 
                 if ((event.isTrigger & 1) && this[type]) {
 
                     // Interrupt processing of the outer synthetic .trigger()ed event
-                    // Saved data should be false in such cases, but might be a leftover capture object
-                    // from an async native handler (gh-4350)
-                    if (!saved.length) {
+                    if (!saved) {
 
                         // Store arguments for use when handling the inner native event
                         // There will always be at least one argument (an event object), so this array
                         // will not be confused with a leftover capture object.
                         saved = slice.call(arguments);
                         dataPriv.set(this, type, saved);
 
                         // Trigger the native event and capture its result
-                        // Support: IE <=9 - 11+
-                        // focus() and blur() are asynchronous
-                        notAsync = expectSync(this, type);
                         this[type]();
                         result = dataPriv.get(this, type);
-                        if (saved !== result || notAsync) {
-                            dataPriv.set(this, type, false);
-                        } else {
-                            result = {};
-                        }
+                        dataPriv.set(this, type, false);
+
                         if (saved !== result) {
 
                             // Cancel the outer synthetic event
                             event.stopImmediatePropagation();
                             event.preventDefault();
 
-                            // Support: Chrome 86+
-                            // In Chrome, if an element having a focusout handler is blurred by
-                            // clicking outside of it, it invokes the handler synchronously. If
-                            // that handler calls `.remove()` on the element, the data is cleared,
-                            // leaving `result` undefined. We need to guard against this.
-                            return result && result.value;
+                            return result;
                         }
 
                         // If this is an inner synthetic event for an event with a bubbling surrogate
-                        // (focus or blur), assume that the surrogate already propagated from triggering the
-                        // native event and prevent that from happening again here.
+                        // (focus or blur), assume that the surrogate already propagated from triggering
+                        // the native event and prevent that from happening again here.
                         // This technically gets the ordering wrong w.r.t. to `.trigger()` (in which the
                         // bubbling surrogate propagates *after* the non-bubbling base), but that seems
                         // less bad than duplication.
                     } else if ((jQuery.event.special[type] || {}).delegateType) {
                         event.stopPropagation();
                     }
 
                     // If this is a native event triggered above, everything is now in order
                     // Fire an inner synthetic event with the original arguments
-                } else if (saved.length) {
+                } else if (saved) {
 
                     // ...and capture the result
-                    dataPriv.set(this, type, {
-                        value: jQuery.event.trigger(
-
-                            // Support: IE <=9 - 11+
-                            // Extend with the prototype to reset the above stopImmediatePropagation()
-                            jQuery.extend(saved[0], jQuery.Event.prototype),
-                            saved.slice(1),
-                            this
-                        )
-                    });
-
-                    // Abort handling of the native event
-                    event.stopImmediatePropagation();
+                    dataPriv.set(this, type, jQuery.event.trigger(
+                        saved[0],
+                        saved.slice(1),
+                        this
+                    ));
+
+                    // Abort handling of the native event by all jQuery handlers while allowing
+                    // native handlers on the same element to run. On target, this is achieved
+                    // by stopping immediate propagation just on the jQuery event. However,
+                    // the native event is re-wrapped by a jQuery one on each level of the
+                    // propagation so the only way to stop it for jQuery is to stop it for
+                    // everyone via native `stopPropagation()`. This is not a problem for
+                    // focus/blur which don't bubble, but it does also stop click on checkboxes
+                    // and radios. We accept this limitation.
+                    event.stopPropagation();
+                    event.isImmediatePropagationStopped = returnTrue;
                 }
             }
         });
     }
 
     jQuery.removeEvent = function(elem, type, handle) {
 
@@ -5764,15 +5457,15 @@
                 // Support: Android <=2.3 only
                 src.returnValue === false ?
                 returnTrue :
                 returnFalse;
 
             // Create target properties
             // Support: Safari <=6 - 7 only
-            // Target should not be a text node (#504, #13143)
+            // Target should not be a text node (trac-504, trac-13143)
             this.target = (src.target && src.target.nodeType === 3) ?
                 src.target.parentNode :
                 src.target;
 
             this.currentTarget = src.currentTarget;
             this.relatedTarget = src.relatedTarget;
 
@@ -5868,44 +5561,169 @@
         which: true
     }, jQuery.event.addProp);
 
     jQuery.each({
         focus: "focusin",
         blur: "focusout"
     }, function(type, delegateType) {
+
+        function focusMappedHandler(nativeEvent) {
+            if (document.documentMode) {
+
+                // Support: IE 11+
+                // Attach a single focusin/focusout handler on the document while someone wants
+                // focus/blur. This is because the former are synchronous in IE while the latter
+                // are async. In other browsers, all those handlers are invoked synchronously.
+
+                // `handle` from private data would already wrap the event, but we need
+                // to change the `type` here.
+                var handle = dataPriv.get(this, "handle"),
+                    event = jQuery.event.fix(nativeEvent);
+                event.type = nativeEvent.type === "focusin" ? "focus" : "blur";
+                event.isSimulated = true;
+
+                // First, handle focusin/focusout
+                handle(nativeEvent);
+
+                // ...then, handle focus/blur
+                //
+                // focus/blur don't bubble while focusin/focusout do; simulate the former by only
+                // invoking the handler at the lower level.
+                if (event.target === event.currentTarget) {
+
+                    // The setup part calls `leverageNative`, which, in turn, calls
+                    // `jQuery.event.add`, so event handle will already have been set
+                    // by this point.
+                    handle(event);
+                }
+            } else {
+
+                // For non-IE browsers, attach a single capturing handler on the document
+                // while someone wants focusin/focusout.
+                jQuery.event.simulate(delegateType, nativeEvent.target,
+                    jQuery.event.fix(nativeEvent));
+            }
+        }
+
         jQuery.event.special[type] = {
 
             // Utilize native event if possible so blur/focus sequence is correct
             setup: function() {
 
+                var attaches;
+
                 // Claim the first handler
                 // dataPriv.set( this, "focus", ... )
                 // dataPriv.set( this, "blur", ... )
-                leverageNative(this, type, expectSync);
+                leverageNative(this, type, true);
 
-                // Return false to allow normal processing in the caller
-                return false;
+                if (document.documentMode) {
+
+                    // Support: IE 9 - 11+
+                    // We use the same native handler for focusin & focus (and focusout & blur)
+                    // so we need to coordinate setup & teardown parts between those events.
+                    // Use `delegateType` as the key as `type` is already used by `leverageNative`.
+                    attaches = dataPriv.get(this, delegateType);
+                    if (!attaches) {
+                        this.addEventListener(delegateType, focusMappedHandler);
+                    }
+                    dataPriv.set(this, delegateType, (attaches || 0) + 1);
+                } else {
+
+                    // Return false to allow normal processing in the caller
+                    return false;
+                }
             },
             trigger: function() {
 
                 // Force setup before trigger
                 leverageNative(this, type);
 
                 // Return non-false to allow normal event-path propagation
                 return true;
             },
 
-            // Suppress native focus or blur as it's already being fired
-            // in leverageNative.
-            _default: function() {
-                return true;
+            teardown: function() {
+                var attaches;
+
+                if (document.documentMode) {
+                    attaches = dataPriv.get(this, delegateType) - 1;
+                    if (!attaches) {
+                        this.removeEventListener(delegateType, focusMappedHandler);
+                        dataPriv.remove(this, delegateType);
+                    } else {
+                        dataPriv.set(this, delegateType, attaches);
+                    }
+                } else {
+
+                    // Return false to indicate standard teardown should be applied
+                    return false;
+                }
+            },
+
+            // Suppress native focus or blur if we're currently inside
+            // a leveraged native-event stack
+            _default: function(event) {
+                return dataPriv.get(event.target, type);
             },
 
             delegateType: delegateType
         };
+
+        // Support: Firefox <=44
+        // Firefox doesn't have focus(in | out) events
+        // Related ticket - https://bugzilla.mozilla.org/show_bug.cgi?id=687787
+        //
+        // Support: Chrome <=48 - 49, Safari <=9.0 - 9.1
+        // focus(in | out) events fire after focus & blur events,
+        // which is spec violation - http://www.w3.org/TR/DOM-Level-3-Events/#events-focusevent-event-order
+        // Related ticket - https://bugs.chromium.org/p/chromium/issues/detail?id=449857
+        //
+        // Support: IE 9 - 11+
+        // To preserve relative focusin/focus & focusout/blur event order guaranteed on the 3.x branch,
+        // attach a single handler for both events in IE.
+        jQuery.event.special[delegateType] = {
+            setup: function() {
+
+                // Handle: regular nodes (via `this.ownerDocument`), window
+                // (via `this.document`) & document (via `this`).
+                var doc = this.ownerDocument || this.document || this,
+                    dataHolder = document.documentMode ? this : doc,
+                    attaches = dataPriv.get(dataHolder, delegateType);
+
+                // Support: IE 9 - 11+
+                // We use the same native handler for focusin & focus (and focusout & blur)
+                // so we need to coordinate setup & teardown parts between those events.
+                // Use `delegateType` as the key as `type` is already used by `leverageNative`.
+                if (!attaches) {
+                    if (document.documentMode) {
+                        this.addEventListener(delegateType, focusMappedHandler);
+                    } else {
+                        doc.addEventListener(type, focusMappedHandler, true);
+                    }
+                }
+                dataPriv.set(dataHolder, delegateType, (attaches || 0) + 1);
+            },
+            teardown: function() {
+                var doc = this.ownerDocument || this.document || this,
+                    dataHolder = document.documentMode ? this : doc,
+                    attaches = dataPriv.get(dataHolder, delegateType) - 1;
+
+                if (!attaches) {
+                    if (document.documentMode) {
+                        this.removeEventListener(delegateType, focusMappedHandler);
+                    } else {
+                        doc.removeEventListener(type, focusMappedHandler, true);
+                    }
+                    dataPriv.remove(dataHolder, delegateType);
+                } else {
+                    dataPriv.set(dataHolder, delegateType, attaches);
+                }
+            }
+        };
     });
 
     // Create mouseenter/leave events using mouseover/out and event-time checks
     // so that event delegation works in jQuery.
     // Do the same for pointerenter/pointerleave and pointerover/pointerout
     //
     // Support: Safari 7 only
@@ -5992,15 +5810,16 @@
         // Support: IE <=10 - 11, Edge 12 - 13 only
         // In IE/Edge using regex groups here causes severe slowdowns.
         // See https://connect.microsoft.com/IE/feedback/details/1736512/
         rnoInnerhtml = /<script|<style|<link/i,
 
         // checked="checked" or checked
         rchecked = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        rcleanScript = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+
+        rcleanScript = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
     // Prefer a tbody over its parent table for containing new rows
     function manipulationTarget(elem, content) {
         if (nodeName(elem, "table") &&
             nodeName(content.nodeType !== 11 ? content : content.firstChild, "tr")) {
 
             return jQuery(elem).children("tbody")[0] || elem;
@@ -6107,15 +5926,15 @@
             // Require either new content or an interest in ignored elements to invoke the callback
             if (first || ignored) {
                 scripts = jQuery.map(getAll(fragment, "script"), disableScript);
                 hasScripts = scripts.length;
 
                 // Use the original fragment for the last item
                 // instead of the first because it can end up
-                // being emptied incorrectly in certain situations (#8070).
+                // being emptied incorrectly in certain situations (trac-8070).
                 for (; i < l; i++) {
                     node = fragment;
 
                     if (i !== iNoClone) {
                         node = jQuery.clone(node, true, true);
 
                         // Keep references to cloned scripts for later restoration
@@ -6148,14 +5967,20 @@
                                 // Optional AJAX dependency, but won't run scripts if not present
                                 if (jQuery._evalUrl && !node.noModule) {
                                     jQuery._evalUrl(node.src, {
                                         nonce: node.nonce || node.getAttribute("nonce")
                                     }, doc);
                                 }
                             } else {
+
+                                // Unwrap a CDATA section containing script contents. This shouldn't be
+                                // needed as in XML documents they're already not visible when
+                                // inspecting element contents and in HTML documents they have no
+                                // meaning but we're preserving that logic for backwards compatibility.
+                                // This will be removed completely in 4.0. See gh-4904.
                                 DOMEval(node.textContent.replace(rcleanScript, ""), node, doc);
                             }
                         }
                     }
                 }
             }
         }
@@ -6195,15 +6020,16 @@
                 clone = elem.cloneNode(true),
                 inPage = isAttached(elem);
 
             // Fix IE cloning issues
             if (!support.noCloneChecked && (elem.nodeType === 1 || elem.nodeType === 11) &&
                 !jQuery.isXMLDoc(elem)) {
 
-                // We eschew Sizzle here for performance reasons: https://jsperf.com/getall-vs-sizzle/2
+                // We eschew jQuery#find here for performance reasons:
+                // https://jsperf.com/getall-vs-sizzle/2
                 destElements = getAll(clone);
                 srcElements = getAll(elem);
 
                 for (i = 0, l = srcElements.length; i < l; i++) {
                     fixInput(srcElements[i], destElements[i]);
                 }
             }
@@ -6433,17 +6259,20 @@
             }
 
             return this.pushStack(ret);
         };
     });
     var rnumnonpx = new RegExp("^(" + pnum + ")(?!px)[a-z%]+$", "i");
 
+    var rcustomProp = /^--/;
+
+
     var getStyles = function(elem) {
 
-        // Support: IE <=11 only, Firefox <=30 (#15098, #14150)
+        // Support: IE <=11 only, Firefox <=30 (trac-15098, trac-14150)
         // IE throws on elements created in popups
         // FF meanwhile throws on frame elements through "defaultView.getComputedStyle"
         var view = elem.ownerDocument.defaultView;
 
         if (!view || !view.opener) {
             view = window;
         }
@@ -6535,15 +6364,15 @@
 
         // Finish early in limited (non-browser) environments
         if (!div.style) {
             return;
         }
 
         // Support: IE <=9 - 11 only
-        // Style of cloned element affects source element cloned (#8908)
+        // Style of cloned element affects source element cloned (trac-8908)
         div.style.backgroundClip = "content-box";
         div.cloneNode(true).style.backgroundClip = "";
         support.clearCloneStyle = div.style.backgroundClip === "content-box";
 
         jQuery.extend(support, {
             boxSizingReliable: function() {
                 computeStyleTests();
@@ -6615,29 +6444,61 @@
             }
         });
     })();
 
 
     function curCSS(elem, name, computed) {
         var width, minWidth, maxWidth, ret,
+            isCustomProp = rcustomProp.test(name),
 
             // Support: Firefox 51+
             // Retrieving style before computed somehow
             // fixes an issue with getting wrong values
             // on detached elements
             style = elem.style;
 
         computed = computed || getStyles(elem);
 
         // getPropertyValue is needed for:
-        //   .css('filter') (IE 9 only, #12537)
-        //   .css('--customProperty) (#3144)
+        //   .css('filter') (IE 9 only, trac-12537)
+        //   .css('--customProperty) (gh-3144)
         if (computed) {
+
+            // Support: IE <=9 - 11+
+            // IE only supports `"float"` in `getPropertyValue`; in computed styles
+            // it's only available as `"cssFloat"`. We no longer modify properties
+            // sent to `.css()` apart from camelCasing, so we need to check both.
+            // Normally, this would create difference in behavior: if
+            // `getPropertyValue` returns an empty string, the value returned
+            // by `.css()` would be `undefined`. This is usually the case for
+            // disconnected elements. However, in IE even disconnected elements
+            // with no styles return `"none"` for `getPropertyValue( "float" )`
             ret = computed.getPropertyValue(name) || computed[name];
 
+            if (isCustomProp && ret) {
+
+                // Support: Firefox 105+, Chrome <=105+
+                // Spec requires trimming whitespace for custom properties (gh-4926).
+                // Firefox only trims leading whitespace. Chrome just collapses
+                // both leading & trailing whitespace to a single space.
+                //
+                // Fall back to `undefined` if empty string returned.
+                // This collapses a missing definition with property defined
+                // and set to an empty string but there's no standard API
+                // allowing us to differentiate them without a performance penalty
+                // and returning `undefined` aligns with older jQuery.
+                //
+                // rtrimCSS treats U+000D CARRIAGE RETURN and U+000C FORM FEED
+                // as whitespace while CSS does not, but this is not a problem
+                // because CSS preprocessing replaces them with U+000A LINE FEED
+                // (which *is* CSS whitespace)
+                // https://www.w3.org/TR/css-syntax-3/#input-preprocessing
+                ret = ret.replace(rtrimCSS, "$1") || undefined;
+            }
+
             if (ret === "" && !isAttached(elem)) {
                 ret = jQuery.style(elem, name);
             }
 
             // A tribute to the "awesome hack by Dean Edwards"
             // Android Browser returns percentage for some values,
             // but width seems to be reliably pixels.
@@ -6725,15 +6586,14 @@
 
     var
 
         // Swappable if display is none or starts with table
         // except "table", "table-cell", or "table-caption"
         // See here for display values: https://developer.mozilla.org/en-US/docs/CSS/display
         rdisplayswap = /^(none|table(?!-c[ea]).+)/,
-        rcustomProp = /^--/,
         cssShow = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
         cssNormalTransform = {
             letterSpacing: "0",
@@ -6751,26 +6611,29 @@
             Math.max(0, matches[2] - (subtract || 0)) + (matches[3] || "px") :
             value;
     }
 
     function boxModelAdjustment(elem, dimension, box, isBorderBox, styles, computedVal) {
         var i = dimension === "width" ? 1 : 0,
             extra = 0,
-            delta = 0;
+            delta = 0,
+            marginDelta = 0;
 
         // Adjustment may not be necessary
         if (box === (isBorderBox ? "border" : "content")) {
             return 0;
         }
 
         for (; i < 4; i += 2) {
 
             // Both box models exclude margin
+            // Count margin delta separately to only add it after scroll gutter adjustment.
+            // This is needed to make negative margins work with `outerHeight( true )` (gh-3982).
             if (box === "margin") {
-                delta += jQuery.css(elem, box + cssExpand[i], true, styles);
+                marginDelta += jQuery.css(elem, box + cssExpand[i], true, styles);
             }
 
             // If we get here with a content-box, we're seeking "padding" or "border" or "margin"
             if (!isBorderBox) {
 
                 // Add padding
                 delta += jQuery.css(elem, "padding" + cssExpand[i], true, styles);
@@ -6813,15 +6676,15 @@
                 0.5
 
                 // If offsetWidth/offsetHeight is unknown, then we can't determine content-box scroll gutter
                 // Use an explicit zero to avoid NaN (gh-3964)
             )) || 0;
         }
 
-        return delta;
+        return delta + marginDelta;
     }
 
     function getWidthOrHeight(elem, dimension, extra) {
 
         // Start with computed style
         var styles = getStyles(elem),
 
@@ -6911,34 +6774,43 @@
                     }
                 }
             }
         },
 
         // Don't automatically add "px" to these possibly-unitless properties
         cssNumber: {
-            "animationIterationCount": true,
-            "columnCount": true,
-            "fillOpacity": true,
-            "flexGrow": true,
-            "flexShrink": true,
-            "fontWeight": true,
-            "gridArea": true,
-            "gridColumn": true,
-            "gridColumnEnd": true,
-            "gridColumnStart": true,
-            "gridRow": true,
-            "gridRowEnd": true,
-            "gridRowStart": true,
-            "lineHeight": true,
-            "opacity": true,
-            "order": true,
-            "orphans": true,
-            "widows": true,
-            "zIndex": true,
-            "zoom": true
+            animationIterationCount: true,
+            aspectRatio: true,
+            borderImageSlice: true,
+            columnCount: true,
+            flexGrow: true,
+            flexShrink: true,
+            fontWeight: true,
+            gridArea: true,
+            gridColumn: true,
+            gridColumnEnd: true,
+            gridColumnStart: true,
+            gridRow: true,
+            gridRowEnd: true,
+            gridRowStart: true,
+            lineHeight: true,
+            opacity: true,
+            order: true,
+            orphans: true,
+            scale: true,
+            widows: true,
+            zIndex: true,
+            zoom: true,
+
+            // SVG-related
+            fillOpacity: true,
+            floodOpacity: true,
+            stopOpacity: true,
+            strokeMiterlimit: true,
+            strokeOpacity: true
         },
 
         // Add in properties whose names you wish to fix before
         // setting or getting the value
         cssProps: {},
 
         // Get and set the style property on a DOM Node
@@ -6965,23 +6837,23 @@
             // Gets hook for the prefixed version, then unprefixed version
             hooks = jQuery.cssHooks[name] || jQuery.cssHooks[origName];
 
             // Check if we're setting a value
             if (value !== undefined) {
                 type = typeof value;
 
-                // Convert "+=" or "-=" to relative numbers (#7345)
+                // Convert "+=" or "-=" to relative numbers (trac-7345)
                 if (type === "string" && (ret = rcssNum.exec(value)) && ret[1]) {
                     value = adjustCSS(elem, name, ret);
 
-                    // Fixes bug #9237
+                    // Fixes bug trac-9237
                     type = "number";
                 }
 
-                // Make sure that null and NaN values aren't set (#7116)
+                // Make sure that null and NaN values aren't set (trac-7116)
                 if (value == null || value !== value) {
                     return;
                 }
 
                 // If a number was passed in, add the unit (except for certain CSS properties)
                 // The isCustomProp check can be removed in jQuery 4.0 when we only auto-append
                 // "px" to a few hardcoded values.
@@ -7195,15 +7067,14 @@
                     jQuery.css(elem, name);
             }, name, value, arguments.length > 1);
         }
     });
 
 
     // Based off of the plugin by Clint Helfers, with permission.
-    // https://web.archive.org/web/20100324014747/http://blindsignals.com/index.php/2009/07/jquery-delay/
     jQuery.fn.delay = function(time, type) {
         time = jQuery.fx ? jQuery.fx.speeds[time] || time : time;
         type = type || "fx";
 
         return this.queue(type, function(next, hooks) {
             var timeout = window.setTimeout(next, time);
             hooks.stop = function() {
@@ -7420,16 +7291,15 @@
         propHooks: {
             tabIndex: {
                 get: function(elem) {
 
                     // Support: IE <=9 - 11 only
                     // elem.tabIndex doesn't always return the
                     // correct value when it hasn't been explicitly set
-                    // https://web.archive.org/web/20141116233347/http://fluidproject.org/blog/2008/01/09/getting-setting-and-removing-tabindex-values-with-javascript/
-                    // Use proper attribute retrieval(#12072)
+                    // Use proper attribute retrieval (trac-12072)
                     var tabindex = jQuery.find.attr(elem, "tabindex");
 
                     if (tabindex) {
                         return parseInt(tabindex, 10);
                     }
 
                     if (
@@ -7525,123 +7395,121 @@
             return value.match(rnothtmlwhite) || [];
         }
         return [];
     }
 
     jQuery.fn.extend({
         addClass: function(value) {
-            var classes, elem, cur, curValue, clazz, j, finalValue,
-                i = 0;
+            var classNames, cur, curValue, className, i, finalValue;
 
             if (isFunction(value)) {
                 return this.each(function(j) {
                     jQuery(this).addClass(value.call(this, j, getClass(this)));
                 });
             }
 
-            classes = classesToArray(value);
+            classNames = classesToArray(value);
 
-            if (classes.length) {
-                while ((elem = this[i++])) {
-                    curValue = getClass(elem);
-                    cur = elem.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
+            if (classNames.length) {
+                return this.each(function() {
+                    curValue = getClass(this);
+                    cur = this.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
 
                     if (cur) {
-                        j = 0;
-                        while ((clazz = classes[j++])) {
-                            if (cur.indexOf(" " + clazz + " ") < 0) {
-                                cur += clazz + " ";
+                        for (i = 0; i < classNames.length; i++) {
+                            className = classNames[i];
+                            if (cur.indexOf(" " + className + " ") < 0) {
+                                cur += className + " ";
                             }
                         }
 
                         // Only assign if different to avoid unneeded rendering.
                         finalValue = stripAndCollapse(cur);
                         if (curValue !== finalValue) {
-                            elem.setAttribute("class", finalValue);
+                            this.setAttribute("class", finalValue);
                         }
                     }
-                }
+                });
             }
 
             return this;
         },
 
         removeClass: function(value) {
-            var classes, elem, cur, curValue, clazz, j, finalValue,
-                i = 0;
+            var classNames, cur, curValue, className, i, finalValue;
 
             if (isFunction(value)) {
                 return this.each(function(j) {
                     jQuery(this).removeClass(value.call(this, j, getClass(this)));
                 });
             }
 
             if (!arguments.length) {
                 return this.attr("class", "");
             }
 
-            classes = classesToArray(value);
+            classNames = classesToArray(value);
 
-            if (classes.length) {
-                while ((elem = this[i++])) {
-                    curValue = getClass(elem);
+            if (classNames.length) {
+                return this.each(function() {
+                    curValue = getClass(this);
 
                     // This expression is here for better compressibility (see addClass)
-                    cur = elem.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
+                    cur = this.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
 
                     if (cur) {
-                        j = 0;
-                        while ((clazz = classes[j++])) {
+                        for (i = 0; i < classNames.length; i++) {
+                            className = classNames[i];
 
                             // Remove *all* instances
-                            while (cur.indexOf(" " + clazz + " ") > -1) {
-                                cur = cur.replace(" " + clazz + " ", " ");
+                            while (cur.indexOf(" " + className + " ") > -1) {
+                                cur = cur.replace(" " + className + " ", " ");
                             }
                         }
 
                         // Only assign if different to avoid unneeded rendering.
                         finalValue = stripAndCollapse(cur);
                         if (curValue !== finalValue) {
-                            elem.setAttribute("class", finalValue);
+                            this.setAttribute("class", finalValue);
                         }
                     }
-                }
+                });
             }
 
             return this;
         },
 
         toggleClass: function(value, stateVal) {
-            var type = typeof value,
+            var classNames, className, i, self,
+                type = typeof value,
                 isValidValue = type === "string" || Array.isArray(value);
 
-            if (typeof stateVal === "boolean" && isValidValue) {
-                return stateVal ? this.addClass(value) : this.removeClass(value);
-            }
-
             if (isFunction(value)) {
                 return this.each(function(i) {
                     jQuery(this).toggleClass(
                         value.call(this, i, getClass(this), stateVal),
                         stateVal
                     );
                 });
             }
 
-            return this.each(function() {
-                var className, i, self, classNames;
+            if (typeof stateVal === "boolean" && isValidValue) {
+                return stateVal ? this.addClass(value) : this.removeClass(value);
+            }
 
+            classNames = classesToArray(value);
+
+            return this.each(function() {
                 if (isValidValue) {
 
                     // Toggle individual class names
-                    i = 0;
                     self = jQuery(this);
-                    classNames = classesToArray(value);
 
-                    while ((className = classNames[i++])) {
+                    for (i = 0; i < classNames.length; i++) {
+                        className = classNames[i];
 
                         // Check each className given, space separated list
                         if (self.hasClass(className)) {
                             self.removeClass(className);
                         } else {
                             self.addClass(className);
                         }
@@ -7767,15 +7635,15 @@
                 get: function(elem) {
 
                     var val = jQuery.find.attr(elem, "value");
                     return val != null ?
                         val :
 
                         // Support: IE <=10 - 11 only
-                        // option.text throws exceptions (#14686, #14858)
+                        // option.text throws exceptions (trac-14686, trac-14858)
                         // Strip and collapse whitespace
                         // https://html.spec.whatwg.org/#strip-and-collapse-whitespace
                         stripAndCollapse(jQuery.text(elem));
                 }
             },
             select: {
                 get: function(elem) {
@@ -7794,15 +7662,15 @@
                     }
 
                     // Loop through all the selected options
                     for (; i < max; i++) {
                         option = options[i];
 
                         // Support: IE <=9 only
-                        // IE8-9 doesn't update selected after form reset (#2551)
+                        // IE8-9 doesn't update selected after form reset (trac-2551)
                         if ((option.selected || i === index) &&
 
                             // Don't return options that are disabled or in a disabled optgroup
                             !option.disabled &&
                             (!option.parentNode.disabled ||
                                 !nodeName(option.parentNode, "optgroup"))) {
 
@@ -7870,15 +7738,39 @@
 
 
 
 
     // Return jQuery for attributes-only inclusion
 
 
-    support.focusin = "onfocusin" in window;
+    // Cross-browser xml parsing
+    jQuery.parseXML = function(data) {
+        var xml, parserErrorElem;
+        if (!data || typeof data !== "string") {
+            return null;
+        }
+
+        // Support: IE 9 - 11 only
+        // IE throws on parseFromString with invalid input.
+        try {
+            xml = (new window.DOMParser()).parseFromString(data, "text/xml");
+        } catch (e) {}
+
+        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
+        if (!xml || parserErrorElem) {
+            jQuery.error("Invalid XML: " + (
+                parserErrorElem ?
+                jQuery.map(parserErrorElem.childNodes, function(el) {
+                    return el.textContent;
+                }).join("\n") :
+                data
+            ));
+        }
+        return xml;
+    };
 
 
     var rfocusMorph = /^(?:focusinfocus|focusoutblur)$/,
         stopPropagationCallback = function(e) {
             e.stopPropagation();
         };
 
@@ -7936,16 +7828,16 @@
 
             // Allow special events to draw outside the lines
             special = jQuery.event.special[type] || {};
             if (!onlyHandlers && special.trigger && special.trigger.apply(elem, data) === false) {
                 return;
             }
 
-            // Determine event propagation path in advance, per W3C events spec (#9951)
-            // Bubble up to document, then to window; watch for a global ownerDocument var (#9724)
+            // Determine event propagation path in advance, per W3C events spec (trac-9951)
+            // Bubble up to document, then to window; watch for a global ownerDocument var (trac-9724)
             if (!onlyHandlers && !special.noBubble && !isWindow(elem)) {
 
                 bubbleType = special.delegateType || type;
                 if (!rfocusMorph.test(bubbleType + type)) {
                     cur = cur.parentNode;
                 }
                 for (; cur; cur = cur.parentNode) {
@@ -7989,15 +7881,15 @@
             if (!onlyHandlers && !event.isDefaultPrevented()) {
 
                 if ((!special._default ||
                         special._default.apply(eventPath.pop(), data) === false) &&
                     acceptData(elem)) {
 
                     // Call a native DOM method on the target with the same name as the event.
-                    // Don't do default actions on window, that's where global variables be (#6170)
+                    // Don't do default actions on window, that's where global variables be (trac-6170)
                     if (ontype && isFunction(elem[type]) && !isWindow(elem)) {
 
                         // Don't re-trigger an onFOO event when we call its FOO() method
                         tmp = elem[ontype];
 
                         if (tmp) {
                             elem[ontype] = null;
@@ -8056,90 +7948,14 @@
             if (elem) {
                 return jQuery.event.trigger(type, data, elem, true);
             }
         }
     });
 
 
-    // Support: Firefox <=44
-    // Firefox doesn't have focus(in | out) events
-    // Related ticket - https://bugzilla.mozilla.org/show_bug.cgi?id=687787
-    //
-    // Support: Chrome <=48 - 49, Safari <=9.0 - 9.1
-    // focus(in | out) events fire after focus & blur events,
-    // which is spec violation - http://www.w3.org/TR/DOM-Level-3-Events/#events-focusevent-event-order
-    // Related ticket - https://bugs.chromium.org/p/chromium/issues/detail?id=449857
-    if (!support.focusin) {
-        jQuery.each({
-            focus: "focusin",
-            blur: "focusout"
-        }, function(orig, fix) {
-
-            // Attach a single capturing handler on the document while someone wants focusin/focusout
-            var handler = function(event) {
-                jQuery.event.simulate(fix, event.target, jQuery.event.fix(event));
-            };
-
-            jQuery.event.special[fix] = {
-                setup: function() {
-
-                    // Handle: regular nodes (via `this.ownerDocument`), window
-                    // (via `this.document`) & document (via `this`).
-                    var doc = this.ownerDocument || this.document || this,
-                        attaches = dataPriv.access(doc, fix);
-
-                    if (!attaches) {
-                        doc.addEventListener(orig, handler, true);
-                    }
-                    dataPriv.access(doc, fix, (attaches || 0) + 1);
-                },
-                teardown: function() {
-                    var doc = this.ownerDocument || this.document || this,
-                        attaches = dataPriv.access(doc, fix) - 1;
-
-                    if (!attaches) {
-                        doc.removeEventListener(orig, handler, true);
-                        dataPriv.remove(doc, fix);
-
-                    } else {
-                        dataPriv.access(doc, fix, attaches);
-                    }
-                }
-            };
-        });
-    }
-
-
-    // Cross-browser xml parsing
-    jQuery.parseXML = function(data) {
-        var xml, parserErrorElem;
-        if (!data || typeof data !== "string") {
-            return null;
-        }
-
-        // Support: IE 9 - 11 only
-        // IE throws on parseFromString with invalid input.
-        try {
-            xml = (new window.DOMParser()).parseFromString(data, "text/xml");
-        } catch (e) {}
-
-        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
-        if (!xml || parserErrorElem) {
-            jQuery.error("Invalid XML: " + (
-                parserErrorElem ?
-                jQuery.map(parserErrorElem.childNodes, function(el) {
-                    return el.textContent;
-                }).join("\n") :
-                data
-            ));
-        }
-        return xml;
-    };
-
-
     var
         rbracket = /\[\]$/,
         rCRLF = /\r?\n/g,
         rsubmitterTypes = /^(?:submit|button|image|reset|file)$/i,
         rsubmittable = /^(?:input|select|textarea|keygen)/i;
 
     function buildParams(prefix, obj, traditional, add) {
@@ -8719,15 +8535,17 @@
     );
 
 
 
 
     // Support: Android <=4.0 only
     // Make sure we trim BOM and NBSP
-    var rtrim = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    // Require that the "whitespace run" starts from a non-whitespace
+    // to avoid O(N^2) behavior when the engine would try matching "\s+$" at each space position.
+    var rtrim = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
 
     // Bind a function to a context, optionally partially applying any
     // arguments.
     // jQuery.proxy is deprecated to promote standards (specifically Function#bind)
     // However, it is not slated for removal any time soon
     jQuery.proxy = function(fn, context) {
         var tmp, args, proxy;
@@ -8786,15 +8604,15 @@
             // subtraction forces infinities to NaN
             !isNaN(obj - parseFloat(obj));
     };
 
     jQuery.trim = function(text) {
         return text == null ?
             "" :
-            (text + "").replace(rtrim, "");
+            (text + "").replace(rtrim, "$1");
     };
 
 
 
     // Register as a named AMD module, since jQuery can be concatenated with other
     // files that may use define, but not via a proper concatenation script that
     // understands anonymous AMD modules. A named AMD is safest and most robust
@@ -8834,16 +8652,16 @@
             window.jQuery = _jQuery;
         }
 
         return jQuery;
     };
 
     // Expose jQuery and $ identifiers, even in AMD
-    // (#7102#comment:10, https://github.com/jquery/jquery/pull/557)
-    // and CommonJS for browser emulators (#13566)
+    // (trac-7102#comment:10, https://github.com/jquery/jquery/pull/557)
+    // and CommonJS for browser emulators (trac-13566)
     if (typeof noGlobal === "undefined") {
         window.jQuery = window.$ = jQuery;
     }
```

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/openseadragon-scalebar.js` & `openslide-python-1.3.0/examples/deepzoom/static/openseadragon-scalebar.js`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/static/openseadragon.js` & `openslide-python-1.3.0/examples/deepzoom/static/openseadragon.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-//! openseadragon 3.0.0
-//! Built on 2021-12-15
-//! Git commit: v3.0.0-0-3eded36
+//! openseadragon 4.1.0
+//! Built on 2023-05-25
+//! Git commit: v4.1.0-0-8849681
 //! http://openseadragon.github.io
 //! License: http://openseadragon.github.io/license/
 
 /*
  * OpenSeadragon
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -62,15 +62,15 @@
  * OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
  * WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  */
 
 /*
  * Portions of this source file taken from mattsnider.com:
  *
- * Copyright (c) 2006-2013 Matt Snider
+ * Copyright (c) 2006-2022 Matt Snider
  *
  * Permission is hereby granted, free of charge, to any person obtaining a
  * copy of this software and associated documentation files (the "Software"),
  * to deal in the Software without restriction, including without limitation
  * the rights to use, copy, modify, merge, publish, distribute, sublicense,
  * and/or sell copies of the Software, and to permit persons to whom the
  * Software is furnished to do so, subject to the following conditions:
@@ -86,15 +86,15 @@
  * OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
  * THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  */
 
 
 /**
  * @namespace OpenSeadragon
- * @version openseadragon 3.0.0
+ * @version openseadragon 4.1.0
  * @classdesc The root namespace for OpenSeadragon.  All utility methods
  * and classes are defined on or below this namespace.
  *
  */
 
 
 // Typedefs
@@ -165,14 +165,18 @@
  * @property {Boolean} [debugMode=false]
  *     TODO: provide an in-screen panel providing event detail feedback.
  *
  * @property {String} [debugGridColor=['#437AB2', '#1B9E77', '#D95F02', '#7570B3', '#E7298A', '#66A61E', '#E6AB02', '#A6761D', '#666666']]
  *     The colors of grids in debug mode. Each tiled image's grid uses a consecutive color.
  *     If there are more tiled images than provided colors, the color vector is recycled.
  *
+ * @property {Boolean} [silenceMultiImageWarnings=false]
+ *     Silences warnings when calling viewport coordinate functions with multi-image.
+ *     Useful when you're overlaying multiple images on top of one another.
+ *
  * @property {Number} [blendTime=0]
  *     Specifies the duration of animation as higher or lower level tiles are
  *     replacing the existing tile.
  *
  * @property {Boolean} [alwaysBlend=false]
  *     Forces the tile to always blend.  By default the tiles skip blending
  *     when the blendTime is surpassed and the current animation frame would
@@ -211,14 +215,25 @@
  *     This property can be changed in {@link Viewer.Drawer.setImageSmoothingEnabled}.
  *
  * @property {String|CanvasGradient|CanvasPattern|Function} [placeholderFillStyle=null]
  *     Draws a colored rectangle behind the tile if it is not loaded yet.
  *     You can pass a CSS color value like "#FF8800".
  *     When passing a function the tiledImage and canvas context are available as argument which is useful when you draw a gradient or pattern.
  *
+ * @property {Object} [subPixelRoundingForTransparency=null]
+ *     Determines when subpixel rounding should be applied for tiles when rendering images that support transparency.
+ *     This property is a subpixel rounding enum values dictionary [{@link BROWSERS}] --> {@link SUBPIXEL_ROUNDING_OCCURRENCES}.
+ *     The key is a {@link BROWSERS} value, and the value is one of {@link SUBPIXEL_ROUNDING_OCCURRENCES},
+ *     indicating, for a given browser, when to apply subpixel rounding.
+ *     Key '*' is the fallback value for any browser not specified in the dictionary.
+ *     This property has a simple mode, and one can set it directly to
+ *     {@link SUBPIXEL_ROUNDING_OCCURRENCES.NEVER}, {@link SUBPIXEL_ROUNDING_OCCURRENCES.ONLY_AT_REST} or {@link SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS}
+ *     in order to apply this rule for all browser. The values {@link SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS} would be equivalent to { '*', SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS }.
+ *     The default is {@link SUBPIXEL_ROUNDING_OCCURRENCES.NEVER} for all browsers, for backward compatibility reason.
+ *
  * @property {Number} [degrees=0]
  *     Initial rotation.
  *
  * @property {Boolean} [flipped=false]
  *     Initial flip state.
  *
  * @property {Number} [minZoomLevel=null]
@@ -319,92 +334,110 @@
  *      The maximum distance allowed between two pointer click events
  *      to be treated as a double-click gesture.
  *
  * @property {Number} [springStiffness=6.5]
  *
  * @property {Number} [animationTime=1.2]
  *     Specifies the animation duration per each {@link OpenSeadragon.Spring}
- *     which occur when the image is dragged or zoomed.
+ *     which occur when the image is dragged, zoomed or rotated.
  *
  * @property {OpenSeadragon.GestureSettings} [gestureSettingsMouse]
  *     Settings for gestures generated by a mouse pointer device. (See {@link OpenSeadragon.GestureSettings})
  * @property {Boolean} [gestureSettingsMouse.dragToPan=true] - Pan on drag gesture
  * @property {Boolean} [gestureSettingsMouse.scrollToZoom=true] - Zoom on scroll gesture
  * @property {Boolean} [gestureSettingsMouse.clickToZoom=true] - Zoom on click gesture
  * @property {Boolean} [gestureSettingsMouse.dblClickToZoom=false] - Zoom on double-click gesture. Note: If set to true
  *     then clickToZoom should be set to false to prevent multiple zooms.
+ * @property {Boolean} [gestureSettingsMouse.dblClickDragToZoom=false] - Zoom on dragging through
+ * double-click gesture ( single click and next click to drag).  Note: If set to true
+ *     then clickToZoom should be set to false to prevent multiple zooms.
  * @property {Boolean} [gestureSettingsMouse.pinchToZoom=false] - Zoom on pinch gesture
  * @property {Boolean} [gestureSettingsMouse.zoomToRefPoint=true] - If zoomToRefPoint is true, the zoom is centered at the pointer position. Otherwise,
  *     the zoom is centered at the canvas center.
  * @property {Boolean} [gestureSettingsMouse.flickEnabled=false] - Enable flick gesture
  * @property {Number} [gestureSettingsMouse.flickMinSpeed=120] - If flickEnabled is true, the minimum speed to initiate a flick gesture (pixels-per-second)
  * @property {Number} [gestureSettingsMouse.flickMomentum=0.25] - If flickEnabled is true, the momentum factor for the flick gesture
  * @property {Boolean} [gestureSettingsMouse.pinchRotate=false] - If pinchRotate is true, the user will have the ability to rotate the image using their fingers.
  *
  * @property {OpenSeadragon.GestureSettings} [gestureSettingsTouch]
  *     Settings for gestures generated by a touch pointer device. (See {@link OpenSeadragon.GestureSettings})
- * @property {Boolean} [gestureSettingsMouse.dragToPan=true] - Pan on drag gesture
+ * @property {Boolean} [gestureSettingsTouch.dragToPan=true] - Pan on drag gesture
  * @property {Boolean} [gestureSettingsTouch.scrollToZoom=false] - Zoom on scroll gesture
  * @property {Boolean} [gestureSettingsTouch.clickToZoom=false] - Zoom on click gesture
  * @property {Boolean} [gestureSettingsTouch.dblClickToZoom=true] - Zoom on double-click gesture. Note: If set to true
  *     then clickToZoom should be set to false to prevent multiple zooms.
+ * @property {Boolean} [gestureSettingsTouch.dblClickDragToZoom=true] - Zoom on dragging through
+ * double-click gesture ( single click and next click to drag).  Note: If set to true
+ *     then clickToZoom should be set to false to prevent multiple zooms.
+ 
  * @property {Boolean} [gestureSettingsTouch.pinchToZoom=true] - Zoom on pinch gesture
  * @property {Boolean} [gestureSettingsTouch.zoomToRefPoint=true] - If zoomToRefPoint is true, the zoom is centered at the pointer position. Otherwise,
  *     the zoom is centered at the canvas center.
  * @property {Boolean} [gestureSettingsTouch.flickEnabled=true] - Enable flick gesture
  * @property {Number} [gestureSettingsTouch.flickMinSpeed=120] - If flickEnabled is true, the minimum speed to initiate a flick gesture (pixels-per-second)
  * @property {Number} [gestureSettingsTouch.flickMomentum=0.25] - If flickEnabled is true, the momentum factor for the flick gesture
  * @property {Boolean} [gestureSettingsTouch.pinchRotate=false] - If pinchRotate is true, the user will have the ability to rotate the image using their fingers.
  *
  * @property {OpenSeadragon.GestureSettings} [gestureSettingsPen]
  *     Settings for gestures generated by a pen pointer device. (See {@link OpenSeadragon.GestureSettings})
- * @property {Boolean} [gestureSettingsMouse.dragToPan=true] - Pan on drag gesture
+ * @property {Boolean} [gestureSettingsPen.dragToPan=true] - Pan on drag gesture
  * @property {Boolean} [gestureSettingsPen.scrollToZoom=false] - Zoom on scroll gesture
  * @property {Boolean} [gestureSettingsPen.clickToZoom=true] - Zoom on click gesture
  * @property {Boolean} [gestureSettingsPen.dblClickToZoom=false] - Zoom on double-click gesture. Note: If set to true
  *     then clickToZoom should be set to false to prevent multiple zooms.
  * @property {Boolean} [gestureSettingsPen.pinchToZoom=false] - Zoom on pinch gesture
  * @property {Boolean} [gestureSettingsPen.zoomToRefPoint=true] - If zoomToRefPoint is true, the zoom is centered at the pointer position. Otherwise,
  *     the zoom is centered at the canvas center.
  * @property {Boolean} [gestureSettingsPen.flickEnabled=false] - Enable flick gesture
  * @property {Number} [gestureSettingsPen.flickMinSpeed=120] - If flickEnabled is true, the minimum speed to initiate a flick gesture (pixels-per-second)
  * @property {Number} [gestureSettingsPen.flickMomentum=0.25] - If flickEnabled is true, the momentum factor for the flick gesture
  * @property {Boolean} [gestureSettingsPen.pinchRotate=false] - If pinchRotate is true, the user will have the ability to rotate the image using their fingers.
  *
  * @property {OpenSeadragon.GestureSettings} [gestureSettingsUnknown]
  *     Settings for gestures generated by unknown pointer devices. (See {@link OpenSeadragon.GestureSettings})
- * @property {Boolean} [gestureSettingsMouse.dragToPan=true] - Pan on drag gesture
+ * @property {Boolean} [gestureSettingsUnknown.dragToPan=true] - Pan on drag gesture
  * @property {Boolean} [gestureSettingsUnknown.scrollToZoom=true] - Zoom on scroll gesture
  * @property {Boolean} [gestureSettingsUnknown.clickToZoom=false] - Zoom on click gesture
  * @property {Boolean} [gestureSettingsUnknown.dblClickToZoom=true] - Zoom on double-click gesture. Note: If set to true
  *     then clickToZoom should be set to false to prevent multiple zooms.
+ * @property {Boolean} [gestureSettingsUnknown.dblClickDragToZoom=false] - Zoom on dragging through
+ * double-click gesture ( single click and next click to drag).  Note: If set to true
+ *     then clickToZoom should be set to false to prevent multiple zooms.
  * @property {Boolean} [gestureSettingsUnknown.pinchToZoom=true] - Zoom on pinch gesture
  * @property {Boolean} [gestureSettingsUnknown.zoomToRefPoint=true] - If zoomToRefPoint is true, the zoom is centered at the pointer position. Otherwise,
  *     the zoom is centered at the canvas center.
  * @property {Boolean} [gestureSettingsUnknown.flickEnabled=true] - Enable flick gesture
  * @property {Number} [gestureSettingsUnknown.flickMinSpeed=120] - If flickEnabled is true, the minimum speed to initiate a flick gesture (pixels-per-second)
  * @property {Number} [gestureSettingsUnknown.flickMomentum=0.25] - If flickEnabled is true, the momentum factor for the flick gesture
  * @property {Boolean} [gestureSettingsUnknown.pinchRotate=false] - If pinchRotate is true, the user will have the ability to rotate the image using their fingers.
  *
  * @property {Number} [zoomPerClick=2.0]
  *     The "zoom distance" per mouse click or touch tap. <em><strong>Note:</strong> Setting this to 1.0 effectively disables the click-to-zoom feature (also see gestureSettings[Mouse|Touch|Pen].clickToZoom/dblClickToZoom).</em>
  *
  * @property {Number} [zoomPerScroll=1.2]
  *     The "zoom distance" per mouse scroll or touch pinch. <em><strong>Note:</strong> Setting this to 1.0 effectively disables the mouse-wheel zoom feature (also see gestureSettings[Mouse|Touch|Pen].scrollToZoom}).</em>
  *
+ * @property {Number} [zoomPerDblClickDrag=1.2]
+ *     The "zoom distance" per double-click mouse drag. <em><strong>Note:</strong> Setting this to 1.0 effectively disables the double-click-drag-to-Zoom feature (also see gestureSettings[Mouse|Touch|Pen].dblClickDragToZoom).</em>
+ *
  * @property {Number} [zoomPerSecond=1.0]
  *     Sets the zoom amount per second when zoomIn/zoomOut buttons are pressed and held.
  *     The value is a factor of the current zoom, so 1.0 (the default) disables zooming when the zoomIn/zoomOut buttons
  *     are held. Higher values will increase the rate of zoom when the zoomIn/zoomOut buttons are held. Note that values
  *     < 1.0 will reverse the operation of the zoomIn/zoomOut buttons (zoomIn button will decrease the zoom, zoomOut will
  *     increase the zoom).
  *
  * @property {Boolean} [showNavigator=false]
  *     Set to true to make the navigator minimap appear.
  *
+ * @property {Element} [navigatorElement=null]
+ *     The element to hold the navigator minimap.
+ *     If an element is specified, the Id option (see navigatorId) is ignored.
+ *     If no element nor ID is specified, a div element will be generated accordingly.
+ *
  * @property {String} [navigatorId=navigator-GENERATED DATE]
  *     The ID of a div to hold the navigator minimap.
  *     If an ID is specified, the navigatorPosition, navigatorSizeRatio, navigatorMaintainSizeRatio, navigator[Top|Left|Height|Width] and navigatorAutoFade options will be ignored.
  *     If an ID is not specified, a div element will be generated and placed on top of the main image.
  *
  * @property {String} [navigatorPosition='TOP_RIGHT']
  *     Valid values are 'TOP_LEFT', 'TOP_RIGHT', 'BOTTOM_LEFT', 'BOTTOM_RIGHT', or 'ABSOLUTE'.<br>
@@ -464,14 +497,20 @@
  *
  * @property {Number} [maxImageCacheCount=200]
  *     The max number of images we should keep in memory (per drawer).
  *
  * @property {Number} [timeout=30000]
  *     The max number of milliseconds that an image job may take to complete.
  *
+ * @property {Number} [tileRetryMax=0]
+ *     The max number of retries when a tile download fails. By default it's 0, so retries are disabled.
+ *
+ * @property {Number} [tileRetryDelay=2500]
+ *     Milliseconds to wait after each tile retry if tileRetryMax is set.
+ *
  * @property {Boolean} [useCanvas=true]
  *     Set to false to not use an HTML canvas element for image rendering even if canvas is supported.
  *
  * @property {Number} [minPixelRatio=0.5]
  *     The higher the minPixelRatio, the lower the quality of the image that
  *     is considered sufficient to stop rendering a given zoom level.  For
  *     example, if you are targeting mobile devices with less bandwidth you may
@@ -528,58 +567,58 @@
  *     Placement of the default sequence controls.
  *
  * @property {Boolean} [navPrevNextWrap=false]
  *     If true then the 'previous' button will wrap to the last image when
  *     viewing the first image and the 'next' button will wrap to the first
  *     image when viewing the last image.
  *
- * @property {String} zoomInButton
- *     Set the id of the custom 'Zoom in' button to use.
+ *@property {String|Element} zoomInButton
+ *     Set the id or element of the custom 'Zoom in' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} zoomOutButton
- *     Set the id of the custom 'Zoom out' button to use.
+ * @property {String|Element} zoomOutButton
+ *     Set the id or element of the custom 'Zoom out' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} homeButton
- *     Set the id of the custom 'Go home' button to use.
+ * @property {String|Element} homeButton
+ *     Set the id or element of the custom 'Go home' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} fullPageButton
- *     Set the id of the custom 'Toggle full page' button to use.
+ * @property {String|Element} fullPageButton
+ *     Set the id or element of the custom 'Toggle full page' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} rotateLeftButton
- *     Set the id of the custom 'Rotate left' button to use.
+ * @property {String|Element} rotateLeftButton
+ *     Set the id or element of the custom 'Rotate left' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} rotateRightButton
- *     Set the id of the custom 'Rotate right' button to use.
+ * @property {String|Element} rotateRightButton
+ *     Set the id or element of the custom 'Rotate right' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} previousButton
- *     Set the id of the custom 'Previous page' button to use.
+ * @property {String|Element} previousButton
+ *     Set the id or element of the custom 'Previous page' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
- * @property {String} nextButton
- *     Set the id of the custom 'Next page' button to use.
+ * @property {String|Element} nextButton
+ *     Set the id or element of the custom 'Next page' button to use.
  *     This is useful to have a custom button anywhere in the web page.<br>
  *     To only change the button images, consider using
  *     {@link OpenSeadragon.Options.navImages}
  *
  * @property {Boolean} [sequenceMode=false]
  *     Set to true to have the viewer treat your tilesources as a sequence of images to
  *     be opened one at a time rather than all at once.
@@ -650,14 +689,28 @@
  * @property {Boolean} [loadTilesWithAjax=false]
  *     Whether to load tile data using AJAX requests.
  *     Note that this can be overridden at the {@link OpenSeadragon.TileSource} level.
  *
  * @property {Object} [ajaxHeaders={}]
  *     A set of headers to include when making AJAX requests for tile sources or tiles.
  *
+ * @property {Boolean} [splitHashDataForPost=false]
+ *     Allows to treat _first_ hash ('#') symbol as a separator for POST data:
+ *     URL to be opened by a {@link OpenSeadragon.TileSource} can thus look like: http://some.url#postdata=here.
+ *     The whole URL is used to fetch image info metadata and it is then split to 'http://some.url' and
+ *     'postdata=here'; post data is given to the {@link OpenSeadragon.TileSource} of the choice and can be further
+ *     used within tile requests (see TileSource methods).
+ *     NOTE: {@link OpenSeadragon.TileSource.prototype.configure} return value should contain the post data
+ *     if you want to use it later - so that it is given to your constructor later.
+ *     NOTE: usually, post data is expected to be ampersand-separated (just like GET parameters), and is NOT USED
+ *     to fetch tile image data unless explicitly programmed, or if loadTilesWithAjax=false 4
+ *     (but it is still used for the initial image info request).
+ *     NOTE: passing POST data from URL by this feature only supports string values, however,
+ *     TileSource can send any data using POST as long as the header is correct
+ *     (@see OpenSeadragon.TileSource.prototype.getTilePostData)
  */
 
 /**
  * Settings for gestures generated by a pointer device.
  *
  * @typedef {Object} GestureSettings
  * @memberof OpenSeadragon
@@ -768,31 +821,33 @@
      * @property {String} versionStr - The version number as a string ('major.minor.revision').
      * @property {Number} major - The major version number.
      * @property {Number} minor - The minor version number.
      * @property {Number} revision - The revision number.
      * @since 1.0.0
      */
     $.version = {
-        versionStr: '3.0.0',
-        major: parseInt('3', 10),
-        minor: parseInt('0', 10),
+        versionStr: '4.1.0',
+        major: parseInt('4', 10),
+        minor: parseInt('1', 10),
         revision: parseInt('0', 10)
     };
 
 
     /**
      * Taken from jquery 1.6.1
      * [[Class]] -> type pairs
      * @private
      */
     var class2type = {
             '[object Boolean]': 'boolean',
             '[object Number]': 'number',
             '[object String]': 'string',
             '[object Function]': 'function',
+            '[object AsyncFunction]': 'function',
+            '[object Promise]': 'promise',
             '[object Array]': 'array',
             '[object Date]': 'date',
             '[object RegExp]': 'regexp',
             '[object Object]': 'object'
         },
         // Save a reference to some core methods
         toString = Object.prototype.toString,
@@ -804,15 +859,14 @@
      * @memberof OpenSeadragon
      * @see {@link http://www.jquery.com/ jQuery}
      */
     $.isFunction = function(obj) {
         return $.type(obj) === "function";
     };
 
-
     /**
      * Taken from jQuery 1.6.1
      * @function isArray
      * @memberof OpenSeadragon
      * @see {@link http://www.jquery.com/ jQuery}
      */
     $.isArray = Array.isArray || function(obj) {
@@ -890,15 +944,15 @@
         }
         return true;
     };
 
     /**
      * Shim around Object.freeze. Does nothing if Object.freeze is not supported.
      * @param {Object} obj The object to freeze.
-     * @return {Object} obj The frozen object.
+     * @returns {Object} obj The frozen object.
      */
     $.freezeObject = function(obj) {
         if (Object.freeze) {
             $.freezeObject = Object.freeze;
         } else {
             $.freezeObject = function(obj) {
                 return obj;
@@ -1069,24 +1123,37 @@
 
         for (; i < length; i++) {
             // Only deal with non-null/undefined values
             options = arguments[i];
             if (options !== null || options !== undefined) {
                 // Extend the base object
                 for (name in options) {
-                    src = target[name];
-                    copy = options[name];
+                    var descriptor = Object.getOwnPropertyDescriptor(options, name);
+
+                    if (descriptor !== undefined) {
+                        if (descriptor.get || descriptor.set) {
+                            Object.defineProperty(target, name, descriptor);
+                            continue;
+                        }
+
+                        copy = descriptor.value;
+                    } else {
+                        $.console.warn('Could not copy inherited property "' + name + '".');
+                        continue;
+                    }
 
                     // Prevent never-ending loop
                     if (target === copy) {
                         continue;
                     }
 
                     // Recurse if we're merging plain objects or arrays
                     if (deep && copy && (OpenSeadragon.isPlainObject(copy) || (copyIsArray = OpenSeadragon.isArray(copy)))) {
+                        src = target[name];
+
                         if (copyIsArray) {
                             copyIsArray = false;
                             clone = src && OpenSeadragon.isArray(src) ? src : [];
 
                         } else {
                             clone = src && OpenSeadragon.isPlainObject(src) ? src : {};
                         }
@@ -1131,14 +1198,15 @@
             tileSources: null,
             tileHost: null,
             initialPage: 0,
             crossOriginPolicy: false,
             ajaxWithCredentials: false,
             loadTilesWithAjax: false,
             ajaxHeaders: {},
+            splitHashDataForPost: false,
 
             //PAN AND ZOOM SETTINGS AND CONSTRAINTS
             panHorizontal: true,
             panVertical: true,
             constrainDuringPan: false,
             wrapHorizontal: false,
             wrapVertical: false,
@@ -1157,59 +1225,64 @@
             springStiffness: 6.5,
             animationTime: 1.2,
             gestureSettingsMouse: {
                 dragToPan: true,
                 scrollToZoom: true,
                 clickToZoom: true,
                 dblClickToZoom: false,
+                dblClickDragToZoom: false,
                 pinchToZoom: false,
                 zoomToRefPoint: true,
                 flickEnabled: false,
                 flickMinSpeed: 120,
                 flickMomentum: 0.25,
                 pinchRotate: false
             },
             gestureSettingsTouch: {
                 dragToPan: true,
                 scrollToZoom: false,
                 clickToZoom: false,
                 dblClickToZoom: true,
+                dblClickDragToZoom: true,
                 pinchToZoom: true,
                 zoomToRefPoint: true,
                 flickEnabled: true,
                 flickMinSpeed: 120,
                 flickMomentum: 0.25,
                 pinchRotate: false
             },
             gestureSettingsPen: {
                 dragToPan: true,
                 scrollToZoom: false,
                 clickToZoom: true,
                 dblClickToZoom: false,
+                dblClickDragToZoom: false,
                 pinchToZoom: false,
                 zoomToRefPoint: true,
                 flickEnabled: false,
                 flickMinSpeed: 120,
                 flickMomentum: 0.25,
                 pinchRotate: false
             },
             gestureSettingsUnknown: {
                 dragToPan: true,
                 scrollToZoom: false,
                 clickToZoom: false,
                 dblClickToZoom: true,
+                dblClickDragToZoom: false,
                 pinchToZoom: true,
                 zoomToRefPoint: true,
                 flickEnabled: true,
                 flickMinSpeed: 120,
                 flickMomentum: 0.25,
                 pinchRotate: false
             },
             zoomPerClick: 2,
             zoomPerScroll: 1.2,
+            zoomPerDblClickDrag: 1.2,
             zoomPerSecond: 1.0,
             blendTime: 0,
             alwaysBlend: false,
             autoHideControls: true,
             immediateRender: false,
             minZoomImageRatio: 0.9, //-> closer to 0 allows zoom out to infinity
             maxZoomPixelRatio: 1.1, //-> higher allows 'over zoom' into pixels
@@ -1237,14 +1310,15 @@
             showFlipControl: false, //FLIP
             controlsFadeDelay: 2000, //ZOOM/HOME/FULL/SEQUENCE
             controlsFadeLength: 1500, //ZOOM/HOME/FULL/SEQUENCE
             mouseNavEnabled: true, //GENERAL MOUSE INTERACTIVITY
 
             //VIEWPORT NAVIGATOR SETTINGS
             showNavigator: false,
+            navigatorElement: null,
             navigatorId: null,
             navigatorPosition: null,
             navigatorSizeRatio: 0.2,
             navigatorMaintainSizeRatio: false,
             navigatorTop: null,
             navigatorLeft: null,
             navigatorHeight: null,
@@ -1265,14 +1339,15 @@
 
             // APPEARANCE
             opacity: 1,
             preload: false,
             compositeOperation: null,
             imageSmoothingEnabled: true,
             placeholderFillStyle: null,
+            subPixelRoundingForTransparency: null,
 
             //REFERENCE STRIP SETTINGS
             showReferenceStrip: false,
             referenceStripScroll: 'horizontal',
             referenceStripElement: null,
             referenceStripHeight: null,
             referenceStripWidth: null,
@@ -1288,14 +1363,16 @@
             collectionTileMargin: 80,
 
             //PERFORMANCE SETTINGS
             imageLoaderLimit: 0,
             maxImageCacheCount: 200,
             timeout: 30000,
             useCanvas: true, // Use canvas element for drawing if available
+            tileRetryMax: 0,
+            tileRetryDelay: 2500,
 
             //INTERFACE RESOURCE SETTINGS
             prefixUrl: "/images/",
             navImages: {
                 zoomIn: {
                     REST: 'zoomin_rest.png',
                     GROUP: 'zoomin_grouphover.png',
@@ -1350,15 +1427,17 @@
                     HOVER: 'next_hover.png',
                     DOWN: 'next_pressed.png'
                 }
             },
 
             //DEVELOPER SETTINGS
             debugMode: false,
-            debugGridColor: ['#437AB2', '#1B9E77', '#D95F02', '#7570B3', '#E7298A', '#66A61E', '#E6AB02', '#A6761D', '#666666']
+            debugGridColor: ['#437AB2', '#1B9E77', '#D95F02', '#7570B3', '#E7298A', '#66A61E', '#E6AB02', '#A6761D', '#666666'],
+            silenceMultiImageWarnings: false
+
         },
 
 
         /**
          * TODO: get rid of this.  I can't see how it's required at all.  Looks
          *       like an early legacy code artifact.
          * @static
@@ -1406,14 +1485,28 @@
             CHROME: 4,
             OPERA: 5,
             EDGE: 6,
             CHROMEEDGE: 7
         },
 
         /**
+         * An enumeration of when subpixel rounding should occur.
+         * @static
+         * @type {Object}
+         * @property {Number} NEVER Never apply subpixel rounding for transparency.
+         * @property {Number} ONLY_AT_REST Do not apply subpixel rounding for transparency during animation (panning, zoom, rotation) and apply it once animation is over.
+         * @property {Number} ALWAYS Apply subpixel rounding for transparency during animation and when animation is over.
+         */
+        SUBPIXEL_ROUNDING_OCCURRENCES: {
+            NEVER: 0,
+            ONLY_AT_REST: 1,
+            ALWAYS: 2
+        },
+
+        /**
          * Keep track of which {@link Viewer}s have been created.
          * - Key: {@link Element} to which a Viewer is attached.
          * - Value: {@link Viewer} of the element defined by the key.
          * @private
          * @static
          * @type {Object}
          */
@@ -1591,27 +1684,28 @@
          */
         capitalizeFirstLetter: function(string) {
             return string.charAt(0).toUpperCase() + string.slice(1);
         },
 
         /**
          * Compute the modulo of a number but makes sure to always return
-         * a positive value.
-         * @param {Number} number the number to computes the modulo of
+         * a positive value (also known as Euclidean modulo).
+         * @param {Number} number the number to compute the modulo of
          * @param {Number} modulo the modulo
          * @returns {Number} the result of the modulo of number
          */
         positiveModulo: function(number, modulo) {
             var result = number % modulo;
             if (result < 0) {
                 result += modulo;
             }
             return result;
         },
 
+
         /**
          * Determines if a point is within the bounding rectangle of the given element (hit-test).
          * @function
          * @param {Element|String} element
          * @param {OpenSeadragon.Point} point
          * @returns {Boolean}
          */
@@ -1942,15 +2036,15 @@
          * Sets the specified element's pointer-events style attribute to the passed value.
          * @function
          * @param {Element|String} element
          * @param {String} value
          */
         setElementPointerEvents: function(element, value) {
             element = $.getElement(element);
-            if (typeof element.style.pointerEvents !== 'undefined') {
+            if (typeof element.style !== 'undefined' && typeof element.style.pointerEvents !== 'undefined') {
                 element.style.pointerEvents = value;
             }
         },
 
 
         /**
          * Sets the specified element's pointer-events style attribute to 'none'.
@@ -2050,15 +2144,15 @@
          * Convert passed addEventListener() options to boolean or options object,
          * depending on browser support.
          * @function
          * @param {Boolean|Object} [options] Boolean useCapture, or if [supportsEventListenerOptions]{@link OpenSeadragon.supportsEventListenerOptions}, can be an object
          * @param {Boolean} [options.capture]
          * @param {Boolean} [options.passive]
          * @param {Boolean} [options.once]
-         * @return {String} The protocol (http:, https:, file:, ftp: ...)
+         * @returns {String} The protocol (http:, https:, file:, ftp: ...)
          */
         normalizeEventListenerOptions: function(options) {
             var opts;
             if (typeof options !== 'undefined') {
                 if (typeof options === 'boolean') {
                     // Legacy Boolean useCapture
                     opts = $.supportsEventListenerOptions ? {
@@ -2218,15 +2312,15 @@
 
         /**
          * Retrieves the protocol used by the url. The url can either be absolute
          * or relative.
          * @function
          * @private
          * @param {String} url The url to retrieve the protocol from.
-         * @return {String} The protocol (http:, https:, file:, ftp: ...)
+         * @returns {String} The protocol (http:, https:, file:, ftp: ...)
          */
         getUrlProtocol: function(url) {
             var match = url.match(/^([a-z]+:)\/\//i);
             if (match === null) {
                 // Relative URL, retrive the protocol from window.location
                 return window.location.protocol;
             }
@@ -2278,32 +2372,36 @@
         /**
          * Makes an AJAX request.
          * @param {Object} options
          * @param {String} options.url - the url to request
          * @param {Function} options.success - a function to call on a successful response
          * @param {Function} options.error - a function to call on when an error occurs
          * @param {Object} options.headers - headers to add to the AJAX request
-         * @param {String} options.responseType - the response type of the the AJAX request
+         * @param {String} options.responseType - the response type of the AJAX request
+         * @param {String} options.postData - HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+         *      see TileSource::getPostData), GET method used if null
          * @param {Boolean} [options.withCredentials=false] - whether to set the XHR's withCredentials
          * @throws {Error}
          * @returns {XMLHttpRequest}
          */
         makeAjaxRequest: function(url, onSuccess, onError) {
             var withCredentials;
             var headers;
             var responseType;
+            var postData;
 
             // Note that our preferred API is that you pass in a single object; the named
             // arguments are for legacy support.
             if ($.isPlainObject(url)) {
                 onSuccess = url.success;
                 onError = url.error;
                 withCredentials = url.withCredentials;
                 headers = url.headers;
                 responseType = url.responseType || null;
+                postData = url.postData || null;
                 url = url.url;
             }
 
             var protocol = $.getUrlProtocol(url);
             var request = $.createAjaxRequest(protocol === "file:");
 
             if (!$.isFunction(onSuccess)) {
@@ -2319,25 +2417,26 @@
                     // the 200's on Firefox and 0 on other browsers
                     if ((request.status >= 200 && request.status < 300) ||
                         (request.status === 0 &&
                             protocol !== "http:" &&
                             protocol !== "https:")) {
                         onSuccess(request);
                     } else {
-                        $.console.log("AJAX request returned %d: %s", request.status, url);
-
                         if ($.isFunction(onError)) {
                             onError(request);
+                        } else {
+                            $.console.error("AJAX request returned %d: %s", request.status, url);
                         }
                     }
                 }
             };
 
+            var method = postData ? "POST" : "GET";
             try {
-                request.open("GET", url, true);
+                request.open(method, url, true);
 
                 if (responseType) {
                     request.responseType = responseType;
                 }
 
                 if (headers) {
                     for (var headerName in headers) {
@@ -2347,17 +2446,17 @@
                     }
                 }
 
                 if (withCredentials) {
                     request.withCredentials = true;
                 }
 
-                request.send(null);
+                request.send(postData);
             } catch (e) {
-                $.console.log("%s while making AJAX request: %s", e.name, e.message);
+                $.console.error("%s while making AJAX request: %s", e.name, e.message);
 
                 request.onreadystatechange = function() {};
 
                 if ($.isFunction(onError)) {
                     onError(request, e);
                 }
             }
@@ -2817,15 +2916,15 @@
     return OpenSeadragon;
 }));
 
 /*
  * OpenSeadragon - full-screen support functions
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -2967,15 +3066,15 @@
 
 })(OpenSeadragon);
 
 /*
  * OpenSeadragon - EventSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -3023,55 +3122,65 @@
     };
 
     /** @lends OpenSeadragon.EventSource.prototype */
     $.EventSource.prototype = {
 
         /**
          * Add an event handler to be triggered only once (or a given number of times)
-         * for a given event.
+         * for a given event. It is not removable with removeHandler().
          * @function
          * @param {String} eventName - Name of event to register.
          * @param {OpenSeadragon.EventHandler} handler - Function to call when event
          * is triggered.
          * @param {Object} [userData=null] - Arbitrary object to be passed unchanged
          * to the handler.
          * @param {Number} [times=1] - The number of times to handle the event
          * before removing it.
+         * @param {Number} [priority=0] - Handler priority. By default, all priorities are 0. Higher number = priority.
          */
-        addOnceHandler: function(eventName, handler, userData, times) {
+        addOnceHandler: function(eventName, handler, userData, times, priority) {
             var self = this;
             times = times || 1;
             var count = 0;
             var onceHandler = function(event) {
                 count++;
                 if (count === times) {
                     self.removeHandler(eventName, onceHandler);
                 }
-                handler(event);
+                return handler(event);
             };
-            this.addHandler(eventName, onceHandler, userData);
+            this.addHandler(eventName, onceHandler, userData, priority);
         },
 
         /**
          * Add an event handler for a given event.
          * @function
          * @param {String} eventName - Name of event to register.
          * @param {OpenSeadragon.EventHandler} handler - Function to call when event is triggered.
          * @param {Object} [userData=null] - Arbitrary object to be passed unchanged to the handler.
+         * @param {Number} [priority=0] - Handler priority. By default, all priorities are 0. Higher number = priority.
          */
-        addHandler: function(eventName, handler, userData) {
+        addHandler: function(eventName, handler, userData, priority) {
             var events = this.events[eventName];
             if (!events) {
                 this.events[eventName] = events = [];
             }
             if (handler && $.isFunction(handler)) {
-                events[events.length] = {
-                    handler: handler,
-                    userData: userData || null
-                };
+                var index = events.length,
+                    event = {
+                        handler: handler,
+                        userData: userData || null,
+                        priority: priority || 0
+                    };
+                events[index] = event;
+                while (index > 0 && events[index - 1].priority < events[index].priority) {
+                    events[index] = events[index - 1];
+                    events[index - 1] = event;
+                    index--;
+                }
             }
         },
 
         /**
          * Remove a specific event handler for a given event.
          * @function
          * @param {String} eventName - Name of event for which the handler is to be removed.
@@ -3090,14 +3199,26 @@
                         handlers.push(events[i]);
                     }
                 }
                 this.events[eventName] = handlers;
             }
         },
 
+        /**
+         * Get the amount of handlers registered for a given event.
+         * @param {String} eventName - Name of event to inspect.
+         * @returns {number} amount of events
+         */
+        numberOfHandlers: function(eventName) {
+            var events = this.events[eventName];
+            if (!events) {
+                return 0;
+            }
+            return events.length;
+        },
 
         /**
          * Remove all event handlers for a given event type. If no type is given all
          * event handlers for every event type are removed.
          * @function
          * @param {String} eventName - Name of event for which all handlers are to be removed.
          */
@@ -3141,33 +3262,30 @@
          * @function
          * @param {String} eventName - Name of event to register.
          * @param {Object} eventArgs - Event-specific data.
          */
         raiseEvent: function(eventName, eventArgs) {
             //uncomment if you want to get a log of all events
             //$.console.log( eventName );
-            var handler = this.getHandler(eventName);
 
+            var handler = this.getHandler(eventName);
             if (handler) {
-                if (!eventArgs) {
-                    eventArgs = {};
-                }
-
-                handler(this, eventArgs);
+                return handler(this, eventArgs || {});
             }
+            return undefined;
         }
     };
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - MouseTracker
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -3322,16 +3440,16 @@
          * will be treated as a double-click gesture.
          * @member {Number} dblClickTimeThreshold
          * @memberof OpenSeadragon.MouseTracker#
          */
         this.dblClickTimeThreshold = options.dblClickTimeThreshold || $.DEFAULT_SETTINGS.dblClickTimeThreshold;
         /**
          * The maximum distance allowed between two pointer click events
-         * to be treated as a click gesture.
-         * @member {Number} clickDistThreshold
+         * to be treated as a double-click gesture.
+         * @member {Number} dblClickDistThreshold
          * @memberof OpenSeadragon.MouseTracker#
          */
         this.dblClickDistThreshold = options.dblClickDistThreshold || $.DEFAULT_SETTINGS.dblClickDistThreshold;
         /*eslint-disable no-multi-spaces*/
         this.userData = options.userData || null;
         this.stopDelay = options.stopDelay || 50;
 
@@ -4635,15 +4753,14 @@
          * It will make sure the count does not go below 0.
          * @function
          */
         removeContact: function() {
             --this.contacts;
 
             if (this.contacts < 0) {
-                $.console.warn('GesturePointList.removeContact() Implausible contacts value');
                 this.contacts = 0;
             }
         }
     };
 
 
     ///////////////////////////////////////////////////////////////////////////////
@@ -6054,18 +6171,15 @@
                 $.console.warn('stopTrackingPointer() called on captured pointer');
                 releasePointer(tracker, trackedGPoint);
             }
 
             // If child element relinquishes capture to a parent we may get here
             //   from a pointerleave event while a pointerup event will never be received.
             //   In that case, we'll clean up the contact count
-            if ((pointsList.type === 'mouse' || pointsList.type === 'pen') &&
-                pointsList.contacts > 0) {
-                pointsList.removeContact();
-            }
+            pointsList.removeContact();
 
             listLength = pointsList.removeById(gPoint.id);
         } else {
             listLength = pointsList.getLength();
         }
 
         return listLength;
@@ -6515,21 +6629,20 @@
             updateGPoint.lastTime = updateGPoint.currentTime;
             updateGPoint.currentPos = gPoint.currentPos;
             updateGPoint.currentTime = gPoint.currentTime;
 
             gPoint = updateGPoint;
         } else {
             // Initialize for tracking and add to the tracking list (no pointerenter event occurred before this)
-            $.console.warn('pointerdown event on untracked pointer');
+            // NOTE: pointerdown event on untracked pointer
             gPoint.captured = false; // Handled by updatePointerCaptured()
             gPoint.insideElementPressed = true;
             gPoint.insideElement = true;
             gPoint.originalTarget = eventInfo.originalEvent.target;
             startTrackingPointer(pointsList, gPoint);
-            return;
         }
 
         pointsList.addContact();
         //$.console.log('contacts++ ', pointsList.contacts);
 
         if (!eventInfo.preventGesture && !eventInfo.defaultPrevented) {
             eventInfo.shouldCapture = true;
@@ -6661,16 +6774,16 @@
             if (!updateGPoint.insideElement) {
                 stopTrackingPointer(tracker, pointsList, updateGPoint);
             }
 
             releasePoint = updateGPoint.currentPos;
             releaseTime = updateGPoint.currentTime;
         } else {
-            // should never get here...we'll start to track pointer anyway
-            $.console.warn('updatePointerUp(): pointerup on untracked gPoint');
+            // NOTE: updatePointerUp(): pointerup on untracked gPoint
+            // ...we'll start to track pointer again
             gPoint.captured = false; // Handled by updatePointerCaptured()
             gPoint.insideElementPressed = false;
             gPoint.insideElement = true;
             startTrackingPointer(pointsList, gPoint);
 
             updateGPoint = gPoint;
         }
@@ -6685,15 +6798,15 @@
                 if (tracker.dragHandler || tracker.dragEndHandler || tracker.pinchHandler) {
                     $.MouseTracker.gesturePointVelocityTracker.removePoint(tracker, updateGPoint);
                 }
 
                 if (pointsList.contacts === 0) {
 
                     // Release (pressed in our element)
-                    if (tracker.releaseHandler) {
+                    if (tracker.releaseHandler && releasePoint) {
                         tracker.releaseHandler({
                             eventSource: tracker,
                             pointerType: updateGPoint.type,
                             position: getPointRelativeToAbsolute(releasePoint, tracker.element),
                             buttons: pointsList.buttons,
                             insideElementPressed: updateGPoint.insideElementPressed,
                             insideElementReleased: updateGPoint.insideElement,
@@ -6779,15 +6892,15 @@
                 }
             } else {
                 // Pointer was activated in another element but removed in our element
 
                 eventInfo.shouldReleaseCapture = false;
 
                 // Release (pressed in another element)
-                if (tracker.releaseHandler) {
+                if (tracker.releaseHandler && releasePoint) {
                     tracker.releaseHandler({
                         eventSource: tracker,
                         pointerType: updateGPoint.type,
                         position: getPointRelativeToAbsolute(releasePoint, tracker.element),
                         buttons: pointsList.buttons,
                         insideElementPressed: updateGPoint.insideElementPressed,
                         insideElementReleased: updateGPoint.insideElement,
@@ -6984,15 +7097,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Control
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -7056,14 +7169,15 @@
      *  relative to the container.
      * @param {Boolean} [options.attachToViewer=true] - Whether the control should be added directly to the viewer, or
      *  directly to the container
      * @param {Boolean} [options.autoFade=true] - Whether the control should have the autofade behavior
      * @param {Element} container - the element to control will be anchored too.
      */
     $.Control = function(element, options, container) {
+
         var parent = element.parentNode;
         if (typeof options === 'number') {
             $.console.error("Passing an anchor directly into the OpenSeadragon.Control constructor is deprecated; " +
                 "please use an options object instead.  " +
                 "Support for this deprecated variant is scheduled for removal in December 2013");
             options = {
                 anchor: options
@@ -7133,14 +7247,15 @@
                 );
             } else {
                 this.container.appendChild(this.wrapper);
             }
         } else {
             parent.appendChild(this.wrapper);
         }
+
     };
 
     /** @lends OpenSeadragon.Control.prototype */
     $.Control.prototype = {
 
         /**
          * Removes the control from the container.
@@ -7152,15 +7267,15 @@
                 this.container.removeChild(this.wrapper);
             }
         },
 
         /**
          * Determines if the control is currently visible.
          * @function
-         * @return {Boolean} true if currently visible, false otherwise.
+         * @returns {Boolean} true if currently visible, false otherwise.
          */
         isVisible: function() {
             return this.wrapper.style.display !== "none";
         },
 
         /**
          * Toggles the visibility of the control.
@@ -7189,15 +7304,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - ControlDock
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -7336,15 +7451,15 @@
             );
             element.style.display = "inline-block";
         },
 
 
         /**
          * @function
-         * @return {OpenSeadragon.ControlDock} Chainable.
+         * @returns {OpenSeadragon.ControlDock} Chainable.
          */
         removeControl: function(element) {
             element = $.getElement(element);
             var i = getControlIndex(this, element);
 
             if (i >= 0) {
                 this.controls[i].destroy();
@@ -7352,28 +7467,28 @@
             }
 
             return this;
         },
 
         /**
          * @function
-         * @return {OpenSeadragon.ControlDock} Chainable.
+         * @returns {OpenSeadragon.ControlDock} Chainable.
          */
         clearControls: function() {
             while (this.controls.length > 0) {
                 this.controls.pop().destroy();
             }
 
             return this;
         },
 
 
         /**
          * @function
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         areControlsEnabled: function() {
             var i;
 
             for (i = this.controls.length - 1; i >= 0; i--) {
                 if (this.controls[i].isVisible()) {
                     return true;
@@ -7382,15 +7497,15 @@
 
             return false;
         },
 
 
         /**
          * @function
-         * @return {OpenSeadragon.ControlDock} Chainable.
+         * @returns {OpenSeadragon.ControlDock} Chainable.
          */
         setControlsEnabled: function(enabled) {
             var i;
 
             for (i = this.controls.length - 1; i >= 0; i--) {
                 this.controls[i].setVisible(enabled);
             }
@@ -7558,15 +7673,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Viewer
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -7738,15 +7853,15 @@
             collectionDrawer: null,
 
             //UI image resources
             //TODO: rename navImages to uiImages
             navImages: null,
 
             //interface button controls
-            buttons: null,
+            buttonGroup: null,
 
             //TODO: this is defunct so safely remove it
             profiler: null
 
         }, $.DEFAULT_SETTINGS, options);
 
         if (typeof(this.hash) === "undefined") {
@@ -7760,23 +7875,27 @@
 
         //Private state properties
         THIS[this.hash] = {
             fsBoundsDelta: new $.Point(1, 1),
             prevContainerSize: null,
             animating: false,
             forceRedraw: false,
+            needsResize: false,
+            forceResize: false,
             mouseInside: false,
             group: null,
             // whether we should be continuously zooming
             zooming: false,
             // how much we should be continuously zooming by
             zoomFactor: null,
             lastZoomTime: null,
             fullPage: false,
-            onfullscreenchange: null
+            onfullscreenchange: null,
+            lastClickTime: null,
+            draggingToZoom: false,
         };
 
         this._sequenceIndex = 0;
         this._firstOpen = true;
         this._updateRequestId = null;
         this._loadQueue = [];
         this.currentOverlays = [];
@@ -7859,15 +7978,17 @@
             enterHandler: $.delegate(this, onCanvasEnter),
             leaveHandler: $.delegate(this, onCanvasLeave),
             pressHandler: $.delegate(this, onCanvasPress),
             releaseHandler: $.delegate(this, onCanvasRelease),
             nonPrimaryPressHandler: $.delegate(this, onCanvasNonPrimaryPress),
             nonPrimaryReleaseHandler: $.delegate(this, onCanvasNonPrimaryRelease),
             scrollHandler: $.delegate(this, onCanvasScroll),
-            pinchHandler: $.delegate(this, onCanvasPinch)
+            pinchHandler: $.delegate(this, onCanvasPinch),
+            focusHandler: $.delegate(this, onCanvasFocus),
+            blurHandler: $.delegate(this, onCanvasBlur),
         });
 
         this.outerTracker = new $.MouseTracker({
             userData: 'Viewer.outerTracker',
             element: this.container,
             startDisabled: !this.mouseNavEnabled,
             clickTimeThreshold: this.clickTimeThreshold,
@@ -7884,14 +8005,25 @@
             });
         }
 
         this.bindStandardControls();
 
         THIS[this.hash].prevContainerSize = _getSafeElemSize(this.container);
 
+        if (window.ResizeObserver) {
+            this._autoResizePolling = false;
+            this._resizeObserver = new ResizeObserver(function() {
+                THIS[_this.hash].needsResize = true;
+            });
+
+            this._resizeObserver.observe(this.container, {});
+        } else {
+            this._autoResizePolling = true;
+        }
+
         // Create the world
         this.world = new $.World({
             viewer: this
         });
 
         this.world.addHandler('add-item', function(event) {
             // For backwards compatibility, we maintain the source property
@@ -7940,23 +8072,26 @@
             minZoomLevel: this.minZoomLevel,
             maxZoomLevel: this.maxZoomLevel,
             viewer: this,
             degrees: this.degrees,
             flipped: this.flipped,
             navigatorRotate: this.navigatorRotate,
             homeFillsViewer: this.homeFillsViewer,
-            margins: this.viewportMargins
+            margins: this.viewportMargins,
+            silenceMultiImageWarnings: this.silenceMultiImageWarnings
         });
 
         this.viewport._setContentBounds(this.world.getHomeBounds(), this.world.getContentFactor());
 
         // Create the image loader
         this.imageLoader = new $.ImageLoader({
             jobLimit: this.imageLoaderLimit,
-            timeout: options.timeout
+            timeout: options.timeout,
+            tileRetryMax: this.tileRetryMax,
+            tileRetryDelay: this.tileRetryDelay
         });
 
         // Create the tile cache
         this.tileCache = new $.TileCache({
             maxImageCacheCount: this.maxImageCacheCount
         });
 
@@ -7988,14 +8123,15 @@
         }
 
         this._addUpdatePixelDensityRatioEvent();
 
         //Instantiate a navigator if configured
         if (this.showNavigator) {
             this.navigator = new $.Navigator({
+                element: this.navigatorElement,
                 id: this.navigatorId,
                 position: this.navigatorPosition,
                 sizeRatio: this.navigatorSizeRatio,
                 maintainSizeRatio: this.navigatorMaintainSizeRatio,
                 top: this.navigatorTop,
                 left: this.navigatorLeft,
                 width: this.navigatorWidth,
@@ -8005,15 +8141,16 @@
                 prefixUrl: this.prefixUrl,
                 viewer: this,
                 navigatorRotate: this.navigatorRotate,
                 background: this.navigatorBackground,
                 opacity: this.navigatorOpacity,
                 borderColor: this.navigatorBorderColor,
                 displayRegionColor: this.navigatorDisplayRegionColor,
-                crossOriginPolicy: this.crossOriginPolicy
+                crossOriginPolicy: this.crossOriginPolicy,
+                animationTime: this.animationTime,
             });
         }
 
         // Sequence mode
         if (this.sequenceMode) {
             this.bindSequenceControls();
         }
@@ -8047,15 +8184,15 @@
     };
 
     $.extend($.Viewer.prototype, $.EventSource.prototype, $.ControlDock.prototype, /** @lends OpenSeadragon.Viewer.prototype */ {
 
 
         /**
          * @function
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         isOpen: function() {
             return !!this.world.getItemCount();
         },
 
         // deprecated
         openDzi: function(dzi) {
@@ -8065,29 +8202,35 @@
 
         // deprecated
         openTileSource: function(tileSource) {
             $.console.error("[Viewer.openTileSource] this function is deprecated; use Viewer.open() instead.");
             return this.open(tileSource);
         },
 
+        //deprecated
+        get buttons() {
+            $.console.warn('Viewer.buttons is deprecated; Please use Viewer.buttonGroup');
+            return this.buttonGroup;
+        },
+
         /**
          * Open tiled images into the viewer, closing any others.
          * To get the TiledImage instance created by open, add an event listener for
          * {@link OpenSeadragon.Viewer.html#.event:open}, which when fired can be used to get access
          * to the instance, i.e., viewer.world.getItemAt(0).
          * @function
          * @param {Array|String|Object|Function} tileSources - This can be a TiledImage
          * specifier, a TileSource specifier, or an array of either. A TiledImage specifier
          * is the same as the options parameter for {@link OpenSeadragon.Viewer#addTiledImage},
          * except for the index property; images are added in sequence.
          * A TileSource specifier is anything you could pass as the tileSource property
          * of the options parameter for {@link OpenSeadragon.Viewer#addTiledImage}.
          * @param {Number} initialPage - If sequenceMode is true, display this page initially
          * for the given tileSources. If specified, will overwrite the Viewer's existing initialPage property.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:open
          * @fires OpenSeadragon.Viewer.event:open-failed
          */
         open: function(tileSources, initialPage) {
             var _this = this;
 
             this.close();
@@ -8253,15 +8396,15 @@
 
             return this;
         },
 
 
         /**
          * @function
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:close
          */
         close: function() {
             if (!THIS[this.hash]) {
                 //this viewer has already been destroyed: returning immediately
                 return this;
             }
@@ -8274,14 +8417,15 @@
 
             if (!this.preserveOverlays) {
                 this.clearOverlays();
                 this.overlaysContainer.innerHTML = "";
             }
 
             THIS[this.hash].animating = false;
+
             this.world.removeAll();
             this.imageLoader.clear();
 
             /**
              * Raised when the viewer is closed (see {@link OpenSeadragon.Viewer#close}).
              *
              * @event close
@@ -8305,31 +8449,47 @@
          * });
          *
          * //when you are done with the viewer:
          * viewer.destroy();
          * viewer = null; //important
          *
          * @function
+         * @fires OpenSeadragon.Viewer.event:before-destroy
+         * @fires OpenSeadragon.Viewer.event:destroy
          */
         destroy: function() {
             if (!THIS[this.hash]) {
                 //this viewer has already been destroyed: returning immediately
                 return;
             }
 
+            /**
+             * Raised when the viewer is about to be destroyed (see {@link OpenSeadragon.Viewer#before-destroy}).
+             *
+             * @event before-destroy
+             * @memberof OpenSeadragon.Viewer
+             * @type {object}
+             * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
+             * @property {?Object} userData - Arbitrary subscriber-defined object.
+             */
+            this.raiseEvent('before-destroy');
+
             this._removeUpdatePixelDensityRatioEvent();
 
             this.close();
 
             this.clearOverlays();
             this.overlaysContainer.innerHTML = "";
 
             //TODO: implement this...
             //this.unbindSequenceControls()
             //this.unbindStandardControls()
+            if (this._resizeObserver) {
+                this._resizeObserver.disconnect();
+            }
 
             if (this.referenceStrip) {
                 this.referenceStrip.destroy();
                 this.referenceStrip = null;
             }
 
             if (this._updateRequestId !== null) {
@@ -8344,15 +8504,14 @@
             if (this.navigator) {
                 this.navigator.destroy();
                 THIS[this.navigator.hash] = null;
                 delete THIS[this.navigator.hash];
                 this.navigator = null;
             }
 
-            this.removeAllHandlers();
 
             if (this.buttonGroup) {
                 this.buttonGroup.destroy();
             } else if (this.customButtons) {
                 while (this.customButtons.length) {
                     this.customButtons.pop().destroy();
                 }
@@ -8390,28 +8549,41 @@
             this.container = null;
 
             // Unregister the viewer
             $._viewers.delete(this.element);
 
             // clear our reference to the main element - they will need to pass it in again, creating a new viewer
             this.element = null;
+
+            /**
+             * Raised when the viewer is destroyed (see {@link OpenSeadragon.Viewer#destroy}).
+             *
+             * @event destroy
+             * @memberof OpenSeadragon.Viewer
+             * @type {object}
+             * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
+             * @property {?Object} userData - Arbitrary subscriber-defined object.
+             */
+            this.raiseEvent('destroy');
+
+            this.removeAllHandlers();
         },
 
         /**
          * @function
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         isMouseNavEnabled: function() {
             return this.innerTracker.isTracking();
         },
 
         /**
          * @function
          * @param {Boolean} enabled - true to enable, false to disable
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:mouse-enabled
          */
         setMouseNavEnabled: function(enabled) {
             this.innerTracker.setTracking(enabled);
             this.outerTracker.setTracking(enabled);
             /**
              * Raised when mouse/touch navigation is enabled or disabled (see {@link OpenSeadragon.Viewer#setMouseNavEnabled}).
@@ -8428,15 +8600,15 @@
             });
             return this;
         },
 
 
         /**
          * @function
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         areControlsEnabled: function() {
             var enabled = this.controls.length,
                 i;
             for (i = 0; i < this.controls.length; i++) {
                 enabled = enabled && this.controls[i].isVisible();
             }
@@ -8445,15 +8617,15 @@
 
 
         /**
          * Shows or hides the controls (e.g. the default navigation buttons).
          *
          * @function
          * @param {Boolean} true to show, false to hide.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:controls-enabled
          */
         setControlsEnabled: function(enabled) {
             if (enabled) {
                 abortControlsAutoHide(this);
             } else {
                 beginControlsAutoHide(this);
@@ -8474,41 +8646,98 @@
             return this;
         },
 
         /**
          * Turns debugging mode on or off for this viewer.
          *
          * @function
-         * @param {Boolean} true to turn debug on, false to turn debug off.
+         * @param {Boolean} debugMode true to turn debug on, false to turn debug off.
          */
         setDebugMode: function(debugMode) {
 
             for (var i = 0; i < this.world.getItemCount(); i++) {
                 this.world.getItemAt(i).debugMode = debugMode;
             }
 
             this.debugMode = debugMode;
             this.forceRedraw();
         },
 
         /**
+         * Update headers to include when making AJAX requests.
+         *
+         * Unless `propagate` is set to false (which is likely only useful in rare circumstances),
+         * the updated headers are propagated to all tiled images, each of which will subsequently
+         * propagate the changed headers to all their tiles.
+         * If applicable, the headers of the viewer's navigator and reference strip will also be updated.
+         *
+         * Note that the rules for merging headers still apply, i.e. headers returned by
+         * {@link OpenSeadragon.TileSource#getTileAjaxHeaders} take precedence over
+         * `TiledImage.ajaxHeaders`, which take precedence over the headers here in the viewer.
+         *
+         * @function
+         * @param {Object} ajaxHeaders Updated AJAX headers.
+         * @param {Boolean} [propagate=true] Whether to propagate updated headers to tiled images, etc.
+         */
+        setAjaxHeaders: function(ajaxHeaders, propagate) {
+            if (ajaxHeaders === null) {
+                ajaxHeaders = {};
+            }
+            if (!$.isPlainObject(ajaxHeaders)) {
+                console.error('[Viewer.setAjaxHeaders] Ignoring invalid headers, must be a plain object');
+                return;
+            }
+            if (propagate === undefined) {
+                propagate = true;
+            }
+
+            this.ajaxHeaders = ajaxHeaders;
+
+            if (propagate) {
+                for (var i = 0; i < this.world.getItemCount(); i++) {
+                    this.world.getItemAt(i)._updateAjaxHeaders(true);
+                }
+
+                if (this.navigator) {
+                    this.navigator.setAjaxHeaders(this.ajaxHeaders, true);
+                }
+
+                if (this.referenceStrip && this.referenceStrip.miniViewers) {
+                    for (var key in this.referenceStrip.miniViewers) {
+                        this.referenceStrip.miniViewers[key].setAjaxHeaders(this.ajaxHeaders, true);
+                    }
+                }
+            }
+        },
+
+        /**
+         * Adds the given button to this viewer.
+         *
          * @function
-         * @return {Boolean}
+         * @param {OpenSeadragon.Button} button
+         */
+        addButton: function(button) {
+            this.buttonGroup.addButton(button);
+        },
+
+        /**
+         * @function
+         * @returns {Boolean}
          */
         isFullPage: function() {
             return THIS[this.hash].fullPage;
         },
 
 
         /**
          * Toggle full page mode.
          * @function
          * @param {Boolean} fullPage
          *      If true, enter full page mode.  If false, exit full page mode.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:pre-full-page
          * @fires OpenSeadragon.Viewer.event:full-page
          */
         setFullPage: function(fullPage) {
 
             var body = document.body,
                 bodyStyle = body.style,
@@ -8604,16 +8833,16 @@
                     //on the mode
                     $.addClass(this.toolbar.element, 'fullpage');
                 }
 
                 $.addClass(this.element, 'fullpage');
                 body.appendChild(this.element);
 
-                this.element.style.height = $.getWindowSize().y + 'px';
-                this.element.style.width = $.getWindowSize().x + 'px';
+                this.element.style.height = '100vh';
+                this.element.style.width = '100vw';
 
                 if (this.toolbar && this.toolbar.element) {
                     this.element.style.height = (
                         $.getElementSize(this.element).y - $.getElementSize(this.toolbar.element).y
                     ) + 'px';
                 }
 
@@ -8717,15 +8946,15 @@
         },
 
         /**
          * Toggle full screen mode if supported. Toggle full page mode otherwise.
          * @function
          * @param {Boolean} fullScreen
          *      If true, enter full screen mode.  If false, exit full screen mode.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:pre-full-screen
          * @fires OpenSeadragon.Viewer.event:full-screen
          */
         setFullScreen: function(fullScreen) {
             var _this = this;
 
             if (!$.supportsFullScreen) {
@@ -8814,25 +9043,34 @@
                 $.exitFullScreen();
             }
             return this;
         },
 
         /**
          * @function
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         isVisible: function() {
             return this.container.style.visibility !== "hidden";
         },
 
 
+        //
+        /**
+         * @function
+         * @returns {Boolean} returns true if the viewer is in fullscreen
+         */
+        isFullScreen: function() {
+            return $.isFullScreen() && this.isFullPage();
+        },
+
         /**
          * @function
          * @param {Boolean} visible
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:visible
          */
         setVisible: function(visible) {
             this.container.style.visibility = visible ? "" : "hidden";
             /**
              * Raised when the viewer is shown or hidden (see {@link OpenSeadragon.Viewer#setVisible}).
              *
@@ -8897,15 +9135,14 @@
          * @param {Boolean} [options.loadTilesWithAjax]
          *      Whether to load tile data using AJAX requests.
          *      Defaults to the setting in {@link OpenSeadragon.Options}.
          * @param {Object} [options.ajaxHeaders]
          *      A set of headers to include when making tile AJAX requests.
          *      Note that these headers will be merged over any headers specified in {@link OpenSeadragon.Options}.
          *      Specifying a falsy value for a header will clear its existing value set at the Viewer level (if any).
-         * requests.
          * @param {Function} [options.success] A function that gets called when the image is
          * successfully added. It's passed the event object which contains a single property:
          * "item", which is the resulting instance of TiledImage.
          * @param {Function} [options.error] A function that gets called if the image is
          * unable to be added. It's passed the error event object, which contains "message"
          * and "source" properties.
          * @param {Boolean} [options.collectionImmediately=false] If collectionMode is on,
@@ -8945,18 +9182,16 @@
             }
             if (options.ajaxWithCredentials === undefined) {
                 options.ajaxWithCredentials = this.ajaxWithCredentials;
             }
             if (options.loadTilesWithAjax === undefined) {
                 options.loadTilesWithAjax = this.loadTilesWithAjax;
             }
-            if (options.ajaxHeaders === undefined || options.ajaxHeaders === null) {
-                options.ajaxHeaders = this.ajaxHeaders;
-            } else if ($.isPlainObject(options.ajaxHeaders) && $.isPlainObject(this.ajaxHeaders)) {
-                options.ajaxHeaders = $.extend({}, this.ajaxHeaders, options.ajaxHeaders);
+            if (!$.isPlainObject(options.ajaxHeaders)) {
+                options.ajaxHeaders = {};
             }
 
             var myQueueItem = {
                 options: options
             };
 
             function raiseAddItemFailed(event) {
@@ -9065,15 +9300,16 @@
                         minPixelRatio: _this.minPixelRatio,
                         smoothTileEdgesMinZoom: _this.smoothTileEdgesMinZoom,
                         iOSDevice: _this.iOSDevice,
                         crossOriginPolicy: queueItem.options.crossOriginPolicy,
                         ajaxWithCredentials: queueItem.options.ajaxWithCredentials,
                         loadTilesWithAjax: queueItem.options.loadTilesWithAjax,
                         ajaxHeaders: queueItem.options.ajaxHeaders,
-                        debugMode: _this.debugMode
+                        debugMode: _this.debugMode,
+                        subPixelRoundingForTransparency: _this.subPixelRoundingForTransparency
                     });
 
                     if (_this.collectionMode) {
                         _this.world.setAutoRefigureSizes(false);
                     }
 
                     if (_this.navigator) {
@@ -9205,16 +9441,24 @@
          */
         forceRedraw: function() {
             THIS[this.hash].forceRedraw = true;
             return this;
         },
 
         /**
+         * Force the viewer to reset its size to match its container.
+         */
+        forceResize: function() {
+            THIS[this.hash].needsResize = true;
+            THIS[this.hash].forceResize = true;
+        },
+
+        /**
          * @function
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          */
         bindSequenceControls: function() {
 
             //////////////////////////////////////////////////////////////////////////
             // Image Sequence Controls
             //////////////////////////////////////////////////////////////////////////
             var onFocusHandler = $.delegate(this, onFocus),
@@ -9297,15 +9541,15 @@
             }
             return this;
         },
 
 
         /**
          * @function
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          */
         bindStandardControls: function() {
             //////////////////////////////////////////////////////////////////////////
             // Navigation Controls
             //////////////////////////////////////////////////////////////////////////
             var beginZoomingInHandler = $.delegate(this, beginZoomingIn),
                 endZoomingHandler = $.delegate(this, endZooming),
@@ -9481,23 +9725,23 @@
             }
             return this;
         },
 
         /**
          * Gets the active page of a sequence
          * @function
-         * @return {Number}
+         * @returns {Number}
          */
         currentPage: function() {
             return this._sequenceIndex;
         },
 
         /**
          * @function
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:page
          */
         goToPage: function(page) {
             if (this.tileSources && page >= 0 && page < this.tileSources.length) {
                 this._sequenceIndex = page;
 
                 this._updateSequenceButtons(page);
@@ -9540,15 +9784,15 @@
          *      rectangle which will be overlaid. This is a viewport relative location.
          * @param {OpenSeadragon.Placement} [placement=OpenSeadragon.Placement.TOP_LEFT] - The position of the
          *      viewport which the location coordinates will be treated as relative
          *      to.
          * @param {function} [onDraw] - If supplied the callback is called when the overlay
          *      needs to be drawn. It it the responsibility of the callback to do any drawing/positioning.
          *      It is passed position, size and element.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:add-overlay
          */
         addOverlay: function(element, location, placement, onDraw) {
             var options;
             if ($.isPlainObject(element)) {
                 options = element;
             } else {
@@ -9598,15 +9842,15 @@
          * @param {Element|String} element - A reference to an element or an id for
          *      the element which is overlaid.
          * @param {OpenSeadragon.Point|OpenSeadragon.Rect} location - The point or
          *      rectangle which will be overlaid. This is a viewport relative location.
          * @param {OpenSeadragon.Placement} [placement=OpenSeadragon.Placement.TOP_LEFT] - The position of the
          *      viewport which the location coordinates will be treated as relative
          *      to.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:update-overlay
          */
         updateOverlay: function(element, location, placement) {
             var i;
 
             element = $.getElement(element);
             i = getOverlayIndex(this.currentOverlays, element);
@@ -9639,15 +9883,15 @@
 
         /**
          * Removes an overlay identified by the reference element or element id
          * and schedules an update.
          * @method
          * @param {Element|String} element - A reference to the element or an
          *      element id which represent the ovelay content to be removed.
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:remove-overlay
          */
         removeOverlay: function(element) {
             var i;
 
             element = $.getElement(element);
             i = getOverlayIndex(this.currentOverlays, element);
@@ -9675,15 +9919,15 @@
             return this;
         },
 
         /**
          * Removes all currently configured Overlays from this Viewer and schedules
          * an update.
          * @method
-         * @return {OpenSeadragon.Viewer} Chainable.
+         * @returns {OpenSeadragon.Viewer} Chainable.
          * @fires OpenSeadragon.Viewer.event:clear-overlay
          */
         clearOverlays: function() {
             while (this.currentOverlays.length > 0) {
                 this.currentOverlays.pop().destroy();
             }
             THIS[this.hash].forceRedraw = true;
@@ -9702,15 +9946,15 @@
 
         /**
          * Finds an overlay identified by the reference element or element id
          * and returns it as an object, return null if not found.
          * @method
          * @param {Element|String} element - A reference to the element or an
          *      element id which represents the overlay content.
-         * @return {OpenSeadragon.Overlay} the matching overlay or null if none found.
+         * @returns {OpenSeadragon.Overlay} the matching overlay or null if none found.
          */
         getOverlayById: function(element) {
             var i;
 
             element = $.getElement(element);
             i = getOverlayIndex(this.currentOverlays, element);
 
@@ -9783,15 +10027,15 @@
             }
         },
 
         /**
          * Gets this viewer's gesture settings for the given pointer device type.
          * @method
          * @param {String} type - The pointer device type to get the gesture settings for ("mouse", "touch", "pen", etc.).
-         * @return {OpenSeadragon.GestureSettings}
+         * @returns {OpenSeadragon.GestureSettings}
          */
         gestureSettingsByDeviceType: function(type) {
             switch (type) {
                 case 'mouse':
                     return this.gestureSettingsMouse;
                 case 'touch':
                     return this.gestureSettingsTouch;
@@ -9925,14 +10169,18 @@
         goToNextPage: function() {
             var next = this._sequenceIndex + 1;
             if (this.navPrevNextWrap && next >= this.tileSources.length) {
                 next = 0;
             }
             this.goToPage(next);
         },
+
+        isAnimating: function() {
+            return THIS[this.hash].animating;
+        },
     });
 
 
     /**
      * _getSafeElemSize is like getElementSize(), but refuses to return 0 for x or y,
      * which was causing some calling operations to return NaN.
      * @returns {Point}
@@ -9994,14 +10242,15 @@
                 tileSource = new $.TileSource({
                     url: tileSource,
                     crossOriginPolicy: imgOptions.crossOriginPolicy !== undefined ?
                         imgOptions.crossOriginPolicy : viewer.crossOriginPolicy,
                     ajaxWithCredentials: viewer.ajaxWithCredentials,
                     ajaxHeaders: imgOptions.ajaxHeaders ?
                         imgOptions.ajaxHeaders : viewer.ajaxHeaders,
+                    splitHashDataForPost: viewer.splitHashDataForPost,
                     useCanvas: viewer.useCanvas,
                     success: function(event) {
                         successCallback(event.tileSource);
                     }
                 });
                 tileSource.addHandler('open-failed', function(event) {
                     failCallback(event);
@@ -10234,16 +10483,16 @@
         event.preventDefault = eventArgs.preventDefault;
     }
 
     function onCanvasKeyDown(event) {
         var canvasKeyDownEventArgs = {
             originalEvent: event.originalEvent,
             preventDefaultAction: false,
-            preventVerticalPan: event.preventVerticalPan,
-            preventHorizontalPan: event.preventHorizontalPan
+            preventVerticalPan: event.preventVerticalPan || !this.panVertical,
+            preventHorizontalPan: event.preventHorizontalPan || !this.panHorizontal
         };
 
         /**
          * Raised when a keyboard key is pressed and the focus is on the {@link OpenSeadragon.Viewer#canvas} element.
          *
          * @event canvas-key
          * @memberof OpenSeadragon.Viewer
@@ -10256,26 +10505,26 @@
          * @property {?Object} userData - Arbitrary subscriber-defined object.
          */
 
         this.raiseEvent('canvas-key', canvasKeyDownEventArgs);
 
         if (!canvasKeyDownEventArgs.preventDefaultAction && !event.ctrl && !event.alt && !event.meta) {
             switch (event.keyCode) {
-                case 38: //up arrow
+                case 38: //up arrow/shift uparrow
                     if (!canvasKeyDownEventArgs.preventVerticalPan) {
                         if (event.shift) {
                             this.viewport.zoomBy(1.1);
                         } else {
                             this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(0, -this.pixelsPerArrowPress)));
                         }
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                case 40: //down arrow
+                case 40: //down arrow/shift downarrow
                     if (!canvasKeyDownEventArgs.preventVerticalPan) {
                         if (event.shift) {
                             this.viewport.zoomBy(0.9);
                         } else {
                             this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(0, this.pixelsPerArrowPress)));
                         }
                         this.viewport.applyConstraints();
@@ -10292,129 +10541,121 @@
                 case 39: //right arrow
                     if (!canvasKeyDownEventArgs.preventHorizontalPan) {
                         this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(this.pixelsPerArrowPress, 0)));
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                default:
-                    //console.log( 'navigator keycode %s', event.keyCode );
-                    event.preventDefault = false;
-                    break;
-            }
-        } else {
-            event.preventDefault = false;
-        }
-    }
-
-    function onCanvasKeyPress(event) {
-        var canvasKeyPressEventArgs = {
-            originalEvent: event.originalEvent,
-            preventDefaultAction: false,
-            preventVerticalPan: event.preventVerticalPan,
-            preventHorizontalPan: event.preventHorizontalPan
-        };
-
-        // This event is documented in onCanvasKeyDown
-        this.raiseEvent('canvas-key', canvasKeyPressEventArgs);
-
-        if (!canvasKeyPressEventArgs.preventDefaultAction && !event.ctrl && !event.alt && !event.meta) {
-            switch (event.keyCode) {
-                case 43: //=|+
-                case 61: //=|+
+                case 187: //=|+
                     this.viewport.zoomBy(1.1);
                     this.viewport.applyConstraints();
                     event.preventDefault = true;
                     break;
-                case 45: //-|_
+                case 189: //-|_
                     this.viewport.zoomBy(0.9);
                     this.viewport.applyConstraints();
                     event.preventDefault = true;
                     break;
                 case 48: //0|)
                     this.viewport.goHome();
                     this.viewport.applyConstraints();
                     event.preventDefault = true;
                     break;
-                case 119: //w
-                case 87: //W
-                    if (!canvasKeyPressEventArgs.preventVerticalPan) {
+                case 87: //W/w
+                    if (!canvasKeyDownEventArgs.preventVerticalPan) {
                         if (event.shift) {
                             this.viewport.zoomBy(1.1);
                         } else {
                             this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(0, -40)));
                         }
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                case 115: //s
-                case 83: //S
-                    if (!canvasKeyPressEventArgs.preventVerticalPan) {
+                case 83: //S/s
+                    if (!canvasKeyDownEventArgs.preventVerticalPan) {
                         if (event.shift) {
                             this.viewport.zoomBy(0.9);
                         } else {
                             this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(0, 40)));
                         }
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                case 97: //a
-                    if (!canvasKeyPressEventArgs.preventHorizontalPan) {
+                case 65: //a/A
+                    if (!canvasKeyDownEventArgs.preventHorizontalPan) {
                         this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(-40, 0)));
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                case 100: //d
-                    if (!canvasKeyPressEventArgs.preventHorizontalPan) {
+                case 68: //d/D
+                    if (!canvasKeyDownEventArgs.preventHorizontalPan) {
                         this.viewport.panBy(this.viewport.deltaPointsFromPixels(new $.Point(40, 0)));
                         this.viewport.applyConstraints();
                     }
                     event.preventDefault = true;
                     break;
-                case 114: //r - clockwise rotation
-                    if (this.viewport.flipped) {
-                        this.viewport.setRotation($.positiveModulo(this.viewport.degrees - this.rotationIncrement, 360));
-                    } else {
-                        this.viewport.setRotation($.positiveModulo(this.viewport.degrees + this.rotationIncrement, 360));
-                    }
-                    this.viewport.applyConstraints();
-                    event.preventDefault = true;
-                    break;
-                case 82: //R - counterclockwise  rotation
-                    if (this.viewport.flipped) {
-                        this.viewport.setRotation($.positiveModulo(this.viewport.degrees + this.rotationIncrement, 360));
+                case 82: //r - clockwise rotation/R - counterclockwise rotation
+                    if (event.shift) {
+                        if (this.viewport.flipped) {
+                            this.viewport.setRotation(this.viewport.getRotation() + this.rotationIncrement);
+                        } else {
+                            this.viewport.setRotation(this.viewport.getRotation() - this.rotationIncrement);
+                        }
                     } else {
-                        this.viewport.setRotation($.positiveModulo(this.viewport.degrees - this.rotationIncrement, 360));
+                        if (this.viewport.flipped) {
+                            this.viewport.setRotation(this.viewport.getRotation() - this.rotationIncrement);
+                        } else {
+                            this.viewport.setRotation(this.viewport.getRotation() + this.rotationIncrement);
+                        }
                     }
                     this.viewport.applyConstraints();
                     event.preventDefault = true;
                     break;
-                case 102: //f
+                case 70: //f/F
                     this.viewport.toggleFlip();
                     event.preventDefault = true;
                     break;
-                case 106: //j - previous image source
+                case 74: //j - previous image source
                     this.goToPreviousPage();
                     break;
-                case 107: //k - next image source
+                case 75: //k - next image source
                     this.goToNextPage();
                     break;
                 default:
-                    // console.log( 'navigator keycode %s', event.keyCode );
+                    //console.log( 'navigator keycode %s', event.keyCode );
                     event.preventDefault = false;
                     break;
             }
         } else {
             event.preventDefault = false;
         }
     }
 
+    function onCanvasKeyPress(event) {
+        var canvasKeyPressEventArgs = {
+            originalEvent: event.originalEvent,
+        };
+
+        /**
+         * Raised when a keyboard key is pressed and the focus is on the {@link OpenSeadragon.Viewer#canvas} element.
+         *
+         * @event canvas-key-press
+         * @memberof OpenSeadragon.Viewer
+         * @type {object}
+         * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
+         * @property {Object} originalEvent - The original DOM event.
+         * @property {?Object} userData - Arbitrary subscriber-defined object.
+         */
+
+        this.raiseEvent('canvas-key-press', canvasKeyPressEventArgs);
+    }
+
     function onCanvasClick(event) {
         var gestureSettings;
 
         var haveKeyboardFocus = document.activeElement === this.canvas;
 
         // If we don't have keyboard focus, request it.
         if (!haveKeyboardFocus) {
@@ -10446,25 +10687,38 @@
          * @property {Boolean} quick - True only if the clickDistThreshold and clickTimeThreshold are both passed. Useful for differentiating between clicks and drags.
          * @property {Boolean} shift - True if the shift key was pressed during this event.
          * @property {Object} originalEvent - The original DOM event.
          * @property {Element} originalTarget - The DOM element clicked on.
          * @property {Boolean} preventDefaultAction - Set to true to prevent default click to zoom behaviour. Default: false.
          * @property {?Object} userData - Arbitrary subscriber-defined object.
          */
+
         this.raiseEvent('canvas-click', canvasClickEventArgs);
 
+
         if (!canvasClickEventArgs.preventDefaultAction && this.viewport && event.quick) {
             gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
-            if (gestureSettings.clickToZoom) {
+
+            if (gestureSettings.clickToZoom === true) {
                 this.viewport.zoomBy(
                     event.shift ? 1.0 / this.zoomPerClick : this.zoomPerClick,
                     gestureSettings.zoomToRefPoint ? this.viewport.pointFromPixel(event.position, true) : null
                 );
                 this.viewport.applyConstraints();
             }
+
+            if (gestureSettings.dblClickDragToZoom) {
+                if (THIS[this.hash].draggingToZoom === true) {
+                    THIS[this.hash].lastClickTime = null;
+                    THIS[this.hash].draggingToZoom = false;
+                } else {
+                    THIS[this.hash].lastClickTime = $.now();
+                }
+            }
+
         }
     }
 
     function onCanvasDblClick(event) {
         var gestureSettings;
 
         var canvasDblClickEventArgs = {
@@ -10536,51 +10790,58 @@
          * @property {Boolean} preventDefaultAction - Set to true to prevent default drag to pan behaviour. Default: false.
          * @property {?Object} userData - Arbitrary subscriber-defined object.
          */
         this.raiseEvent('canvas-drag', canvasDragEventArgs);
 
         gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
 
-        if (gestureSettings.dragToPan && !canvasDragEventArgs.preventDefaultAction && this.viewport) {
-            if (!this.panHorizontal) {
-                event.delta.x = 0;
-            }
-            if (!this.panVertical) {
-                event.delta.y = 0;
-            }
-            if (this.viewport.flipped) {
-                event.delta.x = -event.delta.x;
-            }
+        if (!canvasDragEventArgs.preventDefaultAction && this.viewport) {
 
-            if (this.constrainDuringPan) {
-                var delta = this.viewport.deltaPointsFromPixels(event.delta.negate());
+            if (gestureSettings.dblClickDragToZoom && THIS[this.hash].draggingToZoom) {
+                var factor = Math.pow(this.zoomPerDblClickDrag, event.delta.y / 50);
+                this.viewport.zoomBy(factor);
+            } else if (gestureSettings.dragToPan && !THIS[this.hash].draggingToZoom) {
+                if (!this.panHorizontal) {
+                    event.delta.x = 0;
+                }
+                if (!this.panVertical) {
+                    event.delta.y = 0;
+                }
+                if (this.viewport.flipped) {
+                    event.delta.x = -event.delta.x;
+                }
 
-                this.viewport.centerSpringX.target.value += delta.x;
-                this.viewport.centerSpringY.target.value += delta.y;
+                if (this.constrainDuringPan) {
+                    var delta = this.viewport.deltaPointsFromPixels(event.delta.negate());
 
-                var bounds = this.viewport.getBounds();
-                var constrainedBounds = this.viewport.getConstrainedBounds();
+                    this.viewport.centerSpringX.target.value += delta.x;
+                    this.viewport.centerSpringY.target.value += delta.y;
 
-                this.viewport.centerSpringX.target.value -= delta.x;
-                this.viewport.centerSpringY.target.value -= delta.y;
+                    var constrainedBounds = this.viewport.getConstrainedBounds();
 
-                if (bounds.x !== constrainedBounds.x) {
-                    event.delta.x = 0;
-                }
+                    this.viewport.centerSpringX.target.value -= delta.x;
+                    this.viewport.centerSpringY.target.value -= delta.y;
 
-                if (bounds.y !== constrainedBounds.y) {
-                    event.delta.y = 0;
+                    if (constrainedBounds.xConstrained) {
+                        event.delta.x = 0;
+                    }
+
+                    if (constrainedBounds.yConstrained) {
+                        event.delta.y = 0;
+                    }
                 }
+                this.viewport.panBy(this.viewport.deltaPointsFromPixels(event.delta.negate()), gestureSettings.flickEnabled && !this.constrainDuringPan);
             }
 
-            this.viewport.panBy(this.viewport.deltaPointsFromPixels(event.delta.negate()), gestureSettings.flickEnabled && !this.constrainDuringPan);
         }
+
     }
 
     function onCanvasDragEnd(event) {
+        var gestureSettings;
         var canvasDragEndEventArgs = {
             tracker: event.eventSource,
             pointerType: event.pointerType,
             position: event.position,
             speed: event.speed,
             direction: event.direction,
             shift: event.shift,
@@ -10603,17 +10864,19 @@
          * @property {Boolean} shift - True if the shift key was pressed during this event.
          * @property {Object} originalEvent - The original DOM event.
          * @property {Boolean} preventDefaultAction - Set to true to prevent default drag-end flick behaviour. Default: false.
          * @property {?Object} userData - Arbitrary subscriber-defined object.
          */
         this.raiseEvent('canvas-drag-end', canvasDragEndEventArgs);
 
+        gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
+
         if (!canvasDragEndEventArgs.preventDefaultAction && this.viewport) {
-            var gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
-            if (gestureSettings.flickEnabled &&
+            if (!THIS[this.hash].draggingToZoom &&
+                gestureSettings.flickEnabled &&
                 event.speed >= gestureSettings.flickMinSpeed) {
                 var amplitudeX = 0;
                 if (this.panHorizontal) {
                     amplitudeX = gestureSettings.flickMomentum * event.speed *
                         Math.cos(event.direction);
                 }
                 var amplitudeY = 0;
@@ -10625,14 +10888,21 @@
                     this.viewport.getCenter(true));
                 var target = this.viewport.pointFromPixel(
                     new $.Point(center.x - amplitudeX, center.y - amplitudeY));
                 this.viewport.panTo(target, false);
             }
             this.viewport.applyConstraints();
         }
+
+
+        if (gestureSettings.dblClickDragToZoom && THIS[this.hash].draggingToZoom === true) {
+            THIS[this.hash].draggingToZoom = false;
+        }
+
+
     }
 
     function onCanvasEnter(event) {
         /**
          * Raised when a pointer enters the {@link OpenSeadragon.Viewer#canvas} element.
          *
          * @event canvas-enter
@@ -10688,14 +10958,16 @@
             insideElementPressed: event.insideElementPressed,
             buttonDownAny: event.buttonDownAny,
             originalEvent: event.originalEvent
         });
     }
 
     function onCanvasPress(event) {
+        var gestureSettings;
+
         /**
          * Raised when the primary mouse button is pressed or touch starts on the {@link OpenSeadragon.Viewer#canvas} element.
          *
          * @event canvas-press
          * @memberof OpenSeadragon.Viewer
          * @type {object}
          * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
@@ -10711,14 +10983,32 @@
             tracker: event.eventSource,
             pointerType: event.pointerType,
             position: event.position,
             insideElementPressed: event.insideElementPressed,
             insideElementReleased: event.insideElementReleased,
             originalEvent: event.originalEvent
         });
+
+
+        gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
+        if (gestureSettings.dblClickDragToZoom) {
+            var lastClickTime = THIS[this.hash].lastClickTime;
+            var currClickTime = $.now();
+
+            if (lastClickTime === null) {
+                return;
+            }
+
+            if ((currClickTime - lastClickTime) < this.dblClickTimeThreshold) {
+                THIS[this.hash].draggingToZoom = true;
+            }
+
+            THIS[this.hash].lastClickTime = null;
+        }
+
     }
 
     function onCanvasRelease(event) {
         /**
          * Raised when the primary mouse button is released or touch ends on the {@link OpenSeadragon.Viewer#canvas} element.
          *
          * @event canvas-release
@@ -10844,41 +11134,79 @@
         this.raiseEvent('canvas-pinch', canvasPinchEventArgs);
 
         if (this.viewport) {
             gestureSettings = this.gestureSettingsByDeviceType(event.pointerType);
             if (gestureSettings.pinchToZoom &&
                 (!canvasPinchEventArgs.preventDefaultPanAction || !canvasPinchEventArgs.preventDefaultZoomAction)) {
                 centerPt = this.viewport.pointFromPixel(event.center, true);
-                if (!canvasPinchEventArgs.preventDefaultZoomAction) {
-                    this.viewport.zoomBy(event.distance / event.lastDistance, centerPt, true);
-                }
                 if (gestureSettings.zoomToRefPoint && !canvasPinchEventArgs.preventDefaultPanAction) {
                     lastCenterPt = this.viewport.pointFromPixel(event.lastCenter, true);
                     panByPt = lastCenterPt.minus(centerPt);
                     if (!this.panHorizontal) {
                         panByPt.x = 0;
                     }
                     if (!this.panVertical) {
                         panByPt.y = 0;
                     }
                     this.viewport.panBy(panByPt, true);
                 }
+                if (!canvasPinchEventArgs.preventDefaultZoomAction) {
+                    this.viewport.zoomBy(event.distance / event.lastDistance, centerPt, true);
+                }
                 this.viewport.applyConstraints();
             }
             if (gestureSettings.pinchRotate && !canvasPinchEventArgs.preventDefaultRotateAction) {
                 // Pinch rotate
                 var angle1 = Math.atan2(event.gesturePoints[0].currentPos.y - event.gesturePoints[1].currentPos.y,
                     event.gesturePoints[0].currentPos.x - event.gesturePoints[1].currentPos.x);
                 var angle2 = Math.atan2(event.gesturePoints[0].lastPos.y - event.gesturePoints[1].lastPos.y,
                     event.gesturePoints[0].lastPos.x - event.gesturePoints[1].lastPos.x);
-                this.viewport.setRotation(this.viewport.getRotation() + ((angle1 - angle2) * (180 / Math.PI)));
+                centerPt = this.viewport.pointFromPixel(event.center, true);
+                this.viewport.rotateTo(this.viewport.getRotation(true) + ((angle1 - angle2) * (180 / Math.PI)), centerPt, true);
             }
         }
     }
 
+    function onCanvasFocus(event) {
+
+        /**
+         * Raised when the {@link OpenSeadragon.Viewer#canvas} element gets keyboard focus.
+         *
+         * @event canvas-focus
+         * @memberof OpenSeadragon.Viewer
+         * @type {object}
+         * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
+         * @property {OpenSeadragon.MouseTracker} tracker - A reference to the MouseTracker which originated this event.
+         * @property {Object} originalEvent - The original DOM event.
+         * @property {?Object} userData - Arbitrary subscriber-defined object.
+         */
+        this.raiseEvent('canvas-focus', {
+            tracker: event.eventSource,
+            originalEvent: event.originalEvent
+        });
+    }
+
+    function onCanvasBlur(event) {
+        /**
+         * Raised when the {@link OpenSeadragon.Viewer#canvas} element loses keyboard focus.
+         *
+         * @event canvas-blur
+         * @memberof OpenSeadragon.Viewer
+         * @type {object}
+         * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
+         * @property {OpenSeadragon.MouseTracker} tracker - A reference to the MouseTracker which originated this event.
+         * @property {Object} originalEvent - The original DOM event.
+         * @property {?Object} userData - Arbitrary subscriber-defined object.
+         */
+        this.raiseEvent('canvas-blur', {
+            tracker: event.eventSource,
+            originalEvent: event.originalEvent
+        });
+    }
+
     function onCanvasScroll(event) {
         var canvasScrollEventArgs,
             gestureSettings,
             factor,
             thisScrollTime,
             deltaScrollTime;
 
@@ -11020,45 +11348,60 @@
         if (viewer.isOpen()) {
             viewer._updateRequestId = scheduleUpdate(viewer, updateMulti);
         } else {
             viewer._updateRequestId = false;
         }
     }
 
+    function doViewerResize(viewer, containerSize) {
+        var viewport = viewer.viewport;
+        var zoom = viewport.getZoom();
+        var center = viewport.getCenter();
+        viewport.resize(containerSize, viewer.preserveImageSizeOnResize);
+        viewport.panTo(center, true);
+        var resizeRatio;
+        if (viewer.preserveImageSizeOnResize) {
+            resizeRatio = THIS[viewer.hash].prevContainerSize.x / containerSize.x;
+        } else {
+            var origin = new $.Point(0, 0);
+            var prevDiag = new $.Point(THIS[viewer.hash].prevContainerSize.x, THIS[viewer.hash].prevContainerSize.y).distanceTo(origin);
+            var newDiag = new $.Point(containerSize.x, containerSize.y).distanceTo(origin);
+            resizeRatio = newDiag / prevDiag * THIS[viewer.hash].prevContainerSize.x / containerSize.x;
+        }
+        viewport.zoomTo(zoom * resizeRatio, null, true);
+        THIS[viewer.hash].prevContainerSize = containerSize;
+        THIS[viewer.hash].forceRedraw = true;
+        THIS[viewer.hash].needsResize = false;
+        THIS[viewer.hash].forceResize = false;
+    }
+
     function updateOnce(viewer) {
 
         //viewer.profiler.beginUpdate();
 
         if (viewer._opening || !THIS[viewer.hash]) {
             return;
         }
-
-        if (viewer.autoResize) {
-            var containerSize = _getSafeElemSize(viewer.container);
-            var prevContainerSize = THIS[viewer.hash].prevContainerSize;
-            if (!containerSize.equals(prevContainerSize)) {
-                var viewport = viewer.viewport;
-                if (viewer.preserveImageSizeOnResize) {
-                    var resizeRatio = prevContainerSize.x / containerSize.x;
-                    var zoom = viewport.getZoom() * resizeRatio;
-                    var center = viewport.getCenter();
-                    viewport.resize(containerSize, false);
-                    viewport.zoomTo(zoom, null, true);
-                    viewport.panTo(center, true);
-                } else {
-                    // maintain image position
-                    var oldBounds = viewport.getBounds();
-                    viewport.resize(containerSize, true);
-                    viewport.fitBoundsWithConstraints(oldBounds, true);
+        if (viewer.autoResize || THIS[viewer.hash].forceResize) {
+            var containerSize;
+            if (viewer._autoResizePolling) {
+                containerSize = _getSafeElemSize(viewer.container);
+                var prevContainerSize = THIS[viewer.hash].prevContainerSize;
+                if (!containerSize.equals(prevContainerSize)) {
+                    THIS[viewer.hash].needsResize = true;
                 }
-                THIS[viewer.hash].prevContainerSize = containerSize;
-                THIS[viewer.hash].forceRedraw = true;
             }
+            if (THIS[viewer.hash].needsResize) {
+                doViewerResize(viewer, containerSize || _getSafeElemSize(viewer.container));
+            }
+
         }
 
+
+
         var viewportChange = viewer.viewport.update();
         var animated = viewer.world.update() || viewportChange;
 
         if (viewportChange) {
             /**
              * Raised when any spring animation update occurs (zoom, pan, etc.),
              * before the viewer has drawn the new location.
@@ -11072,29 +11415,37 @@
             viewer.raiseEvent('viewport-change');
         }
 
         if (viewer.referenceStrip) {
             animated = viewer.referenceStrip.update(viewer.viewport) || animated;
         }
 
-        if (!THIS[viewer.hash].animating && animated) {
+        var currentAnimating = THIS[viewer.hash].animating;
+
+        if (!currentAnimating && animated) {
             /**
              * Raised when any spring animation starts (zoom, pan, etc.).
              *
              * @event animation-start
              * @memberof OpenSeadragon.Viewer
              * @type {object}
              * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
              * @property {?Object} userData - Arbitrary subscriber-defined object.
              */
             viewer.raiseEvent("animation-start");
             abortControlsAutoHide(viewer);
         }
 
-        if (animated || THIS[viewer.hash].forceRedraw || viewer.world.needsDraw()) {
+        var isAnimationFinished = currentAnimating && !animated;
+
+        if (isAnimationFinished) {
+            THIS[viewer.hash].animating = false;
+        }
+
+        if (animated || isAnimationFinished || THIS[viewer.hash].forceRedraw || viewer.world.needsDraw()) {
             drawWorld(viewer);
             viewer._drawOverlays();
             if (viewer.navigator) {
                 viewer.navigator.update(viewer.viewport);
             }
 
             THIS[viewer.hash].forceRedraw = false;
@@ -11110,15 +11461,15 @@
                  * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
                  * @property {?Object} userData - Arbitrary subscriber-defined object.
                  */
                 viewer.raiseEvent("animation");
             }
         }
 
-        if (THIS[viewer.hash].animating && !animated) {
+        if (isAnimationFinished) {
             /**
              * Raised when any spring animation ends (zoom, pan, etc.).
              *
              * @event animation-finish
              * @memberof OpenSeadragon.Viewer
              * @type {object}
              * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
@@ -11261,30 +11612,30 @@
     }
 
     function onRotateLeft() {
         if (this.viewport) {
             var currRotation = this.viewport.getRotation();
 
             if (this.viewport.flipped) {
-                currRotation = $.positiveModulo(currRotation + this.rotationIncrement, 360);
+                currRotation += this.rotationIncrement;
             } else {
-                currRotation = $.positiveModulo(currRotation - this.rotationIncrement, 360);
+                currRotation -= this.rotationIncrement;
             }
             this.viewport.setRotation(currRotation);
         }
     }
 
     function onRotateRight() {
         if (this.viewport) {
             var currRotation = this.viewport.getRotation();
 
             if (this.viewport.flipped) {
-                currRotation = $.positiveModulo(currRotation - this.rotationIncrement, 360);
+                currRotation -= this.rotationIncrement;
             } else {
-                currRotation = $.positiveModulo(currRotation + this.rotationIncrement, 360);
+                currRotation += this.rotationIncrement;
             }
             this.viewport.setRotation(currRotation);
         }
     }
     /**
      * Note: When pressed flip control button
      */
@@ -11294,15 +11645,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Navigator
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -11337,26 +11688,51 @@
      * of reference in the larger viewport as to which portion of the image
      * is currently being examined.  The navigator's viewport can be interacted
      * with using the keyboard or the mouse.
      *
      * @memberof OpenSeadragon
      * @extends OpenSeadragon.Viewer
      * @extends OpenSeadragon.EventSource
-     * @param {Object} options
+     * @param {Object} options - Navigator options
+     * @param {Element} [options.element] - An element to use for the navigator.
+     * @param {String} [options.id] - Id of the element to use for the navigator. However, this is ignored if {@link options.element} is provided.
      */
     $.Navigator = function(options) {
 
         var viewer = options.viewer,
             _this = this,
             viewerSize,
             navigatorSize;
 
         //We may need to create a new element and id if they did not
-        //provide the id for the existing element
-        if (!options.id) {
+        //provide the id for the existing element or the element itself
+        if (options.element || options.id) {
+            if (options.element) {
+                if (options.id) {
+                    $.console.warn("Given option.id for Navigator was ignored since option.element was provided and is being used instead.");
+                }
+
+                // Don't overwrite the element's id if it has one already
+                if (options.element.id) {
+                    options.id = options.element.id;
+                } else {
+                    options.id = 'navigator-' + $.now();
+                }
+
+                this.element = options.element;
+            } else {
+                this.element = document.getElementById(options.id);
+            }
+
+            options.controlOptions = {
+                anchor: $.ControlAnchor.NONE,
+                attachToViewer: false,
+                autoFade: false
+            };
+        } else {
             options.id = 'navigator-' + $.now();
             this.element = $.makeNeutralElement("div");
             options.controlOptions = {
                 anchor: $.ControlAnchor.TOP_RIGHT,
                 attachToViewer: true,
                 autoFade: options.autoFade
             };
@@ -11374,22 +11750,14 @@
                     options.controlOptions.anchor = $.ControlAnchor.ABSOLUTE;
                     options.controlOptions.top = options.top;
                     options.controlOptions.left = options.left;
                     options.controlOptions.height = options.height;
                     options.controlOptions.width = options.width;
                 }
             }
-
-        } else {
-            this.element = document.getElementById(options.id);
-            options.controlOptions = {
-                anchor: $.ControlAnchor.NONE,
-                attachToViewer: false,
-                autoFade: false
-            };
         }
         this.element.id = options.id;
         this.element.className += ' navigator';
 
         options = $.extend(true, {
             sizeRatio: $.DEFAULT_SETTINGS.navigatorSizeRatio
         }, options, {
@@ -11399,16 +11767,17 @@
             //the navigator is a viewer and a viewer has a navigator
             showNavigator: false,
             mouseNavEnabled: false,
             showNavigationControl: false,
             showSequenceControl: false,
             immediateRender: true,
             blendTime: 0,
-            animationTime: 0,
-            autoResize: options.autoResize,
+            animationTime: options.animationTime,
+            // disable autoResize since resize behavior is implemented differently by the navigator
+            autoResize: false,
             // prevent resizing the navigator from adding unwanted space around the image
             minZoomImageRatio: 1.0,
             background: options.background,
             opacity: options.opacity,
             borderColor: options.borderColor,
             displayRegionColor: options.displayRegionColor
         });
@@ -11458,14 +11827,15 @@
             /*jshint sub:true */
             style['float'] = 'left'; //Webkit
 
             style.cssFloat = 'left'; //Firefox
             style.styleFloat = 'left'; //IE
             style.zIndex = 999999999;
             style.cursor = 'default';
+            style.boxSizing = 'content-box';
         }(this.displayRegion.style, this.borderWidth));
         $.setElementPointerEventsNone(this.displayRegion);
         $.setElementTouchActionNone(this.displayRegion);
 
         this.displayRegionContainer = $.makeNeutralElement("div");
         this.displayRegionContainer.id = this.element.id + '-displayregioncontainer';
         this.displayRegionContainer.className = "displayregioncontainer";
@@ -11497,27 +11867,27 @@
         this.oldContainerSize = new $.Point(0, 0);
 
         $.Viewer.apply(this, [options]);
 
         this.displayRegionContainer.appendChild(this.displayRegion);
         this.element.getElementsByTagName('div')[0].appendChild(this.displayRegionContainer);
 
-        function rotate(degrees) {
+        function rotate(degrees, immediately) {
             _setTransformRotate(_this.displayRegionContainer, degrees);
             _setTransformRotate(_this.displayRegion, -degrees);
-            _this.viewport.setRotation(degrees);
+            _this.viewport.setRotation(degrees, immediately);
         }
         if (options.navigatorRotate) {
             var degrees = options.viewer.viewport ?
                 options.viewer.viewport.getRotation() :
                 options.viewer.degrees || 0;
 
-            rotate(degrees);
+            rotate(degrees, true);
             options.viewer.addHandler("rotate", function(args) {
-                rotate(args.degrees);
+                rotate(args.degrees, args.immediately);
             });
         }
 
 
         // Remove the base class' (Viewer's) innerTracker and replace it with our own
         this.innerTracker.destroy();
         this.innerTracker = new $.MouseTracker({
@@ -11597,24 +11967,26 @@
          * Explicitly sets the width of the navigator, in web coordinates. Disables automatic resizing.
          * @param {Number|String} width - the new width, either a number of pixels or a CSS string, such as "100%"
          */
         setWidth: function(width) {
             this.width = width;
             this.element.style.width = typeof(width) === "number" ? (width + 'px') : width;
             this._resizeWithViewer = false;
+            this.updateSize();
         },
 
         /**
          * Explicitly sets the height of the navigator, in web coordinates. Disables automatic resizing.
          * @param {Number|String} height - the new height, either a number of pixels or a CSS string, such as "100%"
          */
         setHeight: function(height) {
             this.height = height;
             this.element.style.height = typeof(height) === "number" ? (height + 'px') : height;
             this._resizeWithViewer = false;
+            this.updateSize();
         },
 
         /**
          * Flip navigator element
          * @param {Boolean} state - Flip state to set.
          */
         setFlip: function(state) {
@@ -11668,23 +12040,28 @@
 
             if (viewport && this.viewport) {
                 bounds = viewport.getBoundsNoRotate(true);
                 topleft = this.viewport.pixelFromPointNoRotate(bounds.getTopLeft(), false);
                 bottomright = this.viewport.pixelFromPointNoRotate(bounds.getBottomRight(), false)
                     .minus(this.totalBorderWidths);
 
+                if (!this.navigatorRotate) {
+                    var degrees = viewport.getRotation(true);
+                    _setTransformRotate(this.displayRegion, -degrees);
+                }
+
                 //update style for navigator-box
                 var style = this.displayRegion.style;
                 style.display = this.world.getItemCount() ? 'block' : 'none';
 
-                style.top = Math.round(topleft.y) + 'px';
-                style.left = Math.round(topleft.x) + 'px';
+                style.top = topleft.y.toFixed(2) + "px";
+                style.left = topleft.x.toFixed(2) + "px";
 
-                var width = Math.abs(topleft.x - bottomright.x);
-                var height = Math.abs(topleft.y - bottomright.y);
+                var width = bottomright.x - topleft.x;
+                var height = bottomright.y - topleft.y;
                 // make sure width and height are non-negative so IE doesn't throw
                 style.width = Math.round(Math.max(width, 0)) + 'px';
                 style.height = Math.round(Math.max(height, 0)) + 'px';
             }
 
         },
 
@@ -11941,15 +12318,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - getString/setString
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -12022,15 +12399,15 @@
             for (i = 0; i < props.length - 1; i++) {
                 // in case not a subproperty
                 container = container[props[i]] || {};
             }
             string = container[props[i]];
 
             if (typeof(string) !== "string") {
-                $.console.log("Untranslated source string:", prop);
+                $.console.error("Untranslated source string:", prop);
                 string = ""; // FIXME: this breaks gettext()-style convention, which would return source
             }
 
             return string.replace(/\{\d+\}/g, function(capture) {
                 var i = parseInt(capture.match(/\d+/), 10) + 1;
                 return i < args.length ?
                     args[i] :
@@ -12063,15 +12440,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Point
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -12309,15 +12686,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - TileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -12376,14 +12753,17 @@
      * @param {Function} [options.success]
      *      A function to be called upon successful creation.
      * @param {Boolean} [options.ajaxWithCredentials]
      *      If this TileSource needs to make an AJAX call, this specifies whether to set
      *      the XHR's withCredentials (for accessing secure data).
      * @param {Object} [options.ajaxHeaders]
      *      A set of headers to include in AJAX requests.
+     * @param {Boolean} [options.splitHashDataForPost]
+     *      First occurrence of '#' in the options.url is used to split URL
+     *      and the latter part is treated as POST data (applies to getImageInfo(...))
      * @param {Number} [options.width]
      *      Width of the source image at max resolution in pixels.
      * @param {Number} [options.height]
      *      Height of the source image at max resolution in pixels.
      * @param {Number} [options.tileSize]
      *      The size of the tiles to assumed to make up each pyramid layer in pixels.
      *      Tile size determines the point at which the image pyramid must be
@@ -12752,14 +13132,23 @@
                 filename = urlParts[urlParts.length - 1];
                 lastDot = filename.lastIndexOf('.');
                 if (lastDot > -1) {
                     urlParts[urlParts.length - 1] = filename.slice(0, lastDot);
                 }
             }
 
+            var postData = null;
+            if (this.splitHashDataForPost) {
+                var hashIdx = url.indexOf("#");
+                if (hashIdx !== -1) {
+                    postData = url.substring(hashIdx + 1);
+                    url = url.substr(0, hashIdx);
+                }
+            }
+
             callback = function(data) {
                 if (typeof(data) === "string") {
                     data = $.parseXml(data);
                 }
                 var $TileSource = $.TileSource.determineType(_this, data, url);
                 if (!$TileSource) {
                     /**
@@ -12776,15 +13165,15 @@
                     _this.raiseEvent('open-failed', {
                         message: "Unable to load TileSource",
                         source: url
                     });
                     return;
                 }
 
-                options = $TileSource.prototype.configure.apply(_this, [data, url]);
+                options = $TileSource.prototype.configure.apply(_this, [data, url, postData]);
                 if (options.ajaxWithCredentials === undefined) {
                     options.ajaxWithCredentials = _this.ajaxWithCredentials;
                 }
 
                 readySource = new $TileSource(options);
                 _this.ready = true;
                 /**
@@ -12813,14 +13202,15 @@
                     callbackName: callbackName,
                     callback: callback
                 });
             } else {
                 // request info via xhr asynchronously.
                 $.makeAjaxRequest({
                     url: url,
+                    postData: postData,
                     withCredentials: this.ajaxWithCredentials,
                     headers: this.ajaxHeaders,
                     success: function(xhr) {
                         var data = processResponse(xhr);
                         callback(data);
                     },
                     error: function(xhr, exc) {
@@ -12828,40 +13218,45 @@
 
                         /*
                             IE < 10 will block XHR requests to different origins. Any property access on the request
                             object will raise an exception which we'll attempt to handle by formatting the original
                             exception rather than the second one raised when we try to access xhr.status
                          */
                         try {
-                            msg = "HTTP " + xhr.status + " attempting to load TileSource";
+                            msg = "HTTP " + xhr.status + " attempting to load TileSource: " + url;
                         } catch (e) {
                             var formattedExc;
                             if (typeof(exc) === "undefined" || !exc.toString) {
                                 formattedExc = "Unknown error";
                             } else {
                                 formattedExc = exc.toString();
                             }
 
-                            msg = formattedExc + " attempting to load TileSource";
+                            msg = formattedExc + " attempting to load TileSource: " + url;
                         }
 
+                        $.console.error(msg);
+
                         /***
                          * Raised when an error occurs loading a TileSource.
                          *
                          * @event open-failed
                          * @memberof OpenSeadragon.TileSource
                          * @type {object}
                          * @property {OpenSeadragon.TileSource} eventSource - A reference to the TileSource which raised the event.
                          * @property {String} message
                          * @property {String} source
+                         * @property {String} postData - HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+                         *      see TileSource::getPostData) or null
                          * @property {?Object} userData - Arbitrary subscriber-defined object.
                          */
                         _this.raiseEvent('open-failed', {
                             message: msg,
-                            source: url
+                            source: url,
+                            postData: postData
                         });
                     }
                 });
             }
 
         },
 
@@ -12873,15 +13268,15 @@
          * understand that iteration order of TileSources is not guarunteed so
          * please make sure your data or url is expressive enough to ensure a simple
          * and sufficient mechanisim for clear determination.
          * @function
          * @param {String|Object|Array|Document} data
          * @param {String} url - the url the data was loaded
          *      from if any.
-         * @return {Boolean}
+         * @returns {Boolean}
          */
         supports: function(data, url) {
             return false;
         },
 
         /**
          * Responsible for parsing and configuring the
@@ -12890,70 +13285,324 @@
          * announcing you have to implement it.  Because of the variety of tile
          * server technologies, and various specifications for building image
          * pyramids, this method is here to allow easy integration.
          * @function
          * @param {String|Object|Array|Document} data
          * @param {String} url - the url the data was loaded
          *      from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
-         *      to configure this tile sources constructor.
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null value obtained from
+         *      the protocol URL after '#' sign if flag splitHashDataForPost set to 'true'
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
+         *      to configure the tile source constructor (include all values you want to
+         *      instantiate the TileSource subclass with - what _options_ object should contain).
          * @throws {Error}
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
             throw new Error("Method not implemented.");
         },
 
         /**
          * Responsible for retrieving the url which will return an image for the
          * region specified by the given x, y, and level components.
          * This method is not implemented by this class other than to throw an Error
          * announcing you have to implement it.  Because of the variety of tile
          * server technologies, and various specifications for building image
          * pyramids, this method is here to allow easy integration.
          * @function
          * @param {Number} level
          * @param {Number} x
          * @param {Number} y
+         * @returns {String|Function} url - A string for the url or a function that returns a url string.
          * @throws {Error}
          */
         getTileUrl: function(level, x, y) {
             throw new Error("Method not implemented.");
         },
 
         /**
+         * Must use AJAX in order to work, i.e. loadTilesWithAjax = true is set.
+         * If a value is returned, ajax issues POST request to the tile url.
+         * If null is returned, ajax issues GET request.
+         * The return value must comply to the header 'content type'.
+         *
+         * Examples (USED HEADER --> getTilePostData CODE):
+         * 'Content-type': 'application/x-www-form-urlencoded' -->
+         *   return "key1=value=1&key2=value2";
+         *
+         * 'Content-type': 'application/x-www-form-urlencoded' -->
+         *   return JSON.stringify({key: "value", number: 5});
+         *
+         * 'Content-type': 'multipart/form-data' -->
+         *   let result = new FormData();
+         *   result.append("data", myData);
+         *   return result;
+         *
+         * IMPORTANT: in case you move all the logic on image fetching
+         * to post data, you must re-define 'getTileHashKey(...)' to
+         * stay unique for different tile images.
+         *
+         * @param {Number} level
+         * @param {Number} x
+         * @param {Number} y
+         * @returns {*|null} post data to send with tile configuration request
+         */
+        getTilePostData: function(level, x, y) {
+            return null;
+        },
+
+        /**
          * Responsible for retrieving the headers which will be attached to the image request for the
          * region specified by the given x, y, and level components.
          * This option is only relevant if {@link OpenSeadragon.Options}.loadTilesWithAjax is set to true.
          * The headers returned here will override headers specified at the Viewer or TiledImage level.
          * Specifying a falsy value for a header will clear its existing value set at the Viewer or
          * TiledImage level (if any).
+         *
+         * Note that the headers of existing tiles don't automatically change when this function
+         * returns updated headers. To do that, you need to call {@link OpenSeadragon.Viewer#setAjaxHeaders}
+         * and propagate the changes.
+         *
          * @function
          * @param {Number} level
          * @param {Number} x
          * @param {Number} y
          * @returns {Object}
          */
         getTileAjaxHeaders: function(level, x, y) {
             return {};
         },
 
         /**
+         * The tile cache object is uniquely determined by this key and used to lookup
+         * the image data in cache: keys should be different if images are different.
+         *
+         * In case a tile has context2D property defined (TileSource.prototype.getContext2D)
+         * or its context2D is set manually; the cache is not used and this function
+         * is irrelevant.
+         * Note: default behaviour does not take into account post data.
+         * @param {Number} level tile level it was fetched with
+         * @param {Number} x x-coordinate in the pyramid level
+         * @param {Number} y y-coordinate in the pyramid level
+         * @param {String} url the tile was fetched with
+         * @param {Object} ajaxHeaders the tile was fetched with
+         * @param {*} postData data the tile was fetched with (type depends on getTilePostData(..) return type)
+         */
+        getTileHashKey: function(level, x, y, url, ajaxHeaders, postData) {
+            function withHeaders(hash) {
+                return ajaxHeaders ? hash + "+" + JSON.stringify(ajaxHeaders) : hash;
+            }
+
+            if (typeof url !== "string") {
+                return withHeaders(level + "/" + x + "_" + y);
+            }
+            return withHeaders(url);
+        },
+
+        /**
          * @function
          * @param {Number} level
          * @param {Number} x
          * @param {Number} y
          */
         tileExists: function(level, x, y) {
             var numTiles = this.getNumTiles(level);
             return level >= this.minLevel &&
                 level <= this.maxLevel &&
                 x >= 0 &&
                 y >= 0 &&
                 x < numTiles.x &&
                 y < numTiles.y;
+        },
+
+        /**
+         * Decide whether tiles have transparency: this is crucial for correct images blending.
+         * @returns {boolean} true if the image has transparency
+         */
+        hasTransparency: function(context2D, url, ajaxHeaders, post) {
+            return !!context2D || url.match('.png');
+        },
+
+        /**
+         * Download tile data.
+         * Note that if you override this function, you should override also downloadTileAbort().
+         * @param {ImageJob} context job context that you have to call finish(...) on.
+         * @param {String} [context.src] - URL of image to download.
+         * @param {String} [context.loadWithAjax] - Whether to load this image with AJAX.
+         * @param {String} [context.ajaxHeaders] - Headers to add to the image request if using AJAX.
+         * @param {Boolean} [context.ajaxWithCredentials] - Whether to set withCredentials on AJAX requests.
+         * @param {String} [context.crossOriginPolicy] - CORS policy to use for downloads
+         * @param {String} [context.postData] - HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+         *   see TileSource::getPostData) or null
+         * @param {*} [context.userData] - Empty object to attach your own data and helper variables to.
+         * @param {Function} [context.finish] - Should be called unless abort() was executed, e.g. on all occasions,
+         *   be it successful or unsuccessful request.
+         *   Usage: context.finish(data, request, errMessage). Pass the downloaded data object or null upon failure.
+         *   Add also reference to an ajax request if used. Provide error message in case of failure.
+         * @param {Function} [context.abort] - Called automatically when the job times out.
+         *   Usage: context.abort().
+         * @param {Function} [context.callback] @private - Called automatically once image has been downloaded
+         *   (triggered by finish).
+         * @param {Number} [context.timeout] @private - The max number of milliseconds that
+         *   this image job may take to complete.
+         * @param {string} [context.errorMsg] @private - The final error message, default null (set by finish).
+         */
+        downloadTileStart: function(context) {
+            var dataStore = context.userData,
+                image = new Image();
+
+            dataStore.image = image;
+            dataStore.request = null;
+
+            var finish = function(error) {
+                if (!image) {
+                    context.finish(null, dataStore.request, "Image load failed: undefined Image instance.");
+                    return;
+                }
+                image.onload = image.onerror = image.onabort = null;
+                context.finish(error ? null : image, dataStore.request, error);
+            };
+            image.onload = function() {
+                finish();
+            };
+            image.onabort = image.onerror = function() {
+                finish("Image load aborted.");
+            };
+
+            // Load the tile with an AJAX request if the loadWithAjax option is
+            // set. Otherwise load the image by setting the source proprety of the image object.
+            if (context.loadWithAjax) {
+                dataStore.request = $.makeAjaxRequest({
+                    url: context.src,
+                    withCredentials: context.ajaxWithCredentials,
+                    headers: context.ajaxHeaders,
+                    responseType: "arraybuffer",
+                    postData: context.postData,
+                    success: function(request) {
+                        var blb;
+                        // Make the raw data into a blob.
+                        // BlobBuilder fallback adapted from
+                        // http://stackoverflow.com/questions/15293694/blob-constructor-browser-compatibility
+                        try {
+                            blb = new window.Blob([request.response]);
+                        } catch (e) {
+                            var BlobBuilder = (
+                                window.BlobBuilder ||
+                                window.WebKitBlobBuilder ||
+                                window.MozBlobBuilder ||
+                                window.MSBlobBuilder
+                            );
+                            if (e.name === 'TypeError' && BlobBuilder) {
+                                var bb = new BlobBuilder();
+                                bb.append(request.response);
+                                blb = bb.getBlob();
+                            }
+                        }
+                        // If the blob is empty for some reason consider the image load a failure.
+                        if (blb.size === 0) {
+                            finish("Empty image response.");
+                        } else {
+                            // Create a URL for the blob data and make it the source of the image object.
+                            // This will still trigger Image.onload to indicate a successful tile load.
+                            image.src = (window.URL || window.webkitURL).createObjectURL(blb);
+                        }
+                    },
+                    error: function(request) {
+                        finish("Image load aborted - XHR error");
+                    }
+                });
+            } else {
+                if (context.crossOriginPolicy !== false) {
+                    image.crossOrigin = context.crossOriginPolicy;
+                }
+                image.src = context.src;
+            }
+        },
+
+        /**
+         * Provide means of aborting the execution.
+         * Note that if you override this function, you should override also downloadTileStart().
+         * @param {ImageJob} context job, the same object as with downloadTileStart(..)
+         * @param {*} [context.userData] - Empty object to attach (and mainly read) your own data.
+         */
+        downloadTileAbort: function(context) {
+            if (context.userData.request) {
+                context.userData.request.abort();
+            }
+            var image = context.userData.image;
+            if (context.userData.image) {
+                image.onload = image.onerror = image.onabort = null;
+            }
+        },
+
+        /**
+         * Create cache object from the result of the download process. The
+         * cacheObject parameter should be used to attach the data to, there are no
+         * conventions on how it should be stored - all the logic is implemented within *TileCache() functions.
+         *
+         * Note that if you override any of *TileCache() functions, you should override all of them.
+         * @param {object} cacheObject context cache object
+         * @param {*} data image data, the data sent to ImageJob.prototype.finish(), by default an Image object
+         * @param {Tile} tile instance the cache was created with
+         */
+        createTileCache: function(cacheObject, data, tile) {
+            cacheObject._data = data;
+        },
+
+        /**
+         * Cache object destructor, unset all properties you created to allow GC collection.
+         * Note that if you override any of *TileCache() functions, you should override all of them.
+         * @param {object} cacheObject context cache object
+         */
+        destroyTileCache: function(cacheObject) {
+            cacheObject._data = null;
+            cacheObject._renderedContext = null;
+        },
+
+        /**
+         * Raw data getter
+         * Note that if you override any of *TileCache() functions, you should override all of them.
+         * @param {object} cacheObject context cache object
+         * @returns {*} cache data
+         */
+        getTileCacheData: function(cacheObject) {
+            return cacheObject._data;
+        },
+
+        /**
+         * Compatibility image element getter
+         *  - plugins might need image representation of the data
+         *  - div HTML rendering relies on image element presence
+         * Note that if you override any of *TileCache() functions, you should override all of them.
+         *  @param {object} cacheObject context cache object
+         *  @returns {Image} cache data as an Image
+         */
+        getTileCacheDataAsImage: function(cacheObject) {
+            return cacheObject._data; //the data itself by default is Image
+        },
+
+        /**
+         * Compatibility context 2D getter
+         *  - most heavily used rendering method is a canvas-based approach,
+         *    convert the data to a canvas and return it's 2D context
+         * Note that if you override any of *TileCache() functions, you should override all of them.
+         * @param {object} cacheObject context cache object
+         * @returns {CanvasRenderingContext2D} context of the canvas representation of the cache data
+         */
+        getTileCacheDataAsContext2D: function(cacheObject) {
+            if (!cacheObject._renderedContext) {
+                var canvas = document.createElement('canvas');
+                canvas.width = cacheObject._data.width;
+                canvas.height = cacheObject._data.height;
+                cacheObject._renderedContext = canvas.getContext('2d');
+                cacheObject._renderedContext.drawImage(cacheObject._data, 0, 0);
+                //since we are caching the prerendered image on a canvas
+                //allow the image to not be held in memory
+                cacheObject._data = null;
+            }
+            return cacheObject._renderedContext;
         }
     };
 
 
     $.extend(true, $.TileSource.prototype, $.EventSource.prototype);
 
 
@@ -12977,15 +13626,15 @@
             status = xhr.status;
             statusText = (status === 404) ?
                 "Not Found" :
                 xhr.statusText;
             throw new Error($.getString("Errors.Status", status, statusText));
         }
 
-        if (responseText.match(/\s*<.*/)) {
+        if (responseText.match(/^\s*<.*/)) {
             try {
                 data = (xhr.responseXML && xhr.responseXML.documentElement) ?
                     xhr.responseXML :
                     $.parseXml(responseText);
             } catch (e) {
                 data = xhr.responseText;
             }
@@ -13032,15 +13681,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - DziTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -13154,18 +13803,19 @@
         },
 
         /**
          *
          * @function
          * @param {Object|XMLDocument} data - the raw configuration
          * @param {String} url - the url the data was retrieved from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
 
             var options;
 
             if (!$.isPlainObject(data)) {
 
                 options = configureFromXML(this, data);
 
@@ -13418,15 +14068,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - IIIFTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2023 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -13467,16 +14117,19 @@
      */
     $.IIIFTileSource = function(options) {
 
         /* eslint-disable camelcase */
 
         $.extend(true, this, options);
 
-        if (!(this.height && this.width && this['@id'])) {
-            throw new Error('IIIF required parameters not provided.');
+        /* Normalizes v3-style 'id' keys to an "_id" internal property */
+        this._id = this["@id"] || this["id"] || this['identifier'] || null;
+
+        if (!(this.height && this.width && this._id)) {
+            throw new Error('IIIF required parameters (width, height, or id) not provided.');
         }
 
         options.tileSizePerScaleFactor = {};
 
         this.tileFormat = this.tileFormat || 'jpg';
 
         this.version = options.version;
@@ -13547,31 +14200,46 @@
             this.levels = options.levels;
         } else {
             $.console.error("Nothing in the info.json to construct image pyramids from");
         }
 
         if (!options.maxLevel && !this.emulateLegacyImagePyramid) {
             if (!this.scale_factors) {
-                options.maxLevel = Number(Math.ceil(Math.log(Math.max(this.width, this.height), 2)));
+                options.maxLevel = Number(Math.round(Math.log(Math.max(this.width, this.height), 2)));
             } else {
                 var maxScaleFactor = Math.max.apply(null, this.scale_factors);
                 options.maxLevel = Math.round(Math.log(maxScaleFactor) * Math.LOG2E);
             }
         }
 
+        // Create an array with our exact resolution sizes if these have been supplied
+        if (this.sizes) {
+            var sizeLength = this.sizes.length;
+            if ((sizeLength === options.maxLevel) || (sizeLength === options.maxLevel + 1)) {
+                this.levelSizes = this.sizes;
+                // Need to take into account that the list may or may not include the full resolution size
+                if (sizeLength === options.maxLevel) {
+                    this.levelSizes.push({
+                        width: this.width,
+                        height: this.height
+                    });
+                }
+            }
+        }
+
         $.TileSource.apply(this, [options]);
     };
 
     $.extend($.IIIFTileSource.prototype, $.TileSource.prototype, /** @lends OpenSeadragon.IIIFTileSource.prototype */ {
         /**
          * Determine if the data and/or url imply the image service is supported by
          * this tile source.
          * @function
          * @param {Object|Array} data
-         * @param {String} optional - url
+         * @param {String} [url] - url
          */
 
         supports: function(data, url) {
             // Version 2.0 and forwards
             if (data.protocol && data.protocol === 'http://iiif.io/api/image') {
                 return true;
                 // Version 1.1
@@ -13596,43 +14264,51 @@
                 // Not IIIF
             } else {
                 return false;
             }
         },
 
         /**
+         * A static function used to prepare an incoming IIIF Image API info.json
+         * response for processing by the tile handler. Normalizes data for all
+         * versions of IIIF (1.0, 1.1, 2.x, 3.x) and returns a data object that
+         * may be passed to the IIIFTileSource.
          *
          * @function
+         * @static
          * @param {Object} data - the raw configuration
-         * @example <caption>IIIF 1.1 Info Looks like this</caption>
+         * @param {String} url - the url configuration was retrieved from
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} A normalized IIIF data object
+         * @example <caption>IIIF 2.x Info Looks like this</caption>
          * {
-         *   "@context" : "http://library.stanford.edu/iiif/image-api/1.1/context.json",
-         *   "@id" : "http://iiif.example.com/prefix/1E34750D-38DB-4825-A38A-B60A345E591C",
-         *   "width" : 6000,
-         *   "height" : 4000,
-         *   "scale_factors" : [ 1, 2, 4 ],
-         *   "tile_width" : 1024,
-         *   "tile_height" : 1024,
-         *   "formats" : [ "jpg", "png" ],
-         *   "qualities" : [ "native", "grey" ],
-         *   "profile" : "http://library.stanford.edu/iiif/image-api/1.1/compliance.html#level0"
+         * "@context": "http://iiif.io/api/image/2/context.json",
+         * "@id": "http://iiif.example.com/prefix/1E34750D-38DB-4825-A38A-B60A345E591C",
+         * "protocol": "http://iiif.io/api/image",
+         * "height": 1024,
+         * "width": 775,
+         * "tiles" : [{"width":256, "scaleFactors":[1,2,4,8]}],
+         *  "profile": ["http://iiif.io/api/image/2/level1.json", {
+         *    "qualities": [ "native", "bitonal", "grey", "color" ],
+         *    "formats": [ "jpg", "png", "gif" ]
+         *   }]
          * }
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
             // Try to deduce our version and fake it upwards if needed
             if (!$.isPlainObject(data)) {
                 var options = configureFromXml10(data);
                 options['@context'] = "http://iiif.io/api/image/1.0/context.json";
-                options['@id'] = url.replace('/info.xml', '');
+                options["@id"] = url.replace('/info.xml', '');
                 options.version = 1;
                 return options;
             } else {
                 if (!data['@context']) {
                     data['@context'] = 'http://iiif.io/api/image/1.0/context.json';
-                    data['@id'] = url.replace('/info.json', '');
+                    data["@id"] = url.replace('/info.json', '');
                     data.version = 1;
                 } else {
                     var context = data['@context'];
                     if (Array.isArray(context)) {
                         for (var i = 0; i < context.length; i++) {
                             if (typeof context[i] === 'string' &&
                                 (/^http:\/\/iiif\.io\/api\/image\/[1-3]\/context\.json$/.test(context[i]) ||
@@ -13653,17 +14329,15 @@
                         case 'http://iiif.io/api/image/3/context.json':
                             data.version = 3;
                             break;
                         default:
                             $.console.error('Data has a @context property which contains no known IIIF context URI.');
                     }
                 }
-                if (!data['@id'] && data['id']) {
-                    data['@id'] = data['id'];
-                }
+
                 if (data.preferredFormats) {
                     for (var f = 0; f < data.preferredFormats.length; f++) {
                         if (OpenSeadragon.imageFormatSupported(data.preferredFormats[f])) {
                             data.tileFormat = data.preferredFormats[f];
                             break;
                         }
                     }
@@ -13740,29 +14414,67 @@
                 if (scale) {
                     return new $.Point(1, 1);
                 } else {
                     return new $.Point(0, 0);
                 }
             }
 
-            return $.TileSource.prototype.getNumTiles.call(this, level);
+            // Use supplied list of scaled resolution sizes if these exist
+            if (this.levelSizes) {
+                var levelSize = this.levelSizes[level];
+                var x = Math.ceil(levelSize.width / this.getTileWidth(level)),
+                    y = Math.ceil(levelSize.height / this.getTileHeight(level));
+                return new $.Point(x, y);
+            }
+            // Otherwise call default TileSource->getNumTiles() function
+            else {
+                return $.TileSource.prototype.getNumTiles.call(this, level);
+            }
         },
 
 
         /**
          * @function
          * @param {Number} level
          * @param {OpenSeadragon.Point} point
          */
         getTileAtPoint: function(level, point) {
 
             if (this.emulateLegacyImagePyramid) {
                 return new $.Point(0, 0);
             }
 
+            // Use supplied list of scaled resolution sizes if these exist
+            if (this.levelSizes) {
+
+                var validPoint = point.x >= 0 && point.x <= 1 &&
+                    point.y >= 0 && point.y <= 1 / this.aspectRatio;
+                $.console.assert(validPoint, "[TileSource.getTileAtPoint] must be called with a valid point.");
+
+                var widthScaled = this.levelSizes[level].width;
+                var pixelX = point.x * widthScaled;
+                var pixelY = point.y * widthScaled;
+
+                var x = Math.floor(pixelX / this.getTileWidth(level));
+                var y = Math.floor(pixelY / this.getTileHeight(level));
+
+                // When point.x == 1 or point.y == 1 / this.aspectRatio we want to
+                // return the last tile of the row/column
+                if (point.x >= 1) {
+                    x = this.getNumTiles(level).x - 1;
+                }
+                var EPSILON = 1e-15;
+                if (point.y >= 1 / this.aspectRatio - EPSILON) {
+                    y = this.getNumTiles(level).y - 1;
+                }
+
+                return new $.Point(x, y);
+            }
+
+            // Otherwise call default TileSource->getTileAtPoint() function
             return $.TileSource.prototype.getTileAtPoint.call(this, level, point);
         },
 
 
         /**
          * Responsible for retrieving the url which will return an image for the
          * region specified by the given x, y, and level components.
@@ -13782,18 +14494,17 @@
                 return url;
             }
 
             //# constants
             var IIIF_ROTATION = '0',
                 //## get the scale (level as a decimal)
                 scale = Math.pow(0.5, this.maxLevel - level),
-
                 //# image dimensions at this level
-                levelWidth = Math.ceil(this.width * scale),
-                levelHeight = Math.ceil(this.height * scale),
+                levelWidth,
+                levelHeight,
 
                 //## iiif region
                 tileWidth,
                 tileHeight,
                 iiifTileSizeWidth,
                 iiifTileSizeHeight,
                 iiifRegion,
@@ -13803,18 +14514,29 @@
                 iiifTileH,
                 iiifSize,
                 iiifSizeW,
                 iiifSizeH,
                 iiifQuality,
                 uri;
 
+            // Use supplied list of scaled resolution sizes if these exist
+            if (this.levelSizes) {
+                levelWidth = this.levelSizes[level].width;
+                levelHeight = this.levelSizes[level].height;
+            }
+            // Otherwise calculate the sizes ourselves
+            else {
+                levelWidth = Math.ceil(this.width * scale);
+                levelHeight = Math.ceil(this.height * scale);
+            }
+
             tileWidth = this.getTileWidth(level);
             tileHeight = this.getTileHeight(level);
-            iiifTileSizeWidth = Math.ceil(tileWidth / scale);
-            iiifTileSizeHeight = Math.ceil(tileHeight / scale);
+            iiifTileSizeWidth = Math.round(tileWidth / scale);
+            iiifTileSizeHeight = Math.round(tileHeight / scale);
             if (this.version === 1) {
                 iiifQuality = "native." + this.tileFormat;
             } else {
                 iiifQuality = "default." + this.tileFormat;
             }
             if (levelWidth < tileWidth && levelHeight < tileHeight) {
                 if (this.version === 2 && levelWidth === this.width) {
@@ -13833,43 +14555,46 @@
                 iiifTileW = Math.min(iiifTileSizeWidth, this.width - iiifTileX);
                 iiifTileH = Math.min(iiifTileSizeHeight, this.height - iiifTileY);
                 if (x === 0 && y === 0 && iiifTileW === this.width && iiifTileH === this.height) {
                     iiifRegion = "full";
                 } else {
                     iiifRegion = [iiifTileX, iiifTileY, iiifTileW, iiifTileH].join(',');
                 }
-                iiifSizeW = Math.ceil(iiifTileW * scale);
-                iiifSizeH = Math.ceil(iiifTileH * scale);
+                iiifSizeW = Math.min(tileWidth, levelWidth - (x * tileWidth));
+                iiifSizeH = Math.min(tileHeight, levelHeight - (y * tileHeight));
                 if (this.version === 2 && iiifSizeW === this.width) {
                     iiifSize = "full";
                 } else if (this.version === 3 && iiifSizeW === this.width && iiifSizeH === this.height) {
                     iiifSize = "max";
                 } else if (this.version === 3) {
                     iiifSize = iiifSizeW + "," + iiifSizeH;
                 } else {
                     iiifSize = iiifSizeW + ",";
                 }
             }
-            uri = [this['@id'], iiifRegion, iiifSize, IIIF_ROTATION, iiifQuality].join('/');
+            uri = [this._id, iiifRegion, iiifSize, IIIF_ROTATION, iiifQuality].join('/');
 
             return uri;
         },
 
         __testonly__: {
             canBeTiled: canBeTiled,
             constructLevels: constructLevels
         }
 
     });
 
     /**
      * Determine whether arbitrary tile requests can be made against a service with the given profile
      * @function
-     * @param {array} profile - IIIF profile array
-     * @throws {Error}
+     * @param {Object} options
+     * @param {Array|String} options.profile
+     * @param {Number} options.version
+     * @param {String[]} options.extraFeatures
+     * @returns {Boolean}
      */
     function canBeTiled(options) {
         var level0Profiles = [
             "http://library.stanford.edu/iiif/image-api/compliance.html#level0",
             "http://library.stanford.edu/iiif/image-api/1.1/compliance.html#level0",
             "http://iiif.io/api/image/2/level0.json",
             "level0",
@@ -13893,15 +14618,15 @@
      * @param {object} options - infoJson
      * @throws {Error}
      */
     function constructLevels(options) {
         var levels = [];
         for (var i = 0; i < options.sizes.length; i++) {
             levels.push({
-                url: options['@id'] + '/full/' + options.sizes[i].width + ',' +
+                url: options._id + '/full/' + options.sizes[i].width + ',' +
                     (options.version === 3 ? options.sizes[i].height : '') +
                     '/0/default.' + options.tileFormat,
                 width: options.sizes[i].width,
                 height: options.sizes[i].height
             });
         }
         return levels.sort(function(a, b) {
@@ -13962,15 +14687,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - OsmTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -14082,18 +14807,19 @@
         },
 
         /**
          *
          * @function
          * @param {Object} data - the raw configuration
          * @param {String} url - the url the data was retrieved from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
             return data;
         },
 
 
         /**
          * @function
          * @param {Number} level
@@ -14108,15 +14834,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - TmsTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -14217,18 +14943,19 @@
         },
 
         /**
          *
          * @function
          * @param {Object} data - the raw configuration
          * @param {String} url - the url the data was retrieved from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
             return data;
         },
 
 
         /**
          * @function
          * @param {Number} level
@@ -14366,18 +15093,19 @@
         },
 
         /**
          *
          * @function
          * @param {Object} data - the raw configuration
          * @param {String} url - the url the data was retrieved from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(data, url) {
+        configure: function(data, url, postData) {
             return data;
         },
 
         /**
          * @function
          * @param {Number} level
          * @param {Number} x
@@ -14396,15 +15124,15 @@
 }(OpenSeadragon));
 
 
 /*
  * OpenSeadragon - LegacyTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -14515,18 +15243,19 @@
 
 
         /**
          *
          * @function
          * @param {Object|XMLDocument} configuration - the raw configuration
          * @param {String} dataUrl - the url the data was retrieved from if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(configuration, dataUrl) {
+        configure: function(configuration, dataUrl, postData) {
 
             var options;
 
             if (!$.isPlainObject(configuration)) {
 
                 options = configureFromXML(this, configuration);
 
@@ -14685,15 +15414,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - ImageTileSource
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -14772,18 +15501,19 @@
             return data.type && data.type === "image";
         },
         /**
          *
          * @function
          * @param {Object} options - the options
          * @param {String} dataUrl - the url the image was retrieved from, if any.
-         * @return {Object} options - A dictionary of keyword arguments sufficient
+         * @param {String} postData - HTTP POST data in k=v&k2=v2... form or null
+         * @returns {Object} options - A dictionary of keyword arguments sufficient
          *      to configure this tile sources constructor.
          */
-        configure: function(options, dataUrl) {
+        configure: function(options, dataUrl, postData) {
             return options;
         },
         /**
          * Responsible for retrieving, and caching the
          * image metadata pertinent to this TileSources implementation.
          * @function
          * @param {String} url
@@ -14956,27 +15686,29 @@
          * Free up canvas memory
          * (iOS 12 or higher on 2GB RAM device has only 224MB canvas memory,
          * and Safari keeps canvas until its height and width will be set to 0).
          * @function
          */
         _freeupCanvasMemory: function() {
             for (var i = 0; i < this.levels.length; i++) {
-                this.levels[i].context2D.canvas.height = 0;
-                this.levels[i].context2D.canvas.width = 0;
+                if (this.levels[i].context2D) {
+                    this.levels[i].context2D.canvas.height = 0;
+                    this.levels[i].context2D.canvas.width = 0;
+                }
             }
         },
     });
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - TileSourceCollection
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -15011,15 +15743,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Button
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -15425,22 +16157,24 @@
 
         /**
          * @function
          */
         disable: function() {
             this.notifyGroupExit();
             this.element.disabled = true;
+            this.tracker.setTracking(false);
             $.setElementOpacity(this.element, 0.2, true);
         },
 
         /**
          * @function
          */
         enable: function() {
             this.element.disabled = false;
+            this.tracker.setTracking(true);
             $.setElementOpacity(this.element, 1.0, true);
             this.notifyGroupEnter();
         },
 
         destroy: function() {
             if (this.imgRest) {
                 this.element.removeChild(this.imgRest);
@@ -15572,15 +16306,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - ButtonGroup
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -15683,14 +16417,25 @@
         });
     };
 
     /** @lends OpenSeadragon.ButtonGroup.prototype */
     $.ButtonGroup.prototype = {
 
         /**
+         * Adds the given button to this button group.
+         *
+         * @function
+         * @param {OpenSeadragon.Button} button
+         */
+        addButton: function(button) {
+            this.buttons.push(button);
+            this.element.appendChild(button.element);
+        },
+
+        /**
          * TODO: Figure out why this is used on the public API and if a more useful
          * api can be created.
          * @function
          * @private
          */
         emulateEnter: function() {
             this.tracker.enterHandler({
@@ -15724,15 +16469,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Rect
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -15952,25 +16697,25 @@
             ).rotate(this.degrees, this.getTopLeft());
         },
 
         /**
          * Returns the width and height component as a vector OpenSeadragon.Point
          * @function
          * @returns {OpenSeadragon.Point} The 2 dimensional vector representing the
-         *  the width and height of the rectangle.
+         *  width and height of the rectangle.
          */
         getSize: function() {
             return new $.Point(this.width, this.height);
         },
 
         /**
          * Determines if two Rectangles have equivalent components.
          * @function
          * @param {OpenSeadragon.Rect} rectangle The Rectangle to compare to.
-         * @return {Boolean} 'true' if all components are equal, otherwise 'false'.
+         * @returns {Boolean} 'true' if all components are equal, otherwise 'false'.
          */
         equals: function(other) {
             return (other instanceof $.Rect) &&
                 this.x === other.x &&
                 this.y === other.y &&
                 this.width === other.width &&
                 this.height === other.height &&
@@ -16009,15 +16754,15 @@
                 this.degrees);
         },
 
         /**
          * Returns the smallest rectangle that will contain this and the given
          * rectangle bounding boxes.
          * @param {OpenSeadragon.Rect} rect
-         * @return {OpenSeadragon.Rect} The new rectangle.
+         * @returns {OpenSeadragon.Rect} The new rectangle.
          */
         union: function(rect) {
             var thisBoundingBox = this.getBoundingBox();
             var otherBoundingBox = rect.getBoundingBox();
 
             var left = Math.min(thisBoundingBox.x, otherBoundingBox.x);
             var top = Math.min(thisBoundingBox.y, otherBoundingBox.y);
@@ -16035,15 +16780,15 @@
                 bottom - top);
         },
 
         /**
          * Returns the bounding box of the intersection of this rectangle with the
          * given rectangle.
          * @param {OpenSeadragon.Rect} rect
-         * @return {OpenSeadragon.Rect} the bounding box of the intersection
+         * @returns {OpenSeadragon.Rect} the bounding box of the intersection
          * or null if the rectangles don't intersect.
          */
         intersection: function(rect) {
             // Simplified version of Weiler Atherton clipping algorithm
             // https://en.wikipedia.org/wiki/Weiler%E2%80%93Atherton_clipping_algorithm
             // Because we just want the bounding box of the intersection,
             // we can just compute the bounding box of:
@@ -16165,15 +16910,15 @@
 
         /**
          * Rotates a rectangle around a point.
          * @function
          * @param {Number} degrees The angle in degrees to rotate.
          * @param {OpenSeadragon.Point} [pivot] The point about which to rotate.
          * Defaults to the center of the rectangle.
-         * @return {OpenSeadragon.Rect}
+         * @returns {OpenSeadragon.Rect}
          */
         rotate: function(degrees, pivot) {
             degrees = $.positiveModulo(degrees, 360);
             if (degrees === 0) {
                 return this.clone();
             }
 
@@ -16290,15 +17035,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - ReferenceStrip
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -16560,15 +17305,15 @@
         },
 
         /**
          * @function
          */
         update: function() {
             if (THIS[this.id].animating) {
-                $.console.log('image reference strip update');
+                // $.console.log( 'image reference strip update' );
                 return true;
             }
             return false;
         },
 
         destroy: function() {
             if (this.miniViewers) {
@@ -16593,15 +17338,16 @@
      * @function
      */
     function onStripClick(event) {
         if (event.quick) {
             var page;
 
             if ('horizontal' === this.scroll) {
-                page = Math.floor(event.position.x / this.panelWidth);
+                // +4px fix to solve problem with precision on thumbnail selection if there is a lot of them
+                page = Math.floor(event.position.x / (this.panelWidth + 4));
             } else {
                 page = Math.floor(event.position.y / this.panelHeight);
             }
 
             this.viewer.goToPage(page);
         }
 
@@ -16955,15 +17701,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - DisplayRect
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -17027,15 +17773,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Spring
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -17285,15 +18031,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - ImageLoader
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -17318,142 +18064,104 @@
  * NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 (function($) {
 
     /**
-     * @private
      * @class ImageJob
      * @classdesc Handles downloading of a single image.
      * @param {Object} options - Options for this ImageJob.
      * @param {String} [options.src] - URL of image to download.
+     * @param {Tile} [options.tile] - Tile that belongs the data to.
+     * @param {TileSource} [options.source] - Image loading strategy
      * @param {String} [options.loadWithAjax] - Whether to load this image with AJAX.
      * @param {String} [options.ajaxHeaders] - Headers to add to the image request if using AJAX.
+     * @param {Boolean} [options.ajaxWithCredentials] - Whether to set withCredentials on AJAX requests.
      * @param {String} [options.crossOriginPolicy] - CORS policy to use for downloads
+     * @param {String} [options.postData] - HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+     *      see TileSource::getPostData) or null
      * @param {Function} [options.callback] - Called once image has been downloaded.
      * @param {Function} [options.abort] - Called when this image job is aborted.
      * @param {Number} [options.timeout] - The max number of milliseconds that this image job may take to complete.
+     * @param {Number} [options.tries] - Actual number of the current try.
      */
-    function ImageJob(options) {
+    $.ImageJob = function(options) {
 
         $.extend(true, this, {
             timeout: $.DEFAULT_SETTINGS.timeout,
-            jobId: null
+            jobId: null,
+            tries: 0
         }, options);
 
         /**
-         * Image object which will contain downloaded image.
-         * @member {Image} image
+         * Data object which will contain downloaded image data.
+         * @member {Image|*} data data object, by default an Image object (depends on TileSource)
          * @memberof OpenSeadragon.ImageJob#
          */
-        this.image = null;
-    }
+        this.data = null;
+
+        /**
+         * User workspace to populate with helper variables
+         * @member {*} userData to append custom data and avoid namespace collision
+         * @memberof OpenSeadragon.ImageJob#
+         */
+        this.userData = {};
 
-    ImageJob.prototype = {
-        errorMsg: null,
+        /**
+         * Error message holder
+         * @member {string} error message
+         * @memberof OpenSeadragon.ImageJob#
+         * @private
+         */
+        this.errorMsg = null;
+    };
 
+    $.ImageJob.prototype = {
         /**
          * Starts the image job.
          * @method
          */
         start: function() {
+            this.tries++;
+
             var self = this;
             var selfAbort = this.abort;
 
-            this.image = new Image();
-
-            this.image.onload = function() {
-                self.finish(true);
-            };
-            this.image.onabort = this.image.onerror = function() {
-                self.errorMsg = "Image load aborted";
-                self.finish(false);
-            };
-
             this.jobId = window.setTimeout(function() {
-                self.errorMsg = "Image load exceeded timeout (" + self.timeout + " ms)";
-                self.finish(false);
+                self.finish(null, null, "Image load exceeded timeout (" + self.timeout + " ms)");
             }, this.timeout);
 
-            // Load the tile with an AJAX request if the loadWithAjax option is
-            // set. Otherwise load the image by setting the source proprety of the image object.
-            if (this.loadWithAjax) {
-                this.request = $.makeAjaxRequest({
-                    url: this.src,
-                    withCredentials: this.ajaxWithCredentials,
-                    headers: this.ajaxHeaders,
-                    responseType: "arraybuffer",
-                    success: function(request) {
-                        var blb;
-                        // Make the raw data into a blob.
-                        // BlobBuilder fallback adapted from
-                        // http://stackoverflow.com/questions/15293694/blob-constructor-browser-compatibility
-                        try {
-                            blb = new window.Blob([request.response]);
-                        } catch (e) {
-                            var BlobBuilder = (
-                                window.BlobBuilder ||
-                                window.WebKitBlobBuilder ||
-                                window.MozBlobBuilder ||
-                                window.MSBlobBuilder
-                            );
-                            if (e.name === 'TypeError' && BlobBuilder) {
-                                var bb = new BlobBuilder();
-                                bb.append(request.response);
-                                blb = bb.getBlob();
-                            }
-                        }
-                        // If the blob is empty for some reason consider the image load a failure.
-                        if (blb.size === 0) {
-                            self.errorMsg = "Empty image response.";
-                            self.finish(false);
-                        }
-                        // Create a URL for the blob data and make it the source of the image object.
-                        // This will still trigger Image.onload to indicate a successful tile load.
-                        var url = (window.URL || window.webkitURL).createObjectURL(blb);
-                        self.image.src = url;
-                    },
-                    error: function(request) {
-                        self.errorMsg = "Image load aborted - XHR error";
-                        self.finish(false);
-                    }
-                });
-
-                // Provide a function to properly abort the request.
-                this.abort = function() {
-                    self.request.abort();
-
-                    // Call the existing abort function if available
-                    if (typeof selfAbort === "function") {
-                        selfAbort();
-                    }
-                };
-            } else {
-                if (this.crossOriginPolicy !== false) {
-                    this.image.crossOrigin = this.crossOriginPolicy;
+            this.abort = function() {
+                self.source.downloadTileAbort(self);
+                if (typeof selfAbort === "function") {
+                    selfAbort();
                 }
+            };
 
-                this.image.src = this.src;
-            }
+            this.source.downloadTileStart(this);
         },
 
-        finish: function(successful) {
-            this.image.onload = this.image.onerror = this.image.onabort = null;
-            if (!successful) {
-                this.image = null;
-            }
+        /**
+         * Finish this job.
+         * @param {*} data data that has been downloaded
+         * @param {XMLHttpRequest} request reference to the request if used
+         * @param {string} errorMessage description upon failure
+         */
+        finish: function(data, request, errorMessage) {
+            this.data = data;
+            this.request = request;
+            this.errorMsg = errorMessage;
 
             if (this.jobId) {
                 window.clearTimeout(this.jobId);
             }
 
             this.callback(this);
         }
-
     };
 
     /**
      * @class ImageLoader
      * @memberof OpenSeadragon
      * @classdesc Handles downloading of a set of images using asynchronous queue pattern.
      * You generally won't have to interact with the ImageLoader directly.
@@ -17463,51 +18171,70 @@
      */
     $.ImageLoader = function(options) {
 
         $.extend(true, this, {
             jobLimit: $.DEFAULT_SETTINGS.imageLoaderLimit,
             timeout: $.DEFAULT_SETTINGS.timeout,
             jobQueue: [],
+            failedTiles: [],
             jobsInProgress: 0
         }, options);
 
     };
 
     /** @lends OpenSeadragon.ImageLoader.prototype */
     $.ImageLoader.prototype = {
 
         /**
          * Add an unloaded image to the loader queue.
          * @method
          * @param {Object} options - Options for this job.
          * @param {String} [options.src] - URL of image to download.
+         * @param {Tile} [options.tile] - Tile that belongs the data to. The tile instance
+         *      is not internally used and serves for custom TileSources implementations.
+         * @param {TileSource} [options.source] - Image loading strategy
          * @param {String} [options.loadWithAjax] - Whether to load this image with AJAX.
          * @param {String} [options.ajaxHeaders] - Headers to add to the image request if using AJAX.
          * @param {String|Boolean} [options.crossOriginPolicy] - CORS policy to use for downloads
+         * @param {String} [options.postData] - POST parameters (usually but not necessarily in k=v&k2=v2... form,
+         *      see TileSource::getPostData) or null
          * @param {Boolean} [options.ajaxWithCredentials] - Whether to set withCredentials on AJAX
-         * requests.
+         *      requests.
          * @param {Function} [options.callback] - Called once image has been downloaded.
          * @param {Function} [options.abort] - Called when this image job is aborted.
          */
         addJob: function(options) {
+            if (!options.source) {
+                $.console.error('ImageLoader.prototype.addJob() requires [options.source]. ' +
+                    'TileSource since new API defines how images are fetched. Creating a dummy TileSource.');
+                var implementation = $.TileSource.prototype;
+                options.source = {
+                    downloadTileStart: implementation.downloadTileStart,
+                    downloadTileAbort: implementation.downloadTileAbort
+                };
+            }
+
             var _this = this,
                 complete = function(job) {
                     completeJob(_this, job, options.callback);
                 },
                 jobOptions = {
                     src: options.src,
+                    tile: options.tile || {},
+                    source: options.source,
                     loadWithAjax: options.loadWithAjax,
                     ajaxHeaders: options.loadWithAjax ? options.ajaxHeaders : null,
                     crossOriginPolicy: options.crossOriginPolicy,
                     ajaxWithCredentials: options.ajaxWithCredentials,
+                    postData: options.postData,
                     callback: complete,
                     abort: options.abort,
                     timeout: this.timeout
                 },
-                newJob = new ImageJob(jobOptions);
+                newJob = new $.ImageJob(jobOptions);
 
             if (!this.jobLimit || this.jobsInProgress < this.jobLimit) {
                 newJob.start();
                 this.jobsInProgress++;
             } else {
                 this.jobQueue.push(newJob);
             }
@@ -17526,42 +18253,56 @@
             }
 
             this.jobQueue = [];
         }
     };
 
     /**
-     * Cleans up ImageJob once completed.
+     * Cleans up ImageJob once completed. Restarts job after tileRetryDelay seconds if failed
+     * but max tileRetryMax times
      * @method
      * @private
      * @param loader - ImageLoader used to start job.
      * @param job - The ImageJob that has completed.
      * @param callback - Called once cleanup is finished.
      */
     function completeJob(loader, job, callback) {
+        if (job.errorMsg !== '' && (job.data === null || job.data === undefined) && job.tries < 1 + loader.tileRetryMax) {
+            loader.failedTiles.push(job);
+        }
         var nextJob;
 
         loader.jobsInProgress--;
 
         if ((!loader.jobLimit || loader.jobsInProgress < loader.jobLimit) && loader.jobQueue.length > 0) {
             nextJob = loader.jobQueue.shift();
             nextJob.start();
             loader.jobsInProgress++;
         }
 
-        callback(job.image, job.errorMsg, job.request);
+        if (loader.tileRetryMax > 0 && loader.jobQueue.length === 0) {
+            if ((!loader.jobLimit || loader.jobsInProgress < loader.jobLimit) && loader.failedTiles.length > 0) {
+                nextJob = loader.failedTiles.shift();
+                setTimeout(function() {
+                    nextJob.start();
+                }, loader.tileRetryDelay);
+                loader.jobsInProgress++;
+            }
+        }
+
+        callback(job.data, job.errorMsg, job.request);
     }
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Tile
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -17595,24 +18336,27 @@
      * @param {Number} level The zoom level this tile belongs to.
      * @param {Number} x The vector component 'x'.
      * @param {Number} y The vector component 'y'.
      * @param {OpenSeadragon.Rect} bounds Where this tile fits, in normalized
      *      coordinates.
      * @param {Boolean} exists Is this tile a part of a sparse image? ( Also has
      *      this tile failed to load? )
-     * @param {String} url The URL of this tile's image.
+     * @param {String|Function} url The URL of this tile's image or a function that returns a url.
      * @param {CanvasRenderingContext2D} context2D The context2D of this tile if it
-     * is provided directly by the tile source.
+     *      is provided directly by the tile source.
      * @param {Boolean} loadWithAjax Whether this tile image should be loaded with an AJAX request .
      * @param {Object} ajaxHeaders The headers to send with this tile's AJAX request (if applicable).
      * @param {OpenSeadragon.Rect} sourceBounds The portion of the tile to use as the source of the
-     * drawing operation, in pixels. Note that this only works when drawing with canvas; when drawing
-     * with HTML the entire tile is always used.
+     *      drawing operation, in pixels. Note that this only works when drawing with canvas; when drawing
+     *      with HTML the entire tile is always used.
+     * @param {String} postData HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+     *      see TileSource::getPostData) or null
+     * @param {String} cacheKey key to act as a tile cache, must be unique for tiles with unique image data
      */
-    $.Tile = function(level, x, y, bounds, exists, url, context2D, loadWithAjax, ajaxHeaders, sourceBounds) {
+    $.Tile = function(level, x, y, bounds, exists, url, context2D, loadWithAjax, ajaxHeaders, sourceBounds, postData, cacheKey) {
         /**
          * The zoom level this tile belongs to.
          * @member {Number} level
          * @memberof OpenSeadragon.Tile#
          */
         this.level = level;
         /**
@@ -17643,19 +18387,29 @@
         /**
          * Is this tile a part of a sparse image? Also has this tile failed to load?
          * @member {Boolean} exists
          * @memberof OpenSeadragon.Tile#
          */
         this.exists = exists;
         /**
-         * The URL of this tile's image.
-         * @member {String} url
+         * Private property to hold string url or url retriever function.
+         * Consumers should access via Tile.getUrl()
+         * @private
+         * @member {String|Function} url
          * @memberof OpenSeadragon.Tile#
          */
-        this.url = url;
+        this._url = url;
+        /**
+         * Post parameters for this tile. For example, it can be an URL-encoded string
+         * in k1=v1&k2=v2... format, or a JSON, or a FormData instance... or null if no POST request used
+         * @member {String} postData HTTP POST data (usually but not necessarily in k=v&k2=v2... form,
+         *      see TileSource::getPostData) or null
+         * @memberof OpenSeadragon.Tile#
+         */
+        this.postData = postData;
         /**
          * The context2D of this tile if it is provided directly by the tile source.
          * @member {CanvasRenderingContext2D} context2D
          * @memberOf OpenSeadragon.Tile#
          */
         this.context2D = context2D;
         /**
@@ -17667,24 +18421,26 @@
         /**
          * The headers to be used in requesting this tile's image.
          * Only used if loadWithAjax is set to true.
          * @member {Object} ajaxHeaders
          * @memberof OpenSeadragon.Tile#
          */
         this.ajaxHeaders = ajaxHeaders;
+
+        if (cacheKey === undefined) {
+            $.console.warn("Tile constructor needs 'cacheKey' variable: creation tile cache" +
+                " in Tile class is deprecated. TileSource.prototype.getTileHashKey will be used.");
+            cacheKey = $.TileSource.prototype.getTileHashKey(level, x, y, url, ajaxHeaders, postData);
+        }
         /**
          * The unique cache key for this tile.
          * @member {String} cacheKey
          * @memberof OpenSeadragon.Tile#
          */
-        if (this.ajaxHeaders) {
-            this.cacheKey = this.url + "+" + JSON.stringify(this.ajaxHeaders);
-        } else {
-            this.cacheKey = this.url;
-        }
+        this.cacheKey = cacheKey;
         /**
          * Is this tile loaded?
          * @member {Boolean} loaded
          * @memberof OpenSeadragon.Tile#
          */
         this.loaded = false;
         /**
@@ -17702,20 +18458,14 @@
         this.element = null;
         /**
          * The HTML img element for this tile.
          * @member {Element} imgElement
          * @memberof OpenSeadragon.Tile#
          */
         this.imgElement = null;
-        /**
-         * The Image object for this tile.
-         * @member {Object} image
-         * @memberof OpenSeadragon.Tile#
-         */
-        this.image = null;
 
         /**
          * The alias of this.element.style.
          * @member {String} style
          * @memberof OpenSeadragon.Tile#
          */
         this.style = null;
@@ -17761,14 +18511,21 @@
          * The visibility score of this tile.
          * @member {Number} visibility
          * @memberof OpenSeadragon.Tile#
          */
         this.visibility = null;
 
         /**
+         * The transparency indicator of this tile.
+         * @member {Boolean} hasTransparency true if tile contains transparency for correct rendering
+         * @memberof OpenSeadragon.Tile#
+         */
+        this.hasTransparency = false;
+
+        /**
          * Whether this tile is currently being drawn.
          * @member {Boolean} beingDrawn
          * @memberof OpenSeadragon.Tile#
          */
         this.beingDrawn = false;
 
         /**
@@ -17804,15 +18561,17 @@
          */
         toString: function() {
             return this.level + "/" + this.x + "_" + this.y;
         },
 
         // private
         _hasTransparencyChannel: function() {
-            return !!this.context2D || this.url.match('.png');
+            console.warn("Tile.prototype._hasTransparencyChannel() has been " +
+                "deprecated and will be removed in the future. Use TileSource.prototype.hasTransparency() instead.");
+            return !!this.context2D || this.getUrl().match('.png');
         },
 
         /**
          * Renders the tile in an html container.
          * @function
          * @param {Element} container
          */
@@ -17832,16 +18591,21 @@
                 return;
             }
 
             //EXPERIMENTAL - trying to figure out how to scale the container
             //               content during animation of the container size.
 
             if (!this.element) {
+                var image = this.getImage();
+                if (!image) {
+                    return;
+                }
+
                 this.element = $.makeNeutralElement("div");
-                this.imgElement = this.cacheImageRecord.getImage().cloneNode();
+                this.imgElement = image.cloneNode();
                 this.imgElement.style.msInterpolationMode = "nearest-neighbor";
                 this.imgElement.style.width = "100%";
                 this.imgElement.style.height = "100%";
 
                 this.style = this.element.style;
                 this.style.position = "absolute";
             }
@@ -17861,49 +18625,105 @@
                 this.style.transform = "scaleX(-1)";
             }
 
             $.setElementOpacity(this.element, this.opacity);
         },
 
         /**
+         * The Image object for this tile.
+         * @member {Object} image
+         * @memberof OpenSeadragon.Tile#
+         * @deprecated
+         * @returns {Image}
+         */
+        get image() {
+            $.console.error("[Tile.image] property has been deprecated. Use [Tile.prototype.getImage] instead.");
+            return this.getImage();
+        },
+
+        /**
+         * The URL of this tile's image.
+         * @member {String} url
+         * @memberof OpenSeadragon.Tile#
+         * @deprecated
+         * @returns {String}
+         */
+        get url() {
+            $.console.error("[Tile.url] property has been deprecated. Use [Tile.prototype.getUrl] instead.");
+            return this.getUrl();
+        },
+
+        /**
+         * Get the Image object for this tile.
+         * @returns {Image}
+         */
+        getImage: function() {
+            return this.cacheImageRecord.getImage();
+        },
+
+        /**
+         * Get the url string for this tile.
+         * @returns {String}
+         */
+        getUrl: function() {
+            if (typeof this._url === 'function') {
+                return this._url();
+            }
+
+            return this._url;
+        },
+
+        /**
+         * Get the CanvasRenderingContext2D instance for tile image data drawn
+         * onto Canvas if enabled and available
+         * @returns {CanvasRenderingContext2D}
+         */
+        getCanvasContext: function() {
+            return this.context2D || this.cacheImageRecord.getRenderedContext();
+        },
+
+        /**
          * Renders the tile in a canvas-based context.
          * @function
          * @param {Canvas} context
          * @param {Function} drawingHandler - Method for firing the drawing event.
          * drawingHandler({context, tile, rendered})
          * where <code>rendered</code> is the context with the pre-drawn image.
          * @param {Number} [scale=1] - Apply a scale to position and size
          * @param {OpenSeadragon.Point} [translate] - A translation vector
+         * @param {Boolean} [shouldRoundPositionAndSize] - Tells whether to round
+         * position and size of tiles supporting alpha channel in non-transparency
+         * context.
+         * @param {OpenSeadragon.TileSource} source - The source specification of the tile.
          */
-        drawCanvas: function(context, drawingHandler, scale, translate) {
+        drawCanvas: function(context, drawingHandler, scale, translate, shouldRoundPositionAndSize, source) {
 
             var position = this.position.times($.pixelDensityRatio),
                 size = this.size.times($.pixelDensityRatio),
                 rendered;
 
             if (!this.context2D && !this.cacheImageRecord) {
                 $.console.warn(
                     '[Tile.drawCanvas] attempting to draw tile %s when it\'s not cached',
                     this.toString());
                 return;
             }
 
-            rendered = this.context2D || this.cacheImageRecord.getRenderedContext();
+            rendered = this.getCanvasContext();
 
             if (!this.loaded || !rendered) {
                 $.console.warn(
                     "Attempting to draw tile %s when it's not yet loaded.",
                     this.toString()
                 );
 
                 return;
             }
 
             context.save();
-
             context.globalAlpha = this.opacity;
 
             if (typeof scale === 'number' && scale !== 1) {
                 // draw tile at a different scale
                 position = position.times(scale);
                 size = size.times(scale);
             }
@@ -17913,15 +18733,23 @@
                 position = position.plus(translate);
             }
 
             //if we are supposed to be rendering fully opaque rectangle,
             //ie its done fading or fading is turned off, and if we are drawing
             //an image with an alpha channel, then the only way
             //to avoid seeing the tile underneath is to clear the rectangle
-            if (context.globalAlpha === 1 && this._hasTransparencyChannel()) {
+            if (context.globalAlpha === 1 && this.hasTransparency) {
+                if (shouldRoundPositionAndSize) {
+                    // Round to the nearest whole pixel so we don't get seams from overlap.
+                    position.x = Math.round(position.x);
+                    position.y = Math.round(position.y);
+                    size.x = Math.round(size.x);
+                    size.y = Math.round(size.y);
+                }
+
                 //clearing only the inside of the rectangle occupied
                 //by the png prevents edge flikering
                 context.clearRect(
                     position.x,
                     position.y,
                     size.x,
                     size.y
@@ -17963,15 +18791,15 @@
 
             context.restore();
         },
 
         /**
          * Get the ratio between current and original size.
          * @function
-         * @return {Float}
+         * @returns {Float}
          */
         getScaleForEdgeSmoothing: function() {
             var context;
             if (this.cacheImageRecord) {
                 context = this.cacheImageRecord.getRenderedContext();
             } else if (this.context2D) {
                 context = this.context2D;
@@ -17985,15 +18813,15 @@
         },
 
         /**
          * Get a translation vector that when applied to the tile position produces integer coordinates.
          * Needed to avoid swimming and twitching.
          * @function
          * @param {Number} [scale=1] - Scale to be applied to position.
-         * @return {OpenSeadragon.Point}
+         * @returns {OpenSeadragon.Point}
          */
         getTranslationForEdgeSmoothing: function(scale, canvasSize, sketchCanvasSize) {
             // The translation vector must have positive values, otherwise the image goes a bit off
             // the sketch canvas to the top and left and we must use negative coordinates to repaint it
             // to the main canvas. In that case, some browsers throw:
             // INDEX_SIZE_ERR: DOM Exception 1: Index or size was negative, or greater than the allowed value.
             var x = Math.max(1, Math.ceil((sketchCanvasSize.x - canvasSize.x) / 2));
@@ -18029,15 +18857,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Overlay
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -18326,26 +19154,26 @@
         // private
         _getOverlayPositionAndSize: function(viewport) {
             var position = viewport.pixelFromPoint(this.location, true);
             var size = this._getSizeInPixels(viewport);
             this.adjust(position, size);
 
             var rotate = 0;
-            if (viewport.degrees &&
+            if (viewport.getRotation(true) &&
                 this.rotationMode !== $.OverlayRotationMode.NO_ROTATION) {
                 // BOUNDING_BOX is only valid if both directions get scaled.
                 // Get replaced by EXACT otherwise.
                 if (this.rotationMode === $.OverlayRotationMode.BOUNDING_BOX &&
                     this.width !== null && this.height !== null) {
                     var rect = new $.Rect(position.x, position.y, size.x, size.y);
-                    var boundingBox = this._getBoundingBox(rect, viewport.degrees);
+                    var boundingBox = this._getBoundingBox(rect, viewport.getRotation(true));
                     position = boundingBox.getTopLeft();
                     size = boundingBox.getSize();
                 } else {
-                    rotate = viewport.degrees;
+                    rotate = viewport.getRotation(true);
                 }
             }
 
             return {
                 position: position,
                 size: size,
                 rotate: rotate
@@ -18474,15 +19302,15 @@
             return this._adjustBoundsForRotation(
                 viewport, new $.Rect(location.x, location.y, width, height));
         },
 
         // private
         _adjustBoundsForRotation: function(viewport, bounds) {
             if (!viewport ||
-                viewport.degrees === 0 ||
+                viewport.getRotation(true) === 0 ||
                 this.rotationMode === $.OverlayRotationMode.EXACT) {
                 return bounds;
             }
             if (this.rotationMode === $.OverlayRotationMode.BOUNDING_BOX) {
                 // If overlay not fully scalable, BOUNDING_BOX falls back to EXACT
                 if (this.width === null || this.height === null) {
                     return bounds;
@@ -18494,26 +19322,26 @@
                     positionAndSize.position.x,
                     positionAndSize.position.y,
                     positionAndSize.size.x,
                     positionAndSize.size.y));
             }
 
             // NO_ROTATION case
-            return bounds.rotate(-viewport.degrees,
+            return bounds.rotate(-viewport.getRotation(true),
                 this._getPlacementPoint(bounds));
         }
     };
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Drawer
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -18679,14 +19507,15 @@
 
         /**
          * This function converts the given point from to the drawer coordinate by
          * multiplying it with the pixel density.
          * This function does not take rotation into account, thus assuming provided
          * point is at 0 degree.
          * @param {OpenSeadragon.Point} point - the pixel point to convert
+         * @returns {OpenSeadragon.Point} Point in drawer coordinate system.
          */
         viewportCoordToDrawerCoord: function(point) {
             var vpPoint = this.viewport.pixelFromPointNoRotate(point, true);
             return new $.Point(
                 vpPoint.x * $.pixelDensityRatio,
                 vpPoint.y * $.pixelDensityRatio
             );
@@ -18711,15 +19540,15 @@
             });
             context.clip();
         },
 
         /**
          * Set the opacity of the drawer.
          * @param {Number} opacity
-         * @return {OpenSeadragon.Drawer} Chainable.
+         * @returns {OpenSeadragon.Drawer} Chainable.
          */
         setOpacity: function(opacity) {
             $.console.error("drawer.setOpacity is deprecated. Use tiledImage.setOpacity instead.");
             var world = this.viewer.world;
             for (var i = 0; i < world.getItemCount(); i++) {
                 world.getItemAt(i).setOpacity(opacity);
             }
@@ -18767,15 +19596,15 @@
             $.console.error("[Drawer.update] this function is deprecated. Use Drawer.clear and World.draw instead.");
             this.clear();
             this.viewer.world.draw();
             return this;
         },
 
         /**
-         * @return {Boolean} True if rotation is supported.
+         * @returns {Boolean} True if rotation is supported.
          */
         canRotate: function() {
             return this.useCanvas;
         },
 
         /**
          * Destroy the drawer (unload current loaded tiles)
@@ -18824,15 +19653,15 @@
             }
         },
 
         /**
          * Scale from OpenSeadragon viewer rectangle to drawer rectangle
          * (ignoring rotation)
          * @param {OpenSeadragon.Rect} rectangle - The rectangle in viewport coordinate system.
-         * @return {OpenSeadragon.Rect} Rectangle in drawer coordinate system.
+         * @returns {OpenSeadragon.Rect} Rectangle in drawer coordinate system.
          */
         viewportToDrawerRectangle: function(rectangle) {
             var topLeft = this.viewport.pixelFromPointNoRotate(rectangle.getTopLeft(), true);
             var size = this.viewport.deltaPixelsFromPointsNoRotate(rectangle.getSize(), true);
 
             return new $.Rect(
                 topLeft.x * $.pixelDensityRatio,
@@ -18847,23 +19676,27 @@
          * @param {OpenSeadragon.Tile} tile - The tile to draw.
          * @param {Function} drawingHandler - Method for firing the drawing event if using canvas.
          * drawingHandler({context, tile, rendered})
          * @param {Boolean} useSketch - Whether to use the sketch canvas or not.
          * where <code>rendered</code> is the context with the pre-drawn image.
          * @param {Float} [scale=1] - Apply a scale to tile position and size. Defaults to 1.
          * @param {OpenSeadragon.Point} [translate] A translation vector to offset tile position
+         * @param {Boolean} [shouldRoundPositionAndSize] - Tells whether to round
+         * position and size of tiles supporting alpha channel in non-transparency
+         * context.
+         * @param {OpenSeadragon.TileSource} source - The source specification of the tile.
          */
-        drawTile: function(tile, drawingHandler, useSketch, scale, translate) {
+        drawTile: function(tile, drawingHandler, useSketch, scale, translate, shouldRoundPositionAndSize, source) {
             $.console.assert(tile, '[Drawer.drawTile] tile is required');
             $.console.assert(drawingHandler, '[Drawer.drawTile] drawingHandler is required');
 
             if (this.useCanvas) {
                 var context = this._getContext(useSketch);
                 scale = scale || 1;
-                tile.drawCanvas(context, drawingHandler, scale, translate);
+                tile.drawCanvas(context, drawingHandler, scale, translate, shouldRoundPositionAndSize, source);
             } else {
                 tile.drawHTML(this.canvas);
             }
         },
 
         _getContext: function(useSketch) {
             var context = this.context;
@@ -19047,27 +19880,28 @@
             var context = this.context;
             context.save();
             context.lineWidth = 2 * $.pixelDensityRatio;
             context.font = 'small-caps bold ' + (13 * $.pixelDensityRatio) + 'px arial';
             context.strokeStyle = this.debugGridColor[colorIndex];
             context.fillStyle = this.debugGridColor[colorIndex];
 
-            if (this.viewport.degrees !== 0) {
+            if (this.viewport.getRotation(true) % 360 !== 0) {
                 this._offsetForRotation({
-                    degrees: this.viewport.degrees
+                    degrees: this.viewport.getRotation(true)
                 });
             }
             if (tiledImage.getRotation(true) % 360 !== 0) {
                 this._offsetForRotation({
                     degrees: tiledImage.getRotation(true),
                     point: tiledImage.viewport.pixelFromPointNoRotate(
                         tiledImage._getRotationPoint(true), true)
                 });
             }
-            if (tiledImage.viewport.degrees === 0 && tiledImage.getRotation(true) % 360 === 0) {
+            if (tiledImage.viewport.getRotation(true) % 360 === 0 &&
+                tiledImage.getRotation(true) % 360 === 0) {
                 if (tiledImage._drawer.viewer.viewport.getFlip()) {
                     tiledImage._drawer._flip();
                 }
             }
 
             context.strokeRect(
                 tile.position.x * $.pixelDensityRatio,
@@ -19077,15 +19911,15 @@
             );
 
             var tileCenterX = (tile.position.x + (tile.size.x / 2)) * $.pixelDensityRatio;
             var tileCenterY = (tile.position.y + (tile.size.y / 2)) * $.pixelDensityRatio;
 
             // Rotate the text the right way around.
             context.translate(tileCenterX, tileCenterY);
-            context.rotate(Math.PI / 180 * -this.viewport.degrees);
+            context.rotate(Math.PI / 180 * -this.viewport.getRotation(true));
             context.translate(-tileCenterX, -tileCenterY);
 
             if (tile.x === 0 && tile.y === 0) {
                 context.fillText(
                     "Zoom: " + this.viewport.getZoom(),
                     tile.position.x * $.pixelDensityRatio,
                     (tile.position.y - 30) * $.pixelDensityRatio
@@ -19123,22 +19957,23 @@
             );
             context.fillText(
                 "Position: " + tile.position.toString(),
                 (tile.position.x + 10) * $.pixelDensityRatio,
                 (tile.position.y + 70) * $.pixelDensityRatio
             );
 
-            if (this.viewport.degrees !== 0) {
+            if (this.viewport.getRotation(true) % 360 !== 0) {
                 this._restoreRotationChanges();
             }
             if (tiledImage.getRotation(true) % 360 !== 0) {
                 this._restoreRotationChanges();
             }
 
-            if (tiledImage.viewport.degrees === 0 && tiledImage.getRotation(true) % 360 === 0) {
+            if (tiledImage.viewport.getRotation(true) % 360 === 0 &&
+                tiledImage.getRotation(true) % 360 === 0) {
                 if (tiledImage._drawer.viewer.viewport.getFlip()) {
                     tiledImage._drawer._flip();
                 }
             }
 
             context.restore();
         },
@@ -19268,15 +20103,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - Viewport
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -19320,14 +20155,15 @@
      * @param {Boolean} [options.wrapHorizontal] - See wrapHorizontal in {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.wrapVertical] - See wrapVertical in {@link OpenSeadragon.Options}.
      * @param {Number} [options.defaultZoomLevel] - See defaultZoomLevel in {@link OpenSeadragon.Options}.
      * @param {Number} [options.minZoomLevel] - See minZoomLevel in {@link OpenSeadragon.Options}.
      * @param {Number} [options.maxZoomLevel] - See maxZoomLevel in {@link OpenSeadragon.Options}.
      * @param {Number} [options.degrees] - See degrees in {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.homeFillsViewer] - See homeFillsViewer in {@link OpenSeadragon.Options}.
+     * @param {Boolean} [options.silenceMultiImageWarnings] - See silenceMultiImageWarnings in {@link OpenSeadragon.Options}.
      */
     $.Viewport = function(options) {
 
         //backward compatibility for positional args while preferring more
         //idiomatic javascript options object as the only argument
         var args = arguments;
         if (args.length && args[0] instanceof $.Point) {
@@ -19351,38 +20187,43 @@
             top: 0,
             right: 0,
             bottom: 0
         }, options.margins || {});
 
         delete options.margins;
 
+        options.initialDegrees = options.degrees;
+        delete options.degrees;
+
         $.extend(true, this, {
 
             //required settings
             containerSize: null,
             contentSize: null,
 
             //internal state properties
             zoomPoint: null,
+            rotationPivot: null,
             viewer: null,
 
             //configurable options
             springStiffness: $.DEFAULT_SETTINGS.springStiffness,
             animationTime: $.DEFAULT_SETTINGS.animationTime,
             minZoomImageRatio: $.DEFAULT_SETTINGS.minZoomImageRatio,
             maxZoomPixelRatio: $.DEFAULT_SETTINGS.maxZoomPixelRatio,
             visibilityRatio: $.DEFAULT_SETTINGS.visibilityRatio,
             wrapHorizontal: $.DEFAULT_SETTINGS.wrapHorizontal,
             wrapVertical: $.DEFAULT_SETTINGS.wrapVertical,
             defaultZoomLevel: $.DEFAULT_SETTINGS.defaultZoomLevel,
             minZoomLevel: $.DEFAULT_SETTINGS.minZoomLevel,
             maxZoomLevel: $.DEFAULT_SETTINGS.maxZoomLevel,
-            degrees: $.DEFAULT_SETTINGS.degrees,
+            initialDegrees: $.DEFAULT_SETTINGS.degrees,
             flipped: $.DEFAULT_SETTINGS.flipped,
-            homeFillsViewer: $.DEFAULT_SETTINGS.homeFillsViewer
+            homeFillsViewer: $.DEFAULT_SETTINGS.homeFillsViewer,
+            silenceMultiImageWarnings: $.DEFAULT_SETTINGS.silenceMultiImageWarnings
 
         }, options);
 
         this._updateContainerInnerSize();
 
         this.centerSpringX = new $.Spring({
             initial: 0,
@@ -19397,31 +20238,51 @@
         this.zoomSpring = new $.Spring({
             exponential: true,
             initial: 1,
             springStiffness: this.springStiffness,
             animationTime: this.animationTime
         });
 
+        this.degreesSpring = new $.Spring({
+            initial: options.initialDegrees,
+            springStiffness: this.springStiffness,
+            animationTime: this.animationTime
+        });
+
         this._oldCenterX = this.centerSpringX.current.value;
         this._oldCenterY = this.centerSpringY.current.value;
         this._oldZoom = this.zoomSpring.current.value;
+        this._oldDegrees = this.degreesSpring.current.value;
 
         this._setContentBounds(new $.Rect(0, 0, 1, 1), 1);
 
         this.goHome(true);
         this.update();
     };
 
     /** @lends OpenSeadragon.Viewport.prototype */
     $.Viewport.prototype = {
+
+        // deprecated
+        get degrees() {
+            $.console.warn('Accessing [Viewport.degrees] is deprecated. Use viewport.getRotation instead.');
+            return this.getRotation();
+        },
+
+        // deprecated
+        set degrees(degrees) {
+            $.console.warn('Setting [Viewport.degrees] is deprecated. Use viewport.rotateTo, viewport.rotateBy, or viewport.setRotation instead.');
+            this.rotateTo(degrees);
+        },
+
         /**
          * Updates the viewport's home bounds and constraints for the given content size.
          * @function
          * @param {OpenSeadragon.Point} contentSize - size of the content in content units
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:reset-size
          */
         resetContentSize: function(contentSize) {
             $.console.assert(contentSize, "[Viewport.resetContentSize] contentSize is required");
             $.console.assert(contentSize instanceof $.Point, "[Viewport.resetContentSize] contentSize must be an OpenSeadragon.Point");
             $.console.assert(contentSize.x > 0, "[Viewport.resetContentSize] contentSize.x must be greater than 0");
             $.console.assert(contentSize.y > 0, "[Viewport.resetContentSize] contentSize.y must be greater than 0");
@@ -19448,15 +20309,15 @@
             $.console.assert(bounds.width > 0, "[Viewport._setContentBounds] bounds.width must be greater than 0");
             $.console.assert(bounds.height > 0, "[Viewport._setContentBounds] bounds.height must be greater than 0");
 
             this._contentBoundsNoRotate = bounds.clone();
             this._contentSizeNoRotate = this._contentBoundsNoRotate.getSize().times(
                 contentFactor);
 
-            this._contentBounds = bounds.rotate(this.degrees).getBoundingBox();
+            this._contentBounds = bounds.rotate(this.getRotation()).getBoundingBox();
             this._contentSize = this._contentBounds.getSize().times(contentFactor);
             this._contentAspectRatio = this._contentSize.x / this._contentSize.y;
 
             if (this.viewer) {
                 /**
                  * Raised when the viewer's content size or home bounds are reset
                  * (see {@link OpenSeadragon.Viewport#resetContentSize}).
@@ -19631,15 +20492,15 @@
         /**
          * Returns the bounds of the visible area in viewport coordinates.
          * @function
          * @param {Boolean} current - Pass true for the current location; defaults to false (target location).
          * @returns {OpenSeadragon.Rect} The location you are zoomed/panned to, in viewport coordinates.
          */
         getBounds: function(current) {
-            return this.getBoundsNoRotate(current).rotate(-this.getRotation());
+            return this.getBoundsNoRotate(current).rotate(-this.getRotation(current));
         },
 
         /**
          * Returns the bounds of the visible area in viewport coordinates.
          * This method ignores the viewport rotation. Use
          * {@link OpenSeadragon.Viewport#getBounds} to take it into account.
          * @function
@@ -19663,15 +20524,15 @@
          * @function
          * @param {Boolean} current - Pass true for the current location; defaults to false (target location).
          * @returns {OpenSeadragon.Rect} The location you are zoomed/panned to,
          * including the space taken by margins, in viewport coordinates.
          */
         getBoundsWithMargins: function(current) {
             return this.getBoundsNoRotateWithMargins(current).rotate(
-                -this.getRotation(), this.getCenter(current));
+                -this.getRotation(current), this.getCenter(current));
         },
 
         /**
          * @function
          * @param {Boolean} current - Pass true for the current location; defaults to false (target location).
          * @returns {OpenSeadragon.Rect} The location you are zoomed/panned to,
          * including the space taken by margins, in viewport coordinates.
@@ -19723,15 +20584,15 @@
                 centerCurrent.x - width / 2.0,
                 centerCurrent.y - height / 2.0,
                 width,
                 height
             );
 
             newZoomPixel = this._pixelFromPoint(this.zoomPoint, bounds);
-            deltaZoomPixels = newZoomPixel.minus(oldZoomPixel);
+            deltaZoomPixels = newZoomPixel.minus(oldZoomPixel).rotate(-this.getRotation(true));
             deltaZoomPoints = deltaZoomPixels.divide(this._containerInnerSize.x * zoom);
 
             return centerTarget.plus(deltaZoomPoints);
         },
 
         /**
          * @function
@@ -19752,60 +20613,86 @@
                 this.getMinZoom());
         },
 
         /**
          * @function
          * @private
          * @param {OpenSeadragon.Rect} bounds
-         * @return {OpenSeadragon.Rect} constrained bounds.
+         * @returns {OpenSeadragon.Rect} constrained bounds.
          */
         _applyBoundaryConstraints: function(bounds) {
-            var newBounds = new $.Rect(
-                bounds.x,
-                bounds.y,
-                bounds.width,
-                bounds.height);
+            var newBounds = this.viewportToViewerElementRectangle(bounds).getBoundingBox();
+            var cb = this.viewportToViewerElementRectangle(this._contentBoundsNoRotate).getBoundingBox();
+
+            var xConstrained = false;
+            var yConstrained = false;
 
             if (this.wrapHorizontal) {
                 //do nothing
             } else {
-                var horizontalThreshold = this.visibilityRatio * newBounds.width;
                 var boundsRight = newBounds.x + newBounds.width;
-                var contentRight = this._contentBoundsNoRotate.x + this._contentBoundsNoRotate.width;
-                var leftDx = this._contentBoundsNoRotate.x - boundsRight + horizontalThreshold;
-                var rightDx = contentRight - newBounds.x - horizontalThreshold;
+                var contentRight = cb.x + cb.width;
+
+                var horizontalThreshold, leftDx, rightDx;
+                if (newBounds.width > cb.width) {
+                    horizontalThreshold = this.visibilityRatio * cb.width;
+                } else {
+                    horizontalThreshold = this.visibilityRatio * newBounds.width;
+                }
 
-                if (horizontalThreshold > this._contentBoundsNoRotate.width) {
+                leftDx = cb.x - boundsRight + horizontalThreshold;
+                rightDx = contentRight - newBounds.x - horizontalThreshold;
+                if (horizontalThreshold > cb.width) {
                     newBounds.x += (leftDx + rightDx) / 2;
+                    xConstrained = true;
                 } else if (rightDx < 0) {
                     newBounds.x += rightDx;
+                    xConstrained = true;
                 } else if (leftDx > 0) {
                     newBounds.x += leftDx;
+                    xConstrained = true;
                 }
+
             }
 
             if (this.wrapVertical) {
                 //do nothing
             } else {
-                var verticalThreshold = this.visibilityRatio * newBounds.height;
                 var boundsBottom = newBounds.y + newBounds.height;
-                var contentBottom = this._contentBoundsNoRotate.y + this._contentBoundsNoRotate.height;
-                var topDy = this._contentBoundsNoRotate.y - boundsBottom + verticalThreshold;
-                var bottomDy = contentBottom - newBounds.y - verticalThreshold;
+                var contentBottom = cb.y + cb.height;
+
+                var verticalThreshold, topDy, bottomDy;
+                if (newBounds.height > cb.height) {
+                    verticalThreshold = this.visibilityRatio * cb.height;
+                } else {
+                    verticalThreshold = this.visibilityRatio * newBounds.height;
+                }
 
-                if (verticalThreshold > this._contentBoundsNoRotate.height) {
+                topDy = cb.y - boundsBottom + verticalThreshold;
+                bottomDy = contentBottom - newBounds.y - verticalThreshold;
+                if (verticalThreshold > cb.height) {
                     newBounds.y += (topDy + bottomDy) / 2;
+                    yConstrained = true;
                 } else if (bottomDy < 0) {
                     newBounds.y += bottomDy;
+                    yConstrained = true;
                 } else if (topDy > 0) {
                     newBounds.y += topDy;
+                    yConstrained = true;
                 }
+
             }
 
-            return newBounds;
+            var constraintApplied = xConstrained || yConstrained;
+            var newViewportBounds = constraintApplied ? this.viewerElementToViewportRectangle(newBounds) : bounds.clone();
+            newViewportBounds.xConstrained = xConstrained;
+            newViewportBounds.yConstrained = yConstrained;
+            newViewportBounds.constraintApplied = constraintApplied;
+
+            return newViewportBounds;
         },
 
         /**
          * @function
          * @private
          * @param {Boolean} [immediately=false] - whether the function that triggered this event was
          * called with the "immediately" flag
@@ -19830,56 +20717,52 @@
         },
 
         /**
          * Enforces the minZoom, maxZoom and visibilityRatio constraints by
          * zooming and panning to the closest acceptable zoom and location.
          * @function
          * @param {Boolean} [immediately=false]
-         * @return {OpenSeadragon.Viewport} Chainable.
-         * @fires OpenSeadragon.Viewer.event:constrain
+         * @returns {OpenSeadragon.Viewport} Chainable.
+         * @fires OpenSeadragon.Viewer.event:constrain if constraints were applied
          */
         applyConstraints: function(immediately) {
             var actualZoom = this.getZoom();
             var constrainedZoom = this._applyZoomConstraints(actualZoom);
 
             if (actualZoom !== constrainedZoom) {
                 this.zoomTo(constrainedZoom, this.zoomPoint, immediately);
             }
 
-            var bounds = this.getBoundsNoRotate();
-            var constrainedBounds = this._applyBoundaryConstraints(bounds);
-            this._raiseConstraintsEvent(immediately);
-
-            if (bounds.x !== constrainedBounds.x ||
-                bounds.y !== constrainedBounds.y ||
-                immediately) {
-                this.fitBounds(
-                    constrainedBounds.rotate(-this.getRotation()),
-                    immediately);
+            var constrainedBounds = this.getConstrainedBounds(false);
+
+            if (constrainedBounds.constraintApplied) {
+                this.fitBounds(constrainedBounds, immediately);
+                this._raiseConstraintsEvent(immediately);
             }
+
             return this;
         },
 
         /**
          * Equivalent to {@link OpenSeadragon.Viewport#applyConstraints}
          * @function
          * @param {Boolean} [immediately=false]
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:constrain
          */
         ensureVisible: function(immediately) {
             return this.applyConstraints(immediately);
         },
 
         /**
          * @function
          * @private
          * @param {OpenSeadragon.Rect} bounds
          * @param {Object} options (immediately=false, constraints=false)
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         _fitBounds: function(bounds, options) {
             options = options || {};
             var immediately = options.immediately || false;
             var constraints = options.constraints || false;
 
             var aspect = this.getAspectRatio();
@@ -19901,66 +20784,74 @@
             }
 
             // Compute x and y from width, height and center position
             newBounds.x = center.x - newBounds.width / 2;
             newBounds.y = center.y - newBounds.height / 2;
             var newZoom = 1.0 / newBounds.width;
 
-            if (constraints) {
-                var newBoundsAspectRatio = newBounds.getAspectRatio();
-                var newConstrainedZoom = this._applyZoomConstraints(newZoom);
-
-                if (newZoom !== newConstrainedZoom) {
-                    newZoom = newConstrainedZoom;
-                    newBounds.width = 1.0 / newZoom;
-                    newBounds.x = center.x - newBounds.width / 2;
-                    newBounds.height = newBounds.width / newBoundsAspectRatio;
-                    newBounds.y = center.y - newBounds.height / 2;
-                }
-
-                newBounds = this._applyBoundaryConstraints(newBounds);
-                center = newBounds.getCenter();
-                this._raiseConstraintsEvent(immediately);
-            }
-
             if (immediately) {
                 this.panTo(center, true);
-                return this.zoomTo(newZoom, null, true);
+                this.zoomTo(newZoom, null, true);
+                if (constraints) {
+                    this.applyConstraints(true);
+                }
+                return this;
             }
 
-            this.panTo(this.getCenter(true), true);
-            this.zoomTo(this.getZoom(true), null, true);
+            var currentCenter = this.getCenter(true);
+            var currentZoom = this.getZoom(true);
+            this.panTo(currentCenter, true);
+            this.zoomTo(currentZoom, null, true);
 
             var oldBounds = this.getBounds();
             var oldZoom = this.getZoom();
 
             if (oldZoom === 0 || Math.abs(newZoom / oldZoom - 1) < 0.00000001) {
-                this.zoomTo(newZoom, true);
-                return this.panTo(center, immediately);
+                this.zoomTo(newZoom, null, true);
+                this.panTo(center, immediately);
+                if (constraints) {
+                    this.applyConstraints(false);
+                }
+                return this;
             }
 
-            newBounds = newBounds.rotate(-this.getRotation());
-            var referencePoint = newBounds.getTopLeft().times(newZoom)
-                .minus(oldBounds.getTopLeft().times(oldZoom))
-                .divide(newZoom - oldZoom);
+            if (constraints) {
+                this.panTo(center, false);
+
+                newZoom = this._applyZoomConstraints(newZoom);
+                this.zoomTo(newZoom, null, false);
+
+                var constrainedBounds = this.getConstrainedBounds();
 
-            return this.zoomTo(newZoom, referencePoint, immediately);
+                this.panTo(currentCenter, true);
+                this.zoomTo(currentZoom, null, true);
+
+                this.fitBounds(constrainedBounds);
+            } else {
+                var rotatedNewBounds = newBounds.rotate(-this.getRotation());
+                var referencePoint = rotatedNewBounds.getTopLeft().times(newZoom)
+                    .minus(oldBounds.getTopLeft().times(oldZoom))
+                    .divide(newZoom - oldZoom);
+
+                this.zoomTo(newZoom, referencePoint, immediately);
+            }
+            return this;
         },
 
         /**
          * Makes the viewport zoom and pan so that the specified bounds take
          * as much space as possible in the viewport.
          * Note: this method ignores the constraints (minZoom, maxZoom and
          * visibilityRatio).
          * Use {@link OpenSeadragon.Viewport#fitBoundsWithConstraints} to enforce
          * them.
          * @function
          * @param {OpenSeadragon.Rect} bounds
          * @param {Boolean} [immediately=false]
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         fitBounds: function(bounds, immediately) {
             return this._fitBounds(bounds, {
                 immediately: immediately,
                 constraints: false
             });
         },
@@ -19971,41 +20862,41 @@
          * (minZoom, maxZoom and visibilityRatio).
          * Note: because this method enforces the constraints, part of the
          * provided bounds may end up outside of the viewport.
          * Use {@link OpenSeadragon.Viewport#fitBounds} to ignore them.
          * @function
          * @param {OpenSeadragon.Rect} bounds
          * @param {Boolean} [immediately=false]
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         fitBoundsWithConstraints: function(bounds, immediately) {
             return this._fitBounds(bounds, {
                 immediately: immediately,
                 constraints: true
             });
         },
 
         /**
          * Zooms so the image just fills the viewer vertically.
          * @param {Boolean} immediately
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         fitVertically: function(immediately) {
             var box = new $.Rect(
                 this._contentBounds.x + (this._contentBounds.width / 2),
                 this._contentBounds.y,
                 0,
                 this._contentBounds.height);
             return this.fitBounds(box, immediately);
         },
 
         /**
          * Zooms so the image just fills the viewer horizontally.
          * @param {Boolean} immediately
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         fitHorizontally: function(immediately) {
             var box = new $.Rect(
                 this._contentBounds.x,
                 this._contentBounds.y + (this._contentBounds.height / 2),
                 this._contentBounds.width,
                 0);
@@ -20013,15 +20904,18 @@
         },
 
 
         /**
          * Returns bounds taking constraints into account
          * Added to improve constrained panning
          * @param {Boolean} current - Pass true for the current location; defaults to false (target location).
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Rect} The bounds in viewport coordinates after applying constraints. The returned $.Rect
+         *                               contains additional properties constraintsApplied, xConstrained and yConstrained.
+         *                               These flags indicate whether the viewport bounds were modified by the constraints
+         *                               of the viewer rectangle, and in which dimension(s).
          */
         getConstrainedBounds: function(current) {
             var bounds,
                 constrainedBounds;
 
             bounds = this.getBounds(current);
 
@@ -20030,30 +20924,30 @@
             return constrainedBounds;
         },
 
         /**
          * @function
          * @param {OpenSeadragon.Point} delta
          * @param {Boolean} immediately
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:pan
          */
         panBy: function(delta, immediately) {
             var center = new $.Point(
                 this.centerSpringX.target.value,
                 this.centerSpringY.target.value
             );
             return this.panTo(center.plus(delta), immediately);
         },
 
         /**
          * @function
          * @param {OpenSeadragon.Point} center
          * @param {Boolean} immediately
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:pan
          */
         panTo: function(center, immediately) {
             if (immediately) {
                 this.centerSpringX.resetTo(center.x);
                 this.centerSpringY.resetTo(center.y);
             } else {
@@ -20080,30 +20974,30 @@
             }
 
             return this;
         },
 
         /**
          * @function
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:zoom
          */
         zoomBy: function(factor, refPoint, immediately) {
             return this.zoomTo(
                 this.zoomSpring.target.value * factor, refPoint, immediately);
         },
 
         /**
          * Zooms to the specified zoom level
          * @function
          * @param {Number} zoom The zoom level to zoom to.
          * @param {OpenSeadragon.Point} [refPoint] The point which will stay at
          * the same screen location. Defaults to the viewport center.
          * @param {Boolean} [immediately=false]
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:zoom
          */
         zoomTo: function(zoom, refPoint, immediately) {
             var _this = this;
 
             this.zoomPoint = refPoint instanceof $.Point &&
                 !isNaN(refPoint.x) &&
@@ -20142,54 +21036,140 @@
             return this;
         },
 
         /**
          * Rotates this viewport to the angle specified.
          * @function
          * @param {Number} degrees The degrees to set the rotation to.
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @param {Boolean} [immediately=false] Whether to animate to the new angle
+         * or rotate immediately.
+         * * @returns {OpenSeadragon.Viewport} Chainable.
          */
-        setRotation: function(degrees) {
+        setRotation: function(degrees, immediately) {
+            return this.rotateTo(degrees, null, immediately);
+        },
+
+        /**
+         * Gets the current rotation in degrees.
+         * @function
+         * @param {Boolean} [current=false] True for current rotation, false for target.
+         * @returns {Number} The current rotation in degrees.
+         */
+        getRotation: function(current) {
+            return current ?
+                this.degreesSpring.current.value :
+                this.degreesSpring.target.value;
+        },
+
+        /**
+         * Rotates this viewport to the angle specified around a pivot point. Alias for rotateTo.
+         * @function
+         * @param {Number} degrees The degrees to set the rotation to.
+         * @param {OpenSeadragon.Point} [pivot] (Optional) point in viewport coordinates
+         * around which the rotation should be performed. Defaults to the center of the viewport.
+         * @param {Boolean} [immediately=false] Whether to animate to the new angle
+         * or rotate immediately.
+         * * @returns {OpenSeadragon.Viewport} Chainable.
+         */
+        setRotationWithPivot: function(degrees, pivot, immediately) {
+            return this.rotateTo(degrees, pivot, immediately);
+        },
+
+        /**
+         * Rotates this viewport to the angle specified.
+         * @function
+         * @param {Number} degrees The degrees to set the rotation to.
+         * @param {OpenSeadragon.Point} [pivot] (Optional) point in viewport coordinates
+         * around which the rotation should be performed. Defaults to the center of the viewport.
+         * @param {Boolean} [immediately=false] Whether to animate to the new angle
+         * or rotate immediately.
+         * @returns {OpenSeadragon.Viewport} Chainable.
+         */
+        rotateTo: function(degrees, pivot, immediately) {
             if (!this.viewer || !this.viewer.drawer.canRotate()) {
                 return this;
             }
-            this.degrees = $.positiveModulo(degrees, 360);
+
+            if (this.degreesSpring.target.value === degrees &&
+                this.degreesSpring.isAtTargetValue()) {
+                return this;
+            }
+            this.rotationPivot = pivot instanceof $.Point &&
+                !isNaN(pivot.x) &&
+                !isNaN(pivot.y) ?
+                pivot :
+                null;
+            if (immediately) {
+                if (this.rotationPivot) {
+                    var changeInDegrees = degrees - this._oldDegrees;
+                    if (!changeInDegrees) {
+                        this.rotationPivot = null;
+                        return this;
+                    }
+                    this._rotateAboutPivot(degrees);
+                } else {
+                    this.degreesSpring.resetTo(degrees);
+                }
+            } else {
+                var normalizedFrom = $.positiveModulo(this.degreesSpring.current.value, 360);
+                var normalizedTo = $.positiveModulo(degrees, 360);
+                var diff = normalizedTo - normalizedFrom;
+                if (diff > 180) {
+                    normalizedTo -= 360;
+                } else if (diff < -180) {
+                    normalizedTo += 360;
+                }
+
+                var reverseDiff = normalizedFrom - normalizedTo;
+                this.degreesSpring.resetTo(degrees + reverseDiff);
+                this.degreesSpring.springTo(degrees);
+            }
+
             this._setContentBounds(
                 this.viewer.world.getHomeBounds(),
                 this.viewer.world.getContentFactor());
             this.viewer.forceRedraw();
 
             /**
              * Raised when rotation has been changed.
              *
              * @event rotate
              * @memberof OpenSeadragon.Viewer
              * @type {object}
              * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
              * @property {Number} degrees - The number of degrees the rotation was set to.
+             * @property {Boolean} immediately - Whether the rotation happened immediately or was animated
+             * @property {OpenSeadragon.Point} pivot - The point in viewport coordinates around which the rotation (if any) happened
              * @property {?Object} userData - Arbitrary subscriber-defined object.
              */
             this.viewer.raiseEvent('rotate', {
-                degrees: degrees
+                degrees: degrees,
+                immediately: !!immediately,
+                pivot: this.rotationPivot || this.getCenter()
             });
             return this;
         },
 
         /**
-         * Gets the current rotation in degrees.
+         * Rotates this viewport by the angle specified.
          * @function
-         * @return {Number} The current rotation in degrees.
+         * @param {Number} degrees The degrees by which to rotate the viewport.
+         * @param {OpenSeadragon.Point} [pivot] (Optional) point in viewport coordinates
+         * around which the rotation should be performed. Defaults to the center of the viewport.
+         * * @param {Boolean} [immediately=false] Whether to animate to the new angle
+         * or rotate immediately.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
-        getRotation: function() {
-            return this.degrees;
+        rotateBy: function(degrees, pivot, immediately) {
+            return this.rotateTo(this.degreesSpring.target.value + degrees, pivot, immediately);
         },
 
         /**
          * @function
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          * @fires OpenSeadragon.Viewer.event:resize
          */
         resize: function(newContainerSize, maintain) {
             var oldBounds = this.getBoundsNoRotate(),
                 newBounds = oldBounds,
                 widthDeltaFactor;
 
@@ -20203,15 +21183,18 @@
                 widthDeltaFactor = newContainerSize.x / this.containerSize.x;
                 newBounds.width = oldBounds.width * widthDeltaFactor;
                 newBounds.height = newBounds.width / this.getAspectRatio();
             }
 
             if (this.viewer) {
                 /**
-                 * Raised when the viewer is resized (see {@link OpenSeadragon.Viewport#resize}).
+                 * Raised when a viewer resize operation is initiated (see {@link OpenSeadragon.Viewport#resize}).
+                 * This event happens before the viewport bounds have been updated.
+                 * See also {@link OpenSeadragon.Viewer#after-resize} which reflects
+                 * the new viewport bounds following the resize action.
                  *
                  * @event resize
                  * @memberof OpenSeadragon.Viewer
                  * @type {object}
                  * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
                  * @property {OpenSeadragon.Point} newContainerSize
                  * @property {Boolean} maintain
@@ -20219,50 +21202,105 @@
                  */
                 this.viewer.raiseEvent('resize', {
                     newContainerSize: newContainerSize,
                     maintain: maintain
                 });
             }
 
-            return this.fitBounds(newBounds, true);
+            var output = this.fitBounds(newBounds, true);
+
+            if (this.viewer) {
+                /**
+                 * Raised after the viewer is resized (see {@link OpenSeadragon.Viewport#resize}).
+                 * See also {@link OpenSeadragon.Viewer#resize} event which happens
+                 * before the new bounds have been calculated and applied.
+                 *
+                 * @event after-resize
+                 * @memberof OpenSeadragon.Viewer
+                 * @type {object}
+                 * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised this event.
+                 * @property {OpenSeadragon.Point} newContainerSize
+                 * @property {Boolean} maintain
+                 * @property {?Object} userData - Arbitrary subscriber-defined object.
+                 */
+                this.viewer.raiseEvent('after-resize', {
+                    newContainerSize: newContainerSize,
+                    maintain: maintain
+                });
+            }
+
+            return output;
         },
 
         // private
         _updateContainerInnerSize: function() {
             this._containerInnerSize = new $.Point(
                 Math.max(1, this.containerSize.x - (this._margins.left + this._margins.right)),
                 Math.max(1, this.containerSize.y - (this._margins.top + this._margins.bottom))
             );
         },
 
         /**
-         * Update the zoom and center (X and Y) springs.
+         * Update the zoom, degrees, and center (X and Y) springs.
          * @function
          * @returns {Boolean} True if any change has been made, false otherwise.
          */
         update: function() {
             var _this = this;
             this._adjustCenterSpringsForZoomPoint(function() {
                 _this.zoomSpring.update();
             });
-
+            if (this.degreesSpring.isAtTargetValue()) {
+                this.rotationPivot = null;
+            }
             this.centerSpringX.update();
             this.centerSpringY.update();
 
+            if (this.rotationPivot) {
+                this._rotateAboutPivot(true);
+            } else {
+                this.degreesSpring.update();
+            }
+
+
             var changed = this.centerSpringX.current.value !== this._oldCenterX ||
                 this.centerSpringY.current.value !== this._oldCenterY ||
-                this.zoomSpring.current.value !== this._oldZoom;
+                this.zoomSpring.current.value !== this._oldZoom ||
+                this.degreesSpring.current.value !== this._oldDegrees;
+
 
             this._oldCenterX = this.centerSpringX.current.value;
             this._oldCenterY = this.centerSpringY.current.value;
             this._oldZoom = this.zoomSpring.current.value;
+            this._oldDegrees = this.degreesSpring.current.value;
 
             return changed;
         },
 
+        // private - pass true to use spring, or a number for degrees for immediate rotation
+        _rotateAboutPivot: function(degreesOrUseSpring) {
+            var useSpring = degreesOrUseSpring === true;
+
+            var delta = this.rotationPivot.minus(this.getCenter());
+            this.centerSpringX.shiftBy(delta.x);
+            this.centerSpringY.shiftBy(delta.y);
+
+            if (useSpring) {
+                this.degreesSpring.update();
+            } else {
+                this.degreesSpring.resetTo(degreesOrUseSpring);
+            }
+
+            var changeInDegrees = this.degreesSpring.current.value - this._oldDegrees;
+            var rdelta = delta.rotate(changeInDegrees * -1).times(-1);
+            this.centerSpringX.shiftBy(rdelta.x);
+            this.centerSpringY.shiftBy(rdelta.y);
+        },
+
+        // private
         _adjustCenterSpringsForZoomPoint: function(zoomSpringHandler) {
             if (this.zoomPoint) {
                 var oldZoomPixel = this.pixelFromPoint(this.zoomPoint, true);
                 zoomSpringHandler();
                 var newZoomPixel = this.pixelFromPoint(this.zoomPoint, true);
 
                 var deltaZoomPixels = newZoomPixel.minus(oldZoomPixel);
@@ -20301,15 +21339,15 @@
          * @param {OpenSeadragon.Point} deltaPoints - The translation vector to convert.
          * @param {Boolean} [current=false] - Pass true for the current location;
          * defaults to false (target location).
          * @returns {OpenSeadragon.Point}
          */
         deltaPixelsFromPoints: function(deltaPoints, current) {
             return this.deltaPixelsFromPointsNoRotate(
-                deltaPoints.rotate(this.getRotation()),
+                deltaPoints.rotate(this.getRotation(current)),
                 current);
         },
 
         /**
          * Convert a delta (translation vector) from pixels coordinates to viewport
          * coordinates. This method does not take rotation into account.
          * Consider using deltaPointsFromPixels if you need to account for rotation.
@@ -20330,15 +21368,15 @@
          * @param {OpenSeadragon.Point} deltaPixels - The translation vector to convert.
          * @param {Boolean} [current=false] - Pass true for the current location;
          * defaults to false (target location).
          * @returns {OpenSeadragon.Point}
          */
         deltaPointsFromPixels: function(deltaPixels, current) {
             return this.deltaPointsFromPixelsNoRotate(deltaPixels, current)
-                .rotate(-this.getRotation());
+                .rotate(-this.getRotation(current));
         },
 
         /**
          * Convert viewport coordinates to pixels coordinates.
          * This method does not take rotation into account.
          * Consider using pixelFromPoint if you need to account for rotation.
          * @param {OpenSeadragon.Point} point the viewport coordinates
@@ -20372,15 +21410,15 @@
                 new $.Point(this._margins.left, this._margins.top)
             );
         },
 
         // private
         _pixelFromPoint: function(point, bounds) {
             return this._pixelFromPointNoRotate(
-                point.rotate(this.getRotation(), this.getCenter(true)),
+                point.rotate(this.getRotation(true), this.getCenter(true)),
                 bounds);
         },
 
         /**
          * Convert pixel coordinates to viewport coordinates.
          * This method does not take rotation into account.
          * Consider using pointFromPixel if you need to account for rotation.
@@ -20405,16 +21443,16 @@
          * @param {OpenSeadragon.Point} pixel Pixel coordinates
          * @param {Boolean} [current=false] - Pass true for the current location;
          * defaults to false (target location).
          * @returns {OpenSeadragon.Point}
          */
         pointFromPixel: function(pixel, current) {
             return this.pointFromPixelNoRotate(pixel, current).rotate(
-                -this.getRotation(),
-                this.getCenter(true)
+                -this.getRotation(current),
+                this.getCenter(current)
             );
         },
 
         // private
         _viewportToImageDelta: function(viewerX, viewerY) {
             var scale = this._contentBoundsNoRotate.width;
             return new $.Point(
@@ -20427,27 +21465,29 @@
          * This method can be called either by passing X,Y coordinates or an
          * OpenSeadragon.Point
          * Note: not accurate with multi-image; use TiledImage.viewportToImageCoordinates instead.
          * @function
          * @param {(OpenSeadragon.Point|Number)} viewerX either a point or the X
          * coordinate in viewport coordinate system.
          * @param {Number} [viewerY] Y coordinate in viewport coordinate system.
-         * @return {OpenSeadragon.Point} a point representing the coordinates in the image.
+         * @returns {OpenSeadragon.Point} a point representing the coordinates in the image.
          */
         viewportToImageCoordinates: function(viewerX, viewerY) {
             if (viewerX instanceof $.Point) {
                 //they passed a point instead of individual components
                 return this.viewportToImageCoordinates(viewerX.x, viewerX.y);
             }
 
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.viewportToImageCoordinates] is not accurate ' +
-                        'with multi-image; use TiledImage.viewportToImageCoordinates instead.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.viewportToImageCoordinates] is not accurate ' +
+                            'with multi-image; use TiledImage.viewportToImageCoordinates instead.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.viewportToImageCoordinates
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.viewportToImageCoordinates(viewerX, viewerY, true);
                 }
@@ -20471,27 +21511,29 @@
          * This method can be called either by passing X,Y coordinates or an
          * OpenSeadragon.Point
          * Note: not accurate with multi-image; use TiledImage.imageToViewportCoordinates instead.
          * @function
          * @param {(OpenSeadragon.Point | Number)} imageX the point or the
          * X coordinate in image coordinate system.
          * @param {Number} [imageY] Y coordinate in image coordinate system.
-         * @return {OpenSeadragon.Point} a point representing the coordinates in the viewport.
+         * @returns {OpenSeadragon.Point} a point representing the coordinates in the viewport.
          */
         imageToViewportCoordinates: function(imageX, imageY) {
             if (imageX instanceof $.Point) {
                 //they passed a point instead of individual components
                 return this.imageToViewportCoordinates(imageX.x, imageX.y);
             }
 
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.imageToViewportCoordinates] is not accurate ' +
-                        'with multi-image; use TiledImage.imageToViewportCoordinates instead.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.imageToViewportCoordinates] is not accurate ' +
+                            'with multi-image; use TiledImage.imageToViewportCoordinates instead.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.viewportToImageCoordinates
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.imageToViewportCoordinates(imageX, imageY, true);
                 }
@@ -20524,16 +21566,18 @@
                 //they passed individual components instead of a rectangle
                 rect = new $.Rect(imageX, imageY, pixelWidth, pixelHeight);
             }
 
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.imageToViewportRectangle] is not accurate ' +
-                        'with multi-image; use TiledImage.imageToViewportRectangle instead.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.imageToViewportRectangle] is not accurate ' +
+                            'with multi-image; use TiledImage.imageToViewportRectangle instead.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.imageToViewportRectangle
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.imageToViewportRectangle(
                         imageX, imageY, pixelWidth, pixelHeight, true);
@@ -20572,16 +21616,18 @@
                 //they passed individual components instead of a rectangle
                 rect = new $.Rect(viewerX, viewerY, pointWidth, pointHeight);
             }
 
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.viewportToImageRectangle] is not accurate ' +
-                        'with multi-image; use TiledImage.viewportToImageRectangle instead.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.viewportToImageRectangle] is not accurate ' +
+                            'with multi-image; use TiledImage.viewportToImageRectangle instead.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.viewportToImageCoordinates
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.viewportToImageRectangle(
                         viewerX, viewerY, pointWidth, pointHeight, true);
@@ -20737,16 +21783,18 @@
          * target zoom.
          * @returns {Number} imageZoom The image zoom
          */
         viewportToImageZoom: function(viewportZoom) {
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.viewportToImageZoom] is not ' +
-                        'accurate with multi-image.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.viewportToImageZoom] is not ' +
+                            'accurate with multi-image.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.viewportToImageZoom
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.viewportToImageZoom(viewportZoom);
                 }
@@ -20771,16 +21819,18 @@
          * target zoom.
          * @returns {Number} viewportZoom The viewport zoom
          */
         imageToViewportZoom: function(imageZoom) {
             if (this.viewer) {
                 var count = this.viewer.world.getItemCount();
                 if (count > 1) {
-                    $.console.error('[Viewport.imageToViewportZoom] is not accurate ' +
-                        'with multi-image.');
+                    if (!this.silenceMultiImageWarnings) {
+                        $.console.error('[Viewport.imageToViewportZoom] is not accurate ' +
+                            'with multi-image.');
+                    }
                 } else if (count === 1) {
                     // It is better to use TiledImage.imageToViewportZoom
                     // because this._contentBoundsNoRotate can not be relied on
                     // with clipping.
                     var item = this.viewer.world.getItemAt(0);
                     return item.imageToViewportZoom(imageZoom);
                 }
@@ -20792,35 +21842,35 @@
             var viewportToImageZoomRatio = (imageWidth / containerWidth) / scale;
             return imageZoom * viewportToImageZoomRatio;
         },
 
         /**
          * Toggles flip state and demands a new drawing on navigator and viewer objects.
          * @function
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         toggleFlip: function() {
             this.setFlip(!this.getFlip());
             return this;
         },
 
         /**
          * Get flip state stored on viewport.
          * @function
-         * @return {Boolean} Flip state.
+         * @returns {Boolean} Flip state.
          */
         getFlip: function() {
             return this.flipped;
         },
 
         /**
          * Sets flip state according to the state input argument.
          * @function
          * @param {Boolean} state - Flip state to set.
-         * @return {OpenSeadragon.Viewport} Chainable.
+         * @returns {OpenSeadragon.Viewport} Chainable.
          */
         setFlip: function(state) {
             if (this.flipped === state) {
                 return this;
             }
 
             this.flipped = state;
@@ -20849,15 +21899,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - TiledImage
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -20919,15 +21969,16 @@
      * @param {Number} [options.blendTime] - See {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.alwaysBlend] - See {@link OpenSeadragon.Options}.
      * @param {Number} [options.minPixelRatio] - See {@link OpenSeadragon.Options}.
      * @param {Number} [options.smoothTileEdgesMinZoom] - See {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.iOSDevice] - See {@link OpenSeadragon.Options}.
      * @param {Number} [options.opacity=1] - Set to draw at proportional opacity. If zero, images will not draw.
      * @param {Boolean} [options.preload=false] - Set true to load even when the image is hidden by zero opacity.
-     * @param {String} [options.compositeOperation] - How the image is composited onto other images; see compositeOperation in {@link OpenSeadragon.Options} for possible values.
+     * @param {String} [options.compositeOperation] - How the image is composited onto other images; see compositeOperation in {@link OpenSeadragon.Options} for possible
+     values.
      * @param {Boolean} [options.debugMode] - See {@link OpenSeadragon.Options}.
      * @param {String|CanvasGradient|CanvasPattern|Function} [options.placeholderFillStyle] - See {@link OpenSeadragon.Options}.
      * @param {String|Boolean} [options.crossOriginPolicy] - See {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.ajaxWithCredentials] - See {@link OpenSeadragon.Options}.
      * @param {Boolean} [options.loadTilesWithAjax]
      *      Whether to load tile data using AJAX requests.
      *      Defaults to the setting in {@link OpenSeadragon.Options}.
@@ -20993,14 +22044,17 @@
         delete options.fitBounds;
         var fitBoundsPlacement = options.fitBoundsPlacement || OpenSeadragon.Placement.CENTER;
         delete options.fitBoundsPlacement;
 
         var degrees = options.degrees || 0;
         delete options.degrees;
 
+        var ajaxHeaders = options.ajaxHeaders;
+        delete options.ajaxHeaders;
+
         $.extend(true, this, {
 
             //internal state properties
             viewer: null,
             tilesMatrix: {}, // A '3d' dictionary [level][x][y] --> Tile.
             coverage: {}, // A '3d' dictionary [level][x][y] --> Boolean; shows what areas have been drawn.
             loadingCoverage: {}, // A '3d' dictionary [level][x][y] --> Boolean; shows what areas are loaded or are being loaded/blended.
@@ -21024,15 +22078,16 @@
             iOSDevice: $.DEFAULT_SETTINGS.iOSDevice,
             debugMode: $.DEFAULT_SETTINGS.debugMode,
             crossOriginPolicy: $.DEFAULT_SETTINGS.crossOriginPolicy,
             ajaxWithCredentials: $.DEFAULT_SETTINGS.ajaxWithCredentials,
             placeholderFillStyle: $.DEFAULT_SETTINGS.placeholderFillStyle,
             opacity: $.DEFAULT_SETTINGS.opacity,
             preload: $.DEFAULT_SETTINGS.preload,
-            compositeOperation: $.DEFAULT_SETTINGS.compositeOperation
+            compositeOperation: $.DEFAULT_SETTINGS.compositeOperation,
+            subPixelRoundingForTransparency: $.DEFAULT_SETTINGS.subPixelRoundingForTransparency
         }, options);
 
         this._preload = this.preload;
         delete this.preload;
 
         this._fullyLoaded = false;
 
@@ -21083,14 +22138,17 @@
              * @property {OpenSeadragon.Tile} rendered - The HTML canvas context containing the tile imagery.
              * @property {?Object} userData - Arbitrary subscriber-defined object.
              */
             _this.viewer.raiseEvent('tile-drawing', $.extend({
                 tiledImage: _this
             }, args));
         };
+
+        this._ownAjaxHeaders = {};
+        this.setAjaxHeaders(ajaxHeaders, false);
     };
 
     $.extend($.TiledImage.prototype, $.EventSource.prototype, /** @lends OpenSeadragon.TiledImage.prototype */ {
         /**
          * @returns {Boolean} Whether the TiledImage needs to be drawn.
          */
         needsDraw: function() {
@@ -21288,15 +22346,15 @@
 
         /**
          * Translates from OpenSeadragon viewer coordinate system to image coordinate system.
          * This method can be called either by passing X,Y coordinates or an {@link OpenSeadragon.Point}.
          * @param {Number|OpenSeadragon.Point} viewerX - The X coordinate or point in viewport coordinate system.
          * @param {Number} [viewerY] - The Y coordinate in viewport coordinate system.
          * @param {Boolean} [current=false] - Pass true to use the current location; false for target location.
-         * @return {OpenSeadragon.Point} A point representing the coordinates in the image.
+         * @returns {OpenSeadragon.Point} A point representing the coordinates in the image.
          */
         viewportToImageCoordinates: function(viewerX, viewerY, current) {
             var point;
             if (viewerX instanceof $.Point) {
                 //they passed a point instead of individual components
                 current = viewerY;
                 point = viewerX;
@@ -21323,15 +22381,15 @@
 
         /**
          * Translates from image coordinate system to OpenSeadragon viewer coordinate system
          * This method can be called either by passing X,Y coordinates or an {@link OpenSeadragon.Point}.
          * @param {Number|OpenSeadragon.Point} imageX - The X coordinate or point in image coordinate system.
          * @param {Number} [imageY] - The Y coordinate in image coordinate system.
          * @param {Boolean} [current=false] - Pass true to use the current location; false for target location.
-         * @return {OpenSeadragon.Point} A point representing the coordinates in the viewport.
+         * @returns {OpenSeadragon.Point} A point representing the coordinates in the viewport.
          */
         imageToViewportCoordinates: function(imageX, imageY, current) {
             if (imageX instanceof $.Point) {
                 //they passed a point instead of individual components
                 current = imageY;
                 imageY = imageX.y;
                 imageX = imageX.x;
@@ -21354,15 +22412,15 @@
          * pixel coordinates to OpenSeadragon viewport rectangle coordinates.
          * This method can be called either by passing X,Y,width,height or an {@link OpenSeadragon.Rect}.
          * @param {Number|OpenSeadragon.Rect} imageX - The left coordinate or rectangle in image coordinate system.
          * @param {Number} [imageY] - The top coordinate in image coordinate system.
          * @param {Number} [pixelWidth] - The width in pixel of the rectangle.
          * @param {Number} [pixelHeight] - The height in pixel of the rectangle.
          * @param {Boolean} [current=false] - Pass true to use the current location; false for target location.
-         * @return {OpenSeadragon.Rect} A rect representing the coordinates in the viewport.
+         * @returns {OpenSeadragon.Rect} A rect representing the coordinates in the viewport.
          */
         imageToViewportRectangle: function(imageX, imageY, pixelWidth, pixelHeight, current) {
             var rect = imageX;
             if (rect instanceof $.Rect) {
                 //they passed a rect instead of individual components
                 current = imageY;
             } else {
@@ -21386,15 +22444,15 @@
          * the viewport in point coordinates to image rectangle coordinates.
          * This method can be called either by passing X,Y,width,height or an {@link OpenSeadragon.Rect}.
          * @param {Number|OpenSeadragon.Rect} viewerX - The left coordinate or rectangle in viewport coordinate system.
          * @param {Number} [viewerY] - The top coordinate in viewport coordinate system.
          * @param {Number} [pointWidth] - The width in viewport coordinate system.
          * @param {Number} [pointHeight] - The height in viewport coordinate system.
          * @param {Boolean} [current=false] - Pass true to use the current location; false for target location.
-         * @return {OpenSeadragon.Rect} A rect representing the coordinates in the image.
+         * @returns {OpenSeadragon.Rect} A rect representing the coordinates in the image.
          */
         viewportToImageRectangle: function(viewerX, viewerY, pointWidth, pointHeight, current) {
             var rect = viewerX;
             if (viewerX instanceof $.Rect) {
                 //they passed a rect instead of individual components
                 current = viewerY;
             } else {
@@ -21851,14 +22909,98 @@
              * @property {?Object} userData - Arbitrary subscriber-defined object.
              */
             this.raiseEvent('composite-operation-change', {
                 compositeOperation: this.compositeOperation
             });
         },
 
+        /**
+         * Update headers to include when making AJAX requests.
+         *
+         * Unless `propagate` is set to false (which is likely only useful in rare circumstances),
+         * the updated headers are propagated to all tiles and queued image loader jobs.
+         *
+         * Note that the rules for merging headers still apply, i.e. headers returned by
+         * {@link OpenSeadragon.TileSource#getTileAjaxHeaders} take precedence over
+         * the headers here in the tiled image (`TiledImage.ajaxHeaders`).
+         *
+         * @function
+         * @param {Object} ajaxHeaders Updated AJAX headers, which will be merged over any headers specified in {@link OpenSeadragon.Options}.
+         * @param {Boolean} [propagate=true] Whether to propagate updated headers to existing tiles and queued image loader jobs.
+         */
+        setAjaxHeaders: function(ajaxHeaders, propagate) {
+            if (ajaxHeaders === null) {
+                ajaxHeaders = {};
+            }
+            if (!$.isPlainObject(ajaxHeaders)) {
+                console.error('[TiledImage.setAjaxHeaders] Ignoring invalid headers, must be a plain object');
+                return;
+            }
+
+            this._ownAjaxHeaders = ajaxHeaders;
+            this._updateAjaxHeaders(propagate);
+        },
+
+        /**
+         * Update headers to include when making AJAX requests.
+         *
+         * This function has the same effect as calling {@link OpenSeadragon.TiledImage#setAjaxHeaders},
+         * except that the headers for this tiled image do not change. This is especially useful
+         * for propagating updated headers from {@link OpenSeadragon.TileSource#getTileAjaxHeaders}
+         * to existing tiles.
+         *
+         * @private
+         * @function
+         * @param {Boolean} [propagate=true] Whether to propagate updated headers to existing tiles and queued image loader jobs.
+         */
+        _updateAjaxHeaders: function(propagate) {
+            if (propagate === undefined) {
+                propagate = true;
+            }
+
+            // merge with viewer's headers
+            if ($.isPlainObject(this.viewer.ajaxHeaders)) {
+                this.ajaxHeaders = $.extend({}, this.viewer.ajaxHeaders, this._ownAjaxHeaders);
+            } else {
+                this.ajaxHeaders = this._ownAjaxHeaders;
+            }
+
+            // propagate header updates to all tiles and queued image loader jobs
+            if (propagate) {
+                var numTiles, xMod, yMod, tile;
+
+                for (var level in this.tilesMatrix) {
+                    numTiles = this.source.getNumTiles(level);
+
+                    for (var x in this.tilesMatrix[level]) {
+                        xMod = (numTiles.x + (x % numTiles.x)) % numTiles.x;
+
+                        for (var y in this.tilesMatrix[level][x]) {
+                            yMod = (numTiles.y + (y % numTiles.y)) % numTiles.y;
+                            tile = this.tilesMatrix[level][x][y];
+
+                            tile.loadWithAjax = this.loadTilesWithAjax;
+                            if (tile.loadWithAjax) {
+                                var tileAjaxHeaders = this.source.getTileAjaxHeaders(level, xMod, yMod);
+                                tile.ajaxHeaders = $.extend({}, this.ajaxHeaders, tileAjaxHeaders);
+                            } else {
+                                tile.ajaxHeaders = null;
+                            }
+                        }
+                    }
+                }
+
+                for (var i = 0; i < this._imageLoader.jobQueue.length; i++) {
+                    var job = this._imageLoader.jobQueue[i];
+                    job.loadWithAjax = job.tile.loadWithAjax;
+                    job.ajaxHeaders = job.tile.loadWithAjax ? job.tile.ajaxHeaders : null;
+                }
+            }
+        },
+
         // private
         _setScale: function(scale, immediately) {
             var sameTarget = (this._scaleSpring.target.value === scale);
             if (immediately) {
                 if (sameTarget && this._scaleSpring.current.value === scale) {
                     return;
                 }
@@ -22011,39 +23153,38 @@
                 var optimalRatio = this.immediateRender ? 1 : targetZeroRatio;
                 var levelOpacity = Math.min(1, (currentRenderPixelRatio - 0.5) / 0.5);
                 var levelVisibility = optimalRatio / Math.abs(
                     optimalRatio - targetRenderPixelRatio
                 );
 
                 // Update the level and keep track of 'best' tile to load
-                bestTile = updateLevel(
-                    this,
+                bestTile = this._updateLevel(
                     haveDrawn,
                     drawLevel,
                     level,
                     levelOpacity,
                     levelVisibility,
                     drawArea,
                     currentTime,
                     bestTile
                 );
 
                 // Stop the loop if lower-res tiles would all be covered by
                 // already drawn tiles
-                if (providesCoverage(this.coverage, level)) {
+                if (this._providesCoverage(this.coverage, level)) {
                     break;
                 }
             }
 
             // Perform the actual drawing
-            drawTiles(this, this.lastDrawn);
+            this._drawTiles(this.lastDrawn);
 
             // Load the new 'best' tile
             if (bestTile && !bestTile.context2D) {
-                loadTile(this, bestTile, currentTime);
+                this._loadTile(bestTile, currentTime);
                 this._needsDraw = true;
                 this._setFullyLoaded(false);
             } else {
                 this._setFullyLoaded(this._tilesLoading === 0);
             }
         },
 
@@ -22082,990 +23223,1083 @@
                 bottomRightTile.y += numTiles.y * Math.floor(bottomRightBound.y / aspectRatio);
             }
 
             return {
                 topLeft: topLeftTile,
                 bottomRight: bottomRightTile,
             };
-        }
-    });
-
-    /**
-     * @private
-     * @inner
-     * Updates all tiles at a given resolution level.
-     * @param {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
-     * @param {Boolean} haveDrawn
-     * @param {Boolean} drawLevel
-     * @param {Number} level
-     * @param {Number} levelOpacity
-     * @param {Number} levelVisibility
-     * @param {OpenSeadragon.Point} viewportTL - The index of the most top-left visible tile.
-     * @param {OpenSeadragon.Point} viewportBR - The index of the most bottom-right visible tile.
-     * @param {Number} currentTime
-     * @param {OpenSeadragon.Tile} best - The current "best" tile to draw.
-     */
-    function updateLevel(tiledImage, haveDrawn, drawLevel, level, levelOpacity,
-        levelVisibility, drawArea, currentTime, best) {
-
-        var topLeftBound = drawArea.getBoundingBox().getTopLeft();
-        var bottomRightBound = drawArea.getBoundingBox().getBottomRight();
+        },
 
-        if (tiledImage.viewer) {
-            /**
-             * <em>- Needs documentation -</em>
-             *
-             * @event update-level
-             * @memberof OpenSeadragon.Viewer
-             * @type {object}
-             * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
-             * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
-             * @property {Object} havedrawn
-             * @property {Object} level
-             * @property {Object} opacity
-             * @property {Object} visibility
-             * @property {OpenSeadragon.Rect} drawArea
-             * @property {Object} topleft deprecated, use drawArea instead
-             * @property {Object} bottomright deprecated, use drawArea instead
-             * @property {Object} currenttime
-             * @property {Object} best
-             * @property {?Object} userData - Arbitrary subscriber-defined object.
-             */
-            tiledImage.viewer.raiseEvent('update-level', {
-                tiledImage: tiledImage,
-                havedrawn: haveDrawn,
-                level: level,
-                opacity: levelOpacity,
-                visibility: levelVisibility,
-                drawArea: drawArea,
-                topleft: topLeftBound,
-                bottomright: bottomRightBound,
-                currenttime: currentTime,
-                best: best
-            });
-        }
+        /**
+         * Updates all tiles at a given resolution level.
+         * @private
+         * @param {Boolean} haveDrawn
+         * @param {Boolean} drawLevel
+         * @param {Number} level
+         * @param {Number} levelOpacity
+         * @param {Number} levelVisibility
+         * @param {OpenSeadragon.Rect} drawArea
+         * @param {Number} currentTime
+         * @param {OpenSeadragon.Tile} best - The current "best" tile to draw.
+         */
+        _updateLevel: function(haveDrawn, drawLevel, level, levelOpacity,
+            levelVisibility, drawArea, currentTime, best) {
 
-        resetCoverage(tiledImage.coverage, level);
-        resetCoverage(tiledImage.loadingCoverage, level);
+            var topLeftBound = drawArea.getBoundingBox().getTopLeft();
+            var bottomRightBound = drawArea.getBoundingBox().getBottomRight();
 
-        //OK, a new drawing so do your calculations
-        var cornerTiles = tiledImage._getCornerTiles(level, topLeftBound, bottomRightBound);
-        var topLeftTile = cornerTiles.topLeft;
-        var bottomRightTile = cornerTiles.bottomRight;
-        var numberOfTiles = tiledImage.source.getNumTiles(level);
-
-        var viewportCenter = tiledImage.viewport.pixelFromPoint(
-            tiledImage.viewport.getCenter());
-
-        if (tiledImage.getFlip()) {
-            // The right-most tile can be narrower than the others. When flipped,
-            // this tile is now on the left. Because it is narrower than the normal
-            // left-most tile, the subsequent tiles may not be wide enough to completely
-            // fill the viewport. Fix this by rendering an extra column of tiles. If we
-            // are not wrapping, make sure we never render more than the number of tiles
-            // in the image.
-            bottomRightTile.x += 1;
-            if (!tiledImage.wrapHorizontal) {
-                bottomRightTile.x = Math.min(bottomRightTile.x, numberOfTiles.x - 1);
+            if (this.viewer) {
+                /**
+                 * <em>- Needs documentation -</em>
+                 *
+                 * @event update-level
+                 * @memberof OpenSeadragon.Viewer
+                 * @type {object}
+                 * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
+                 * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
+                 * @property {Object} havedrawn
+                 * @property {Object} level
+                 * @property {Object} opacity
+                 * @property {Object} visibility
+                 * @property {OpenSeadragon.Rect} drawArea
+                 * @property {Object} topleft deprecated, use drawArea instead
+                 * @property {Object} bottomright deprecated, use drawArea instead
+                 * @property {Object} currenttime
+                 * @property {Object} best
+                 * @property {?Object} userData - Arbitrary subscriber-defined object.
+                 */
+                this.viewer.raiseEvent('update-level', {
+                    tiledImage: this,
+                    havedrawn: haveDrawn,
+                    level: level,
+                    opacity: levelOpacity,
+                    visibility: levelVisibility,
+                    drawArea: drawArea,
+                    topleft: topLeftBound,
+                    bottomright: bottomRightBound,
+                    currenttime: currentTime,
+                    best: best
+                });
             }
-        }
 
-        for (var x = topLeftTile.x; x <= bottomRightTile.x; x++) {
-            for (var y = topLeftTile.y; y <= bottomRightTile.y; y++) {
-
-                var flippedX;
-                if (tiledImage.getFlip()) {
-                    var xMod = (numberOfTiles.x + (x % numberOfTiles.x)) % numberOfTiles.x;
-                    flippedX = x + numberOfTiles.x - xMod - xMod - 1;
-                } else {
-                    flippedX = x;
-                }
+            this._resetCoverage(this.coverage, level);
+            this._resetCoverage(this.loadingCoverage, level);
 
-                if (drawArea.intersection(tiledImage.getTileBounds(level, flippedX, y)) === null) {
-                    // This tile is outside of the viewport, no need to draw it
-                    continue;
-                }
+            //OK, a new drawing so do your calculations
+            var cornerTiles = this._getCornerTiles(level, topLeftBound, bottomRightBound);
+            var topLeftTile = cornerTiles.topLeft;
+            var bottomRightTile = cornerTiles.bottomRight;
+            var numberOfTiles = this.source.getNumTiles(level);
 
-                best = updateTile(
-                    tiledImage,
-                    drawLevel,
-                    haveDrawn,
-                    flippedX, y,
-                    level,
-                    levelOpacity,
-                    levelVisibility,
-                    viewportCenter,
-                    numberOfTiles,
-                    currentTime,
-                    best
-                );
+            var viewportCenter = this.viewport.pixelFromPoint(this.viewport.getCenter());
 
+            if (this.getFlip()) {
+                // The right-most tile can be narrower than the others. When flipped,
+                // this tile is now on the left. Because it is narrower than the normal
+                // left-most tile, the subsequent tiles may not be wide enough to completely
+                // fill the viewport. Fix this by rendering an extra column of tiles. If we
+                // are not wrapping, make sure we never render more than the number of tiles
+                // in the image.
+                bottomRightTile.x += 1;
+                if (!this.wrapHorizontal) {
+                    bottomRightTile.x = Math.min(bottomRightTile.x, numberOfTiles.x - 1);
+                }
             }
-        }
 
-        return best;
-    }
+            for (var x = topLeftTile.x; x <= bottomRightTile.x; x++) {
+                for (var y = topLeftTile.y; y <= bottomRightTile.y; y++) {
+
+                    var flippedX;
+                    if (this.getFlip()) {
+                        var xMod = (numberOfTiles.x + (x % numberOfTiles.x)) % numberOfTiles.x;
+                        flippedX = x + numberOfTiles.x - xMod - xMod - 1;
+                    } else {
+                        flippedX = x;
+                    }
 
-    /**
-     * @private
-     * @inner
-     * Update a single tile at a particular resolution level.
-     * @param {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
-     * @param {Boolean} haveDrawn
-     * @param {Boolean} drawLevel
-     * @param {Number} x
-     * @param {Number} y
-     * @param {Number} level
-     * @param {Number} levelOpacity
-     * @param {Number} levelVisibility
-     * @param {OpenSeadragon.Point} viewportCenter
-     * @param {Number} numberOfTiles
-     * @param {Number} currentTime
-     * @param {OpenSeadragon.Tile} best - The current "best" tile to draw.
-     */
-    function updateTile(tiledImage, haveDrawn, drawLevel, x, y, level, levelOpacity, levelVisibility, viewportCenter, numberOfTiles, currentTime, best) {
-
-        var tile = getTile(
-                x, y,
-                level,
-                tiledImage,
-                tiledImage.source,
-                tiledImage.tilesMatrix,
-                currentTime,
-                numberOfTiles,
-                tiledImage._worldWidthCurrent,
-                tiledImage._worldHeightCurrent
-            ),
-            drawTile = drawLevel;
+                    if (drawArea.intersection(this.getTileBounds(level, flippedX, y)) === null) {
+                        // This tile is outside of the viewport, no need to draw it
+                        continue;
+                    }
 
-        if (tiledImage.viewer) {
-            /**
-             * <em>- Needs documentation -</em>
-             *
-             * @event update-tile
-             * @memberof OpenSeadragon.Viewer
-             * @type {object}
-             * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
-             * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
-             * @property {OpenSeadragon.Tile} tile
-             * @property {?Object} userData - Arbitrary subscriber-defined object.
-             */
-            tiledImage.viewer.raiseEvent('update-tile', {
-                tiledImage: tiledImage,
-                tile: tile
-            });
-        }
+                    best = this._updateTile(
+                        drawLevel,
+                        haveDrawn,
+                        flippedX, y,
+                        level,
+                        levelOpacity,
+                        levelVisibility,
+                        viewportCenter,
+                        numberOfTiles,
+                        currentTime,
+                        best
+                    );
+                }
+            }
 
-        setCoverage(tiledImage.coverage, level, x, y, false);
+            return best;
+        },
 
-        var loadingCoverage = tile.loaded || tile.loading || isCovered(tiledImage.loadingCoverage, level, x, y);
-        setCoverage(tiledImage.loadingCoverage, level, x, y, loadingCoverage);
+        /**
+         * @private
+         * @inner
+         * Update a single tile at a particular resolution level.
+         * @param {Boolean} haveDrawn
+         * @param {Boolean} drawLevel
+         * @param {Number} x
+         * @param {Number} y
+         * @param {Number} level
+         * @param {Number} levelOpacity
+         * @param {Number} levelVisibility
+         * @param {OpenSeadragon.Point} viewportCenter
+         * @param {Number} numberOfTiles
+         * @param {Number} currentTime
+         * @param {OpenSeadragon.Tile} best - The current "best" tile to draw.
+         */
+        _updateTile: function(haveDrawn, drawLevel, x, y, level, levelOpacity,
+            levelVisibility, viewportCenter, numberOfTiles, currentTime, best) {
 
-        if (!tile.exists) {
-            return best;
-        }
+            var tile = this._getTile(
+                    x, y,
+                    level,
+                    currentTime,
+                    numberOfTiles,
+                    this._worldWidthCurrent,
+                    this._worldHeightCurrent
+                ),
+                drawTile = drawLevel;
 
-        if (haveDrawn && !drawTile) {
-            if (isCovered(tiledImage.coverage, level, x, y)) {
-                setCoverage(tiledImage.coverage, level, x, y, true);
-            } else {
-                drawTile = true;
+            if (this.viewer) {
+                /**
+                 * <em>- Needs documentation -</em>
+                 *
+                 * @event update-tile
+                 * @memberof OpenSeadragon.Viewer
+                 * @type {object}
+                 * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
+                 * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
+                 * @property {OpenSeadragon.Tile} tile
+                 * @property {?Object} userData - Arbitrary subscriber-defined object.
+                 */
+                this.viewer.raiseEvent('update-tile', {
+                    tiledImage: this,
+                    tile: tile
+                });
             }
-        }
 
-        if (!drawTile) {
-            return best;
-        }
+            this._setCoverage(this.coverage, level, x, y, false);
 
-        positionTile(
-            tile,
-            tiledImage.source.tileOverlap,
-            tiledImage.viewport,
-            viewportCenter,
-            levelVisibility,
-            tiledImage
-        );
+            var loadingCoverage = tile.loaded || tile.loading || this._isCovered(this.loadingCoverage, level, x, y);
+            this._setCoverage(this.loadingCoverage, level, x, y, loadingCoverage);
 
-        if (!tile.loaded) {
-            if (tile.context2D) {
-                setTileLoaded(tiledImage, tile);
-            } else {
-                var imageRecord = tiledImage._tileCache.getImageRecord(tile.cacheKey);
-                if (imageRecord) {
-                    var image = imageRecord.getImage();
-                    setTileLoaded(tiledImage, tile, image);
+            if (!tile.exists) {
+                return best;
+            }
+
+            if (haveDrawn && !drawTile) {
+                if (this._isCovered(this.coverage, level, x, y)) {
+                    this._setCoverage(this.coverage, level, x, y, true);
+                } else {
+                    drawTile = true;
                 }
             }
-        }
 
-        if (tile.loaded) {
-            var needsDraw = blendTile(
-                tiledImage,
+            if (!drawTile) {
+                return best;
+            }
+
+            this._positionTile(
                 tile,
-                x, y,
-                level,
-                levelOpacity,
-                currentTime
+                this.source.tileOverlap,
+                this.viewport,
+                viewportCenter,
+                levelVisibility
             );
 
-            if (needsDraw) {
-                tiledImage._needsDraw = true;
+            if (!tile.loaded) {
+                if (tile.context2D) {
+                    this._setTileLoaded(tile);
+                } else {
+                    var imageRecord = this._tileCache.getImageRecord(tile.cacheKey);
+                    if (imageRecord) {
+                        this._setTileLoaded(tile, imageRecord.getData());
+                    }
+                }
             }
-        } else if (tile.loading) {
-            // the tile is already in the download queue
-            tiledImage._tilesLoading++;
-        } else if (!loadingCoverage) {
-            best = compareTiles(best, tile);
-        }
-
-        return best;
-    }
 
-    /**
-     * @private
-     * @inner
-     * Obtains a tile at the given location.
-     * @param {Number} x
-     * @param {Number} y
-     * @param {Number} level
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.TileSource} tileSource
-     * @param {Object} tilesMatrix - A '3d' dictionary [level][x][y] --> Tile.
-     * @param {Number} time
-     * @param {Number} numTiles
-     * @param {Number} worldWidth
-     * @param {Number} worldHeight
-     * @returns {OpenSeadragon.Tile}
-     */
-    function getTile(
-        x, y,
-        level,
-        tiledImage,
-        tileSource,
-        tilesMatrix,
-        time,
-        numTiles,
-        worldWidth,
-        worldHeight
-    ) {
-        var xMod,
-            yMod,
-            bounds,
-            sourceBounds,
-            exists,
-            url,
-            ajaxHeaders,
-            context2D,
-            tile;
-
-        if (!tilesMatrix[level]) {
-            tilesMatrix[level] = {};
-        }
-        if (!tilesMatrix[level][x]) {
-            tilesMatrix[level][x] = {};
-        }
-
-        if (!tilesMatrix[level][x][y] || !tilesMatrix[level][x][y].flipped !== !tiledImage.flipped) {
-            xMod = (numTiles.x + (x % numTiles.x)) % numTiles.x;
-            yMod = (numTiles.y + (y % numTiles.y)) % numTiles.y;
-            bounds = tiledImage.getTileBounds(level, x, y);
-            sourceBounds = tileSource.getTileBounds(level, xMod, yMod, true);
-            exists = tileSource.tileExists(level, xMod, yMod);
-            url = tileSource.getTileUrl(level, xMod, yMod);
-
-            // Headers are only applicable if loadTilesWithAjax is set
-            if (tiledImage.loadTilesWithAjax) {
-                ajaxHeaders = tileSource.getTileAjaxHeaders(level, xMod, yMod);
-                // Combine tile AJAX headers with tiled image AJAX headers (if applicable)
-                if ($.isPlainObject(tiledImage.ajaxHeaders)) {
-                    ajaxHeaders = $.extend({}, tiledImage.ajaxHeaders, ajaxHeaders);
-                }
-            } else {
-                ajaxHeaders = null;
-            }
-
-            context2D = tileSource.getContext2D ?
-                tileSource.getContext2D(level, xMod, yMod) : undefined;
-
-            tile = new $.Tile(
-                level,
-                x,
-                y,
+            if (tile.loaded) {
+                var needsDraw = this._blendTile(
+                    tile,
+                    x, y,
+                    level,
+                    levelOpacity,
+                    currentTime
+                );
+
+                if (needsDraw) {
+                    this._needsDraw = true;
+                }
+            } else if (tile.loading) {
+                // the tile is already in the download queue
+                this._tilesLoading++;
+            } else if (!loadingCoverage) {
+                best = this._compareTiles(best, tile);
+            }
+
+            return best;
+        },
+
+        /**
+         * @private
+         * @inner
+         * Obtains a tile at the given location.
+         * @param {Number} x
+         * @param {Number} y
+         * @param {Number} level
+         * @param {Number} time
+         * @param {Number} numTiles
+         * @param {Number} worldWidth
+         * @param {Number} worldHeight
+         * @returns {OpenSeadragon.Tile}
+         */
+        _getTile: function(
+            x, y,
+            level,
+            time,
+            numTiles,
+            worldWidth,
+            worldHeight
+        ) {
+            var xMod,
+                yMod,
                 bounds,
+                sourceBounds,
                 exists,
-                url,
-                context2D,
-                tiledImage.loadTilesWithAjax,
+                urlOrGetter,
+                post,
                 ajaxHeaders,
-                sourceBounds
-            );
+                context2D,
+                tile,
+                tilesMatrix = this.tilesMatrix,
+                tileSource = this.source;
+
+            if (!tilesMatrix[level]) {
+                tilesMatrix[level] = {};
+            }
+            if (!tilesMatrix[level][x]) {
+                tilesMatrix[level][x] = {};
+            }
 
-            if (tiledImage.getFlip()) {
-                if (xMod === 0) {
-                    tile.isRightMost = true;
+            if (!tilesMatrix[level][x][y] || !tilesMatrix[level][x][y].flipped !== !this.flipped) {
+                xMod = (numTiles.x + (x % numTiles.x)) % numTiles.x;
+                yMod = (numTiles.y + (y % numTiles.y)) % numTiles.y;
+                bounds = this.getTileBounds(level, x, y);
+                sourceBounds = tileSource.getTileBounds(level, xMod, yMod, true);
+                exists = tileSource.tileExists(level, xMod, yMod);
+                urlOrGetter = tileSource.getTileUrl(level, xMod, yMod);
+                post = tileSource.getTilePostData(level, xMod, yMod);
+
+                // Headers are only applicable if loadTilesWithAjax is set
+                if (this.loadTilesWithAjax) {
+                    ajaxHeaders = tileSource.getTileAjaxHeaders(level, xMod, yMod);
+                    // Combine tile AJAX headers with tiled image AJAX headers (if applicable)
+                    if ($.isPlainObject(this.ajaxHeaders)) {
+                        ajaxHeaders = $.extend({}, this.ajaxHeaders, ajaxHeaders);
+                    }
+                } else {
+                    ajaxHeaders = null;
                 }
-            } else {
-                if (xMod === numTiles.x - 1) {
-                    tile.isRightMost = true;
+
+                context2D = tileSource.getContext2D ?
+                    tileSource.getContext2D(level, xMod, yMod) : undefined;
+
+                tile = new $.Tile(
+                    level,
+                    x,
+                    y,
+                    bounds,
+                    exists,
+                    urlOrGetter,
+                    context2D,
+                    this.loadTilesWithAjax,
+                    ajaxHeaders,
+                    sourceBounds,
+                    post,
+                    tileSource.getTileHashKey(level, xMod, yMod, urlOrGetter, ajaxHeaders, post)
+                );
+
+                if (this.getFlip()) {
+                    if (xMod === 0) {
+                        tile.isRightMost = true;
+                    }
+                } else {
+                    if (xMod === numTiles.x - 1) {
+                        tile.isRightMost = true;
+                    }
                 }
-            }
 
-            if (yMod === numTiles.y - 1) {
-                tile.isBottomMost = true;
+                if (yMod === numTiles.y - 1) {
+                    tile.isBottomMost = true;
+                }
+
+                tile.flipped = this.flipped;
+
+                tilesMatrix[level][x][y] = tile;
             }
 
-            tile.flipped = tiledImage.flipped;
+            tile = tilesMatrix[level][x][y];
+            tile.lastTouchTime = time;
 
-            tilesMatrix[level][x][y] = tile;
-        }
+            return tile;
+        },
 
-        tile = tilesMatrix[level][x][y];
-        tile.lastTouchTime = time;
+        /**
+         * @private
+         * @inner
+         * Dispatch a job to the ImageLoader to load the Image for a Tile.
+         * @param {OpenSeadragon.Tile} tile
+         * @param {Number} time
+         */
+        _loadTile: function(tile, time) {
+            var _this = this;
+            tile.loading = true;
+            this._imageLoader.addJob({
+                src: tile.getUrl(),
+                tile: tile,
+                source: this.source,
+                postData: tile.postData,
+                loadWithAjax: tile.loadWithAjax,
+                ajaxHeaders: tile.ajaxHeaders,
+                crossOriginPolicy: this.crossOriginPolicy,
+                ajaxWithCredentials: this.ajaxWithCredentials,
+                callback: function(data, errorMsg, tileRequest) {
+                    _this._onTileLoad(tile, time, data, errorMsg, tileRequest);
+                },
+                abort: function() {
+                    tile.loading = false;
+                }
+            });
+        },
 
-        return tile;
-    }
+        /**
+         * @private
+         * @inner
+         * Callback fired when a Tile's Image finished downloading.
+         * @param {OpenSeadragon.Tile} tile
+         * @param {Number} time
+         * @param {*} data image data
+         * @param {String} errorMsg
+         * @param {XMLHttpRequest} tileRequest
+         */
+        _onTileLoad: function(tile, time, data, errorMsg, tileRequest) {
+            if (!data) {
+                $.console.error("Tile %s failed to load: %s - error: %s", tile, tile.getUrl(), errorMsg);
+                /**
+                 * Triggered when a tile fails to load.
+                 *
+                 * @event tile-load-failed
+                 * @memberof OpenSeadragon.Viewer
+                 * @type {object}
+                 * @property {OpenSeadragon.Tile} tile - The tile that failed to load.
+                 * @property {OpenSeadragon.TiledImage} tiledImage - The tiled image the tile belongs to.
+                 * @property {number} time - The time in milliseconds when the tile load began.
+                 * @property {string} message - The error message.
+                 * @property {XMLHttpRequest} tileRequest - The XMLHttpRequest used to load the tile if available.
+                 */
+                this.viewer.raiseEvent("tile-load-failed", {
+                    tile: tile,
+                    tiledImage: this,
+                    time: time,
+                    message: errorMsg,
+                    tileRequest: tileRequest
+                });
+                tile.loading = false;
+                tile.exists = false;
+                return;
+            } else {
+                tile.exists = true;
+            }
 
-    /**
-     * @private
-     * @inner
-     * Dispatch a job to the ImageLoader to load the Image for a Tile.
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile} tile
-     * @param {Number} time
-     */
-    function loadTile(tiledImage, tile, time) {
-        tile.loading = true;
-        tiledImage._imageLoader.addJob({
-            src: tile.url,
-            loadWithAjax: tile.loadWithAjax,
-            ajaxHeaders: tile.ajaxHeaders,
-            crossOriginPolicy: tiledImage.crossOriginPolicy,
-            ajaxWithCredentials: tiledImage.ajaxWithCredentials,
-            callback: function(image, errorMsg, tileRequest) {
-                onTileLoad(tiledImage, tile, time, image, errorMsg, tileRequest);
-            },
-            abort: function() {
+            if (time < this.lastResetTime) {
+                $.console.warn("Ignoring tile %s loaded before reset: %s", tile, tile.getUrl());
                 tile.loading = false;
+                return;
+            }
+
+            var _this = this,
+                finish = function() {
+                    var ccc = _this.source;
+                    var cutoff = ccc.getClosestLevel();
+                    _this._setTileLoaded(tile, data, cutoff, tileRequest);
+                };
+
+            // Check if we're mid-update; this can happen on IE8 because image load events for
+            // cached images happen immediately there
+            if (!this._midDraw) {
+                finish();
+            } else {
+                // Wait until after the update, in case caching unloads any tiles
+                window.setTimeout(finish, 1);
+            }
+        },
+
+        /**
+         * @private
+         * @inner
+         * @param {OpenSeadragon.Tile} tile
+         * @param {*} data image data, the data sent to ImageJob.prototype.finish(), by default an Image object
+         * @param {Number|undefined} cutoff
+         * @param {XMLHttpRequest|undefined} tileRequest
+         */
+        _setTileLoaded: function(tile, data, cutoff, tileRequest) {
+            var increment = 0,
+                eventFinished = false,
+                _this = this;
+
+            function getCompletionCallback() {
+                if (eventFinished) {
+                    $.console.error("Event 'tile-loaded' argument getCompletionCallback must be called synchronously. " +
+                        "Its return value should be called asynchronously.");
+                }
+                increment++;
+                return completionCallback;
+            }
+
+            function completionCallback() {
+                increment--;
+                if (increment === 0) {
+                    tile.loading = false;
+                    tile.loaded = true;
+                    tile.hasTransparency = _this.source.hasTransparency(
+                        tile.context2D, tile.getUrl(), tile.ajaxHeaders, tile.postData
+                    );
+                    if (!tile.context2D) {
+                        _this._tileCache.cacheTile({
+                            data: data,
+                            tile: tile,
+                            cutoff: cutoff,
+                            tiledImage: _this
+                        });
+                    }
+                    _this._needsDraw = true;
+                }
             }
-        });
-    }
 
-    /**
-     * @private
-     * @inner
-     * Callback fired when a Tile's Image finished downloading.
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile} tile
-     * @param {Number} time
-     * @param {Image} image
-     * @param {String} errorMsg
-     * @param {XMLHttpRequest} tileRequest
-     */
-    function onTileLoad(tiledImage, tile, time, image, errorMsg, tileRequest) {
-        if (!image) {
-            $.console.log("Tile %s failed to load: %s - error: %s", tile, tile.url, errorMsg);
             /**
-             * Triggered when a tile fails to load.
+             * Triggered when a tile has just been loaded in memory. That means that the
+             * image has been downloaded and can be modified before being drawn to the canvas.
              *
-             * @event tile-load-failed
+             * @event tile-loaded
              * @memberof OpenSeadragon.Viewer
              * @type {object}
-             * @property {OpenSeadragon.Tile} tile - The tile that failed to load.
-             * @property {OpenSeadragon.TiledImage} tiledImage - The tiled image the tile belongs to.
-             * @property {number} time - The time in milliseconds when the tile load began.
-             * @property {string} message - The error message.
-             * @property {XMLHttpRequest} tileRequest - The XMLHttpRequest used to load the tile if available.
+             * @property {Image|*} image - The image (data) of the tile. Deprecated.
+             * @property {*} data image data, the data sent to ImageJob.prototype.finish(), by default an Image object
+             * @property {OpenSeadragon.TiledImage} tiledImage - The tiled image of the loaded tile.
+             * @property {OpenSeadragon.Tile} tile - The tile which has been loaded.
+             * @property {XMLHttpRequest} tileRequest - The AJAX request that loaded this tile (if applicable).
+             * @property {function} getCompletionCallback - A function giving a callback to call
+             * when the asynchronous processing of the image is done. The image will be
+             * marked as entirely loaded when the callback has been called once for each
+             * call to getCompletionCallback.
              */
-            tiledImage.viewer.raiseEvent("tile-load-failed", {
+
+            var fallbackCompletion = getCompletionCallback();
+            this.viewer.raiseEvent("tile-loaded", {
                 tile: tile,
-                tiledImage: tiledImage,
-                time: time,
-                message: errorMsg,
-                tileRequest: tileRequest
+                tiledImage: this,
+                tileRequest: tileRequest,
+                get image() {
+                    $.console.error("[tile-loaded] event 'image' has been deprecated. Use 'data' property instead.");
+                    return data;
+                },
+                data: data,
+                getCompletionCallback: getCompletionCallback
             });
-            tile.loading = false;
-            tile.exists = false;
-            return;
-        }
+            eventFinished = true;
+            // In case the completion callback is never called, we at least force it once.
+            fallbackCompletion();
+        },
 
-        if (time < tiledImage.lastResetTime) {
-            $.console.log("Ignoring tile %s loaded before reset: %s", tile, tile.url);
-            tile.loading = false;
-            return;
-        }
+        /**
+         * @private
+         * @inner
+         * @param {OpenSeadragon.Tile} tile
+         * @param {Boolean} overlap
+         * @param {OpenSeadragon.Viewport} viewport
+         * @param {OpenSeadragon.Point} viewportCenter
+         * @param {Number} levelVisibility
+         */
+        _positionTile: function(tile, overlap, viewport, viewportCenter, levelVisibility) {
+            var boundsTL = tile.bounds.getTopLeft();
 
-        var finish = function() {
-            var cutoff = tiledImage.source.getClosestLevel();
-            setTileLoaded(tiledImage, tile, image, cutoff, tileRequest);
-        };
+            boundsTL.x *= this._scaleSpring.current.value;
+            boundsTL.y *= this._scaleSpring.current.value;
+            boundsTL.x += this._xSpring.current.value;
+            boundsTL.y += this._ySpring.current.value;
 
-        // Check if we're mid-update; this can happen on IE8 because image load events for
-        // cached images happen immediately there
-        if (!tiledImage._midDraw) {
-            finish();
-        } else {
-            // Wait until after the update, in case caching unloads any tiles
-            window.setTimeout(finish, 1);
-        }
-    }
+            var boundsSize = tile.bounds.getSize();
 
-    /**
-     * @private
-     * @inner
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile} tile
-     * @param {Image} image
-     * @param {Number} cutoff
-     */
-    function setTileLoaded(tiledImage, tile, image, cutoff, tileRequest) {
-        var increment = 0;
+            boundsSize.x *= this._scaleSpring.current.value;
+            boundsSize.y *= this._scaleSpring.current.value;
 
-        function getCompletionCallback() {
-            increment++;
-            return completionCallback;
-        }
+            var positionC = viewport.pixelFromPointNoRotate(boundsTL, true),
+                positionT = viewport.pixelFromPointNoRotate(boundsTL, false),
+                sizeC = viewport.deltaPixelsFromPointsNoRotate(boundsSize, true),
+                sizeT = viewport.deltaPixelsFromPointsNoRotate(boundsSize, false),
+                tileCenter = positionT.plus(sizeT.divide(2)),
+                tileSquaredDistance = viewportCenter.squaredDistanceTo(tileCenter);
 
-        function completionCallback() {
-            increment--;
-            if (increment === 0) {
-                tile.loading = false;
-                tile.loaded = true;
-                if (!tile.context2D) {
-                    tiledImage._tileCache.cacheTile({
-                        image: image,
-                        tile: tile,
-                        cutoff: cutoff,
-                        tiledImage: tiledImage
-                    });
-                }
-                tiledImage._needsDraw = true;
+            if (!overlap) {
+                sizeC = sizeC.plus(new $.Point(1, 1));
             }
-        }
 
-        /**
-         * Triggered when a tile has just been loaded in memory. That means that the
-         * image has been downloaded and can be modified before being drawn to the canvas.
-         *
-         * @event tile-loaded
-         * @memberof OpenSeadragon.Viewer
-         * @type {object}
-         * @property {Image} image - The image of the tile.
-         * @property {OpenSeadragon.TiledImage} tiledImage - The tiled image of the loaded tile.
-         * @property {OpenSeadragon.Tile} tile - The tile which has been loaded.
-         * @property {XMLHttpRequest} tileRequest - The AJAX request that loaded this tile (if applicable).
-         * @property {function} getCompletionCallback - A function giving a callback to call
-         * when the asynchronous processing of the image is done. The image will be
-         * marked as entirely loaded when the callback has been called once for each
-         * call to getCompletionCallback.
-         */
-        tiledImage.viewer.raiseEvent("tile-loaded", {
-            tile: tile,
-            tiledImage: tiledImage,
-            tileRequest: tileRequest,
-            image: image,
-            getCompletionCallback: getCompletionCallback
-        });
-        // In case the completion callback is never called, we at least force it once.
-        getCompletionCallback()();
-    }
-
-    /**
-     * @private
-     * @inner
-     * @param {OpenSeadragon.Tile} tile
-     * @param {Boolean} overlap
-     * @param {OpenSeadragon.Viewport} viewport
-     * @param {OpenSeadragon.Point} viewportCenter
-     * @param {Number} levelVisibility
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     */
-    function positionTile(tile, overlap, viewport, viewportCenter, levelVisibility, tiledImage) {
-        var boundsTL = tile.bounds.getTopLeft();
-
-        boundsTL.x *= tiledImage._scaleSpring.current.value;
-        boundsTL.y *= tiledImage._scaleSpring.current.value;
-        boundsTL.x += tiledImage._xSpring.current.value;
-        boundsTL.y += tiledImage._ySpring.current.value;
-
-        var boundsSize = tile.bounds.getSize();
+            if (tile.isRightMost && this.wrapHorizontal) {
+                sizeC.x += 0.75; // Otherwise Firefox and Safari show seams
+            }
 
-        boundsSize.x *= tiledImage._scaleSpring.current.value;
-        boundsSize.y *= tiledImage._scaleSpring.current.value;
+            if (tile.isBottomMost && this.wrapVertical) {
+                sizeC.y += 0.75; // Otherwise Firefox and Safari show seams
+            }
 
-        var positionC = viewport.pixelFromPointNoRotate(boundsTL, true),
-            positionT = viewport.pixelFromPointNoRotate(boundsTL, false),
-            sizeC = viewport.deltaPixelsFromPointsNoRotate(boundsSize, true),
-            sizeT = viewport.deltaPixelsFromPointsNoRotate(boundsSize, false),
-            tileCenter = positionT.plus(sizeT.divide(2)),
-            tileSquaredDistance = viewportCenter.squaredDistanceTo(tileCenter);
+            tile.position = positionC;
+            tile.size = sizeC;
+            tile.squaredDistance = tileSquaredDistance;
+            tile.visibility = levelVisibility;
+        },
 
-        if (!overlap) {
-            sizeC = sizeC.plus(new $.Point(1, 1));
-        }
+        /**
+         * @private
+         * @inner
+         * Updates the opacity of a tile according to the time it has been on screen
+         * to perform a fade-in.
+         * Updates coverage once a tile is fully opaque.
+         * Returns whether the fade-in has completed.
+         *
+         * @param {OpenSeadragon.Tile} tile
+         * @param {Number} x
+         * @param {Number} y
+         * @param {Number} level
+         * @param {Number} levelOpacity
+         * @param {Number} currentTime
+         * @returns {Boolean}
+         */
+        _blendTile: function(tile, x, y, level, levelOpacity, currentTime) {
+            var blendTimeMillis = 1000 * this.blendTime,
+                deltaTime,
+                opacity;
 
-        if (tile.isRightMost && tiledImage.wrapHorizontal) {
-            sizeC.x += 0.75; // Otherwise Firefox and Safari show seams
-        }
+            if (!tile.blendStart) {
+                tile.blendStart = currentTime;
+            }
 
-        if (tile.isBottomMost && tiledImage.wrapVertical) {
-            sizeC.y += 0.75; // Otherwise Firefox and Safari show seams
-        }
+            deltaTime = currentTime - tile.blendStart;
+            opacity = blendTimeMillis ? Math.min(1, deltaTime / (blendTimeMillis)) : 1;
 
-        tile.position = positionC;
-        tile.size = sizeC;
-        tile.squaredDistance = tileSquaredDistance;
-        tile.visibility = levelVisibility;
-    }
+            if (this.alwaysBlend) {
+                opacity *= levelOpacity;
+            }
 
-    /**
-     * @private
-     * @inner
-     * Updates the opacity of a tile according to the time it has been on screen
-     * to perform a fade-in.
-     * Updates coverage once a tile is fully opaque.
-     * Returns whether the fade-in has completed.
-     *
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile} tile
-     * @param {Number} x
-     * @param {Number} y
-     * @param {Number} level
-     * @param {Number} levelOpacity
-     * @param {Number} currentTime
-     * @returns {Boolean}
-     */
-    function blendTile(tiledImage, tile, x, y, level, levelOpacity, currentTime) {
-        var blendTimeMillis = 1000 * tiledImage.blendTime,
-            deltaTime,
-            opacity;
+            tile.opacity = opacity;
 
-        if (!tile.blendStart) {
-            tile.blendStart = currentTime;
-        }
+            this.lastDrawn.push(tile);
 
-        deltaTime = currentTime - tile.blendStart;
-        opacity = blendTimeMillis ? Math.min(1, deltaTime / (blendTimeMillis)) : 1;
+            if (opacity === 1) {
+                this._setCoverage(this.coverage, level, x, y, true);
+                this._hasOpaqueTile = true;
+            } else if (deltaTime < blendTimeMillis) {
+                return true;
+            }
 
-        if (tiledImage.alwaysBlend) {
-            opacity *= levelOpacity;
-        }
+            return false;
+        },
 
-        tile.opacity = opacity;
 
-        tiledImage.lastDrawn.push(tile);
+        /**
+         * @private
+         * @inner
+         * Determines whether the 'last best' tile for the area is better than the
+         * tile in question.
+         *
+         * @param {OpenSeadragon.Tile} previousBest
+         * @param {OpenSeadragon.Tile} tile
+         * @returns {OpenSeadragon.Tile} The new best tile.
+         */
+        _compareTiles: function(previousBest, tile) {
+            if (!previousBest) {
+                return tile;
+            }
 
-        if (opacity === 1) {
-            setCoverage(tiledImage.coverage, level, x, y, true);
-            tiledImage._hasOpaqueTile = true;
-        } else if (deltaTime < blendTimeMillis) {
-            return true;
-        }
+            if (tile.visibility > previousBest.visibility) {
+                return tile;
+            } else if (tile.visibility === previousBest.visibility) {
+                if (tile.squaredDistance < previousBest.squaredDistance) {
+                    return tile;
+                }
+            }
+            return previousBest;
+        },
 
-        return false;
-    }
+        /**
+         * @private
+         * @inner
+         * Draws a TiledImage.
+         * @param {OpenSeadragon.Tile[]} lastDrawn - An unordered list of Tiles drawn last frame.
+         */
+        _drawTiles: function(lastDrawn) {
+            if (this.opacity === 0 || (lastDrawn.length === 0 && !this.placeholderFillStyle)) {
+                return;
+            }
 
-    /**
-     * @private
-     * @inner
-     * Returns true if the given tile provides coverage to lower-level tiles of
-     * lower resolution representing the same content. If neither x nor y is
-     * given, returns true if the entire visible level provides coverage.
-     *
-     * Note that out-of-bounds tiles provide coverage in this sense, since
-     * there's no content that they would need to cover. Tiles at non-existent
-     * levels that are within the image bounds, however, do not.
-     *
-     * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
-     * @param {Number} level - The resolution level of the tile.
-     * @param {Number} x - The X position of the tile.
-     * @param {Number} y - The Y position of the tile.
-     * @returns {Boolean}
-     */
-    function providesCoverage(coverage, level, x, y) {
-        var rows,
-            cols,
-            i, j;
+            var tile = lastDrawn[0];
+            var useSketch;
 
-        if (!coverage[level]) {
-            return false;
-        }
+            if (tile) {
+                useSketch = this.opacity < 1 ||
+                    (this.compositeOperation && this.compositeOperation !== 'source-over') ||
+                    (!this._isBottomItem() &&
+                        this.source.hasTransparency(tile.context2D, tile.getUrl(), tile.ajaxHeaders, tile.postData));
+            }
+
+            var sketchScale;
+            var sketchTranslate;
+
+            var zoom = this.viewport.getZoom(true);
+            var imageZoom = this.viewportToImageZoom(zoom);
+
+            if (lastDrawn.length > 1 &&
+                imageZoom > this.smoothTileEdgesMinZoom &&
+                !this.iOSDevice &&
+                this.getRotation(true) % 360 === 0 && // TODO: support tile edge smoothing with tiled image rotation.
+                $.supportsCanvas && this.viewer.useCanvas) {
+                // When zoomed in a lot (>100%) the tile edges are visible.
+                // So we have to composite them at ~100% and scale them up together.
+                // Note: Disabled on iOS devices per default as it causes a native crash
+                useSketch = true;
+                sketchScale = tile.getScaleForEdgeSmoothing();
+                sketchTranslate = tile.getTranslationForEdgeSmoothing(sketchScale,
+                    this._drawer.getCanvasSize(false),
+                    this._drawer.getCanvasSize(true));
+            }
 
-        if (x === undefined || y === undefined) {
-            rows = coverage[level];
-            for (i in rows) {
-                if (Object.prototype.hasOwnProperty.call(rows, i)) {
-                    cols = rows[i];
-                    for (j in cols) {
-                        if (Object.prototype.hasOwnProperty.call(cols, j) && !cols[j]) {
-                            return false;
+            var bounds;
+            if (useSketch) {
+                if (!sketchScale) {
+                    // Except when edge smoothing, we only clean the part of the
+                    // sketch canvas we are going to use for performance reasons.
+                    bounds = this.viewport.viewportToViewerElementRectangle(
+                            this.getClippedBounds(true))
+                        .getIntegerBoundingBox();
+
+                    if (this._drawer.viewer.viewport.getFlip()) {
+                        if (this.viewport.getRotation(true) % 360 !== 0 ||
+                            this.getRotation(true) % 360 !== 0) {
+                            bounds.x = this._drawer.viewer.container.clientWidth - (bounds.x + bounds.width);
                         }
                     }
+
+                    bounds = bounds.times($.pixelDensityRatio);
                 }
+                this._drawer._clear(true, bounds);
             }
 
-            return true;
-        }
+            // When scaling, we must rotate only when blending the sketch canvas to
+            // avoid interpolation
+            if (!sketchScale) {
+                if (this.viewport.getRotation(true) % 360 !== 0) {
+                    this._drawer._offsetForRotation({
+                        degrees: this.viewport.getRotation(true),
+                        useSketch: useSketch
+                    });
+                }
+                if (this.getRotation(true) % 360 !== 0) {
+                    this._drawer._offsetForRotation({
+                        degrees: this.getRotation(true),
+                        point: this.viewport.pixelFromPointNoRotate(
+                            this._getRotationPoint(true), true),
+                        useSketch: useSketch
+                    });
+                }
 
-        return (
-            coverage[level][x] === undefined ||
-            coverage[level][x][y] === undefined ||
-            coverage[level][x][y] === true
-        );
-    }
+                if (this.viewport.getRotation(true) % 360 === 0 &&
+                    this.getRotation(true) % 360 === 0) {
+                    if (this._drawer.viewer.viewport.getFlip()) {
+                        this._drawer._flip();
+                    }
+                }
+            }
 
-    /**
-     * @private
-     * @inner
-     * Returns true if the given tile is completely covered by higher-level
-     * tiles of higher resolution representing the same content. If neither x
-     * nor y is given, returns true if the entire visible level is covered.
-     *
-     * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
-     * @param {Number} level - The resolution level of the tile.
-     * @param {Number} x - The X position of the tile.
-     * @param {Number} y - The Y position of the tile.
-     * @returns {Boolean}
-     */
-    function isCovered(coverage, level, x, y) {
-        if (x === undefined || y === undefined) {
-            return providesCoverage(coverage, level + 1);
-        } else {
-            return (
-                providesCoverage(coverage, level + 1, 2 * x, 2 * y) &&
-                providesCoverage(coverage, level + 1, 2 * x, 2 * y + 1) &&
-                providesCoverage(coverage, level + 1, 2 * x + 1, 2 * y) &&
-                providesCoverage(coverage, level + 1, 2 * x + 1, 2 * y + 1)
-            );
-        }
-    }
+            var usedClip = false;
+            if (this._clip) {
+                this._drawer.saveContext(useSketch);
 
-    /**
-     * @private
-     * @inner
-     * Sets whether the given tile provides coverage or not.
-     *
-     * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
-     * @param {Number} level - The resolution level of the tile.
-     * @param {Number} x - The X position of the tile.
-     * @param {Number} y - The Y position of the tile.
-     * @param {Boolean} covers - Whether the tile provides coverage.
-     */
-    function setCoverage(coverage, level, x, y, covers) {
-        if (!coverage[level]) {
-            $.console.warn(
-                "Setting coverage for a tile before its level's coverage has been reset: %s",
-                level
-            );
-            return;
-        }
+                var box = this.imageToViewportRectangle(this._clip, true);
+                box = box.rotate(-this.getRotation(true), this._getRotationPoint(true));
+                var clipRect = this._drawer.viewportToDrawerRectangle(box);
+                if (sketchScale) {
+                    clipRect = clipRect.times(sketchScale);
+                }
+                if (sketchTranslate) {
+                    clipRect = clipRect.translate(sketchTranslate);
+                }
+                this._drawer.setClip(clipRect, useSketch);
 
-        if (!coverage[level][x]) {
-            coverage[level][x] = {};
-        }
+                usedClip = true;
+            }
 
-        coverage[level][x][y] = covers;
-    }
+            if (this._croppingPolygons) {
+                var self = this;
+                this._drawer.saveContext(useSketch);
+                try {
+                    var polygons = this._croppingPolygons.map(function(polygon) {
+                        return polygon.map(function(coord) {
+                            var point = self
+                                .imageToViewportCoordinates(coord.x, coord.y, true)
+                                .rotate(-self.getRotation(true), self._getRotationPoint(true));
+                            var clipPoint = self._drawer.viewportCoordToDrawerCoord(point);
+                            if (sketchScale) {
+                                clipPoint = clipPoint.times(sketchScale);
+                            }
+                            if (sketchTranslate) {
+                                clipPoint = clipPoint.plus(sketchTranslate);
+                            }
+                            return clipPoint;
+                        });
+                    });
+                    this._drawer.clipWithPolygons(polygons, useSketch);
+                } catch (e) {
+                    $.console.error(e);
+                }
+                usedClip = true;
+            }
 
-    /**
-     * @private
-     * @inner
-     * Resets coverage information for the given level. This should be called
-     * after every draw routine. Note that at the beginning of the next draw
-     * routine, coverage for every visible tile should be explicitly set.
-     *
-     * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
-     * @param {Number} level - The resolution level of tiles to completely reset.
-     */
-    function resetCoverage(coverage, level) {
-        coverage[level] = {};
-    }
+            if (this.placeholderFillStyle && this._hasOpaqueTile === false) {
+                var placeholderRect = this._drawer.viewportToDrawerRectangle(this.getBounds(true));
+                if (sketchScale) {
+                    placeholderRect = placeholderRect.times(sketchScale);
+                }
+                if (sketchTranslate) {
+                    placeholderRect = placeholderRect.translate(sketchTranslate);
+                }
 
-    /**
-     * @private
-     * @inner
-     * Determines whether the 'last best' tile for the area is better than the
-     * tile in question.
-     *
-     * @param {OpenSeadragon.Tile} previousBest
-     * @param {OpenSeadragon.Tile} tile
-     * @returns {OpenSeadragon.Tile} The new best tile.
-     */
-    function compareTiles(previousBest, tile) {
-        if (!previousBest) {
-            return tile;
-        }
+                var fillStyle = null;
+                if (typeof this.placeholderFillStyle === "function") {
+                    fillStyle = this.placeholderFillStyle(this, this._drawer.context);
+                } else {
+                    fillStyle = this.placeholderFillStyle;
+                }
 
-        if (tile.visibility > previousBest.visibility) {
-            return tile;
-        } else if (tile.visibility === previousBest.visibility) {
-            if (tile.squaredDistance < previousBest.squaredDistance) {
-                return tile;
+                this._drawer.drawRectangle(placeholderRect, fillStyle, useSketch);
             }
-        }
 
-        return previousBest;
-    }
+            var subPixelRoundingRule = determineSubPixelRoundingRule(this.subPixelRoundingForTransparency);
 
-    /**
-     * @private
-     * @inner
-     * Draws a TiledImage.
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile[]} lastDrawn - An unordered list of Tiles drawn last frame.
-     */
-    function drawTiles(tiledImage, lastDrawn) {
-        if (tiledImage.opacity === 0 || (lastDrawn.length === 0 && !tiledImage.placeholderFillStyle)) {
-            return;
-        }
-
-        var tile = lastDrawn[0];
-        var useSketch;
+            var shouldRoundPositionAndSize = false;
 
-        if (tile) {
-            useSketch = tiledImage.opacity < 1 ||
-                (tiledImage.compositeOperation &&
-                    tiledImage.compositeOperation !== 'source-over') ||
-                (!tiledImage._isBottomItem() && tile._hasTransparencyChannel());
-        }
-
-        var sketchScale;
-        var sketchTranslate;
-
-        var zoom = tiledImage.viewport.getZoom(true);
-        var imageZoom = tiledImage.viewportToImageZoom(zoom);
-
-        if (lastDrawn.length > 1 &&
-            imageZoom > tiledImage.smoothTileEdgesMinZoom &&
-            !tiledImage.iOSDevice &&
-            tiledImage.getRotation(true) % 360 === 0 && // TODO: support tile edge smoothing with tiled image rotation.
-            $.supportsCanvas) {
-            // When zoomed in a lot (>100%) the tile edges are visible.
-            // So we have to composite them at ~100% and scale them up together.
-            // Note: Disabled on iOS devices per default as it causes a native crash
-            useSketch = true;
-            sketchScale = tile.getScaleForEdgeSmoothing();
-            sketchTranslate = tile.getTranslationForEdgeSmoothing(sketchScale,
-                tiledImage._drawer.getCanvasSize(false),
-                tiledImage._drawer.getCanvasSize(true));
-        }
+            if (subPixelRoundingRule === $.SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS) {
+                shouldRoundPositionAndSize = true;
+            } else if (subPixelRoundingRule === $.SUBPIXEL_ROUNDING_OCCURRENCES.ONLY_AT_REST) {
+                var isAnimating = this.viewer && this.viewer.isAnimating();
+                shouldRoundPositionAndSize = !isAnimating;
+            }
 
-        var bounds;
-        if (useSketch) {
-            if (!sketchScale) {
-                // Except when edge smoothing, we only clean the part of the
-                // sketch canvas we are going to use for performance reasons.
-                bounds = tiledImage.viewport.viewportToViewerElementRectangle(
-                        tiledImage.getClippedBounds(true))
-                    .getIntegerBoundingBox();
+            for (var i = lastDrawn.length - 1; i >= 0; i--) {
+                tile = lastDrawn[i];
+                this._drawer.drawTile(tile, this._drawingHandler, useSketch, sketchScale,
+                    sketchTranslate, shouldRoundPositionAndSize, this.source);
+                tile.beingDrawn = true;
 
-                if (tiledImage._drawer.viewer.viewport.getFlip()) {
-                    if (tiledImage.viewport.degrees !== 0 || tiledImage.getRotation(true) % 360 !== 0) {
-                        bounds.x = tiledImage._drawer.viewer.container.clientWidth - (bounds.x + bounds.width);
-                    }
+                if (this.viewer) {
+                    /**
+                     * <em>- Needs documentation -</em>
+                     *
+                     * @event tile-drawn
+                     * @memberof OpenSeadragon.Viewer
+                     * @type {object}
+                     * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
+                     * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
+                     * @property {OpenSeadragon.Tile} tile
+                     * @property {?Object} userData - Arbitrary subscriber-defined object.
+                     */
+                    this.viewer.raiseEvent('tile-drawn', {
+                        tiledImage: this,
+                        tile: tile
+                    });
                 }
+            }
 
-                bounds = bounds.times($.pixelDensityRatio);
+            if (usedClip) {
+                this._drawer.restoreContext(useSketch);
             }
-            tiledImage._drawer._clear(true, bounds);
-        }
 
-        // When scaling, we must rotate only when blending the sketch canvas to
-        // avoid interpolation
-        if (!sketchScale) {
-            if (tiledImage.viewport.degrees !== 0) {
-                tiledImage._drawer._offsetForRotation({
-                    degrees: tiledImage.viewport.degrees,
-                    useSketch: useSketch
-                });
+            if (!sketchScale) {
+                if (this.getRotation(true) % 360 !== 0) {
+                    this._drawer._restoreRotationChanges(useSketch);
+                }
+                if (this.viewport.getRotation(true) % 360 !== 0) {
+                    this._drawer._restoreRotationChanges(useSketch);
+                }
             }
-            if (tiledImage.getRotation(true) % 360 !== 0) {
-                tiledImage._drawer._offsetForRotation({
-                    degrees: tiledImage.getRotation(true),
-                    point: tiledImage.viewport.pixelFromPointNoRotate(
-                        tiledImage._getRotationPoint(true), true),
-                    useSketch: useSketch
+
+            if (useSketch) {
+                if (sketchScale) {
+                    if (this.viewport.getRotation(true) % 360 !== 0) {
+                        this._drawer._offsetForRotation({
+                            degrees: this.viewport.getRotation(true),
+                            useSketch: false
+                        });
+                    }
+                    if (this.getRotation(true) % 360 !== 0) {
+                        this._drawer._offsetForRotation({
+                            degrees: this.getRotation(true),
+                            point: this.viewport.pixelFromPointNoRotate(
+                                this._getRotationPoint(true), true),
+                            useSketch: false
+                        });
+                    }
+                }
+                this._drawer.blendSketch({
+                    opacity: this.opacity,
+                    scale: sketchScale,
+                    translate: sketchTranslate,
+                    compositeOperation: this.compositeOperation,
+                    bounds: bounds
                 });
+                if (sketchScale) {
+                    if (this.getRotation(true) % 360 !== 0) {
+                        this._drawer._restoreRotationChanges(false);
+                    }
+                    if (this.viewport.getRotation(true) % 360 !== 0) {
+                        this._drawer._restoreRotationChanges(false);
+                    }
+                }
             }
 
-            if (tiledImage.viewport.degrees === 0 && tiledImage.getRotation(true) % 360 === 0) {
-                if (tiledImage._drawer.viewer.viewport.getFlip()) {
-                    tiledImage._drawer._flip();
+            if (!sketchScale) {
+                if (this.viewport.getRotation(true) % 360 === 0 &&
+                    this.getRotation(true) % 360 === 0) {
+                    if (this._drawer.viewer.viewport.getFlip()) {
+                        this._drawer._flip();
+                    }
                 }
             }
-        }
 
-        var usedClip = false;
-        if (tiledImage._clip) {
-            tiledImage._drawer.saveContext(useSketch);
+            this._drawDebugInfo(lastDrawn);
+        },
 
-            var box = tiledImage.imageToViewportRectangle(tiledImage._clip, true);
-            box = box.rotate(-tiledImage.getRotation(true), tiledImage._getRotationPoint(true));
-            var clipRect = tiledImage._drawer.viewportToDrawerRectangle(box);
-            if (sketchScale) {
-                clipRect = clipRect.times(sketchScale);
-            }
-            if (sketchTranslate) {
-                clipRect = clipRect.translate(sketchTranslate);
+        /**
+         * @private
+         * @inner
+         * Draws special debug information for a TiledImage if in debug mode.
+         * @param {OpenSeadragon.Tile[]} lastDrawn - An unordered list of Tiles drawn last frame.
+         */
+        _drawDebugInfo: function(lastDrawn) {
+            if (this.debugMode) {
+                for (var i = lastDrawn.length - 1; i >= 0; i--) {
+                    var tile = lastDrawn[i];
+                    try {
+                        this._drawer.drawDebugInfo(tile, lastDrawn.length, i, this);
+                    } catch (e) {
+                        $.console.error(e);
+                    }
+                }
             }
-            tiledImage._drawer.setClip(clipRect, useSketch);
+        },
 
-            usedClip = true;
-        }
+        /**
+         * @private
+         * @inner
+         * Returns true if the given tile provides coverage to lower-level tiles of
+         * lower resolution representing the same content. If neither x nor y is
+         * given, returns true if the entire visible level provides coverage.
+         *
+         * Note that out-of-bounds tiles provide coverage in this sense, since
+         * there's no content that they would need to cover. Tiles at non-existent
+         * levels that are within the image bounds, however, do not.
+         *
+         * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
+         * @param {Number} level - The resolution level of the tile.
+         * @param {Number} x - The X position of the tile.
+         * @param {Number} y - The Y position of the tile.
+         * @returns {Boolean}
+         */
+        _providesCoverage: function(coverage, level, x, y) {
+            var rows,
+                cols,
+                i, j;
 
-        if (tiledImage._croppingPolygons) {
-            tiledImage._drawer.saveContext(useSketch);
-            try {
-                var polygons = tiledImage._croppingPolygons.map(function(polygon) {
-                    return polygon.map(function(coord) {
-                        var point = tiledImage
-                            .imageToViewportCoordinates(coord.x, coord.y, true)
-                            .rotate(-tiledImage.getRotation(true), tiledImage._getRotationPoint(true));
-                        var clipPoint = tiledImage._drawer.viewportCoordToDrawerCoord(point);
-                        if (sketchScale) {
-                            clipPoint = clipPoint.times(sketchScale);
-                        }
-                        return clipPoint;
-                    });
-                });
-                tiledImage._drawer.clipWithPolygons(polygons, useSketch);
-            } catch (e) {
-                $.console.error(e);
+            if (!coverage[level]) {
+                return false;
             }
-            usedClip = true;
-        }
 
-        if (tiledImage.placeholderFillStyle && tiledImage._hasOpaqueTile === false) {
-            var placeholderRect = tiledImage._drawer.viewportToDrawerRectangle(tiledImage.getBounds(true));
-            if (sketchScale) {
-                placeholderRect = placeholderRect.times(sketchScale);
+            if (x === undefined || y === undefined) {
+                rows = coverage[level];
+                for (i in rows) {
+                    if (Object.prototype.hasOwnProperty.call(rows, i)) {
+                        cols = rows[i];
+                        for (j in cols) {
+                            if (Object.prototype.hasOwnProperty.call(cols, j) && !cols[j]) {
+                                return false;
+                            }
+                        }
+                    }
+                }
+
+                return true;
             }
-            if (sketchTranslate) {
-                placeholderRect = placeholderRect.translate(sketchTranslate);
+
+            return (
+                coverage[level][x] === undefined ||
+                coverage[level][x][y] === undefined ||
+                coverage[level][x][y] === true
+            );
+        },
+
+        /**
+         * @private
+         * @inner
+         * Returns true if the given tile is completely covered by higher-level
+         * tiles of higher resolution representing the same content. If neither x
+         * nor y is given, returns true if the entire visible level is covered.
+         *
+         * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
+         * @param {Number} level - The resolution level of the tile.
+         * @param {Number} x - The X position of the tile.
+         * @param {Number} y - The Y position of the tile.
+         * @returns {Boolean}
+         */
+        _isCovered: function(coverage, level, x, y) {
+            if (x === undefined || y === undefined) {
+                return this._providesCoverage(coverage, level + 1);
+            } else {
+                return (
+                    this._providesCoverage(coverage, level + 1, 2 * x, 2 * y) &&
+                    this._providesCoverage(coverage, level + 1, 2 * x, 2 * y + 1) &&
+                    this._providesCoverage(coverage, level + 1, 2 * x + 1, 2 * y) &&
+                    this._providesCoverage(coverage, level + 1, 2 * x + 1, 2 * y + 1)
+                );
             }
+        },
 
-            var fillStyle = null;
-            if (typeof tiledImage.placeholderFillStyle === "function") {
-                fillStyle = tiledImage.placeholderFillStyle(tiledImage, tiledImage._drawer.context);
-            } else {
-                fillStyle = tiledImage.placeholderFillStyle;
+        /**
+         * @private
+         * @inner
+         * Sets whether the given tile provides coverage or not.
+         *
+         * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
+         * @param {Number} level - The resolution level of the tile.
+         * @param {Number} x - The X position of the tile.
+         * @param {Number} y - The Y position of the tile.
+         * @param {Boolean} covers - Whether the tile provides coverage.
+         */
+        _setCoverage: function(coverage, level, x, y, covers) {
+            if (!coverage[level]) {
+                $.console.warn(
+                    "Setting coverage for a tile before its level's coverage has been reset: %s",
+                    level
+                );
+                return;
             }
 
-            tiledImage._drawer.drawRectangle(placeholderRect, fillStyle, useSketch);
-        }
+            if (!coverage[level][x]) {
+                coverage[level][x] = {};
+            }
 
-        for (var i = lastDrawn.length - 1; i >= 0; i--) {
-            tile = lastDrawn[i];
-            tiledImage._drawer.drawTile(tile, tiledImage._drawingHandler, useSketch, sketchScale, sketchTranslate);
-            tile.beingDrawn = true;
+            coverage[level][x][y] = covers;
+        },
 
-            if (tiledImage.viewer) {
-                /**
-                 * <em>- Needs documentation -</em>
-                 *
-                 * @event tile-drawn
-                 * @memberof OpenSeadragon.Viewer
-                 * @type {object}
-                 * @property {OpenSeadragon.Viewer} eventSource - A reference to the Viewer which raised the event.
-                 * @property {OpenSeadragon.TiledImage} tiledImage - Which TiledImage is being drawn.
-                 * @property {OpenSeadragon.Tile} tile
-                 * @property {?Object} userData - Arbitrary subscriber-defined object.
-                 */
-                tiledImage.viewer.raiseEvent('tile-drawn', {
-                    tiledImage: tiledImage,
-                    tile: tile
-                });
-            }
+        /**
+         * @private
+         * @inner
+         * Resets coverage information for the given level. This should be called
+         * after every draw routine. Note that at the beginning of the next draw
+         * routine, coverage for every visible tile should be explicitly set.
+         *
+         * @param {Object} coverage - A '3d' dictionary [level][x][y] --> Boolean.
+         * @param {Number} level - The resolution level of tiles to completely reset.
+         */
+        _resetCoverage: function(coverage, level) {
+            coverage[level] = {};
         }
+    });
 
-        if (usedClip) {
-            tiledImage._drawer.restoreContext(useSketch);
-        }
 
-        if (!sketchScale) {
-            if (tiledImage.getRotation(true) % 360 !== 0) {
-                tiledImage._drawer._restoreRotationChanges(useSketch);
-            }
-            if (tiledImage.viewport.degrees !== 0) {
-                tiledImage._drawer._restoreRotationChanges(useSketch);
-            }
-        }
+    /**
+     * @private
+     * @inner
+     * Defines the value for subpixel rounding to fallback to in case of missing or
+     * invalid value.
+     */
+    var DEFAULT_SUBPIXEL_ROUNDING_RULE = $.SUBPIXEL_ROUNDING_OCCURRENCES.NEVER;
 
-        if (useSketch) {
-            if (sketchScale) {
-                if (tiledImage.viewport.degrees !== 0) {
-                    tiledImage._drawer._offsetForRotation({
-                        degrees: tiledImage.viewport.degrees,
-                        useSketch: false
-                    });
-                }
-                if (tiledImage.getRotation(true) % 360 !== 0) {
-                    tiledImage._drawer._offsetForRotation({
-                        degrees: tiledImage.getRotation(true),
-                        point: tiledImage.viewport.pixelFromPointNoRotate(
-                            tiledImage._getRotationPoint(true), true),
-                        useSketch: false
-                    });
-                }
-            }
-            tiledImage._drawer.blendSketch({
-                opacity: tiledImage.opacity,
-                scale: sketchScale,
-                translate: sketchTranslate,
-                compositeOperation: tiledImage.compositeOperation,
-                bounds: bounds
-            });
-            if (sketchScale) {
-                if (tiledImage.getRotation(true) % 360 !== 0) {
-                    tiledImage._drawer._restoreRotationChanges(false);
-                }
-                if (tiledImage.viewport.degrees !== 0) {
-                    tiledImage._drawer._restoreRotationChanges(false);
-                }
-            }
-        }
+    /**
+     * @private
+     * @inner
+     * Checks whether the input value is an invalid subpixel rounding enum value.
+     *
+     * @param {SUBPIXEL_ROUNDING_OCCURRENCES} value - The subpixel rounding enum value to check.
+     * @returns {Boolean} Returns true if the input value is none of the expected
+     * {@link SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS}, {@link SUBPIXEL_ROUNDING_OCCURRENCES.ONLY_AT_REST} or {@link SUBPIXEL_ROUNDING_OCCURRENCES.NEVER} value.
+     */
+    function isSubPixelRoundingRuleUnknown(value) {
+        return value !== $.SUBPIXEL_ROUNDING_OCCURRENCES.ALWAYS &&
+            value !== $.SUBPIXEL_ROUNDING_OCCURRENCES.ONLY_AT_REST &&
+            value !== $.SUBPIXEL_ROUNDING_OCCURRENCES.NEVER;
+    }
 
-        if (!sketchScale) {
-            if (tiledImage.viewport.degrees === 0 && tiledImage.getRotation(true) % 360 === 0) {
-                if (tiledImage._drawer.viewer.viewport.getFlip()) {
-                    tiledImage._drawer._flip();
-                }
-            }
+    /**
+     * @private
+     * @inner
+     * Ensures the returned value is always a valid subpixel rounding enum value,
+     * defaulting to {@link SUBPIXEL_ROUNDING_OCCURRENCES.NEVER} if input is missing or invalid.
+     *
+     * @param {SUBPIXEL_ROUNDING_OCCURRENCES} value - The subpixel rounding enum value to normalize.
+     * @returns {SUBPIXEL_ROUNDING_OCCURRENCES} Returns a valid subpixel rounding enum value.
+     */
+    function normalizeSubPixelRoundingRule(value) {
+        if (isSubPixelRoundingRuleUnknown(value)) {
+            return DEFAULT_SUBPIXEL_ROUNDING_RULE;
         }
-
-        drawDebugInfo(tiledImage, lastDrawn);
+        return value;
     }
 
     /**
      * @private
      * @inner
-     * Draws special debug information for a TiledImage if in debug mode.
-     * @param {OpenSeadragon.TiledImage} tiledImage
-     * @param {OpenSeadragon.Tile[]} lastDrawn - An unordered list of Tiles drawn last frame.
+     * Ensures the returned value is always a valid subpixel rounding enum value,
+     * defaulting to 'NEVER' if input is missing or invalid.
+     *
+     * @param {Object} subPixelRoundingRules - A subpixel rounding enum values dictionary [{@link BROWSERS}] --> {@link SUBPIXEL_ROUNDING_OCCURRENCES}.
+     * @returns {SUBPIXEL_ROUNDING_OCCURRENCES} Returns the determined subpixel rounding enum value for the
+     * current browser.
      */
-    function drawDebugInfo(tiledImage, lastDrawn) {
-        if (tiledImage.debugMode) {
-            for (var i = lastDrawn.length - 1; i >= 0; i--) {
-                var tile = lastDrawn[i];
-                try {
-                    tiledImage._drawer.drawDebugInfo(
-                        tile, lastDrawn.length, i, tiledImage);
-                } catch (e) {
-                    $.console.error(e);
-                }
-            }
+    function determineSubPixelRoundingRule(subPixelRoundingRules) {
+        if (typeof subPixelRoundingRules === 'number') {
+            return normalizeSubPixelRoundingRule(subPixelRoundingRules);
         }
+
+        if (!subPixelRoundingRules || !$.Browser) {
+            return DEFAULT_SUBPIXEL_ROUNDING_RULE;
+        }
+
+        var subPixelRoundingRule = subPixelRoundingRules[$.Browser.vendor];
+
+        if (isSubPixelRoundingRuleUnknown(subPixelRoundingRule)) {
+            subPixelRoundingRule = subPixelRoundingRules['*'];
+        }
+
+        return normalizeSubPixelRoundingRule(subPixelRoundingRule);
     }
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - TileCache
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
@@ -23101,51 +24335,30 @@
         this.tile = options.tile;
         this.tiledImage = options.tiledImage;
     };
 
     // private class
     var ImageRecord = function(options) {
         $.console.assert(options, "[ImageRecord] options is required");
-        $.console.assert(options.image, "[ImageRecord] options.image is required");
-        this._image = options.image;
+        $.console.assert(options.data, "[ImageRecord] options.data is required");
         this._tiles = [];
+
+        options.create.apply(null, [this, options.data, options.ownerTile]);
+        this._destroyImplementation = options.destroy.bind(null, this);
+        this.getImage = options.getImage.bind(null, this);
+        this.getData = options.getData.bind(null, this);
+        this.getRenderedContext = options.getRenderedContext.bind(null, this);
     };
 
     ImageRecord.prototype = {
         destroy: function() {
-            this._image = null;
-            this._renderedContext = null;
+            this._destroyImplementation();
             this._tiles = null;
         },
 
-        getImage: function() {
-            return this._image;
-        },
-
-        getRenderedContext: function() {
-            if (!this._renderedContext) {
-                var canvas = document.createElement('canvas');
-                canvas.width = this._image.width;
-                canvas.height = this._image.height;
-                this._renderedContext = canvas.getContext('2d');
-                this._renderedContext.drawImage(this._image, 0, 0);
-                //since we are caching the prerendered image on a canvas
-                //allow the image to not be held in memory
-                this._image = null;
-            }
-            return this._renderedContext;
-        },
-
-        setRenderedContext: function(renderedContext) {
-            $.console.error("ImageRecord.setRenderedContext is deprecated. " +
-                "The rendered context should be created by the ImageRecord " +
-                "itself when calling ImageRecord.getRenderedContext.");
-            this._renderedContext = renderedContext;
-        },
-
         addTile: function(tile) {
             $.console.assert(tile, '[ImageRecord.addTile] tile is required');
             this._tiles.push(tile);
         },
 
         removeTile: function(tile) {
             for (var i = 0; i < this._tiles.length; i++) {
@@ -23213,17 +24426,30 @@
             $.console.assert(options.tiledImage, "[TileCache.cacheTile] options.tiledImage is required");
 
             var cutoff = options.cutoff || 0;
             var insertionIndex = this._tilesLoaded.length;
 
             var imageRecord = this._imagesLoaded[options.tile.cacheKey];
             if (!imageRecord) {
-                $.console.assert(options.image, "[TileCache.cacheTile] options.image is required to create an ImageRecord");
+
+                if (!options.data) {
+                    $.console.error("[TileCache.cacheTile] options.image was renamed to options.data. '.image' attribute " +
+                        "has been deprecated and will be removed in the future.");
+                    options.data = options.image;
+                }
+
+                $.console.assert(options.data, "[TileCache.cacheTile] options.data is required to create an ImageRecord");
                 imageRecord = this._imagesLoaded[options.tile.cacheKey] = new ImageRecord({
-                    image: options.image
+                    data: options.data,
+                    ownerTile: options.tile,
+                    create: options.tiledImage.source.createTileCache,
+                    destroy: options.tiledImage.source.destroyTileCache,
+                    getImage: options.tiledImage.source.getTileCacheDataAsImage,
+                    getData: options.tiledImage.source.getTileCacheData,
+                    getRenderedContext: options.tiledImage.source.getTileCacheDataAsContext2D,
                 });
 
                 this._imagesLoadedCount++;
             }
 
             imageRecord.addTile(options.tile);
             options.tile.cacheImageRecord = imageRecord;
@@ -23332,15 +24558,15 @@
 
 }(OpenSeadragon));
 
 /*
  * OpenSeadragon - World
  *
  * Copyright (C) 2009 CodePlex Foundation
- * Copyright (C) 2010-2013 OpenSeadragon contributors
+ * Copyright (C) 2010-2022 OpenSeadragon contributors
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are
  * met:
  *
  * - Redistributions of source code must retain the above copyright notice,
  *   this list of conditions and the following disclaimer.
```

### Comparing `openslide-python-1.2.0/examples/deepzoom/templates/files.html` & `openslide-python-1.3.0/examples/deepzoom/templates/files.html`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/templates/slide-fullpage.html` & `openslide-python-1.3.0/examples/deepzoom/templates/slide-fullpage.html`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/examples/deepzoom/templates/slide-multipane.html` & `openslide-python-1.3.0/examples/deepzoom/templates/slide-multipane.html`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/lgpl-2.1.txt` & `openslide-python-1.3.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/openslide/__init__.py` & `openslide-python-1.3.0/openslide/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # openslide-python - Python bindings for the OpenSlide library
 #
 # Copyright (c) 2010-2014 Carnegie Mellon University
-# Copyright (c) 2021      Benjamin Gilbert
+# Copyright (c) 2021-2023 Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -20,16 +20,17 @@
 
 """A library for reading whole-slide images.
 
 This package provides Python bindings for the OpenSlide library.
 """
 
 from collections.abc import Mapping
+from io import BytesIO
 
-from PIL import Image
+from PIL import Image, ImageCms
 
 from openslide import lowlevel
 
 # For the benefit of library users
 from openslide._version import __version__  # noqa: F401  module-imported-but-unused
 from openslide.lowlevel import (  # noqa: F401  module-imported-but-unused
     OpenSlideError,
@@ -51,14 +52,17 @@
 PROPERTY_NAME_BOUNDS_WIDTH = 'openslide.bounds-width'
 PROPERTY_NAME_BOUNDS_HEIGHT = 'openslide.bounds-height'
 
 
 class AbstractSlide:
     """The base class of a slide object."""
 
+    def __init__(self):
+        self._profile = None
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
         return False
 
@@ -107,14 +111,21 @@
     @property
     def associated_images(self):
         """Images associated with this whole-slide image.
 
         This is a map: image name -> PIL.Image."""
         raise NotImplementedError
 
+    @property
+    def color_profile(self):
+        """Color profile for the whole-slide image, or None if unavailable."""
+        if self._profile is None:
+            return None
+        return ImageCms.getOpenProfile(BytesIO(self._profile))
+
     def get_best_level_for_downsample(self, downsample):
         """Return the best level for displaying the given downsample."""
         raise NotImplementedError
 
     def read_region(self, location, level, size):
         """Return a PIL.Image containing the contents of the region.
 
@@ -140,14 +151,16 @@
         # Apply on solid background
         bg_color = '#' + self.properties.get(PROPERTY_NAME_BACKGROUND_COLOR, 'ffffff')
         thumb = Image.new('RGB', tile.size, bg_color)
         thumb.paste(tile, None, tile)
         # Image.Resampling added in Pillow 9.1.0
         # Image.LANCZOS removed in Pillow 10
         thumb.thumbnail(size, getattr(Image, 'Resampling', Image).LANCZOS)
+        if self._profile is not None:
+            thumb.info['icc_profile'] = self._profile
         return thumb
 
 
 class OpenSlide(AbstractSlide):
     """An open whole-slide image.
 
     close() is called automatically when the object is deleted.
@@ -160,14 +173,16 @@
     """
 
     def __init__(self, filename):
         """Open a whole-slide image."""
         AbstractSlide.__init__(self)
         self._filename = filename
         self._osr = lowlevel.open(str(filename))
+        if lowlevel.read_icc_profile.available:
+            self._profile = lowlevel.read_icc_profile(self._osr)
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self._filename!r})'
 
     @classmethod
     def detect_format(cls, filename):
         """Return a string describing the format vendor of the specified file.
@@ -213,15 +228,15 @@
     def associated_images(self):
         """Images associated with this whole-slide image.
 
         This is a map: image name -> PIL.Image.
 
         Unlike in the C interface, the images accessible via this property
         are not premultiplied."""
-        return _AssociatedImageMap(self._osr)
+        return _AssociatedImageMap(self._osr, self._profile)
 
     def get_best_level_for_downsample(self, downsample):
         """Return the best level for displaying the given downsample."""
         return lowlevel.get_best_level_for_downsample(self._osr, downsample)
 
     def read_region(self, location, level, size):
         """Return a PIL.Image containing the contents of the region.
@@ -229,17 +244,20 @@
         location: (x, y) tuple giving the top left pixel in the level 0
                   reference frame.
         level:    the level number.
         size:     (width, height) tuple giving the region size.
 
         Unlike in the C interface, the image data returned by this
         function is not premultiplied."""
-        return lowlevel.read_region(
+        region = lowlevel.read_region(
             self._osr, location[0], location[1], level, size[0], size[1]
         )
+        if self._profile is not None:
+            region.info['icc_profile'] = self._profile
+        return region
 
     def set_cache(self, cache):
         """Use the specified cache to store recently decoded slide tiles.
 
         By default, the object has a private cache with a default size.
 
         cache: an OpenSlideCache object."""
@@ -276,21 +294,33 @@
         v = lowlevel.get_property_value(self._osr, key)
         if v is None:
             raise KeyError()
         return v
 
 
 class _AssociatedImageMap(_OpenSlideMap):
+    def __init__(self, osr, profile):
+        _OpenSlideMap.__init__(self, osr)
+        self._profile = profile
+
     def _keys(self):
         return lowlevel.get_associated_image_names(self._osr)
 
     def __getitem__(self, key):
         if key not in self._keys():
             raise KeyError()
-        return lowlevel.read_associated_image(self._osr, key)
+        image = lowlevel.read_associated_image(self._osr, key)
+        if lowlevel.read_associated_image_icc_profile.available:
+            profile = lowlevel.read_associated_image_icc_profile(self._osr, key)
+            if profile == self._profile:
+                # reuse profile copy from main image to save memory
+                profile = self._profile
+            if profile is not None:
+                image.info['icc_profile'] = profile
+        return image
 
 
 class OpenSlideCache:
     """An in-memory tile cache.
 
     Tile caches can be attached to one or more OpenSlide objects with
     OpenSlide.set_cache() to cache recently-decoded tiles.  By default,
@@ -317,14 +347,15 @@
         self._file_arg = file
         if isinstance(file, Image.Image):
             self._close = False
             self._image = file
         else:
             self._close = True
             self._image = Image.open(file)
+        self._profile = self._image.info.get('icc_profile')
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self._file_arg!r})'
 
     @classmethod
     def detect_format(cls, filename):
         """Return a string describing the format of the specified file.
@@ -406,14 +437,16 @@
             'fail' for tl, br in zip(image_topleft, image_bottomright) if br - tl < 0
         ]:  # "< 0" not a typo
             # Crop size is greater than zero in both dimensions.
             # PIL thinks the bottom right is the first *excluded* pixel
             crop = self._image.crop(image_topleft + [d + 1 for d in image_bottomright])
             tile_offset = tuple(il - l for il, l in zip(image_topleft, location))
             tile.paste(crop, tile_offset)
+        if self._profile is not None:
+            tile.info['icc_profile'] = self._profile
         return tile
 
     def set_cache(self, cache):
         """Use the specified cache to store recently decoded slide tiles.
 
         ImageSlide does not support caching, so this method does nothing.
```

### Comparing `openslide-python-1.2.0/openslide/_convert.c` & `openslide-python-1.3.0/openslide/_convert.c`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/openslide/_version.py` & `openslide-python-1.3.0/openslide/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #
 
 """The openslide package version.
 
 This module is an implementation detail.  The package version should be
 obtained from openslide.__version__."""
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
```

### Comparing `openslide-python-1.2.0/openslide/deepzoom.py` & `openslide-python-1.3.0/openslide/deepzoom.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,25 +167,30 @@
         level:     the Deep Zoom level.
         address:   the address of the tile within the level as a (col, row)
                    tuple."""
 
         # Read tile
         args, z_size = self._get_tile_info(level, address)
         tile = self._osr.read_region(*args)
+        profile = tile.info.get('icc_profile')
 
         # Apply on solid background
         bg = Image.new('RGB', tile.size, self._bg_color)
         tile = Image.composite(tile, bg, tile)
 
         # Scale to the correct size
         if tile.size != z_size:
             # Image.Resampling added in Pillow 9.1.0
             # Image.LANCZOS removed in Pillow 10
             tile.thumbnail(z_size, getattr(Image, 'Resampling', Image).LANCZOS)
 
+        # Reference ICC profile
+        if profile is not None:
+            tile.info['icc_profile'] = profile
+
         return tile
 
     def _get_tile_info(self, dz_level, t_location):
         # Check parameters
         if dz_level < 0 or dz_level >= self._dz_levels:
             raise ValueError("Invalid level")
         for t, t_lim in zip(t_location, self._t_dimensions[dz_level]):
```

### Comparing `openslide-python-1.2.0/openslide/lowlevel.py` & `openslide-python-1.3.0/openslide/lowlevel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # openslide-python - Python bindings for the OpenSlide library
 #
 # Copyright (c) 2010-2013 Carnegie Mellon University
-# Copyright (c) 2016-2021 Benjamin Gilbert
+# Copyright (c) 2016-2023 Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -29,63 +29,71 @@
 returned by OpenSlide into a non-premultiplied PIL.Image happens here
 rather than in the high-level interface.)
 """
 
 from ctypes import (
     POINTER,
     byref,
+    c_char,
     c_char_p,
     c_double,
     c_int32,
     c_int64,
     c_size_t,
     c_uint32,
     c_void_p,
     cdll,
 )
 from itertools import count
 import platform
 
-import PIL.Image
+from PIL import Image
 
 from . import _convert
 
-if platform.system() == 'Windows':
-    try:
-        _lib = cdll.LoadLibrary('libopenslide-0.dll')
-    except FileNotFoundError:
-        import os
-
-        if hasattr(os, 'add_dll_directory'):
-            # Python >= 3.8
-            _admonition = 'Did you call os.add_dll_directory()?'
-        else:
-            _admonition = 'Did you add OpenSlide to PATH?'
-        raise ModuleNotFoundError(
-            f"Couldn't locate OpenSlide DLL.  {_admonition}  "
-            "https://openslide.org/api/python/#installing"
-        )
-elif platform.system() == 'Darwin':
-    try:
-        _lib = cdll.LoadLibrary('libopenslide.0.dylib')
-    except OSError:
-        # MacPorts doesn't add itself to the dyld search path, but
-        # does add itself to the find_library() search path
-        # (DEFAULT_LIBRARY_FALLBACK in ctypes.macholib.dyld).
-        import ctypes.util
 
-        _lib = ctypes.util.find_library('openslide')
-        if _lib is None:
+def _load_library():
+    def try_load(names):
+        for name in names:
+            try:
+                return cdll.LoadLibrary(name)
+            except OSError:
+                if name == names[-1]:
+                    raise
+
+    if platform.system() == 'Windows':
+        try:
+            return try_load(['libopenslide-1.dll', 'libopenslide-0.dll'])
+        except FileNotFoundError:
             raise ModuleNotFoundError(
-                "Couldn't locate OpenSlide dylib.  Is OpenSlide installed "
-                "correctly?  https://openslide.org/api/python/#installing"
+                "Couldn't locate OpenSlide DLL.  "
+                "Did you call os.add_dll_directory()?  "
+                "https://openslide.org/api/python/#installing"
             )
-        _lib = cdll.LoadLibrary(_lib)
-else:
-    _lib = cdll.LoadLibrary('libopenslide.so.0')
+    elif platform.system() == 'Darwin':
+        try:
+            return try_load(['libopenslide.1.dylib', 'libopenslide.0.dylib'])
+        except OSError:
+            # MacPorts doesn't add itself to the dyld search path, but
+            # does add itself to the find_library() search path
+            # (DEFAULT_LIBRARY_FALLBACK in ctypes.macholib.dyld).
+            import ctypes.util
+
+            lib = ctypes.util.find_library('openslide')
+            if lib is None:
+                raise ModuleNotFoundError(
+                    "Couldn't locate OpenSlide dylib.  Is OpenSlide installed "
+                    "correctly?  https://openslide.org/api/python/#installing"
+                )
+            return cdll.LoadLibrary(lib)
+    else:
+        return try_load(['libopenslide.so.1', 'libopenslide.so.0'])
+
+
+_lib = _load_library()
 
 
 class OpenSlideError(Exception):
     """An error produced by the OpenSlide library.
 
     Import this from openslide rather than from openslide.lowlevel.
     """
@@ -182,15 +190,15 @@
             raise ValueError('Value out of range')
         return c_size_t(obj)
 
 
 def _load_image(buf, size):
     '''buf must be a mutable buffer.'''
     _convert.argb2rgba(buf)
-    return PIL.Image.frombuffer('RGBA', size, buf, 'raw', 'RGBA', 0, 1)
+    return Image.frombuffer('RGBA', size, buf, 'raw', 'RGBA', 0, 1)
 
 
 # check for errors opening an image file and wrap the resulting handle
 def _check_open(result, _func, _args):
     if result is None:
         raise OpenSlideUnsupportedFormatError("Unsupported or missing image file")
     slide = _OpenSlide(c_void_p(result))
@@ -246,22 +254,36 @@
         if minimum_version is None:
             raise
 
         # optional function doesn't exist; fail at runtime
         def function_unavailable(*_args):
             raise OpenSlideVersionError(minimum_version)
 
+        # allow checking for availability without calling the function
+        function_unavailable.available = False
+
         return function_unavailable
     func.argtypes = argtypes
     func.restype = restype
     if errcheck is not None:
         func.errcheck = errcheck
+    func.available = True
     return func
 
 
+def _wraps_funcs(wrapped):
+    def decorator(f):
+        f.available = True
+        for w in wrapped:
+            f.available = f.available and w.available
+        return f
+
+    return decorator
+
+
 try:
     detect_vendor = _func('openslide_detect_vendor', c_char_p, [_utf8_p], _check_string)
 except AttributeError:
     raise OpenSlideVersionError('3.4.0')
 
 open = _func('openslide_open', c_void_p, [_utf8_p], _check_open)
 
@@ -272,14 +294,15 @@
 _get_level_dimensions = _func(
     'openslide_get_level_dimensions',
     None,
     [_OpenSlide, c_int32, POINTER(c_int64), POINTER(c_int64)],
 )
 
 
+@_wraps_funcs([_get_level_dimensions])
 def get_level_dimensions(slide, level):
     w, h = c_int64(), c_int64()
     _get_level_dimensions(slide, level, byref(w), byref(h))
     return w.value, h.value
 
 
 get_level_downsample = _func(
@@ -293,29 +316,55 @@
 _read_region = _func(
     'openslide_read_region',
     None,
     [_OpenSlide, POINTER(c_uint32), c_int64, c_int64, c_int32, c_int64, c_int64],
 )
 
 
+@_wraps_funcs([_read_region])
 def read_region(slide, x, y, level, w, h):
     if w < 0 or h < 0:
         # OpenSlide would catch this, but not before we tried to allocate
         # a negative-size buffer
         raise OpenSlideError(
             "negative width (%d) or negative height (%d) not allowed" % (w, h)
         )
     if w == 0 or h == 0:
-        # PIL.Image.frombuffer() would raise an exception
-        return PIL.Image.new('RGBA', (w, h))
+        # Image.frombuffer() would raise an exception
+        return Image.new('RGBA', (w, h))
     buf = (w * h * c_uint32)()
     _read_region(slide, buf, x, y, level, w, h)
     return _load_image(buf, (w, h))
 
 
+get_icc_profile_size = _func(
+    'openslide_get_icc_profile_size',
+    c_int64,
+    [_OpenSlide],
+    minimum_version='4.0.0',
+)
+
+_read_icc_profile = _func(
+    'openslide_read_icc_profile',
+    None,
+    [_OpenSlide, POINTER(c_char)],
+    minimum_version='4.0.0',
+)
+
+
+@_wraps_funcs([get_icc_profile_size, _read_icc_profile])
+def read_icc_profile(slide):
+    size = get_icc_profile_size(slide)
+    if size == 0:
+        return None
+    buf = (size * c_char)()
+    _read_icc_profile(slide, buf)
+    return buf.raw
+
+
 get_error = _func('openslide_get_error', c_char_p, [_OpenSlide], _check_string)
 
 get_property_names = _func(
     'openslide_get_property_names', POINTER(c_char_p), [_OpenSlide], _check_name_list
 )
 
 get_property_value = _func(
@@ -332,46 +381,75 @@
 _get_associated_image_dimensions = _func(
     'openslide_get_associated_image_dimensions',
     None,
     [_OpenSlide, _utf8_p, POINTER(c_int64), POINTER(c_int64)],
 )
 
 
+@_wraps_funcs([_get_associated_image_dimensions])
 def get_associated_image_dimensions(slide, name):
     w, h = c_int64(), c_int64()
     _get_associated_image_dimensions(slide, name, byref(w), byref(h))
     return w.value, h.value
 
 
 _read_associated_image = _func(
     'openslide_read_associated_image', None, [_OpenSlide, _utf8_p, POINTER(c_uint32)]
 )
 
 
+@_wraps_funcs([get_associated_image_dimensions, _read_associated_image])
 def read_associated_image(slide, name):
     w, h = get_associated_image_dimensions(slide, name)
     buf = (w * h * c_uint32)()
     _read_associated_image(slide, name, buf)
     return _load_image(buf, (w, h))
 
 
+get_associated_image_icc_profile_size = _func(
+    'openslide_get_associated_image_icc_profile_size',
+    c_int64,
+    [_OpenSlide, _utf8_p],
+    minimum_version='4.0.0',
+)
+
+_read_associated_image_icc_profile = _func(
+    'openslide_read_associated_image_icc_profile',
+    None,
+    [_OpenSlide, _utf8_p, POINTER(c_char)],
+    minimum_version='4.0.0',
+)
+
+
+@_wraps_funcs(
+    [get_associated_image_icc_profile_size, _read_associated_image_icc_profile]
+)
+def read_associated_image_icc_profile(slide, name):
+    size = get_associated_image_icc_profile_size(slide, name)
+    if size == 0:
+        return None
+    buf = (size * c_char)()
+    _read_associated_image_icc_profile(slide, name, buf)
+    return buf.raw
+
+
 get_version = _func('openslide_get_version', c_char_p, [], _check_string)
 
 cache_create = _func(
     'openslide_cache_create',
     c_void_p,
     [_size_t],
     _check_cache_create,
-    minimum_version='3.5.0',
+    minimum_version='4.0.0',
 )
 
 set_cache = _func(
     'openslide_set_cache',
     None,
     [_OpenSlide, _OpenSlideCache],
     None,
-    minimum_version='3.5.0',
+    minimum_version='4.0.0',
 )
 
 cache_release = _func(
-    'openslide_cache_release', None, [_OpenSlideCache], None, minimum_version='3.5.0'
+    'openslide_cache_release', None, [_OpenSlideCache], None, minimum_version='4.0.0'
 )
```

### Comparing `openslide-python-1.2.0/openslide_python.egg-info/PKG-INFO` & `openslide-python-1.3.0/openslide_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: openslide-python
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python interface to OpenSlide
 Home-page: https://openslide.org/
 Maintainer: OpenSlide project
 Maintainer-email: openslide-users@lists.andrew.cmu.edu
 License: GNU Lesser General Public License, version 2.1
 Keywords: openslide whole-slide image virtual slide library
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: COPYING.LESSER
 
 # OpenSlide Python
 
 OpenSlide Python is a Python interface to the OpenSlide library.
 
 [OpenSlide] is a C library that provides a simple interface for reading
 whole-slide images, also known as virtual slides, which are high-resolution
@@ -38,39 +37,41 @@
 libraries, which are designed for images that can be comfortably
 uncompressed into RAM.  Whole-slide images are typically multi-resolution;
 OpenSlide allows reading a small amount of image data at the resolution
 closest to a desired zoom level.
 
 OpenSlide can read virtual slides in several formats:
 
-* [Aperio][]: (`.svs`, `.tif`)
-* [Hamamatsu][]: (`.ndpi`, `.vms`, `.vmu`)
-* [Leica][]: (`.scn`)
-* [MIRAX][]: (`.mrxs`)
-* [Philips][]: (`.tiff`)
-* [Sakura][]: (`.svslide`)
-* [Trestle][]: (`.tif`)
-* [Ventana][]: (`.bif`, `.tif`)
-* [Generic tiled TIFF][]: (`.tif`)
+* [Aperio][] (`.svs`, `.tif`)
+* [DICOM][] (`.dcm`)
+* [Hamamatsu][] (`.ndpi`, `.vms`, `.vmu`)
+* [Leica][] (`.scn`)
+* [MIRAX][] (`.mrxs`)
+* [Philips][] (`.tiff`)
+* [Sakura][] (`.svslide`)
+* [Trestle][] (`.tif`)
+* [Ventana][] (`.bif`, `.tif`)
+* [Generic tiled TIFF][] (`.tif`)
 
 [OpenSlide]: https://openslide.org/
 [Aperio]: https://openslide.org/formats/aperio/
+[DICOM]: https://openslide.org/formats/dicom/
 [Hamamatsu]: https://openslide.org/formats/hamamatsu/
 [Leica]: https://openslide.org/formats/leica/
 [MIRAX]: https://openslide.org/formats/mirax/
 [Philips]: https://openslide.org/formats/philips/
 [Sakura]: https://openslide.org/formats/sakura/
 [Trestle]: https://openslide.org/formats/trestle/
 [Ventana]: https://openslide.org/formats/ventana/
 [Generic tiled TIFF]: https://openslide.org/formats/generic-tiff/
 
 
 ## Requirements
 
-* Python &ge; 3.7
+* Python &ge; 3.8
 * OpenSlide &ge; 3.4.0
 * Pillow
 
 
 ## Installation
 
 OpenSlide Python requires [OpenSlide].  For instructions on installing both
@@ -79,19 +80,22 @@
 
 [installing]: https://openslide.org/api/python/#installing
 
 
 ## More Information
 
 - [API documentation](https://openslide.org/api/python/)
-- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md)
+- [Changelog](https://github.com/openslide/openslide-python/blob/main/CHANGELOG.md#notable-changes-in-openslide-python)
 - [Website][OpenSlide]
 - [GitHub](https://github.com/openslide/openslide-python)
-- [Sample data](http://openslide.cs.cmu.edu/download/openslide-testdata/)
+- [Sample data](https://openslide.cs.cmu.edu/download/openslide-testdata/)
 
 
 ## License
 
 OpenSlide Python is released under the terms of the [GNU Lesser General
-Public License, version 2.1](https://raw.github.com/openslide/openslide-python/main/lgpl-2.1.txt).
-
+Public License, version 2.1](https://openslide.org/license/).
 
+OpenSlide Python is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
+License for more details.
```

### Comparing `openslide-python-1.2.0/openslide_python.egg-info/SOURCES.txt` & `openslide-python-1.3.0/openslide_python.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGELOG.md
-LICENSE.txt
+COPYING.LESSER
 MANIFEST.in
 README.md
-lgpl-2.1.txt
+pytest.ini
 setup.py
 doc/conf.py
 doc/index.rst
 doc/jekyll_fix.py
 examples/deepzoom/deepzoom_multiserver.py
 examples/deepzoom/deepzoom_server.py
 examples/deepzoom/deepzoom_tile.py
@@ -55,17 +55,20 @@
 openslide/lowlevel.py
 openslide_python.egg-info/PKG-INFO
 openslide_python.egg-info/SOURCES.txt
 openslide_python.egg-info/dependency_links.txt
 openslide_python.egg-info/requires.txt
 openslide_python.egg-info/top_level.txt
 openslide_python.egg-info/zip-safe
-tests/__init__.py
-tests/boxes.png
-tests/boxes.tiff
-tests/small.svs
+tests/common.py
 tests/test_base.py
 tests/test_deepzoom.py
 tests/test_imageslide.py
 tests/test_openslide.py
-tests/unopenable.tiff
-tests/unreadable.svs
+tests/fixtures/boxes-no-icc.png
+tests/fixtures/boxes.png
+tests/fixtures/boxes.tiff
+tests/fixtures/boxes_0.dcm
+tests/fixtures/boxes_1.dcm
+tests/fixtures/small.svs
+tests/fixtures/unopenable.tiff
+tests/fixtures/unreadable.svs
```

### Comparing `openslide-python-1.2.0/setup.py` & `openslide-python-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,19 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'Pillow',
     ],
     zip_safe=True,
 )
```

### Comparing `openslide-python-1.2.0/tests/__init__.py` & `openslide-python-1.3.0/tests/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,50 +13,24 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
-from functools import wraps
 import os
 from pathlib import Path
 
 # Handle Windows-specific first-import logic here, so individual modules
 # don't have to
 if os.name == 'nt':
     # In application code, you probably shouldn't use an environment
     # variable for this, unless you're sure you can trust the contents of the
     # environment.
     _dll_path = os.getenv('OPENSLIDE_PATH')
     if _dll_path is not None:
-        if hasattr(os, 'add_dll_directory'):
-            # Python >= 3.8
-            with os.add_dll_directory(_dll_path):
-                import openslide
-        else:
-            # Python < 3.8
-            _orig_path = os.environ.get('PATH', '')
-            os.environ['PATH'] = _orig_path + ';' + _dll_path
+        with os.add_dll_directory(_dll_path):
             import openslide  # noqa: F401  module-imported-but-unused
 
-            os.environ['PATH'] = _orig_path
-
-from openslide import OpenSlideVersionError
-
 
 def file_path(name):
-    return Path(__file__).parent / name
-
-
-def maybe_supported(f):
-    '''Decorator to ignore test failures caused by an OpenSlide version that
-    doesn't support the tested functionality.'''
-
-    @wraps(f)
-    def wrapper(*args, **kwargs):
-        try:
-            return f(*args, **kwargs)
-        except OpenSlideVersionError:
-            pass
-
-    return wrapper
+    return Path(__file__).parent / 'fixtures' / name
```

### Comparing `openslide-python-1.2.0/tests/small.svs` & `openslide-python-1.3.0/tests/fixtures/small.svs`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/tests/test_deepzoom.py` & `openslide-python-1.3.0/tests/test_deepzoom.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
 import unittest
 
-from openslide import ImageSlide, OpenSlide
-from openslide.deepzoom import DeepZoomGenerator
+from common import file_path
 
-from . import file_path
+from openslide import ImageSlide, OpenSlide, lowlevel
+from openslide.deepzoom import DeepZoomGenerator
 
 
 class _BoxesDeepZoomTest:
     def setUp(self):
         self.osr = self.CLASS(file_path(self.FILENAME))
         self.dz = DeepZoomGenerator(self.osr, 254, 1)
 
@@ -73,14 +73,19 @@
                 (300, 250),
             ),
         )
 
     def test_get_tile(self):
         self.assertEqual(self.dz.get_tile(9, (1, 0)).size, (47, 250))
 
+    def test_tile_color_profile(self):
+        if self.CLASS is OpenSlide and not lowlevel.read_icc_profile.available:
+            self.skipTest("requires OpenSlide 4.0.0")
+        self.assertEqual(len(self.dz.get_tile(9, (1, 0)).info['icc_profile']), 588)
+
     def test_get_tile_bad_level(self):
         self.assertRaises(ValueError, lambda: self.dz.get_tile(-1, (0, 0)))
         self.assertRaises(ValueError, lambda: self.dz.get_tile(10, (0, 0)))
 
     def test_get_tile_bad_address(self):
         self.assertRaises(ValueError, lambda: self.dz.get_tile(0, (-1, 0)))
         self.assertRaises(ValueError, lambda: self.dz.get_tile(0, (1, 0)))
```

### Comparing `openslide-python-1.2.0/tests/test_imageslide.py` & `openslide-python-1.3.0/tests/test_imageslide.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # openslide-python - Python bindings for the OpenSlide library
 #
-# Copyright (c) 2016-2021 Benjamin Gilbert
+# Copyright (c) 2016-2023 Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -16,18 +16,17 @@
 # along with this library; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 
 import unittest
 
 from PIL import Image
+from common import file_path
 
-from openslide import ImageSlide, OpenSlideCache, OpenSlideError
-
-from . import file_path, maybe_supported
+from openslide import ImageSlide, OpenSlideCache, OpenSlideError, lowlevel
 
 
 class TestImageWithoutOpening(unittest.TestCase):
     def test_detect_format(self):
         self.assertTrue(ImageSlide.detect_format(file_path('__missing_file')) is None)
         self.assertTrue(ImageSlide.detect_format(file_path('../setup.py')) is None)
         self.assertEqual(ImageSlide.detect_format(file_path('boxes.png')), 'PNG')
@@ -59,21 +58,25 @@
         with osr:
             pass
         self.assertRaises(
             AttributeError, lambda: osr.read_region((0, 0), 0, (100, 100))
         )
 
 
-class TestImage(unittest.TestCase):
+class _SlideTest:
     def setUp(self):
-        self.osr = ImageSlide(file_path('boxes.png'))
+        self.osr = ImageSlide(file_path(self.FILENAME))
 
     def tearDown(self):
         self.osr.close()
 
+
+class TestImage(_SlideTest, unittest.TestCase):
+    FILENAME = 'boxes.png'
+
     def test_repr(self):
         self.assertEqual(repr(self.osr), 'ImageSlide(%r)' % file_path('boxes.png'))
 
     def test_metadata(self):
         self.assertEqual(self.osr.level_count, 1)
         self.assertEqual(self.osr.level_dimensions, ((300, 250),))
         self.assertEqual(self.osr.dimensions, (300, 250))
@@ -81,14 +84,23 @@
 
         self.assertEqual(self.osr.get_best_level_for_downsample(0.5), 0)
         self.assertEqual(self.osr.get_best_level_for_downsample(3), 0)
 
         self.assertEqual(self.osr.properties, {})
         self.assertEqual(self.osr.associated_images, {})
 
+    def test_color_profile(self):
+        self.assertEqual(self.osr.color_profile.profile.device_class, 'mntr')
+        self.assertEqual(
+            len(self.osr.read_region((0, 0), 0, (100, 100)).info['icc_profile']), 588
+        )
+        self.assertEqual(
+            len(self.osr.get_thumbnail((100, 100)).info['icc_profile']), 588
+        )
+
     def test_read_region(self):
         self.assertEqual(
             self.osr.read_region((-10, -10), 0, (400, 400)).size, (400, 400)
         )
 
     def test_read_region_size_dimension_zero(self):
         self.assertEqual(self.osr.read_region((0, 0), 0, (400, 0)).size, (400, 0))
@@ -102,11 +114,22 @@
         self.assertRaises(
             OpenSlideError, lambda: self.osr.read_region((0, 0), 0, (400, -5))
         )
 
     def test_thumbnail(self):
         self.assertEqual(self.osr.get_thumbnail((100, 100)).size, (100, 83))
 
-    @maybe_supported
+    @unittest.skipUnless(lowlevel.cache_create.available, "requires OpenSlide 4.0.0")
     def test_set_cache(self):
         self.osr.set_cache(OpenSlideCache(64 << 10))
         self.assertEqual(self.osr.read_region((0, 0), 0, (400, 400)).size, (400, 400))
+
+
+class TestNoIccImage(_SlideTest, unittest.TestCase):
+    FILENAME = 'boxes-no-icc.png'
+
+    def test_color_profile(self):
+        self.assertIsNone(self.osr.color_profile)
+        self.assertNotIn(
+            'icc_profile', self.osr.read_region((0, 0), 0, (100, 100)).info
+        )
+        self.assertNotIn('icc_profile', self.osr.get_thumbnail((100, 100)).info)
```

### Comparing `openslide-python-1.2.0/tests/test_openslide.py` & `openslide-python-1.3.0/tests/test_openslide.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # openslide-python - Python bindings for the OpenSlide library
 #
-# Copyright (c) 2016-2021 Benjamin Gilbert
+# Copyright (c) 2016-2023 Benjamin Gilbert
 #
 # This library is free software; you can redistribute it and/or modify it
 # under the terms of version 2.1 of the GNU Lesser General Public License
 # as published by the Free Software Foundation.
 #
 # This library is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
@@ -19,27 +19,27 @@
 
 from ctypes import ArgumentError
 import re
 import sys
 import unittest
 
 from PIL import Image
+from common import file_path
 
 from openslide import (
     OpenSlide,
     OpenSlideCache,
     OpenSlideError,
     OpenSlideUnsupportedFormatError,
+    lowlevel,
 )
 
-from . import file_path, maybe_supported
-
 
 class TestCache(unittest.TestCase):
-    @maybe_supported
+    @unittest.skipUnless(lowlevel.cache_create.available, "requires OpenSlide 4.0.0")
     def test_create_cache(self):
         OpenSlideCache(0)
         OpenSlideCache(1)
         OpenSlideCache(4 << 20)
         self.assertRaises(ArgumentError, lambda: OpenSlideCache(-1))
         self.assertRaises(ArgumentError, lambda: OpenSlideCache(1.3))
 
@@ -119,14 +119,26 @@
         self.assertEqual(
             len([v for v in self.osr.properties]), len(self.osr.properties)
         )
         self.assertEqual(
             repr(self.osr.properties), '<_PropertyMap %r>' % dict(self.osr.properties)
         )
 
+    @unittest.skipUnless(
+        lowlevel.read_icc_profile.available, "requires OpenSlide 4.0.0"
+    )
+    def test_color_profile(self):
+        self.assertEqual(self.osr.color_profile.profile.device_class, 'mntr')
+        self.assertEqual(
+            len(self.osr.read_region((0, 0), 0, (100, 100)).info['icc_profile']), 588
+        )
+        self.assertEqual(
+            len(self.osr.get_thumbnail((100, 100)).info['icc_profile']), 588
+        )
+
     def test_read_region(self):
         self.assertEqual(
             self.osr.read_region((-10, -10), 1, (400, 400)).size, (400, 400)
         )
 
     def test_read_region_size_dimension_zero(self):
         self.assertEqual(self.osr.read_region((0, 0), 1, (400, 0)).size, (400, 0))
@@ -152,15 +164,15 @@
         self.assertEqual(
             self.osr.read_region((1000, 1000), 0, (32768, 16384)).size, (32768, 16384)
         )
 
     def test_thumbnail(self):
         self.assertEqual(self.osr.get_thumbnail((100, 100)).size, (100, 83))
 
-    @maybe_supported
+    @unittest.skipUnless(lowlevel.cache_create.available, "requires OpenSlide 4.0.0")
     def test_set_cache(self):
         self.osr.set_cache(OpenSlideCache(64 << 10))
         self.assertEqual(self.osr.read_region((0, 0), 0, (400, 400)).size, (400, 400))
         self.assertRaises(TypeError, lambda: self.osr.set_cache(None))
         self.assertRaises(TypeError, lambda: self.osr.set_cache(3))
 
 
@@ -180,14 +192,39 @@
             return re.sub('0x[0-9a-fA-F]+', '(mangled)', repr(o))
 
         self.assertEqual(
             mangle_repr(self.osr.associated_images),
             '<_AssociatedImageMap %s>' % mangle_repr(dict(self.osr.associated_images)),
         )
 
+    def test_color_profile(self):
+        self.assertIsNone(self.osr.color_profile)
+        self.assertNotIn(
+            'icc_profile', self.osr.read_region((0, 0), 0, (100, 100)).info
+        )
+        self.assertNotIn('icc_profile', self.osr.associated_images['thumbnail'].info)
+        self.assertNotIn('icc_profile', self.osr.get_thumbnail((100, 100)).info)
+
+
+# Requires DICOM support in OpenSlide.  Use associated image ICC support as
+# a proxy.
+@unittest.skipUnless(
+    lowlevel.read_associated_image_icc_profile.available, "requires OpenSlide 4.0.0"
+)
+class TestDicomSlide(_SlideTest, unittest.TestCase):
+    FILENAME = 'boxes_0.dcm'
+
+    def test_color_profile(self):
+        self.assertEqual(self.osr.color_profile.profile.device_class, 'mntr')
+        main_profile = self.osr.read_region((0, 0), 0, (100, 100)).info['icc_profile']
+        associated_profile = self.osr.associated_images['thumbnail'].info['icc_profile']
+        self.assertEqual(len(main_profile), 456)
+        self.assertEqual(main_profile, associated_profile)
+        self.assertIs(main_profile, associated_profile)
+
 
 class TestUnreadableSlide(_SlideTest, unittest.TestCase):
     FILENAME = 'unreadable.svs'
 
     def test_read_bad_region(self):
         self.assertEqual(self.osr.properties['openslide.vendor'], 'aperio')
         self.assertRaises(
```

### Comparing `openslide-python-1.2.0/tests/unopenable.tiff` & `openslide-python-1.3.0/tests/fixtures/unopenable.tiff`

 * *Files identical despite different names*

### Comparing `openslide-python-1.2.0/tests/unreadable.svs` & `openslide-python-1.3.0/tests/fixtures/unreadable.svs`

 * *Files identical despite different names*

