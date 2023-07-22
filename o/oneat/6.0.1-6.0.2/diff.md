# Comparing `tmp/oneat-6.0.1.tar.gz` & `tmp/oneat-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.0.1.tar", last modified: Sat Jul 22 10:34:14 2023, max compression
+gzip compressed data, was "oneat-6.0.2.tar", last modified: Sat Jul 22 19:14:16 2023, max compression
```

## Comparing `oneat-6.0.1.tar` & `oneat-6.0.2.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.357244 oneat-6.0.1/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-21 15:19:05.000000 oneat-6.0.1/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.0.1/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.334573 oneat-6.0.1/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.337341 oneat-6.0.1/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.0.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1002 2023-07-21 10:27:28.000000 oneat-6.0.1/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.338324 oneat-6.0.1/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.338456 oneat-6.0.1/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.0.1/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.1/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.0.1/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 10:34:14.357334 oneat-6.0.1/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.0.1/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.342102 oneat-6.0.1/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.0.1/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.0.1/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.343804 oneat-6.0.1/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.0.1/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-22 10:34:14.357697 oneat-6.0.1/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.335023 oneat-6.0.1/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.344536 oneat-6.0.1/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.348042 oneat-6.0.1/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38183 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.350139 oneat-6.0.1/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51261 2023-07-22 10:31:13.000000 oneat-6.0.1/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.351015 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.351942 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.352463 oneat-6.0.1/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.356346 oneat-6.0.1/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.345319 oneat-6.0.1/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2630 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.0.1/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.738637 oneat-6.0.2/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.0.2/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.0.2/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.716122 oneat-6.0.2/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.719224 oneat-6.0.2/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.0.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.0.2/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.720250 oneat-6.0.2/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.720381 oneat-6.0.2/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.0.2/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.0.2/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.2/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.0.2/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 19:14:16.738726 oneat-6.0.2/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.0.2/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.724224 oneat-6.0.2/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.0.2/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.0.2/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.0.2/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.725610 oneat-6.0.2/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.0.2/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.0.2/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-22 19:14:16.739091 oneat-6.0.2/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.716560 oneat-6.0.2/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.726365 oneat-6.0.2/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.730291 oneat-6.0.2/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    37827 2023-07-22 19:13:20.000000 oneat-6.0.2/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.732339 oneat-6.0.2/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.0.2/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.733230 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.734082 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.734486 oneat-6.0.2/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.738407 oneat-6.0.2/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.0.2/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 19:14:16.727200 oneat-6.0.2/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-22 19:14:16.000000 oneat-6.0.2/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.0.2/tox.ini
```

### Comparing `oneat-6.0.1/.DS_Store` & `oneat-6.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/.github/workflows/test_and_deploy.yml` & `oneat-6.0.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/.gitignore` & `oneat-6.0.2/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -78,9 +78,8 @@
 
 # pyenv
 .python-version
 
 # OS
 .DS_Store
 
-# written by setuptools_scm
-**/_version.py
+
```

### Comparing `oneat-6.0.1/.pre-commit-config.yaml` & `oneat-6.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/LICENSE` & `oneat-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/PKG-INFO` & `oneat-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.1
+Version: 6.0.2
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.1/README.md` & `oneat-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/Xenopus_example.jpg` & `oneat-6.0.2/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/Xenopus_example.png` & `oneat-6.0.2/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_0_crop.png` & `oneat-6.0.2/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_1_crop.png` & `oneat-6.0.2/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_2_crop.png` & `oneat-6.0.2/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_3_crop.png` & `oneat-6.0.2/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_4_crop.png` & `oneat-6.0.2/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/images/ch_5_crop.png` & `oneat-6.0.2/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/Apache-2` & `oneat-6.0.2/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/BSD-3` & `oneat-6.0.2/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/GPL-3` & `oneat-6.0.2/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/LGPL-3` & `oneat-6.0.2/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/MIT` & `oneat-6.0.2/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/licenses/MPL-2` & `oneat-6.0.2/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/setup.cfg` & `oneat-6.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.0.2/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.0.2/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.0.2/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.0.2/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/__init__.py` & `oneat-6.0.2/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/config.py` & `oneat-6.0.2/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.0.2/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/loss.py` & `oneat-6.0.2/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,23 +175,16 @@
         self.Y = self.Y.reshape((self.Y.shape[0],1, 1, 1, self.Y.shape[1]))
         self.Y_val = self.Y_val.reshape((self.Y_val.shape[0],1, 1, 1, self.Y_val.shape[1]))
 
     def TrainModel(self):
 
         #ZYXT
         input_shape = (self.X.shape[1], self.X.shape[2], self.X.shape[3], self.X.shape[4])
-        print(self.X.shape)
-        print(input_shape)
         Path(self.model_dir).mkdir(exist_ok=True)
-
-  
         Y_rest = self.Y[:, :, :, :, self.categories:]
-        print(Y_rest.shape)
-
-        
 
         dummyY = np.zeros(
             [self.Y.shape[0], self.Y.shape[1], self.Y.shape[2], self.Y.shape[3], self.categories + self.nboxes * self.box_vector])
         dummyY[:,:, :, :, :self.Y.shape[-1]] = self.Y
 
         dummyY_val = np.zeros([self.Y_val.shape[0], self.Y_val.shape[1], self.Y_val.shape[2], self.Y_val.shape[3],
                                self.categories + self.nboxes * self.box_vector])
@@ -204,15 +197,14 @@
                                                                                                                  self.categories: self.categories + self.box_vector]
             dummyY_val[:, :, :,:,
             self.categories + b * self.box_vector:self.categories + (b + 1) * self.box_vector] = self.Y_val[:, :, :,:,
                                                                                                  self.categories: self.categories + self.box_vector]
 
         self.Y = dummyY
         self.Y_val = dummyY_val
-        print(self.Y.shape)
 
         self.Trainingmodel = self.model_keras(input_shape, self.categories, 
                                               box_vector=Y_rest.shape[-1], yolo_loss = self.yolo_loss, nboxes=self.nboxes,
                                               stage_number=self.stage_number,
                                               depth=self.depth, start_kernel=self.start_kernel,
                                               mid_kernel=self.mid_kernel, 
                                               startfilter=self.startfilter, input_model=self.model_dir,
@@ -222,25 +214,24 @@
         self.Trainingmodel.compile(optimizer=sgd, loss=self.yolo_loss, metrics=['accuracy'])
         self.Trainingmodel.summary()
        
    
         # Keras callbacks
         lrate = callbacks.ReduceLROnPlateau(monitor='loss', factor=0.1, patience=4, verbose=1)
         hrate = callbacks.History()
-        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss', verbose=1,
-                                          save_best_only=False, save_weights_only=False, mode='auto', save_freq=1)
+        srate = callbacks.ModelCheckpoint(self.model_dir, monitor='loss',
+                                          save_best_only=False, save_weights_only=False, mode='auto')
         prate = plotters.PlotVolumeHistory(self.Trainingmodel, self.X_val, self.Y_val, self.key_categories, self.key_cord,
                                      self.gridx, self.gridy, self.gridz, plot=self.show, nboxes=self.nboxes)
         
-        log_dir = "logs/fit/" + datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-        tensorboard_callback = callbacks.TensorBoard(log_dir=log_dir, histogram_freq=1)
+       
         # Train the model and save as a h5 file
         self.Trainingmodel.fit(self.X, self.Y, batch_size=self.batch_size,
-                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val), shuffle=True,
-                               callbacks=[lrate, hrate, srate, prate, tensorboard_callback])
+                               epochs=self.epochs, validation_data=(self.X_val, self.Y_val),
+                               callbacks=[lrate, hrate, srate, prate])
 
 
         self.Trainingmodel.save(self.model_dir)
     """
     The input image and seg image are numpy arrays that have to be read prior to being loaded in the function
     """
     def get_markers(self,
```

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_focus.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.0.2/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATModels/nets.py` & `oneat-6.0.2/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.0.2/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.0.2/src/oneat/NEATUtils/MovieCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,15 @@
     if normalizeimage:
         image = normalizeFloatZeroOne(
             image.astype(dtype), 1, 99.8, dtype=dtype
         )
     if time > size_tminus:
 
         # slice the images
-
+    
         currentsegimage = segimage[int(time), :].astype("uint16")
         image_props = getHWD(
             x, y, z, currentsegimage, imagesizex, imagesizey, imagesizez
         )
         if image_props is not None:
             height, width, depth, center, seg_label = image_props
             smallimage = CreateVolume(
```

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/NMS.py` & `oneat-6.0.2/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.0.2/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.0.2/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.0.2/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.0.2/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/plotters.py` & `oneat-6.0.2/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/NEATUtils/utils.py` & `oneat-6.0.2/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/__init__.py` & `oneat-6.0.2/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/_tests/test_nets.py` & `oneat-6.0.2/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/_tests/utils.py` & `oneat-6.0.2/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.0.2/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/_tests/variables/variables.index` & `oneat-6.0.2/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat/pretrained.py` & `oneat-6.0.2/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.1/src/oneat.egg-info/PKG-INFO` & `oneat-6.0.2/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.1
+Version: 6.0.2
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.1/src/oneat.egg-info/SOURCES.txt` & `oneat-6.0.2/src/oneat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .DS_Store
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+1
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
```

### Comparing `oneat-6.0.1/tox.ini` & `oneat-6.0.2/tox.ini`

 * *Files identical despite different names*

