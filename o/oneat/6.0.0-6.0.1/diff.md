# Comparing `tmp/oneat-6.0.0.tar.gz` & `tmp/oneat-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.0.0.tar", last modified: Thu Dec  1 17:14:24 2022, max compression
+gzip compressed data, was "oneat-6.0.1.tar", last modified: Sat Jul 22 10:34:14 2023, max compression
```

## Comparing `oneat-6.0.0.tar` & `oneat-6.0.1.tar`

### file list

```diff
@@ -1,135 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.969071 oneat-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2022-12-01 17:14:07.000000 oneat-6.0.0/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-01 17:14:07.000000 oneat-6.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2022-12-01 17:14:07.000000 oneat-6.0.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-01 17:14:07.000000 oneat-6.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/Yoloneat.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/other.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-01 17:14:07.000000 oneat-6.0.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-01 17:14:07.000000 oneat-6.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:14:07.000000 oneat-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-01 17:14:07.000000 oneat-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:14:24.969071 oneat-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2022-12-01 17:14:07.000000 oneat-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   190057 2022-12-01 17:14:07.000000 oneat-6.0.0/images/Xenopus_example.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   752746 2022-12-01 17:14:07.000000 oneat-6.0.0/images/Xenopus_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    33384 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_0_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    34434 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_1_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    64858 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_2_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    79433 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_3_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    50517 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_4_crop.png
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2022-12-01 17:14:07.000000 oneat-6.0.0/images/ch_5_crop.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/Apache-2
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/BSD-3
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/GPL-3
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/LGPL-3
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/MIT
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2022-12-01 17:14:07.000000 oneat-6.0.0/licenses/MPL-2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/logs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.945070 oneat-6.0.0/logs/fit/20221123-151122/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-151122/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-151122/train/events.out.tfevents.1669212683.KAPOORLABS.12084.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-151247/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-151247/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-151247/train/events.out.tfevents.1669212767.KAPOORLABS.6468.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152314/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152314/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152314/train/events.out.tfevents.1669213394.KAPOORLABS.37528.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152337/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152337/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152337/train/events.out.tfevents.1669213417.KAPOORLABS.17652.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152411/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.953070 oneat-6.0.0/logs/fit/20221123-152411/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152411/train/events.out.tfevents.1669213451.KAPOORLABS.20748.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-152525/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-152525/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-152525/train/events.out.tfevents.1669213525.Kapoorlabs.1753.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153101/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153101/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153101/train/events.out.tfevents.1669213861.Kapoorlabs.1839.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153142/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153142/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153142/train/events.out.tfevents.1669213902.Kapoorlabs.1925.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153330/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153330/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153330/train/events.out.tfevents.1669214010.Kapoorlabs.2330.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153435/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153435/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153435/train/events.out.tfevents.1669214075.KAPOORLABS.24332.0.v2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/logs/fit/20221123-153515/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/logs/fit/20221123-153515/train/
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2022-12-01 17:14:07.000000 oneat-6.0.0/logs/fit/20221123-153515/train/events.out.tfevents.1669214115.KAPOORLABS.40224.0.v2
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-01 17:14:07.000000 oneat-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-01 17:14:24.969071 oneat-6.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.949070 oneat-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/src/oneat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATModels/
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    38176 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40718 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    27082 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    39187 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    38167 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40628 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/
--rw-r--r--   0 runner    (1001) docker     (123)    24113 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 runner    (1001) docker     (123)    51303 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25380 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25029 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    70487 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.961070 oneat-6.0.0/src/oneat/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.969071 oneat-6.0.0/src/oneat/_tests/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  5142983 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/caped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2022-12-01 17:14:07.000000 oneat-6.0.0/src/oneat/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 17:14:24.957070 oneat-6.0.0/src/oneat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-01 17:14:24.000000 oneat-6.0.0/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-01 17:14:07.000000 oneat-6.0.0/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.357244 oneat-6.0.1/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-21 15:19:05.000000 oneat-6.0.1/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.0.1/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.334573 oneat-6.0.1/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.337341 oneat-6.0.1/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.0.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1002 2023-07-21 10:27:28.000000 oneat-6.0.1/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.338324 oneat-6.0.1/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.338456 oneat-6.0.1/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.0.1/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.1/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.0.1/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 10:34:14.357334 oneat-6.0.1/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.0.1/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.342102 oneat-6.0.1/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.0.1/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.0.1/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.0.1/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.343804 oneat-6.0.1/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.0.1/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.0.1/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-22 10:34:14.357697 oneat-6.0.1/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.335023 oneat-6.0.1/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.344536 oneat-6.0.1/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.348042 oneat-6.0.1/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13041 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38183 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.350139 oneat-6.0.1/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51261 2023-07-22 10:31:13.000000 oneat-6.0.1/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.351015 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.351942 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.352463 oneat-6.0.1/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.356346 oneat-6.0.1/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.0.1/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-22 10:34:14.345319 oneat-6.0.1/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2630 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-22 10:34:14.000000 oneat-6.0.1/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.0.1/tox.ini
```

### Comparing `oneat-6.0.0/.DS_Store` & `oneat-6.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/.github/workflows/test_and_deploy.yml` & `oneat-6.0.1/.github/workflows/test_and_deploy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
       - name: Coverage
         uses: codecov/codecov-action@v2
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
-    #needs: [test]
+    needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
```

### Comparing `oneat-6.0.0/.gitignore` & `oneat-6.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/.pre-commit-config.yaml` & `oneat-6.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/LICENSE` & `oneat-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/PKG-INFO` & `oneat-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.0
+Version: 6.0.1
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.0/README.md` & `oneat-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/Xenopus_example.jpg` & `oneat-6.0.1/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/Xenopus_example.png` & `oneat-6.0.1/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_0_crop.png` & `oneat-6.0.1/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_1_crop.png` & `oneat-6.0.1/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_2_crop.png` & `oneat-6.0.1/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_3_crop.png` & `oneat-6.0.1/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_4_crop.png` & `oneat-6.0.1/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/images/ch_5_crop.png` & `oneat-6.0.1/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/Apache-2` & `oneat-6.0.1/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/BSD-3` & `oneat-6.0.1/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/GPL-3` & `oneat-6.0.1/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/LGPL-3` & `oneat-6.0.1/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/MIT` & `oneat-6.0.1/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/licenses/MPL-2` & `oneat-6.0.1/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/setup.cfg` & `oneat-6.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 install_requires = 
 	pandas
 	vollseg-napari
 	scipy
 	tifffile
 	matplotlib
 	imagecodecs
-	napari[all]
 	scikit-learn
 	dask
 	natsort
 	napari-animation
 	pydot
 	graphviz
 	oneat-augmentations
```

### Comparing `oneat-6.0.0/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.0.1/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.0.1/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.0.1/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.0.1/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/__init__.py` & `oneat-6.0.1/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/config.py` & `oneat-6.0.1/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.0.1/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/loss.py` & `oneat-6.0.1/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import tensorflow as tf
 from tqdm import tqdm
 from oneat.NEATModels import nets
 from oneat.NEATModels.nets import Concat
 from oneat.NEATModels.loss import volume_yolo_loss
 from oneat.pretrained import get_registered_models, get_model_details, get_model_instance
 from pathlib import Path
-from tensorflow.keras.models import load_model
+from keras.models import load_model
 from tifffile import imread
 
 
 class NEATDenseVollNet(object):
     """
     Parameters
     ----------
@@ -242,15 +242,15 @@
         self.Trainingmodel.save(self.model_dir)
     """
     The input image and seg image are numpy arrays that have to be read prior to being loaded in the function
     """
     def get_markers(self, 
                     segimage : np.ndarray):
 
-        self.segimage = segimage
+        self.segimage = segimage.astype(np.uint16)
         print('Obtaining Markers')
         self.pad_width = (self.config['imagey'], self.config['imagex'])
         self.markers = GenerateVolumeMarkers(self.segimage, pad_width = self.pad_width)
         self.marker_tree = MakeForest(self.markers)
         self.segimage = None         
 
         return self.marker_tree
```

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_focus.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.0.1/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATModels/nets.py` & `oneat-6.0.1/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.0.1/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,18 +370,18 @@
 
                 listscore = Score.tolist()
                 listconfidence = Confidence.tolist()
 
                 for i in range(len(listtime)):
 
                     tcenter = int(listtime[i])
-                    ycenter = listy[i]
-                    xcenter = listx[i]
-                    size = listsize[i]
-                    score = listscore[i]
+                    ycenter = float(listy[i])
+                    xcenter = float(listx[i])
+                    size = float(listsize[i])
+                    score = float(listscore[i])
                     confidence = listconfidence[i]
                     if score > event_threshold:
                         event_locations.append(
                             [int(tcenter), int(ycenter), int(xcenter)]
                         )
 
                         if int(tcenter) in event_locations_dict.keys():
```

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.0.1/src/oneat/NEATUtils/MovieCreator.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,18 @@
                 event_name = static_name[i]
                 trainlabel = static_label[i]
                 classfound = Csvname == csv_name_diff + event_name + name
                 if classfound:
                     print(Csvname)
                     image = imread(fname).astype(dtype)
                     dataset = pd.read_csv(csvfname)
-                    time = dataset[dataset.keys()[0]][1:]
-                    z = dataset[dataset.keys()[1]][1:]
-                    y = dataset[dataset.keys()[2]][1:]
-                    x = dataset[dataset.keys()[3]][1:]
+                    time = dataset[dataset.keys()[0]]
+                    z = dataset[dataset.keys()[1]]
+                    y = dataset[dataset.keys()[2]]
+                    x = dataset[dataset.keys()[3]]
 
                     # Categories + XYHW + Confidence
                     for (key, t) in time.items():
 
                         SimpleMovieMaker4D(
                             normalizeimage,
                             t,
@@ -670,17 +670,17 @@
                             Csvname == csv_name_diff + event_name + name
                         )
                         if classfound:
                             print(Csvname)
                             image = imread(fname).astype(dtype)
                             segimage = imread(Segfname).astype("uint16")
                             dataset = pd.read_csv(csvfname)
-                            time = dataset[dataset.keys()[0]][1:]
-                            y = dataset[dataset.keys()[1]][1:]
-                            x = dataset[dataset.keys()[2]][1:]
+                            time = dataset[dataset.keys()[0]]
+                            y = dataset[dataset.keys()[1]]
+                            x = dataset[dataset.keys()[2]]
 
                             # Categories + XYHW + Confidence
                             for (key, t) in time.items():
 
                                 MovieMaker(
                                     t,
                                     y[key],
@@ -713,15 +713,15 @@
     csv_name_diff,
     crop_size,
     gridx=1,
     gridy=1,
     gridz=1,
     tshift=0,
     normalizeimage=True,
-    dtype=np.uint8,
+    dtype=np.float32,
 ):
 
     raw_path = os.path.join(image_dir, "*tif")
     Seg_path = os.path.join(seg_image_dir, "*tif")
     Csv_path = os.path.join(csv_dir, "*csv")
     files_raw = glob.glob(raw_path)
     files_raw.sort
@@ -751,18 +751,18 @@
                             Csvname == csv_name_diff + event_name + name
                         )
                         if classfound:
                             print(Csvname)
                             image = imread(fname).astype(dtype)
                             segimage = imread(Segfname).astype("uint16")
                             dataset = pd.read_csv(csvfname)
-                            time = dataset[dataset.keys()[0]][1:]
-                            z = dataset[dataset.keys()[1]][1:]
-                            y = dataset[dataset.keys()[2]][1:]
-                            x = dataset[dataset.keys()[3]][1:]
+                            time = dataset[dataset.keys()[0]]
+                            z = dataset[dataset.keys()[1]]
+                            y = dataset[dataset.keys()[2]]
+                            x = dataset[dataset.keys()[3]]
 
                             # Categories + XYZHW + Confidence
                             for (key, t) in time.items():
 
                                 VolumeMaker(
                                     t,
                                     z[key],
```

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/NMS.py` & `oneat-6.0.1/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.0.1/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.0.1/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,79 +64,80 @@
 
         for (k, v) in self.event_locations_dict.items():
             currenttime = k
             event_locations = v
 
             if len(event_locations) > 0:
                 tree = spatial.cKDTree(event_locations)
-                forwardtime = currenttime + 1
-                if int(forwardtime) in self.event_locations_dict.keys():
-                    forward_event_locations = self.event_locations_dict[
-                        int(forwardtime)
-                    ]
-                    for location in forward_event_locations:
-                        if (
-                            int(forwardtime),
-                            int(location[0]),
-                            int(location[1]),
-                            int(location[2]),
-                        ) in self.event_locations_size_dict:
-                            (
-                                forwardsize,
-                                forwardscore,
-                                forwardconfidence,
-                            ) = self.event_locations_size_dict[
+                for i in range(1,3):
+                    forwardtime = currenttime + i
+                    if int(forwardtime) in self.event_locations_dict.keys():
+                        forward_event_locations = self.event_locations_dict[
+                            int(forwardtime)
+                        ]
+                        for location in forward_event_locations:
+                            if (
                                 int(forwardtime),
                                 int(location[0]),
                                 int(location[1]),
                                 int(location[2]),
-                            ]
-                            distance, nearest_location = tree.query(location)
-                            nearest_location = (
-                                int(event_locations[nearest_location][0]),
-                                int(event_locations[nearest_location][1]),
-                                int(event_locations[nearest_location][2]),
-                            )
-
-                            if distance <= nms_space:
-                                if (
-                                    int(currenttime),
-                                    int(nearest_location[0]),
-                                    int(nearest_location[1]),
-                                    int(nearest_location[2]),
-                                ) in self.event_locations_size_dict:
-                                    (
-                                        currentsize,
-                                        currentscore,
-                                        currentconfidence,
-                                    ) = self.event_locations_size_dict[
+                            ) in self.event_locations_size_dict:
+                                (
+                                    forwardsize,
+                                    forwardscore,
+                                    forwardconfidence,
+                                ) = self.event_locations_size_dict[
+                                    int(forwardtime),
+                                    int(location[0]),
+                                    int(location[1]),
+                                    int(location[2]),
+                                ]
+                                distance, nearest_location = tree.query(location)
+                                nearest_location = (
+                                    int(event_locations[nearest_location][0]),
+                                    int(event_locations[nearest_location][1]),
+                                    int(event_locations[nearest_location][2]),
+                                )
+
+                                if distance <= nms_space:
+                                    if (
                                         int(currenttime),
                                         int(nearest_location[0]),
                                         int(nearest_location[1]),
                                         int(nearest_location[2]),
-                                    ]
-                                    if currentscore >= forwardscore:
-                                        self.event_locations_size_dict.pop(
-                                            (
-                                                int(forwardtime),
-                                                int(location[0]),
-                                                int(location[1]),
-                                                int(location[2]),
+                                    ) in self.event_locations_size_dict:
+                                        (
+                                            currentsize,
+                                            currentscore,
+                                            currentconfidence,
+                                        ) = self.event_locations_size_dict[
+                                            int(currenttime),
+                                            int(nearest_location[0]),
+                                            int(nearest_location[1]),
+                                            int(nearest_location[2]),
+                                        ]
+                                        if currentscore >= forwardscore:
+                                            self.event_locations_size_dict.pop(
+                                                (
+                                                    int(forwardtime),
+                                                    int(location[0]),
+                                                    int(location[1]),
+                                                    int(location[2]),
+                                                )
                                             )
-                                        )
 
-                                    if currentscore < forwardscore:
-                                        self.event_locations_size_dict.pop(
-                                            (
-                                                int(currenttime),
-                                                int(nearest_location[0]),
-                                                int(nearest_location[1]),
-                                                int(nearest_location[2]),
+                                        if currentscore < forwardscore:
+                                            self.event_locations_size_dict.pop(
+                                                (
+                                                    int(currenttime),
+                                                    int(nearest_location[0]),
+                                                    int(nearest_location[1]),
+                                                    int(nearest_location[2]),
+                                                )
                                             )
-                                        )
 
         print("after", len(self.event_locations_size_dict))
         self.show_clean_csv()
 
     def show_clean_csv(self):
         self.cleaneventlist = []
         self.cleantimelist = []
@@ -281,15 +282,15 @@
                         and self.seg_image is not None
                     ):
 
                         all_cells = self.cell_count[i]
                         celllist.append(all_cells + 1)
                         normeventlist.append(countT / (all_cells + 1))
                 self.cleannormeventlist = []
-                if len(self.cleaneventlist) > 0:
+                if len(celllist) > 0:
                     for k in range(len(self.cleaneventlist)):
                         self.cleannormeventlist.append(
                             self.cleaneventlist[k] / celllist[k]
                         )
 
                 if self.plot_event_name == self.event_count_plot:
                     self.ax.plot(timelist, eventlist, "-r")
@@ -418,22 +419,22 @@
                 csvname = list(Path(self.csvdir).glob("*.csv"))[0]
         if csvname is not None:
 
             self.event_name = csv_event_name
             self.dataset = pd.read_csv(csvname, delimiter=",")
             nrows = len(self.dataset.columns)
             for index, row in self.dataset.iterrows():
-                tcenter = int(row[0])
-                zcenter = row[1]
-                ycenter = row[2]
-                xcenter = row[3]
+                tcenter = int(float(row[0]))
+                zcenter = float(row[1]) - 1
+                ycenter = float(row[2])
+                xcenter = float(row[3])
                 if nrows > 4:
-                    score = row[4]
-                    size = row[5]
-                    confidence = row[6]
+                    score = float(row[4])
+                    size = float(row[5])
+                    confidence = float(row[6])
                 else:
                     score = 1.0
                     size = 10
                     confidence = 1.0
                 self.dataset_index = self.dataset.index
                 if score > event_threshold:
                     self.event_locations.append(
```

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.0.1/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/plotters.py` & `oneat-6.0.1/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/NEATUtils/utils.py` & `oneat-6.0.1/src/oneat/NEATUtils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from skimage import measure, morphology
 from skimage.measure import label
 from skimage.morphology import binary_dilation, dilation, square
 from skimage.util import invert as invertimage
 from tifffile import imwrite
 from tqdm import tqdm
 from skimage.measure import regionprops
+from tifffile import imread
 
 def location_map(
     event_locations_dict: dict,
     seg_image: np.ndarray,
     heatmapsteps: int,
     display_3d: bool = True,
 ):
@@ -138,15 +139,14 @@
         indices = [prop.centroid for prop in waterproperties]
         MarkerList.append([i, indices[0], indices[1]])
     return MarkerList
 
 
 def load_json(fpath):
     with open(fpath) as f:
-
         return json.load(f)
 
 
 def save_json(data, fpath, **kwargs):
     with open(fpath, "w") as f:
         f.write(json.dumps(data, **kwargs))
 
@@ -184,57 +184,61 @@
 
 
 def generate_membrane_locations(membranesegimage : np.ndarray, csvfile: str, savefile: str):
     
     dataset = pd.read_csv(csvfile, delimiter = ',')
     
     
-    writer = csv.writer(open(savefile + ".csv", "a", newline=""))
+    writer = csv.writer(open(savefile, "a", newline=""))
     writer.writerow(
                         [
                             "T",
                             "Z",
                             "Y",
                             "X",
                             "Score",
                             "Size",
                             "Confidence",
                         ]
     )
     nrows = len(dataset.columns)
     dict_membrane = {}
-    for i in range(membranesegimage.shape[0]):
+    if isinstance(membranesegimage, str):
+        membranesegimage = imread(membranesegimage)
+
+    for i in tqdm(range(membranesegimage.shape[0])):
         currentimage = membranesegimage[i,:,:,:]
         properties = measure.regionprops(currentimage) 
         membrane_coordinates = [prop.centroid for prop in properties]
         dict_membrane[i] =  membrane_coordinates
         
     for index, row in dataset.iterrows():
         time = int(row[0])
         z = int(row[1])
         y = int(row[2])
         x = int(row[3])
         index = (z,y,x)
-        if nrows > 4:
-                    score = row[4]
-                    size = row[5]
-                    confidence = row[6]
-        else:
-                    score = 1.0
-                    size = 10
-                    confidence = 1.0
-        membrane_coordinates = dict_membrane[time]
-        if len(membrane_coordinates) > 0:
-           tree = spatial.cKDTree(membrane_coordinates)  
-           distance, nearest_location = tree.query(index)          
-                    
-           z = membrane_coordinates[nearest_location][0]         
-           y = membrane_coordinates[nearest_location][1]
-           x = membrane_coordinates[nearest_location][2]
-           writer.writerow([time, z, y, x, score, size, confidence])
+        if time < membranesegimage.shape[0]:
+            if nrows > 4:
+                        score = row[4]
+                        size = row[5]
+                        confidence = row[6]
+            else:
+                        score = 1.0
+                        size = 10
+                        confidence = 1.0
+            membrane_coordinates = dict_membrane[time]
+            if len(membrane_coordinates) > 0:
+                tree = spatial.cKDTree(membrane_coordinates)  
+                distance, nearest_location = tree.query(index)          
+                            
+                z = int(membrane_coordinates[nearest_location][0])         
+                y = membrane_coordinates[nearest_location][1]
+                x = membrane_coordinates[nearest_location][2]
+                writer.writerow([time, z, y, x, score, size, confidence])
 
 
 def load_training_data(directory, filename, axes=None, verbose=True):
     """Load training data in .npz format.
     The data file is expected to have the keys 'data' and 'label'
     """
     if directory is not None:
@@ -569,39 +573,40 @@
     # TZYX
     Markers = np.zeros(
         [
             segimage.shape[0],
             segimage.shape[1],
             segimage.shape[2] + pad_width[0],
             segimage.shape[3] + pad_width[1],
-        ]
+        ],
+        dtype=np.uint16,
     )
 
     for i in tqdm(range(0, segimage.shape[0])):
 
         smallimage = segimage[i, :]
         newsmallimage = pad_timelapse(smallimage, pad_width)
-        properties = measure.regionprops(newsmallimage.astype("uint16"))
+        properties = measure.regionprops(newsmallimage.astype(np.uint16))
 
         Coordinates = [prop.centroid for prop in properties]
         if len(Coordinates) > 0:
             Coordinates = sorted(Coordinates, key=lambda k: [k[2], k[1], k[0]])
             Coordinates = np.asarray(Coordinates)
 
             coordinates_int = np.round(Coordinates).astype(int)
             markers_raw = np.zeros_like(newsmallimage)
             markers_raw[tuple(coordinates_int.T)] = 1 + np.arange(
                 len(Coordinates)
             )
             if ndim == 4:
                 markers = morphology.dilation(
-                    markers_raw.astype("uint16"), morphology.ball(2)
+                    markers_raw.astype(np.uint16), morphology.ball(2)
                 )
 
-            Markers[i, :] = label(markers.astype("uint16"))
+            Markers[i, :] = label(markers.astype(np.uint16))
 
     return Markers
 
 
 def GenerateMarkers(
     segimage, start_project_mid=4, end_project_mid=4, pad_width=(0, 0)
 ):
```

### Comparing `oneat-6.0.0/src/oneat/__init__.py` & `oneat-6.0.1/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/_tests/test_nets.py` & `oneat-6.0.1/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/_tests/utils.py` & `oneat-6.0.1/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.0.1/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/_tests/variables/variables.index` & `oneat-6.0.1/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat/pretrained.py` & `oneat-6.0.1/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.0.0/src/oneat.egg-info/PKG-INFO` & `oneat-6.0.1/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.0.0
+Version: 6.0.1
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.0.0/tox.ini` & `oneat-6.0.1/tox.ini`

 * *Files identical despite different names*

