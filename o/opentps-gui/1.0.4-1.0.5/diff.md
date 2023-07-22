# Comparing `tmp/opentps-gui-1.0.4.tar.gz` & `tmp/opentps_gui-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentps-gui-1.0.4.tar", max compression
+gzip compressed data, was "opentps_gui-1.0.5.tar", max compression
```

## Comparing `opentps-gui-1.0.4.tar` & `opentps_gui-1.0.5.tar`

### file list

```diff
@@ -1,126 +1,130 @@
--rw-r--r--   0        0        0      652 2022-09-26 19:16:59.330368 opentps-gui-1.0.4/LICENSE
--rw-r--r--   0        0        0     1388 2022-09-28 12:17:48.088336 opentps-gui-1.0.4/README.md
--rw-r--r--   0        0        0      268 2022-09-28 08:09:03.691704 opentps-gui-1.0.4/opentps/gui/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 09:19:35.243520 opentps-gui-1.0.4/opentps/gui/examples/extension/extension/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 09:17:07.392639 opentps-gui-1.0.4/opentps/gui/examples/extension/extension/gui/__init__.py
--rw-r--r--   0        0        0      384 2022-09-29 09:16:21.753019 opentps-gui-1.0.4/opentps/gui/examples/extension/extension/gui/extensionPanel.py
--rw-r--r--   0        0        0      146 2022-09-29 09:19:50.279415 opentps-gui-1.0.4/opentps/gui/examples/extension/extension/main.py
--rw-r--r--   0        0        0      246 2022-09-29 09:20:14.359249 opentps-gui-1.0.4/opentps/gui/examples/extension/extension/utils.py
--rw-r--r--   0        0        0      856 2022-09-28 13:26:22.527515 opentps-gui-1.0.4/opentps/gui/main.py
--rw-r--r--   0        0        0     1892 2022-09-26 20:04:57.055860 opentps-gui-1.0.4/opentps/gui/mainWindow.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/__init__.py
--rw-r--r--   0        0        0    10276 2022-09-26 20:30:40.847844 opentps-gui-1.0.4/opentps/gui/panels/breathingSignalPanel.py
--rw-r--r--   0        0        0     4297 2022-09-26 20:30:40.807844 opentps-gui-1.0.4/opentps/gui/panels/doseComparisonPanel.py
--rw-r--r--   0        0        0     8469 2022-09-28 19:40:28.452999 opentps-gui-1.0.4/opentps/gui/panels/doseComputationPanel.py
--rw-r--r--   0        0        0    17856 2022-09-26 19:49:57.285220 opentps-gui-1.0.4/opentps/gui/panels/drrPanel.py
--rw-r--r--   0        0        0     3605 2022-09-28 09:56:47.047575 opentps-gui-1.0.4/opentps/gui/panels/mainToolbar.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/__init__.py
--rw-r--r--   0        0        0     6823 2022-09-26 20:30:40.867844 opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataMenu.py
--rw-r--r--   0        0        0     5971 2022-09-26 20:04:56.927861 opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataPanel.py
--rw-r--r--   0        0        0    11655 2022-09-26 20:30:41.039842 opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataSelection.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/planDesignPanel/__init__.py
--rw-r--r--   0        0        0     5161 2022-09-26 20:30:41.063842 opentps-gui-1.0.4/opentps/gui/panels/planDesignPanel/planDesignPanel.py
--rw-r--r--   0        0        0    11631 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/planDesignPanel/robustnessSettings.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/planOptimizationPanel/__init__.py
--rw-r--r--   0        0        0     8068 2022-09-26 20:30:40.819844 opentps-gui-1.0.4/opentps/gui/panels/planOptimizationPanel/objectivesWindow.py
--rw-r--r--   0        0        0     9056 2022-09-26 20:32:11.082883 opentps-gui-1.0.4/opentps/gui/panels/planOptimizationPanel/planOptiPanel.py
--rw-r--r--   0        0        0     5772 2022-09-26 20:32:11.114883 opentps-gui-1.0.4/opentps/gui/panels/registrationPanel.py
--rw-r--r--   0        0        0     4261 2022-09-26 20:30:40.991842 opentps-gui-1.0.4/opentps/gui/panels/roiPanel.py
--rw-r--r--   0        0        0        0 2022-09-26 14:41:03.201735 opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/__init__.py
--rw-r--r--   0        0        0     7116 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/pythonHighlighter.py
--rw-r--r--   0        0        0     3928 2022-09-26 20:04:57.091859 opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/scriptingPanel.py
--rw-r--r--   0        0        0     1573 2022-09-26 20:04:57.019860 opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/scriptingWindow.py
--rw-r--r--   0        0        0     4120 2022-09-28 19:40:28.444999 opentps-gui-1.0.4/opentps/gui/programSettingEditor.py
--rw-r--r--   0        0        0    15788 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/OpenTPS_icon.png
--rw-r--r--   0        0        0      592 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/arrow-135.png
--rw-r--r--   0        0        0      722 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/chain-unchain.png
--rw-r--r--   0        0        0      430 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/chain.png
--rw-r--r--   0        0        0      659 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/chart.png
--rw-r--r--   0        0        0      560 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/color-adjustment.png
--rw-r--r--   0        0        0      811 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/color.png
--rw-r--r--   0        0        0     1921 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/colormap_histogram.png
--rw-r--r--   0        0        0      618 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/colormap_jet.png
--rw-r--r--   0        0        0      678 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/contrast.png
--rw-r--r--   0        0        0     8956 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/crop.png
--rw-r--r--   0        0        0      544 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/cross.png
--rw-r--r--   0        0        0     1752 2022-09-16 09:19:32.275534 opentps-gui-1.0.4/opentps/gui/res/icons/cube.png
--rw-r--r--   0        0        0      507 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/disk.png
--rw-r--r--   0        0        0      624 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/dvh.png
--rw-r--r--   0        0        0      492 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/equalizer.png
--rw-r--r--   0        0        0     4048 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/fast.png
--rw-r--r--   0        0        0      647 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/folder-open.png
--rw-r--r--   0        0        0      450 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/geolocation.png
--rw-r--r--   0        0        0     6608 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/graph.png
--rw-r--r--   0        0        0     5284 2022-09-16 13:43:00.964689 opentps-gui-1.0.4/opentps/gui/res/icons/iba_nozzle.stl
--rw-r--r--   0        0        0     2502 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/independent_views.png
--rw-r--r--   0        0        0    17284 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/pause.jpg
--rw-r--r--   0        0        0     1637 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/pencil--plus.png
--rw-r--r--   0        0        0    24904 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/play.png
--rw-r--r--   0        0        0      730 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/profile.png
--rw-r--r--   0        0        0    16231 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/reload.png
--rw-r--r--   0        0        0     1872 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/resample.png
--rw-r--r--   0        0        0    10339 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/save.png
--rw-r--r--   0        0        0      503 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/settings-5-line.png
--rw-r--r--   0        0        0     4110 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/slider.png
--rw-r--r--   0        0        0     4117 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/slow.png
--rw-r--r--   0        0        0      605 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/tick-button.png
--rw-r--r--   0        0        0      859 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/icons/x-ray.png
--rw-r--r--   0        0        0    73684 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/res/viewer/human_standing.stl
--rw-r--r--   0        0        0      197 2022-09-26 15:10:03.751747 opentps-gui-1.0.4/opentps/gui/statusBar.py
--rw-r--r--   0        0        0      145 2022-09-26 20:04:57.055860 opentps-gui-1.0.4/opentps/gui/tools/__init__.py
--rw-r--r--   0        0        0    11389 2022-09-26 20:30:40.811844 opentps-gui-1.0.4/opentps/gui/tools/_cropTool.py
--rw-r--r--   0        0        0     3478 2022-09-26 20:30:41.023842 opentps-gui-1.0.4/opentps/gui/tools/_resampleTool.py
--rw-r--r--   0        0        0     9575 2022-09-26 20:30:40.823844 opentps-gui-1.0.4/opentps/gui/viewController.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/viewer/__init__.py
--rw-r--r--   0        0        0      307 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/viewer/dataExplorer.py
--rw-r--r--   0        0        0     2562 2022-09-26 20:30:41.003842 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/ROIContourForViewer.py
--rw-r--r--   0        0        0     2028 2022-09-28 11:42:14.816250 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/ROIMaskForViewer.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/__init__.py
--rw-r--r--   0        0        0     1132 2022-09-26 16:29:36.798123 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dataMultiton.py
--rw-r--r--   0        0        0     2034 2022-09-26 20:05:51.963325 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dyn2DSeqForViewer.py
--rw-r--r--   0        0        0     2168 2022-09-26 20:05:52.003325 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dyn3DSeqForViewer.py
--rw-r--r--   0        0        0     3273 2022-09-26 20:05:51.971325 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/genericImageForViewer.py
--rw-r--r--   0        0        0     2931 2022-09-26 20:05:52.015324 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/image2DForViewer.py
--rw-r--r--   0        0        0     1719 2022-09-26 20:05:52.023324 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/image3DForViewer.py
--rw-r--r--   0        0        0      444 2022-09-26 20:05:52.031324 opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/polyDataForViewer.py
--rw-r--r--   0        0        0    28279 2022-09-26 20:30:40.967843 opentps-gui-1.0.4/opentps/gui/viewer/dataViewer.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/__init__.py
--rw-r--r--   0        0        0      448 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/blackEmptyPlot.py
--rw-r--r--   0        0        0     3605 2022-09-26 20:04:56.935861 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dataViewerToolbar.py
--rw-r--r--   0        0        0     3475 2022-09-26 20:30:40.947843 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/doseComparisonImageProvider.py
--rw-r--r--   0        0        0    11455 2022-09-26 20:30:40.879844 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dvhPlot.py
--rw-r--r--   0        0        0     1401 2022-09-26 20:05:51.963325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dvhViewerActions.py
--rw-r--r--   0        0        0     1859 2022-09-26 20:05:51.999325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dynamicImage2DViewer.py
--rw-r--r--   0        0        0     1792 2022-09-26 20:05:51.979325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dynamicImage3DViewer.py
--rw-r--r--   0        0        0    17639 2022-09-26 20:30:40.803844 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image2DViewer.py
--rw-r--r--   0        0        0    18471 2022-09-26 20:30:40.907843 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image3DViewer.py
--rw-r--r--   0        0        0     4728 2022-09-26 20:30:40.939843 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image3DViewer_3D.py
--rw-r--r--   0        0        0     3963 2022-09-26 20:05:51.959325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageFusionPropEditor.py
--rw-r--r--   0        0        0     9651 2022-09-26 20:30:41.059842 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerActions.py
--rw-r--r--   0        0        0        0 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/__init__.py
--rw-r--r--   0        0        0     6578 2022-09-26 20:30:40.831844 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/contourLayer.py
--rw-r--r--   0        0        0     2400 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/crossHairLayer.py
--rw-r--r--   0        0        0     4212 2022-09-20 16:24:36.198027 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/lookupTables.py
--rw-r--r--   0        0        0     2582 2022-09-26 20:05:51.955325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/polyData3DLayer_3D.py
--rw-r--r--   0        0        0     4941 2022-09-26 20:05:52.015324 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage2DLayer.py
--rw-r--r--   0        0        0     4865 2022-09-26 20:05:52.007325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer.py
--rw-r--r--   0        0        0     3126 2022-09-26 20:05:52.011325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer_3D.py
--rw-r--r--   0        0        0     4916 2022-09-26 20:30:41.027842 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtPlanLayer.py
--rw-r--r--   0        0        0     2902 2022-09-26 20:30:40.839844 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtplanLayer_3D.py
--rw-r--r--   0        0        0     3160 2022-09-26 20:05:52.027324 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage2DLayer.py
--rw-r--r--   0        0        0     3085 2022-09-26 20:05:51.971325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer.py
--rw-r--r--   0        0        0     1420 2022-09-26 20:05:51.987325 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer_3D.py
--rw-r--r--   0        0        0     2548 2022-09-05 07:11:24.794151 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/textLayer.py
--rw-r--r--   0        0        0     2640 2022-09-26 20:30:40.799845 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/patientDataPropertyEditor.py
--rw-r--r--   0        0        0     5923 2022-09-26 19:50:22.996942 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/profileViewer.py
--rw-r--r--   0        0        0     7233 2022-09-26 20:05:52.019324 opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/profileWidget.py
--rw-r--r--   0        0        0     3890 2022-09-26 20:30:40.911843 opentps-gui-1.0.4/opentps/gui/viewer/doseComparisonDataViewer.py
--rw-r--r--   0        0        0     4766 2022-09-16 16:56:54.450642 opentps-gui-1.0.4/opentps/gui/viewer/dynamicDisplayController.py
--rw-r--r--   0        0        0     3344 2022-09-26 20:04:57.147859 opentps-gui-1.0.4/opentps/gui/viewer/exportWindow.py
--rw-r--r--   0        0        0      573 2022-09-05 07:11:24.798151 opentps-gui-1.0.4/opentps/gui/viewer/grid.py
--rw-r--r--   0        0        0     7663 2022-09-26 20:04:57.079860 opentps-gui-1.0.4/opentps/gui/viewer/gridFourElements.py
--rw-r--r--   0        0        0     3695 2022-09-26 20:04:57.115859 opentps-gui-1.0.4/opentps/gui/viewer/viewerPanel.py
--rw-r--r--   0        0        0    12646 2022-09-26 20:04:57.091859 opentps-gui-1.0.4/opentps/gui/viewer/viewerToolbar.py
--rw-r--r--   0        0        0     1035 2022-09-29 16:27:52.290676 opentps-gui-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    52854 2022-09-29 16:27:55.057104 opentps-gui-1.0.4/setup.py
--rw-r--r--   0        0        0     2274 2022-09-29 16:27:55.057699 opentps-gui-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-04-03 11:10:36.361624 opentps_gui-1.0.5/LICENSE
+-rw-r--r--   0        0        0      338 2023-04-03 11:10:36.362624 opentps_gui-1.0.5/opentps/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.363624 opentps_gui-1.0.5/opentps/gui/examples/extension/extension/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.363624 opentps_gui-1.0.5/opentps/gui/examples/extension/extension/gui/__init__.py
+-rw-r--r--   0        0        0      397 2023-04-03 11:10:36.364624 opentps_gui-1.0.5/opentps/gui/examples/extension/extension/gui/extensionPanel.py
+-rw-r--r--   0        0        0      150 2023-04-03 11:10:36.364624 opentps_gui-1.0.5/opentps/gui/examples/extension/extension/main.py
+-rw-r--r--   0        0        0      252 2023-04-03 11:10:36.364624 opentps_gui-1.0.5/opentps/gui/examples/extension/extension/utils.py
+-rw-r--r--   0        0        0     1350 2023-04-03 11:10:36.365625 opentps_gui-1.0.5/opentps/gui/main.py
+-rw-r--r--   0        0        0     2145 2023-04-03 11:10:36.365625 opentps_gui-1.0.5/opentps/gui/mainWindow.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.366624 opentps_gui-1.0.5/opentps/gui/panels/__init__.py
+-rw-r--r--   0        0        0    10517 2023-04-03 11:10:36.367665 opentps_gui-1.0.5/opentps/gui/panels/breathingSignalPanel.py
+-rw-r--r--   0        0        0     1890 2023-04-03 11:10:36.367665 opentps_gui-1.0.5/opentps/gui/panels/doseComparisonPanel.py
+-rw-r--r--   0        0        0     8062 2023-04-03 11:10:36.368626 opentps_gui-1.0.5/opentps/gui/panels/doseComputationPanel.py
+-rw-r--r--   0        0        0    18237 2023-04-03 11:10:36.368626 opentps_gui-1.0.5/opentps/gui/panels/drrPanel.py
+-rw-r--r--   0        0        0     3960 2023-04-03 11:10:36.369627 opentps_gui-1.0.5/opentps/gui/panels/mainToolbar.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.370624 opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/__init__.py
+-rw-r--r--   0        0        0     6976 2023-04-03 11:10:36.370624 opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataMenu.py
+-rw-r--r--   0        0        0     6111 2023-04-03 11:10:36.371626 opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataPanel.py
+-rw-r--r--   0        0        0    11968 2023-04-03 11:10:36.372625 opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataSelection.py
+-rw-r--r--   0        0        0     3591 2023-04-03 11:10:36.372625 opentps_gui-1.0.5/opentps/gui/panels/patientDataWidgets.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.373629 opentps_gui-1.0.5/opentps/gui/panels/planDesignPanel/__init__.py
+-rw-r--r--   0        0        0     2051 2023-04-03 11:10:36.373629 opentps_gui-1.0.5/opentps/gui/panels/planDesignPanel/beamDialog.py
+-rw-r--r--   0        0        0     8819 2023-04-03 11:10:36.374627 opentps_gui-1.0.5/opentps/gui/panels/planDesignPanel/planDesignPanel.py
+-rw-r--r--   0        0        0    15199 2023-04-03 11:10:36.374627 opentps_gui-1.0.5/opentps/gui/panels/planDesignPanel/robustnessSettings.py
+-rw-r--r--   0        0        0     8103 2023-07-05 10:15:09.994112 opentps_gui-1.0.5/opentps/gui/panels/planEvaluationPanel.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.375628 opentps_gui-1.0.5/opentps/gui/panels/planOptimizationPanel/__init__.py
+-rw-r--r--   0        0        0    13080 2023-04-03 11:10:36.376627 opentps_gui-1.0.5/opentps/gui/panels/planOptimizationPanel/objectivesWindow.py
+-rw-r--r--   0        0        0     4820 2023-04-03 11:10:36.376627 opentps_gui-1.0.5/opentps/gui/panels/planOptimizationPanel/optimizationSettings.py
+-rw-r--r--   0        0        0    17159 2023-04-03 11:10:36.377627 opentps_gui-1.0.5/opentps/gui/panels/planOptimizationPanel/planOptiPanel.py
+-rw-r--r--   0        0        0     5922 2023-04-03 11:10:36.377627 opentps_gui-1.0.5/opentps/gui/panels/registrationPanel.py
+-rw-r--r--   0        0        0     4394 2023-04-03 11:10:36.378627 opentps_gui-1.0.5/opentps/gui/panels/roiPanel.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.378627 opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/__init__.py
+-rw-r--r--   0        0        0     7310 2023-04-03 11:10:36.379627 opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/pythonHighlighter.py
+-rw-r--r--   0        0        0     4052 2023-04-03 11:10:36.379627 opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/scriptingPanel.py
+-rw-r--r--   0        0        0     1624 2023-04-03 11:10:36.379627 opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/scriptingWindow.py
+-rw-r--r--   0        0        0     5208 2023-04-03 11:10:36.380627 opentps_gui-1.0.5/opentps/gui/programSettingEditor.py
+-rw-r--r--   0        0        0      592 2023-04-03 11:10:36.381627 opentps_gui-1.0.5/opentps/gui/res/icons/arrow-135.png
+-rw-r--r--   0        0        0      722 2023-04-03 11:10:36.382627 opentps_gui-1.0.5/opentps/gui/res/icons/chain-unchain.png
+-rw-r--r--   0        0        0      430 2023-04-03 11:10:36.383627 opentps_gui-1.0.5/opentps/gui/res/icons/chain.png
+-rw-r--r--   0        0        0      659 2023-04-03 11:10:36.383627 opentps_gui-1.0.5/opentps/gui/res/icons/chart.png
+-rw-r--r--   0        0        0      560 2023-04-03 11:10:36.384627 opentps_gui-1.0.5/opentps/gui/res/icons/color-adjustment.png
+-rw-r--r--   0        0        0      811 2023-04-03 11:10:36.384627 opentps_gui-1.0.5/opentps/gui/res/icons/color.png
+-rw-r--r--   0        0        0     1921 2023-04-03 11:10:36.384627 opentps_gui-1.0.5/opentps/gui/res/icons/colormap_histogram.png
+-rw-r--r--   0        0        0      618 2023-04-03 11:10:36.385627 opentps_gui-1.0.5/opentps/gui/res/icons/colormap_jet.png
+-rw-r--r--   0        0        0      678 2023-04-03 11:10:36.385627 opentps_gui-1.0.5/opentps/gui/res/icons/contrast.png
+-rw-r--r--   0        0        0     8956 2023-04-03 11:10:36.385627 opentps_gui-1.0.5/opentps/gui/res/icons/crop.png
+-rw-r--r--   0        0        0      544 2023-04-03 11:10:36.386627 opentps_gui-1.0.5/opentps/gui/res/icons/cross.png
+-rw-r--r--   0        0        0     1752 2023-04-03 11:10:36.386627 opentps_gui-1.0.5/opentps/gui/res/icons/cube.png
+-rw-r--r--   0        0        0      507 2023-04-03 11:10:36.387627 opentps_gui-1.0.5/opentps/gui/res/icons/disk.png
+-rw-r--r--   0        0        0      624 2023-04-03 11:10:36.387627 opentps_gui-1.0.5/opentps/gui/res/icons/dvh.png
+-rw-r--r--   0        0        0      492 2023-04-03 11:10:36.387627 opentps_gui-1.0.5/opentps/gui/res/icons/equalizer.png
+-rw-r--r--   0        0        0     4048 2023-04-03 11:10:36.388626 opentps_gui-1.0.5/opentps/gui/res/icons/fast.png
+-rw-r--r--   0        0        0      647 2023-04-03 11:10:36.389625 opentps_gui-1.0.5/opentps/gui/res/icons/folder-open.png
+-rw-r--r--   0        0        0      450 2023-04-03 11:10:36.390654 opentps_gui-1.0.5/opentps/gui/res/icons/geolocation.png
+-rw-r--r--   0        0        0     6608 2023-04-03 11:10:36.390654 opentps_gui-1.0.5/opentps/gui/res/icons/graph.png
+-rw-r--r--   0        0        0     5284 2023-04-03 11:10:36.391627 opentps_gui-1.0.5/opentps/gui/res/icons/iba_nozzle.stl
+-rw-r--r--   0        0        0     2502 2023-04-03 11:10:36.392670 opentps_gui-1.0.5/opentps/gui/res/icons/independent_views.png
+-rw-r--r--   0        0        0    15788 2023-04-03 11:10:36.381627 opentps_gui-1.0.5/opentps/gui/res/icons/OpenTPS_icon.png
+-rw-r--r--   0        0        0    17284 2023-04-03 11:10:36.392670 opentps_gui-1.0.5/opentps/gui/res/icons/pause.jpg
+-rw-r--r--   0        0        0     1637 2023-04-03 11:10:36.392670 opentps_gui-1.0.5/opentps/gui/res/icons/pencil--plus.png
+-rw-r--r--   0        0        0    24904 2023-04-03 11:10:36.393624 opentps_gui-1.0.5/opentps/gui/res/icons/play.png
+-rw-r--r--   0        0        0      730 2023-04-03 11:10:36.394624 opentps_gui-1.0.5/opentps/gui/res/icons/profile.png
+-rw-r--r--   0        0        0    16231 2023-04-03 11:10:36.394624 opentps_gui-1.0.5/opentps/gui/res/icons/reload.png
+-rw-r--r--   0        0        0     1872 2023-04-03 11:10:36.395626 opentps_gui-1.0.5/opentps/gui/res/icons/resample.png
+-rw-r--r--   0        0        0    10339 2023-04-03 11:10:36.395626 opentps_gui-1.0.5/opentps/gui/res/icons/save.png
+-rw-r--r--   0        0        0      503 2023-04-03 11:10:36.395626 opentps_gui-1.0.5/opentps/gui/res/icons/settings-5-line.png
+-rw-r--r--   0        0        0     4110 2023-04-03 11:10:36.396625 opentps_gui-1.0.5/opentps/gui/res/icons/slider.png
+-rw-r--r--   0        0        0     4117 2023-04-03 11:10:36.396625 opentps_gui-1.0.5/opentps/gui/res/icons/slow.png
+-rw-r--r--   0        0        0      605 2023-04-03 11:10:36.396625 opentps_gui-1.0.5/opentps/gui/res/icons/tick-button.png
+-rw-r--r--   0        0        0      859 2023-04-03 11:10:36.397624 opentps_gui-1.0.5/opentps/gui/res/icons/x-ray.png
+-rw-r--r--   0        0        0    73684 2023-04-03 11:10:36.398624 opentps_gui-1.0.5/opentps/gui/res/viewer/human_standing.stl
+-rw-r--r--   0        0        0      205 2023-04-03 11:10:36.398624 opentps_gui-1.0.5/opentps/gui/statusBar.py
+-rw-r--r--   0        0        0      151 2023-04-03 11:10:36.399639 opentps_gui-1.0.5/opentps/gui/tools/__init__.py
+-rw-r--r--   0        0        0    11664 2023-04-03 11:10:36.400624 opentps_gui-1.0.5/opentps/gui/tools/_cropTool.py
+-rw-r--r--   0        0        0     3573 2023-04-03 11:10:36.400624 opentps_gui-1.0.5/opentps/gui/tools/_resampleTool.py
+-rw-r--r--   0        0        0    11328 2023-04-03 11:10:36.401624 opentps_gui-1.0.5/opentps/gui/viewController.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.401624 opentps_gui-1.0.5/opentps/gui/viewer/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-03 11:10:36.402625 opentps_gui-1.0.5/opentps/gui/viewer/dataExplorer.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.403624 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-03 11:10:36.404627 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dataMultiton.py
+-rw-r--r--   0        0        0     2088 2023-04-03 11:10:36.405626 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dyn2DSeqForViewer.py
+-rw-r--r--   0        0        0     2225 2023-04-03 11:10:36.405626 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dyn3DSeqForViewer.py
+-rw-r--r--   0        0        0     3380 2023-04-03 11:10:36.406625 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/genericImageForViewer.py
+-rw-r--r--   0        0        0     3020 2023-04-03 11:10:36.407625 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/image2DForViewer.py
+-rw-r--r--   0        0        0     1763 2023-04-03 11:10:36.408624 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/image3DForViewer.py
+-rw-r--r--   0        0        0      462 2023-04-03 11:10:36.408624 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/polyDataForViewer.py
+-rw-r--r--   0        0        0     2472 2023-04-03 11:10:36.402625 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/ROIContourForViewer.py
+-rw-r--r--   0        0        0     2490 2023-04-03 11:10:36.403624 opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/ROIMaskForViewer.py
+-rw-r--r--   0        0        0    28288 2023-04-03 11:10:36.409656 opentps_gui-1.0.5/opentps/gui/viewer/dataViewer.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.409656 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-03 11:10:36.410624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/blackEmptyPlot.py
+-rw-r--r--   0        0        0     3694 2023-04-03 11:10:36.410624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dataViewerToolbar.py
+-rw-r--r--   0        0        0     3585 2023-04-03 11:10:36.411661 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/doseComparisonImageProvider.py
+-rw-r--r--   0        0        0    12171 2023-04-03 11:10:36.411661 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dvhPlot.py
+-rw-r--r--   0        0        0     1444 2023-04-03 11:10:36.412624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dvhViewerActions.py
+-rw-r--r--   0        0        0     1916 2023-04-03 11:10:36.412624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dynamicImage2DViewer.py
+-rw-r--r--   0        0        0     1847 2023-04-03 11:10:36.412624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dynamicImage3DViewer.py
+-rw-r--r--   0        0        0    18422 2023-04-03 11:10:36.413624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image2DViewer.py
+-rw-r--r--   0        0        0    19280 2023-04-03 11:10:36.413624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image3DViewer.py
+-rw-r--r--   0        0        0     5882 2023-04-03 11:10:36.413624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image3DViewer_3D.py
+-rw-r--r--   0        0        0     4071 2023-04-03 11:10:36.414624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageFusionPropEditor.py
+-rw-r--r--   0        0        0     9907 2023-04-03 11:10:36.414624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerActions.py
+-rw-r--r--   0        0        0        0 2023-04-03 11:10:36.415624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/__init__.py
+-rw-r--r--   0        0        0     6758 2023-04-03 11:10:36.415624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/contourLayer.py
+-rw-r--r--   0        0        0     4322 2023-04-03 11:10:36.416624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/contourLayer_3D.py
+-rw-r--r--   0        0        0     2471 2023-04-03 11:10:36.416624 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/crossHairLayer.py
+-rw-r--r--   0        0        0     6093 2023-04-03 11:10:36.417626 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/lookupTables.py
+-rw-r--r--   0        0        0     2670 2023-04-03 11:10:36.417626 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/polyData3DLayer_3D.py
+-rw-r--r--   0        0        0     5085 2023-04-03 11:10:36.418626 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage2DLayer.py
+-rw-r--r--   0        0        0     5006 2023-04-03 11:10:36.418626 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer.py
+-rw-r--r--   0        0        0     3289 2023-04-03 11:10:36.418626 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer_3D.py
+-rw-r--r--   0        0        0     5073 2023-04-03 11:10:36.419625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtPlanLayer.py
+-rw-r--r--   0        0        0     2996 2023-04-03 11:10:36.419625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtplanLayer_3D.py
+-rw-r--r--   0        0        0     3259 2023-04-03 11:10:36.420628 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage2DLayer.py
+-rw-r--r--   0        0        0     3183 2023-04-03 11:10:36.420628 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer.py
+-rw-r--r--   0        0        0     1454 2023-04-03 11:10:36.421627 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer_3D.py
+-rw-r--r--   0        0        0     2612 2023-04-03 11:10:36.422625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/textLayer.py
+-rw-r--r--   0        0        0     2710 2023-04-03 11:10:36.422625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/patientDataPropertyEditor.py
+-rw-r--r--   0        0        0     6088 2023-04-03 11:10:36.423625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/profileViewer.py
+-rw-r--r--   0        0        0     7434 2023-04-03 11:10:36.423625 opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/profileWidget.py
+-rw-r--r--   0        0        0     4058 2023-04-03 11:10:36.424624 opentps_gui-1.0.5/opentps/gui/viewer/doseComparisonDataViewer.py
+-rw-r--r--   0        0        0     4902 2023-04-03 11:10:36.425624 opentps_gui-1.0.5/opentps/gui/viewer/dynamicDisplayController.py
+-rw-r--r--   0        0        0     3437 2023-04-03 11:10:36.425624 opentps_gui-1.0.5/opentps/gui/viewer/exportWindow.py
+-rw-r--r--   0        0        0      593 2023-04-03 11:10:36.426624 opentps_gui-1.0.5/opentps/gui/viewer/grid.py
+-rw-r--r--   0        0        0     7915 2023-04-03 11:10:36.426624 opentps_gui-1.0.5/opentps/gui/viewer/gridFourElements.py
+-rw-r--r--   0        0        0     3973 2023-04-03 11:10:36.427631 opentps_gui-1.0.5/opentps/gui/viewer/viewerPanel.py
+-rw-r--r--   0        0        0    12950 2023-04-03 11:10:36.427631 opentps_gui-1.0.5/opentps/gui/viewer/viewerToolbar.py
+-rw-r--r--   0        0        0     1098 2023-07-20 18:20:26.824445 opentps_gui-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1358 2023-07-05 13:26:04.959278 opentps_gui-1.0.5/README.md
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 opentps_gui-1.0.5/PKG-INFO
```

### Comparing `opentps-gui-1.0.4/LICENSE` & `opentps_gui-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-The OpenTPS-gui software has been developed by the OpenTPS consortium initiated by researchers from UCLouvain (Louvain-la-Neuve, Belgium) and IBA s.a. (Louvain-la-Neuve, Belgium).
-Each use of this software must be attributed to the OpenTPS consortium (http://opentps.org/).
-The OpenTPS-gui software is released under the terms of the GPLv3 license. Anyone can use or modify the code provided that the GPLv3 license conditions are met. See the GPLv3 license for more details https://www.gnu.org/licenses/licenses.html
-The OpenTPS-gui software is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
+The OpenTPS-gui software has been developed by the OpenTPS consortium initiated by researchers from UCLouvain (Louvain-la-Neuve, Belgium) and IBA s.a. (Louvain-la-Neuve, Belgium).
+Each use of this software must be attributed to the OpenTPS consortium (http://opentps.org/).
+The OpenTPS-gui software is released under the terms of the GPLv3 license. Anyone can use or modify the code provided that the GPLv3 license conditions are met. See the GPLv3 license for more details https://www.gnu.org/licenses/licenses.html
+The OpenTPS-gui software is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+
```

### Comparing `opentps-gui-1.0.4/README.md` & `opentps_gui-1.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-# opentps-gui
-
-GUI of opentps, a Python application for treatment planning in proton therapy, based on the MCsquare Monte Carlo dose engine.
-
-
-## Installation (Linux):
-Requirements are listed in pyproject.toml.
-To install all required dependencies:
-``` 
-poetry install
-``` 
-
-Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
-
-
-## Installation (Windows):
-Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
-
-1) Install anaconda on your Windows computer
-
-2) Open Anaconda Prompt (via the Anaconda application)
-
-3) Create a new Anaconda environment:
-``` 
-conda create --name OpenTPS python=3.8
-``` 
-
-4) Activate the new environment:
-``` 
-conda activate OpenTPS
-``` 
-
-5) Install the following python modules:
-Python modules:
-``` 
-pip3 install --upgrade --user pip
-pip3 install --user pydicom
-pip3 install --user numpy
-pip3 install --user scipy
-pip3 install --user matplotlib
-pip3 install --user Pillow
-pip3 install --user PyQt5==5.14
-pip3 install --user pyqtgraph
-pip3 install --user sparse_dot_mkl
-pip3 install --user vtk
-pip3 install --user SimpleITK
-pip3 install --user pandas
-pip3
-```
-
-Optional python modules:
-``` 
-pip3 install --user tensorflow
-pip3 install --user keras
-pip3 install --user cupy
-```
-
-
-## Run:
-```
-python3 main.py
-```
-
-or from a python script:
-
-```python
-import opentps.gui as opentps_gui
-opentps_gui.run()
-```
-
+# opentps-gui
+
+GUI of opentps, a Python application for treatment planning in proton therapy, based on the MCsquare Monte Carlo dose engine.
+
+## Installation (Linux):
+
+Requirements are listed in pyproject.toml.
+To install all required dependencies:
+
+```
+poetry install
+```
+
+Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
+
+## Installation (Windows):
+
+Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
+
+1. Install anaconda on your Windows computer
+
+2. Open Anaconda Prompt (via the Anaconda application)
+
+3. Create a new Anaconda environment:
+
+```
+conda create --name OpenTPS python=3.8
+```
+
+4. Activate the new environment:
+
+```
+conda activate OpenTPS
+```
+
+5. Install the following python modules:
+   Python modules:
+
+```
+pip3 install --upgrade pip
+pip3 install pydicom
+pip3 install numpy
+pip3 install scipy
+pip3 install matplotlib
+pip3 install Pillow
+pip3 install PyQt5==5.15.7
+pip3 install pyqtgraph
+pip3 install sparse_dot_mkl
+pip3 install vtk
+pip3 install SimpleITK
+pip3 install pandas
+pip3
+```
+
+Optional python modules:
+
+```
+pip3 install tensorflow
+pip3 install keras
+pip3 install cupy
+```
+
+## Run:
+
+```
+python3 main.py
+```
+
+or from a python script:
+
+```python
+import opentps.gui as opentps_gui
+opentps_gui.run()
+```
```

### Comparing `opentps-gui-1.0.4/opentps/gui/mainWindow.py` & `opentps_gui-1.0.5/opentps/gui/mainWindow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-
-import os
-from PyQt5.QtWidgets import QMainWindow, QHBoxLayout, QWidget
-from PyQt5.QtGui import QIcon
-
-from opentps.gui.panels.mainToolbar import MainToolbar
-from opentps.gui.viewer.viewerPanel import ViewerPanel
-from opentps.gui.programSettingEditor import ProgramSettingEditor
-from opentps.gui.statusBar import StatusBar
-from opentps.core.utils.programSettings import ProgramSettings
-import opentps.gui.res.icons as IconModule
-
-class MainWindow(QMainWindow):
-    def __init__(self, viewControler):
-        QMainWindow.__init__(self)
-
-        self.setWindowTitle('OpenTPS')
-        self.setWindowIcon(QIcon(IconModule.__path__[0] + os.path.sep + 'OpenTPS_icon.png'))
-        self.resize(1400, 920)
-
-        centralWidget = QWidget()
-        self.setCentralWidget(centralWidget)
-        self.mainLayout = QHBoxLayout()  ## not sure the "self" is necessary for mainLayout, it shoudnt be called outside this constructor
-        centralWidget.setLayout(self.mainLayout)
-
-        self._viewControler = viewControler
-
-        # create and add the tool panel on the left
-        self.toolbox_width = 270
-        self.mainToolbar = MainToolbar(self._viewControler)
-        self.mainToolbar.setFixedWidth(self.toolbox_width)
-        self.mainLayout.addWidget(self.mainToolbar)
-
-        ProgramSettingEditor.setProgramSettings(ProgramSettings())
-        ProgramSettingEditor.setMainToolbar(self.mainToolbar)
-
-        # create and add the viewer panel
-        self.viewerPanel = ViewerPanel(self._viewControler, self)
-        self.mainLayout.addWidget(self.viewerPanel)
-
-        self.statusBar = StatusBar()
-        self.setStatusBar(self.statusBar)
-        self.statusBar.show()
-
-    def setLateralToolbar(self, toolbar):
-        self.mainLayout.addWidget(toolbar)
-        toolbar.setFixedWidth(self.toolbox_width)
-
-    def setMainPanel(self, mainPanel):
-        self.mainLayout.addWidget(mainPanel)
+
+import os
+from PyQt5.QtWidgets import QMainWindow, QHBoxLayout, QWidget
+from PyQt5.QtGui import QIcon
+
+from opentps.gui.panels.mainToolbar import MainToolbar
+from opentps.gui.viewer.viewerPanel import ViewerPanel
+from opentps.gui.programSettingEditor import ProgramSettingEditor
+from opentps.gui.statusBar import StatusBar
+from opentps.core.utils.programSettings import ProgramSettings
+import opentps.gui.res.icons as IconModule
+
+class MainWindow(QMainWindow):
+    def __init__(self, viewControler):
+        QMainWindow.__init__(self)
+
+        self.setWindowTitle('OpenTPS')
+        self.setWindowIcon(QIcon(IconModule.__path__[0] + os.path.sep + 'OpenTPS_icon.png'))
+        self.resize(1400, 920)
+
+        centralWidget = QWidget()
+        self.setCentralWidget(centralWidget)
+        self.mainLayout = QHBoxLayout()  ## not sure the "self" is necessary for mainLayout, it shoudnt be called outside this constructor
+        centralWidget.setLayout(self.mainLayout)
+
+        self._viewControler = viewControler
+
+        # create and add the tool panel on the left
+        self.toolbox_width = 270
+        self.mainToolbar = MainToolbar(self._viewControler)
+        self.mainToolbar.setFixedWidth(self.toolbox_width)
+        self.mainLayout.addWidget(self.mainToolbar)
+
+        ProgramSettingEditor.setProgramSettings(ProgramSettings())
+        ProgramSettingEditor.setMainToolbar(self.mainToolbar)
+
+        # create and add the viewer panel
+        self.viewerPanel = ViewerPanel(self._viewControler, self)
+        self.mainLayout.addWidget(self.viewerPanel)
+
+        self.statusBar = StatusBar()
+        self.setStatusBar(self.statusBar)
+        self.statusBar.show()
+
+    @property
+    def viewController(self):
+        return self._viewControler
+
+    def closeEvent(self, QCloseEvent):
+        self.viewerPanel.close()
+        super().closeEvent(QCloseEvent)
+
+
+    def setLateralToolbar(self, toolbar):
+        self.mainLayout.addWidget(toolbar)
+        toolbar.setFixedWidth(self.toolbox_width)
+
+    def setMainPanel(self, mainPanel):
+        self.mainLayout.addWidget(mainPanel)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/breathingSignalPanel.py` & `opentps_gui-1.0.5/opentps/gui/panels/breathingSignalPanel.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-from PyQt5.QtWidgets import QWidget,QVBoxLayout,QPushButton, QGridLayout,QLabel,QDoubleSpinBox, QSpinBox, QComboBox
-import pyqtgraph as pg
-
-from opentps.core.processing.deformableDataAugmentationToolBox.BreathingSignalGeneration import signalGeneration
-from PyQt5.QtCore import Qt
-class BreathingSignalPanel(QWidget):
-    
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-        
-        self._viewController = viewController
-        
-        self.layout = QVBoxLayout()
-        self.layout.setContentsMargins(0, 0, 0, 0)
-        self.setLayout(self.layout)
-        
-        self.Breath_param = {"Period": "", "Amplitude": "", "Duration": "", 
-                             "Step": "", "Variance": "", "Mean": "", "ROI": "",
-                             "nbrImage": "", "Way": ""}
-        self.default_param = {"Period": 3.5, "Amplitude": 10.0, "Duration": 120, 
-                             "Step": 0.2, "Variance": 0.0, "Mean": 0, 
-                             "nbrImage": 3}
-
-        self.layout.addWidget(QLabel('<b>Period:</b>'))
-        self.TimePeriod = QDoubleSpinBox()
-        self.TimePeriod.setGroupSeparatorShown(True)
-        self.TimePeriod.setRange(0.0, 10.0)
-        self.TimePeriod.setSingleStep(0.1)
-        self.TimePeriod.setValue(self.default_param["Period"])
-        self.TimePeriod.setSuffix(" seconds")
-        self.TimePeriod.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.TimePeriod)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>Amplitude:</b>'))
-        self.Amplitude = QDoubleSpinBox()
-        self.Amplitude.setGroupSeparatorShown(True)
-        self.Amplitude.setRange(0.0, 30.0)
-        self.Amplitude.setSingleStep(0.5)
-        self.Amplitude.setValue(self.default_param["Amplitude"])
-        self.Amplitude.setSuffix(" millimeter")
-        self.Amplitude.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.Amplitude)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>Duration:</b>'))
-        self.Duration = QSpinBox()
-        self.Duration.setGroupSeparatorShown(True)
-        self.Duration.setRange(0, 600)
-        self.Duration.setSingleStep(30)
-        self.Duration.setValue(self.default_param["Duration"])
-        self.Duration.setSuffix(" seconds")
-        self.Duration.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.Duration)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>Step size:</b>'))
-        self.Step = QDoubleSpinBox()
-        self.Step.setGroupSeparatorShown(True)
-        self.Step.setRange(0.0, 1.0)
-        self.Step.setSingleStep(0.05)
-        self.Step.setValue(self.default_param["Step"])
-        self.Step.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.Step)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>Noise:</b>'))
-        self.layout.addWidget(QLabel('Variance:'))
-        self.Variance = QDoubleSpinBox()
-        self.Variance.setGroupSeparatorShown(True)
-        self.Variance.setRange(0.0, 10.0)
-        self.Variance.setSingleStep(0.1)
-        self.Variance.setValue(self.default_param["Variance"])
-        self.Variance.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.Variance)
-        self.layout.addWidget(QLabel('Mean:'))
-        self.Mean = QSpinBox()
-        self.Mean.setGroupSeparatorShown(True)
-        self.Mean.setRange(0, 100)
-        self.Mean.setSingleStep(1)
-        self.Mean.setValue(self.default_param["Mean"])
-        self.Mean.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.Mean)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>ROI:</b>'))
-        self.ROI = QComboBox()
-        #self.ROI.setMaximumWidth(self.toolbox_width-18)
-        self.ROI.currentIndexChanged.connect(self.Update_Breath_param)
-        #self.ROI.addItems(["None"])
-        self.layout.addWidget(self.ROI)
-        self.layout.addSpacing(15)
-        self.ROI_loaded = 0
-        
-        self.layout.addWidget(QLabel('<b>Number of images:</b>'))
-        self.nbrImage = QSpinBox()
-        self.nbrImage.setGroupSeparatorShown(True)
-        self.nbrImage.setRange(0, 10)
-        self.nbrImage.setSingleStep(1)
-        self.nbrImage.setValue(self.default_param["nbrImage"])
-        self.nbrImage.valueChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.nbrImage)
-        self.layout.addSpacing(15)
-        
-        self.layout.addWidget(QLabel('<b>Way:</b>'))
-        self.way = QComboBox()
-        #self.way.setMaximumWidth(self.toolbox_width-18)
-        self.way.addItems(["Normal", "Random"])
-        self.way.currentIndexChanged.connect(self.Update_Breath_param)
-        self.layout.addWidget(self.way)
-        self.layout.addSpacing(15)
-        
-        
-        #self.Roi_name()#None if we do not load patient data
-        #self.Update_Breath_param#in the case where we do not change the default values
-        
-        self.newSignalButton = QPushButton('Signal generation')
-        self.layout.addWidget(self.newSignalButton)
-        self.newSignalButton.clicked.connect(self.signalGeneration)
-        
-        self.layout.addStretch()
-        
-        self.xOnClick = 0
-        self.yOnClick = 0
-
-        
-    def signalGeneration(self):       
-        A = self.Amplitude.value() #amplitude (mm)
-        dA = 5 #variation d amplitude possible (mm)
-        T = self.TimePeriod.value() #periode respiratoire (s)
-        df = 0.5 #variation de frequence possible (Hz)
-        dS = 5 #shift du signal (mm)
-        mean = self.Mean.value()
-        sigma = self.Variance.value()
-        step = self.Step.value() #periode d echantillonnage
-        Tend = self.Duration.value() #temps de simulation
-        L = 2/30 #moyenne des evenements aleatoires
-        
-        self.t,self.y = signalGeneration(A, dA, T, df, dS, mean, sigma, step, Tend, L)
-        
-        self.widget = QWidget()
-        self.layout = QGridLayout()
-        self.widget.setLayout(self.layout)
-        self.coordSown = QLabel()
-        self.graphWidget = pg.plot()#pg.GraphicsLayoutWidget()
-        #self.graphWidget.showGrid(x = True, y = True)
-        
-        self.widget.setWindowTitle('Display the breathing signal')
-        self.graphWidget.setBackground('w')
-        self.widget.resize(1000, 1000) 
-        cursor = Qt.CrossCursor
-        self.graphWidget.setCursor(cursor)
-        """
-        self.plot_item = self.graphWidget.addPlot(title = "Breathing signal")
-        self.plot_item.setLabel("left", 'Amplitude', units = 'mm')
-        self.plot_item.setLabel("bottom", 'Time', units = 's')
-        curve = self.plot_item.plot()
-        curve.setData(self.t,self.y)
-
-        """
-        self.graphWidget.setLabel("left", 'Amplitude', units = 'mm')
-        self.graphWidget.setLabel("bottom", 'Time', units = 's')
-        self.graphWidget.setTitle("Breathing signal")
-        self.graphWidget.plot(self.t,self.y)
-        
-        
-        self.coordSown.setText("x={:.1f}".format(self.xOnClick) + ", " + "y={:.1f}".format(self.yOnClick))
-        self.layout.addWidget(self.coordSown, 0, 0,1,2)
-        self.layout.addWidget(self.graphWidget, 1, 0)
-        
-        self.graphWidget.scene().sigMouseClicked.connect(self.onClick)
-        
-        # buttons
-        self.ButtonLayout = QGridLayout()
-        
-        self.ValidateButton = QPushButton('OK')
-        self.ValidateButton.clicked.connect(self.acceptFunct)
-        self.ButtonLayout.addWidget(self.ValidateButton, 1, 0)
-        
-        self.RefreshButton = QPushButton('Refresh')
-        self.RefreshButton.clicked.connect(self.refreshFunct)
-        self.ButtonLayout.addWidget(self.RefreshButton, 1, 1)
-        
-        self.CancelButton = QPushButton('Cancel')
-        self.CancelButton.clicked.connect(self.rejectFunct)
-        self.ButtonLayout.addWidget(self.CancelButton, 1, 2)
-        
-        self.layout.addLayout(self.ButtonLayout, 2, 0)
-        self.Roi_name()#None if we do not load patient data
-        #self.Update_Breath_param()#in the case where we do not change the default values
-        self.widget.show()
-        
-    def Update_Breath_param(self):
-        self.Breath_param["Period"] = self.TimePeriod.value()
-        self.Breath_param["Amplitude"] = self.Amplitude.value()
-        self.Breath_param["Duration"] = self.Duration.value()
-        self.Breath_param["Step"] = self.Step.value()
-        self.Breath_param["Variance"] = self.Variance.value()
-        self.Breath_param["Mean"] = self.Mean.value()
-        self.Breath_param["ROI"] = self.ROI.currentText()
-        self.Breath_param["nbrImage"] = self.nbrImage.value()
-        self.Breath_param["Way"] = self.way.currentText()
-        #self.Compute_Breath(plot = False
-        #self.Roi_name()
-    def Roi_name(self):
-        if self.ROI_loaded == 0:
-            rts = self._viewController.currentPatient.rtStructs#.name
-            listOfNames = []
-            for i in range(len(rts)):
-                for j in range(len(rts[i].contours)):
-                    listOfNames.append(rts[i].contours[j].name)
-                
-            self.ROI.addItems(listOfNames)
-            self.ROI_loaded = 1
-    
-    def acceptFunct(self):
-        print("Chosen parameters ", self.Breath_param)
-        self.widget.close()
-    
-    def rejectFunct(self):
-        print("Reject breathing signal")
-        self.widget.close()
-        
-    def refreshFunct(self):
-        print("Refresh signal")
-        self.signalGeneration()
-        
-    def onClick(self, event):
-        #print("hello")
-        p = self.graphWidget.plotItem.vb.mapSceneToView(event.scenePos())
-        #p = self.graphWidget.vb.mapSceneToView(event.scenePos())
-        #self.graphWidget.setText("x={:.1f}".format(p.x()))
-        #self.label_y.setText("y={:.1f}".format(p.y()))
-        self.coordSown.setText("x={:.1f}".format(p.x()) + ", " + "y={:.1f}".format(p.y()))
-        #self.graphWidget.plotItem.setText("x={:.1f}".format(p.x()) + ", " + "y={:.1f}".format(p.y()))
-        print(f"x: {p.x()}, y: {p.y()}")
-        self.xOnClick = p.x()
-        self.yOnClick = p.y()
-        
-        
-        
+from PyQt5.QtWidgets import QWidget,QVBoxLayout,QPushButton, QGridLayout,QLabel,QDoubleSpinBox, QSpinBox, QComboBox
+import pyqtgraph as pg
+
+from opentps.core.processing.deformableDataAugmentationToolBox.BreathingSignalGeneration import signalGeneration
+from PyQt5.QtCore import Qt
+class BreathingSignalPanel(QWidget):
+    
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+        
+        self._viewController = viewController
+        
+        self.layout = QVBoxLayout()
+        self.layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(self.layout)
+        
+        self.Breath_param = {"Period": "", "Amplitude": "", "Duration": "", 
+                             "Step": "", "Variance": "", "Mean": "", "ROI": "",
+                             "nbrImage": "", "Way": ""}
+        self.default_param = {"Period": 3.5, "Amplitude": 10.0, "Duration": 120, 
+                             "Step": 0.2, "Variance": 0.0, "Mean": 0, 
+                             "nbrImage": 3}
+
+        self.layout.addWidget(QLabel('<b>Period:</b>'))
+        self.TimePeriod = QDoubleSpinBox()
+        self.TimePeriod.setGroupSeparatorShown(True)
+        self.TimePeriod.setRange(0.0, 10.0)
+        self.TimePeriod.setSingleStep(0.1)
+        self.TimePeriod.setValue(self.default_param["Period"])
+        self.TimePeriod.setSuffix(" seconds")
+        self.TimePeriod.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.TimePeriod)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>Amplitude:</b>'))
+        self.Amplitude = QDoubleSpinBox()
+        self.Amplitude.setGroupSeparatorShown(True)
+        self.Amplitude.setRange(0.0, 30.0)
+        self.Amplitude.setSingleStep(0.5)
+        self.Amplitude.setValue(self.default_param["Amplitude"])
+        self.Amplitude.setSuffix(" millimeter")
+        self.Amplitude.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.Amplitude)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>Duration:</b>'))
+        self.Duration = QSpinBox()
+        self.Duration.setGroupSeparatorShown(True)
+        self.Duration.setRange(0, 600)
+        self.Duration.setSingleStep(30)
+        self.Duration.setValue(self.default_param["Duration"])
+        self.Duration.setSuffix(" seconds")
+        self.Duration.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.Duration)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>Step size:</b>'))
+        self.Step = QDoubleSpinBox()
+        self.Step.setGroupSeparatorShown(True)
+        self.Step.setRange(0.0, 1.0)
+        self.Step.setSingleStep(0.05)
+        self.Step.setValue(self.default_param["Step"])
+        self.Step.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.Step)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>Noise:</b>'))
+        self.layout.addWidget(QLabel('Variance:'))
+        self.Variance = QDoubleSpinBox()
+        self.Variance.setGroupSeparatorShown(True)
+        self.Variance.setRange(0.0, 10.0)
+        self.Variance.setSingleStep(0.1)
+        self.Variance.setValue(self.default_param["Variance"])
+        self.Variance.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.Variance)
+        self.layout.addWidget(QLabel('Mean:'))
+        self.Mean = QSpinBox()
+        self.Mean.setGroupSeparatorShown(True)
+        self.Mean.setRange(0, 100)
+        self.Mean.setSingleStep(1)
+        self.Mean.setValue(self.default_param["Mean"])
+        self.Mean.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.Mean)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>ROI:</b>'))
+        self.ROI = QComboBox()
+        #self.ROI.setMaximumWidth(self.toolbox_width-18)
+        self.ROI.currentIndexChanged.connect(self.Update_Breath_param)
+        #self.ROI.addItems(["None"])
+        self.layout.addWidget(self.ROI)
+        self.layout.addSpacing(15)
+        self.ROI_loaded = 0
+        
+        self.layout.addWidget(QLabel('<b>Number of images:</b>'))
+        self.nbrImage = QSpinBox()
+        self.nbrImage.setGroupSeparatorShown(True)
+        self.nbrImage.setRange(0, 10)
+        self.nbrImage.setSingleStep(1)
+        self.nbrImage.setValue(self.default_param["nbrImage"])
+        self.nbrImage.valueChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.nbrImage)
+        self.layout.addSpacing(15)
+        
+        self.layout.addWidget(QLabel('<b>Way:</b>'))
+        self.way = QComboBox()
+        #self.way.setMaximumWidth(self.toolbox_width-18)
+        self.way.addItems(["Normal", "Random"])
+        self.way.currentIndexChanged.connect(self.Update_Breath_param)
+        self.layout.addWidget(self.way)
+        self.layout.addSpacing(15)
+        
+        
+        #self.Roi_name()#None if we do not load patient data
+        #self.Update_Breath_param#in the case where we do not change the default values
+        
+        self.newSignalButton = QPushButton('Signal generation')
+        self.layout.addWidget(self.newSignalButton)
+        self.newSignalButton.clicked.connect(self.signalGeneration)
+        
+        self.layout.addStretch()
+        
+        self.xOnClick = 0
+        self.yOnClick = 0
+
+        
+    def signalGeneration(self):       
+        A = self.Amplitude.value() #amplitude (mm)
+        dA = 5 #variation d amplitude possible (mm)
+        T = self.TimePeriod.value() #periode respiratoire (s)
+        df = 0.5 #variation de frequence possible (Hz)
+        dS = 5 #shift du signal (mm)
+        mean = self.Mean.value()
+        sigma = self.Variance.value()
+        step = self.Step.value() #periode d echantillonnage
+        Tend = self.Duration.value() #temps de simulation
+        L = 2/30 #moyenne des evenements aleatoires
+        
+        self.t,self.y = signalGeneration(A, dA, T, df, dS, mean, sigma, step, Tend, L)
+        
+        self.widget = QWidget()
+        self.layout = QGridLayout()
+        self.widget.setLayout(self.layout)
+        self.coordSown = QLabel()
+        self.graphWidget = pg.plot()#pg.GraphicsLayoutWidget()
+        #self.graphWidget.showGrid(x = True, y = True)
+        
+        self.widget.setWindowTitle('Display the breathing signal')
+        self.graphWidget.setBackground('w')
+        self.widget.resize(1000, 1000) 
+        cursor = Qt.CrossCursor
+        self.graphWidget.setCursor(cursor)
+        """
+        self.plot_item = self.graphWidget.addPlot(title = "Breathing signal")
+        self.plot_item.setLabel("left", 'Amplitude', units = 'mm')
+        self.plot_item.setLabel("bottom", 'Time', units = 's')
+        curve = self.plot_item.plot()
+        curve.setData(self.t,self.y)
+
+        """
+        self.graphWidget.setLabel("left", 'Amplitude', units = 'mm')
+        self.graphWidget.setLabel("bottom", 'Time', units = 's')
+        self.graphWidget.setTitle("Breathing signal")
+        self.graphWidget.plot(self.t,self.y)
+        
+        
+        self.coordSown.setText("x={:.1f}".format(self.xOnClick) + ", " + "y={:.1f}".format(self.yOnClick))
+        self.layout.addWidget(self.coordSown, 0, 0,1,2)
+        self.layout.addWidget(self.graphWidget, 1, 0)
+        
+        self.graphWidget.scene().sigMouseClicked.connect(self.onClick)
+        
+        # buttons
+        self.ButtonLayout = QGridLayout()
+        
+        self.ValidateButton = QPushButton('OK')
+        self.ValidateButton.clicked.connect(self.acceptFunct)
+        self.ButtonLayout.addWidget(self.ValidateButton, 1, 0)
+        
+        self.RefreshButton = QPushButton('Refresh')
+        self.RefreshButton.clicked.connect(self.refreshFunct)
+        self.ButtonLayout.addWidget(self.RefreshButton, 1, 1)
+        
+        self.CancelButton = QPushButton('Cancel')
+        self.CancelButton.clicked.connect(self.rejectFunct)
+        self.ButtonLayout.addWidget(self.CancelButton, 1, 2)
+        
+        self.layout.addLayout(self.ButtonLayout, 2, 0)
+        self.Roi_name()#None if we do not load patient data
+        #self.Update_Breath_param()#in the case where we do not change the default values
+        self.widget.show()
+        
+    def Update_Breath_param(self):
+        self.Breath_param["Period"] = self.TimePeriod.value()
+        self.Breath_param["Amplitude"] = self.Amplitude.value()
+        self.Breath_param["Duration"] = self.Duration.value()
+        self.Breath_param["Step"] = self.Step.value()
+        self.Breath_param["Variance"] = self.Variance.value()
+        self.Breath_param["Mean"] = self.Mean.value()
+        self.Breath_param["ROI"] = self.ROI.currentText()
+        self.Breath_param["nbrImage"] = self.nbrImage.value()
+        self.Breath_param["Way"] = self.way.currentText()
+        #self.Compute_Breath(plot = False
+        #self.Roi_name()
+    def Roi_name(self):
+        if self.ROI_loaded == 0:
+            rts = self._viewController.currentPatient.rtStructs#.name
+            listOfNames = []
+            for i in range(len(rts)):
+                for j in range(len(rts[i].contours)):
+                    listOfNames.append(rts[i].contours[j].name)
+                
+            self.ROI.addItems(listOfNames)
+            self.ROI_loaded = 1
+    
+    def acceptFunct(self):
+        print("Chosen parameters ", self.Breath_param)
+        self.widget.close()
+    
+    def rejectFunct(self):
+        print("Reject breathing signal")
+        self.widget.close()
+        
+    def refreshFunct(self):
+        print("Refresh signal")
+        self.signalGeneration()
+        
+    def onClick(self, event):
+        #print("hello")
+        p = self.graphWidget.plotItem.vb.mapSceneToView(event.scenePos())
+        #p = self.graphWidget.vb.mapSceneToView(event.scenePos())
+        #self.graphWidget.setText("x={:.1f}".format(p.x()))
+        #self.label_y.setText("y={:.1f}".format(p.y()))
+        self.coordSown.setText("x={:.1f}".format(p.x()) + ", " + "y={:.1f}".format(p.y()))
+        #self.graphWidget.plotItem.setText("x={:.1f}".format(p.x()) + ", " + "y={:.1f}".format(p.y()))
+        print(f"x: {p.x()}, y: {p.y()}")
+        self.xOnClick = p.x()
+        self.yOnClick = p.y()
+        
+        
+
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/drrPanel.py` & `opentps_gui-1.0.5/opentps/gui/panels/drrPanel.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-from PyQt5.QtGui import QImage, QPixmap, QPainter, QPalette, QBrush, QPolygon
-from PyQt5.QtCore import QPoint
-import numpy as np
-import math
-
-
-from PyQt5.QtWidgets import *
-from PyQt5.QtCore import Qt, QDir#, pyqtSignal
-from opentps.core import createDRRDynamic2DSequences
-
-
-
-class DRRPanel(QWidget):
-
-    # fluoroSeqCreated = pyqtSignal()
-
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-
-        self._viewController = viewController
-        self._viewController.patientAddedSignal.connect(self.refreshDataList)
-
-        self.patients = self._viewController.patientList
-        # self.toolbox_width = toolbox_width
-        self.data_path = QDir.currentPath()
-        self.CT_disp_ID = ""
-
-        self.layout = QVBoxLayout()
-        self.setLayout(self.layout)
-
-        self.imageSelectionBox = QComboBox()
-        # self.refreshDataList(self._viewController.currentPatient)
-
-        self.layout.addWidget(self.imageSelectionBox) ## --> this must changed to a data selection box (self.imageSelectionBox)
-
-
-        self.fluoSimButton = QPushButton('Fluoroscopy simulation')
-        self.layout.addWidget(self.fluoSimButton)
-        self.fluoSimButton.clicked.connect(self.selectProjectionAngles)
-
-    def refreshDataList(self, patient):
-
-        print('in DRRPanel refresh data list ')
-        for data in patient.getPatientDataOfType('CTImage'):
-            name = data.name
-            self.imageSelectionBox.addItem(name, data)
-        for data in patient.getPatientDataOfType('Dynamic3DSequence'):
-            name = data.name
-            self.imageSelectionBox.addItem(name, data)
-
-    """
-    class PatientComboBox(QComboBox):
-    def __init__(self, viewController):
-        QComboBox.__init__(self)
-
-        self._viewController = viewController
-
-        self._viewController.patientAddedSignal.connect(self._addPatient)
-        self._viewController.patientRemovedSignal.connect(self._removePatient)
-
-        self.currentIndexChanged.connect(self._setCurrentPatient)
-
-    def _addPatient(self, patient):
-        name = patient.name
-        if name is None:
-            name = 'None'
-
-        self.addItem(name, patient)
-        if self.count() == 1:
-            self._viewController.currentPatient = patient
-
-    def _removePatient(self, patient):
-        self.removeItem(self.findData(patient))
-
-    def _setCurrentPatient(self, index):
-        self._viewController.currentPatient = self.currentData()
-    """
-
-    def Data_path_changed(self, data_path):
-        self.data_path = data_path
-
-    def selectProjectionAngles(self):
-
-        fluoroAngleDialog = ChoseAngles_dialog(self._viewController.currentPatient.dynamic3DSequences[0].dyn3DImageList[0])
-
-        if (fluoroAngleDialog.exec()):
-
-            anglesAndAxisList = fluoroAngleDialog.anglesList
-            print('in selectProjectionAngles', anglesAndAxisList)
-            print('this should be change to use the currently selected patient and dyn seq if several')
-
-            # fluoroSeq = self.createDRRs(angles, self._viewController.currentPatient.dynamic3DSequences[0].dyn3DImageList, self._viewController.currentPatient)
-
-            print('in drrPanel selectProjectionAngles !!! source image is hard coded for now')
-            sourceImageOrSeq = self._viewController.currentPatient.dynamic3DSequences[0]
-            dyn2DDRRSeqList = createDRRDynamic2DSequences(sourceImageOrSeq, anglesAndAxisList)
-
-            # plt.figure()
-            # plt.imshow(dyn2DDRRSeqList[0].dyn2DImageList[0].imageArray)
-            # plt.show()
-
-            if sourceImageOrSeq.patient != None:
-                for dyn2DSeq in dyn2DDRRSeqList:
-                    sourceImageOrSeq.patient.appendPatientData(dyn2DSeq)
-
-            # self.fluoroSeqCreated.emit()
-            #self.data_path = QFileDialog.getExistingDirectory(self, "Select 4D data folder", self.data_path)
-            #self.Patients.importDyn4DSeq(self.data_path)
-
-            # display Dynamic series
-#             for series in self.Patients.list[0].Dyn2DSeqList:
-#                 if (series.isLoaded == 1):
-#                     serieRoot = StandardItem(txt=series.SequenceName)
-#                     for image in series.dyn2DImageList:
-#                         imageName = StandardItem(txt=image.ImgName)
-#                         serieRoot.appendRow(imageName)
-#                     self.rootNode.appendRow(serieRoot)
-#                     self.treeView.setModel(self.treeModel)
-#                     self.treeView.expandAll()
-#                     self.treeView.clicked.connect(self.getTreeViewValue)
-#
-    # def createDRRs(self, angleList, Dyn4DSeq, patient, orientation='Axial'):
-    #
-    #     try:
-    #         import tomopy
-    #
-    #         for anglesAndOri in angleList:
-    #
-    #             angle = anglesAndOri[0]
-    #             orientation = anglesAndOri[1]
-    #
-    #             fluoroSeq = Dynamic2DSequence()
-    #             fluoroSeq.type = 'Fluoroscopy simulation'
-    #             fluoroSeq.projectionAngle = angle
-    #             fluoroSeq.SequenceName = 'FluoSim_' + anglesAndOri[1] + '_' + str(
-    #                 int(np.round(angle * 360 / (2 * math.pi))))
-    #             for imageIndex, image in enumerate(Dyn4DSeq.dyn3DImageList):
-    #
-    #                 # to rotate around Z axis
-    #                 if orientation == 'Axial':
-    #                     imageToUse = image.Image.transpose(2, 1, 0)
-    #                 if orientation == 'Coronal':
-    #                     imageToUse = image.Image.transpose(1, 2, 0)
-    #                 if orientation == 'Sagittal':
-    #                     imageToUse = image.Image.transpose(0, 2, 1)
-    #
-    #                 print('! ! ! in fluoroscopy_sim --> les orientation et transpose ici sont à vérifier! ! !')
-    #                 fluoSimImage = tomopy.project(imageToUse, angle)[0]
-    #
-    #                 # plt.figure()
-    #                 # plt.imshow(fluoSimImage)
-    #                 # plt.show()
-    #
-    #                 image_2D = image2D()
-    #                 image_2D.Image = fluoSimImage
-    #                 image_2D.ImgName = str(imageIndex + 1)
-    #                 image_2D.PixelSpacing = [1, 1]
-    #                 fluoroSeq.dyn2DImageList.append(image_2D)
-    #                 fluoroSeq.isLoaded = True
-    #
-    #             patient.Dyn2DSeqList.append(fluoroSeq)
-    #
-    #     except:
-    #         print("No module tomopy available")
-# class StandardItem(QStandardItem):
-#   def __init__(self, txt="", fontSize = 12, setBold=False, color=QColor(0,0,0)):
-#     super().__init__()
-#     self.setEditable(False)
-#     self.setForeground(color)
-#     self.setText(txt)
-
-
-
-class ChoseAngles_dialog(QDialog):
-
-    def __init__(self, Image3D):
-
-        # initialize the window
-        QDialog.__init__(self)
-
-        self.main_layout = QGridLayout()
-        self.setLayout(self.main_layout)
-
-        self.infoLabel = QLabel()
-        self.infoLabel.viewer_palette = QPalette()
-        self.infoLabel.viewer_palette.setColor(QPalette.Window, Qt.black)
-        self.infoLabel.setAlignment(Qt.AlignTop)
-        self.infoLabel.setStyleSheet('color: black')
-        self.infoLabelText = ''
-        self.main_layout.addWidget(self.infoLabel, 0, 0)
-
-        self.imageLabel = QLabel()
-        self.imageLabel.setMaximumSize(512, 512)
-        self.imageLabel.setAlignment(Qt.AlignTop)
-        self.main_layout.addWidget(self.imageLabel, 1, 0)
-
-        self.orientation = "Z"
-        self.image3D = self.prepare_image_for_viewer(Image3D.imageArray)
-        self.imageShape = self.image3D.shape
-        self.resolution = Image3D.spacing
-        self.imageCenter = [self.imageLabel.pos().x() + int(self.imageLabel.width() / 2), self.imageLabel.pos().y() + int(self.imageLabel.height() / 2)]
-        print('in ChoseAngles_dialog constructor', self.imageLabel.pos().x())
-        print(self.imageCenter)
-        self.distanceFromSourceToCenter = min(self.imageCenter[0], self.imageCenter[1]) - 10
-        self.pannelWidth = min(self.imageLabel.width(), self.imageLabel.height())
-
-        self.anglesList = []
-
-        self.currentMousePos = QPoint(0, 0)
-        self.angleBetweenMouseAndCenter = 0
-        self.xRaySourcePoint = QPoint(0, 0)
-        self.pannelPoint1 = QPoint(0, 0)
-        self.pannelPoint2 = QPoint(0, 0)
-        self.getPolygonPoints(self.angleBetweenMouseAndCenter)
-        self.colorList = [Qt.cyan, Qt.red, Qt.blue]
-        self.colorList *= 5
-
-        # buttons
-        self.ButtonLayout = QGridLayout()
-        self.AddAngleButton = QPushButton('Add angle')
-        self.AddAngleButton.clicked.connect(self.addAngle)
-        self.ButtonLayout.addWidget(self.AddAngleButton, 1, 0)
-        self.ValidateButton = QPushButton('OK')
-        self.ValidateButton.clicked.connect(self.accept)
-        self.ButtonLayout.addWidget(self.ValidateButton, 1, 1)
-        self.CancelButton = QPushButton('Cancel')
-        self.ButtonLayout.addWidget(self.CancelButton, 1, 2)
-        self.CancelButton.clicked.connect(self.reject)
-        self.XYButton = QPushButton('Z')
-        self.XYButton.clicked.connect(self.changeImageView)
-        self.ButtonLayout.addWidget(self.XYButton, 0, 0)
-        self.YZButton = QPushButton('Y')
-        self.YZButton.clicked.connect(self.changeImageView)
-        self.ButtonLayout.addWidget(self.YZButton, 0, 1)
-        self.XZButton = QPushButton('X')
-        self.XZButton.clicked.connect(self.changeImageView)
-        self.ButtonLayout.addWidget(self.XZButton, 0, 2)
-
-        self.main_layout.addLayout(self.ButtonLayout, 2, 0)
-
-        self.setWindowTitle('Select angles to use for fluoroscopy projections')
-
-        self.selectSlice()
-        self.resize(512, 512)
-        self.update_viewer()
-
-##-----------------------------------------------------------------------------------------------------------
-    def selectSlice(self):
-
-        if self.orientation == 'Z':
-            self.current_sliceIndex = round(self.imageShape[2] / 2)
-            self.sliceToShow = self.image3D[:, :, self.current_sliceIndex].transpose(1,0)
-        elif self.orientation == 'X':
-            self.current_sliceIndex = round(self.imageShape[0] / 2)
-            self.sliceToShow = np.flip(self.image3D[self.current_sliceIndex, :, :].transpose(1,0), 0)
-        elif self.orientation == 'Y':
-            self.current_sliceIndex = round(self.imageShape[1] / 2)
-            self.sliceToShow = np.flip(self.image3D[:, self.current_sliceIndex, :].transpose(1,0), 0)
-
-        self.sliceToShow = np.require(self.sliceToShow, np.uint8, 'C')
-
-
-##-----------------------------------------------------------------------------------------------------------
-    def getPolygonPoints(self, angle):
-
-        print('in get polygon points')
-        print(self.imageCenter)
-        print(self.imageCenter[0] - 2 * (self.distanceFromSourceToCenter * math.sin(angle)))
-        print(self.imageCenter[1] - 2 * (self.distanceFromSourceToCenter * math.cos(angle)))
-
-        self.xRaySourcePoint = QPoint(int(self.imageCenter[0] - 2 * (self.distanceFromSourceToCenter * math.sin(angle))),
-                                      int(self.imageCenter[1] - 2 * (self.distanceFromSourceToCenter * math.cos(angle))))
-        self.pannelPoint1 = QPoint(int(self.imageCenter[0] + (self.distanceFromSourceToCenter * math.sin(angle)) + math.cos(angle)*self.pannelWidth/2),
-                                    int(self.imageCenter[1] + (self.distanceFromSourceToCenter * math.cos(angle)) - math.sin(angle)*self.pannelWidth/2))
-        self.pannelPoint2 = QPoint(int(self.imageCenter[0] + (self.distanceFromSourceToCenter * math.sin(angle)) - math.cos(angle)*self.pannelWidth/2),
-                                      int(self.imageCenter[1] + (self.distanceFromSourceToCenter * math.cos(angle)) + math.sin(angle)*self.pannelWidth/2))
-
-##-----------------------------------------------------------------------------------------------------------
-    def update_viewer(self):
-
-        # calculate scaling factor
-        if self.orientation == 'Z':
-            Yscaling = self.resolution[1] / self.resolution[0]
-        elif self.orientation == 'X':
-            Yscaling = self.resolution[2] / self.resolution[1]
-        elif self.orientation == 'Y':
-            Yscaling = self.resolution[2] / self.resolution[0]
-
-        self.imageCenter = [self.imageLabel.pos()._x() + int(self.imageLabel.width() / 2),
-                            self.imageLabel.pos()._y() + int(self.imageLabel.height() / 2)]
-        self.distanceFromSourceToCenter = min(self.imageCenter[0], self.imageCenter[1]) - 10
-        self.pannelWidth = min(self.imageLabel.width(), self.imageLabel.height())
-
-        imageQT = QImage(self.sliceToShow, self.sliceToShow.shape[1], self.sliceToShow.shape[0], self.sliceToShow.shape[1], QImage.Format_Indexed8)
-        imageQT = imageQT.convertToFormat(QImage.Format_ARGB32)
-        MergedImage = QImage(self.sliceToShow.shape[1], round(self.sliceToShow.shape[0] * Yscaling), QImage.Format_ARGB32)
-        MergedImage.fill(Qt.black)
-        painter = QPainter()
-        painter.begin(MergedImage)
-        painter.scale(1.0, Yscaling)
-        painter.drawImage(0, 0, imageQT)
-
-        for angleIndex, angle in enumerate(self.anglesList):
-            self.draw_polygon(angle[0], angleIndex, painter)
-        self.draw_polygon(self.angleBetweenMouseAndCenter, -1, painter)
-
-        painter.end()
-
-        self.imageLabel.setPixmap(QPixmap.fromImage(MergedImage).scaledToWidth(self.width() - 10, mode=Qt.SmoothTransformation))
-
-##-----------------------------------------------------------------------------------------------------------
-    def addAngle(self):
-        self.anglesList.append([self.angleBetweenMouseAndCenter, self.orientation])
-        self.infoLabelText += 'Angle ' + str(len(self.anglesList)) + ': ' + str(int(np.round(self.anglesList[-1][0]*(360/(2*math.pi))))) + '°' + '\n'
-        self.infoLabel.setText(self.infoLabelText)
-
-##-----------------------------------------------------------------------------------------------------------
-    def draw_polygon(self, angle, angleIndex, painter):
-
-        self.getPolygonPoints(angle)
-        if angleIndex == -1:
-            painter.setBrush(QBrush(Qt.yellow, Qt.Dense6Pattern))
-        else:
-            painter.setBrush(QBrush(self.colorList[angleIndex], Qt.Dense6Pattern))
-
-        polygon = QPolygon([self.pannelPoint1,
-                            self.pannelPoint2,
-                            self.xRaySourcePoint])
-
-        painter.drawPolygon(polygon)
-
-    # def onClicked(self, item):
-    #     print('test onClicked')
-
-    # def onDoubleClick(self, item):
-    #     print('test onDoubleClick')
-
-##-----------------------------------------------------------------------------------------------------------
-    def mouseMoveEvent(self, QMouseEvent):
-        #print('Mouse coords: ( %d : %d )' % (QMouseEvent.x(), QMouseEvent.y()))
-        self.currentMousePos.setX(QMouseEvent._x())
-        self.currentMousePos.setY(QMouseEvent._y())
-        self.getAngleFromMousePosition()
-
-        self.infoLabel.setText(self.infoLabelText + "Current angle : " + str(int(np.round(self.angleBetweenMouseAndCenter*(360/6.28)))) + '°')
-        self.update_viewer()
-
-##-----------------------------------------------------------------------------------------------------------
-    def getAngleFromMousePosition(self):
-
-        if self.imageCenter[1] == self.currentMousePos.y() and self.imageCenter[0] > self.currentMousePos.x():
-            self.angleBetweenMouseAndCenter = math.pi/2
-        elif self.imageCenter[1] == self.currentMousePos.y() and self.imageCenter[0] < self.currentMousePos.x():
-            self.angleBetweenMouseAndCenter = 3 * math.pi / 2
-        elif self.imageCenter[1] < self.currentMousePos.y() and self.imageCenter[0] == self.currentMousePos.x():
-            self.angleBetweenMouseAndCenter = math.pi
-        elif self.imageCenter[1] > self.currentMousePos.y() and self.imageCenter[0] == self.currentMousePos.x():
-            self.angleBetweenMouseAndCenter = 0
-        elif self.imageCenter[0] > self.currentMousePos.x() and self.imageCenter[1] > self.currentMousePos.y():
-            self.angleBetweenMouseAndCenter = math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
-        elif self.imageCenter[0] > self.currentMousePos.x() and self.imageCenter[1] < self.currentMousePos.y():
-            self.angleBetweenMouseAndCenter = math.pi - math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
-        elif self.imageCenter[0] < self.currentMousePos.x() and self.imageCenter[1] < self.currentMousePos.y():
-            self.angleBetweenMouseAndCenter = math.pi + math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
-        elif self.imageCenter[0] < self.currentMousePos.x() and self.imageCenter[1] > self.currentMousePos.y():
-            self.angleBetweenMouseAndCenter = (2 * math.pi) - math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
-
-    ##-----------------------------------------------------------------------------------------------------------
-    def changeImageView(self):
-        self.orientation = self.sender().text()
-        self.selectSlice()
-        self.update_viewer()
-
-    ##-----------------------------------------------------------------------------------------------------------
-    def prepare_image_for_viewer(self, image):
-        img_min = image.min()
-        # img_max = self.Image.max()
-        img_max = np.percentile(image, 99.995)
-        img = 255 * (image.astype(np.float32) - img_min) / (
-                    img_max - img_min + 1e-5)  # normalize data betwee, 0 and 255
-        img[img > 255] = 255
+from PyQt5.QtGui import QImage, QPixmap, QPainter, QPalette, QBrush, QPolygon
+from PyQt5.QtCore import QPoint
+import numpy as np
+import math
+
+
+from PyQt5.QtWidgets import *
+from PyQt5.QtCore import Qt, QDir#, pyqtSignal
+from opentps.core import createDRRDynamic2DSequences
+
+
+
+class DRRPanel(QWidget):
+
+    # fluoroSeqCreated = pyqtSignal()
+
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+
+        self._viewController = viewController
+        self._viewController.patientAddedSignal.connect(self.refreshDataList)
+
+        self.patients = self._viewController.patientList
+        # self.toolbox_width = toolbox_width
+        self.data_path = QDir.currentPath()
+        self.CT_disp_ID = ""
+
+        self.layout = QVBoxLayout()
+        self.setLayout(self.layout)
+
+        self.imageSelectionBox = QComboBox()
+        # self.refreshDataList(self._viewController.currentPatient)
+
+        self.layout.addWidget(self.imageSelectionBox) ## --> this must changed to a data selection box (self.imageSelectionBox)
+
+
+        self.fluoSimButton = QPushButton('Fluoroscopy simulation')
+        self.layout.addWidget(self.fluoSimButton)
+        self.fluoSimButton.clicked.connect(self.selectProjectionAngles)
+
+    def refreshDataList(self, patient):
+
+        print('in DRRPanel refresh data list ')
+        for data in patient.getPatientDataOfType('CTImage'):
+            name = data.name
+            self.imageSelectionBox.addItem(name, data)
+        for data in patient.getPatientDataOfType('Dynamic3DSequence'):
+            name = data.name
+            self.imageSelectionBox.addItem(name, data)
+
+    """
+    class PatientComboBox(QComboBox):
+    def __init__(self, viewController):
+        QComboBox.__init__(self)
+
+        self._viewController = viewController
+
+        self._viewController.patientAddedSignal.connect(self._addPatient)
+        self._viewController.patientRemovedSignal.connect(self._removePatient)
+
+        self.currentIndexChanged.connect(self._setCurrentPatient)
+
+    def _addPatient(self, patient):
+        name = patient.name
+        if name is None:
+            name = 'None'
+
+        self.addItem(name, patient)
+        if self.count() == 1:
+            self._viewController.currentPatient = patient
+
+    def _removePatient(self, patient):
+        self.removeItem(self.findData(patient))
+
+    def _setCurrentPatient(self, index):
+        self._viewController.currentPatient = self.currentData()
+    """
+
+    def Data_path_changed(self, data_path):
+        self.data_path = data_path
+
+    def selectProjectionAngles(self):
+
+        fluoroAngleDialog = ChoseAngles_dialog(self._viewController.currentPatient.dynamic3DSequences[0].dyn3DImageList[0])
+
+        if (fluoroAngleDialog.exec()):
+
+            anglesAndAxisList = fluoroAngleDialog.anglesList
+            print('in selectProjectionAngles', anglesAndAxisList)
+            print('this should be change to use the currently selected patient and dyn seq if several')
+
+            # fluoroSeq = self.createDRRs(angles, self._viewController.currentPatient.dynamic3DSequences[0].dyn3DImageList, self._viewController.currentPatient)
+
+            print('in drrPanel selectProjectionAngles !!! source image is hard coded for now')
+            sourceImageOrSeq = self._viewController.currentPatient.dynamic3DSequences[0]
+            dyn2DDRRSeqList = createDRRDynamic2DSequences(sourceImageOrSeq, anglesAndAxisList)
+
+            # plt.figure()
+            # plt.imshow(dyn2DDRRSeqList[0].dyn2DImageList[0].imageArray)
+            # plt.show()
+
+            if sourceImageOrSeq.patient != None:
+                for dyn2DSeq in dyn2DDRRSeqList:
+                    sourceImageOrSeq.patient.appendPatientData(dyn2DSeq)
+
+            # self.fluoroSeqCreated.emit()
+            #self.data_path = QFileDialog.getExistingDirectory(self, "Select 4D data folder", self.data_path)
+            #self.Patients.importDyn4DSeq(self.data_path)
+
+            # display Dynamic series
+#             for series in self.Patients.list[0].Dyn2DSeqList:
+#                 if (series.isLoaded == 1):
+#                     serieRoot = StandardItem(txt=series.SequenceName)
+#                     for image in series.dyn2DImageList:
+#                         imageName = StandardItem(txt=image.ImgName)
+#                         serieRoot.appendRow(imageName)
+#                     self.rootNode.appendRow(serieRoot)
+#                     self.treeView.setModel(self.treeModel)
+#                     self.treeView.expandAll()
+#                     self.treeView.clicked.connect(self.getTreeViewValue)
+#
+    # def createDRRs(self, angleList, Dyn4DSeq, patient, orientation='Axial'):
+    #
+    #     try:
+    #         import tomopy
+    #
+    #         for anglesAndOri in angleList:
+    #
+    #             angle = anglesAndOri[0]
+    #             orientation = anglesAndOri[1]
+    #
+    #             fluoroSeq = Dynamic2DSequence()
+    #             fluoroSeq.type = 'Fluoroscopy simulation'
+    #             fluoroSeq.projectionAngle = angle
+    #             fluoroSeq.SequenceName = 'FluoSim_' + anglesAndOri[1] + '_' + str(
+    #                 int(np.round(angle * 360 / (2 * math.pi))))
+    #             for imageIndex, image in enumerate(Dyn4DSeq.dyn3DImageList):
+    #
+    #                 # to rotate around Z axis
+    #                 if orientation == 'Axial':
+    #                     imageToUse = image.Image.transpose(2, 1, 0)
+    #                 if orientation == 'Coronal':
+    #                     imageToUse = image.Image.transpose(1, 2, 0)
+    #                 if orientation == 'Sagittal':
+    #                     imageToUse = image.Image.transpose(0, 2, 1)
+    #
+    #                 print('! ! ! in fluoroscopy_sim --> les orientation et transpose ici sont à vérifier! ! !')
+    #                 fluoSimImage = tomopy.project(imageToUse, angle)[0]
+    #
+    #                 # plt.figure()
+    #                 # plt.imshow(fluoSimImage)
+    #                 # plt.show()
+    #
+    #                 image_2D = image2D()
+    #                 image_2D.Image = fluoSimImage
+    #                 image_2D.ImgName = str(imageIndex + 1)
+    #                 image_2D.PixelSpacing = [1, 1]
+    #                 fluoroSeq.dyn2DImageList.append(image_2D)
+    #                 fluoroSeq.isLoaded = True
+    #
+    #             patient.Dyn2DSeqList.append(fluoroSeq)
+    #
+    #     except:
+    #         print("No module tomopy available")
+# class StandardItem(QStandardItem):
+#   def __init__(self, txt="", fontSize = 12, setBold=False, color=QColor(0,0,0)):
+#     super().__init__()
+#     self.setEditable(False)
+#     self.setForeground(color)
+#     self.setText(txt)
+
+
+
+class ChoseAngles_dialog(QDialog):
+
+    def __init__(self, Image3D):
+
+        # initialize the window
+        QDialog.__init__(self)
+
+        self.main_layout = QGridLayout()
+        self.setLayout(self.main_layout)
+
+        self.infoLabel = QLabel()
+        self.infoLabel.viewer_palette = QPalette()
+        self.infoLabel.viewer_palette.setColor(QPalette.Window, Qt.black)
+        self.infoLabel.setAlignment(Qt.AlignTop)
+        self.infoLabel.setStyleSheet('color: black')
+        self.infoLabelText = ''
+        self.main_layout.addWidget(self.infoLabel, 0, 0)
+
+        self.imageLabel = QLabel()
+        self.imageLabel.setMaximumSize(512, 512)
+        self.imageLabel.setAlignment(Qt.AlignTop)
+        self.main_layout.addWidget(self.imageLabel, 1, 0)
+
+        self.orientation = "Z"
+        self.image3D = self.prepare_image_for_viewer(Image3D.imageArray)
+        self.imageShape = self.image3D.shape
+        self.resolution = Image3D.spacing
+        self.imageCenter = [self.imageLabel.pos().x() + int(self.imageLabel.width() / 2), self.imageLabel.pos().y() + int(self.imageLabel.height() / 2)]
+        print('in ChoseAngles_dialog constructor', self.imageLabel.pos().x())
+        print(self.imageCenter)
+        self.distanceFromSourceToCenter = min(self.imageCenter[0], self.imageCenter[1]) - 10
+        self.pannelWidth = min(self.imageLabel.width(), self.imageLabel.height())
+
+        self.anglesList = []
+
+        self.currentMousePos = QPoint(0, 0)
+        self.angleBetweenMouseAndCenter = 0
+        self.xRaySourcePoint = QPoint(0, 0)
+        self.pannelPoint1 = QPoint(0, 0)
+        self.pannelPoint2 = QPoint(0, 0)
+        self.getPolygonPoints(self.angleBetweenMouseAndCenter)
+        self.colorList = [Qt.cyan, Qt.red, Qt.blue]
+        self.colorList *= 5
+
+        # buttons
+        self.ButtonLayout = QGridLayout()
+        self.AddAngleButton = QPushButton('Add angle')
+        self.AddAngleButton.clicked.connect(self.addAngle)
+        self.ButtonLayout.addWidget(self.AddAngleButton, 1, 0)
+        self.ValidateButton = QPushButton('OK')
+        self.ValidateButton.clicked.connect(self.accept)
+        self.ButtonLayout.addWidget(self.ValidateButton, 1, 1)
+        self.CancelButton = QPushButton('Cancel')
+        self.ButtonLayout.addWidget(self.CancelButton, 1, 2)
+        self.CancelButton.clicked.connect(self.reject)
+        self.XYButton = QPushButton('Z')
+        self.XYButton.clicked.connect(self.changeImageView)
+        self.ButtonLayout.addWidget(self.XYButton, 0, 0)
+        self.YZButton = QPushButton('Y')
+        self.YZButton.clicked.connect(self.changeImageView)
+        self.ButtonLayout.addWidget(self.YZButton, 0, 1)
+        self.XZButton = QPushButton('X')
+        self.XZButton.clicked.connect(self.changeImageView)
+        self.ButtonLayout.addWidget(self.XZButton, 0, 2)
+
+        self.main_layout.addLayout(self.ButtonLayout, 2, 0)
+
+        self.setWindowTitle('Select angles to use for fluoroscopy projections')
+
+        self.selectSlice()
+        self.resize(512, 512)
+        self.update_viewer()
+
+##-----------------------------------------------------------------------------------------------------------
+    def selectSlice(self):
+
+        if self.orientation == 'Z':
+            self.current_sliceIndex = round(self.imageShape[2] / 2)
+            self.sliceToShow = self.image3D[:, :, self.current_sliceIndex].transpose(1,0)
+        elif self.orientation == 'X':
+            self.current_sliceIndex = round(self.imageShape[0] / 2)
+            self.sliceToShow = np.flip(self.image3D[self.current_sliceIndex, :, :].transpose(1,0), 0)
+        elif self.orientation == 'Y':
+            self.current_sliceIndex = round(self.imageShape[1] / 2)
+            self.sliceToShow = np.flip(self.image3D[:, self.current_sliceIndex, :].transpose(1,0), 0)
+
+        self.sliceToShow = np.require(self.sliceToShow, np.uint8, 'C')
+
+
+##-----------------------------------------------------------------------------------------------------------
+    def getPolygonPoints(self, angle):
+
+        print('in get polygon points')
+        print(self.imageCenter)
+        print(self.imageCenter[0] - 2 * (self.distanceFromSourceToCenter * math.sin(angle)))
+        print(self.imageCenter[1] - 2 * (self.distanceFromSourceToCenter * math.cos(angle)))
+
+        self.xRaySourcePoint = QPoint(int(self.imageCenter[0] - 2 * (self.distanceFromSourceToCenter * math.sin(angle))),
+                                      int(self.imageCenter[1] - 2 * (self.distanceFromSourceToCenter * math.cos(angle))))
+        self.pannelPoint1 = QPoint(int(self.imageCenter[0] + (self.distanceFromSourceToCenter * math.sin(angle)) + math.cos(angle)*self.pannelWidth/2),
+                                    int(self.imageCenter[1] + (self.distanceFromSourceToCenter * math.cos(angle)) - math.sin(angle)*self.pannelWidth/2))
+        self.pannelPoint2 = QPoint(int(self.imageCenter[0] + (self.distanceFromSourceToCenter * math.sin(angle)) - math.cos(angle)*self.pannelWidth/2),
+                                      int(self.imageCenter[1] + (self.distanceFromSourceToCenter * math.cos(angle)) + math.sin(angle)*self.pannelWidth/2))
+
+##-----------------------------------------------------------------------------------------------------------
+    def update_viewer(self):
+
+        # calculate scaling factor
+        if self.orientation == 'Z':
+            Yscaling = self.resolution[1] / self.resolution[0]
+        elif self.orientation == 'X':
+            Yscaling = self.resolution[2] / self.resolution[1]
+        elif self.orientation == 'Y':
+            Yscaling = self.resolution[2] / self.resolution[0]
+
+        self.imageCenter = [self.imageLabel.pos()._x() + int(self.imageLabel.width() / 2),
+                            self.imageLabel.pos()._y() + int(self.imageLabel.height() / 2)]
+        self.distanceFromSourceToCenter = min(self.imageCenter[0], self.imageCenter[1]) - 10
+        self.pannelWidth = min(self.imageLabel.width(), self.imageLabel.height())
+
+        imageQT = QImage(self.sliceToShow, self.sliceToShow.shape[1], self.sliceToShow.shape[0], self.sliceToShow.shape[1], QImage.Format_Indexed8)
+        imageQT = imageQT.convertToFormat(QImage.Format_ARGB32)
+        MergedImage = QImage(self.sliceToShow.shape[1], round(self.sliceToShow.shape[0] * Yscaling), QImage.Format_ARGB32)
+        MergedImage.fill(Qt.black)
+        painter = QPainter()
+        painter.begin(MergedImage)
+        painter.scale(1.0, Yscaling)
+        painter.drawImage(0, 0, imageQT)
+
+        for angleIndex, angle in enumerate(self.anglesList):
+            self.draw_polygon(angle[0], angleIndex, painter)
+        self.draw_polygon(self.angleBetweenMouseAndCenter, -1, painter)
+
+        painter.end()
+
+        self.imageLabel.setPixmap(QPixmap.fromImage(MergedImage).scaledToWidth(self.width() - 10, mode=Qt.SmoothTransformation))
+
+##-----------------------------------------------------------------------------------------------------------
+    def addAngle(self):
+        self.anglesList.append([self.angleBetweenMouseAndCenter, self.orientation])
+        self.infoLabelText += 'Angle ' + str(len(self.anglesList)) + ': ' + str(int(np.round(self.anglesList[-1][0]*(360/(2*math.pi))))) + '°' + '\n'
+        self.infoLabel.setText(self.infoLabelText)
+
+##-----------------------------------------------------------------------------------------------------------
+    def draw_polygon(self, angle, angleIndex, painter):
+
+        self.getPolygonPoints(angle)
+        if angleIndex == -1:
+            painter.setBrush(QBrush(Qt.yellow, Qt.Dense6Pattern))
+        else:
+            painter.setBrush(QBrush(self.colorList[angleIndex], Qt.Dense6Pattern))
+
+        polygon = QPolygon([self.pannelPoint1,
+                            self.pannelPoint2,
+                            self.xRaySourcePoint])
+
+        painter.drawPolygon(polygon)
+
+    # def onClicked(self, item):
+    #     print('test onClicked')
+
+    # def onDoubleClick(self, item):
+    #     print('test onDoubleClick')
+
+##-----------------------------------------------------------------------------------------------------------
+    def mouseMoveEvent(self, QMouseEvent):
+        #print('Mouse coords: ( %d : %d )' % (QMouseEvent.x(), QMouseEvent.y()))
+        self.currentMousePos.setX(QMouseEvent._x())
+        self.currentMousePos.setY(QMouseEvent._y())
+        self.getAngleFromMousePosition()
+
+        self.infoLabel.setText(self.infoLabelText + "Current angle : " + str(int(np.round(self.angleBetweenMouseAndCenter*(360/6.28)))) + '°')
+        self.update_viewer()
+
+##-----------------------------------------------------------------------------------------------------------
+    def getAngleFromMousePosition(self):
+
+        if self.imageCenter[1] == self.currentMousePos.y() and self.imageCenter[0] > self.currentMousePos.x():
+            self.angleBetweenMouseAndCenter = math.pi/2
+        elif self.imageCenter[1] == self.currentMousePos.y() and self.imageCenter[0] < self.currentMousePos.x():
+            self.angleBetweenMouseAndCenter = 3 * math.pi / 2
+        elif self.imageCenter[1] < self.currentMousePos.y() and self.imageCenter[0] == self.currentMousePos.x():
+            self.angleBetweenMouseAndCenter = math.pi
+        elif self.imageCenter[1] > self.currentMousePos.y() and self.imageCenter[0] == self.currentMousePos.x():
+            self.angleBetweenMouseAndCenter = 0
+        elif self.imageCenter[0] > self.currentMousePos.x() and self.imageCenter[1] > self.currentMousePos.y():
+            self.angleBetweenMouseAndCenter = math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
+        elif self.imageCenter[0] > self.currentMousePos.x() and self.imageCenter[1] < self.currentMousePos.y():
+            self.angleBetweenMouseAndCenter = math.pi - math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
+        elif self.imageCenter[0] < self.currentMousePos.x() and self.imageCenter[1] < self.currentMousePos.y():
+            self.angleBetweenMouseAndCenter = math.pi + math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
+        elif self.imageCenter[0] < self.currentMousePos.x() and self.imageCenter[1] > self.currentMousePos.y():
+            self.angleBetweenMouseAndCenter = (2 * math.pi) - math.atan(abs(self.imageCenter[0]-self.currentMousePos.x())/abs(self.imageCenter[1]-self.currentMousePos.y()))
+
+    ##-----------------------------------------------------------------------------------------------------------
+    def changeImageView(self):
+        self.orientation = self.sender().text()
+        self.selectSlice()
+        self.update_viewer()
+
+    ##-----------------------------------------------------------------------------------------------------------
+    def prepare_image_for_viewer(self, image):
+        img_min = image.min()
+        # img_max = self.Image.max()
+        img_max = np.percentile(image, 99.995)
+        img = 255 * (image.astype(np.float32) - img_min) / (
+                    img_max - img_min + 1e-5)  # normalize data betwee, 0 and 255
+        img[img > 255] = 255
         return img
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/mainToolbar.py` & `opentps_gui-1.0.5/opentps/gui/panels/mainToolbar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-import functools
-import glob
-import logging
-import os
-
-from PyQt5.QtWidgets import QToolBox, QWidget
-
-from opentps.core import Event
-from opentps.gui.panels.doseComparisonPanel import DoseComparisonPanel
-from opentps.gui.panels.doseComputationPanel import DoseComputationPanel
-from opentps.gui.panels.patientDataPanel.patientDataPanel import PatientDataPanel
-from opentps.gui.panels.planDesignPanel.planDesignPanel import PlanDesignPanel
-from opentps.gui.panels.planOptimizationPanel.planOptiPanel import PlanOptiPanel
-from opentps.gui.panels.roiPanel import ROIPanel
-from opentps.gui.panels.scriptingPanel.scriptingPanel import ScriptingPanel
-from opentps.gui.panels.registrationPanel import RegistrationPanel
-
-logger = logging.getLogger(__name__)
-
-
-class MainToolbar(QToolBox):
-    class ToolbarItem:
-        def __init__(self, panel:QWidget, panelName:str):
-            self.visibleEvent = Event(bool)
-
-            self.panel = panel
-            self.panelName = panelName
-            self.itemNumber = None
-
-            self._visible = True
-
-        @property
-        def visible(self) -> bool:
-            return self._visible
-
-        @visible.setter
-        def visible(self, visible:bool):
-            if visible==self._visible:
-                return
-
-            self._visible = visible
-            self.visibleEvent.emit(self._visible)
-
-    def __init__(self, viewController):
-        QToolBox.__init__(self)
-
-        self._viewController = viewController
-        self._items = []
-        self._maxWidth = 270
-
-        self.setStyleSheet("QToolBox::tab {font: bold; color: #000000; font-size: 16px;}")
-
-        # initialize toolbox panels
-        patientDataPanel = PatientDataPanel(self._viewController)
-        roiPanel = ROIPanel(self._viewController)
-        planDesignPanel = PlanDesignPanel(self._viewController)
-        planDesignPanel.setMaximumWidth(self._maxWidth)
-        planOptiPanel = PlanOptiPanel(self._viewController)
-        planOptiPanel.setMaximumWidth(self._maxWidth)
-        dosePanel = DoseComputationPanel(self._viewController)
-        dosePanel.setMaximumWidth(self._maxWidth)
-        doseComparisonPanel = DoseComparisonPanel(self._viewController)
-        scriptingPanel = ScriptingPanel()
-        #breathingSignalPanel = BreathingSignalPanel(self._viewController)
-        #xRayProjPanel = DRRPanel(self._viewController)
-        registrationPanel = RegistrationPanel(self._viewController)
-
-        self.addWidget(patientDataPanel, 'Patient data')
-        self.addWidget(roiPanel, 'ROI')
-        self.addWidget(planDesignPanel, 'Plan design')
-        self.addWidget(planOptiPanel, 'Plan planOptimization')
-        self.addWidget(dosePanel, 'Dose computation')
-        self.addWidget(doseComparisonPanel, 'Dose comparison')
-        self.addWidget(scriptingPanel, 'Scripting')
-
-    def addWidget(self, widget:QWidget, name:str):
-        item = self.ToolbarItem(widget, name)
-        self.showItem(item)
-        item.visibleEvent.connect(functools.partial(self._handleVisibleEvent, item))
-
-    def _handleVisibleEvent(self, item:ToolbarItem, visible:bool):
-        if visible:
-            self.showItem(item)
-        else:
-            self.hideItem(item)
-
-    def showItem(self, item):
-        if item in self._items:
-            return
-
-        self._items.append(item)
-        self.addItem(item.panel, item.panelName)
-
-    def hideItem(self, item):
-        if not(item in self._items):
-            return
-
-        self.removeItem(self._items.index(item))
-        self._items.remove(item)
-
-    @property
-    def items(self):
-        return [item for item in self._items]
+import functools
+import glob
+import logging
+import os
+
+from PyQt5.QtWidgets import QToolBox, QWidget
+
+from opentps.core import Event
+from opentps.gui.panels.doseComparisonPanel import DoseComparisonPanel
+from opentps.gui.panels.doseComputationPanel import DoseComputationPanel
+from opentps.gui.panels.patientDataPanel.patientDataPanel import PatientDataPanel
+from opentps.gui.panels.planDesignPanel.planDesignPanel import PlanDesignPanel
+from opentps.gui.panels.planEvaluationPanel import PlanEvaluationPanel
+from opentps.gui.panels.planOptimizationPanel.planOptiPanel import PlanOptiPanel
+from opentps.gui.panels.roiPanel import ROIPanel
+from opentps.gui.panels.scriptingPanel.scriptingPanel import ScriptingPanel
+from opentps.gui.panels.registrationPanel import RegistrationPanel
+
+logger = logging.getLogger(__name__)
+
+
+class MainToolbar(QToolBox):
+    class ToolbarItem:
+        def __init__(self, panel:QWidget, panelName:str):
+            self.visibleEvent = Event(bool)
+
+            self.panel = panel
+            self.panelName = panelName
+            self.itemNumber = None
+
+            self._visible = True
+
+        @property
+        def visible(self) -> bool:
+            return self._visible
+
+        @visible.setter
+        def visible(self, visible:bool):
+            if visible==self._visible:
+                return
+
+            self._visible = visible
+            self.visibleEvent.emit(self._visible)
+
+    def __init__(self, viewController):
+        QToolBox.__init__(self)
+
+        self._viewController = viewController
+        self._items = []
+        self._maxWidth = 270
+
+        self.setStyleSheet("QToolBox::tab {font: bold; color: #000000; font-size: 16px;}")
+
+        # initialize toolbox panels
+        patientDataPanel = PatientDataPanel(self._viewController)
+        roiPanel = ROIPanel(self._viewController)
+        planDesignPanel = PlanDesignPanel(self._viewController)
+        planDesignPanel.setMaximumWidth(self._maxWidth)
+        planOptiPanel = PlanOptiPanel(self._viewController)
+        planOptiPanel.setMaximumWidth(self._maxWidth)
+        dosePanel = DoseComputationPanel(self._viewController)
+        dosePanel.setMaximumWidth(self._maxWidth)
+        planEvaluationPanel = PlanEvaluationPanel(self._viewController)
+        planEvaluationPanel.setEnabled(False)
+        doseComparisonPanel = DoseComparisonPanel(self._viewController)
+        scriptingPanel = ScriptingPanel()
+        #breathingSignalPanel = BreathingSignalPanel(self._viewController)
+        #xRayProjPanel = DRRPanel(self._viewController)
+        registrationPanel = RegistrationPanel(self._viewController)
+
+        self.addWidget(patientDataPanel, 'Patient data')
+        self.addWidget(roiPanel, 'ROI')
+        self.addWidget(planDesignPanel, 'Plan design')
+        self.addWidget(planOptiPanel, 'Plan optimization')
+        self.addWidget(dosePanel, 'Dose computation')
+        self.addWidget(planEvaluationPanel, "Plan evaluation")
+        self.addWidget(doseComparisonPanel, 'Dose comparison')
+        self.addWidget(scriptingPanel, 'Scripting')
+
+    def addWidget(self, widget:QWidget, name:str):
+        item = self.ToolbarItem(widget, name)
+        self.showItem(item)
+        item.visibleEvent.connect(functools.partial(self._handleVisibleEvent, item))
+
+    def _handleVisibleEvent(self, item:ToolbarItem, visible:bool):
+        if visible:
+            self.showItem(item)
+        else:
+            self.hideItem(item)
+
+    def showItem(self, item):
+        if item in self._items:
+            return
+
+        self._items.append(item)
+        self.addItem(item.panel, item.panelName)
+
+    def hideItem(self, item):
+        if not(item in self._items):
+            return
+
+        self.removeItem(self._items.index(item))
+        self._items.remove(item)
+
+    @property
+    def items(self):
+        return [item for item in self._items]
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataMenu.py` & `opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataMenu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-
-import copy
-from typing import Sequence, Optional
-
-from PyQt5.QtCore import QDir
-from PyQt5.QtWidgets import QLineEdit, QMenu, QAction, QInputDialog, QMessageBox, QMainWindow
-
-from pydicom.uid import generate_uid
-
-from opentps.core.data.images import CTImage
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.dynamicData.dynamic3DSequence import Dynamic3DSequence
-from opentps.core.data.dynamicData.dynamic3DModel import Dynamic3DModel
-from opentps.core.data import PatientData
-from opentps.core.io.serializedObjectIO import saveSerializedObjects
-from opentps.gui.viewer.dataViewerComponents.patientDataPropertyEditor import PatientDataPropertyEditor
-
-
-class PatientDataMenu:
-    def __init__(self, viewController, parent=None):
-        self._actions = []
-        self._contextMenu = QMenu(parent)
-        self._selectedData = None
-        self._viewController = viewController
-
-        self.dataPath = QDir.currentPath()  # maybe not the ideal default data directory
-
-    @property
-    def selectedData(self) -> Optional[Sequence[PatientData]]:
-        return self._selectedData
-
-    @selectedData.setter
-    def selectedData(self, selectedData:Sequence[PatientData]):
-        self._selectedData = selectedData
-
-        self._buildMenu()
-
-    def _buildMenu(self):
-        self._actions = []
-
-        dataClass = self._selectedData[0].__class__
-        for data in self._selectedData:
-            if data.__class__ != dataClass:
-                dataClass = 'mixed'
-                break
-
-        if (len(self._selectedData) > 0):
-            if len(self._selectedData)==1:
-                self.rename_action = QAction("Rename")
-                self.rename_action.triggered.connect(lambda checked: self._openRenameDataDialog(self._selectedData[0]))
-                self._actions.append(self.rename_action)
-
-                self.copy_action = QAction("Copy")
-                self.copy_action.triggered.connect(lambda checked: self._copyData(self._selectedData[0]))
-                self._actions.append(self.copy_action)
-
-                self.info_action = QAction("Info")
-                self.info_action.triggered.connect(lambda checked: self._showImageInfo(self._selectedData[0]))
-                self._actions.append(self.info_action)
-
-            if not dataClass == 'mixed':
-                # actions for 3D images
-                if (dataClass == Image3D or issubclass(dataClass, Image3D)) and len(self._selectedData) == 1:
-                    self.superimpose_action = QAction("Superimpose")
-                    self.superimpose_action.triggered.connect(lambda checked: self._setSecondaryImage(self._selectedData[0]))
-                    self._actions.append(self.superimpose_action)
-
-                # actions for group of 3DImage
-                if (dataClass == CTImage or issubclass(dataClass, CTImage)) and len(self._selectedData) > 1:  # to generalize to other modalities eventually
-                    self.make_series_action = QAction("Make dynamic 3D sequence")
-                    self.make_series_action.triggered.connect(lambda checked: self._createDynamic3DSequence(self._selectedData))
-                    self._actions.append(self.make_series_action)
-
-            if dataClass == 'mixed':
-                self.no_action = QAction("No action available for this group of data")
-                self.context_menu.addAction(self.no_action)
-
-            # actions for single Dynamic3DSequence
-            if (dataClass == Dynamic3DSequence and len(self._selectedData) == 1):  # or dataClass == 'Dynamic2DSequence'):
-                self.compute3DModelAction = QAction("Compute 4D model (MidP)")
-                self.compute3DModelAction.triggered.connect(lambda checked, selected3DSequence=self._selectedData[0]: self._computeDynamic3DModel(selected3DSequence))
-                self._actions.append(self.compute3DModelAction)
-
-            self.delete_action = QAction("Delete")
-            self.delete_action.triggered.connect(lambda checked: self._openDeleteDataDialog(self._selectedData))
-            self._actions.append(self.delete_action)
-
-            self.export_action = QAction("Export serialized")
-            self.export_action.triggered.connect(lambda checked, selectedData=self._selectedData: self._exportSerializedData(selectedData))
-            self._actions.append(self.export_action)
-
-    def asContextMenu(self) -> QMenu:
-        for action in self._actions:
-            self._contextMenu.addAction(action)
-
-        return self._contextMenu
-
-    def _setSecondaryImage(self, image):
-        self._viewController.secondaryImage = image
-
-    def _copyData(self, selectedData):
-        new_img = copy.deepcopy(selectedData)
-        # new_img.patient = selectedData
-        new_img.name = selectedData.name + '_copy'
-        new_img.patient = selectedData.patient
-
-    def _createDynamic3DSequence(self, selectedImages):
-        newName, okPressed = QInputDialog.getText(None, "Set series name", "Series name:", QLineEdit.Normal, "4DCT")
-
-        if (okPressed):
-            Dynamic3DSequence.fromImagesInPatientList(selectedImages, newName)
-
-    def _computeDynamic3DModel(self, selected3DSequence):
-        newName, okPressed = QInputDialog.getText(None, "Set dynamic 3D model name", "3D model name:", QLineEdit.Normal, "MidP")
-
-        if (okPressed):
-            newMod = Dynamic3DModel()
-            newMod.name = newName
-            newMod.seriesInstanceUID = generate_uid()
-            newMod.computeMidPositionImage(selected3DSequence)
-            self._viewController.currentPatient.appendPatientData(newMod)
-
-    def _openRenameDataDialog(self, data):
-        text, ok = QInputDialog.getText(None, 'Rename data', 'New name:', text=data.name)
-        if ok:
-            data.name = str(text)
-
-    def _openDeleteDataDialog(self, data):
-        msgBox = QMessageBox()
-        msgBox.setIcon(QMessageBox.Information)
-        msgBox.setText("Delete data")
-        msgBox.setWindowTitle("Delete selected data?")
-        msgBox.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
-
-        if msgBox.exec() == QMessageBox.Ok:
-            for dataItem in data:
-                dataItem.patient.removePatientData(dataItem)
-
-    def _showImageInfo(self, image):
-        w = QMainWindow(self._contextMenu.parent())
-        w.setWindowTitle('Image info')
-        w.resize(400, 400)
-        w.setCentralWidget(PatientDataPropertyEditor(image, self._contextMenu.parent()))
-        w.show()
-
-    def _exportSerializedData(self, selectedData):
-        from opentps.gui.panels.patientDataPanel.patientDataPanel import SaveData_dialog
-        fileDialog = SaveData_dialog()
-        savingPath, compressedBool, splitPatientsBool = fileDialog.getSaveFileName(None, dir=self.dataPath)
-
-        saveSerializedObjects(selectedData, savingPath, compressedBool=compressedBool)
+
+import copy
+from typing import Sequence, Optional
+
+from PyQt5.QtCore import QDir
+from PyQt5.QtWidgets import QLineEdit, QMenu, QAction, QInputDialog, QMessageBox, QMainWindow
+
+from pydicom.uid import generate_uid
+
+from opentps.core.data.images import CTImage
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.dynamicData._dynamic3DSequence import Dynamic3DSequence
+from opentps.core.data.dynamicData._dynamic3DModel import Dynamic3DModel
+from opentps.core.data import PatientData
+from opentps.core.io.serializedObjectIO import saveSerializedObjects
+from opentps.gui.viewer.dataViewerComponents.patientDataPropertyEditor import PatientDataPropertyEditor
+
+
+class PatientDataMenu:
+    def __init__(self, viewController, parent=None):
+        self._actions = []
+        self._contextMenu = QMenu(parent)
+        self._selectedData = None
+        self._viewController = viewController
+
+        self.dataPath = QDir.currentPath()  # maybe not the ideal default data directory
+
+    @property
+    def selectedData(self) -> Optional[Sequence[PatientData]]:
+        return self._selectedData
+
+    @selectedData.setter
+    def selectedData(self, selectedData:Sequence[PatientData]):
+        self._selectedData = selectedData
+
+        self._buildMenu()
+
+    def _buildMenu(self):
+        self._actions = []
+
+        dataClass = self._selectedData[0].__class__
+        for data in self._selectedData:
+            if data.__class__ != dataClass:
+                dataClass = 'mixed'
+                break
+
+        if (len(self._selectedData) > 0):
+            if len(self._selectedData)==1:
+                self.rename_action = QAction("Rename")
+                self.rename_action.triggered.connect(lambda checked: self._openRenameDataDialog(self._selectedData[0]))
+                self._actions.append(self.rename_action)
+
+                self.copy_action = QAction("Copy")
+                self.copy_action.triggered.connect(lambda checked: self._copyData(self._selectedData[0]))
+                self._actions.append(self.copy_action)
+
+                self.info_action = QAction("Info")
+                self.info_action.triggered.connect(lambda checked: self._showImageInfo(self._selectedData[0]))
+                self._actions.append(self.info_action)
+
+            if not dataClass == 'mixed':
+                # actions for 3D images
+                if (dataClass == Image3D or issubclass(dataClass, Image3D)) and len(self._selectedData) == 1:
+                    self.superimpose_action = QAction("Superimpose")
+                    self.superimpose_action.triggered.connect(lambda checked: self._setSecondaryImage(self._selectedData[0]))
+                    self._actions.append(self.superimpose_action)
+
+                # actions for group of 3DImage
+                if (dataClass == CTImage or issubclass(dataClass, CTImage)) and len(self._selectedData) > 1:  # to generalize to other modalities eventually
+                    self.make_series_action = QAction("Make dynamic 3D sequence")
+                    self.make_series_action.triggered.connect(lambda checked: self._createDynamic3DSequence(self._selectedData))
+                    self._actions.append(self.make_series_action)
+
+            if dataClass == 'mixed':
+                self.no_action = QAction("No action available for this group of data")
+                self.context_menu.addAction(self.no_action)
+
+            # actions for single Dynamic3DSequence
+            if (dataClass == Dynamic3DSequence and len(self._selectedData) == 1):  # or dataClass == 'Dynamic2DSequence'):
+                self.compute3DModelAction = QAction("Compute 4D model (MidP)")
+                self.compute3DModelAction.triggered.connect(lambda checked, selected3DSequence=self._selectedData[0]: self._computeDynamic3DModel(selected3DSequence))
+                self._actions.append(self.compute3DModelAction)
+
+            self.delete_action = QAction("Delete")
+            self.delete_action.triggered.connect(lambda checked: self._openDeleteDataDialog(self._selectedData))
+            self._actions.append(self.delete_action)
+
+            self.export_action = QAction("Export serialized")
+            self.export_action.triggered.connect(lambda checked, selectedData=self._selectedData: self._exportSerializedData(selectedData))
+            self._actions.append(self.export_action)
+
+    def asContextMenu(self) -> QMenu:
+        for action in self._actions:
+            self._contextMenu.addAction(action)
+
+        return self._contextMenu
+
+    def _setSecondaryImage(self, image):
+        self._viewController.secondaryImage = image
+
+    def _copyData(self, selectedData):
+        new_img = copy.deepcopy(selectedData)
+        # new_img.patient = selectedData
+        new_img.name = selectedData.name + '_copy'
+        new_img.patient = selectedData.patient
+
+    def _createDynamic3DSequence(self, selectedImages):
+        newName, okPressed = QInputDialog.getText(None, "Set series name", "Series name:", QLineEdit.Normal, "4DCT")
+
+        if (okPressed):
+            Dynamic3DSequence.fromImagesInPatientList(selectedImages, newName)
+
+    def _computeDynamic3DModel(self, selected3DSequence):
+        newName, okPressed = QInputDialog.getText(None, "Set dynamic 3D model name", "3D model name:", QLineEdit.Normal, "MidP")
+
+        if (okPressed):
+            newMod = Dynamic3DModel()
+            newMod.name = newName
+            newMod.seriesInstanceUID = generate_uid()
+            newMod.computeMidPositionImage(selected3DSequence)
+            self._viewController.currentPatient.appendPatientData(newMod)
+
+    def _openRenameDataDialog(self, data):
+        text, ok = QInputDialog.getText(None, 'Rename data', 'New name:', text=data.name)
+        if ok:
+            data.name = str(text)
+
+    def _openDeleteDataDialog(self, data):
+        msgBox = QMessageBox()
+        msgBox.setIcon(QMessageBox.Information)
+        msgBox.setText("Delete data")
+        msgBox.setWindowTitle("Delete selected data?")
+        msgBox.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
+
+        if msgBox.exec() == QMessageBox.Ok:
+            for dataItem in data:
+                dataItem.patient.removePatientData(dataItem)
+
+    def _showImageInfo(self, image):
+        w = QMainWindow(self._contextMenu.parent())
+        w.setWindowTitle('Image info')
+        w.resize(400, 400)
+        w.setCentralWidget(PatientDataPropertyEditor(image, self._contextMenu.parent()))
+        w.show()
+
+    def _exportSerializedData(self, selectedData):
+        from opentps.gui.panels.patientDataPanel.patientDataPanel import SaveData_dialog
+        fileDialog = SaveData_dialog()
+        savingPath, compressedBool, splitPatientsBool = fileDialog.getSaveFileName(None, dir=self.dataPath)
+
+        saveSerializedObjects(selectedData, savingPath, compressedBool=compressedBool)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataPanel.py` & `opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataPanel.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-
-from PyQt5.QtCore import QDir
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QPushButton, QFileDialog, QDialog, \
-    QStackedWidget, QListView, QLineEdit, QHBoxLayout, QCheckBox
-
-import opentps.core.io.dataLoader as dataLoader
-from opentps.core.io.serializedObjectIO import saveDataStructure
-from opentps.core import Event
-from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
-
-
-class PatientDataPanel(QWidget):
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-
-        # Events
-        self.patientAddedSignal = Event(object)
-        self.patientRemovedSignal = Event(object)
-
-        self._viewController = viewController
-
-        self._viewController.patientAddedSignal.connect(self.patientAddedSignal.emit)
-
-        self._viewController.patientRemovedSignal.connect(self.patientRemovedSignal.emit)
-
-        self.layout = QVBoxLayout()
-        self.setLayout(self.layout)
-
-        self._patientDataSelection = PatientDataSelection(self._viewController)
-        self.layout.addWidget(self._patientDataSelection)
-
-        self.buttonLayout = QHBoxLayout()
-        loadDataButton = QPushButton('Load data')
-        loadDataButton.clicked.connect(self.loadData)
-        self.buttonLayout.addWidget(loadDataButton)
-        saveDataButton = QPushButton('Save data (Serialized)')
-        saveDataButton.clicked.connect(self.saveData)
-        self.buttonLayout.addWidget(saveDataButton)
-        self.layout.addLayout(self.buttonLayout)
-
-        self.dataPath = QDir.currentPath() # maybe not the ideal default data directory
-
-    def loadData(self):
-        filesOrFoldersList = _getOpenFilesAndDirs(caption="Open patient data files or folders", directory=QDir.currentPath())
-        if len(filesOrFoldersList) < 1:
-            return
-
-        splitPath = filesOrFoldersList[0].split('/')
-        withoutLastElementPath = ''
-        for element in splitPath[:-1]:
-            withoutLastElementPath += element + '/'
-        self.dataPath = withoutLastElementPath
-
-        dataLoader.loadData(self._viewController._patientList, filesOrFoldersList)
-
-    def saveData(self):
-        fileDialog = SaveData_dialog()
-        savingPath, compressedBool, splitPatientsBool = fileDialog.getSaveFileName(None, dir=self.dataPath)
-
-        patientList = self._viewController.activePatients
-        # patientList = [patient.dumpableCopy() for patient in self._viewController._patientList]
-        saveDataStructure(patientList, savingPath, compressedBool=compressedBool, splitPatientsBool=splitPatientsBool)
-
-## ------------------------------------------------------------------------------------------
-class SaveData_dialog(QFileDialog):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # self.defaultName = "Patient"
-
-    def getSaveFileName(self, parent=None,
-                        caption="Select folder and file name to save data tree",
-                        dir=".",
-                        filter='',
-                        initialFilter='',
-                        defaultName="Patient",
-                        options=None):
-
-        self.setWindowTitle(caption)
-        self.setDirectory(dir)
-        self.selectFile(defaultName)
-        self.setAcceptMode(QFileDialog.AcceptSave)  # bouton "Save"
-        self.setOption(QFileDialog.DontUseNativeDialog, True)
-
-        layout = self.layout()
-        # checkBoxLayout = QHBoxLayout
-        self.compressBox = QCheckBox("Compress data", self)
-        self.compressBox.setToolTip('This will compress the data before saving them, it takes longer to save the data this way')
-        layout.addWidget(self.compressBox, 4, 0)
-        self.splitPatientsBox = QCheckBox("Split Patients", self)
-        self.splitPatientsBox.setToolTip('This will split patients into multiple files if multiple patients data are loaded')
-        layout.addWidget(self.splitPatientsBox, 4, 1)
-        self.setLayout(layout)
-
-        if self.exec_():
-            return self.selectedFiles()[0], self.compressBox.isChecked(), self.splitPatientsBox.isChecked()
-        else:
-            return "", ""
-
-def _getOpenFilesAndDirs(parent=None, caption='', directory='',
-                          filter='', initialFilter='', options=None):
-    def updateText():
-      # update the contents of the line edit widget with the selected files
-      selected = []
-      for index in view.selectionModel().selectedRows():
-        selected.append('"{}"'.format(index.data()))
-      lineEdit.setText(' '.join(selected))
-
-    dialog = QFileDialog(parent, windowTitle=caption)
-    dialog.setFileMode(dialog.ExistingFiles)
-    if options:
-      dialog.setOptions(options)
-    dialog.setOption(dialog.DontUseNativeDialog, True)
-    if directory:
-      dialog.setDirectory(directory)
-    if filter:
-      dialog.setNameFilter(filter)
-      if initialFilter:
-        dialog.selectNameFilter(initialFilter)
-
-    # by default, if a directory is opened in file listing mode,
-    # QFileDialog.accept() shows the contents of that directory, but we
-    # need to be able to "open" directories as we can do with files, so we
-    # just override accept() with the default QDialog implementation which
-    # will just return exec_()
-    dialog.accept = lambda: QDialog.accept(dialog)
-
-    # there are many item views in a non-native dialog, but the ones displaying
-    # the actual contents are created inside a QStackedWidget; they are a
-    # QTreeView and a QListView, and the tree is only used when the
-    # viewMode is set to QFileDialog.Details, which is not this case
-    stackedWidget = dialog.findChild(QStackedWidget)
-    view = stackedWidget.findChild(QListView)
-    view.selectionModel().selectionChanged.connect(updateText)
-
-    lineEdit = dialog.findChild(QLineEdit)
-    # clear the line edit contents whenever the current directory changes
-    dialog.directoryEntered.connect(lambda: lineEdit.setText(''))
-
-    dialog.exec_()
+
+from PyQt5.QtCore import QDir
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QPushButton, QFileDialog, QDialog, \
+    QStackedWidget, QListView, QLineEdit, QHBoxLayout, QCheckBox
+
+import opentps.core.io.dataLoader as dataLoader
+from opentps.core.io.serializedObjectIO import saveDataStructure
+from opentps.core import Event
+from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
+
+
+class PatientDataPanel(QWidget):
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+
+        # Events
+        self.patientAddedSignal = Event(object)
+        self.patientRemovedSignal = Event(object)
+
+        self._viewController = viewController
+
+        self._viewController.patientAddedSignal.connect(self.patientAddedSignal.emit)
+
+        self._viewController.patientRemovedSignal.connect(self.patientRemovedSignal.emit)
+
+        self.layout = QVBoxLayout()
+        self.setLayout(self.layout)
+
+        self._patientDataSelection = PatientDataSelection(self._viewController)
+        self.layout.addWidget(self._patientDataSelection)
+
+        self.buttonLayout = QHBoxLayout()
+        loadDataButton = QPushButton('Load data')
+        loadDataButton.clicked.connect(self.loadData)
+        self.buttonLayout.addWidget(loadDataButton)
+        saveDataButton = QPushButton('Save data (Serialized)')
+        saveDataButton.clicked.connect(self.saveData)
+        self.buttonLayout.addWidget(saveDataButton)
+        self.layout.addLayout(self.buttonLayout)
+
+        self.dataPath = QDir.currentPath() # maybe not the ideal default data directory
+
+    def loadData(self):
+        filesOrFoldersList = _getOpenFilesAndDirs(caption="Open patient data files or folders", directory=QDir.currentPath())
+        if len(filesOrFoldersList) < 1:
+            return
+
+        splitPath = filesOrFoldersList[0].split('/')
+        withoutLastElementPath = ''
+        for element in splitPath[:-1]:
+            withoutLastElementPath += element + '/'
+        self.dataPath = withoutLastElementPath
+
+        dataLoader.loadData(self._viewController._patientList, filesOrFoldersList)
+
+    def saveData(self):
+        fileDialog = SaveData_dialog()
+        savingPath, compressedBool, splitPatientsBool = fileDialog.getSaveFileName(None, dir=self.dataPath)
+
+        patientList = self._viewController.activePatients
+        # patientList = [patient.dumpableCopy() for patient in self._viewController._patientList]
+        saveDataStructure(patientList, savingPath, compressedBool=compressedBool, splitPatientsBool=splitPatientsBool)
+
+## ------------------------------------------------------------------------------------------
+class SaveData_dialog(QFileDialog):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # self.defaultName = "Patient"
+
+    def getSaveFileName(self, parent=None,
+                        caption="Select folder and file name to save data tree",
+                        dir=".",
+                        filter='',
+                        initialFilter='',
+                        defaultName="Patient",
+                        options=None):
+
+        self.setWindowTitle(caption)
+        self.setDirectory(dir)
+        self.selectFile(defaultName)
+        self.setAcceptMode(QFileDialog.AcceptSave)  # bouton "Save"
+        self.setOption(QFileDialog.DontUseNativeDialog, True)
+
+        layout = self.layout()
+        # checkBoxLayout = QHBoxLayout
+        self.compressBox = QCheckBox("Compress data", self)
+        self.compressBox.setToolTip('This will compress the data before saving them, it takes longer to save the data this way')
+        layout.addWidget(self.compressBox, 4, 0)
+        self.splitPatientsBox = QCheckBox("Split Patients", self)
+        self.splitPatientsBox.setToolTip('This will split patients into multiple files if multiple patients data are loaded')
+        layout.addWidget(self.splitPatientsBox, 4, 1)
+        self.setLayout(layout)
+
+        if self.exec_():
+            return self.selectedFiles()[0], self.compressBox.isChecked(), self.splitPatientsBox.isChecked()
+        else:
+            return "", ""
+
+def _getOpenFilesAndDirs(parent=None, caption='', directory='',
+                          filter='', initialFilter='', options=None):
+    def updateText():
+      # update the contents of the line edit widget with the selected files
+      selected = []
+      for index in view.selectionModel().selectedRows():
+        selected.append('"{}"'.format(index.data()))
+      lineEdit.setText(' '.join(selected))
+
+    dialog = QFileDialog(parent, windowTitle=caption)
+    dialog.setFileMode(dialog.ExistingFiles)
+    if options:
+      dialog.setOptions(options)
+    dialog.setOption(dialog.DontUseNativeDialog, True)
+    if directory:
+      dialog.setDirectory(directory)
+    if filter:
+      dialog.setNameFilter(filter)
+      if initialFilter:
+        dialog.selectNameFilter(initialFilter)
+
+    # by default, if a directory is opened in file listing mode,
+    # QFileDialog.accept() shows the contents of that directory, but we
+    # need to be able to "open" directories as we can do with files, so we
+    # just override accept() with the default QDialog implementation which
+    # will just return exec_()
+    dialog.accept = lambda: QDialog.accept(dialog)
+
+    # there are many item views in a non-native dialog, but the ones displaying
+    # the actual contents are created inside a QStackedWidget; they are a
+    # QTreeView and a QListView, and the tree is only used when the
+    # viewMode is set to QFileDialog.Details, which is not this case
+    stackedWidget = dialog.findChild(QStackedWidget)
+    view = stackedWidget.findChild(QListView)
+    view.selectionModel().selectionChanged.connect(updateText)
+
+    lineEdit = dialog.findChild(QLineEdit)
+    # clear the line edit contents whenever the current directory changes
+    dialog.directoryEntered.connect(lambda: lineEdit.setText(''))
+
+    dialog.exec_()
     return dialog.selectedFiles()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/patientDataPanel/patientDataSelection.py` & `opentps_gui-1.0.5/opentps/gui/panels/patientDataPanel/patientDataSelection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,310 +1,310 @@
-from typing import Sequence
-
-from PyQt5 import QtCore
-from PyQt5.QtCore import QMimeData, Qt
-from PyQt5.QtGui import QStandardItemModel, QDrag, QFont, QStandardItem, QColor
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QComboBox, QTreeView, QAbstractItemView
-
-from opentps.core.data.dynamicData.dynamic2DSequence import Dynamic2DSequence
-from opentps.core.data.dynamicData.dynamic3DModel import Dynamic3DModel
-from opentps.core.data.dynamicData.dynamic3DSequence import Dynamic3DSequence
-
-from opentps.core.data.images import CTImage
-from opentps.core.data.images import DoseImage
-from opentps.core.data.images import Image2D
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.images import VectorField3D
-from opentps.core.data.plan._rtPlan import RTPlan
-from opentps.core.data import PatientData
-
-from opentps.gui.panels.patientDataPanel.patientDataMenu import PatientDataMenu
-from opentps.gui.viewer.dataViewer import DroppedObject
-
-
-class PatientDataSelection(QWidget):
-    def __init__(self, viewController, parent=None):
-        super().__init__(parent)
-
-        self._viewController = viewController
-
-        self._mainLayout = QVBoxLayout(self)
-        self.setLayout(self._mainLayout)
-
-        self.patientBox = PatientComboBox(self._viewController)
-
-        self._patientDataTree = PatientDataTree(self._viewController, self)
-
-        self._mainLayout.addWidget(self.patientBox)
-        self._mainLayout.addWidget(self._patientDataTree)
-
-    @property
-    def selectedData(self) -> Sequence[PatientData]:
-        selected = self._patientDataTree.selectedIndexes()
-        selectedData = [self._patientDataTree.model().itemFromIndex(selectedData).data for selectedData in selected]
-
-        return selectedData
-
-class PatientComboBox(QComboBox):
-    def __init__(self, viewController):
-        QComboBox.__init__(self)
-
-        self._viewController = viewController
-
-        self._viewController.patientAddedSignal.connect(self._addPatient)
-        self._viewController.patientRemovedSignal.connect(self._removePatient)
-        self._viewController.currentPatientChangedSignal.connect(self._setCurrentPatient)
-
-        self.currentIndexChanged.connect(self._setCurrentPatientInVC)
-
-        self._initialize()
-
-    def closeEvent(self, QCloseEvent):
-        self._viewController.patientAddedSignal.disconnect(self._addPatient)
-        self._viewController.patientRemovedSignal.disconnect(self._removePatient)
-        self._viewController.currentPatientChangedSignal.disconnect(self._setCurrentPatient)
-
-        super().closeEvent(QCloseEvent)
-
-    def _initialize(self):
-        for patient in self._viewController.patientList:
-            self._addPatient(patient)
-
-    def _addPatient(self, patient):
-        name = patient.name
-        if name is None:
-            name = 'None'
-
-        self.addItem(name, patient)
-        if self.count() == 1:
-            self._viewController.currentPatient = patient
-
-    def _removePatient(self, patient):
-        self.removeItem(self.findData(patient))
-
-    def _setCurrentPatient(self, patient):
-        if patient == self.currentData():
-            return
-
-        self.setCurrentIndex(self.findData(patient))
-
-
-    def _setCurrentPatientInVC(self, index):
-        self._viewController.currentPatient = self.currentData()
-
-
-## ------------------------------------------------------------------------------------------
-class PatientDataTree(QTreeView):
-    def __init__(self, viewController, patientDataPanel):
-        QTreeView.__init__(self)
-
-        self._currentPatient = None
-        self.patientDataPanel = patientDataPanel
-        self._viewController = viewController
-
-        self.setHeaderHidden(True)
-        self.setSelectionMode(QAbstractItemView.ExtendedSelection)
-        self.setContextMenuPolicy(Qt.CustomContextMenu)
-        self.viewport().installEventFilter(self)
-        self.customContextMenuRequested.connect(self._handleRightClick)
-        self.resizeColumnToContents(0)
-        self.doubleClicked.connect(self._handleDoubleClick)
-        self.treeModel = QStandardItemModel()
-        self.setModel(self.treeModel)
-        self.setColumnHidden(1, True)
-        self.expandAll()
-
-        self.buildDataTree(self._viewController.currentPatient)
-        self._viewController.currentPatientChangedSignal.connect(self.buildDataTree)
-
-        self.setDragDropMode(QAbstractItemView.InternalMove)
-        self.setDragEnabled(True)
-        self.setAcceptDrops(True)
-
-    def closeEvent(self, QCloseEvent):
-        self._disconnectCurrentPatientAndItems()
-        self._viewController.currentPatientChangedSignal.disconnect(self.buildDataTree)
-
-        super().closeEvent(QCloseEvent)
-
-    def _appendData(self, data):
-        if isinstance(data, Image3D) or isinstance(data, RTPlan) or isinstance(data, Dynamic3DSequence) or isinstance(data, Dynamic2DSequence):
-            rootItem = PatientDataItem(data)
-            self.rootNode.appendRow(rootItem)
-
-            if isinstance(data, Dynamic3DSequence):
-                for image in data.dyn3DImageList:
-                    item = PatientDataItem(image)
-                    rootItem.appendRow(item)
-                self.rootNode.appendRow(rootItem)
-
-            if isinstance(data, Dynamic2DSequence):
-                for image in data.dyn2DImageList:
-                    item = PatientDataItem(image)
-                    rootItem.appendRow(item)
-                self.rootNode.appendRow(rootItem)
-
-    def _removeData(self, data):
-        items = []
-
-        for row in range(self.model().rowCount()):
-            item = self.model().itemFromIndex(self.model().index(row, 0))
-            items.append(item)
-
-        for item in items:
-            if item.data == data:
-                self.rootNode.removeRow(item.row())
-                item.disconnectAll() #Do this explicitely to be sure signals are disconnected
-
-    def mouseMoveEvent(self, event):
-        drag = QDrag(self)
-        mimeData = QMimeData()
-
-        mimeData.setText(DroppedObject.DropTypes.IMAGE)
-        drag.setMimeData(mimeData)
-
-        drag.exec_(QtCore.Qt.CopyAction)
-
-    def buildDataTree(self, patient):
-        self._disconnectCurrentPatientAndItems()
-
-        self.treeModel.clear()
-        self.rootNode = self.treeModel.invisibleRootItem()
-        font_b = QFont()
-        font_b.setBold(True)
-
-        self._currentPatient = patient
-
-        if self._currentPatient is None:
-            return
-
-        self._currentPatient.patientDataAddedSignal.connect(self._appendData)
-        self._currentPatient.patientDataRemovedSignal.connect(self._removeData)
-
-        #TODO: Same with other data
-
-        #images
-        images = self._currentPatient.images
-        for image in images:
-            self._appendData(image)
-
-        if len(images) > 0:
-            self._viewController.selectedImage = images[0]
-
-        for plan in patient.plans:
-            self._appendData(plan)
-
-        # dynamic sequences
-        for dynSeq in patient.dynamic3DSequences:
-            self._appendData(dynSeq)
-
-        for dynSeq in patient.dynamic2DSequences:
-            self._appendData(dynSeq)
-
-        # dynamic models
-        for model in self._currentPatient.dynamic3DModels:
-            serieRoot = PatientDataItem(model)
-            for field in model.deformationList:
-                item = PatientDataItem(field)
-                serieRoot.appendRow(item)
-            self.rootNode.appendRow(serieRoot)
-
-    def _disconnectCurrentPatientAndItems(self):
-        # Disconnect signals
-        if not (self._currentPatient is None):
-            self._currentPatient.patientDataAddedSignal.disconnect(self._appendData)
-            self._currentPatient.patientDataRemovedSignal.disconnect(self._removeData)
-
-        # Do this explicitely to be sure signals are disconnected
-        for row in range(self.model().rowCount()):
-            item = self.model().itemFromIndex(self.model().index(row, 0))
-            if isinstance(item, PatientDataItem):
-                item.disconnectAll()
-
-    def dragEnterEvent(self, event):
-        selection = self.selectionModel().selectedIndexes()[0]
-        self._viewController.selectedImage = self.model().itemFromIndex(selection).data
-
-    def _handleDoubleClick(self, selection):
-        selectedData = self.model().itemFromIndex(selection).data
-
-        if isinstance(selectedData, CTImage) or isinstance(selectedData, Dynamic3DSequence) or isinstance(selectedData, Dynamic2DSequence) or isinstance(selectedData, Image2D):
-            self._viewController.mainImage = selectedData
-        if isinstance(selectedData, RTPlan):
-            self._viewController.plan = selectedData
-        elif isinstance(selectedData, Dynamic3DModel):
-            self._viewController.mainImage = selectedData.midp
-        elif isinstance(selectedData, DoseImage):
-            self._viewController.secondaryImage = selectedData
-
-    def _handleRightClick(self, pos):
-        pos = self.mapToGlobal(pos)
-
-        selected = self.selectedIndexes()
-        selectedData = [self.model().itemFromIndex(selectedData).data for selectedData in selected]
-
-        dataMenu = PatientDataMenu(self._viewController, self)
-        dataMenu.selectedData = selectedData
-        dataMenu.asContextMenu().popup(pos)
-
-
-
-## ------------------------------------------------------------------------------------------
-class PatientDataItem(QStandardItem):
-    def __init__(self, data, txt="", dataType="", color=QColor(75, 75, 75)):
-        QStandardItem.__init__(self)
-
-
-        # print('in patientDataSelection.py, PatientDataItem init', type(data), data.getTypeAsString())
-        self.data = data
-        # print(data.__dict__)
-        self.data.nameChangedSignal.connect(self.setName)
-
-        self.setEditable(False)
-
-        defaultColor = color
-        dynSeqColor = QColor(109, 119, 125)
-        planColor = QColor(56, 130, 176)
-        doseColor = QColor(166, 63, 104)
-        modelColor = QColor(194, 130, 35)
-        vectorFieldColor = QColor(201, 111, 50)
-
-        if isinstance(data, CTImage):
-            self.setName('CT' + ' - ' + self.data.name)
-            self.setForeground(defaultColor)
-        elif isinstance(data, Dynamic3DSequence):
-            self.setName('3D Seq' + ' - ' + self.data.name)
-            self.setForeground(dynSeqColor)
-        elif isinstance(data, Dynamic2DSequence):
-            self.setName('2D Seq' + ' - ' + self.data.name)
-            self.setForeground(dynSeqColor)
-        elif isinstance(data, Image2D):
-            self.setName('2D Img' + ' - ' + self.data.name)
-            self.setForeground(defaultColor)
-        elif isinstance(data, RTPlan):
-            self.setName('plan' + ' - ' + self.data.name)
-            self.setForeground(planColor)
-        elif isinstance(data, Dynamic3DModel):
-            self.setName('DynMod' + ' - ' + self.data.name)
-            self.setForeground(modelColor)
-        elif isinstance(data, VectorField3D):
-            self.setName('Vec Field' + ' - ' + self.data.name)
-            self.setForeground(vectorFieldColor)
-        elif isinstance(data, DoseImage):
-            self.setName('Dose' + ' - ' + self.data.name)
-            self.setForeground(doseColor)
-        else:
-            self.setName(data.getTypeAsString() + ' - ' + self.data.name)
-            self.setForeground(defaultColor)
-
-        # self.setText(txt)
-        # self.setWhatsThis(type)
-
-    def disconnectAll(self):
-        self.data.nameChangedSignal.disconnect(self.setName)
-
-    # No effect: it seems that C destructor of QStandardItem does not trigger __del__
-    def __del__(self):
-        self.disconnectAll()
-
-    def setName(self, name):
-        self.setText(name)
+from typing import Sequence
+
+from PyQt5 import QtCore
+from PyQt5.QtCore import QMimeData, Qt
+from PyQt5.QtGui import QStandardItemModel, QDrag, QFont, QStandardItem, QColor
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QComboBox, QTreeView, QAbstractItemView
+
+from opentps.core.data.dynamicData._dynamic2DSequence import Dynamic2DSequence
+from opentps.core.data.dynamicData._dynamic3DModel import Dynamic3DModel
+from opentps.core.data.dynamicData._dynamic3DSequence import Dynamic3DSequence
+
+from opentps.core.data.images import CTImage
+from opentps.core.data.images import DoseImage
+from opentps.core.data.images import Image2D
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.images import VectorField3D
+from opentps.core.data.plan._rtPlan import RTPlan
+from opentps.core.data import PatientData
+
+from opentps.gui.panels.patientDataPanel.patientDataMenu import PatientDataMenu
+from opentps.gui.viewer.dataViewer import DroppedObject
+
+
+class PatientDataSelection(QWidget):
+    def __init__(self, viewController, parent=None):
+        super().__init__(parent)
+
+        self._viewController = viewController
+
+        self._mainLayout = QVBoxLayout(self)
+        self.setLayout(self._mainLayout)
+
+        self.patientBox = PatientComboBox(self._viewController)
+
+        self._patientDataTree = PatientDataTree(self._viewController, self)
+
+        self._mainLayout.addWidget(self.patientBox)
+        self._mainLayout.addWidget(self._patientDataTree)
+
+    @property
+    def selectedData(self) -> Sequence[PatientData]:
+        selected = self._patientDataTree.selectedIndexes()
+        selectedData = [self._patientDataTree.model().itemFromIndex(selectedData).data for selectedData in selected]
+
+        return selectedData
+
+class PatientComboBox(QComboBox):
+    def __init__(self, viewController):
+        QComboBox.__init__(self)
+
+        self._viewController = viewController
+
+        self._viewController.patientAddedSignal.connect(self._addPatient)
+        self._viewController.patientRemovedSignal.connect(self._removePatient)
+        self._viewController.currentPatientChangedSignal.connect(self._setCurrentPatient)
+
+        self.currentIndexChanged.connect(self._setCurrentPatientInVC)
+
+        self._initialize()
+
+    def closeEvent(self, QCloseEvent):
+        self._viewController.patientAddedSignal.disconnect(self._addPatient)
+        self._viewController.patientRemovedSignal.disconnect(self._removePatient)
+        self._viewController.currentPatientChangedSignal.disconnect(self._setCurrentPatient)
+
+        super().closeEvent(QCloseEvent)
+
+    def _initialize(self):
+        for patient in self._viewController.patientList:
+            self._addPatient(patient)
+
+    def _addPatient(self, patient):
+        name = patient.name
+        if name is None:
+            name = 'None'
+
+        self.addItem(name, patient)
+        if self.count() == 1:
+            self._viewController.currentPatient = patient
+
+    def _removePatient(self, patient):
+        self.removeItem(self.findData(patient))
+
+    def _setCurrentPatient(self, patient):
+        if patient == self.currentData():
+            return
+
+        self.setCurrentIndex(self.findData(patient))
+
+
+    def _setCurrentPatientInVC(self, index):
+        self._viewController.currentPatient = self.currentData()
+
+
+## ------------------------------------------------------------------------------------------
+class PatientDataTree(QTreeView):
+    def __init__(self, viewController, patientDataPanel):
+        QTreeView.__init__(self)
+
+        self._currentPatient = None
+        self.patientDataPanel = patientDataPanel
+        self._viewController = viewController
+
+        self.setHeaderHidden(True)
+        self.setSelectionMode(QAbstractItemView.ExtendedSelection)
+        self.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.viewport().installEventFilter(self)
+        self.customContextMenuRequested.connect(self._handleRightClick)
+        self.resizeColumnToContents(0)
+        self.doubleClicked.connect(self._handleDoubleClick)
+        self.treeModel = QStandardItemModel()
+        self.setModel(self.treeModel)
+        self.setColumnHidden(1, True)
+        self.expandAll()
+
+        self.buildDataTree(self._viewController.currentPatient)
+        self._viewController.currentPatientChangedSignal.connect(self.buildDataTree)
+
+        self.setDragDropMode(QAbstractItemView.InternalMove)
+        self.setDragEnabled(True)
+        self.setAcceptDrops(True)
+
+    def closeEvent(self, QCloseEvent):
+        self._disconnectCurrentPatientAndItems()
+        self._viewController.currentPatientChangedSignal.disconnect(self.buildDataTree)
+
+        super().closeEvent(QCloseEvent)
+
+    def _appendData(self, data):
+        if isinstance(data, Image3D) or isinstance(data, RTPlan) or isinstance(data, Dynamic3DSequence) or isinstance(data, Dynamic2DSequence):
+            rootItem = PatientDataItem(data)
+            self.rootNode.appendRow(rootItem)
+
+            if isinstance(data, Dynamic3DSequence):
+                for image in data.dyn3DImageList:
+                    item = PatientDataItem(image)
+                    rootItem.appendRow(item)
+                self.rootNode.appendRow(rootItem)
+
+            if isinstance(data, Dynamic2DSequence):
+                for image in data.dyn2DImageList:
+                    item = PatientDataItem(image)
+                    rootItem.appendRow(item)
+                self.rootNode.appendRow(rootItem)
+
+    def _removeData(self, data):
+        items = []
+
+        for row in range(self.model().rowCount()):
+            item = self.model().itemFromIndex(self.model().index(row, 0))
+            items.append(item)
+
+        for item in items:
+            if item.data == data:
+                self.rootNode.removeRow(item.row())
+                item.disconnectAll() #Do this explicitely to be sure signals are disconnected
+
+    def mouseMoveEvent(self, event):
+        drag = QDrag(self)
+        mimeData = QMimeData()
+
+        mimeData.setText(DroppedObject.DropTypes.IMAGE)
+        drag.setMimeData(mimeData)
+
+        drag.exec_(QtCore.Qt.CopyAction)
+
+    def buildDataTree(self, patient):
+        self._disconnectCurrentPatientAndItems()
+
+        self.treeModel.clear()
+        self.rootNode = self.treeModel.invisibleRootItem()
+        font_b = QFont()
+        font_b.setBold(True)
+
+        self._currentPatient = patient
+
+        if self._currentPatient is None:
+            return
+
+        self._currentPatient.patientDataAddedSignal.connect(self._appendData)
+        self._currentPatient.patientDataRemovedSignal.connect(self._removeData)
+
+        #TODO: Same with other data
+
+        #images
+        images = self._currentPatient.images
+        for image in images:
+            self._appendData(image)
+
+        if len(images) > 0:
+            self._viewController.selectedImage = images[0]
+
+        for plan in patient.plans:
+            self._appendData(plan)
+
+        # dynamic sequences
+        for dynSeq in patient.dynamic3DSequences:
+            self._appendData(dynSeq)
+
+        for dynSeq in patient.dynamic2DSequences:
+            self._appendData(dynSeq)
+
+        # dynamic models
+        for model in self._currentPatient.dynamic3DModels:
+            serieRoot = PatientDataItem(model)
+            for field in model.deformationList:
+                item = PatientDataItem(field)
+                serieRoot.appendRow(item)
+            self.rootNode.appendRow(serieRoot)
+
+    def _disconnectCurrentPatientAndItems(self):
+        # Disconnect signals
+        if not (self._currentPatient is None):
+            self._currentPatient.patientDataAddedSignal.disconnect(self._appendData)
+            self._currentPatient.patientDataRemovedSignal.disconnect(self._removeData)
+
+        # Do this explicitely to be sure signals are disconnected
+        for row in range(self.model().rowCount()):
+            item = self.model().itemFromIndex(self.model().index(row, 0))
+            if isinstance(item, PatientDataItem):
+                item.disconnectAll()
+
+    def dragEnterEvent(self, event):
+        selection = self.selectionModel().selectedIndexes()[0]
+        self._viewController.selectedImage = self.model().itemFromIndex(selection).data
+
+    def _handleDoubleClick(self, selection):
+        selectedData = self.model().itemFromIndex(selection).data
+
+        if isinstance(selectedData, CTImage) or isinstance(selectedData, Dynamic3DSequence) or isinstance(selectedData, Dynamic2DSequence) or isinstance(selectedData, Image2D):
+            self._viewController.mainImage = selectedData
+        if isinstance(selectedData, RTPlan):
+            self._viewController.plan = selectedData
+        elif isinstance(selectedData, Dynamic3DModel):
+            self._viewController.mainImage = selectedData.midp
+        elif isinstance(selectedData, DoseImage):
+            self._viewController.secondaryImage = selectedData
+
+    def _handleRightClick(self, pos):
+        pos = self.mapToGlobal(pos)
+
+        selected = self.selectedIndexes()
+        selectedData = [self.model().itemFromIndex(selectedData).data for selectedData in selected]
+
+        dataMenu = PatientDataMenu(self._viewController, self)
+        dataMenu.selectedData = selectedData
+        dataMenu.asContextMenu().popup(pos)
+
+
+
+## ------------------------------------------------------------------------------------------
+class PatientDataItem(QStandardItem):
+    def __init__(self, data, txt="", dataType="", color=QColor(75, 75, 75)):
+        QStandardItem.__init__(self)
+
+
+        # print('in patientDataSelection.py, PatientDataItem init', type(data), data.getTypeAsString())
+        self.data = data
+        # print(data.__dict__)
+        self.data.nameChangedSignal.connect(self.setName)
+
+        self.setEditable(False)
+
+        defaultColor = color
+        dynSeqColor = QColor(109, 119, 125)
+        planColor = QColor(56, 130, 176)
+        doseColor = QColor(166, 63, 104)
+        modelColor = QColor(194, 130, 35)
+        vectorFieldColor = QColor(201, 111, 50)
+
+        if isinstance(data, CTImage):
+            self.setName('CT' + ' - ' + self.data.name)
+            self.setForeground(defaultColor)
+        elif isinstance(data, Dynamic3DSequence):
+            self.setName('3D Seq' + ' - ' + self.data.name)
+            self.setForeground(dynSeqColor)
+        elif isinstance(data, Dynamic2DSequence):
+            self.setName('2D Seq' + ' - ' + self.data.name)
+            self.setForeground(dynSeqColor)
+        elif isinstance(data, Image2D):
+            self.setName('2D Img' + ' - ' + self.data.name)
+            self.setForeground(defaultColor)
+        elif isinstance(data, RTPlan):
+            self.setName('plan' + ' - ' + self.data.name)
+            self.setForeground(planColor)
+        elif isinstance(data, Dynamic3DModel):
+            self.setName('DynMod' + ' - ' + self.data.name)
+            self.setForeground(modelColor)
+        elif isinstance(data, VectorField3D):
+            self.setName('Vec Field' + ' - ' + self.data.name)
+            self.setForeground(vectorFieldColor)
+        elif isinstance(data, DoseImage):
+            self.setName('Dose' + ' - ' + self.data.name)
+            self.setForeground(doseColor)
+        else:
+            self.setName(data.getTypeAsString() + ' - ' + self.data.name)
+            self.setForeground(defaultColor)
+
+        # self.setText(txt)
+        # self.setWhatsThis(type)
+
+    def disconnectAll(self):
+        self.data.nameChangedSignal.disconnect(self.setName)
+
+    # No effect: it seems that C destructor of QStandardItem does not trigger __del__
+    def __del__(self):
+        self.disconnectAll()
+
+    def setName(self, name):
+        self.setText(name)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/roiPanel.py` & `opentps_gui-1.0.5/opentps/gui/panels/roiPanel.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from PyQt5.QtWidgets import *
-from PyQt5.QtGui import QColor, QPixmap, QIcon
-
-from opentps.core.data.images import ROIMask
-from opentps.core.data._patient import Patient
-from opentps.core.data._roiContour import ROIContour
-from opentps.core.data._rtStruct import RTStruct
-from opentps.gui.viewer.dataForViewer.ROIContourForViewer import ROIContourForViewer
-from opentps.gui.viewer.dataForViewer.ROIMaskForViewer import ROIMaskForViewer
-
-
-class ROIPanel(QWidget):
-  def __init__(self, viewController):
-    QWidget.__init__(self)
-
-    self.items = []
-    self.layout = QVBoxLayout()
-    self._patient = None
-    self._viewController = viewController
-
-    self.setLayout(self.layout)
-
-    self._filterEdit = QLineEdit(self)
-    self._filterEdit.setPlaceholderText('Filter')
-    self._filterEdit.textEdited.connect(self._setFilteredROIs)
-    self.layout.addWidget(self._filterEdit)
-
-    self._listFrame = QFrame(self)
-    self.layout.addWidget(self._listFrame)
-    self._listLayout = QVBoxLayout()
-    self._listFrame.setLayout(self._listLayout)
-
-    self.layout.addStretch()
-
-    self.setCurrentPatient(self._viewController.currentPatient)
-    self._viewController.currentPatientChangedSignal.connect(self.setCurrentPatient)
-
-  def setCurrentPatient(self, patient:Patient):
-    if patient==self._patient:
-      return
-    elif not self._patient is None:
-      self._patient.rtStructAddedSignal.disconnect(self._setFilteredROIs)
-      self._patient.rtStructRemovedSignal.disconnect(self._setFilteredROIs)
-      self._patient.roiMaskAddedSignal.disconnect(self._setFilteredROIs)
-      self._patient.roiMaskRemovedSignal.disconnect(self._setFilteredROIs)
-
-      self._resetList()
-
-    self._patient = patient
-
-    self._setFilteredROIs()
-
-    if not (self._patient is None):
-      self._patient.rtStructAddedSignal.connect(self._setFilteredROIs)
-      self._patient.rtStructRemovedSignal.connect(self._setFilteredROIs)
-      self._patient.roiMaskAddedSignal.connect(self._setFilteredROIs)
-      self._patient.roiMaskRemovedSignal.connect(self._setFilteredROIs)
-
-  def _resetList(self):
-    for widget in self.items:
-      if isinstance(widget, ROIItem):
-        widget.setVisible(False)
-        self._listLayout.removeWidget(widget)
-    self.items = []
-
-  def _setFilteredROIs(self, *args):
-    if self._patient is None:
-      return
-
-    enteredText = self._filterEdit.text().lower()
-
-    self._resetList()
-
-    for rtStruct in self._patient.rtStructs:
-      for contour in rtStruct.contours:
-        if enteredText in contour.name.lower() or enteredText=='':
-          self.addROIContour(contour)
-
-    for roiMask in self._patient.roiMasks:
-      if enteredText in roiMask.name.lower() or enteredText=='':
-        self.addROIMask(roiMask)
-
-  def addROIContour(self, contour:ROIContour):
-      checkbox = ROIItem(ROIContourForViewer(contour), self._viewController)
-
-      self._listLayout.addWidget(checkbox)
-      self.items.append(checkbox)
-
-  def addROIMask(self, roiMask:ROIMask):
-    checkbox = ROIItem(ROIMaskForViewer(roiMask), self._viewController)
-
-    self._listLayout.addWidget(checkbox)
-    self.items.append(checkbox)
-
-  def removeRTStruct(self, rtStruct:RTStruct):
-    for contour in rtStruct.contours:
-      for item in self.items:
-        if item._contour == contour:
-          self._listLayout.removeWidget(item)
-          item.setParent(None)
-          return
-
-  def removeROIMask(self, roiMask:ROIMask):
-    for item in self.items:
-        if item._contour == roiMask:
-          self._listLayout.removeWidget(item)
-          item.setParent(None)
-          return
-
-class ROIItem(QCheckBox):
-  def __init__(self, contour, viewController):
-    super().__init__(contour.name)
-
-    self._contour = contour
-    self._viewController = viewController
-
-    self.setChecked(self._contour.visible)
-
-    self._contour.visibleChangedSignal.connect(self.setChecked)
-
-    self.clicked.connect(lambda c: self.handleClick(c))
-
-    pixmap = QPixmap(100, 100)
-    pixmap.fill(QColor(contour.color[0], contour.color[1], contour.color[2], 255))
-    self.setIcon(QIcon(pixmap))
-
-  @property
-  def contour(self):
-    return self._contour
-
-  def handleClick(self, isChecked):
-    self._contour.visible = isChecked
-    self._viewController.showContour(self._contour.data)
+from PyQt5.QtWidgets import *
+from PyQt5.QtGui import QColor, QPixmap, QIcon
+
+from opentps.core.data.images import ROIMask
+from opentps.core.data._patient import Patient
+from opentps.core.data._roiContour import ROIContour
+from opentps.core.data._rtStruct import RTStruct
+from opentps.gui.viewer.dataForViewer.ROIContourForViewer import ROIContourForViewer
+from opentps.gui.viewer.dataForViewer.ROIMaskForViewer import ROIMaskForViewer
+
+
+class ROIPanel(QWidget):
+  def __init__(self, viewController):
+    QWidget.__init__(self)
+
+    self.items = []
+    self.layout = QVBoxLayout()
+    self._patient = None
+    self._viewController = viewController
+
+    self.setLayout(self.layout)
+
+    self._filterEdit = QLineEdit(self)
+    self._filterEdit.setPlaceholderText('Filter')
+    self._filterEdit.textEdited.connect(self._setFilteredROIs)
+    self.layout.addWidget(self._filterEdit)
+
+    self._listFrame = QFrame(self)
+    self.layout.addWidget(self._listFrame)
+    self._listLayout = QVBoxLayout()
+    self._listFrame.setLayout(self._listLayout)
+
+    self.layout.addStretch()
+
+    self.setCurrentPatient(self._viewController.currentPatient)
+    self._viewController.currentPatientChangedSignal.connect(self.setCurrentPatient)
+
+  def setCurrentPatient(self, patient:Patient):
+    if patient==self._patient:
+      return
+    elif not self._patient is None:
+      self._patient.rtStructAddedSignal.disconnect(self._setFilteredROIs)
+      self._patient.rtStructRemovedSignal.disconnect(self._setFilteredROIs)
+      self._patient.roiMaskAddedSignal.disconnect(self._setFilteredROIs)
+      self._patient.roiMaskRemovedSignal.disconnect(self._setFilteredROIs)
+
+      self._resetList()
+
+    self._patient = patient
+
+    self._setFilteredROIs()
+
+    if not (self._patient is None):
+      self._patient.rtStructAddedSignal.connect(self._setFilteredROIs)
+      self._patient.rtStructRemovedSignal.connect(self._setFilteredROIs)
+      self._patient.roiMaskAddedSignal.connect(self._setFilteredROIs)
+      self._patient.roiMaskRemovedSignal.connect(self._setFilteredROIs)
+
+  def _resetList(self):
+    for widget in self.items:
+      if isinstance(widget, ROIItem):
+        widget.setVisible(False)
+        self._listLayout.removeWidget(widget)
+    self.items = []
+
+  def _setFilteredROIs(self, *args):
+    if self._patient is None:
+      return
+
+    enteredText = self._filterEdit.text().lower()
+
+    self._resetList()
+
+    for rtStruct in self._patient.rtStructs:
+      for contour in rtStruct.contours:
+        if enteredText in contour.name.lower() or enteredText=='':
+          self.addROIContour(contour)
+
+    for roiMask in self._patient.roiMasks:
+      if enteredText in roiMask.name.lower() or enteredText=='':
+        self.addROIMask(roiMask)
+
+  def addROIContour(self, contour:ROIContour):
+      checkbox = ROIItem(ROIContourForViewer(contour), self._viewController)
+
+      self._listLayout.addWidget(checkbox)
+      self.items.append(checkbox)
+
+  def addROIMask(self, roiMask:ROIMask):
+    checkbox = ROIItem(ROIMaskForViewer(roiMask), self._viewController)
+
+    self._listLayout.addWidget(checkbox)
+    self.items.append(checkbox)
+
+  def removeRTStruct(self, rtStruct:RTStruct):
+    for contour in rtStruct.contours:
+      for item in self.items:
+        if item._contour == contour:
+          self._listLayout.removeWidget(item)
+          item.setParent(None)
+          return
+
+  def removeROIMask(self, roiMask:ROIMask):
+    for item in self.items:
+        if item._contour == roiMask:
+          self._listLayout.removeWidget(item)
+          item.setParent(None)
+          return
+
+class ROIItem(QCheckBox):
+  def __init__(self, contour, viewController):
+    super().__init__(contour.name)
+
+    self._contour = contour
+    self._viewController = viewController
+
+    self.setChecked(self._contour.visible)
+
+    self._contour.visibleChangedSignal.connect(self.setChecked)
+
+    self.clicked.connect(lambda c: self.handleClick(c))
+
+    pixmap = QPixmap(100, 100)
+    pixmap.fill(QColor(contour.color[0], contour.color[1], contour.color[2], 255))
+    self.setIcon(QIcon(pixmap))
+
+  @property
+  def contour(self):
+    return self._contour
+
+  def handleClick(self, isChecked):
+    self._contour.visible = isChecked
+    self._viewController.showContour(self._contour.data)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/pythonHighlighter.py` & `opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/pythonHighlighter.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-#Sorry, can't find the original authors...
-#Credit is not ours
-
-from PyQt5 import QtGui
-from PyQt5.QtCore import QRegExp
-
-def format(color, style=''):
-    """Return a QTextCharFormat with the given attributes.
-    """
-    _color = QtGui.QColor()
-    _color.setNamedColor(color)
-
-    _format = QtGui.QTextCharFormat()
-    _format.setForeground(_color)
-    if 'bold' in style:
-        _format.setFontWeight(QtGui.QFont.Bold)
-    if 'italic' in style:
-        _format.setFontItalic(True)
-
-    return _format
-
-
-# Syntax styles that can be shared by all languages
-STYLES = {
-    'keyword': format('blue'),
-    'operator': format('red'),
-    'brace': format('darkGray'),
-    'defclass': format('black', 'bold'),
-    'string': format('magenta'),
-    'string2': format('darkMagenta'),
-    'comment': format('darkGreen', 'italic'),
-    'self': format('black', 'italic'),
-    'numbers': format('brown'),
-}
-
-
-class PythonHighlighter (QtGui.QSyntaxHighlighter):
-    """Syntax highlighter for the Python language.
-    """
-    # Python keywords
-    keywords = [
-        'and', 'assert', 'break', 'class', 'continue', 'def',
-        'del', 'elif', 'else', 'except', 'exec', 'finally',
-        'for', 'from', 'global', 'if', 'import', 'in',
-        'is', 'lambda', 'not', 'or', 'pass', 'print',
-        'raise', 'return', 'try', 'while', 'yield',
-        'None', 'True', 'False',
-    ]
-
-    # Python operators
-    operators = [
-        '=',
-        # Comparison
-        '==', '!=', '<', '<=', '>', '>=',
-        # Arithmetic
-        '\+', '-', '\*', '/', '//', '\%', '\*\*',
-        # In-place
-        '\+=', '-=', '\*=', '/=', '\%=',
-        # Bitwise
-        '\^', '\|', '\&', '\~', '>>', '<<',
-    ]
-
-    # Python braces
-    braces = [
-        '\{', '\}', '\(', '\)', '\[', '\]',
-    ]
-
-    def __init__(self, parent: QtGui.QTextDocument) -> None:
-        super().__init__(parent)
-
-        # Multi-line strings (expression, flag, style)
-        self.tri_single = (QRegExp("'''"), 1, STYLES['string2'])
-        self.tri_double = (QRegExp('"""'), 2, STYLES['string2'])
-
-        rules = []
-
-        # Keyword, operator, and brace rules
-        rules += [(r'\b%s\b' % w, 0, STYLES['keyword'])
-            for w in PythonHighlighter.keywords]
-        rules += [(r'%s' % o, 0, STYLES['operator'])
-            for o in PythonHighlighter.operators]
-        rules += [(r'%s' % b, 0, STYLES['brace'])
-            for b in PythonHighlighter.braces]
-
-        # All other rules
-        rules += [
-            # 'self'
-            (r'\bself\b', 0, STYLES['self']),
-
-            # 'def' followed by an identifier
-            (r'\bdef\b\s*(\w+)', 1, STYLES['defclass']),
-            # 'class' followed by an identifier
-            (r'\bclass\b\s*(\w+)', 1, STYLES['defclass']),
-
-            # Numeric literals
-            (r'\b[+-]?[0-9]+[lL]?\b', 0, STYLES['numbers']),
-            (r'\b[+-]?0[xX][0-9A-Fa-f]+[lL]?\b', 0, STYLES['numbers']),
-            (r'\b[+-]?[0-9]+(?:\.[0-9]+)?(?:[eE][+-]?[0-9]+)?\b', 0, STYLES['numbers']),
-
-            # Double-quoted string, possibly containing escape sequences
-            (r'"[^"\\]*(\\.[^"\\]*)*"', 0, STYLES['string']),
-            # Single-quoted string, possibly containing escape sequences
-            (r"'[^'\\]*(\\.[^'\\]*)*'", 0, STYLES['string']),
-
-            # From '#' until a newline
-            (r'#[^\n]*', 0, STYLES['comment']),
-        ]
-
-        # Build a QRegExp for each pattern
-        self.rules = [(QRegExp(pat), index, fmt)
-            for (pat, index, fmt) in rules]
-
-    def highlightBlock(self, text):
-        """Apply syntax highlighting to the given block of text.
-        """
-        self.tripleQuoutesWithinStrings = []
-        # Do other syntax formatting
-        for expression, nth, format in self.rules:
-            index = expression.indexIn(text, 0)
-            if index >= 0:
-                # if there is a string we check
-                # if there are some triple quotes within the string
-                # they will be ignored if they are matched again
-                if expression.pattern() in [r'"[^"\\]*(\\.[^"\\]*)*"', r"'[^'\\]*(\\.[^'\\]*)*'"]:
-                    innerIndex = self.tri_single[0].indexIn(text, index + 1)
-                    if innerIndex == -1:
-                        innerIndex = self.tri_double[0].indexIn(text, index + 1)
-
-                    if innerIndex != -1:
-                        tripleQuoteIndexes = range(innerIndex, innerIndex + 3)
-                        self.tripleQuoutesWithinStrings.extend(tripleQuoteIndexes)
-
-            while index >= 0:
-                # skipping triple quotes within strings
-                if index in self.tripleQuoutesWithinStrings:
-                    index += 1
-                    expression.indexIn(text, index)
-                    continue
-
-                # We actually want the index of the nth match
-                index = expression.pos(nth)
-                length = len(expression.cap(nth))
-                self.setFormat(index, length, format)
-                index = expression.indexIn(text, index + length)
-
-        self.setCurrentBlockState(0)
-
-        # Do multi-line strings
-        in_multiline = self.match_multiline(text, *self.tri_single)
-        if not in_multiline:
-            in_multiline = self.match_multiline(text, *self.tri_double)
-
-    def match_multiline(self, text, delimiter, in_state, style):
-        """Do highlighting of multi-line strings. ``delimiter`` should be a
-        ``QRegExp`` for triple-single-quotes or triple-double-quotes, and
-        ``in_state`` should be a unique integer to represent the corresponding
-        state changes when inside those strings. Returns True if we're still
-        inside a multi-line string when this function is finished.
-        """
-        # If inside triple-single quotes, start at 0
-        if self.previousBlockState() == in_state:
-            start = 0
-            add = 0
-        # Otherwise, look for the delimiter on this line
-        else:
-            start = delimiter.indexIn(text)
-            # skipping triple quotes within strings
-            if start in self.tripleQuoutesWithinStrings:
-                return False
-            # Move past this match
-            add = delimiter.matchedLength()
-
-        # As long as there's a delimiter match on this line...
-        while start >= 0:
-            # Look for the ending delimiter
-            end = delimiter.indexIn(text, start + add)
-            # Ending delimiter on this line?
-            if end >= add:
-                length = end - start + add + delimiter.matchedLength()
-                self.setCurrentBlockState(0)
-            # No; multi-line string
-            else:
-                self.setCurrentBlockState(in_state)
-                length = len(text) - start + add
-            # Apply formatting
-            self.setFormat(start, length, style)
-            # Look for the next match
-            start = delimiter.indexIn(text, start + length)
-
-        # Return True if still inside a multi-line string, False otherwise
-        if self.currentBlockState() == in_state:
-            return True
-        else:
-            return False
+#Sorry, can't find the original authors...
+#Credit is not ours
+
+from PyQt5 import QtGui
+from PyQt5.QtCore import QRegExp
+
+def format(color, style=''):
+    """Return a QTextCharFormat with the given attributes.
+    """
+    _color = QtGui.QColor()
+    _color.setNamedColor(color)
+
+    _format = QtGui.QTextCharFormat()
+    _format.setForeground(_color)
+    if 'bold' in style:
+        _format.setFontWeight(QtGui.QFont.Bold)
+    if 'italic' in style:
+        _format.setFontItalic(True)
+
+    return _format
+
+
+# Syntax styles that can be shared by all languages
+STYLES = {
+    'keyword': format('blue'),
+    'operator': format('red'),
+    'brace': format('darkGray'),
+    'defclass': format('black', 'bold'),
+    'string': format('magenta'),
+    'string2': format('darkMagenta'),
+    'comment': format('darkGreen', 'italic'),
+    'self': format('black', 'italic'),
+    'numbers': format('brown'),
+}
+
+
+class PythonHighlighter (QtGui.QSyntaxHighlighter):
+    """Syntax highlighter for the Python language.
+    """
+    # Python keywords
+    keywords = [
+        'and', 'assert', 'break', 'class', 'continue', 'def',
+        'del', 'elif', 'else', 'except', 'exec', 'finally',
+        'for', 'from', 'global', 'if', 'import', 'in',
+        'is', 'lambda', 'not', 'or', 'pass', 'print',
+        'raise', 'return', 'try', 'while', 'yield',
+        'None', 'True', 'False',
+    ]
+
+    # Python operators
+    operators = [
+        '=',
+        # Comparison
+        '==', '!=', '<', '<=', '>', '>=',
+        # Arithmetic
+        '\+', '-', '\*', '/', '//', '\%', '\*\*',
+        # In-place
+        '\+=', '-=', '\*=', '/=', '\%=',
+        # Bitwise
+        '\^', '\|', '\&', '\~', '>>', '<<',
+    ]
+
+    # Python braces
+    braces = [
+        '\{', '\}', '\(', '\)', '\[', '\]',
+    ]
+
+    def __init__(self, parent: QtGui.QTextDocument) -> None:
+        super().__init__(parent)
+
+        # Multi-line strings (expression, flag, style)
+        self.tri_single = (QRegExp("'''"), 1, STYLES['string2'])
+        self.tri_double = (QRegExp('"""'), 2, STYLES['string2'])
+
+        rules = []
+
+        # Keyword, operator, and brace rules
+        rules += [(r'\b%s\b' % w, 0, STYLES['keyword'])
+            for w in PythonHighlighter.keywords]
+        rules += [(r'%s' % o, 0, STYLES['operator'])
+            for o in PythonHighlighter.operators]
+        rules += [(r'%s' % b, 0, STYLES['brace'])
+            for b in PythonHighlighter.braces]
+
+        # All other rules
+        rules += [
+            # 'self'
+            (r'\bself\b', 0, STYLES['self']),
+
+            # 'def' followed by an identifier
+            (r'\bdef\b\s*(\w+)', 1, STYLES['defclass']),
+            # 'class' followed by an identifier
+            (r'\bclass\b\s*(\w+)', 1, STYLES['defclass']),
+
+            # Numeric literals
+            (r'\b[+-]?[0-9]+[lL]?\b', 0, STYLES['numbers']),
+            (r'\b[+-]?0[xX][0-9A-Fa-f]+[lL]?\b', 0, STYLES['numbers']),
+            (r'\b[+-]?[0-9]+(?:\.[0-9]+)?(?:[eE][+-]?[0-9]+)?\b', 0, STYLES['numbers']),
+
+            # Double-quoted string, possibly containing escape sequences
+            (r'"[^"\\]*(\\.[^"\\]*)*"', 0, STYLES['string']),
+            # Single-quoted string, possibly containing escape sequences
+            (r"'[^'\\]*(\\.[^'\\]*)*'", 0, STYLES['string']),
+
+            # From '#' until a newline
+            (r'#[^\n]*', 0, STYLES['comment']),
+        ]
+
+        # Build a QRegExp for each pattern
+        self.rules = [(QRegExp(pat), index, fmt)
+            for (pat, index, fmt) in rules]
+
+    def highlightBlock(self, text):
+        """Apply syntax highlighting to the given block of text.
+        """
+        self.tripleQuoutesWithinStrings = []
+        # Do other syntax formatting
+        for expression, nth, format in self.rules:
+            index = expression.indexIn(text, 0)
+            if index >= 0:
+                # if there is a string we check
+                # if there are some triple quotes within the string
+                # they will be ignored if they are matched again
+                if expression.pattern() in [r'"[^"\\]*(\\.[^"\\]*)*"', r"'[^'\\]*(\\.[^'\\]*)*'"]:
+                    innerIndex = self.tri_single[0].indexIn(text, index + 1)
+                    if innerIndex == -1:
+                        innerIndex = self.tri_double[0].indexIn(text, index + 1)
+
+                    if innerIndex != -1:
+                        tripleQuoteIndexes = range(innerIndex, innerIndex + 3)
+                        self.tripleQuoutesWithinStrings.extend(tripleQuoteIndexes)
+
+            while index >= 0:
+                # skipping triple quotes within strings
+                if index in self.tripleQuoutesWithinStrings:
+                    index += 1
+                    expression.indexIn(text, index)
+                    continue
+
+                # We actually want the index of the nth match
+                index = expression.pos(nth)
+                length = len(expression.cap(nth))
+                self.setFormat(index, length, format)
+                index = expression.indexIn(text, index + length)
+
+        self.setCurrentBlockState(0)
+
+        # Do multi-line strings
+        in_multiline = self.match_multiline(text, *self.tri_single)
+        if not in_multiline:
+            in_multiline = self.match_multiline(text, *self.tri_double)
+
+    def match_multiline(self, text, delimiter, in_state, style):
+        """Do highlighting of multi-line strings. ``delimiter`` should be a
+        ``QRegExp`` for triple-single-quotes or triple-double-quotes, and
+        ``in_state`` should be a unique integer to represent the corresponding
+        state changes when inside those strings. Returns True if we're still
+        inside a multi-line string when this function is finished.
+        """
+        # If inside triple-single quotes, start at 0
+        if self.previousBlockState() == in_state:
+            start = 0
+            add = 0
+        # Otherwise, look for the delimiter on this line
+        else:
+            start = delimiter.indexIn(text)
+            # skipping triple quotes within strings
+            if start in self.tripleQuoutesWithinStrings:
+                return False
+            # Move past this match
+            add = delimiter.matchedLength()
+
+        # As long as there's a delimiter match on this line...
+        while start >= 0:
+            # Look for the ending delimiter
+            end = delimiter.indexIn(text, start + add)
+            # Ending delimiter on this line?
+            if end >= add:
+                length = end - start + add + delimiter.matchedLength()
+                self.setCurrentBlockState(0)
+            # No; multi-line string
+            else:
+                self.setCurrentBlockState(in_state)
+                length = len(text) - start + add
+            # Apply formatting
+            self.setFormat(start, length, style)
+            # Look for the next match
+            start = delimiter.indexIn(text, start + length)
+
+        # Return True if still inside a multi-line string, False otherwise
+        if self.currentBlockState() == in_state:
+            return True
+        else:
+            return False
```

### Comparing `opentps-gui-1.0.4/opentps/gui/panels/scriptingPanel/scriptingPanel.py` & `opentps_gui-1.0.5/opentps/gui/panels/scriptingPanel/scriptingPanel.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import os
-
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QPushButton, QFrame, QMessageBox, QFileDialog, QLabel, QHBoxLayout
-
-from opentps.core import APIInterpreter
-from opentps.gui.panels.scriptingPanel.scriptingWindow import ScriptingWindow
-
-
-class ScriptingPanel(QWidget):
-    newScriptingWindowSignal = pyqtSignal()
-
-    def __init__(self):
-        QWidget.__init__(self)
-
-        self._layout = QVBoxLayout()
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self.setLayout(self._layout)
-
-        self._newScriptingWindowButton = QPushButton('New scripting window')
-        self._newScriptingWindowButton.clicked.connect(self.newScriptingWindow)
-        self._layout.addWidget(self._newScriptingWindowButton)
-
-        self._newScriptFileViewButton = QPushButton('Select new script file')
-        self._newScriptFileViewButton.clicked.connect(self.newScriptFile)
-        self._layout.addWidget(self._newScriptFileViewButton)
-
-        self._scriptFileViewsFrame = QFrame()
-        self._scriptFileViewsFrame.setFrameShape(QFrame.StyledPanel)
-        self._layout.addWidget(self._scriptFileViewsFrame)
-
-        self._scriptFileViewsLayout = QVBoxLayout()
-        self._scriptFileViewsLayout.setContentsMargins(0, 0, 0, 0)
-        self._scriptFileViewsFrame.setLayout(self._scriptFileViewsLayout)
-
-        self._layout.addStretch()
-
-    def newScriptingWindow(self):
-        self.scriptingWindow = ScriptingWindow()
-        self.scriptingWindow.show()
-
-    def newScriptFile(self):
-        self._scriptFileViewsLayout.addWidget(ScriptingFileView())
-
-
-class ScriptingFileView(QWidget):
-    _scriptPath = None
-
-    def __init__(self):
-        QWidget.__init__(self)
-
-        self._layout = QVBoxLayout()
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self.setLayout(self._layout)
-
-        self._topFrame = QFrame()
-        self._topFrame.setFrameShape(QFrame.StyledPanel)
-        self._layout.addWidget(self._topFrame)
-
-        self._bottomFrame = QFrame()
-        self._bottomFrame.setFrameShape(QFrame.StyledPanel)
-        self._layout.addWidget(self._bottomFrame)
-
-        topLayout = QHBoxLayout()
-        topLayout.setContentsMargins(0, 0, 0, 0)
-        self._topFrame.setLayout(topLayout)
-
-        bottomLayout = QHBoxLayout()
-        bottomLayout.setContentsMargins(0, 0, 0, 0)
-        self._bottomFrame.setLayout(bottomLayout)
-
-        closeButton = QPushButton('X')
-        closeButton.clicked.connect(self.close)
-
-        selectFileButton = QPushButton('Select file')
-        selectFileButton.clicked.connect(self._selectAndSetFile)
-
-        runButton = QPushButton('Run')
-        runButton.clicked.connect(self._runFile)
-
-        topLayout.addWidget(closeButton)
-        topLayout.addWidget(selectFileButton)
-        topLayout.addWidget(runButton)
-
-        self._fileNameLabel = QLabel()
-        bottomLayout.addWidget(self._fileNameLabel)
-
-    def close(self):
-        self.setParent(None)
-
-    def _selectAndSetFile(self):
-        self._scriptPath = self._openFileSelection()
-        self._setFileNameLabel()
-
-    def _openFileSelection(self):
-        filePath, _ = QFileDialog.getOpenFileName(self, "Select a python script", self._scriptPath, "python script (*.py)")
-        return filePath
-
-    def _setFileNameLabel(self):
-        self._fileNameLabel.setText(os.path.basename(self._scriptPath))
-
-    def _runFile(self):
-        msg = QMessageBox()
-        msg.setWindowTitle(os.path.basename(self._scriptPath))
-        msg.setIcon(QMessageBox.Information)
-
-        code = self._readFile()
-
-        try:
-            output = APIInterpreter.run(code)
-            msg.setText(output)
-        except Exception as err:
-            msg.setText(format(err))
-            raise err from err
-
-        msg.exec_()
-
-    def _readFile(self):
-        code = ''
-
-        with open(self._scriptPath, 'r') as file:
-            code = file.read()
-
-        return code
+import os
+
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QPushButton, QFrame, QMessageBox, QFileDialog, QLabel, QHBoxLayout
+
+from opentps.core import APIInterpreter
+from opentps.gui.panels.scriptingPanel.scriptingWindow import ScriptingWindow
+
+
+class ScriptingPanel(QWidget):
+    newScriptingWindowSignal = pyqtSignal()
+
+    def __init__(self):
+        QWidget.__init__(self)
+
+        self._layout = QVBoxLayout()
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(self._layout)
+
+        self._newScriptingWindowButton = QPushButton('New scripting window')
+        self._newScriptingWindowButton.clicked.connect(self.newScriptingWindow)
+        self._layout.addWidget(self._newScriptingWindowButton)
+
+        self._newScriptFileViewButton = QPushButton('Select new script file')
+        self._newScriptFileViewButton.clicked.connect(self.newScriptFile)
+        self._layout.addWidget(self._newScriptFileViewButton)
+
+        self._scriptFileViewsFrame = QFrame()
+        self._scriptFileViewsFrame.setFrameShape(QFrame.StyledPanel)
+        self._layout.addWidget(self._scriptFileViewsFrame)
+
+        self._scriptFileViewsLayout = QVBoxLayout()
+        self._scriptFileViewsLayout.setContentsMargins(0, 0, 0, 0)
+        self._scriptFileViewsFrame.setLayout(self._scriptFileViewsLayout)
+
+        self._layout.addStretch()
+
+    def newScriptingWindow(self):
+        self.scriptingWindow = ScriptingWindow()
+        self.scriptingWindow.show()
+
+    def newScriptFile(self):
+        self._scriptFileViewsLayout.addWidget(ScriptingFileView())
+
+
+class ScriptingFileView(QWidget):
+    _scriptPath = None
+
+    def __init__(self):
+        QWidget.__init__(self)
+
+        self._layout = QVBoxLayout()
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(self._layout)
+
+        self._topFrame = QFrame()
+        self._topFrame.setFrameShape(QFrame.StyledPanel)
+        self._layout.addWidget(self._topFrame)
+
+        self._bottomFrame = QFrame()
+        self._bottomFrame.setFrameShape(QFrame.StyledPanel)
+        self._layout.addWidget(self._bottomFrame)
+
+        topLayout = QHBoxLayout()
+        topLayout.setContentsMargins(0, 0, 0, 0)
+        self._topFrame.setLayout(topLayout)
+
+        bottomLayout = QHBoxLayout()
+        bottomLayout.setContentsMargins(0, 0, 0, 0)
+        self._bottomFrame.setLayout(bottomLayout)
+
+        closeButton = QPushButton('X')
+        closeButton.clicked.connect(self.close)
+
+        selectFileButton = QPushButton('Select file')
+        selectFileButton.clicked.connect(self._selectAndSetFile)
+
+        runButton = QPushButton('Run')
+        runButton.clicked.connect(self._runFile)
+
+        topLayout.addWidget(closeButton)
+        topLayout.addWidget(selectFileButton)
+        topLayout.addWidget(runButton)
+
+        self._fileNameLabel = QLabel()
+        bottomLayout.addWidget(self._fileNameLabel)
+
+    def close(self):
+        self.setParent(None)
+
+    def _selectAndSetFile(self):
+        self._scriptPath = self._openFileSelection()
+        self._setFileNameLabel()
+
+    def _openFileSelection(self):
+        filePath, _ = QFileDialog.getOpenFileName(self, "Select a python script", self._scriptPath, "python script (*.py)")
+        return filePath
+
+    def _setFileNameLabel(self):
+        self._fileNameLabel.setText(os.path.basename(self._scriptPath))
+
+    def _runFile(self):
+        msg = QMessageBox()
+        msg.setWindowTitle(os.path.basename(self._scriptPath))
+        msg.setIcon(QMessageBox.Information)
+
+        code = self._readFile()
+
+        try:
+            output = APIInterpreter.run(code)
+            msg.setText(output)
+        except Exception as err:
+            msg.setText(format(err))
+            raise err from err
+
+        msg.exec_()
+
+    def _readFile(self):
+        code = ''
+
+        with open(self._scriptPath, 'r') as file:
+            code = file.read()
+
+        return code
```

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/OpenTPS_icon.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/OpenTPS_icon.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/arrow-135.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/arrow-135.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/chain-unchain.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/chain-unchain.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/chart.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/chart.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/color-adjustment.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/color-adjustment.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/color.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/color.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/colormap_histogram.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/colormap_histogram.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/colormap_jet.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/colormap_jet.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/contrast.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/contrast.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/crop.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/crop.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/cross.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/cross.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/cube.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/cube.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/dvh.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/dvh.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/fast.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/fast.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/folder-open.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/folder-open.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/graph.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/graph.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/iba_nozzle.stl` & `opentps_gui-1.0.5/opentps/gui/res/icons/iba_nozzle.stl`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/independent_views.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/independent_views.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/pause.jpg` & `opentps_gui-1.0.5/opentps/gui/res/icons/pause.jpg`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/pencil--plus.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/pencil--plus.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/play.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/play.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/profile.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/profile.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/reload.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/reload.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/resample.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/resample.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/save.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/save.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/slider.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/slider.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/slow.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/slow.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/tick-button.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/tick-button.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/icons/x-ray.png` & `opentps_gui-1.0.5/opentps/gui/res/icons/x-ray.png`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/res/viewer/human_standing.stl` & `opentps_gui-1.0.5/opentps/gui/res/viewer/human_standing.stl`

 * *Files identical despite different names*

### Comparing `opentps-gui-1.0.4/opentps/gui/tools/_cropTool.py` & `opentps_gui-1.0.5/opentps/gui/tools/_cropTool.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,276 +1,276 @@
-
-__docformat__ = "restructuredtext en"
-__all__ = ['CropWidget']
-
-from typing import Optional, Sequence
-
-import numpy as np
-from PyQt5.QtWidgets import QWidget, QHBoxLayout, QMainWindow, QVBoxLayout, QPushButton, QLabel, QFrame
-from vtkmodules import vtkCommonMath
-from vtkmodules.vtkInteractionWidgets import vtkBoxWidget2, vtkBoxRepresentation
-
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.processing.imageProcessing.resampler3D import crop3DDataAroundBox
-from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
-from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
-from opentps.gui.viewer.dataViewer import DroppedObject
-
-
-class CropWidget(QMainWindow):
-    def __init__(self, viewController, parent=None):
-        super().__init__(parent)
-
-        self._viewController = viewController
-
-        self.setWindowTitle('Crop tool')
-        self.resize(800, 600)
-
-        centralWidget = QWidget()
-        self.setCentralWidget(centralWidget)
-        self._mainLayout = QHBoxLayout()
-        centralWidget.setLayout(self._mainLayout)
-
-        self._viewers = ThreeViewsGrid(self._viewController)
-
-        self._dragLabel = QLabel("Select as many images as you want to crop.\nDrop the image needed to create a box.", self)
-        self._dragLabel.setWordWrap(True)
-
-        self._cropDataButton = QPushButton('Crop all selected data')
-        self._cropDataButton.clicked.connect(self._cropData)
-
-        self._dataSelection = PatientDataSelection(self._viewController, self)
-
-        self._menuFrame = QFrame(self)
-        self._menuFrame.setFixedWidth(200)
-        self._menuLayout = QVBoxLayout(self._menuFrame)
-        self._menuFrame.setLayout(self._menuLayout)
-
-        self._mainLayout.addWidget(self._menuFrame)
-        self._menuLayout.addWidget(self._dragLabel)
-        self._menuLayout.addWidget(self._dataSelection)
-        self._menuLayout.addWidget(self._cropDataButton)
-        self._mainLayout.addWidget(self._viewers)
-
-    def closeEvent(self, event):
-        self._viewers.close()
-        super().closeEvent(event)
-
-    def _cropData(self):
-        selectedData = self._dataSelection.selectedData
-
-        box = self._viewers.getBoundingBox()
-
-        xx = np.array([box[0], box[1]])
-        yy = np.array([box[2], box[3]])
-        zz = np.array([box[4], box[5]])
-
-        box = [[xx.min(), xx.max()], [yy.min(), yy.max()], [zz.min(), zz.max()]]
-
-        for data in selectedData:
-            crop3DDataAroundBox(data, box, marginInMM=[0, 0, 0])
-
-
-class ThreeViewsGrid(QWidget):
-    def __init__(self, viewController):
-        super().__init__()
-
-        self._viewController = viewController
-
-        self._mainLayout = QHBoxLayout(self)
-        self.setLayout(self._mainLayout)
-
-        self._viewer0 = Image3DViewer(viewController)
-        self._viewer1 = Image3DViewer(viewController)
-        self._viewer2 = Image3DViewer(viewController)
-
-        self._viewer0.viewType = Image3DViewer.ViewerTypes.CORONAL
-        self._viewer1.viewType = Image3DViewer.ViewerTypes.AXIAL
-        self._viewer2.viewType = Image3DViewer.ViewerTypes.SAGITTAL
-
-        self._viewer0.crossHairEnabled = True
-        self._viewer1.crossHairEnabled = True
-        self._viewer2.crossHairEnabled = True
-
-        self._mainLayout.addWidget(self._viewer0)
-        self._mainLayout.addWidget(self._viewer1)
-        self._mainLayout.addWidget(self._viewer2)
-
-        self.setAcceptDrops(True)
-        self.dragEnterEvent = lambda event: event.accept()
-        self.dropEvent = lambda event: self._dropEvent(event)
-
-    def close(self):
-        self._viewer0.close()
-        self._viewer1.close()
-        self._viewer2.close()
-
-    def _dropEvent(self, e):
-        if e.mimeData().hasText():
-            droppedIsImage = e.mimeData().text() == DroppedObject.DropTypes.IMAGE
-
-            if droppedIsImage:
-                e.accept()
-                self._setMainImage(self._viewController.selectedImage)
-                return
-        e.ignore()
-
-
-    def _setMainImage(self, image: Optional[Image3D]):
-        if isinstance(image, Image3D) or (image is None):
-            self._viewer0.primaryImage = image
-            self._viewer1.primaryImage = image
-            self._viewer2.primaryImage = image
-
-            interactor0 = self._viewer0._renderWindow.GetInteractor()
-            interactor1 = self._viewer1._renderWindow.GetInteractor()
-            interactor2 = self._viewer2._renderWindow.GetInteractor()
-
-            self.boxRep0 = vtkBoxRepresentation()
-            self.boxRep0.SetPlaceFactor(1)
-            self.boxRep0.PlaceWidget(self._viewer0._primaryImageLayer._mainActor.GetBounds())
-
-            self.boxRep1 = vtkBoxRepresentation()
-            self.boxRep1.SetPlaceFactor(1)
-            self.boxRep1.PlaceWidget(self._viewer1._primaryImageLayer._mainActor.GetBounds())
-
-            self.boxRep2 = vtkBoxRepresentation()
-            self.boxRep2.SetPlaceFactor(1)
-            self.boxRep2.PlaceWidget(self._viewer2._primaryImageLayer._mainActor.GetBounds())
-
-
-            self.boxWidget0 = vtkBoxWidget2()
-            self.boxWidget0.SetRotationEnabled(False)
-            self.boxWidget0.SetInteractor(interactor0)
-            self.boxWidget0.SetRepresentation(self.boxRep0)
-            self.boxWidget0.On()
-
-            self.boxWidget1 = vtkBoxWidget2()
-            self.boxWidget1.SetRotationEnabled(False)
-            self.boxWidget1.SetInteractor(interactor1)
-            self.boxWidget1.SetRepresentation(self.boxRep1)
-            self.boxWidget1.On()
-
-            self.boxWidget2 = vtkBoxWidget2()
-            self.boxWidget2.SetRotationEnabled(False)
-            self.boxWidget2.SetInteractor(interactor2)
-            self.boxWidget2.SetRepresentation(self.boxRep2)
-            self.boxWidget2.On()
-
-            self._viewer0._renderWindow.Render()
-            self._viewer1._renderWindow.Render()
-            self._viewer2._renderWindow.Render()
-
-            interactor0.Start()
-            interactor1.Start()
-            interactor2.Start()
-
-            self.boxWidget0.AddObserver('InteractionEvent', self.onInteraction0)
-            self.boxWidget1.AddObserver('InteractionEvent', self.onInteraction1)
-            self.boxWidget2.AddObserver('InteractionEvent', self.onInteraction2)
-
-    def onInteraction0(self, obj, event):
-        self.boxRep1.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer0, self.boxRep0, self._viewer1, self.boxRep1))
-        self.boxRep2.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer0, self.boxRep0, self._viewer2, self.boxRep2))
-        self._viewer1._renderWindow.Render()
-        self._viewer2._renderWindow.Render()
-
-    def onInteraction1(self, obj, event):
-        self.boxRep0.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer1, self.boxRep1, self._viewer0, self.boxRep0))
-        self.boxRep2.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer1, self.boxRep1, self._viewer2, self.boxRep2))
-        self._viewer0._renderWindow.Render()
-        self._viewer2._renderWindow.Render()
-
-    def onInteraction2(self, obj, event):
-        self.boxRep0.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer2, self.boxRep2, self._viewer0, self.boxRep0))
-        self.boxRep1.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer2, self.boxRep2, self._viewer1, self.boxRep1))
-        self._viewer0._renderWindow.Render()
-        self._viewer1._renderWindow.Render()
-
-    def _2DboundsFromViewerToViewer(self, viewer0:Image3DViewer, boxRep0, viewer1:Image3DViewer, boxRep1) -> Sequence[float]:
-        bounds = self._boundsFromViewerToViewer(viewer0, boxRep0, viewer1, boxRep1)
-        return [bounds[0], bounds[1], bounds[2], bounds[3], 0, 0]
-
-    def _boundsFromViewerToViewer(self, viewer0:Image3DViewer, boxRep0, viewer1:Image3DViewer, boxRep1) -> Sequence[float]:
-        bounds0 = boxRep0.GetBounds()
-        bounds1 = boxRep1.GetBounds()
-
-        corner0Odd = [bounds0[0], bounds0[2], bounds0[4]]
-        corner0Even = [bounds0[1], bounds0[3], bounds0[5]]
-
-        corner1Odd = [bounds1[0], bounds1[2], bounds1[4]]
-        corner1Even = [bounds1[1], bounds1[3], bounds1[5]]
-
-
-        tform0 = vtkCommonMath.vtkMatrix4x4()
-        tform0.DeepCopy(viewer0._viewMatrix)
-
-        tform0Inverted = vtkCommonMath.vtkMatrix4x4()
-        tform0Inverted.DeepCopy(viewer0._viewMatrix)
-        tform0Inverted.Invert()
-
-        tform1 = vtkCommonMath.vtkMatrix4x4()
-        tform1.DeepCopy(viewer1._viewMatrix)
-
-        tform1Inverted = vtkCommonMath.vtkMatrix4x4()
-        tform1Inverted.DeepCopy(viewer1._viewMatrix)
-        tform1Inverted.Invert()
-
-        corner1Odd_2 = tform1.MultiplyPoint((corner1Odd[0], corner1Odd[1], corner1Odd[2], 1))
-        corner1Odd_2 = tform0Inverted.MultiplyPoint((corner1Odd_2[0], corner1Odd_2[1], corner1Odd_2[2], 1))
-
-        corner0OddTransformed = tform0.MultiplyPoint((corner0Odd[0], corner0Odd[1], corner1Odd_2[2], 1))
-
-        corner0Odd_2 = tform1Inverted.MultiplyPoint((corner0OddTransformed[0], corner0OddTransformed[1], corner0OddTransformed[2], 1))
-
-        corner1Even_2 = tform1.MultiplyPoint((corner1Even[0], corner1Even[1], corner1Even[2], 1))
-        corner1Even_2 = tform0Inverted.MultiplyPoint((corner1Even_2[0], corner1Even_2[1], corner1Even_2[2], 1))
-
-        corner0EvenTransformed = tform0.MultiplyPoint((corner0Even[0], corner0Even[1], corner1Even_2[2], 1))
-
-        corner0Even_2 = tform1Inverted.MultiplyPoint((corner0EvenTransformed[0], corner0EvenTransformed[1], corner0EvenTransformed[2], 1))
-
-        return [corner0Odd_2[0], corner0Even_2[0], corner0Odd_2[1], corner0Even_2[1], corner0Odd_2[2], corner0Even_2[2]]
-
-
-    def getBoundingBox(self):
-        viewer0 = self._viewer0
-        viewer1 = self._viewer1
-
-        boxRep0 = self.boxRep0
-        boxRep1 = self.boxRep1
-
-        bounds0 = boxRep0.GetBounds()
-        bounds1 = boxRep1.GetBounds()
-
-        corner0Odd = [bounds0[0], bounds0[2], bounds0[4]]
-        corner0Even = [bounds0[1], bounds0[3], bounds0[5]]
-
-        corner1Odd = [bounds1[0], bounds1[2], bounds1[4]]
-        corner1Even = [bounds1[1], bounds1[3], bounds1[5]]
-
-        tform0 = vtkCommonMath.vtkMatrix4x4()
-        tform0.DeepCopy(viewer0._viewMatrix)
-
-        tform0Inverted = vtkCommonMath.vtkMatrix4x4()
-        tform0Inverted.DeepCopy(viewer0._viewMatrix)
-        tform0Inverted.Invert()
-
-        tform1 = vtkCommonMath.vtkMatrix4x4()
-        tform1.DeepCopy(viewer1._viewMatrix)
-
-        tform1Inverted = vtkCommonMath.vtkMatrix4x4()
-        tform1Inverted.DeepCopy(viewer1._viewMatrix)
-        tform1Inverted.Invert()
-
-        corner1Odd_2 = tform1.MultiplyPoint((corner1Odd[0], corner1Odd[1], corner1Odd[2], 1))
-        corner1Odd_2 = tform0Inverted.MultiplyPoint((corner1Odd_2[0], corner1Odd_2[1], corner1Odd_2[2], 1))
-
-        corner0OddTransformed = tform0.MultiplyPoint((corner0Odd[0], corner0Odd[1], corner1Odd_2[2], 1))
-
-
-        corner1Even_2 = tform1.MultiplyPoint((corner1Even[0], corner1Even[1], corner1Even[2], 1))
-        corner1Even_2 = tform0Inverted.MultiplyPoint((corner1Even_2[0], corner1Even_2[1], corner1Even_2[2], 1))
-
-        corner0EvenTransformed = tform0.MultiplyPoint((corner0Even[0], corner0Even[1], corner1Even_2[2], 1))
-
+
+__docformat__ = "restructuredtext en"
+__all__ = ['CropWidget']
+
+from typing import Optional, Sequence
+
+import numpy as np
+from PyQt5.QtWidgets import QWidget, QHBoxLayout, QMainWindow, QVBoxLayout, QPushButton, QLabel, QFrame
+from vtkmodules import vtkCommonMath
+from vtkmodules.vtkInteractionWidgets import vtkBoxWidget2, vtkBoxRepresentation
+
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.processing.imageProcessing.resampler3D import crop3DDataAroundBox
+from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
+from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
+from opentps.gui.viewer.dataViewer import DroppedObject
+
+
+class CropWidget(QMainWindow):
+    def __init__(self, viewController, parent=None):
+        super().__init__(parent)
+
+        self._viewController = viewController
+
+        self.setWindowTitle('Crop tool')
+        self.resize(800, 600)
+
+        centralWidget = QWidget()
+        self.setCentralWidget(centralWidget)
+        self._mainLayout = QHBoxLayout()
+        centralWidget.setLayout(self._mainLayout)
+
+        self._viewers = ThreeViewsGrid(self._viewController)
+
+        self._dragLabel = QLabel("Select as many images as you want to crop.\nDrop the image needed to create a box.", self)
+        self._dragLabel.setWordWrap(True)
+
+        self._cropDataButton = QPushButton('Crop all selected data')
+        self._cropDataButton.clicked.connect(self._cropData)
+
+        self._dataSelection = PatientDataSelection(self._viewController, self)
+
+        self._menuFrame = QFrame(self)
+        self._menuFrame.setFixedWidth(200)
+        self._menuLayout = QVBoxLayout(self._menuFrame)
+        self._menuFrame.setLayout(self._menuLayout)
+
+        self._mainLayout.addWidget(self._menuFrame)
+        self._menuLayout.addWidget(self._dragLabel)
+        self._menuLayout.addWidget(self._dataSelection)
+        self._menuLayout.addWidget(self._cropDataButton)
+        self._mainLayout.addWidget(self._viewers)
+
+    def closeEvent(self, event):
+        self._viewers.close()
+        super().closeEvent(event)
+
+    def _cropData(self):
+        selectedData = self._dataSelection.selectedData
+
+        box = self._viewers.getBoundingBox()
+
+        xx = np.array([box[0], box[1]])
+        yy = np.array([box[2], box[3]])
+        zz = np.array([box[4], box[5]])
+
+        box = [[xx.min(), xx.max()], [yy.min(), yy.max()], [zz.min(), zz.max()]]
+
+        for data in selectedData:
+            crop3DDataAroundBox(data, box, marginInMM=[0, 0, 0])
+
+
+class ThreeViewsGrid(QWidget):
+    def __init__(self, viewController):
+        super().__init__()
+
+        self._viewController = viewController
+
+        self._mainLayout = QHBoxLayout(self)
+        self.setLayout(self._mainLayout)
+
+        self._viewer0 = Image3DViewer(viewController)
+        self._viewer1 = Image3DViewer(viewController)
+        self._viewer2 = Image3DViewer(viewController)
+
+        self._viewer0.viewType = Image3DViewer.ViewerTypes.CORONAL
+        self._viewer1.viewType = Image3DViewer.ViewerTypes.AXIAL
+        self._viewer2.viewType = Image3DViewer.ViewerTypes.SAGITTAL
+
+        self._viewer0.crossHairEnabled = True
+        self._viewer1.crossHairEnabled = True
+        self._viewer2.crossHairEnabled = True
+
+        self._mainLayout.addWidget(self._viewer0)
+        self._mainLayout.addWidget(self._viewer1)
+        self._mainLayout.addWidget(self._viewer2)
+
+        self.setAcceptDrops(True)
+        self.dragEnterEvent = lambda event: event.accept()
+        self.dropEvent = lambda event: self._dropEvent(event)
+
+    def close(self):
+        self._viewer0.close()
+        self._viewer1.close()
+        self._viewer2.close()
+
+    def _dropEvent(self, e):
+        if e.mimeData().hasText():
+            droppedIsImage = e.mimeData().text() == DroppedObject.DropTypes.IMAGE
+
+            if droppedIsImage:
+                e.accept()
+                self._setMainImage(self._viewController.selectedImage)
+                return
+        e.ignore()
+
+
+    def _setMainImage(self, image: Optional[Image3D]):
+        if isinstance(image, Image3D) or (image is None):
+            self._viewer0.primaryImage = image
+            self._viewer1.primaryImage = image
+            self._viewer2.primaryImage = image
+
+            interactor0 = self._viewer0._renderWindow.GetInteractor()
+            interactor1 = self._viewer1._renderWindow.GetInteractor()
+            interactor2 = self._viewer2._renderWindow.GetInteractor()
+
+            self.boxRep0 = vtkBoxRepresentation()
+            self.boxRep0.SetPlaceFactor(1)
+            self.boxRep0.PlaceWidget(self._viewer0._primaryImageLayer._mainActor.GetBounds())
+
+            self.boxRep1 = vtkBoxRepresentation()
+            self.boxRep1.SetPlaceFactor(1)
+            self.boxRep1.PlaceWidget(self._viewer1._primaryImageLayer._mainActor.GetBounds())
+
+            self.boxRep2 = vtkBoxRepresentation()
+            self.boxRep2.SetPlaceFactor(1)
+            self.boxRep2.PlaceWidget(self._viewer2._primaryImageLayer._mainActor.GetBounds())
+
+
+            self.boxWidget0 = vtkBoxWidget2()
+            self.boxWidget0.SetRotationEnabled(False)
+            self.boxWidget0.SetInteractor(interactor0)
+            self.boxWidget0.SetRepresentation(self.boxRep0)
+            self.boxWidget0.On()
+
+            self.boxWidget1 = vtkBoxWidget2()
+            self.boxWidget1.SetRotationEnabled(False)
+            self.boxWidget1.SetInteractor(interactor1)
+            self.boxWidget1.SetRepresentation(self.boxRep1)
+            self.boxWidget1.On()
+
+            self.boxWidget2 = vtkBoxWidget2()
+            self.boxWidget2.SetRotationEnabled(False)
+            self.boxWidget2.SetInteractor(interactor2)
+            self.boxWidget2.SetRepresentation(self.boxRep2)
+            self.boxWidget2.On()
+
+            self._viewer0._renderWindow.Render()
+            self._viewer1._renderWindow.Render()
+            self._viewer2._renderWindow.Render()
+
+            interactor0.Start()
+            interactor1.Start()
+            interactor2.Start()
+
+            self.boxWidget0.AddObserver('InteractionEvent', self.onInteraction0)
+            self.boxWidget1.AddObserver('InteractionEvent', self.onInteraction1)
+            self.boxWidget2.AddObserver('InteractionEvent', self.onInteraction2)
+
+    def onInteraction0(self, obj, event):
+        self.boxRep1.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer0, self.boxRep0, self._viewer1, self.boxRep1))
+        self.boxRep2.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer0, self.boxRep0, self._viewer2, self.boxRep2))
+        self._viewer1._renderWindow.Render()
+        self._viewer2._renderWindow.Render()
+
+    def onInteraction1(self, obj, event):
+        self.boxRep0.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer1, self.boxRep1, self._viewer0, self.boxRep0))
+        self.boxRep2.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer1, self.boxRep1, self._viewer2, self.boxRep2))
+        self._viewer0._renderWindow.Render()
+        self._viewer2._renderWindow.Render()
+
+    def onInteraction2(self, obj, event):
+        self.boxRep0.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer2, self.boxRep2, self._viewer0, self.boxRep0))
+        self.boxRep1.PlaceWidget(self._2DboundsFromViewerToViewer(self._viewer2, self.boxRep2, self._viewer1, self.boxRep1))
+        self._viewer0._renderWindow.Render()
+        self._viewer1._renderWindow.Render()
+
+    def _2DboundsFromViewerToViewer(self, viewer0:Image3DViewer, boxRep0, viewer1:Image3DViewer, boxRep1) -> Sequence[float]:
+        bounds = self._boundsFromViewerToViewer(viewer0, boxRep0, viewer1, boxRep1)
+        return [bounds[0], bounds[1], bounds[2], bounds[3], 0, 0]
+
+    def _boundsFromViewerToViewer(self, viewer0:Image3DViewer, boxRep0, viewer1:Image3DViewer, boxRep1) -> Sequence[float]:
+        bounds0 = boxRep0.GetBounds()
+        bounds1 = boxRep1.GetBounds()
+
+        corner0Odd = [bounds0[0], bounds0[2], bounds0[4]]
+        corner0Even = [bounds0[1], bounds0[3], bounds0[5]]
+
+        corner1Odd = [bounds1[0], bounds1[2], bounds1[4]]
+        corner1Even = [bounds1[1], bounds1[3], bounds1[5]]
+
+
+        tform0 = vtkCommonMath.vtkMatrix4x4()
+        tform0.DeepCopy(viewer0._viewMatrix)
+
+        tform0Inverted = vtkCommonMath.vtkMatrix4x4()
+        tform0Inverted.DeepCopy(viewer0._viewMatrix)
+        tform0Inverted.Invert()
+
+        tform1 = vtkCommonMath.vtkMatrix4x4()
+        tform1.DeepCopy(viewer1._viewMatrix)
+
+        tform1Inverted = vtkCommonMath.vtkMatrix4x4()
+        tform1Inverted.DeepCopy(viewer1._viewMatrix)
+        tform1Inverted.Invert()
+
+        corner1Odd_2 = tform1.MultiplyPoint((corner1Odd[0], corner1Odd[1], corner1Odd[2], 1))
+        corner1Odd_2 = tform0Inverted.MultiplyPoint((corner1Odd_2[0], corner1Odd_2[1], corner1Odd_2[2], 1))
+
+        corner0OddTransformed = tform0.MultiplyPoint((corner0Odd[0], corner0Odd[1], corner1Odd_2[2], 1))
+
+        corner0Odd_2 = tform1Inverted.MultiplyPoint((corner0OddTransformed[0], corner0OddTransformed[1], corner0OddTransformed[2], 1))
+
+        corner1Even_2 = tform1.MultiplyPoint((corner1Even[0], corner1Even[1], corner1Even[2], 1))
+        corner1Even_2 = tform0Inverted.MultiplyPoint((corner1Even_2[0], corner1Even_2[1], corner1Even_2[2], 1))
+
+        corner0EvenTransformed = tform0.MultiplyPoint((corner0Even[0], corner0Even[1], corner1Even_2[2], 1))
+
+        corner0Even_2 = tform1Inverted.MultiplyPoint((corner0EvenTransformed[0], corner0EvenTransformed[1], corner0EvenTransformed[2], 1))
+
+        return [corner0Odd_2[0], corner0Even_2[0], corner0Odd_2[1], corner0Even_2[1], corner0Odd_2[2], corner0Even_2[2]]
+
+
+    def getBoundingBox(self):
+        viewer0 = self._viewer0
+        viewer1 = self._viewer1
+
+        boxRep0 = self.boxRep0
+        boxRep1 = self.boxRep1
+
+        bounds0 = boxRep0.GetBounds()
+        bounds1 = boxRep1.GetBounds()
+
+        corner0Odd = [bounds0[0], bounds0[2], bounds0[4]]
+        corner0Even = [bounds0[1], bounds0[3], bounds0[5]]
+
+        corner1Odd = [bounds1[0], bounds1[2], bounds1[4]]
+        corner1Even = [bounds1[1], bounds1[3], bounds1[5]]
+
+        tform0 = vtkCommonMath.vtkMatrix4x4()
+        tform0.DeepCopy(viewer0._viewMatrix)
+
+        tform0Inverted = vtkCommonMath.vtkMatrix4x4()
+        tform0Inverted.DeepCopy(viewer0._viewMatrix)
+        tform0Inverted.Invert()
+
+        tform1 = vtkCommonMath.vtkMatrix4x4()
+        tform1.DeepCopy(viewer1._viewMatrix)
+
+        tform1Inverted = vtkCommonMath.vtkMatrix4x4()
+        tform1Inverted.DeepCopy(viewer1._viewMatrix)
+        tform1Inverted.Invert()
+
+        corner1Odd_2 = tform1.MultiplyPoint((corner1Odd[0], corner1Odd[1], corner1Odd[2], 1))
+        corner1Odd_2 = tform0Inverted.MultiplyPoint((corner1Odd_2[0], corner1Odd_2[1], corner1Odd_2[2], 1))
+
+        corner0OddTransformed = tform0.MultiplyPoint((corner0Odd[0], corner0Odd[1], corner1Odd_2[2], 1))
+
+
+        corner1Even_2 = tform1.MultiplyPoint((corner1Even[0], corner1Even[1], corner1Even[2], 1))
+        corner1Even_2 = tform0Inverted.MultiplyPoint((corner1Even_2[0], corner1Even_2[1], corner1Even_2[2], 1))
+
+        corner0EvenTransformed = tform0.MultiplyPoint((corner0Even[0], corner0Even[1], corner1Even_2[2], 1))
+
         return [corner0OddTransformed[0], corner0EvenTransformed[0], corner0OddTransformed[1], corner0EvenTransformed[1], corner0OddTransformed[2], corner0EvenTransformed[2]]
```

### Comparing `opentps-gui-1.0.4/opentps/gui/tools/_resampleTool.py` & `opentps_gui-1.0.5/opentps/gui/tools/_resampleTool.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-
-__docformat__ = "restructuredtext en"
-__all__ = ['ResampleWidget']
-
-from typing import Sequence
-
-import numpy as np
-from PyQt5.QtWidgets import QWidget, QHBoxLayout, QMainWindow, QVBoxLayout, QPushButton, QFrame, QLabel, QDoubleSpinBox
-
-from opentps.core.processing.imageProcessing import resampler3D
-from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
-
-
-class ResampleWidget(QMainWindow):
-    def __init__(self, viewController, parent=None):
-        super().__init__(parent)
-
-        self._viewController = viewController
-
-        self.setWindowTitle('Crop tool')
-
-        centralWidget = QWidget()
-        self.setCentralWidget(centralWidget)
-        self._mainLayout = QHBoxLayout()
-        centralWidget.setLayout(self._mainLayout)
-
-        self._resampleOptions = ResampleOptions(self._viewController)
-
-        self._cropDataButton = QPushButton('Resample all selected data')
-        self._cropDataButton.clicked.connect(self._resampleData)
-
-        self._dataSelection = PatientDataSelection((self._viewController))
-
-        self._menuFrame = QFrame(self)
-        self._menuFrame.setMaximumWidth(400)
-        self._menuLayout = QVBoxLayout(self._menuFrame)
-        self._menuFrame.setLayout(self._menuLayout)
-
-        self._mainLayout.addWidget(self._menuFrame)
-        self._menuLayout.addWidget(self._dataSelection)
-        self._menuLayout.addWidget(self._resampleOptions)
-        self._menuLayout.addWidget(self._cropDataButton)
-
-    def _resampleData(self):
-        newSpacing = np.array(self._resampleOptions.newSpacing)
-
-        for data in self._dataSelection.selectedData:
-            resampler3D.resampleImage3D(data, newSpacing, inPlace=True)
-
-
-class ResampleOptions(QWidget):
-    def __init__(self, viewController):
-        super().__init__()
-
-        self._viewController = viewController
-
-        self._mainLayout = QVBoxLayout()
-        self.setLayout(self._mainLayout)
-
-        self._layerLabel = QLabel('New spacing:')
-        self._mainLayout.addWidget(self._layerLabel)
-        self._spacing1Spin = QDoubleSpinBox()
-
-        self._spacingFrame = QFrame(self)
-        self._mainLayout.addWidget(self._spacingFrame)
-        self._spacingFrame.setFixedWidth(200)
-        self._spacingLayout = QHBoxLayout(self._spacingFrame)
-        self._spacingFrame.setLayout(self._spacingLayout)
-
-        self._spacing1Spin.setGroupSeparatorShown(True)
-        self._spacing1Spin.setRange(0.1, 100.0)
-        self._spacing1Spin.setSingleStep(1.0)
-        self._spacing1Spin.setValue(2.0)
-        self._spacing1Spin.setSuffix(" mm")
-        self._spacingLayout.addWidget(self._spacing1Spin)
-
-        self._spacing2Spin = QDoubleSpinBox()
-        self._spacing2Spin.setGroupSeparatorShown(True)
-        self._spacing2Spin.setRange(0.1, 100.0)
-        self._spacing2Spin.setSingleStep(1.0)
-        self._spacing2Spin.setValue(2.0)
-        self._spacing2Spin.setSuffix(" mm")
-        self._spacingLayout.addWidget(self._spacing2Spin)
-
-        self._spacing3Spin = QDoubleSpinBox()
-        self._spacing3Spin.setGroupSeparatorShown(True)
-        self._spacing3Spin.setRange(0.1, 100.0)
-        self._spacing3Spin.setSingleStep(1.0)
-        self._spacing3Spin.setValue(2.0)
-        self._spacing3Spin.setSuffix(" mm")
-        self._spacingLayout.addWidget(self._spacing3Spin)
-
-    @property
-    def newSpacing(self) -> Sequence[float]:
-        return (self._spacing1Spin.value(), self._spacing2Spin.value(), self._spacing3Spin.value())
+
+__docformat__ = "restructuredtext en"
+__all__ = ['ResampleWidget']
+
+from typing import Sequence
+
+import numpy as np
+from PyQt5.QtWidgets import QWidget, QHBoxLayout, QMainWindow, QVBoxLayout, QPushButton, QFrame, QLabel, QDoubleSpinBox
+
+from opentps.core.processing.imageProcessing import resampler3D
+from opentps.gui.panels.patientDataPanel.patientDataSelection import PatientDataSelection
+
+
+class ResampleWidget(QMainWindow):
+    def __init__(self, viewController, parent=None):
+        super().__init__(parent)
+
+        self._viewController = viewController
+
+        self.setWindowTitle('Crop tool')
+
+        centralWidget = QWidget()
+        self.setCentralWidget(centralWidget)
+        self._mainLayout = QHBoxLayout()
+        centralWidget.setLayout(self._mainLayout)
+
+        self._resampleOptions = ResampleOptions(self._viewController)
+
+        self._cropDataButton = QPushButton('Resample all selected data')
+        self._cropDataButton.clicked.connect(self._resampleData)
+
+        self._dataSelection = PatientDataSelection((self._viewController))
+
+        self._menuFrame = QFrame(self)
+        self._menuFrame.setMaximumWidth(400)
+        self._menuLayout = QVBoxLayout(self._menuFrame)
+        self._menuFrame.setLayout(self._menuLayout)
+
+        self._mainLayout.addWidget(self._menuFrame)
+        self._menuLayout.addWidget(self._dataSelection)
+        self._menuLayout.addWidget(self._resampleOptions)
+        self._menuLayout.addWidget(self._cropDataButton)
+
+    def _resampleData(self):
+        newSpacing = np.array(self._resampleOptions.newSpacing)
+
+        for data in self._dataSelection.selectedData:
+            resampler3D.resampleImage3D(data, newSpacing, inPlace=True)
+
+
+class ResampleOptions(QWidget):
+    def __init__(self, viewController):
+        super().__init__()
+
+        self._viewController = viewController
+
+        self._mainLayout = QVBoxLayout()
+        self.setLayout(self._mainLayout)
+
+        self._layerLabel = QLabel('New spacing:')
+        self._mainLayout.addWidget(self._layerLabel)
+        self._spacing1Spin = QDoubleSpinBox()
+
+        self._spacingFrame = QFrame(self)
+        self._mainLayout.addWidget(self._spacingFrame)
+        self._spacingFrame.setFixedWidth(200)
+        self._spacingLayout = QHBoxLayout(self._spacingFrame)
+        self._spacingFrame.setLayout(self._spacingLayout)
+
+        self._spacing1Spin.setGroupSeparatorShown(True)
+        self._spacing1Spin.setRange(0.1, 100.0)
+        self._spacing1Spin.setSingleStep(1.0)
+        self._spacing1Spin.setValue(2.0)
+        self._spacing1Spin.setSuffix(" mm")
+        self._spacingLayout.addWidget(self._spacing1Spin)
+
+        self._spacing2Spin = QDoubleSpinBox()
+        self._spacing2Spin.setGroupSeparatorShown(True)
+        self._spacing2Spin.setRange(0.1, 100.0)
+        self._spacing2Spin.setSingleStep(1.0)
+        self._spacing2Spin.setValue(2.0)
+        self._spacing2Spin.setSuffix(" mm")
+        self._spacingLayout.addWidget(self._spacing2Spin)
+
+        self._spacing3Spin = QDoubleSpinBox()
+        self._spacing3Spin.setGroupSeparatorShown(True)
+        self._spacing3Spin.setRange(0.1, 100.0)
+        self._spacing3Spin.setSingleStep(1.0)
+        self._spacing3Spin.setValue(2.0)
+        self._spacing3Spin.setSuffix(" mm")
+        self._spacingLayout.addWidget(self._spacing3Spin)
+
+    @property
+    def newSpacing(self) -> Sequence[float]:
+        return (self._spacing1Spin.value(), self._spacing2Spin.value(), self._spacing3Spin.value())
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/ROIContourForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/ROIMaskForViewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,68 @@
-import numpy as np
-from vtkmodules.vtkIOImage import vtkImageImport
-
-from opentps.core.data.images._image3D import Image3D
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.dataMultiton import DataMultiton
-
-
-class ROIContourForViewer(DataMultiton):
-    def __init__(self, roiContour):
-        super().__init__(roiContour)
-
-        if hasattr(self, '_visible'):
-            return
-
-        self.visibleChangedSignal = Event(bool)
-
-        self._dataImporter = vtkImageImport()
-        self._referenceImage = None
-        self._visible = False
-        self._vtkOutputPort = None
-
-        self._updateVtkOutputPort()
-
-    def __setattr__(self, key, value):
-        super().__setattr__(key, value)
-
-    @property
-    def referenceImage(self) -> Image3D:
-        return self._referenceImage
-
-    @referenceImage.setter
-    def referenceImage(self, image: Image3D):
-        self._referenceImage = image
-        self._updateVtkOutputPort()
-
-    @property
-    def visible(self) -> bool:
-        return self._visible
-
-    @visible.setter
-    def visible(self, visible: bool):
-        self._visible = visible
-        self.visibleChangedSignal.emit(self._visible)
-
-    def _updateVtkOutputPort(self):
-        if self._referenceImage is None:
-            return
-
-        referenceShape = self.referenceImage.gridSize
-        referenceOrigin = self.referenceImage.origin
-        referenceSpacing = self.referenceImage.spacing
-
-        mask = self.getBinaryMask(origin=referenceOrigin, gridSize=referenceShape,
-                                           spacing=referenceSpacing)
-        maskData = mask._imageArray
-        maskData = np.swapaxes(maskData, 0, 2)
-        num_array = np.array(np.ravel(maskData), dtype=np.float32)
-
-        self._dataImporter.SetNumberOfScalarComponents(1)
-        self._dataImporter.SetDataScalarTypeToFloat()
-
-        self._dataImporter.SetDataExtent(0, referenceShape[0] - 1, 0, referenceShape[1] - 1, 0, referenceShape[2] - 1)
-        self._dataImporter.SetWholeExtent(0, referenceShape[0] - 1, 0, referenceShape[1] - 1, 0, referenceShape[2] - 1)
-        self._dataImporter.SetDataSpacing(referenceSpacing[0], referenceSpacing[1], referenceSpacing[2])
-        self._dataImporter.SetDataOrigin(referenceOrigin[0], referenceOrigin[1], referenceOrigin[2])
-
-        data_string = num_array.tobytes()
-        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
-
-        self._vtkOutputPort = self._dataImporter.GetOutputPort()
-
-    @property
-    def vtkOutputPort(self):
-        return self._vtkOutputPort
+import numpy as np
+from vtkmodules.vtkIOImage import vtkImageImport
+
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents import lookupTables
+
+
+class ROIMaskForViewer(GenericImageForViewer):
+    def __init__(self, roiContour):
+        super().__init__(roiContour)
+
+        if hasattr(self, '_dataImporter'):
+            return
+
+        self.visibleChangedSignal = Event(bool)
+
+        self._dataImporter = vtkImageImport()
+        self._visible = False
+        self._vtkOutputPort = None
+
+        self.colorChangedSignal.connect(self._updateLT)
+
+        self._updateVtkOutputPort()
+
+    def __setattr__(self, key, value):
+        super().__setattr__(key, value)
+
+    @property
+    def visible(self) -> bool:
+        return self._visible
+
+    @visible.setter
+    def visible(self, visible: bool):
+        self._visible = visible
+        self.visibleChangedSignal.emit(self._visible)
+
+    def _updateLT(self, *args):
+        self._lookupTable = lookupTables.uniqueColorLT(1., 0.8, [self.color[0]/255, self.color[1]/255, self.color[2]/255])
+        self.lookupTableChangedSignal.emit(self._lookupTable)
+
+    def _updateVtkOutputPort(self):
+        if self._imageArray is None:
+            return
+        referenceShape = self.gridSize
+        referenceOrigin = self.origin
+        referenceSpacing = self.spacing
+
+        maskData = self._imageArray
+        maskData = np.swapaxes(maskData, 0, 2)
+        num_array = np.array(np.ravel(maskData), dtype=np.float32)
+
+        self._dataImporter.SetNumberOfScalarComponents(1)
+        self._dataImporter.SetDataScalarTypeToFloat()
+
+        self._dataImporter.SetDataExtent(0, referenceShape[0] - 1, 0, referenceShape[1] - 1, 0, referenceShape[2] - 1)
+        self._dataImporter.SetWholeExtent(0, referenceShape[0] - 1, 0, referenceShape[1] - 1, 0, referenceShape[2] - 1)
+        self._dataImporter.SetDataSpacing(referenceSpacing[0], referenceSpacing[1], referenceSpacing[2])
+        self._dataImporter.SetDataOrigin(referenceOrigin[0], referenceOrigin[1], referenceOrigin[2])
+
+        data_string = num_array.tobytes()
+        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
+
+        self._vtkOutputPort = self._dataImporter.GetOutputPort()
+
+    @property
+    def vtkOutputPort(self):
+        return self._vtkOutputPort
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dataMultiton.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dataMultiton.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-
-class DataMultiton(object):
-    _allViewerDatas = []
-
-    def __new__(cls, data):
-        if data is None:
-            return None
-
-        # if there is already a DataMultiton for this data instance
-        for dataMultiton in DataMultiton._allViewerDatas:
-            if dataMultiton.data == data:
-                dataMultiton.subClass(cls)
-                return dataMultiton
-
-        # else
-        dataMultiton = super().__new__(cls)
-        DataMultiton._allViewerDatas.append(dataMultiton)
-        return dataMultiton
-
-    def subClass(self, cls):
-        self.__class__ = cls  # Subclass the existing DataMultiton
-
-    def __init__(self, data):
-        if data is None:
-            return
-
-        if hasattr(self, 'data'):
-            return
-
-        super().__init__()
-        self.data = data
-
-    def __getattribute__(self, item):
-        try:
-            return object.__getattribute__(self, item)
-        except:
-            # we cannot return data from data
-            if item=='data':
-                raise AttributeError("data not initialized in DataMultiton")
-            return self.data.__getattribute__(item)
+
+class DataMultiton(object):
+    _allViewerDatas = []
+
+    def __new__(cls, data):
+        if data is None:
+            return None
+
+        # if there is already a DataMultiton for this data instance
+        for dataMultiton in DataMultiton._allViewerDatas:
+            if dataMultiton.data == data:
+                dataMultiton.subClass(cls)
+                return dataMultiton
+
+        # else
+        dataMultiton = super().__new__(cls)
+        DataMultiton._allViewerDatas.append(dataMultiton)
+        return dataMultiton
+
+    def subClass(self, cls):
+        self.__class__ = cls  # Subclass the existing DataMultiton
+
+    def __init__(self, data):
+        if data is None:
+            return
+
+        if hasattr(self, 'data'):
+            return
+
+        super().__init__()
+        self.data = data
+
+    def __getattribute__(self, item):
+        try:
+            return object.__getattribute__(self, item)
+        except:
+            # we cannot return data from data
+            if item=='data':
+                raise AttributeError("data not initialized in DataMultiton")
+            return self.data.__getattribute__(item)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dyn2DSeqForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dyn2DSeqForViewer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import numpy as np
-from vtkmodules.vtkImagingGeneral import vtkSimpleImageFilterExample
-
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image2DForViewer import Image2DForViewer
-
-
-class Dyn2DSeqForViewer(GenericImageForViewer):
-    def __init__(self, dyn2DSeq):
-        super().__init__(dyn2DSeq)
-
-        if hasattr(self, '_image3DForViewerList'):
-            return
-
-        dyn2DSeq = self.data
-        self._selectedPosition = np.array(dyn2DSeq.dyn2DImageList[0].origin) + np.array(dyn2DSeq.dyn2DImageList[0].gridSize) * np.array(dyn2DSeq.dyn2DImageList[0].spacing) / 2.0
-
-        # This creates all image3DForViewers within the image sequence with the side effect that all VTK output port are initialized.
-        self._image2DForViewerList = self._getImg2DForViewerList(dyn2DSeq.dyn2DImageList)
-
-        self._simpleFilter = vtkSimpleImageFilterExample()
-        self._currentIndexIn2DSeq = 0
-        self._updateVTKOutputPort()
-        self._vtkOutputPort = self._simpleFilter.GetOutputPort()
-        self._range = (np.min(self.data.dyn2DImageList[0].imageArray), np.max(self.data.dyn2DImageList[0].imageArray))
-
-    def _getImg2DForViewerList(self, dyn2DSeqImgList):
-        vtkImageList = []
-        for image in dyn2DSeqImgList:
-            vtkImageList.append(Image2DForViewer(image))
-
-        return vtkImageList
-
-    @property
-    def currentIndexIn2DSeq(self):
-        return self._currentIndexIn2DSeq
-
-    @currentIndexIn2DSeq.setter
-    def currentIndexIn2DSeq(self, ind):
-        if self._currentIndexIn2DSeq == ind:
-            return
-
-        self._currentIndexIn2DSeq = ind
-        self._updateVTKOutputPort()
-
-    def _updateVTKOutputPort(self):
-        self._simpleFilter.RemoveAllInputs()
-        currImageForViewer = self._image2DForViewerList[self._currentIndexIn2DSeq]
-        self._simpleFilter.SetInputConnection(currImageForViewer.vtkOutputPort)
-
-    @property
-    def vtkOutputPort(self):
-        return self._vtkOutputPort
-
+import numpy as np
+from vtkmodules.vtkImagingGeneral import vtkSimpleImageFilterExample
+
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image2DForViewer import Image2DForViewer
+
+
+class Dyn2DSeqForViewer(GenericImageForViewer):
+    def __init__(self, dyn2DSeq):
+        super().__init__(dyn2DSeq)
+
+        if hasattr(self, '_image3DForViewerList'):
+            return
+
+        dyn2DSeq = self.data
+        self._selectedPosition = np.array(dyn2DSeq.dyn2DImageList[0].origin) + np.array(dyn2DSeq.dyn2DImageList[0].gridSize) * np.array(dyn2DSeq.dyn2DImageList[0].spacing) / 2.0
+
+        # This creates all image3DForViewers within the image sequence with the side effect that all VTK output port are initialized.
+        self._image2DForViewerList = self._getImg2DForViewerList(dyn2DSeq.dyn2DImageList)
+
+        self._simpleFilter = vtkSimpleImageFilterExample()
+        self._currentIndexIn2DSeq = 0
+        self._updateVTKOutputPort()
+        self._vtkOutputPort = self._simpleFilter.GetOutputPort()
+        self._range = (np.min(self.data.dyn2DImageList[0].imageArray), np.max(self.data.dyn2DImageList[0].imageArray))
+
+    def _getImg2DForViewerList(self, dyn2DSeqImgList):
+        vtkImageList = []
+        for image in dyn2DSeqImgList:
+            vtkImageList.append(Image2DForViewer(image))
+
+        return vtkImageList
+
+    @property
+    def currentIndexIn2DSeq(self):
+        return self._currentIndexIn2DSeq
+
+    @currentIndexIn2DSeq.setter
+    def currentIndexIn2DSeq(self, ind):
+        if self._currentIndexIn2DSeq == ind:
+            return
+
+        self._currentIndexIn2DSeq = ind
+        self._updateVTKOutputPort()
+
+    def _updateVTKOutputPort(self):
+        self._simpleFilter.RemoveAllInputs()
+        currImageForViewer = self._image2DForViewerList[self._currentIndexIn2DSeq]
+        self._simpleFilter.SetInputConnection(currImageForViewer.vtkOutputPort)
+
+    @property
+    def vtkOutputPort(self):
+        return self._vtkOutputPort
+
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/dyn3DSeqForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/dyn3DSeqForViewer.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import numpy as np
-from vtkmodules.vtkImagingGeneral import vtkSimpleImageFilterExample
-
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-
-
-class Dyn3DSeqForViewer(GenericImageForViewer):
-    def __init__(self, dyn3DSeq):
-        super().__init__(dyn3DSeq)
-
-        if hasattr(self, '_image3DForViewerList'):
-            return
-
-        self.dataChangedSignal = Event() # Not implemented in data class but required by opentps_core
-
-        dyn3DSeq = self.data
-        self._selectedPosition = np.array(dyn3DSeq.dyn3DImageList[0].origin) + np.array(dyn3DSeq.dyn3DImageList[0].gridSize) * np.array(dyn3DSeq.dyn3DImageList[0].spacing) / 2.0
-
-        # This creates all image3DForViewers within the image sequence with the side effect that all VTK output port are initialized.
-        self._image3DForViewerList = self._getImg3DForViewerList(dyn3DSeq.dyn3DImageList)
-
-        self._simpleFilter = vtkSimpleImageFilterExample()
-        self._currentIndexIn3DSeq = 0
-        self._updateVTKOutputPort()
-        self._vtkOutputPort = self._simpleFilter.GetOutputPort()
-        self._range = (np.min(self.data.dyn3DImageList[0].imageArray), np.max(self.data.dyn3DImageList[0].imageArray))
-
-    def _getImg3DForViewerList(self, dyn3DSeqImgList):
-        vtkImageList = []
-        for image in dyn3DSeqImgList:
-            vtkImageList.append(Image3DForViewer(image))
-
-        return vtkImageList
-
-    @property
-    def currentIndexIn3DSeq(self):
-        return self._currentIndexIn3DSeq
-
-    @currentIndexIn3DSeq.setter
-    def currentIndexIn3DSeq(self, ind):
-        if self._currentIndexIn3DSeq == ind:
-            return
-
-        self._currentIndexIn3DSeq = ind
-        self._updateVTKOutputPort()
-
-    def _updateVTKOutputPort(self):
-        self._simpleFilter.RemoveAllInputs()
-        currImageForViewer = self._image3DForViewerList[self._currentIndexIn3DSeq]
-        self._simpleFilter.SetInputConnection(currImageForViewer.vtkOutputPort)
-
-    @property
-    def vtkOutputPort(self):
-        return self._vtkOutputPort
-
+import numpy as np
+from vtkmodules.vtkImagingGeneral import vtkSimpleImageFilterExample
+
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+
+
+class Dyn3DSeqForViewer(GenericImageForViewer):
+    def __init__(self, dyn3DSeq):
+        super().__init__(dyn3DSeq)
+
+        if hasattr(self, '_image3DForViewerList'):
+            return
+
+        self.dataChangedSignal = Event() # Not implemented in data class but required by opentps_core
+
+        dyn3DSeq = self.data
+        self._selectedPosition = np.array(dyn3DSeq.dyn3DImageList[0].origin) + np.array(dyn3DSeq.dyn3DImageList[0].gridSize) * np.array(dyn3DSeq.dyn3DImageList[0].spacing) / 2.0
+
+        # This creates all image3DForViewers within the image sequence with the side effect that all VTK output port are initialized.
+        self._image3DForViewerList = self._getImg3DForViewerList(dyn3DSeq.dyn3DImageList)
+
+        self._simpleFilter = vtkSimpleImageFilterExample()
+        self._currentIndexIn3DSeq = 0
+        self._updateVTKOutputPort()
+        self._vtkOutputPort = self._simpleFilter.GetOutputPort()
+        self._range = (np.min(self.data.dyn3DImageList[0].imageArray), np.max(self.data.dyn3DImageList[0].imageArray))
+
+    def _getImg3DForViewerList(self, dyn3DSeqImgList):
+        vtkImageList = []
+        for image in dyn3DSeqImgList:
+            vtkImageList.append(Image3DForViewer(image))
+
+        return vtkImageList
+
+    @property
+    def currentIndexIn3DSeq(self):
+        return self._currentIndexIn3DSeq
+
+    @currentIndexIn3DSeq.setter
+    def currentIndexIn3DSeq(self, ind):
+        if self._currentIndexIn3DSeq == ind:
+            return
+
+        self._currentIndexIn3DSeq = ind
+        self._updateVTKOutputPort()
+
+    def _updateVTKOutputPort(self):
+        self._simpleFilter.RemoveAllInputs()
+        currImageForViewer = self._image3DForViewerList[self._currentIndexIn3DSeq]
+        self._simpleFilter.SetInputConnection(currImageForViewer.vtkOutputPort)
+
+    @property
+    def vtkOutputPort(self):
+        return self._vtkOutputPort
+
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/genericImageForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/genericImageForViewer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-
-import typing
-from math import isclose
-
-from opentps.core import Event
-
-from opentps.gui.viewer.dataForViewer.dataMultiton import DataMultiton
-import opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables as lookupTables
-
-
-class GenericImageForViewer(DataMultiton):
-    def __init__(self, image):
-        super().__init__(image)
-
-        if hasattr(self, '_wwlValue'):
-            return
-
-        self.wwlChangedSignal = Event(tuple)
-        self.lookupTableChangedSignal = Event(object)
-        self.selectedPositionChangedSignal = Event(tuple)
-        self.rangeChangedSignal = Event(tuple)
-
-        self._range = (-500, 500)
-        self._wwlValue = (self._range[1]-self._range[0], (self._range[1]+self._range[0])/2.)
-        self._lookupTableName = 'gray'
-        self._opacity = 0.5
-        self._selectedPosition = (0, 0, 0)
-        self._vtkOutputPort = None
-
-        self._updateLT()
-
-    @property
-    def selectedPosition(self) -> tuple:
-        return self._selectedPosition
-
-    @selectedPosition.setter
-    def selectedPosition(self, position: typing.Sequence):
-        self._selectedPosition = (position[0], position[1], position[2])
-        self.selectedPositionChangedSignal.emit(self._selectedPosition)
-
-    @property
-    def wwlValue(self) -> tuple:
-        return self._wwlValue
-
-    @wwlValue.setter
-    def wwlValue(self, wwl: typing.Sequence):
-        if isclose(wwl[0], self._wwlValue[0], abs_tol=0.1) and isclose(wwl[1], self._wwlValue[1], abs_tol=0.1):
-            return
-
-        self._wwlValue = (wwl[0], wwl[1])
-        self.range = (wwl[1]-wwl[0]/2., wwl[1]+wwl[0]/2.)
-        self.wwlChangedSignal.emit(self._wwlValue)
-
-    @property
-    def lookupTable(self) :
-        return self._lookupTable
-
-    @property
-    def lookupTableName(self) -> str:
-        return self._lookupTableName
-
-    @lookupTableName.setter
-    def lookupTableName(self, lookupTableName:str):
-        if self._lookupTableName == lookupTableName:
-            return
-
-        self._lookupTableName = lookupTableName
-        self._updateLT()
-
-    def _updateLT(self):
-        if self._lookupTableName == 'gray':
-            self._lookupTable = lookupTables.grayLT(self._range)
-        else:
-            self._lookupTable = lookupTables.fusionLT(self._range, self._opacity, self._lookupTableName)
-        self.lookupTableChangedSignal.emit(self._lookupTable)
-
-    @property
-    def range(self) -> tuple:
-        return self._range
-
-    @range.setter
-    def range(self, range: typing.Sequence):
-        if isclose(range[0], self._range[0], abs_tol=0.1) and isclose(range[1], self._range[1], abs_tol=0.1):
-            return
-
-        self._range = (range[0], range[1])
-        self.wwlValue = (range[1]-range[0], (range[1]+range[0])/2.)
-
-        if not (self._lookupTable is None) and self._lookupTableName=='gray':
-            self._lookupTable.SetRange(self._range[0], self._range[1])
-        else:
-            self._updateLT()
-
-        self.rangeChangedSignal.emit(self._range)
-
-    @property
-    def opacity(self) -> float:
-        return self._opacity
-
-    @opacity.setter
-    def opacity(self, opacity: float):
-        self._opacity = opacity
-        self._updateLT()
-
-    @property
-    def vtkOutputPort(self):
-        raise NotImplementedError()
+
+import typing
+from math import isclose
+
+from opentps.core import Event
+
+from opentps.gui.viewer.dataForViewer.dataMultiton import DataMultiton
+import opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables as lookupTables
+
+
+class GenericImageForViewer(DataMultiton):
+    def __init__(self, image):
+        super().__init__(image)
+
+        if hasattr(self, '_wwlValue'):
+            return
+
+        self.wwlChangedSignal = Event(tuple)
+        self.lookupTableChangedSignal = Event(object)
+        self.selectedPositionChangedSignal = Event(tuple)
+        self.rangeChangedSignal = Event(tuple)
+
+        self._range = (-500, 500)
+        self._wwlValue = (self._range[1]-self._range[0], (self._range[1]+self._range[0])/2.)
+        self._lookupTableName = 'gray'
+        self._opacity = 0.5
+        self._selectedPosition = (0, 0, 0)
+        self._vtkOutputPort = None
+
+        self._updateLT()
+
+    @property
+    def selectedPosition(self) -> tuple:
+        return self._selectedPosition
+
+    @selectedPosition.setter
+    def selectedPosition(self, position: typing.Sequence):
+        self._selectedPosition = (position[0], position[1], position[2])
+        self.selectedPositionChangedSignal.emit(self._selectedPosition)
+
+    @property
+    def wwlValue(self) -> tuple:
+        return self._wwlValue
+
+    @wwlValue.setter
+    def wwlValue(self, wwl: typing.Sequence):
+        if isclose(wwl[0], self._wwlValue[0], abs_tol=0.1) and isclose(wwl[1], self._wwlValue[1], abs_tol=0.1):
+            return
+
+        self._wwlValue = (wwl[0], wwl[1])
+        self.range = (wwl[1]-wwl[0]/2., wwl[1]+wwl[0]/2.)
+        self.wwlChangedSignal.emit(self._wwlValue)
+
+    @property
+    def lookupTable(self) :
+        return self._lookupTable
+
+    @property
+    def lookupTableName(self) -> str:
+        return self._lookupTableName
+
+    @lookupTableName.setter
+    def lookupTableName(self, lookupTableName:str):
+        if self._lookupTableName == lookupTableName:
+            return
+
+        self._lookupTableName = lookupTableName
+        self._updateLT()
+
+    def _updateLT(self):
+        if self._lookupTableName == 'gray':
+            self._lookupTable = lookupTables.grayLT(self._range)
+        else:
+            self._lookupTable = lookupTables.fusionLT(self._range, self._opacity, self._lookupTableName)
+        self.lookupTableChangedSignal.emit(self._lookupTable)
+
+    @property
+    def range(self) -> tuple:
+        return self._range
+
+    @range.setter
+    def range(self, range: typing.Sequence):
+        if isclose(range[0], self._range[0], abs_tol=0.1) and isclose(range[1], self._range[1], abs_tol=0.1):
+            return
+
+        self._range = (range[0], range[1])
+        self.wwlValue = (range[1]-range[0], (range[1]+range[0])/2.)
+
+        if not (self._lookupTable is None) and self._lookupTableName=='gray':
+            self._lookupTable.SetRange(self._range[0], self._range[1])
+        else:
+            self._updateLT()
+
+        self.rangeChangedSignal.emit(self._range)
+
+    @property
+    def opacity(self) -> float:
+        return self._opacity
+
+    @opacity.setter
+    def opacity(self, opacity: float):
+        self._opacity = opacity
+        self._updateLT()
+
+    @property
+    def vtkOutputPort(self):
+        raise NotImplementedError()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/image2DForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/image2DForViewer.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-
-import numpy as np
-from vtkmodules.vtkIOImage import vtkImageImport
-
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-
-
-class Image2DForViewer(GenericImageForViewer):
-
-    def __init__(self, image):
-        super().__init__(image)
-
-        if hasattr(self, '_dataImporter'):
-            return
-
-        # print('in image2DForViewer init', type(image))
-        # print('in image2DForViewer init', type(self.data))
-
-
-        self._dataImporter = vtkImageImport()
-        self._selectedPosition = self.data.origin# + self.data.gridSizeInWorldUnit/2.
-        self._range = (np.min(self.data.imageArray), np.max(self.data.imageArray))
-
-        self.data.dataChangedSignal.connect(self._updateVTKOutputPort)
-        self._updateVTKOutputPort()
-
-    def _updateVTKOutputPort(self):
-        print('in image2DForViewer _updateVTKOutputPort')
-        print(self.gridSize)
-        print(self.spacing)
-        print(self.origin)
-
-        shape = self.gridSize  ## dataMultiton magic makes all this available here
-        imageOrigin = self.origin
-        imageSpacing = self.spacing
-        # imageData = np.swapaxes(self.imageArray, 0, 2)
-        imageData = self.imageArray
-        # imageData[100:140, 200:500] = 300
-        imageData -= np.min(imageData)
-
-        # imageData = np.tile(imageData, (3, 1, 1))
-        # print(imageData.shape)
-        # shape = imageData.shape
-        # plt.figure()
-        # plt.imshow(imageData)
-        # plt.show()
-        # shape = imageData.shape
-        # print(shape)
-
-        num_array = np.array(np.ravel(imageData), dtype=np.float32)
-
-        self._dataImporter.SetNumberOfScalarComponents(1)
-        self._dataImporter.SetDataExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, 0)
-        self._dataImporter.SetWholeExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, 0)
-        self._dataImporter.SetDataSpacing(imageSpacing[0], imageSpacing[1], 1)
-        self._dataImporter.SetDataOrigin(imageOrigin[0], imageOrigin[1], imageOrigin[2])
-        self._dataImporter.SetDataScalarTypeToFloat()
-
-        data_string = num_array.tobytes()
-        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
-
-        self._vtkOutputPort = self._dataImporter.GetOutputPort()
-
-        import vtk
-
-        mapper = vtk.vtkImageMapper()
-        print(type(self._vtkOutputPort))
-        mapper.SetInputConnection(self._vtkOutputPort)
-        # mapper.SetInputData(self._vtkOutputPort)
-        actor = vtk.vtkActor2D()
-        actor.SetMapper(mapper)
-
-        ren = vtk.vtkRenderer()
-        ren.AddActor(actor)
-        ren.SetBackground(0.1, 0.2, 0.4)
-
-        renWin = vtk.vtkRenderWindow()
-        renWin.AddRenderer(ren)
-        renWin.SetSize(400, 400)
-
-        iren = vtk.vtkRenderWindowInteractor()
-        iren.SetRenderWindow(renWin)
-
-        renWin.Render()
-        iren.Start()
-
-    @property
-    def vtkOutputPort(self):
-        return self._vtkOutputPort
+
+import numpy as np
+from vtkmodules.vtkIOImage import vtkImageImport
+
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+
+
+class Image2DForViewer(GenericImageForViewer):
+
+    def __init__(self, image):
+        super().__init__(image)
+
+        if hasattr(self, '_dataImporter'):
+            return
+
+        # print('in image2DForViewer init', type(image))
+        # print('in image2DForViewer init', type(self.data))
+
+
+        self._dataImporter = vtkImageImport()
+        self._selectedPosition = self.data.origin# + self.data.gridSizeInWorldUnit/2.
+        self._range = (np.min(self.data.imageArray), np.max(self.data.imageArray))
+
+        self.data.dataChangedSignal.connect(self._updateVTKOutputPort)
+        self._updateVTKOutputPort()
+
+    def _updateVTKOutputPort(self):
+        print('in image2DForViewer _updateVTKOutputPort')
+        print(self.gridSize)
+        print(self.spacing)
+        print(self.origin)
+
+        shape = self.gridSize  ## dataMultiton magic makes all this available here
+        imageOrigin = self.origin
+        imageSpacing = self.spacing
+        # imageData = np.swapaxes(self.imageArray, 0, 2)
+        imageData = self.imageArray
+        # imageData[100:140, 200:500] = 300
+        imageData -= np.min(imageData)
+
+        # imageData = np.tile(imageData, (3, 1, 1))
+        # print(imageData.shape)
+        # shape = imageData.shape
+        # plt.figure()
+        # plt.imshow(imageData)
+        # plt.show()
+        # shape = imageData.shape
+        # print(shape)
+
+        num_array = np.array(np.ravel(imageData), dtype=np.float32)
+
+        self._dataImporter.SetNumberOfScalarComponents(1)
+        self._dataImporter.SetDataExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, 0)
+        self._dataImporter.SetWholeExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, 0)
+        self._dataImporter.SetDataSpacing(imageSpacing[0], imageSpacing[1], 1)
+        self._dataImporter.SetDataOrigin(imageOrigin[0], imageOrigin[1], imageOrigin[2])
+        self._dataImporter.SetDataScalarTypeToFloat()
+
+        data_string = num_array.tobytes()
+        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
+
+        self._vtkOutputPort = self._dataImporter.GetOutputPort()
+
+        import vtk
+
+        mapper = vtk.vtkImageMapper()
+        print(type(self._vtkOutputPort))
+        mapper.SetInputConnection(self._vtkOutputPort)
+        # mapper.SetInputData(self._vtkOutputPort)
+        actor = vtk.vtkActor2D()
+        actor.SetMapper(mapper)
+
+        ren = vtk.vtkRenderer()
+        ren.AddActor(actor)
+        ren.SetBackground(0.1, 0.2, 0.4)
+
+        renWin = vtk.vtkRenderWindow()
+        renWin.AddRenderer(ren)
+        renWin.SetSize(400, 400)
+
+        iren = vtk.vtkRenderWindowInteractor()
+        iren.SetRenderWindow(renWin)
+
+        renWin.Render()
+        iren.Start()
+
+    @property
+    def vtkOutputPort(self):
+        return self._vtkOutputPort
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataForViewer/image3DForViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataForViewer/image3DForViewer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
-import numpy as np
-from vtkmodules.vtkIOImage import vtkImageImport
-
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-
-
-class Image3DForViewer(GenericImageForViewer):
-
-    def __init__(self, image):
-        super().__init__(image)
-
-        if hasattr(self, '_dataImporter'):
-            return
-
-        self._dataImporter = vtkImageImport()
-        self._selectedPosition = self.data.origin + self.data.gridSizeInWorldUnit/2.
-        self._range = (np.min(self.data.imageArray), np.max(self.data.imageArray))
-
-        self.data.dataChangedSignal.connect(self._updateVTKOutputPort)
-        self._updateVTKOutputPort()
-
-    def _updateVTKOutputPort(self):
-        shape = self.gridSize  ## dataMultiton magic makes all this available here
-        imageOrigin = self.origin
-        imageSpacing = self.spacing
-        imageData = np.swapaxes(self.imageArray, 0, 2)
-        num_array = np.array(np.ravel(imageData), dtype=np.float32)
-
-        self._dataImporter.SetNumberOfScalarComponents(1)
-        self._dataImporter.SetDataExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, shape[2] - 1)
-        self._dataImporter.SetWholeExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, shape[2] - 1)
-        self._dataImporter.SetDataSpacing(imageSpacing[0], imageSpacing[1], imageSpacing[2])
-        self._dataImporter.SetDataOrigin(imageOrigin[0], imageOrigin[1], imageOrigin[2])
-        self._dataImporter.SetDataScalarTypeToFloat()
-
-        data_string = num_array.tobytes()
-        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
-
-        self._vtkOutputPort = self._dataImporter.GetOutputPort()
-
-    @property
-    def vtkOutputPort(self):
-        return self._vtkOutputPort
+
+import numpy as np
+from vtkmodules.vtkIOImage import vtkImageImport
+
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+
+
+class Image3DForViewer(GenericImageForViewer):
+
+    def __init__(self, image):
+        super().__init__(image)
+
+        if hasattr(self, '_dataImporter'):
+            return
+
+        self._dataImporter = vtkImageImport()
+        self._selectedPosition = self.data.origin + self.data.gridSizeInWorldUnit/2.
+        self._range = (np.min(self.data.imageArray), np.max(self.data.imageArray))
+
+        self.data.dataChangedSignal.connect(self._updateVTKOutputPort)
+        self._updateVTKOutputPort()
+
+    def _updateVTKOutputPort(self):
+        shape = self.gridSize  ## dataMultiton magic makes all this available here
+        imageOrigin = self.origin
+        imageSpacing = self.spacing
+        imageData = np.swapaxes(self.imageArray, 0, 2)
+        num_array = np.array(np.ravel(imageData), dtype=np.float32)
+
+        self._dataImporter.SetNumberOfScalarComponents(1)
+        self._dataImporter.SetDataExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, shape[2] - 1)
+        self._dataImporter.SetWholeExtent(0, shape[0] - 1, 0, shape[1] - 1, 0, shape[2] - 1)
+        self._dataImporter.SetDataSpacing(imageSpacing[0], imageSpacing[1], imageSpacing[2])
+        self._dataImporter.SetDataOrigin(imageOrigin[0], imageOrigin[1], imageOrigin[2])
+        self._dataImporter.SetDataScalarTypeToFloat()
+
+        data_string = num_array.tobytes()
+        self._dataImporter.CopyImportVoidPointer(data_string, len(data_string))
+
+        self._vtkOutputPort = self._dataImporter.GetOutputPort()
+
+    @property
+    def vtkOutputPort(self):
+        return self._vtkOutputPort
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,655 +1,644 @@
-from enum import Enum
-from typing import Union, Optional
-
-from PyQt5.QtWidgets import QWidget, QVBoxLayout
-
-from opentps.core.data.images import DoseImage
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.images import Image2D
-from opentps.core.data.dynamicData.dynamic3DSequence import Dynamic3DSequence
-from opentps.core.data.dynamicData.dynamic3DModel import Dynamic3DModel
-from opentps.core.data.dynamicData.dynamic2DSequence import Dynamic2DSequence
-from opentps.core.data.plan._rtPlan import RTPlan
-from opentps.core import Event
-from opentps.gui.viewer.dataViewerComponents.dvhViewerActions import DVHViewerActions
-from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
-from opentps.gui.viewer.dataViewerComponents.dynamicImage3DViewer import DynamicImage3DViewer
-from opentps.gui.viewer.dataViewerComponents.image2DViewer import Image2DViewer
-from opentps.gui.viewer.dataViewerComponents.dynamicImage2DViewer import DynamicImage2DViewer
-from opentps.gui.viewer.dataViewerComponents.image3DViewer_3D import Image3DViewer_3D
-from opentps.gui.viewer.dataViewerComponents.imageViewerActions import ImageViewerActions
-from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
-from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
-from opentps.gui.viewer.dataViewerComponents.dvhPlot import DVHViewer
-from opentps.gui.viewer.dataViewerComponents.profileViewer import ProfileViewer
-
-
-class DroppedObject:
-    """
-    This class aims to standardized object dropping
-    TODO: we might want to move this to another file
-    """
-    class DropTypes:
-        # DropTypes is not an Enum because Enum does not preserve string type of class attributes. But we want Drop types
-        # to be string to be compatible with QMimeData
-        IMAGE = 'IMAGE'
-        PLAN = 'PLAN'
-
-    def __init__(self, dropType, droppedData):
-        self.dropType = dropType
-        self.droppedData = droppedData
-
-
-class DataViewer(QWidget):
-    """
-    This class displays the type of viewer specified as input and a toolbar to switch between them.
-    All viewers are cached for responsiveness.
-    Example::
-     dataViewer = DataViewer(viewController)
-     dataViewer.viewerMode = dataViewer.ViewerModes.STATIC # Static mode (for data which are not time series)
-     dataViewer.displayType = dataViewer.ViewerTypes.VIEWER_IMAGE # Show an image viewer
-     dataViewe.displayMode = dataViewer.ViewerTypes.VIEWER_DVH # Switch to a DVH viewer
-    Currently the DataViewer has its own logic based on events in viewController. Should we have a controller to specifically handle the logical part?
-    """
-    class DisplayTypes(Enum):
-        """
-            viewer types
-        """
-        NONE = None
-        DISPLAY_DVH = 'DISPLAY_DVH'
-        DISPLAY_PROFILE = 'DISPLAY_PROFILE'
-        DISPLAY_IMAGE3D = 'DISPLAY_IMAGE3D'
-        DISPLAY_IMAGE2D = 'DISPLAY_IMAGE2D'
-        DISPLAY_IMAGE3D_3D = 'DISPLAY_IMAGE3D_3D'
-
-        DEFAULT = DISPLAY_IMAGE3D
-
-    class DisplayModes(Enum):
-        """
-            viewer modes
-        """
-        STATIC = 'STATIC'
-        DYNAMIC = 'DYNAMIC'
-
-        DEFAULT = STATIC
-
-    class DropModes(Enum):
-        AUTO = 'auto'
-        PRIMARY = 'primary'
-        SECONDARY = 'secondary'
-
-        DEFAULT = AUTO
-
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-
-        # It might seems weird to have a signal which is only used within the class but it is if someday we want to move the logical part out of this class.
-        self.droppedImageSignal = Event(object)
-        self.droppedPlanSignal = Event(object)
-        self.displayTypeChangedSignal = Event(object)
-
-        self._viewController = viewController
-
-        self._currentViewer = None
-        self._displayMode = self.DisplayModes.DEFAULT
-        self._displayType = None
-
-        self._dropMode = self._viewController.dropMode
-        self._dropEnabled = False
-
-        self._mainLayout = QVBoxLayout(self)
-        self.setLayout(self._mainLayout)
-        self._mainLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._toolbar = DataViewerToolbar(self)
-
-        # For responsiveness, we instantiate all possible viewers and hide them == cached viewers:
-        self._dvhViewer = DVHViewer(self)
-        self._noneViewer = BlackEmptyPlot(self)
-        self._staticProfileviewer = ProfileViewer(viewController)
-        self._staticImage3DViewer = Image3DViewer(viewController)
-        self._staticImage2DViewer = Image2DViewer(viewController)
-        self._staticImage3DViewer_3D = Image3DViewer_3D(viewController)
-
-        ## dynamic stuff
-        self._dynImage3DViewer = DynamicImage3DViewer(viewController)
-        self._dynImage2DViewer = DynamicImage2DViewer(viewController)
-
-        ## hide everything
-        self._dvhViewer.hide()
-        self._noneViewer.hide()
-        self._staticProfileviewer.hide()
-        self._staticImage3DViewer.hide()
-        self._staticImage2DViewer.hide()
-        self._staticImage3DViewer_3D.hide()
-
-        self._dynImage3DViewer.hide()
-        self._dynImage2DViewer.hide()
-
-        self._addViewersToLayout()
-
-        self._setDisplayType(self.DisplayTypes.DEFAULT)
-
-        # Logical control of the DataViewer is set here. We might want to move this to dedicated controller class
-        self._initializeControl()
-
-    def _addViewersToLayout(self):
-        self._mainLayout.addWidget(self._toolbar)
-        self._mainLayout.addWidget(self._dynImage3DViewer)
-        self._mainLayout.addWidget(self._dynImage2DViewer)
-        self._mainLayout.addWidget(self._staticImage3DViewer)
-        self._mainLayout.addWidget(self._staticImage3DViewer_3D)
-        self._mainLayout.addWidget(self._staticImage2DViewer)
-        self._mainLayout.addWidget(self._staticProfileviewer)
-        self._mainLayout.addWidget(self._noneViewer)
-        self._mainLayout.addWidget(self._dvhViewer)
-
-    @property
-    def cachedDynamicImage3DViewer(self) -> DynamicImage3DViewer:
-        """
-            The dynamic 3D image viewer currently in cache (read-only)
-
-            :type: Dynamic3DImageViewer
-        """
-        return self._dynImage3DViewer
-
-    @property
-    def cachedDynamicImage2DViewer(self) -> DynamicImage2DViewer:
-        """
-            The dynamic 2D image viewer currently in cache (read-only)
-
-            :type: Dynamic2DImageViewer
-        """
-        return self._dynImage2DViewer
-
-    @property
-    def cachedStaticDVHViewer(self) -> DVHViewer:
-        """
-            The DVH viewer currently in cache
-        """
-        return self._dvhViewer
-
-    @property
-    def cachedStaticImage3DViewer(self) -> Image3DViewer:
-        """
-            The static image 3D viewer currently in cache (read-only)
-
-            :type: Image3DViewer
-        """
-        return self._staticImage3DViewer
-
-    @property
-    def cachedStaticImage3DViewer_3D(self) -> Image3DViewer_3D:
-        return self._staticImage3DViewer_3D
-
-    @property
-    def cachedStaticImage2DViewer(self) -> Image2DViewer:
-        """
-            The static image 2D viewer currently in cache (read-only)
-
-            :type: Image2DViewer
-        """
-        return self._staticImage2DViewer
-
-    @property
-    def cachedStaticProfileViewer(self) -> ProfileViewer:
-        """
-        The profile viewer currently in cache (read-only)
-
-        :type: ProfilePlot
-        """
-        return self._staticProfileviewer
-
-    @property
-    def currentViewer(self) -> Optional[Union[DVHViewer, ProfileViewer, Image3DViewer]]:
-        """
-        The viewer currently displayed (read-only)viewerTypes
-
-        :type: Optional[Union[DVHViewer, ProfilePlot, ImageViewer]]
-        """
-        return self._currentViewer
-
-    @property
-    def displayType(self):
-        """
-        The display type of the data viewer tells whether a image viewer, a dvh viewer, ... is displayed
-
-        :type: DataViewer.viewerTypes
-        """
-        return self._displayType
-
-    @displayType.setter
-    def displayType(self, displayType):
-        self._setDisplayType(displayType)
-
-    def _setDisplayType(self, displayType):
-        if displayType == self._displayType:
-            return
-
-        isModeDynamic = self._displayMode == self.DisplayModes.DYNAMIC
-
-        if isModeDynamic:
-            self._setDisplayInDynamicMode(displayType)
-        else:
-            self._setDisplayInStaticMode(displayType)
-
-        self.displayTypeChangedSignal.emit(displayType)
-
-    def setDisplayTypeAndMode(self, args):
-        """
-        This should be used instead of the displayType and displayMode setters when the type and mode change simultaneously, for example when passing from a 3D dynamic image to a 2D static image or DVH plot
-
-        Parameters
-        ----------
-        args
-
-        Returns
-        -------
-
-        """
-        print(NotImplementedError)
-
-        return
-
-    @property
-    def displayMode(self):
-        """
-        The mode of the viewer can be dynamic for dynamic data (time series) or static for static data
-        """
-        return self._displayMode
-
-    @displayMode.setter
-    def displayMode(self, mode):
-        if mode == self._displayMode:
-            return
-
-        # Notify dynamicDisplayController - we have a problem of multiple responsibilities here
-        previousModeWasStatic = self.displayMode == self.DisplayModes.STATIC
-        if previousModeWasStatic:
-            self._viewController.dynamicDisplayController.addDynamicViewer(self.cachedDynamicImage3DViewer)
-        else:
-            self._viewController.dynamicDisplayController.removeDynamicViewer(self.cachedDynamicImage3DViewer)
-
-        self._displayMode = mode
-
-        # Reset display
-        isModeDynamic = self._displayMode == self.DisplayModes.DYNAMIC
-
-        if isModeDynamic:
-            self._setDisplayInDynamicMode(self._displayType)
-        else:
-            self._setDisplayInStaticMode(self._displayType)
-
-    @property
-    def dropMode(self):
-        return self._dropMode
-
-    @dropMode.setter
-    def dropMode(self, mode):
-        if mode==self._dropMode:
-            return
-        self._dropMode = mode
-
-    def _setDisplayInDynamicMode(self, displayType):
-        if not (self._currentViewer is None):
-            self._currentViewer.hide()
-
-        self._displayType = displayType
-
-        if self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
-            self._setCurrentViewerToDynamicImage3DViewer()
-        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
-            self._setCurrentViewerToDynamicImage2DViewer()
-        elif self._displayType == self.DisplayTypes.DISPLAY_PROFILE:
-            self._currentViewer = self._staticProfileviewer
-        elif self._displayType == self.DisplayTypes.NONE:
-            self._currentViewer = self._noneViewer
-        else:
-            raise ValueError('Invalid display type: ' + str(self._displayType))
-
-        self._currentViewer.show()
-
-    def _setDisplayInStaticMode(self, displayType):
-        if not (self._currentViewer is None):
-            self._currentViewer.hide()
-
-        self._displayType = displayType
-
-        if self._displayType == self.DisplayTypes.DISPLAY_DVH:
-            self._currentViewer = self._dvhViewer
-        elif self._displayType == self.DisplayTypes.NONE:
-            self._currentViewer = self._noneViewer
-        elif self._displayType == self.DisplayTypes.DISPLAY_PROFILE:
-            self._currentViewer = self._staticProfileviewer
-        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
-            self._setCurrentViewerToStaticImage3DViewer()
-        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
-            self._setCurrentViewerToStaticImage2DViewer()
-        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D_3D:
-            self._setCurrentViewerToStaticImage3DViewer_3D()
-        else:
-            raise ValueError('Invalid display type: ' + str(self._displayType))
-
-        self._currentViewer.show()
-
-    def _setCurrentViewerToDynamicImage3DViewer(self):
-
-        self._disconnectCurrentViewer()
-        self._currentViewer = self._dynImage3DViewer
-        self.dropEnabled = self._dropEnabled
-
-        self._viewController.crossHairEnabledSignal.connect(self._dynImage3DViewer.setCrossHairEnabled)
-        self._viewController.profileWidgetEnabledSignal.connect(self._dynImage3DViewer.setProfileWidgetEnabled)
-        self._viewController.showContourSignal.connect(self._dynImage3DViewer._contourLayer.setNewContour)
-        self._viewController.windowLevelEnabledSignal.connect(self._dynImage3DViewer.setWWLEnabled)
-
-    def _setCurrentViewerToDynamicImage2DViewer(self):
-
-        self._disconnectCurrentViewer()
-        self._currentViewer = self._dynImage2DViewer
-        self.dropEnabled = self._dropEnabled
-
-        # self._viewController.crossHairEnabledSignal.disconnect(self._staticImage3DViewer.setCrossHairEnabled)
-        # self._viewController.profileWidgetEnabledSignal.disconnect(self._staticImage3DViewer.setProfileWidgetEnabled)
-        # self._viewController.showContourSignal.disconnect(self._staticImage3DViewer._contourLayer.setNewContour)
-        # self._viewController.showContourSignal.disconnect(self._dvhViewer.appendROI)
-        # self._viewController.windowLevelEnabledSignal.disconnect(self._staticImage3DViewer.setWWLEnabled)
-
-        self._viewController.crossHairEnabledSignal.connect(self._dynImage2DViewer.setCrossHairEnabled)
-        self._viewController.profileWidgetEnabledSignal.connect(self._dynImage2DViewer.setProfileWidgetEnabled)
-        self._viewController.showContourSignal.connect(self._dynImage2DViewer._contourLayer.setNewContour)
-        self._viewController.windowLevelEnabledSignal.connect(self._dynImage2DViewer.setWWLEnabled)
-
-    def _setCurrentViewerToStaticImage3DViewer(self):
-
-        self._disconnectCurrentViewer()
-        self._currentViewer = self._staticImage3DViewer
-        self.dropEnabled = self._dropEnabled
-
-        # self._viewController.crossHairEnabledSignal.disconnect(self._dynImage3DViewer.setCrossHairEnabled)
-        # self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage3DViewer.setProfileWidgetEnabled)
-        # self._viewController.showContourSignal.disconnect(self._dynImage3DViewer._contourLayer.setNewContour)
-        # self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage3DViewer.setWWLEnabled)
-
-        self._viewController.crossHairEnabledSignal.connect(self._staticImage3DViewer.setCrossHairEnabled)
-        self._viewController.profileWidgetEnabledSignal.connect(self._staticImage3DViewer.setProfileWidgetEnabled)
-        self._viewController.showContourSignal.connect(self._staticImage3DViewer._contourLayer.setNewContour)
-        self._viewController.showContourSignal.connect(self._dvhViewer.appendROI)
-        self._viewController.windowLevelEnabledSignal.connect(self._staticImage3DViewer.setWWLEnabled)
-
-    def _setCurrentViewerToStaticImage3DViewer_3D(self):
-
-        self._disconnectCurrentViewer()
-        self._currentViewer = self._staticImage3DViewer_3D
-        self.dropEnabled = self._dropEnabled
-
-        # self._viewController.crossHairEnabledSignal.disconnect(self._dynImage3DViewer.setCrossHairEnabled)
-        # self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage3DViewer.setProfileWidgetEnabled)
-        # self._viewController.showContourSignal.disconnect(self._dynImage3DViewer._contourLayer.setNewContour)
-        # self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage3DViewer.setWWLEnabled)
-
-    def _setCurrentViewerToStaticImage2DViewer(self):
-
-        self._disconnectCurrentViewer()
-        self._currentViewer = self._staticImage2DViewer
-        self.dropEnabled = self._dropEnabled
-
-        self._viewController.crossHairEnabledSignal.connect(self._staticImage2DViewer.setCrossHairEnabled)
-        self._viewController.profileWidgetEnabledSignal.connect(self._staticImage2DViewer.setProfileWidgetEnabled)
-        self._viewController.showContourSignal.connect(self._staticImage2DViewer._contourLayer.setNewContour)
-        # self._viewController.showContourSignal.connect(self._dvhViewer.appendROI)
-        self._viewController.windowLevelEnabledSignal.connect(self._staticImage2DViewer.setWWLEnabled)
-
-    def _disconnectCurrentViewer(self):
-
-        if self._currentViewer == self._staticImage3DViewer:
-
-            self._viewController.crossHairEnabledSignal.disconnect(self._staticImage3DViewer.setCrossHairEnabled)
-            self._viewController.profileWidgetEnabledSignal.disconnect(self._staticImage3DViewer.setProfileWidgetEnabled)
-            self._viewController.showContourSignal.disconnect(self._staticImage3DViewer._contourLayer.setNewContour)
-            self._viewController.windowLevelEnabledSignal.disconnect(self._staticImage3DViewer.setWWLEnabled)
-            self._viewController.showContourSignal.disconnect(self._dvhViewer.appendROI)
-
-        elif self._currentViewer == self._dynImage3DViewer:
-
-            self._viewController.crossHairEnabledSignal.disconnect(self._dynImage3DViewer.setCrossHairEnabled)
-            self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage3DViewer.setProfileWidgetEnabled)
-            self._viewController.showContourSignal.disconnect(self._dynImage3DViewer._contourLayer.setNewContour)
-            self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage3DViewer.setWWLEnabled)
-
-        elif self._currentViewer == self._staticImage2DViewer:
-
-            self._viewController.crossHairEnabledSignal.disconnect(self._staticImage2DViewer.setCrossHairEnabled)
-            self._viewController.profileWidgetEnabledSignal.disconnect(self._staticImage2DViewer.setProfileWidgetEnabled)
-            self._viewController.showContourSignal.disconnect(self._staticImage2DViewer._contourLayer.setNewContour)
-            self._viewController.windowLevelEnabledSignal.disconnect(self._staticImage2DViewer.setWWLEnabled)
-
-        elif self._currentViewer == self._dynImage2DViewer:
-
-            self._viewController.crossHairEnabledSignal.disconnect(self._dynImage2DViewer.setCrossHairEnabled)
-            self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage2DViewer.setProfileWidgetEnabled)
-            self._viewController.showContourSignal.disconnect(self._dynImage2DViewer._contourLayer.setNewContour)
-            self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage2DViewer.setWWLEnabled)
-
-        elif self._currentViewer == self._staticImage3DViewer_3D:
-            pass
-
-
-    @property
-    def dropEnabled(self) -> bool:
-        """
-        Drag and drop enabled
-
-        :type: bool
-        """
-        return self._dropEnabled
-
-    @dropEnabled.setter
-    #TODO: Should not drop be implemented in each specific viewer?
-    def dropEnabled(self, enabled: bool):
-        self._dropEnabled = enabled
-
-        if enabled:
-            self.setAcceptDrops(True)
-            self.dragEnterEvent = lambda event: event.accept()
-            self.dropEvent = lambda event: self._dropEvent(event)
-        else:
-            self.setAcceptDrops(False)
-
-    def _dropEvent(self, e):
-        """
-            Handles a drop in the data viewer
-        """
-        if e.mimeData().hasText():
-            droppedIsImage = e.mimeData().text() == DroppedObject.DropTypes.IMAGE
-            droppedIsPlan = e.mimeData().text() == DroppedObject.DropTypes.PLAN
-
-            if droppedIsImage:
-                e.accept()
-                self.droppedImageSignal.emit(self._viewController.selectedImage)
-                return
-            elif droppedIsPlan:
-                e.accept()
-                self.droppedPlanSignal.emit(self._viewController.selectedImage)
-                return
-        e.ignore()
-
-
-
-    ####################################################################################################################
-    # This is the logical part of the viewer. Should we migrate this to a dedicated controller?
-    def _initializeControl(self):
-        self._imageViewerActions = ImageViewerActions(self._staticImage3DViewer)
-        self._dvhViewerActions = DVHViewerActions(self._dvhViewer)
-
-        self._imageViewerActions.addToToolbar(self._toolbar)
-        self._dvhViewerActions.addToToolbar(self._toolbar)
-
-        self.displayTypeChangedSignal.connect(self._handleDisplayTypeChange)
-
-        self._viewController.independentViewsEnabledSignal.connect(self.enableDrop)
-        self._viewController.mainImageChangedSignal.connect(self._setMainImageAnSwitchDisplayModeAndType)
-        self._viewController.secondaryImageChangedSignal.connect(self._setSecondaryImage)
-        self._viewController.planChangedSignal.connect(self._setPlan)
-        self._viewController.dropModeSignal.connect(self._setDropMode)
-        self._viewController.droppedDataSignal.connect(self._setDroppedData)
-
-        self.enableDrop(self._viewController.independentViewsEnabled)
-
-        self._handleDisplayTypeChange(self.displayType) # Initialize with current display type
-
-    def _handleDisplayTypeChange(self, displayType):
-        self._imageViewerActions.hide()
-
-        if displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
-            self._imageViewerActions.setImageViewer(self._currentViewer)
-            self._imageViewerActions.show()
-        if displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
-            self._imageViewerActions.setImageViewer(self._currentViewer)
-            self._imageViewerActions.show()
-
-    def enableDrop(self, enabled):
-        self.dropEnabled = enabled
-
-        if enabled:
-            # It might seems weird to have a signal connected within the class but it is if someday we want to move the logical part out of this class.
-            # See also comment on dropEnabled : Should we implement drop directly in ImageViewer?
-            self.droppedImageSignal.connect(self._setDroppedData)
-            self.droppedPlanSignal.connect(self._setPlan)
-        else:
-            self.droppedImageSignal.disconnect(self._setDroppedData)
-            self.droppedPlanSignal.disconnect(self._setPlan)
-
-    def _setDropMode(self, dropMode):
-        self.dropMode = dropMode
-
-    def _setDroppedData(self, data):
-        if isinstance(data, RTPlan):
-            self._setPlan(data)
-            return
-
-        if self._dropMode==self.DropModes.PRIMARY:
-            self._setMainImageAnSwitchDisplayModeAndType(data)
-        if self._dropMode==self.DropModes.SECONDARY:
-            self._setSecondaryImage(data)
-        if self._dropMode==self.DropModes.AUTO:
-            if isinstance(data, DoseImage):
-                self._setSecondaryImage(data)
-            else:
-                self._setMainImageAnSwitchDisplayModeAndType(data)
-
-    def _setMainImageAnSwitchDisplayModeAndType(self, image):
-        """
-            Switch display mode according to image type and then display image
-        """
-        if isinstance(image, Image3D) or isinstance(image, Dynamic3DModel):
-            self.displayMode = self.DisplayModes.STATIC
-            self.displayType = self.DisplayTypes.DISPLAY_IMAGE3D
-        elif isinstance(image, Image2D):
-            self.displayMode = self.DisplayModes.STATIC
-            self.displayType = self.DisplayTypes.DISPLAY_IMAGE2D
-        elif isinstance(image, Dynamic3DSequence):
-            self.displayMode = self.DisplayModes.DYNAMIC
-            self.displayType = self.DisplayTypes.DISPLAY_IMAGE3D
-        elif isinstance(image, Dynamic2DSequence):
-            self.displayMode = self.DisplayModes.DYNAMIC
-            self.displayType = self.DisplayTypes.DISPLAY_IMAGE2D
-        elif image is None:
-            pass
-        else:
-            raise ValueError('Image type not supported')
-
-        self._setMainImage(image)
-
-    def _setMainImage(self, image: Optional[Union[Image3D, Dynamic3DSequence, Image2D, Dynamic2DSequence, Dynamic3DModel]]):
-        """
-        Set main image to the appropriate cached image viewer.
-        Does not affect viewer visibility.
-        """
-        if isinstance(image, Image3D):
-            self.cachedStaticImage3DViewer.primaryImage = image
-            self.cachedStaticImage3DViewer_3D.primaryImage = image
-            if self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D_3D:
-                self.cachedStaticImage3DViewer_3D.update()
-        elif isinstance(image, Image2D):
-            self.cachedStaticImage2DViewer.primaryImage = image
-        elif isinstance(image, Dynamic3DSequence):
-            self.cachedDynamicImage3DViewer.primaryImage = image
-        elif isinstance(image, Dynamic2DSequence):
-            self.cachedDynamicImage2DViewer.primaryImage = image
-        elif isinstance(image, Dynamic3DModel):
-            self.cachedStaticImage3DViewer.primaryImage = image.midp
-        elif image is None:
-            if self.displayMode == self.DisplayModes.STATIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D:
-                self.cachedStaticImage3DViewer.primaryImage = None
-                self.cachedStaticImage3DViewer_3D.primaryImage = image
-            elif self.displayMode == self.DisplayModes.STATIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE2D:
-                self.cachedStaticImage2DViewer.primaryImage = None
-            elif self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D:
-                self.cachedDynamicImage3DViewer.primaryImage = None
-            elif self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE2D:
-                self.cachedDynamicImage2DViewer.primaryImage = None
-
-        else:
-            raise ValueError('Image type not supported')
-
-        if not image is None and not image.patient is None:
-            image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
-
-    def _setSecondaryImage(self, image: Optional[Image3D]):
-        """
-            Display the image (in static mode)
-            Does not affect viewer visibility nor viewer type.
-        """
-
-        if image is None:
-            oldImage = self.cachedStaticImage3DViewer.secondaryImage
-            if oldImage is None:
-                return
-        elif not (image.patient is None):
-            image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
-
-        self.cachedStaticImage3DViewer.secondaryImage = image
-        self.cachedStaticImage3DViewer_3D.secondaryImage = image
-        self._setDVHDose(image)
-
-    def _setPlan(self, plan:Optional[RTPlan]):
-        self.cachedStaticImage3DViewer.rtPlan = plan
-        self.cachedStaticImage3DViewer_3D.rtPlan = plan
-        if self.displayMode == self.DisplayModes.DYNAMIC and self.displayType == self.DisplayTypes.DISPLAY_IMAGE3D_3D:
-            self.cachedStaticImage3DViewer_3D.update()
-
-    def _setDVHDose(self, image:Optional[DoseImage]):
-        if image is None:
-            self.cachedStaticDVHViewer.clear()
-        else:
-            self.cachedStaticDVHViewer.dose = image
-
-    def _removeImageFromViewers(self, image: Union[Image3D, ]):
-        """
-        Remove image from all cached viewers --> does not work ?
-        """
-
-        if self.cachedStaticImage3DViewer.primaryImage == image:
-            self.cachedStaticImage3DViewer.primaryImage = None
-        if self.cachedStaticImage3DViewer.secondaryImage == image:
-            self._setSecondaryImage(None)
-
-        if self.cachedDynamicImage3DViewer.primaryImage == image:
-            self.cachedStaticImage3DViewer.primaryImage = image
-
-        if self.cachedStaticImage2DViewer.primaryImage == image:
-            self.cachedStaticImage2DViewer.primaryImage = image
-
-        if self.cachedDynamicImage2DViewer.primaryImage == image:
-            self.cachedDynamicImage2DViewer.primaryImage = None
-
-        if self.cachedStaticDVHViewer.dose == image:
-            self._setDVHDose(None)
-
-        if self.cachedStaticImage3DViewer_3D.primaryImage==image:
-            self.cachedStaticImage3DViewer_3D.primaryImage = None
-        if self.cachedStaticImage3DViewer_3D.secondaryImage==image:
-            self.cachedStaticImage3DViewer_3D.secondaryImage = None
-
-        #image.patient.imageRemovedSignal.disconnect(self._removeImageFromViewers)
+from enum import Enum
+from typing import Union, Optional
+
+from PyQt5.QtWidgets import QWidget, QVBoxLayout
+
+from opentps.core.data.images import DoseImage
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.images import Image2D
+from opentps.core.data.dynamicData._dynamic3DSequence import Dynamic3DSequence
+from opentps.core.data.dynamicData._dynamic3DModel import Dynamic3DModel
+from opentps.core.data.dynamicData._dynamic2DSequence import Dynamic2DSequence
+from opentps.core.data.plan._rtPlan import RTPlan
+from opentps.core import Event
+from opentps.gui.viewer.dataViewerComponents.dvhViewerActions import DVHViewerActions
+from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
+from opentps.gui.viewer.dataViewerComponents.dynamicImage3DViewer import DynamicImage3DViewer
+from opentps.gui.viewer.dataViewerComponents.image2DViewer import Image2DViewer
+from opentps.gui.viewer.dataViewerComponents.dynamicImage2DViewer import DynamicImage2DViewer
+from opentps.gui.viewer.dataViewerComponents.image3DViewer_3D import Image3DViewer_3D
+from opentps.gui.viewer.dataViewerComponents.imageViewerActions import ImageViewerActions
+from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
+from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
+from opentps.gui.viewer.dataViewerComponents.dvhPlot import DVHViewer
+from opentps.gui.viewer.dataViewerComponents.profileViewer import ProfileViewer
+
+
+class DroppedObject:
+    """
+    This class aims to standardized object dropping
+    TODO: we might want to move this to another file
+    """
+    class DropTypes:
+        # DropTypes is not an Enum because Enum does not preserve string type of class attributes. But we want Drop types
+        # to be string to be compatible with QMimeData
+        IMAGE = 'IMAGE'
+        PLAN = 'PLAN'
+
+    def __init__(self, dropType, droppedData):
+        self.dropType = dropType
+        self.droppedData = droppedData
+
+
+class DataViewer(QWidget):
+    """
+    This class displays the type of viewer specified as input and a toolbar to switch between them.
+    All viewers are cached for responsiveness.
+    Example::
+     dataViewer = DataViewer(viewController)
+     dataViewer.viewerMode = dataViewer.ViewerModes.STATIC # Static mode (for data which are not time series)
+     dataViewer.displayType = dataViewer.ViewerTypes.VIEWER_IMAGE # Show an image viewer
+     dataViewe.displayMode = dataViewer.ViewerTypes.VIEWER_DVH # Switch to a DVH viewer
+    Currently the DataViewer has its own logic based on events in viewController. Should we have a controller to specifically handle the logical part?
+    """
+    class DisplayTypes(Enum):
+        """
+            viewer types
+        """
+        NONE = None
+        DISPLAY_DVH = 'DISPLAY_DVH'
+        DISPLAY_PROFILE = 'DISPLAY_PROFILE'
+        DISPLAY_IMAGE3D = 'DISPLAY_IMAGE3D'
+        DISPLAY_IMAGE2D = 'DISPLAY_IMAGE2D'
+        DISPLAY_IMAGE3D_3D = 'DISPLAY_IMAGE3D_3D'
+
+        DEFAULT = DISPLAY_IMAGE3D
+
+    class DisplayModes(Enum):
+        """
+            viewer modes
+        """
+        STATIC = 'STATIC'
+        DYNAMIC = 'DYNAMIC'
+
+        DEFAULT = STATIC
+
+    class DropModes(Enum):
+        AUTO = 'auto'
+        PRIMARY = 'primary'
+        SECONDARY = 'secondary'
+
+        DEFAULT = AUTO
+
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+
+        # It might seems weird to have a signal which is only used within the class but it is if someday we want to move the logical part out of this class.
+        self.droppedImageSignal = Event(object)
+        self.droppedPlanSignal = Event(object)
+        self.displayTypeChangedSignal = Event(object)
+
+        self._viewController = viewController
+
+        self._currentViewer = None
+        self._displayMode = self.DisplayModes.DEFAULT
+        self._displayType = None
+
+        self._dropMode = self._viewController.dropMode
+        self._dropEnabled = False
+
+        self._mainLayout = QVBoxLayout(self)
+        self.setLayout(self._mainLayout)
+        self._mainLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._toolbar = DataViewerToolbar(self)
+
+        # For responsiveness, we instantiate all possible viewers and hide them == cached viewers:
+        self._dvhViewer = DVHViewer(self)
+        self._noneViewer = BlackEmptyPlot(self)
+        self._staticProfileviewer = ProfileViewer(viewController)
+        self._staticImage3DViewer = Image3DViewer(viewController)
+        self._staticImage2DViewer = Image2DViewer(viewController)
+        self._staticImage3DViewer_3D = Image3DViewer_3D(viewController)
+
+        ## dynamic stuff
+        self._dynImage3DViewer = DynamicImage3DViewer(viewController)
+        self._dynImage2DViewer = DynamicImage2DViewer(viewController)
+
+        ## hide everything
+        self._dvhViewer.hide()
+        self._noneViewer.hide()
+        self._staticProfileviewer.hide()
+        self._staticImage3DViewer.hide()
+        self._staticImage2DViewer.hide()
+        self._staticImage3DViewer_3D.hide()
+
+        self._dynImage3DViewer.hide()
+        self._dynImage2DViewer.hide()
+
+        self._addViewersToLayout()
+
+        self._setDisplayType(self.DisplayTypes.DEFAULT)
+
+        # Logical control of the DataViewer is set here. We might want to move this to dedicated controller class
+        self._initializeControl()
+
+    def closeEvent(self, QCloseEvent):
+        self.cachedStaticImage3DViewer.close()
+        self.cachedStaticImage2DViewer.close()
+        self.cachedStaticImage3DViewer_3D.close()
+        self.cachedDynamicImage3DViewer.close()
+        self.cachedDynamicImage2DViewer.close()
+        super().closeEvent(QCloseEvent)
+
+    def _addViewersToLayout(self):
+        self._mainLayout.addWidget(self._toolbar)
+        self._mainLayout.addWidget(self._dynImage3DViewer)
+        self._mainLayout.addWidget(self._dynImage2DViewer)
+        self._mainLayout.addWidget(self._staticImage3DViewer)
+        self._mainLayout.addWidget(self._staticImage3DViewer_3D)
+        self._mainLayout.addWidget(self._staticImage2DViewer)
+        self._mainLayout.addWidget(self._staticProfileviewer)
+        self._mainLayout.addWidget(self._noneViewer)
+        self._mainLayout.addWidget(self._dvhViewer)
+
+    @property
+    def cachedDynamicImage3DViewer(self) -> DynamicImage3DViewer:
+        """
+            The dynamic 3D image viewer currently in cache (read-only)
+
+            :type: Dynamic3DImageViewer
+        """
+        return self._dynImage3DViewer
+
+    @property
+    def cachedDynamicImage2DViewer(self) -> DynamicImage2DViewer:
+        """
+            The dynamic 2D image viewer currently in cache (read-only)
+
+            :type: Dynamic2DImageViewer
+        """
+        return self._dynImage2DViewer
+
+    @property
+    def cachedStaticDVHViewer(self) -> DVHViewer:
+        """
+            The DVH viewer currently in cache
+        """
+        return self._dvhViewer
+
+    @property
+    def cachedStaticImage3DViewer(self) -> Image3DViewer:
+        """
+            The static image 3D viewer currently in cache (read-only)
+
+            :type: Image3DViewer
+        """
+        return self._staticImage3DViewer
+
+    @property
+    def cachedStaticImage3DViewer_3D(self) -> Image3DViewer_3D:
+        return self._staticImage3DViewer_3D
+
+    @property
+    def cachedStaticImage2DViewer(self) -> Image2DViewer:
+        """
+            The static image 2D viewer currently in cache (read-only)
+
+            :type: Image2DViewer
+        """
+        return self._staticImage2DViewer
+
+    @property
+    def cachedStaticProfileViewer(self) -> ProfileViewer:
+        """
+        The profile viewer currently in cache (read-only)
+
+        :type: ProfilePlot
+        """
+        return self._staticProfileviewer
+
+    @property
+    def currentViewer(self) -> Optional[Union[DVHViewer, ProfileViewer, Image3DViewer]]:
+        """
+        The viewer currently displayed (read-only)viewerTypes
+
+        :type: Optional[Union[DVHViewer, ProfilePlot, ImageViewer]]
+        """
+        return self._currentViewer
+
+    @property
+    def displayType(self):
+        """
+        The display type of the data viewer tells whether a image viewer, a dvh viewer, ... is displayed
+
+        :type: DataViewer.viewerTypes
+        """
+        return self._displayType
+
+    @displayType.setter
+    def displayType(self, displayType):
+        self._setDisplayType(displayType)
+
+    def _setDisplayType(self, displayType):
+        if displayType == self._displayType:
+            return
+
+        isModeDynamic = self._displayMode == self.DisplayModes.DYNAMIC
+
+        if isModeDynamic:
+            self._setDisplayInDynamicMode(displayType)
+        else:
+            self._setDisplayInStaticMode(displayType)
+
+        self.displayTypeChangedSignal.emit(displayType)
+
+    def setDisplayTypeAndMode(self, args):
+        """
+        This should be used instead of the displayType and displayMode setters when the type and mode change simultaneously, for example when passing from a 3D dynamic image to a 2D static image or DVH plot
+
+        Parameters
+        ----------
+        args
+
+        Returns
+        -------
+
+        """
+        print(NotImplementedError)
+
+        return
+
+    @property
+    def displayMode(self):
+        """
+        The mode of the viewer can be dynamic for dynamic data (time series) or static for static data
+        """
+        return self._displayMode
+
+    @displayMode.setter
+    def displayMode(self, mode):
+        if mode == self._displayMode:
+            return
+
+        self._disconnectAllViewers()
+
+        # Notify dynamicDisplayController - we have a problem of multiple responsibilities here
+        previousModeWasStatic = self.displayMode == self.DisplayModes.STATIC
+        if previousModeWasStatic:
+            self._viewController.dynamicDisplayController.addDynamicViewer(self.cachedDynamicImage3DViewer)
+        else:
+            self._viewController.dynamicDisplayController.removeDynamicViewer(self.cachedDynamicImage3DViewer)
+
+        self._displayMode = mode
+
+        # Reset display
+        isModeDynamic = self._displayMode == self.DisplayModes.DYNAMIC
+
+        if isModeDynamic:
+            self._setDisplayInDynamicMode(self._displayType)
+        else:
+            self._setDisplayInStaticMode(self._displayType)
+
+    @property
+    def dropMode(self):
+        return self._dropMode
+
+    @dropMode.setter
+    def dropMode(self, mode):
+        if mode==self._dropMode:
+            return
+        self._dropMode = mode
+
+    def _setDisplayInDynamicMode(self, displayType):
+        if not (self._currentViewer is None):
+            self._currentViewer.hide()
+
+        self._displayType = displayType
+
+        if self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
+            self._setCurrentViewerToDynamicImage3DViewer()
+        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
+            self._setCurrentViewerToDynamicImage2DViewer()
+        elif self._displayType == self.DisplayTypes.DISPLAY_PROFILE:
+            self._currentViewer = self._staticProfileviewer
+        elif self._displayType == self.DisplayTypes.NONE:
+            self._currentViewer = self._noneViewer
+        else:
+            raise ValueError('Invalid display type: ' + str(self._displayType))
+
+        self._currentViewer.show()
+
+    def _setDisplayInStaticMode(self, displayType):
+        if not (self._currentViewer is None):
+            self._currentViewer.hide()
+
+        self._displayType = displayType
+
+        if self._displayType == self.DisplayTypes.DISPLAY_DVH:
+            self._currentViewer = self._dvhViewer
+            self._connectAllViewersInStatic3D()
+        elif self._displayType == self.DisplayTypes.NONE:
+            self._currentViewer = self._noneViewer
+        elif self._displayType == self.DisplayTypes.DISPLAY_PROFILE:
+            self._currentViewer = self._staticProfileviewer
+            self._connectAllViewersInStatic3D()
+        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
+            self._setCurrentViewerToStaticImage3DViewer()
+            self._connectAllViewersInStatic3D()
+        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
+            self._setCurrentViewerToStaticImage2DViewer()
+        elif self._displayType == self.DisplayTypes.DISPLAY_IMAGE3D_3D:
+            self._setCurrentViewerToStaticImage3DViewer_3D()
+            self._connectAllViewersInStatic3D()
+        else:
+            raise ValueError('Invalid display type: ' + str(self._displayType))
+
+        self._currentViewer.show()
+
+    def _setCurrentViewerToDynamicImage3DViewer(self):
+        self._currentViewer = self._dynImage3DViewer
+        self.dropEnabled = self._dropEnabled
+
+        self._viewController.crossHairEnabledSignal.connectIfNotAlready(self._dynImage3DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.connectIfNotAlready(self._dynImage3DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.connectIfNotAlready(self._dynImage3DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.connectIfNotAlready(self._dynImage3DViewer.setWWLEnabled)
+
+    def _setCurrentViewerToDynamicImage2DViewer(self):
+        self._currentViewer = self._dynImage2DViewer
+        self.dropEnabled = self._dropEnabled
+
+        self._viewController.crossHairEnabledSignal.connectIfNotAlready(self._dynImage2DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.connectIfNotAlready(self._dynImage2DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.connectIfNotAlready(self._dynImage2DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.connectIfNotAlready(self._dynImage2DViewer.setWWLEnabled)
+
+    def _setCurrentViewerToStaticImage3DViewer(self):
+        self._currentViewer = self._staticImage3DViewer
+        self.dropEnabled = self._dropEnabled
+
+        self._connectStaticImage3DViewer()
+
+    def _connectStaticImage3DViewer(self):
+        self._viewController.crossHairEnabledSignal.connectIfNotAlready(self._staticImage3DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.connectIfNotAlready(self._staticImage3DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.connectIfNotAlready(self._staticImage3DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.connectIfNotAlready(self._staticImage3DViewer.setWWLEnabled)
+
+    def _connectDVHViewer(self):
+        self._viewController.showContourSignal.connectIfNotAlready(self._dvhViewer.appendROI)
+
+    def _setCurrentViewerToStaticImage3DViewer_3D(self):
+        self._currentViewer = self._staticImage3DViewer_3D
+        self.dropEnabled = self._dropEnabled
+
+        self._connectStaticImage3DViewer_3D()
+
+    def _connectStaticImage3DViewer_3D(self):
+        self._viewController.showContourSignal.connectIfNotAlready(self._staticImage3DViewer_3D.setNewContour)
+
+    def _connectAllViewersInStatic3D(self):
+        self._connectDVHViewer()
+        self._connectStaticImage3DViewer()
+        self._connectStaticImage3DViewer_3D()
+
+    def _setCurrentViewerToStaticImage2DViewer(self):
+        self._currentViewer = self._staticImage2DViewer
+        self.dropEnabled = self._dropEnabled
+
+        self._viewController.crossHairEnabledSignal.connectIfNotAlready(self._staticImage2DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.connectIfNotAlready(self._staticImage2DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.connectIfNotAlready(self._staticImage2DViewer._contourLayer.setNewContour)
+        # self._viewController.showContourSignal.connectIfNotAlready(self._dvhViewer.appendROI)
+        self._viewController.windowLevelEnabledSignal.connectIfNotAlready(self._staticImage2DViewer.setWWLEnabled)
+
+    def _disconnectAllViewers(self):
+        self._viewController.crossHairEnabledSignal.disconnect(self._staticImage3DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.disconnect(self._staticImage3DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.disconnect(self._staticImage3DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.disconnect(self._staticImage3DViewer.setWWLEnabled)
+        self._viewController.showContourSignal.disconnect(self._dvhViewer.appendROI)
+
+        self._viewController.crossHairEnabledSignal.disconnect(self._dynImage3DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage3DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.disconnect(self._dynImage3DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage3DViewer.setWWLEnabled)
+
+        self._viewController.crossHairEnabledSignal.disconnect(self._staticImage2DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.disconnect(self._staticImage2DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.disconnect(self._staticImage2DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.disconnect(self._staticImage2DViewer.setWWLEnabled)
+
+        self._viewController.crossHairEnabledSignal.disconnect(self._dynImage2DViewer.setCrossHairEnabled)
+        self._viewController.profileWidgetEnabledSignal.disconnect(self._dynImage2DViewer.setProfileWidgetEnabled)
+        self._viewController.showContourSignal.disconnect(self._dynImage2DViewer._contourLayer.setNewContour)
+        self._viewController.windowLevelEnabledSignal.disconnect(self._dynImage2DViewer.setWWLEnabled)
+
+        self._viewController.showContourSignal.disconnect(self._staticImage3DViewer_3D.setNewContour)
+
+    @property
+    def dropEnabled(self) -> bool:
+        """
+        Drag and drop enabled
+
+        :type: bool
+        """
+        return self._dropEnabled
+
+    @dropEnabled.setter
+    #TODO: Should not drop be implemented in each specific viewer?
+    def dropEnabled(self, enabled: bool):
+        self._dropEnabled = enabled
+
+        if enabled:
+            self.setAcceptDrops(True)
+            self.dragEnterEvent = lambda event: event.accept()
+            self.dropEvent = lambda event: self._dropEvent(event)
+        else:
+            self.setAcceptDrops(False)
+
+    def _dropEvent(self, e):
+        """
+            Handles a drop in the data viewer
+        """
+        if e.mimeData().hasText():
+            droppedIsImage = e.mimeData().text() == DroppedObject.DropTypes.IMAGE
+            droppedIsPlan = e.mimeData().text() == DroppedObject.DropTypes.PLAN
+
+            if droppedIsImage:
+                e.accept()
+                self.droppedImageSignal.emit(self._viewController.selectedImage)
+                return
+            elif droppedIsPlan:
+                e.accept()
+                self.droppedPlanSignal.emit(self._viewController.selectedImage)
+                return
+        e.ignore()
+
+
+
+    ####################################################################################################################
+    # This is the logical part of the viewer. Should we migrate this to a dedicated controller?
+    def _initializeControl(self):
+        self._imageViewerActions = ImageViewerActions(self._staticImage3DViewer)
+        self._dvhViewerActions = DVHViewerActions(self._dvhViewer)
+
+        self._imageViewerActions.addToToolbar(self._toolbar)
+        self._dvhViewerActions.addToToolbar(self._toolbar)
+
+        self.displayTypeChangedSignal.connectIfNotAlready(self._handleDisplayTypeChange)
+
+        self._viewController.independentViewsEnabledSignal.connectIfNotAlready(self.enableDrop)
+        self._viewController.mainImageChangedSignal.connectIfNotAlready(self._setMainImageAnSwitchDisplayModeAndType)
+        self._viewController.secondaryImageChangedSignal.connectIfNotAlready(self._setSecondaryImage)
+        self._viewController.planChangedSignal.connectIfNotAlready(self._setPlan)
+        self._viewController.dropModeSignal.connectIfNotAlready(self._setDropMode)
+        self._viewController.droppedDataSignal.connectIfNotAlready(self._setDroppedData)
+
+        self.enableDrop(self._viewController.independentViewsEnabled)
+
+        self._handleDisplayTypeChange(self.displayType) # Initialize with current display type
+
+    def _handleDisplayTypeChange(self, displayType):
+        self._imageViewerActions.hide()
+
+        if displayType == self.DisplayTypes.DISPLAY_IMAGE3D:
+            self._imageViewerActions.setImageViewer(self._currentViewer)
+            self._imageViewerActions.show()
+        if displayType == self.DisplayTypes.DISPLAY_IMAGE2D:
+            self._imageViewerActions.setImageViewer(self._currentViewer)
+            self._imageViewerActions.show()
+
+    def enableDrop(self, enabled):
+        self.dropEnabled = enabled
+
+        if enabled:
+            # It might seems weird to have a signal connected within the class but it is if someday we want to move the logical part out of this class.
+            # See also comment on dropEnabled : Should we implement drop directly in ImageViewer?
+            self.droppedImageSignal.connectIfNotAlready(self._setDroppedData)
+            self.droppedPlanSignal.connectIfNotAlready(self._setPlan)
+        else:
+            self.droppedImageSignal.disconnect(self._setDroppedData)
+            self.droppedPlanSignal.disconnect(self._setPlan)
+
+    def _setDropMode(self, dropMode):
+        self.dropMode = dropMode
+
+    def _setDroppedData(self, data):
+        if isinstance(data, RTPlan):
+            self._setPlan(data)
+            return
+
+        if self._dropMode==self.DropModes.PRIMARY:
+            self._setMainImageAnSwitchDisplayModeAndType(data)
+        if self._dropMode==self.DropModes.SECONDARY:
+            self._setSecondaryImage(data)
+        if self._dropMode==self.DropModes.AUTO:
+            if isinstance(data, DoseImage):
+                self._setSecondaryImage(data)
+            else:
+                self._setMainImageAnSwitchDisplayModeAndType(data)
+
+    def _setMainImageAnSwitchDisplayModeAndType(self, image):
+        """
+            Switch display mode according to image type and then display image
+        """
+        if isinstance(image, Image3D) or isinstance(image, Dynamic3DModel):
+            self.displayMode = self.DisplayModes.STATIC
+            self.displayType = self.DisplayTypes.DISPLAY_IMAGE3D
+        elif isinstance(image, Image2D):
+            self.displayMode = self.DisplayModes.STATIC
+            self.displayType = self.DisplayTypes.DISPLAY_IMAGE2D
+        elif isinstance(image, Dynamic3DSequence):
+            self.displayMode = self.DisplayModes.DYNAMIC
+            self.displayType = self.DisplayTypes.DISPLAY_IMAGE3D
+        elif isinstance(image, Dynamic2DSequence):
+            self.displayMode = self.DisplayModes.DYNAMIC
+            self.displayType = self.DisplayTypes.DISPLAY_IMAGE2D
+        elif image is None:
+            pass
+        else:
+            raise ValueError('Image type not supported')
+
+        self._setMainImage(image)
+
+    def _setMainImage(self, image: Optional[Union[Image3D, Dynamic3DSequence, Image2D, Dynamic2DSequence, Dynamic3DModel]]):
+        """
+        Set main image to the appropriate cached image viewer.
+        Does not affect viewer visibility.
+        """
+        if isinstance(image, Image3D):
+            self.cachedStaticImage3DViewer.primaryImage = image
+            self.cachedStaticImage3DViewer_3D.primaryImage = image
+            if self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D_3D:
+                self.cachedStaticImage3DViewer_3D.update()
+        elif isinstance(image, Image2D):
+            self.cachedStaticImage2DViewer.primaryImage = image
+        elif isinstance(image, Dynamic3DSequence):
+            self.cachedDynamicImage3DViewer.primaryImage = image
+        elif isinstance(image, Dynamic2DSequence):
+            self.cachedDynamicImage2DViewer.primaryImage = image
+        elif isinstance(image, Dynamic3DModel):
+            self.cachedStaticImage3DViewer.primaryImage = image.midp
+        elif image is None:
+            if self.displayMode == self.DisplayModes.STATIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D:
+                self.cachedStaticImage3DViewer.primaryImage = None
+                self.cachedStaticImage3DViewer_3D.primaryImage = image
+            elif self.displayMode == self.DisplayModes.STATIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE2D:
+                self.cachedStaticImage2DViewer.primaryImage = None
+            elif self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE3D:
+                self.cachedDynamicImage3DViewer.primaryImage = None
+            elif self.displayMode == self.DisplayModes.DYNAMIC and self.displayType==self.DisplayTypes.DISPLAY_IMAGE2D:
+                self.cachedDynamicImage2DViewer.primaryImage = None
+
+        else:
+            raise ValueError('Image type not supported')
+
+        if not image is None and not image.patient is None:
+            image.patient.imageRemovedSignal.connectIfNotAlready(self._removeImageFromViewers)
+
+    def _setSecondaryImage(self, image: Optional[Image3D]):
+        """
+            Display the image (in static mode)
+            Does not affect viewer visibility nor viewer type.
+        """
+
+        if image is None:
+            oldImage = self.cachedStaticImage3DViewer.secondaryImage
+            if oldImage is None:
+                return
+        elif not (image.patient is None):
+            image.patient.imageRemovedSignal.connectIfNotAlready(self._removeImageFromViewers)
+
+        self.cachedStaticImage3DViewer.secondaryImage = image
+        self.cachedStaticImage3DViewer_3D.secondaryImage = image
+        self._setDVHDose(image)
+
+    def _setPlan(self, plan:Optional[RTPlan]):
+        self.cachedStaticImage3DViewer.rtPlan = plan
+        self.cachedStaticImage3DViewer_3D.rtPlan = plan
+        if self.displayMode == self.DisplayModes.DYNAMIC and self.displayType == self.DisplayTypes.DISPLAY_IMAGE3D_3D:
+            self.cachedStaticImage3DViewer_3D.update()
+
+    def _setDVHDose(self, image:Optional[DoseImage]):
+        self.cachedStaticDVHViewer.dose = image
+
+    def _removeImageFromViewers(self, image: Union[Image3D, ]):
+        """
+        Remove image from all cached viewers --> does not work ?
+        """
+
+        if self.cachedStaticImage3DViewer.primaryImage == image:
+            self.cachedStaticImage3DViewer.primaryImage = None
+        if self.cachedStaticImage3DViewer.secondaryImage == image:
+            self._setSecondaryImage(None)
+
+        if self.cachedDynamicImage3DViewer.primaryImage == image:
+            self.cachedStaticImage3DViewer.primaryImage = image
+
+        if self.cachedStaticImage2DViewer.primaryImage == image:
+            self.cachedStaticImage2DViewer.primaryImage = image
+
+        if self.cachedDynamicImage2DViewer.primaryImage == image:
+            self.cachedDynamicImage2DViewer.primaryImage = None
+
+        if self.cachedStaticDVHViewer.dose == image:
+            self._setDVHDose(None)
+
+        if self.cachedStaticImage3DViewer_3D.primaryImage==image:
+            self.cachedStaticImage3DViewer_3D.primaryImage = None
+        if self.cachedStaticImage3DViewer_3D.secondaryImage==image:
+            self.cachedStaticImage3DViewer_3D.secondaryImage = None
+
+        #image.patient.imageRemovedSignal.disconnect(self._removeImageFromViewers)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dataViewerToolbar.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dataViewerToolbar.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import os
-
-from PyQt5.QtCore import QSize
-from PyQt5.QtGui import QIcon
-from PyQt5.QtWidgets import QToolBar, QAction, QMenu, QWidgetAction, QPushButton
-import opentps.gui.res.icons as IconModule
-
-class DataViewerToolbar(QToolBar):
-    def __init__(self, dataViewer):
-        super().__init__(dataViewer)
-
-        self._dataViewer = dataViewer
-
-        self.setIconSize(QSize(16, 16))
-
-        # TODO use full path from import opentps_core.res.icons as iconModule
-        iconPath = IconModule.__path__[0] + os.path.sep
-
-        self._buttonDVH = QAction(QIcon(iconPath + "dvh.png"), "DVH", self)
-        self._buttonDVH.setStatusTip("DVH")
-        self._buttonDVH.triggered.connect(self._handleButtonDVH)
-        self._buttonDVH.setCheckable(True)
-
-        self._buttonProfile = QAction(QIcon(iconPath + "profile.png"), "Graph", self)
-        self._buttonProfile.setStatusTip("Graph")
-        self._buttonProfile.triggered.connect(self._handleButtonGraph)
-        self._buttonProfile.setCheckable(True)
-
-        self._buttonViewer = QAction(QIcon(iconPath + "x-ray.png"), "Image viewer", self)
-        self._buttonViewer.setStatusTip("Image viewer")
-        self._buttonViewer.triggered.connect(self._handleButtonViewer)
-        self._buttonViewer.setCheckable(True)
-
-        self._buttonViewer_3D = QAction(QIcon(iconPath + "cube.png"), "3D Image viewer", self)
-        self._buttonViewer_3D.setStatusTip("3D Image viewer")
-        self._buttonViewer_3D.triggered.connect(self._handleButtonViewer_3D)
-        self._buttonViewer_3D.setCheckable(True)
-
-        self.addAction(self._buttonViewer)
-        self.addAction(self._buttonProfile)
-        self.addAction(self._buttonDVH)
-        self.addAction(self._buttonViewer_3D)
-
-        self._menuButton = QPushButton("tools", self)
-        self._menu = QMenu(self._menuButton)
-        self._menuButton.setMenu(self._menu)
-        self._menuAction = QWidgetAction(None)
-        self._menuAction.setDefaultWidget(self._menuButton)
-        self.addAction(self._menuAction)
-
-        self._dataViewer.displayTypeChangedSignal.connect(self._handleDisplayTypeChange)
-
-    @property
-    def toolsMenu(self) -> QMenu:
-        return self._menu
-
-    def _handleButtonDVH(self, pressed):
-        if pressed:
-            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_DVH
-
-    def _handleButtonGraph(self, pressed):
-        if pressed:
-            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_PROFILE
-
-    def _handleButtonViewer(self, pressed):
-        if pressed:
-            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D
-
-    def _handleButtonViewer_3D(self, pressed):
-        if pressed:
-            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D_3D
-
-    def _handleDisplayTypeChange(self, displayType):
-        self._uncheckAllDisplayButton()
-
-        if displayType == self._dataViewer.DisplayTypes.DISPLAY_DVH:
-            self._buttonDVH.setChecked(True)
-        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_PROFILE:
-            self._buttonProfile.setChecked(True)
-        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D:
-            self._buttonViewer.setChecked(True)
-        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D_3D:
-            self._buttonViewer_3D.setChecked(True)
-
-    def _uncheckAllDisplayButton(self):
-        self._buttonDVH.setChecked(False)
-        self._buttonProfile.setChecked(False)
-        self._buttonViewer.setChecked(False)
-        self._buttonViewer_3D.setChecked(False)
+import os
+
+from PyQt5.QtCore import QSize
+from PyQt5.QtGui import QIcon
+from PyQt5.QtWidgets import QToolBar, QAction, QMenu, QWidgetAction, QPushButton
+import opentps.gui.res.icons as IconModule
+
+class DataViewerToolbar(QToolBar):
+    def __init__(self, dataViewer):
+        super().__init__(dataViewer)
+
+        self._dataViewer = dataViewer
+
+        self.setIconSize(QSize(16, 16))
+
+        # TODO use full path from import opentps_core.res.icons as iconModule
+        iconPath = IconModule.__path__[0] + os.path.sep
+
+        self._buttonDVH = QAction(QIcon(iconPath + "dvh.png"), "DVH", self)
+        self._buttonDVH.setStatusTip("DVH")
+        self._buttonDVH.triggered.connect(self._handleButtonDVH)
+        self._buttonDVH.setCheckable(True)
+
+        self._buttonProfile = QAction(QIcon(iconPath + "profile.png"), "Graph", self)
+        self._buttonProfile.setStatusTip("Graph")
+        self._buttonProfile.triggered.connect(self._handleButtonGraph)
+        self._buttonProfile.setCheckable(True)
+
+        self._buttonViewer = QAction(QIcon(iconPath + "x-ray.png"), "Image viewer", self)
+        self._buttonViewer.setStatusTip("Image viewer")
+        self._buttonViewer.triggered.connect(self._handleButtonViewer)
+        self._buttonViewer.setCheckable(True)
+
+        self._buttonViewer_3D = QAction(QIcon(iconPath + "cube.png"), "3D Image viewer", self)
+        self._buttonViewer_3D.setStatusTip("3D Image viewer")
+        self._buttonViewer_3D.triggered.connect(self._handleButtonViewer_3D)
+        self._buttonViewer_3D.setCheckable(True)
+
+        self.addAction(self._buttonViewer)
+        self.addAction(self._buttonProfile)
+        self.addAction(self._buttonDVH)
+        self.addAction(self._buttonViewer_3D)
+
+        self._menuButton = QPushButton("tools", self)
+        self._menu = QMenu(self._menuButton)
+        self._menuButton.setMenu(self._menu)
+        self._menuAction = QWidgetAction(None)
+        self._menuAction.setDefaultWidget(self._menuButton)
+        self.addAction(self._menuAction)
+
+        self._dataViewer.displayTypeChangedSignal.connect(self._handleDisplayTypeChange)
+
+    @property
+    def toolsMenu(self) -> QMenu:
+        return self._menu
+
+    def _handleButtonDVH(self, pressed):
+        if pressed:
+            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_DVH
+
+    def _handleButtonGraph(self, pressed):
+        if pressed:
+            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_PROFILE
+
+    def _handleButtonViewer(self, pressed):
+        if pressed:
+            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D
+
+    def _handleButtonViewer_3D(self, pressed):
+        if pressed:
+            self._dataViewer.displayType = self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D_3D
+
+    def _handleDisplayTypeChange(self, displayType):
+        self._uncheckAllDisplayButton()
+
+        if displayType == self._dataViewer.DisplayTypes.DISPLAY_DVH:
+            self._buttonDVH.setChecked(True)
+        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_PROFILE:
+            self._buttonProfile.setChecked(True)
+        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D:
+            self._buttonViewer.setChecked(True)
+        elif displayType == self._dataViewer.DisplayTypes.DISPLAY_IMAGE3D_3D:
+            self._buttonViewer_3D.setChecked(True)
+
+    def _uncheckAllDisplayButton(self):
+        self._buttonDVH.setChecked(False)
+        self._buttonProfile.setChecked(False)
+        self._buttonViewer.setChecked(False)
+        self._buttonViewer_3D.setChecked(False)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/doseComparisonImageProvider.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/doseComparisonImageProvider.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import typing
-from enum import Enum
-
-import numpy as np
-
-from opentps.core.data.images import DoseImage
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.processing.imageProcessing import resampler3D
-from opentps.core import Event
-
-
-class DoseComparisonImageProvider:
-    class Metric(Enum):
-        ABSOLUTE_DIFFERENCE = "absolute difference"
-        DIFFERENCE = "difference"
-        GAMMA = "gamma"
-        DEFAULT = "difference"
-
-    def __init__(self):
-        self.doseComparisonImageChangedSignal = Event(object)
-
-        self._dose1:typing.Optional[DoseImage] = None
-        self._dose2:typing.Optional[DoseImage] = None
-        self._comparisonMetric = self.Metric.DEFAULT
-        self._doseComparisonImage = None
-
-    @property
-    def doseComparisonImage(self) -> typing.Optional[Image3D]:
-        return self._doseComparisonImage
-
-    @property
-    def dose1(self):
-        return self._dose1
-
-    @dose1.setter
-    def dose1(self, dose:DoseImage):
-        self._disconnectAll()
-        self._dose1 = dose
-        self._updateDoseComparison()
-        self._connectAll()
-
-    @property
-    def dose2(self):
-        return self._dose2
-
-    @dose2.setter
-    def dose2(self, dose:DoseImage):
-        self._disconnectAll()
-        self._dose2 = dose
-        self._updateDoseComparison()
-        self._connectAll()
-
-    @property
-    def comparisonMetric(self):
-        return self._comparisonMetric
-
-    @comparisonMetric.setter
-    def comparisonMetric(self, m):
-        self._comparisonMetric = m
-        self._updateDoseComparison()
-
-    def _updateDoseComparison(self):
-        if self._dose1 is None:
-            dose = None
-        elif self._dose2 is None:
-            dose = None
-        else:
-            dose = DoseImage.fromImage3D(self._dose1, patient=None)
-            dose2 = resampler3D.resampleImage3DOnImage3D(self._dose2, dose, inPlace=False)
-            dose2.patient = None
-
-            if self._comparisonMetric == self.Metric.DIFFERENCE:
-                dose.imageArray = dose.imageArray - dose2.imageArray
-            elif self._comparisonMetric == self.Metric.ABSOLUTE_DIFFERENCE:
-                dose.imageArray = np.abs(dose.imageArray - dose2.imageArray)
-            elif self.comparisonMetric == self.Metric.GAMMA:
-                raise NotImplementedError
-
-        self._doseComparisonImage = dose
-        if not (self._doseComparisonImage is None):
-            self._setName()
-        self.doseComparisonImageChangedSignal.emit(self._doseComparisonImage)
-
-    def _disconnectAll(self):
-        if not (self._dose1 is None):
-            self._dose1.nameChangedSignal.disconnect(self._setName)
-        if not (self._dose2 is None):
-            self._dose2.nameChangedSignal.disconnect(self._setName)
-
-    def _connectAll(self):
-        if not (self._dose1 is None):
-            self._dose1.nameChangedSignal.connect(self._setName)
-        if not (self._dose2 is None):
-            self._dose2.nameChangedSignal.connect(self._setName)
-
-    def _setName(self, *args):
-        name = ''
-
-        if self._comparisonMetric==self.Metric.DIFFERENCE:
-            name = 'Diff. btw. '
-        elif self._comparisonMetric==self.Metric.ABSOLUTE_DIFFERENCE:
-            name = 'Abs. diff. btw. '
-        elif self._comparisonMetric==self.Metric.GAMMA:
-            name = 'Gamma ind. btw. '
-
-        name += self._dose1.name
-        name += ' and '
-        name += self._dose2.name
-
-        self._doseComparisonImage.name = name
+import typing
+from enum import Enum
+
+import numpy as np
+
+from opentps.core.data.images import DoseImage
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.processing.imageProcessing import resampler3D
+from opentps.core import Event
+
+
+class DoseComparisonImageProvider:
+    class Metric(Enum):
+        ABSOLUTE_DIFFERENCE = "absolute difference"
+        DIFFERENCE = "difference"
+        GAMMA = "gamma"
+        DEFAULT = "difference"
+
+    def __init__(self):
+        self.doseComparisonImageChangedSignal = Event(object)
+
+        self._dose1:typing.Optional[DoseImage] = None
+        self._dose2:typing.Optional[DoseImage] = None
+        self._comparisonMetric = self.Metric.DEFAULT
+        self._doseComparisonImage = None
+
+    @property
+    def doseComparisonImage(self) -> typing.Optional[Image3D]:
+        return self._doseComparisonImage
+
+    @property
+    def dose1(self):
+        return self._dose1
+
+    @dose1.setter
+    def dose1(self, dose:DoseImage):
+        self._disconnectAll()
+        self._dose1 = dose
+        self._updateDoseComparison()
+        self._connectAll()
+
+    @property
+    def dose2(self):
+        return self._dose2
+
+    @dose2.setter
+    def dose2(self, dose:DoseImage):
+        self._disconnectAll()
+        self._dose2 = dose
+        self._updateDoseComparison()
+        self._connectAll()
+
+    @property
+    def comparisonMetric(self):
+        return self._comparisonMetric
+
+    @comparisonMetric.setter
+    def comparisonMetric(self, m):
+        self._comparisonMetric = m
+        self._updateDoseComparison()
+
+    def _updateDoseComparison(self):
+        if self._dose1 is None:
+            dose = None
+        elif self._dose2 is None:
+            dose = None
+        else:
+            dose = DoseImage.fromImage3D(self._dose1, patient=None)
+            dose2 = resampler3D.resampleImage3DOnImage3D(self._dose2, dose, inPlace=False)
+            dose2.patient = None
+
+            if self._comparisonMetric == self.Metric.DIFFERENCE:
+                dose.imageArray = dose.imageArray - dose2.imageArray
+            elif self._comparisonMetric == self.Metric.ABSOLUTE_DIFFERENCE:
+                dose.imageArray = np.abs(dose.imageArray - dose2.imageArray)
+            elif self.comparisonMetric == self.Metric.GAMMA:
+                raise NotImplementedError
+
+        self._doseComparisonImage = dose
+        if not (self._doseComparisonImage is None):
+            self._setName()
+        self.doseComparisonImageChangedSignal.emit(self._doseComparisonImage)
+
+    def _disconnectAll(self):
+        if not (self._dose1 is None):
+            self._dose1.nameChangedSignal.disconnect(self._setName)
+        if not (self._dose2 is None):
+            self._dose2.nameChangedSignal.disconnect(self._setName)
+
+    def _connectAll(self):
+        if not (self._dose1 is None):
+            self._dose1.nameChangedSignal.connect(self._setName)
+        if not (self._dose2 is None):
+            self._dose2.nameChangedSignal.connect(self._setName)
+
+    def _setName(self, *args):
+        name = ''
+
+        if self._comparisonMetric==self.Metric.DIFFERENCE:
+            name = 'Diff. btw. '
+        elif self._comparisonMetric==self.Metric.ABSOLUTE_DIFFERENCE:
+            name = 'Abs. diff. btw. '
+        elif self._comparisonMetric==self.Metric.GAMMA:
+            name = 'Gamma ind. btw. '
+
+        name += self._dose1.name
+        name += ' and '
+        name += self._dose2.name
+
+        self._doseComparisonImage.name = name
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dvhViewerActions.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dvhViewerActions.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
-from PyQt5.QtWidgets import QWidgetAction, QLabel
-
-from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
-from opentps.gui.viewer.dataViewerComponents.dvhPlot import DVHViewer
-
-
-class DVHViewerActions:
-    def __init__(self, dvhViewer:DVHViewer):
-        self._dvhViewer = dvhViewer
-
-        self._separator = None
-
-        self._doseImageLabel = QLabel('')
-        self._doseImageLabel.setFixedHeight(16)
-        self._doseImageAction = QWidgetAction(None)
-        self._doseImageAction.setDefaultWidget(self._doseImageLabel)
-
-        self._handleDoseImage()
-
-        self.hide()
-
-        self._dvhViewer.doseChangeEvent.connect(self._handleDoseImage)
-
-    def addToToolbar(self, toolbar:DataViewerToolbar):
-        self._separator = toolbar.addSeparator()
-        toolbar.addAction(self._doseImageAction)
-
-    def hide(self):
-        if not self._separator is None:
-            self._separator.setVisible(False)
-        self._doseImageAction.setVisible(False)
-
-    def show(self):
-        self._separator.setVisible(True)
-        self._handleDoseImage()
-
-    def _handleDoseImage(self, *args):
-        if self._dvhViewer.dose is None:
-            self._doseImageAction.setVisible(False)
-        else:
-            self._doseImageLabel.setText(self._dvhViewer.dose.name)
-            #TODO:listen to name change event
+
+from PyQt5.QtWidgets import QWidgetAction, QLabel
+
+from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
+from opentps.gui.viewer.dataViewerComponents.dvhPlot import DVHViewer
+
+
+class DVHViewerActions:
+    def __init__(self, dvhViewer:DVHViewer):
+        self._dvhViewer = dvhViewer
+
+        self._separator = None
+
+        self._doseImageLabel = QLabel('')
+        self._doseImageLabel.setFixedHeight(16)
+        self._doseImageAction = QWidgetAction(None)
+        self._doseImageAction.setDefaultWidget(self._doseImageLabel)
+
+        self._handleDoseImage()
+
+        self.hide()
+
+        self._dvhViewer.doseChangeEvent.connect(self._handleDoseImage)
+
+    def addToToolbar(self, toolbar:DataViewerToolbar):
+        self._separator = toolbar.addSeparator()
+        toolbar.addAction(self._doseImageAction)
+
+    def hide(self):
+        if not self._separator is None:
+            self._separator.setVisible(False)
+        self._doseImageAction.setVisible(False)
+
+    def show(self):
+        self._separator.setVisible(True)
+        self._handleDoseImage()
+
+    def _handleDoseImage(self, *args):
+        if self._dvhViewer.dose is None:
+            self._doseImageAction.setVisible(False)
+        else:
+            self._doseImageLabel.setText(self._dvhViewer.dose.name)
+            #TODO:listen to name change event
             self._doseImageAction.setVisible(True)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/dynamicImage2DViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/dynamicImage3DViewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-from opentps.gui.viewer.dataViewerComponents.image2DViewer import Image2DViewer
-from opentps.gui.viewer.dataForViewer.dyn2DSeqForViewer import Dyn2DSeqForViewer
-
-
-class DynamicImage2DViewer(Image2DViewer):
-    def __init__(self, viewController):
-        super().__init__(viewController)
-
-        self._viewController = viewController
-
-        self.dynPrimaryImgSeq = None
-        self.dynPrimaryImgSeqForViewer = None
-
-        self.dynSecondaryImgSeq = None
-        self.dynSecondaryImgSeqForViewer = None
-
-        self.dynContourImgSeq = None
-        self.dynContourImgSeqForViewer = None
-
-        self.curPrimaryImgIdx = 0
-        self.curSecondaryImgIdx = 0
-        self.curContourImgIdx = 0
-
-        self.loopStepNumber = 0
-
-
-    @property
-    def primaryImage(self):
-
-        print('in dynamicImage2DVIewer, primaryImage (property)')
-        if self._primaryImageLayer.image is None:
-            return None
-        return self.dynPrimaryImgSeqForViewer
-
-    @primaryImage.setter
-    def primaryImage(self, dyn3DImgSeq):
-        if dyn3DImgSeq is None:
-            self.dynPrimaryImgSeq = None
-            self.dynPrimaryImgSeqForViewer = None
-            super().image = None
-        elif dyn3DImgSeq != self.dynPrimaryImgSeq:
-            self.dynPrimaryImgSeq = dyn3DImgSeq
-            self.dynPrimaryImgSeqForViewer = Dyn2DSeqForViewer(self.dynPrimaryImgSeq)
-            super()._setPrimaryImageForViewer(self.dynPrimaryImgSeqForViewer)
-
-    def nextImage(self, index):
-        self.curPrimaryImgIdx = index
-        self.dynPrimaryImgSeqForViewer.currentIndexIn3DSeq = index
-        self._renderWindow.Render()
-
-    @property
-    def secondaryImage(self):
-        return None
-
-    def resetDynamicParameters(self):
-        self.curPrimaryImgIdx = 0
-        self.curSecondaryImgIdx = 0
-        self.curContourImgIdx = 0
-
+from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
+from opentps.gui.viewer.dataForViewer.dyn3DSeqForViewer import Dyn3DSeqForViewer
+
+
+class DynamicImage3DViewer(Image3DViewer):
+    def __init__(self, viewController):
+        super().__init__(viewController)
+
+        self._viewController = viewController
+
+        self.dynPrimaryImgSeq = None
+        self.dynPrimaryImgSeqForViewer = None
+
+        self.dynSecondaryImgSeq = None
+        self.dynSecondaryImgSeqForViewer = None
+
+        self.dynContourImgSeq = None
+        self.dynContourImgSeqForViewer = None
+
+        self.curPrimaryImgIdx = 0
+        self.curSecondaryImgIdx = 0
+        self.curContourImgIdx = 0
+
+        self.loopStepNumber = 0
+
+    @property
+    def primaryImage(self):
+        if self._primaryImageLayer.image is None:
+            return None
+        return self.dynPrimaryImgSeqForViewer
+
+    @primaryImage.setter
+    def primaryImage(self, dyn3DImgSeq):
+        if dyn3DImgSeq is None:
+            self.dynPrimaryImgSeq = None
+            self.dynPrimaryImgSeqForViewer = None
+            super().image = None
+        elif dyn3DImgSeq != self.dynPrimaryImgSeq:
+            self.dynPrimaryImgSeq = dyn3DImgSeq
+            self.dynPrimaryImgSeqForViewer = Dyn3DSeqForViewer(self.dynPrimaryImgSeq)
+            super()._setPrimaryImageForViewer(self.dynPrimaryImgSeqForViewer)
+
+    def nextImage(self, index):
+        self.curPrimaryImgIdx = index
+        self.dynPrimaryImgSeqForViewer.currentIndexIn3DSeq = index
+        self._renderWindow.Render()
+
+    @property
+    def secondaryImage(self):
+        return None
+
+    def resetDynamicParameters(self):
+        self.curPrimaryImgIdx = 0
+        self.curSecondaryImgIdx = 0
+        self.curContourImgIdx = 0
+
         self.loopStepNumber = 0
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image2DViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image2DViewer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,448 +1,461 @@
-import typing
-
-from PyQt5.QtWidgets import *
-
-import vtkmodules.vtkRenderingCore as vtkRenderingCore
-import vtkmodules.vtkInteractionStyle as vtkInteractionStyle
-from vtkmodules import vtkCommonMath
-from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
-from vtkmodules.vtkCommonCore import vtkCommand
-from vtkmodules.vtkRenderingCore import vtkCoordinate
-
-from opentps.core.data.images import Image2D
-from opentps.core.data.plan._rtPlan import RTPlan
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image2DForViewer import Image2DForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtPlanLayer import RTPlanLayer
-from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.crossHairLayer import CrossHairLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage2DLayer import PrimaryImage2DLayer
-from opentps.gui.viewer.dataViewerComponents.profileWidget import ProfileWidget
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage2DLayer import SecondaryImage2DLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.textLayer import TextLayer
-
-
-class Image2DViewer(QWidget):
-    # class ViewerTypes(Enum):
-    #     AXIAL = 'axial'
-    #     CORONAL = 'coronal'
-    #     SAGITTAL = 'sagittal'
-    #     DEFAULT = 'sagittal'
-    #
-    # _viewerTypesList = iter(list(ViewerTypes))
-
-
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-
-        self.crossHairEnabledSignal = Event(bool)
-        self.profileWidgeEnabledSignal = Event(bool)
-        self.wwlEnabledSignal = Event(bool)
-        self.wwlEnabledSignal = Event(bool)
-        self.viewTypeChangedSignal = Event(object)
-        self.primaryImageSignal = Event(object)
-        self.secondaryImageSignal = Event(object)
-
-        self._blackWidget = BlackEmptyPlot(self)
-        self._crossHairEnabled = False
-        self._iStyle = vtkInteractionStyle.vtkInteractorStyleImage()
-        self._leftButtonPress = False
-        self._mainLayout = QVBoxLayout()
-        self._profileWidgetNoInteractionYet = False # Used to know if initial position of profile widget must be set
-        self._renderer = vtkRenderingCore.vtkRenderer()
-        self.__sendingWWL = False
-        self._viewController = viewController
-        self._viewMatrix = vtkCommonMath.vtkMatrix4x4()
-        # self._viewType = self.ViewerTypes.DEFAULT
-        self._vtkWidget = QVTKRenderWindowInteractor(self)
-        self._wwlEnabled = False
-
-        self._renderWindow = self._vtkWidget.GetRenderWindow()
-
-        self._crossHairLayer = CrossHairLayer(self._renderer, self._renderWindow)
-        self._primaryImage2DLayer = PrimaryImage2DLayer(self._renderer, self._renderWindow, self._iStyle)
-        self._secondaryImageLayer = SecondaryImage2DLayer(self._renderer, self._renderWindow, self._iStyle)
-        self._profileWidget = ProfileWidget(self._renderer, self._renderWindow)
-        self._textLayer = TextLayer(self._renderer, self._renderWindow)
-        self._contourLayer = ContourLayer(self._renderer, self._renderWindow)
-        self._rtPlanLayer = RTPlanLayer(self._renderer, self._renderWindow)
-
-        self._profileWidget.primaryLayer = self._primaryImage2DLayer
-        self._profileWidget.secondaryLayer = self._secondaryImageLayer
-        self._profileWidget.contourLayer = self._contourLayer
-
-        # self._setViewType(self._viewType)
-        # self._contourLayer.resliceAxes = self._viewMatrix
-        # self._rtPlanLayer.resliceAxes = self._viewMatrix
-
-        self.setLayout(self._mainLayout)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-        self._mainLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._renderer.SetBackground(0, 0, 0)
-        self._renderer.GetActiveCamera().SetParallelProjection(True)
-
-        self._iStyle.SetInteractionModeToImageSlicing()
-
-        self._iStyle.AddObserver("MouseWheelForwardEvent", self.onScroll)
-        self._iStyle.AddObserver("MouseWheelBackwardEvent", self.onScroll)
-        self._iStyle.AddObserver("MouseMoveEvent", self.onMouseMove)
-        self._iStyle.AddObserver("LeftButtonPressEvent", self.onLeftButtonPressed)
-        self._iStyle.AddObserver("LeftButtonReleaseEvent", self.onLeftButtonPressed)
-
-        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
-        self._renderWindow.AddRenderer(self._renderer)
-
-    def close(self):
-        if not (self._primaryImage2DLayer.image is None):
-            self._primaryImage2DLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
-            self._primaryImage2DLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
-
-        if not (self._secondaryImageLayer.image is None):
-            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
-
-        self._primaryImage2DLayer.close()
-        self._secondaryImageLayer.close()
-        self._textLayer.close()
-        self._contourLayer.close()
-        self._crossHairLayer.close()
-        self._rtPlanLayer.close()
-
-    @property
-    def rtPlan(self) -> RTPlan:
-        raise NotImplementedError
-
-    @rtPlan.setter
-    def rtPlan(self, plan:RTPlan):
-        if not self.primaryImage is None:
-            self._rtPlanLayer.setPlan(plan, self.primaryImage)
-
-    @property
-    def primaryImage(self) -> Image2D:
-        if self._primaryImage2DLayer.image is None:
-            return None
-        return self._primaryImage2DLayer.image.data
-
-    @primaryImage.setter
-    def primaryImage(self, image: Image2D):
-        imageAlreadyDisplayed = image == self._primaryImage2DLayer.image or (not (self._primaryImage2DLayer.image is None) and image == self._primaryImage2DLayer.image.data)
-        if imageAlreadyDisplayed:
-            return
-
-        if image is None:
-            self._resetPrimaryImageLayer()
-        else:
-            self._setPrimaryImageForViewer(Image2DForViewer(image))
-
-        self.primaryImageSignal.emit(self.primaryImage)
-
-    def _resetPrimaryImageLayer(self):
-        self._primaryImage2DLayer.image = None
-        self._mainLayout.removeWidget(self._vtkWidget)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-
-    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
-
-        print('in image2DVIewer _setPrimaryImageForViewer', type(image))
-
-        self._primaryImage2DLayer.image = image
-        self._contourLayer.referenceImage = image
-        self._textLayer.setPrimaryTextLine(2, image.name)
-
-        self._handlePosition(self._primaryImage2DLayer.image.selectedPosition)
-
-        if not (self._primaryImage2DLayer.image is None):
-            self._primaryImage2DLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
-            self._primaryImage2DLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
-
-        self._primaryImage2DLayer.image.selectedPositionChangedSignal.connect(self._handlePosition)
-        self._primaryImage2DLayer.image.nameChangedSignal.connect(self._setPrimaryName)
-
-        # self._primaryImage2DLayer.resliceAxes = self._viewMatrix
-        self._contourLayer.resliceAxes = self._viewMatrix
-        self._rtPlanLayer.resliceAxes = self._viewMatrix
-
-        self._blackWidget.hide()
-        self._mainLayout.removeWidget(self._blackWidget)
-        self._mainLayout.addWidget(self._vtkWidget)
-        self._vtkWidget.show()
-
-        # Start interaction
-        self._renderWindow.GetInteractor().Start()
-
-        # Trick to instantiate image property in iStyle
-        self._iStyle.EndWindowLevel()
-        self._iStyle.OnLeftButtonDown()
-        self._iStyle.WindowLevel()
-        self._renderWindow.GetInteractor().SetEventPosition(400, 0)
-        self._iStyle.InvokeEvent(vtkCommand.StartWindowLevelEvent)
-        self._iStyle.OnLeftButtonUp()
-        self._iStyle.EndWindowLevel()
-
-        if self._wwlEnabled:
-            self._iStyle.StartWindowLevel()
-            self._iStyle.OnLeftButtonUp()
-
-        self._iStyle.SetCurrentImageNumber(0)
-
-        self._renderer.ResetCamera()
-
-        self._renderWindow.Render()
-
-    def _setPrimaryName(self, name):
-        self._textLayer.setPrimaryTextLine(2, name)
-
-    @property
-    def profileWidgetEnabled(self) -> bool:
-        return self._profileWidget.enabled
-
-    @profileWidgetEnabled.setter
-    def profileWidgetEnabled(self, enabled: bool):
-        if enabled==self._profileWidget.enabled:
-            return
-
-        if enabled and not self._profileWidget.enabled:
-            self._profileWidgetNoInteractionYet = True
-            self._profileWidget.callback = self._viewController.profileWidgetCallback
-        else:
-            self._profileWidgetNoInteractionYet = False
-        self._profileWidget.enabled = enabled
-
-        self.profileWidgeEnabledSignal.emit(self.profileWidgetEnabled)
-
-    def setProfileWidgetEnabled(self, enabled):
-        self.profileWidgetEnabled = enabled
-
-    @property
-    def secondaryImage(self) -> typing.Optional[Image2D]:
-        if self._secondaryImageLayer.image is None:
-            return None
-        return self._secondaryImageLayer.image.data
-
-    @secondaryImage.setter
-    def secondaryImage(self, image: Image2D):
-        if self.primaryImage is None:
-            return
-
-        imageAlreadyDisplayed = image == self._secondaryImageLayer.image or (not (self._secondaryImageLayer.image is None) and image == self._secondaryImageLayer.image.data)
-        if imageAlreadyDisplayed:
-            return
-
-        self._secondaryImageLayer.image = Image2DForViewer(image)
-
-        if image is None:
-            self._secondaryImageLayer.image = None
-            self.secondaryImageSignal.emit(self.secondaryImage)
-            return
-
-        self._secondaryImageLayer.resliceAxes = self._viewMatrix
-
-        self._textLayer.setSecondaryTextLine(2, self.secondaryImage.name)
-
-        if not (self._secondaryImageLayer.image is None):
-            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
-
-        self._secondaryImageLayer.image.nameChangedSignal.connect(self._setSecondaryName)
-
-        self._renderWindow.Render()
-
-        self.secondaryImageSignal.emit(self.secondaryImage)
-
-    def _setSecondaryName(self, name):
-        self._textLayer.setSecondaryTextLine(2, name)
-
-    @property
-    def secondaryImageLayer(self):
-        return self._secondaryImageLayer
-
-
-    @property
-    def viewType(self):
-        return self._viewType
-
-    @viewType.setter
-    def viewType(self, viewType):
-        if self._viewType == viewType:
-            return
-
-        self._setViewType(viewType)
-
-    def _setViewType(self, viewType):
-        self._viewType = viewType
-        coronal = vtkCommonMath.vtkMatrix4x4()
-        coronal.DeepCopy((1, 0, 0, 0,
-                          0, 0, 1, 0,
-                          0, 1, 0, 0,
-                          0, 0, 0, 1))
-
-        sagittal = vtkCommonMath.vtkMatrix4x4()
-        sagittal.DeepCopy((0, 0, -1, 0,
-                          1, 0, 0, 0,
-                          0, 1, 0, 0,
-                          0, 0, 0, 1))
-
-        axial = vtkCommonMath.vtkMatrix4x4()
-        axial.DeepCopy((1, 0, 0, 0,
-                        0, -1, 0, 0,
-                        0, 0, -1, 0,
-                        0, 0, 0, 1))
-
-        if self._viewType == self.ViewerTypes.SAGITTAL:
-            self._viewMatrix = sagittal
-        if self._viewType == self.ViewerTypes.AXIAL:
-            self._viewMatrix = axial
-        if self._viewType == self.ViewerTypes.CORONAL:
-            self._viewMatrix = coronal
-        else:
-            ValueError('Invalid viewType')
-
-        if not self.primaryImage is None:
-            self._primaryImage2DLayer.resliceAxes = self._viewMatrix
-            self._contourLayer.resliceAxes = self._viewMatrix
-            self._rtPlanLayer.resliceAxes = self._viewMatrix
-        if not self.secondaryImage is None:
-            self._secondaryImageLayer.resliceAxes = self._viewMatrix
-
-        self._renderer.ResetCamera()
-        self._renderWindow.Render()
-
-        self.viewTypeChangedSignal.emit(self._viewType)
-
-    @property
-    def crossHairEnabled(self) -> bool:
-        return self._crossHairEnabled
-
-    @crossHairEnabled.setter
-    def crossHairEnabled(self, enabled: bool):
-        if enabled == self._crossHairEnabled:
-            return
-
-        self._crossHairEnabled = enabled
-        if self._crossHairEnabled:
-            self.wwlEnabled = False
-            self._crossHairLayer.visible = True
-        else:
-            self._crossHairLayer.visible = False
-            self._handlePosition(None)
-            self._renderWindow.Render()
-        self.crossHairEnabledSignal.emit(self._crossHairEnabled)
-
-    def setCrossHairEnabled(self, enabled: bool):
-        self.crossHairEnabled = enabled
-
-    @property
-    def wwlEnabled(self) -> bool:
-        return self._wwlEnabled
-
-    @wwlEnabled.setter
-    def wwlEnabled(self, enabled: bool):
-        if enabled == self._wwlEnabled:
-            return
-
-        self._wwlEnabled = enabled
-
-        if self._wwlEnabled:
-            self.crossHairEnabled = False
-        self.wwlEnabledSignal.emit(enabled)
-
-    def setWWLEnabled(self, enabled: bool):
-        self.wwlEnabled = enabled
-
-    def onLeftButtonPressed(self, obj=None, event='Press'):
-        if 'Press' in event:
-            self._leftButtonPress = True
-
-            if self.profileWidgetEnabled:
-                self._iStyle.OnLeftButtonDown()
-                return
-
-            if self._crossHairEnabled:
-                self.onMouseMove(None, None)
-            else:
-                self._iStyle.OnLeftButtonDown()
-        else:
-            self._leftButtonPress = False
-            self._iStyle.OnLeftButtonUp()
-
-    def onMouseMove(self, obj=None, event=None):
-        (mouseX, mouseY) = self._renderWindow.GetInteractor().GetEventPosition()
-
-        # MouseX and MouseY are not related to image but to renderWindow
-        dPos = vtkCoordinate()
-        dPos.SetCoordinateSystemToDisplay()
-        dPos.SetValue(mouseX, mouseY, 0)
-        worldPos = dPos.GetComputedWorldValue(self._renderer)
-
-        point = self._viewMatrix.MultiplyPoint((worldPos[0], worldPos[1], 0, 1))
-
-        if self.profileWidgetEnabled and self._profileWidgetNoInteractionYet and self._leftButtonPress:
-            self._profileWidget.setInitialPosition((worldPos[0], worldPos[1]))
-            self._profileWidgetNoInteractionYet = False
-            return
-
-        if self._crossHairEnabled and self._leftButtonPress:
-            self._primaryImage2DLayer.image.selectedPosition = (point[0], point[1], point[2])
-
-        if self._leftButtonPress and self._wwlEnabled:
-            self._iStyle.OnMouseMove()
-            self.__sendingWWL = True
-            imageProperty = self._iStyle.GetCurrentImageProperty()
-            self._primaryImage2DLayer.image.wwlValue = (imageProperty.GetColorWindow(), imageProperty.GetColorLevel())
-            self.__sendingWWL = False
-
-        if not self._leftButtonPress:
-            self._iStyle.OnMouseMove()
-
-    def onScroll(self, obj=None, event='Forward'):
-        print(NotImplementedError)
-
-    def _handlePosition(self, position: typing.Sequence):
-        if not self._crossHairEnabled or position is None:
-            self._textLayer.setPrimaryTextLine(0, '')
-            self._textLayer.setPrimaryTextLine(1, '')
-
-            if not self.secondaryImage is None:
-                self._textLayer.setSecondaryTextLine(0, '')
-                self._textLayer.setSecondaryTextLine(1, '')
-            return
-
-        transfo_mat = vtkCommonMath.vtkMatrix4x4()
-        transfo_mat.DeepCopy(self._viewMatrix)
-        transfo_mat.Invert()
-        posAfterInverse = transfo_mat.MultiplyPoint((position[0], position[1], position[2], 1))
-
-        pos = self._viewMatrix.MultiplyPoint((0, 0, posAfterInverse[2], 1))
-
-        self._viewMatrix.SetElement(0, 3, pos[0])
-        self._viewMatrix.SetElement(1, 3, pos[1])
-        self._viewMatrix.SetElement(2, 3, pos[2])
-        if self._crossHairEnabled:
-            self._crossHairLayer.position = (posAfterInverse[0], posAfterInverse[1])
-
-        try:
-            data = self._primaryImage2DLayer.image.getDataAtPosition(position)
-
-            self._textLayer.setPrimaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
-            # self._textLayer.setPrimaryTextLine(0, 'ValueNumpy: ' + "{:.2f}".format(dataNumpy))
-            self._textLayer.setPrimaryTextLine(1,  'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
-                position[1]) + ' ' + "{:.2f}".format(position[2]))
-        except:
-            self._textLayer.setPrimaryTextLine(0, '')
-            self._textLayer.setPrimaryTextLine(1, '')
-
-        if not self.secondaryImage is None:
-            try:
-                data = self._secondaryImageLayer.image.getDataAtPosition(position)
-
-                self._textLayer.setSecondaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
-                self._textLayer.setSecondaryTextLine(1, 'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
-                    position[1]) + ' ' + "{:.2f}".format(position[2]))
-            except:
-                self._textLayer.setSecondaryTextLine(0, '')
-                self._textLayer.setSecondaryTextLine(1, '')
+import typing
+
+from PyQt5.QtWidgets import *
+
+import vtkmodules.vtkRenderingCore as vtkRenderingCore
+import vtkmodules.vtkInteractionStyle as vtkInteractionStyle
+from vtkmodules import vtkCommonMath
+from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+from vtkmodules.vtkCommonCore import vtkCommand
+from vtkmodules.vtkRenderingCore import vtkCoordinate
+
+from opentps.core.data.images import Image2D
+from opentps.core.data.plan._rtPlan import RTPlan
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image2DForViewer import Image2DForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtPlanLayer import RTPlanLayer
+from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.crossHairLayer import CrossHairLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage2DLayer import PrimaryImage2DLayer
+from opentps.gui.viewer.dataViewerComponents.profileWidget import ProfileWidget
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage2DLayer import SecondaryImage2DLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.textLayer import TextLayer
+
+
+class Image2DViewer(QWidget):
+    # class ViewerTypes(Enum):
+    #     AXIAL = 'axial'
+    #     CORONAL = 'coronal'
+    #     SAGITTAL = 'sagittal'
+    #     DEFAULT = 'sagittal'
+    #
+    # _viewerTypesList = iter(list(ViewerTypes))
+
+
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+
+        self.crossHairEnabledSignal = Event(bool)
+        self.profileWidgeEnabledSignal = Event(bool)
+        self.wwlEnabledSignal = Event(bool)
+        self.wwlEnabledSignal = Event(bool)
+        self.viewTypeChangedSignal = Event(object)
+        self.primaryImageSignal = Event(object)
+        self.secondaryImageSignal = Event(object)
+
+        self._blackWidget = BlackEmptyPlot(self)
+        self._crossHairEnabled = False
+        self._iStyle = vtkInteractionStyle.vtkInteractorStyleImage()
+        self._leftButtonPress = False
+        self._mainLayout = QVBoxLayout()
+        self._profileWidgetNoInteractionYet = False # Used to know if initial position of profile widget must be set
+        self._renderer = vtkRenderingCore.vtkRenderer()
+        self.__sendingWWL = False
+        self._viewController = viewController
+        self._viewMatrix = vtkCommonMath.vtkMatrix4x4()
+        # self._viewType = self.ViewerTypes.DEFAULT
+        self._vtkWidget = QVTKRenderWindowInteractor(self)
+        self._wwlEnabled = False
+
+        self._renderWindow = self._vtkWidget.GetRenderWindow()
+
+        self._crossHairLayer = CrossHairLayer(self._renderer, self._renderWindow)
+        self._primaryImage2DLayer = PrimaryImage2DLayer(self._renderer, self._renderWindow, self._iStyle)
+        self._secondaryImageLayer = SecondaryImage2DLayer(self._renderer, self._renderWindow, self._iStyle)
+        self._profileWidget = ProfileWidget(self._renderer, self._renderWindow)
+        self._textLayer = TextLayer(self._renderer, self._renderWindow)
+        self._contourLayer = ContourLayer(self._renderer, self._renderWindow)
+        self._rtPlanLayer = RTPlanLayer(self._renderer, self._renderWindow)
+
+        self._profileWidget.primaryLayer = self._primaryImage2DLayer
+        self._profileWidget.secondaryLayer = self._secondaryImageLayer
+        self._profileWidget.contourLayer = self._contourLayer
+
+        # self._setViewType(self._viewType)
+        # self._contourLayer.resliceAxes = self._viewMatrix
+        # self._rtPlanLayer.resliceAxes = self._viewMatrix
+
+        self.setLayout(self._mainLayout)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+        self._mainLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._renderer.SetBackground(0, 0, 0)
+        self._renderer.GetActiveCamera().SetParallelProjection(True)
+
+        self._iStyle.SetInteractionModeToImageSlicing()
+
+        self._iStyle.AddObserver("MouseWheelForwardEvent", self.onScroll)
+        self._iStyle.AddObserver("MouseWheelBackwardEvent", self.onScroll)
+        self._iStyle.AddObserver("MouseMoveEvent", self.onMouseMove)
+        self._iStyle.AddObserver("LeftButtonPressEvent", self.onLeftButtonPressed)
+        self._iStyle.AddObserver("LeftButtonReleaseEvent", self.onLeftButtonPressed)
+
+        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
+        self._renderWindow.AddRenderer(self._renderer)
+
+        self._closed = False
+
+    def closeEvent(self, QCloseEvent):
+        if self._closed:
+            return
+
+        self._closed = True
+        self.reset()
+        self._renderWindow.Finalize()
+        self._vtkWidget.close()
+        del self._renderWindow, self._vtkWidget
+        super().closeEvent(QCloseEvent)
+
+    def reset(self):
+        if not (self._primaryImage2DLayer.image is None):
+            self._primaryImage2DLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
+            self._primaryImage2DLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
+
+        if not (self._secondaryImageLayer.image is None):
+            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
+
+        self._primaryImage2DLayer.close()
+        self._secondaryImageLayer.close()
+        self._textLayer.close()
+        self._contourLayer.close()
+        self._crossHairLayer.close()
+        self._rtPlanLayer.close()
+
+    @property
+    def rtPlan(self) -> RTPlan:
+        raise NotImplementedError
+
+    @rtPlan.setter
+    def rtPlan(self, plan:RTPlan):
+        if not self.primaryImage is None:
+            self._rtPlanLayer.setPlan(plan, self.primaryImage)
+
+    @property
+    def primaryImage(self) -> Image2D:
+        if self._primaryImage2DLayer.image is None:
+            return None
+        return self._primaryImage2DLayer.image.data
+
+    @primaryImage.setter
+    def primaryImage(self, image: Image2D):
+        imageAlreadyDisplayed = image == self._primaryImage2DLayer.image or (not (self._primaryImage2DLayer.image is None) and image == self._primaryImage2DLayer.image.data)
+        if imageAlreadyDisplayed:
+            return
+
+        if image is None:
+            self._resetPrimaryImageLayer()
+        else:
+            self._setPrimaryImageForViewer(Image2DForViewer(image))
+
+        self.primaryImageSignal.emit(self.primaryImage)
+
+    def _resetPrimaryImageLayer(self):
+        self._primaryImage2DLayer.image = None
+        self._mainLayout.removeWidget(self._vtkWidget)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+
+    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
+
+        print('in image2DVIewer _setPrimaryImageForViewer', type(image))
+
+        self._primaryImage2DLayer.image = image
+        self._contourLayer.referenceImage = image
+        self._textLayer.setPrimaryTextLine(2, image.name)
+
+        self._handlePosition(self._primaryImage2DLayer.image.selectedPosition)
+
+        if not (self._primaryImage2DLayer.image is None):
+            self._primaryImage2DLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
+            self._primaryImage2DLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
+
+        self._primaryImage2DLayer.image.selectedPositionChangedSignal.connect(self._handlePosition)
+        self._primaryImage2DLayer.image.nameChangedSignal.connect(self._setPrimaryName)
+
+        # self._primaryImage2DLayer.resliceAxes = self._viewMatrix
+        self._contourLayer.resliceAxes = self._viewMatrix
+        self._rtPlanLayer.resliceAxes = self._viewMatrix
+
+        self._blackWidget.hide()
+        self._mainLayout.removeWidget(self._blackWidget)
+        self._mainLayout.addWidget(self._vtkWidget)
+        self._vtkWidget.show()
+
+        # Start interaction
+        self._renderWindow.GetInteractor().Start()
+
+        # Trick to instantiate image property in iStyle
+        self._iStyle.EndWindowLevel()
+        self._iStyle.OnLeftButtonDown()
+        self._iStyle.WindowLevel()
+        self._renderWindow.GetInteractor().SetEventPosition(400, 0)
+        self._iStyle.InvokeEvent(vtkCommand.StartWindowLevelEvent)
+        self._iStyle.OnLeftButtonUp()
+        self._iStyle.EndWindowLevel()
+
+        if self._wwlEnabled:
+            self._iStyle.StartWindowLevel()
+            self._iStyle.OnLeftButtonUp()
+
+        self._iStyle.SetCurrentImageNumber(0)
+
+        self._renderer.ResetCamera()
+
+        self._renderWindow.Render()
+
+    def _setPrimaryName(self, name):
+        self._textLayer.setPrimaryTextLine(2, name)
+
+    @property
+    def profileWidgetEnabled(self) -> bool:
+        return self._profileWidget.enabled
+
+    @profileWidgetEnabled.setter
+    def profileWidgetEnabled(self, enabled: bool):
+        if enabled==self._profileWidget.enabled:
+            return
+
+        if enabled and not self._profileWidget.enabled:
+            self._profileWidgetNoInteractionYet = True
+            self._profileWidget.callback = self._viewController.profileWidgetCallback
+        else:
+            self._profileWidgetNoInteractionYet = False
+        self._profileWidget.enabled = enabled
+
+        self.profileWidgeEnabledSignal.emit(self.profileWidgetEnabled)
+
+    def setProfileWidgetEnabled(self, enabled):
+        self.profileWidgetEnabled = enabled
+
+    @property
+    def secondaryImage(self) -> typing.Optional[Image2D]:
+        if self._secondaryImageLayer.image is None:
+            return None
+        return self._secondaryImageLayer.image.data
+
+    @secondaryImage.setter
+    def secondaryImage(self, image: Image2D):
+        if self.primaryImage is None:
+            return
+
+        imageAlreadyDisplayed = image == self._secondaryImageLayer.image or (not (self._secondaryImageLayer.image is None) and image == self._secondaryImageLayer.image.data)
+        if imageAlreadyDisplayed:
+            return
+
+        self._secondaryImageLayer.image = Image2DForViewer(image)
+
+        if image is None:
+            self._secondaryImageLayer.image = None
+            self.secondaryImageSignal.emit(self.secondaryImage)
+            return
+
+        self._secondaryImageLayer.resliceAxes = self._viewMatrix
+
+        self._textLayer.setSecondaryTextLine(2, self.secondaryImage.name)
+
+        if not (self._secondaryImageLayer.image is None):
+            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
+
+        self._secondaryImageLayer.image.nameChangedSignal.connect(self._setSecondaryName)
+
+        self._renderWindow.Render()
+
+        self.secondaryImageSignal.emit(self.secondaryImage)
+
+    def _setSecondaryName(self, name):
+        self._textLayer.setSecondaryTextLine(2, name)
+
+    @property
+    def secondaryImageLayer(self):
+        return self._secondaryImageLayer
+
+
+    @property
+    def viewType(self):
+        return self._viewType
+
+    @viewType.setter
+    def viewType(self, viewType):
+        if self._viewType == viewType:
+            return
+
+        self._setViewType(viewType)
+
+    def _setViewType(self, viewType):
+        self._viewType = viewType
+        coronal = vtkCommonMath.vtkMatrix4x4()
+        coronal.DeepCopy((1, 0, 0, 0,
+                          0, 0, 1, 0,
+                          0, 1, 0, 0,
+                          0, 0, 0, 1))
+
+        sagittal = vtkCommonMath.vtkMatrix4x4()
+        sagittal.DeepCopy((0, 0, -1, 0,
+                          1, 0, 0, 0,
+                          0, 1, 0, 0,
+                          0, 0, 0, 1))
+
+        axial = vtkCommonMath.vtkMatrix4x4()
+        axial.DeepCopy((1, 0, 0, 0,
+                        0, -1, 0, 0,
+                        0, 0, -1, 0,
+                        0, 0, 0, 1))
+
+        if self._viewType == self.ViewerTypes.SAGITTAL:
+            self._viewMatrix = sagittal
+        if self._viewType == self.ViewerTypes.AXIAL:
+            self._viewMatrix = axial
+        if self._viewType == self.ViewerTypes.CORONAL:
+            self._viewMatrix = coronal
+        else:
+            ValueError('Invalid viewType')
+
+        if not self.primaryImage is None:
+            self._primaryImage2DLayer.resliceAxes = self._viewMatrix
+            self._contourLayer.resliceAxes = self._viewMatrix
+            self._rtPlanLayer.resliceAxes = self._viewMatrix
+        if not self.secondaryImage is None:
+            self._secondaryImageLayer.resliceAxes = self._viewMatrix
+
+        self._renderer.ResetCamera()
+        self._renderWindow.Render()
+
+        self.viewTypeChangedSignal.emit(self._viewType)
+
+    @property
+    def crossHairEnabled(self) -> bool:
+        return self._crossHairEnabled
+
+    @crossHairEnabled.setter
+    def crossHairEnabled(self, enabled: bool):
+        if enabled == self._crossHairEnabled:
+            return
+
+        self._crossHairEnabled = enabled
+        if self._crossHairEnabled:
+            self.wwlEnabled = False
+            self._crossHairLayer.visible = True
+        else:
+            self._crossHairLayer.visible = False
+            self._handlePosition(None)
+            self._renderWindow.Render()
+        self.crossHairEnabledSignal.emit(self._crossHairEnabled)
+
+    def setCrossHairEnabled(self, enabled: bool):
+        self.crossHairEnabled = enabled
+
+    @property
+    def wwlEnabled(self) -> bool:
+        return self._wwlEnabled
+
+    @wwlEnabled.setter
+    def wwlEnabled(self, enabled: bool):
+        if enabled == self._wwlEnabled:
+            return
+
+        self._wwlEnabled = enabled
+
+        if self._wwlEnabled:
+            self.crossHairEnabled = False
+        self.wwlEnabledSignal.emit(enabled)
+
+    def setWWLEnabled(self, enabled: bool):
+        self.wwlEnabled = enabled
+
+    def onLeftButtonPressed(self, obj=None, event='Press'):
+        if 'Press' in event:
+            self._leftButtonPress = True
+
+            if self.profileWidgetEnabled:
+                self._iStyle.OnLeftButtonDown()
+                return
+
+            if self._crossHairEnabled:
+                self.onMouseMove(None, None)
+            else:
+                self._iStyle.OnLeftButtonDown()
+        else:
+            self._leftButtonPress = False
+            self._iStyle.OnLeftButtonUp()
+
+    def onMouseMove(self, obj=None, event=None):
+        (mouseX, mouseY) = self._renderWindow.GetInteractor().GetEventPosition()
+
+        # MouseX and MouseY are not related to image but to renderWindow
+        dPos = vtkCoordinate()
+        dPos.SetCoordinateSystemToDisplay()
+        dPos.SetValue(mouseX, mouseY, 0)
+        worldPos = dPos.GetComputedWorldValue(self._renderer)
+
+        point = self._viewMatrix.MultiplyPoint((worldPos[0], worldPos[1], 0, 1))
+
+        if self.profileWidgetEnabled and self._profileWidgetNoInteractionYet and self._leftButtonPress:
+            self._profileWidget.setInitialPosition((worldPos[0], worldPos[1]))
+            self._profileWidgetNoInteractionYet = False
+            return
+
+        if self._crossHairEnabled and self._leftButtonPress:
+            self._primaryImage2DLayer.image.selectedPosition = (point[0], point[1], point[2])
+
+        if self._leftButtonPress and self._wwlEnabled:
+            self._iStyle.OnMouseMove()
+            self.__sendingWWL = True
+            imageProperty = self._iStyle.GetCurrentImageProperty()
+            self._primaryImage2DLayer.image.wwlValue = (imageProperty.GetColorWindow(), imageProperty.GetColorLevel())
+            self.__sendingWWL = False
+
+        if not self._leftButtonPress:
+            self._iStyle.OnMouseMove()
+
+    def onScroll(self, obj=None, event='Forward'):
+        print(NotImplementedError)
+
+    def _handlePosition(self, position: typing.Sequence):
+        if not self._crossHairEnabled or position is None:
+            self._textLayer.setPrimaryTextLine(0, '')
+            self._textLayer.setPrimaryTextLine(1, '')
+
+            if not self.secondaryImage is None:
+                self._textLayer.setSecondaryTextLine(0, '')
+                self._textLayer.setSecondaryTextLine(1, '')
+            return
+
+        transfo_mat = vtkCommonMath.vtkMatrix4x4()
+        transfo_mat.DeepCopy(self._viewMatrix)
+        transfo_mat.Invert()
+        posAfterInverse = transfo_mat.MultiplyPoint((position[0], position[1], position[2], 1))
+
+        pos = self._viewMatrix.MultiplyPoint((0, 0, posAfterInverse[2], 1))
+
+        self._viewMatrix.SetElement(0, 3, pos[0])
+        self._viewMatrix.SetElement(1, 3, pos[1])
+        self._viewMatrix.SetElement(2, 3, pos[2])
+        if self._crossHairEnabled:
+            self._crossHairLayer.position = (posAfterInverse[0], posAfterInverse[1])
+
+        try:
+            data = self._primaryImage2DLayer.image.getDataAtPosition(position)
+
+            self._textLayer.setPrimaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
+            # self._textLayer.setPrimaryTextLine(0, 'ValueNumpy: ' + "{:.2f}".format(dataNumpy))
+            self._textLayer.setPrimaryTextLine(1,  'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
+                position[1]) + ' ' + "{:.2f}".format(position[2]))
+        except:
+            self._textLayer.setPrimaryTextLine(0, '')
+            self._textLayer.setPrimaryTextLine(1, '')
+
+        if not self.secondaryImage is None:
+            try:
+                data = self._secondaryImageLayer.image.getDataAtPosition(position)
+
+                self._textLayer.setSecondaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
+                self._textLayer.setSecondaryTextLine(1, 'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
+                    position[1]) + ' ' + "{:.2f}".format(position[2]))
+            except:
+                self._textLayer.setSecondaryTextLine(0, '')
+                self._textLayer.setSecondaryTextLine(1, '')
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image3DViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image3DViewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,472 +1,486 @@
-import typing
-from enum import Enum
-
-from PyQt5.QtWidgets import *
-
-import vtkmodules.vtkRenderingCore as vtkRenderingCore
-import vtkmodules.vtkInteractionStyle as vtkInteractionStyle
-from vtkmodules import vtkCommonMath
-from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
-from vtkmodules.vtkRenderingCore import vtkCoordinate
-
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.plan._rtPlan import RTPlan
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtPlanLayer import RTPlanLayer
-from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.crossHairLayer import CrossHairLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer import PrimaryImage3DLayer
-from opentps.gui.viewer.dataViewerComponents.profileWidget import ProfileWidget
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage3DLayer import SecondaryImage3DLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.textLayer import TextLayer
-
-
-class Image3DViewer(QWidget):
-    class ViewerTypes(Enum):
-        AXIAL = 'axial'
-        CORONAL = 'coronal'
-        SAGITTAL = 'sagittal'
-        DEFAULT = 'sagittal'
-
-    _viewerTypesList = iter(list(ViewerTypes))
-
-
-    def __init__(self, viewController):
-        QWidget.__init__(self)
-
-        self.crossHairEnabledSignal = Event(bool)
-        self.profileWidgeEnabledSignal = Event(bool)
-        self.wwlEnabledSignal = Event(bool)
-        self.wwlEnabledSignal = Event(bool)
-        self.viewTypeChangedSignal = Event(object)
-        self.primaryImageSignal = Event(object)
-        self.secondaryImageSignal = Event(object)
-
-        self._blackWidget = BlackEmptyPlot(self)
-        self._crossHairEnabled = False
-        self._iStyle = vtkInteractionStyle.vtkInteractorStyleImage()
-        self._leftButtonPress = False
-        self._mainLayout = QVBoxLayout()
-        self._profileWidgetNoInteractionYet = False # Used to know if initial position of profile widget must be set
-        self._renderer = vtkRenderingCore.vtkRenderer()
-        self.__sendingWWL = False
-        self._viewController = viewController
-        self._viewMatrix = vtkCommonMath.vtkMatrix4x4()
-        self._viewType = self.ViewerTypes.DEFAULT
-        self._vtkWidget = QVTKRenderWindowInteractor(self)
-        self._wwlEnabled = False
-
-        self._renderWindow = self._vtkWidget.GetRenderWindow()
-
-        self._crossHairLayer = CrossHairLayer(self._renderer, self._renderWindow)
-        self._primaryImageLayer = PrimaryImage3DLayer(self._renderer, self._renderWindow, self._iStyle)
-        self._secondaryImageLayer = SecondaryImage3DLayer(self._renderer, self._renderWindow, self._iStyle)
-        self._profileWidget = ProfileWidget(self._renderer, self._renderWindow)
-        self._textLayer = TextLayer(self._renderer, self._renderWindow)
-        self._contourLayer = ContourLayer(self._renderer, self._renderWindow)
-        self._rtPlanLayer = RTPlanLayer(self._renderer, self._renderWindow)
-
-        self._profileWidget.primaryLayer = self._primaryImageLayer
-        self._profileWidget.secondaryLayer = self._secondaryImageLayer
-        self._profileWidget.contourLayer = self._contourLayer
-
-        self._setViewType(self._viewType)
-        self._contourLayer.resliceAxes = self._viewMatrix
-        self._rtPlanLayer.resliceAxes = self._viewMatrix
-
-        self.setLayout(self._mainLayout)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-        self._mainLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._renderer.SetBackground(0, 0, 0)
-        self._renderer.GetActiveCamera().SetParallelProjection(True)
-
-        self._iStyle.SetInteractionModeToImageSlicing()
-
-        self._iStyle.AddObserver("MouseWheelForwardEvent", self.onScroll)
-        self._iStyle.AddObserver("MouseWheelBackwardEvent", self.onScroll)
-        self._iStyle.AddObserver("MouseMoveEvent", self.onMouseMove)
-        self._iStyle.AddObserver("LeftButtonPressEvent", self.onLeftButtonPressed)
-        self._iStyle.AddObserver("LeftButtonReleaseEvent", self.onLeftButtonPressed)
-
-        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
-        self._renderWindow.AddRenderer(self._renderer)
-
-    def close(self):
-        if not (self._primaryImageLayer.image is None):
-            self._primaryImageLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
-            self._primaryImageLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
-
-        if not (self._secondaryImageLayer.image is None):
-            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
-
-        self._primaryImageLayer.close()
-        self._secondaryImageLayer.close()
-        self._textLayer.close()
-        self._contourLayer.close()
-        self._crossHairLayer.close()
-        self._rtPlanLayer.close()
-
-    @property
-    def rtPlan(self) -> RTPlan:
-        raise NotImplementedError
-
-    @rtPlan.setter
-    def rtPlan(self, plan:RTPlan):
-        if not self.primaryImage is None:
-            self._rtPlanLayer.setPlan(plan, self.primaryImage)
-
-    @property
-    def primaryImage(self) -> Image3D:
-        if self._primaryImageLayer.image is None:
-            return None
-        return self._primaryImageLayer.image.data
-
-    @primaryImage.setter
-    def primaryImage(self, image: Image3D):
-        imageAlreadyDisplayed = image==self._primaryImageLayer.image or (not (self._primaryImageLayer.image is None) and image==self._primaryImageLayer.image.data)
-        if imageAlreadyDisplayed:
-            return
-
-        if image is None:
-            self._resetPrimaryImageLayer()
-        else:
-            self._setPrimaryImageForViewer(Image3DForViewer(image))
-
-        self.primaryImageSignal.emit(self.primaryImage)
-
-    def _resetPrimaryImageLayer(self):
-        self._primaryImageLayer.image = None
-        self._mainLayout.removeWidget(self._vtkWidget)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-
-    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
-        # If I do not reset secondary image, the interactor sets its colormap to gray???!!!
-        secondaryImage = self._secondaryImageLayer.image
-        self._secondaryImageLayer.image = None
-
-        if not (self._primaryImageLayer.image is None):
-            self._primaryImageLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
-            self._primaryImageLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
-
-        self._primaryImageLayer.image = image
-        self._contourLayer.referenceImage = image
-        self._textLayer.setPrimaryTextLine(2, image.name)
-
-        self._handlePosition(self._primaryImageLayer.image.selectedPosition)
-
-        self._primaryImageLayer.image.selectedPositionChangedSignal.connect(self._handlePosition)
-        self._primaryImageLayer.image.nameChangedSignal.connect(self._setPrimaryName)
-
-        self._primaryImageLayer.resliceAxes = self._viewMatrix
-        self._contourLayer.resliceAxes = self._viewMatrix
-        self._rtPlanLayer.resliceAxes = self._viewMatrix
-
-        self._blackWidget.hide()
-        self._mainLayout.removeWidget(self._blackWidget)
-        self._mainLayout.addWidget(self._vtkWidget)
-        self._vtkWidget.show()
-
-        # Start interaction
-        self._renderWindow.GetInteractor().Start()
-
-        if self._wwlEnabled:
-            self._iStyle.StartWindowLevel()
-            self._iStyle.OnLeftButtonUp()
-
-        self._iStyle.SetCurrentImageNumber(0)
-
-        self._secondaryImageLayer.image = secondaryImage
-
-        self._renderer.ResetCamera()
-        self._renderWindow.Render()
-
-
-
-    def _setPrimaryName(self, name):
-        self._textLayer.setPrimaryTextLine(2, name)
-
-    @property
-    def profileWidgetEnabled(self) -> bool:
-        return self._profileWidget.enabled
-
-    @profileWidgetEnabled.setter
-    def profileWidgetEnabled(self, enabled: bool):
-        if enabled==self._profileWidget.enabled:
-            return
-
-        if enabled and not self._profileWidget.enabled:
-            self._profileWidgetNoInteractionYet = True
-            self._profileWidget.callback = self._viewController.profileWidgetCallback
-        else:
-            self._profileWidgetNoInteractionYet = False
-        self._profileWidget.enabled = enabled
-
-        self.profileWidgeEnabledSignal.emit(self.profileWidgetEnabled)
-
-    def setProfileWidgetEnabled(self, enabled):
-        self.profileWidgetEnabled = enabled
-
-    @property
-    def secondaryImage(self) -> typing.Optional[Image3D]:
-        if self._secondaryImageLayer.image is None:
-            return None
-        return self._secondaryImageLayer.image.data
-
-    @secondaryImage.setter
-    def secondaryImage(self, image: Image3D):
-        if self.primaryImage is None:
-            return
-
-        imageAlreadyDisplayed = image == self._secondaryImageLayer.image or (not (self._secondaryImageLayer.image is None) and image == self._secondaryImageLayer.image.data)
-        if imageAlreadyDisplayed:
-            return
-
-        if not (self._secondaryImageLayer.image is None):
-            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
-
-        self._secondaryImageLayer.image = Image3DForViewer(image)
-
-        if image is None:
-            self._secondaryImageLayer.image = None
-            self.secondaryImageSignal.emit(self.secondaryImage)
-            return
-
-        self._secondaryImageLayer.resliceAxes = self._viewMatrix
-
-        self._textLayer.setSecondaryTextLine(2, self.secondaryImage.name)
-
-        self._secondaryImageLayer.image.nameChangedSignal.connect(self._setSecondaryName)
-
-        self._renderWindow.Render()
-
-        self.secondaryImageSignal.emit(self.secondaryImage)
-
-    def _setSecondaryName(self, name):
-        self._textLayer.setSecondaryTextLine(2, name)
-
-    @property
-    def secondaryImageLayer(self):
-        return self._secondaryImageLayer
-
-
-    @property
-    def viewType(self):
-        return self._viewType
-
-    @viewType.setter
-    def viewType(self, viewType):
-        if self._viewType == viewType:
-            return
-
-        self._setViewType(viewType)
-
-    def _setViewType(self, viewType):
-        self._viewType = viewType
-        coronal = vtkCommonMath.vtkMatrix4x4()
-        coronal.DeepCopy((1, 0, 0, 0,
-                          0, 0, 1, 0,
-                          0, 1, 0, 0,
-                          0, 0, 0, 1))
-
-        sagittal = vtkCommonMath.vtkMatrix4x4()
-        sagittal.DeepCopy((0, 0, -1, 0,
-                          1, 0, 0, 0,
-                          0, 1, 0, 0,
-                          0, 0, 0, 1))
-
-        axial = vtkCommonMath.vtkMatrix4x4()
-        axial.DeepCopy((1, 0, 0, 0,
-                        0, -1, 0, 0,
-                        0, 0, -1, 0,
-                        0, 0, 0, 1))
-
-        if self._viewType == self.ViewerTypes.SAGITTAL:
-            self._viewMatrix = sagittal
-        if self._viewType == self.ViewerTypes.AXIAL:
-            self._viewMatrix = axial
-        if self._viewType == self.ViewerTypes.CORONAL:
-            self._viewMatrix = coronal
-        else:
-            ValueError('Invalid viewType')
-
-        if not self.primaryImage is None:
-            self._primaryImageLayer.resliceAxes = self._viewMatrix
-            self._contourLayer.resliceAxes = self._viewMatrix
-            self._rtPlanLayer.resliceAxes = self._viewMatrix
-        if not self.secondaryImage is None:
-            self._secondaryImageLayer.resliceAxes = self._viewMatrix
-
-        self._renderer.ResetCamera()
-        self._renderWindow.Render()
-
-        self.viewTypeChangedSignal.emit(self._viewType)
-
-    @property
-    def crossHairEnabled(self) -> bool:
-        return self._crossHairEnabled
-
-    @crossHairEnabled.setter
-    def crossHairEnabled(self, enabled: bool):
-        if enabled == self._crossHairEnabled:
-            return
-
-        self._crossHairEnabled = enabled
-        if self._crossHairEnabled:
-            self.wwlEnabled = False
-            self._crossHairLayer.visible = True
-        else:
-            self._crossHairLayer.visible = False
-            self._handlePosition(None)
-            self._renderWindow.Render()
-        self.crossHairEnabledSignal.emit(self._crossHairEnabled)
-
-    def setCrossHairEnabled(self, enabled: bool):
-        self.crossHairEnabled = enabled
-
-    @property
-    def wwlEnabled(self) -> bool:
-        return self._wwlEnabled
-
-    @wwlEnabled.setter
-    def wwlEnabled(self, enabled: bool):
-        if enabled == self._wwlEnabled:
-            return
-
-        self._wwlEnabled = enabled
-
-        if self._wwlEnabled:
-            self.crossHairEnabled = False
-        self.wwlEnabledSignal.emit(enabled)
-
-    def setWWLEnabled(self, enabled: bool):
-        self.wwlEnabled = enabled
-
-    def onLeftButtonPressed(self, obj=None, event='Press'):
-        if 'Press' in event:
-            self._leftButtonPress = True
-
-            if self.profileWidgetEnabled:
-                self._iStyle.OnLeftButtonDown()
-                return
-
-            if self._crossHairEnabled:
-                self.onMouseMove(None, None)
-            else:
-                self._iStyle.OnLeftButtonDown()
-        else:
-            self._leftButtonPress = False
-            self._iStyle.OnLeftButtonUp()
-
-    def onMouseMove(self, obj=None, event=None):
-        (mouseX, mouseY) = self._renderWindow.GetInteractor().GetEventPosition()
-
-        # MouseX and MouseY are not related to image but to renderWindow
-        dPos = vtkCoordinate()
-        dPos.SetCoordinateSystemToDisplay()
-        dPos.SetValue(mouseX, mouseY, 0)
-        worldPos = dPos.GetComputedWorldValue(self._renderer)
-
-        point = self._viewMatrix.MultiplyPoint((worldPos[0], worldPos[1], 0, 1))
-
-        if self.profileWidgetEnabled and self._profileWidgetNoInteractionYet and self._leftButtonPress:
-            self._profileWidget.setInitialPosition((worldPos[0], worldPos[1]))
-            self._profileWidgetNoInteractionYet = False
-            return
-
-        if self._crossHairEnabled and self._leftButtonPress:
-            self._primaryImageLayer.image.selectedPosition = (point[0], point[1], point[2])
-
-        if self._leftButtonPress and self._wwlEnabled:
-            self._iStyle.OnMouseMove()
-            self.__sendingWWL = True
-            imageProperty = self._iStyle.GetCurrentImageProperty()
-            self._primaryImageLayer.image.wwlValue = (imageProperty.GetColorWindow(), imageProperty.GetColorLevel())
-            self.__sendingWWL = False
-
-        if not self._leftButtonPress:
-            self._iStyle.OnMouseMove()
-
-    def onScroll(self, obj=None, event='Forward'):
-        sliceSpacing = self._primaryImageLayer._reslice.GetOutput().GetSpacing()[2]
-
-        deltaY = 0.
-        if 'Forward' in event:
-            deltaY = sliceSpacing
-        if 'Backward' in event:
-            deltaY = -sliceSpacing
-
-        point = (0., 0., 0., 0.)
-        if self._crossHairEnabled:
-            worldPos = Image3DForViewer(self.primaryImage).selectedPosition
-            if worldPos is None:
-                return
-
-            tform = vtkCommonMath.vtkMatrix4x4()
-            tform.DeepCopy(self._viewMatrix)
-            tform.Invert()
-            point = tform.MultiplyPoint((worldPos[0], worldPos[1], worldPos[2], 1))
-
-        # move the center point that we are slicing through
-        center = self._viewMatrix.MultiplyPoint((0, 0, deltaY, 1))
-        self._viewMatrix.SetElement(0, 3, center[0])
-        self._viewMatrix.SetElement(1, 3, center[1])
-        self._viewMatrix.SetElement(2, 3, center[2])
-
-        if self._crossHairEnabled:
-            point = self._viewMatrix.MultiplyPoint((point[0], point[1], point[2], 1))
-            Image3DForViewer(self.primaryImage).selectedPosition = point
-
-        self._renderWindow.Render()
-
-    def _handlePosition(self, position: typing.Sequence):
-        if not self._crossHairEnabled or position is None:
-            self._textLayer.setPrimaryTextLine(0, '')
-            self._textLayer.setPrimaryTextLine(1, '')
-
-            if not self.secondaryImage is None:
-                self._textLayer.setSecondaryTextLine(0, '')
-                self._textLayer.setSecondaryTextLine(1, '')
-            return
-
-        transfo_mat = vtkCommonMath.vtkMatrix4x4()
-        transfo_mat.DeepCopy(self._viewMatrix)
-        transfo_mat.Invert()
-        posAfterInverse = transfo_mat.MultiplyPoint((position[0], position[1], position[2], 1))
-
-        pos = self._viewMatrix.MultiplyPoint((0, 0, posAfterInverse[2], 1))
-
-        self._viewMatrix.SetElement(0, 3, pos[0])
-        self._viewMatrix.SetElement(1, 3, pos[1])
-        self._viewMatrix.SetElement(2, 3, pos[2])
-        if self._crossHairEnabled:
-            self._crossHairLayer.position = (posAfterInverse[0], posAfterInverse[1])
-
-        try:
-            data = self._primaryImageLayer.image.getDataAtPosition(position)
-
-            self._textLayer.setPrimaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
-            # self._textLayer.setPrimaryTextLine(0, 'ValueNumpy: ' + "{:.2f}".format(dataNumpy))
-            self._textLayer.setPrimaryTextLine(1,  'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
-                position[1]) + ' ' + "{:.2f}".format(position[2]))
-        except:
-            self._textLayer.setPrimaryTextLine(0, '')
-            self._textLayer.setPrimaryTextLine(1, '')
-
-        if not self.secondaryImage is None:
-            try:
-                data = self._secondaryImageLayer.image.getDataAtPosition(position)
-
-                self._textLayer.setSecondaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
-                self._textLayer.setSecondaryTextLine(1, 'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
-                    position[1]) + ' ' + "{:.2f}".format(position[2]))
-            except:
-                self._textLayer.setSecondaryTextLine(0, '')
-                self._textLayer.setSecondaryTextLine(1, '')
+import typing
+from enum import Enum
+
+from PyQt5.QtWidgets import *
+
+import vtkmodules.vtkRenderingCore as vtkRenderingCore
+import vtkmodules.vtkInteractionStyle as vtkInteractionStyle
+from vtkmodules import vtkCommonMath
+from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+from vtkmodules.vtkRenderingCore import vtkCoordinate
+
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.plan._rtPlan import RTPlan
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtPlanLayer import RTPlanLayer
+from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.crossHairLayer import CrossHairLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer import PrimaryImage3DLayer
+from opentps.gui.viewer.dataViewerComponents.profileWidget import ProfileWidget
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage3DLayer import SecondaryImage3DLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.textLayer import TextLayer
+
+
+class Image3DViewer(QWidget):
+    class ViewerTypes(Enum):
+        AXIAL = 'axial'
+        CORONAL = 'coronal'
+        SAGITTAL = 'sagittal'
+        DEFAULT = 'sagittal'
+
+    _viewerTypesList = iter(list(ViewerTypes))
+
+
+    def __init__(self, viewController):
+        QWidget.__init__(self)
+
+        self.crossHairEnabledSignal = Event(bool)
+        self.profileWidgeEnabledSignal = Event(bool)
+        self.wwlEnabledSignal = Event(bool)
+        self.wwlEnabledSignal = Event(bool)
+        self.viewTypeChangedSignal = Event(object)
+        self.primaryImageSignal = Event(object)
+        self.secondaryImageSignal = Event(object)
+
+        self._blackWidget = BlackEmptyPlot(self)
+        self._crossHairEnabled = False
+        self._iStyle = vtkInteractionStyle.vtkInteractorStyleImage()
+        self._leftButtonPress = False
+        self._mainLayout = QVBoxLayout()
+        self._profileWidgetNoInteractionYet = False # Used to know if initial position of profile widget must be set
+        self._renderer = vtkRenderingCore.vtkRenderer()
+        self.__sendingWWL = False
+        self._viewController = viewController
+        self._viewMatrix = vtkCommonMath.vtkMatrix4x4()
+        self._viewType = self.ViewerTypes.DEFAULT
+        self._vtkWidget = QVTKRenderWindowInteractor(self)
+        self._wwlEnabled = False
+
+        self._renderWindow = self._vtkWidget.GetRenderWindow()
+
+        self._crossHairLayer = CrossHairLayer(self._renderer, self._renderWindow)
+        self._primaryImageLayer = PrimaryImage3DLayer(self._renderer, self._renderWindow, self._iStyle)
+        self._secondaryImageLayer = SecondaryImage3DLayer(self._renderer, self._renderWindow, self._iStyle)
+        self._profileWidget = ProfileWidget(self._renderer, self._renderWindow)
+        self._textLayer = TextLayer(self._renderer, self._renderWindow)
+        self._contourLayer = ContourLayer(self._renderer, self._renderWindow)
+        self._rtPlanLayer = RTPlanLayer(self._renderer, self._renderWindow)
+
+        self._profileWidget.primaryLayer = self._primaryImageLayer
+        self._profileWidget.secondaryLayer = self._secondaryImageLayer
+        self._profileWidget.contourLayer = self._contourLayer
+
+        self._setViewType(self._viewType)
+        self._contourLayer.resliceAxes = self._viewMatrix
+        self._rtPlanLayer.resliceAxes = self._viewMatrix
+
+        self.setLayout(self._mainLayout)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+        self._mainLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._renderer.SetBackground(0, 0, 0)
+        self._renderer.GetActiveCamera().SetParallelProjection(True)
+
+        self._iStyle.SetInteractionModeToImageSlicing()
+
+        self._iStyle.AddObserver("MouseWheelForwardEvent", self.onScroll)
+        self._iStyle.AddObserver("MouseWheelBackwardEvent", self.onScroll)
+        self._iStyle.AddObserver("MouseMoveEvent", self.onMouseMove)
+        self._iStyle.AddObserver("LeftButtonPressEvent", self.onLeftButtonPressed)
+        self._iStyle.AddObserver("LeftButtonReleaseEvent", self.onLeftButtonPressed)
+
+        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
+        self._renderWindow.AddRenderer(self._renderer)
+
+        self._closed = False
+
+
+    def closeEvent(self, QCloseEvent):
+        if self._closed:
+            return
+
+        self._closed = True
+        self.reset()
+        self._renderWindow.Finalize()
+        self._vtkWidget.close()
+        del self._renderWindow, self._vtkWidget
+        super().closeEvent(QCloseEvent)
+
+    def reset(self):
+        if not (self._primaryImageLayer.image is None):
+            self._primaryImageLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
+            self._primaryImageLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
+
+        if not (self._secondaryImageLayer.image is None):
+            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
+
+        self._primaryImageLayer.close()
+        self._secondaryImageLayer.close()
+        self._textLayer.close()
+        self._contourLayer.close()
+        self._crossHairLayer.close()
+        self._rtPlanLayer.close()
+
+    @property
+    def rtPlan(self) -> RTPlan:
+        raise NotImplementedError
+
+    @rtPlan.setter
+    def rtPlan(self, plan:RTPlan):
+        if not self.primaryImage is None:
+            self._rtPlanLayer.setPlan(plan, self.primaryImage)
+
+    @property
+    def primaryImage(self) -> Image3D:
+        if self._primaryImageLayer.image is None:
+            return None
+        return self._primaryImageLayer.image.data
+
+    @primaryImage.setter
+    def primaryImage(self, image: Image3D):
+        imageAlreadyDisplayed = image==self._primaryImageLayer.image or (not (self._primaryImageLayer.image is None) and image==self._primaryImageLayer.image.data)
+        if imageAlreadyDisplayed:
+            return
+
+        if image is None:
+            self._resetPrimaryImageLayer()
+        else:
+            self._setPrimaryImageForViewer(Image3DForViewer(image))
+
+        self.primaryImageSignal.emit(self.primaryImage)
+
+    def _resetPrimaryImageLayer(self):
+        self._primaryImageLayer.image = None
+        self._mainLayout.removeWidget(self._vtkWidget)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+
+    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
+        # If I do not reset secondary image, the interactor sets its colormap to gray???!!!
+        secondaryImage = self._secondaryImageLayer.image
+        self._secondaryImageLayer.image = None
+
+        if not (self._primaryImageLayer.image is None):
+            self._primaryImageLayer.image.selectedPositionChangedSignal.disconnect(self._handlePosition)
+            self._primaryImageLayer.image.nameChangedSignal.disconnect(self._setPrimaryName)
+
+        self._primaryImageLayer.image = image
+        self._contourLayer.referenceImage = image
+        self._textLayer.setPrimaryTextLine(2, image.name)
+
+        self._handlePosition(self._primaryImageLayer.image.selectedPosition)
+
+        self._primaryImageLayer.image.selectedPositionChangedSignal.connect(self._handlePosition)
+        self._primaryImageLayer.image.nameChangedSignal.connect(self._setPrimaryName)
+
+        self._primaryImageLayer.resliceAxes = self._viewMatrix
+        self._contourLayer.resliceAxes = self._viewMatrix
+        self._rtPlanLayer.resliceAxes = self._viewMatrix
+
+        self._blackWidget.hide()
+        self._mainLayout.removeWidget(self._blackWidget)
+        self._mainLayout.addWidget(self._vtkWidget)
+        self._vtkWidget.show()
+
+        # Start interaction
+        self._renderWindow.GetInteractor().Start()
+
+        if self._wwlEnabled:
+            self._iStyle.StartWindowLevel()
+            self._iStyle.OnLeftButtonUp()
+
+        self._iStyle.SetCurrentImageNumber(0)
+
+        self._secondaryImageLayer.image = secondaryImage
+
+        self._renderer.ResetCamera()
+        self._renderWindow.Render()
+
+
+
+    def _setPrimaryName(self, name):
+        self._textLayer.setPrimaryTextLine(2, name)
+
+    @property
+    def profileWidgetEnabled(self) -> bool:
+        return self._profileWidget.enabled
+
+    @profileWidgetEnabled.setter
+    def profileWidgetEnabled(self, enabled: bool):
+        if enabled==self._profileWidget.enabled:
+            return
+
+        if enabled and not self._profileWidget.enabled:
+            self._profileWidgetNoInteractionYet = True
+            self._profileWidget.callback = self._viewController.profileWidgetCallback
+        else:
+            self._profileWidgetNoInteractionYet = False
+        self._profileWidget.enabled = enabled
+
+        self.profileWidgeEnabledSignal.emit(self.profileWidgetEnabled)
+
+    def setProfileWidgetEnabled(self, enabled):
+        self.profileWidgetEnabled = enabled
+
+    @property
+    def secondaryImage(self) -> typing.Optional[Image3D]:
+        if self._secondaryImageLayer.image is None:
+            return None
+        return self._secondaryImageLayer.image.data
+
+    @secondaryImage.setter
+    def secondaryImage(self, image: Image3D):
+        if self.primaryImage is None:
+            return
+
+        imageAlreadyDisplayed = image == self._secondaryImageLayer.image or (not (self._secondaryImageLayer.image is None) and image == self._secondaryImageLayer.image.data)
+        if imageAlreadyDisplayed:
+            return
+
+        if not (self._secondaryImageLayer.image is None):
+            self._secondaryImageLayer.image.nameChangedSignal.disconnect(self._setSecondaryName)
+
+        self._secondaryImageLayer.image = Image3DForViewer(image)
+
+        if image is None:
+            self._secondaryImageLayer.image = None
+            self.secondaryImageSignal.emit(self.secondaryImage)
+            return
+
+        self._secondaryImageLayer.resliceAxes = self._viewMatrix
+
+        self._textLayer.setSecondaryTextLine(2, self.secondaryImage.name)
+
+        self._secondaryImageLayer.image.nameChangedSignal.connect(self._setSecondaryName)
+
+        self._renderWindow.Render()
+
+        self.secondaryImageSignal.emit(self.secondaryImage)
+
+    def _setSecondaryName(self, name):
+        self._textLayer.setSecondaryTextLine(2, name)
+
+    @property
+    def secondaryImageLayer(self):
+        return self._secondaryImageLayer
+
+
+    @property
+    def viewType(self):
+        return self._viewType
+
+    @viewType.setter
+    def viewType(self, viewType):
+        if self._viewType == viewType:
+            return
+
+        self._setViewType(viewType)
+
+    def _setViewType(self, viewType):
+        self._viewType = viewType
+        coronal = vtkCommonMath.vtkMatrix4x4()
+        coronal.DeepCopy((1, 0, 0, 0,
+                          0, 0, 1, 0,
+                          0, 1, 0, 0,
+                          0, 0, 0, 1))
+
+        sagittal = vtkCommonMath.vtkMatrix4x4()
+        sagittal.DeepCopy((0, 0, -1, 0,
+                          1, 0, 0, 0,
+                          0, 1, 0, 0,
+                          0, 0, 0, 1))
+
+        axial = vtkCommonMath.vtkMatrix4x4()
+        axial.DeepCopy((1, 0, 0, 0,
+                        0, -1, 0, 0,
+                        0, 0, -1, 0,
+                        0, 0, 0, 1))
+
+        if self._viewType == self.ViewerTypes.SAGITTAL:
+            self._viewMatrix = sagittal
+        if self._viewType == self.ViewerTypes.AXIAL:
+            self._viewMatrix = axial
+        if self._viewType == self.ViewerTypes.CORONAL:
+            self._viewMatrix = coronal
+        else:
+            ValueError('Invalid viewType')
+
+        if not self.primaryImage is None:
+            self._primaryImageLayer.resliceAxes = self._viewMatrix
+            self._contourLayer.resliceAxes = self._viewMatrix
+            self._rtPlanLayer.resliceAxes = self._viewMatrix
+        if not self.secondaryImage is None:
+            self._secondaryImageLayer.resliceAxes = self._viewMatrix
+
+        self._renderer.ResetCamera()
+        self._renderWindow.Render()
+
+        self.viewTypeChangedSignal.emit(self._viewType)
+
+    @property
+    def crossHairEnabled(self) -> bool:
+        return self._crossHairEnabled
+
+    @crossHairEnabled.setter
+    def crossHairEnabled(self, enabled: bool):
+        if enabled == self._crossHairEnabled:
+            return
+
+        self._crossHairEnabled = enabled
+        if self._crossHairEnabled:
+            self.wwlEnabled = False
+            self._crossHairLayer.visible = True
+        else:
+            self._crossHairLayer.visible = False
+            self._handlePosition(None)
+            self._renderWindow.Render()
+        self.crossHairEnabledSignal.emit(self._crossHairEnabled)
+
+    def setCrossHairEnabled(self, enabled: bool):
+        self.crossHairEnabled = enabled
+
+    @property
+    def wwlEnabled(self) -> bool:
+        return self._wwlEnabled
+
+    @wwlEnabled.setter
+    def wwlEnabled(self, enabled: bool):
+        if enabled == self._wwlEnabled:
+            return
+
+        self._wwlEnabled = enabled
+
+        if self._wwlEnabled:
+            self.crossHairEnabled = False
+        self.wwlEnabledSignal.emit(enabled)
+
+    def setWWLEnabled(self, enabled: bool):
+        self.wwlEnabled = enabled
+
+    def onLeftButtonPressed(self, obj=None, event='Press'):
+        if 'Press' in event:
+            self._leftButtonPress = True
+
+            if self.profileWidgetEnabled:
+                self._iStyle.OnLeftButtonDown()
+                return
+
+            if self._crossHairEnabled:
+                self.onMouseMove(None, None)
+            else:
+                self._iStyle.OnLeftButtonDown()
+        else:
+            self._leftButtonPress = False
+            self._iStyle.OnLeftButtonUp()
+
+    def onMouseMove(self, obj=None, event=None):
+        (mouseX, mouseY) = self._renderWindow.GetInteractor().GetEventPosition()
+
+        # MouseX and MouseY are not related to image but to renderWindow
+        dPos = vtkCoordinate()
+        dPos.SetCoordinateSystemToDisplay()
+        dPos.SetValue(mouseX, mouseY, 0)
+        worldPos = dPos.GetComputedWorldValue(self._renderer)
+
+        point = self._viewMatrix.MultiplyPoint((worldPos[0], worldPos[1], 0, 1))
+
+        if self.profileWidgetEnabled and self._profileWidgetNoInteractionYet and self._leftButtonPress:
+            self._profileWidget.setInitialPosition((worldPos[0], worldPos[1]))
+            self._profileWidgetNoInteractionYet = False
+            return
+
+        if self._crossHairEnabled and self._leftButtonPress:
+            self._primaryImageLayer.image.selectedPosition = (point[0], point[1], point[2])
+
+        if self._leftButtonPress and self._wwlEnabled:
+            self._iStyle.OnMouseMove()
+            self.__sendingWWL = True
+            imageProperty = self._iStyle.GetCurrentImageProperty()
+            self._primaryImageLayer.image.wwlValue = (imageProperty.GetColorWindow(), imageProperty.GetColorLevel())
+            self.__sendingWWL = False
+
+        if not self._leftButtonPress:
+            self._iStyle.OnMouseMove()
+
+    def onScroll(self, obj=None, event='Forward'):
+        sliceSpacing = self._primaryImageLayer._reslice.GetOutput().GetSpacing()[2]
+
+        deltaY = 0.
+        if 'Forward' in event:
+            deltaY = sliceSpacing
+        if 'Backward' in event:
+            deltaY = -sliceSpacing
+
+        point = (0., 0., 0., 0.)
+        if self._crossHairEnabled:
+            worldPos = Image3DForViewer(self.primaryImage).selectedPosition
+            if worldPos is None:
+                return
+
+            tform = vtkCommonMath.vtkMatrix4x4()
+            tform.DeepCopy(self._viewMatrix)
+            tform.Invert()
+            point = tform.MultiplyPoint((worldPos[0], worldPos[1], worldPos[2], 1))
+
+        # move the center point that we are slicing through
+        center = self._viewMatrix.MultiplyPoint((0, 0, deltaY, 1))
+        self._viewMatrix.SetElement(0, 3, center[0])
+        self._viewMatrix.SetElement(1, 3, center[1])
+        self._viewMatrix.SetElement(2, 3, center[2])
+
+        if self._crossHairEnabled:
+            point = self._viewMatrix.MultiplyPoint((point[0], point[1], point[2], 1))
+            Image3DForViewer(self.primaryImage).selectedPosition = point
+
+        self._renderWindow.Render()
+
+    def _handlePosition(self, position: typing.Sequence):
+        if not self._crossHairEnabled or position is None:
+            self._textLayer.setPrimaryTextLine(0, '')
+            self._textLayer.setPrimaryTextLine(1, '')
+
+            if not self.secondaryImage is None:
+                self._textLayer.setSecondaryTextLine(0, '')
+                self._textLayer.setSecondaryTextLine(1, '')
+            return
+
+        transfo_mat = vtkCommonMath.vtkMatrix4x4()
+        transfo_mat.DeepCopy(self._viewMatrix)
+        transfo_mat.Invert()
+        posAfterInverse = transfo_mat.MultiplyPoint((position[0], position[1], position[2], 1))
+
+        pos = self._viewMatrix.MultiplyPoint((0, 0, posAfterInverse[2], 1))
+
+        self._viewMatrix.SetElement(0, 3, pos[0])
+        self._viewMatrix.SetElement(1, 3, pos[1])
+        self._viewMatrix.SetElement(2, 3, pos[2])
+        if self._crossHairEnabled:
+            self._crossHairLayer.position = (posAfterInverse[0], posAfterInverse[1])
+
+        try:
+            data = self._primaryImageLayer.image.getDataAtPosition(position)
+
+            self._textLayer.setPrimaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
+            # self._textLayer.setPrimaryTextLine(0, 'ValueNumpy: ' + "{:.2f}".format(dataNumpy))
+            self._textLayer.setPrimaryTextLine(1,  'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
+                position[1]) + ' ' + "{:.2f}".format(position[2]))
+        except:
+            self._textLayer.setPrimaryTextLine(0, '')
+            self._textLayer.setPrimaryTextLine(1, '')
+
+        if not self.secondaryImage is None:
+            try:
+                data = self._secondaryImageLayer.image.getDataAtPosition(position)
+
+                self._textLayer.setSecondaryTextLine(0, 'Value: ' + "{:.2f}".format(data))
+                self._textLayer.setSecondaryTextLine(1, 'Pos: ' + "{:.2f}".format(position[0]) + ' ' + "{:.2f}".format(
+                    position[1]) + ' ' + "{:.2f}".format(position[2]))
+            except:
+                self._textLayer.setSecondaryTextLine(0, '')
+                self._textLayer.setSecondaryTextLine(1, '')
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/image3DViewer_3D.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/image3DViewer_3D.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,162 @@
-from typing import Optional
-
-from PyQt5.QtWidgets import *
-
-import vtkmodules.vtkRenderingCore as vtkRenderingCore
-from vtkmodules import vtkInteractionStyle
-from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
-
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.plan import RTPlan
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer_3D import PrimaryImage3DLayer_3D
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtplanLayer_3D import RTPlanLayer_3D
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage3DLayer_3D import SecondaryImage3DLayer_3D
-from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
-
-
-class Image3DViewer_3D(QWidget):
-    def __init__(self, viewController, parent=None):
-        QWidget.__init__(self, parent=parent)
-
-        self.primaryImageSignal = Event(object)
-        self.secondaryImageSignal = Event(object)
-
-        self._blackWidget = BlackEmptyPlot(self)
-        self._renderer = vtkRenderingCore.vtkRenderer()
-        self._viewController = viewController
-        self._vtkWidget = QVTKRenderWindowInteractor(self)
-        self._mainLayout = QVBoxLayout()
-        self._renderWindow = self._vtkWidget.GetRenderWindow()
-
-        self._iStyle = vtkInteractionStyle.vtkInteractorStyleTrackballCamera()
-
-        self._primaryImageLayer = PrimaryImage3DLayer_3D(self._renderer, self._renderWindow, self._iStyle)
-        self._secondaryImageLayer = SecondaryImage3DLayer_3D(self._renderer, self._renderWindow, self._iStyle)
-        self._rtPlanLayer = RTPlanLayer_3D(self._renderer, self._renderWindow)
-
-
-        self.setLayout(self._mainLayout)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-        self._mainLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._renderer.SetBackground(0, 0, 0)
-        self._renderer.GetActiveCamera().SetParallelProjection(True)
-
-        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
-        self._renderWindow.AddRenderer(self._renderer)
-
-    def close(self):
-        self._rtPlanLayer.close()
-        self._primaryImageLayer.close()
-        self._secondaryImageLayer.close()
-
-    def show(self):
-        super(Image3DViewer_3D, self).show()
-        self.update()
-
-    def update(self):
-        self._primaryImageLayer.update()
-        self._secondaryImageLayer.update()
-        self._rtPlanLayer.update()
-
-
-    @property
-    def primaryImage(self) -> Optional[Image3D]:
-        if self._primaryImageLayer.image is None:
-            return None
-        return self._primaryImageLayer.image.data
-
-    @primaryImage.setter
-    def primaryImage(self, image: Image3D):
-        self._setPrimaryImageForViewer(Image3DForViewer(image))
-        if self.isVisible():
-            self.update()
-
-        self.primaryImageSignal.emit(self.primaryImage)
-
-    def _resetPrimaryImageLayer(self):
-        self._primaryImageLayer.image = None
-        self._mainLayout.removeWidget(self._vtkWidget)
-        self._vtkWidget.hide()
-        self._mainLayout.addWidget(self._blackWidget)
-        self._blackWidget.show()
-
-    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
-        self._primaryImageLayer.image = image
-
-        self._blackWidget.hide()
-        self._mainLayout.removeWidget(self._blackWidget)
-        self._mainLayout.addWidget(self._vtkWidget)
-        self._vtkWidget.show()
-
-    @property
-    def secondaryImage(self) -> Optional[Image3D]:
-        if self._secondaryImageLayer.image is None:
-            return None
-        return self._secondaryImageLayer.image.data
-
-    @secondaryImage.setter
-    def secondaryImage(self, image: Image3D):
-        if self.primaryImage is None:
-            return
-
-        if image is None:
-            self._secondaryImageLayer.image = None
-            if self.isVisible():
-                self.update()
-
-            self.secondaryImageSignal.emit(self.secondaryImage)
-            return
-        else:
-            self._secondaryImageLayer.image = Image3DForViewer(image)
-
-        if self.isVisible():
-            self.update()
-
-        self._renderWindow.Render()
-
-        self.secondaryImageSignal.emit(self.secondaryImage)
-
-    @property
-    def rtPlan(self) -> RTPlan:
-        raise NotImplementedError
-
-    @rtPlan.setter
-    def rtPlan(self, plan: RTPlan):
-        self._rtPlanLayer.setPlan(plan)
-
-        if self.isVisible():
-            self.update()
+from typing import Optional, Union
+
+from PyQt5.QtWidgets import *
+
+import vtkmodules.vtkRenderingCore as vtkRenderingCore
+from vtkmodules import vtkInteractionStyle
+from vtkmodules.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
+
+from opentps.core.data import ROIContour
+from opentps.core.data.images import ROIMask
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.plan import RTPlan
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer_3D import ContourLayer_3D
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer_3D import PrimaryImage3DLayer_3D
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.rtplanLayer_3D import RTPlanLayer_3D
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.secondaryImage3DLayer_3D import SecondaryImage3DLayer_3D
+from opentps.gui.viewer.dataViewerComponents.blackEmptyPlot import BlackEmptyPlot
+
+
+class Image3DViewer_3D(QWidget):
+    def __init__(self, viewController, parent=None):
+        QWidget.__init__(self, parent=parent)
+
+        self.primaryImageSignal = Event(object)
+        self.secondaryImageSignal = Event(object)
+
+        self._blackWidget = BlackEmptyPlot(self)
+        self._renderer = vtkRenderingCore.vtkRenderer()
+        self._viewController = viewController
+        self._vtkWidget = QVTKRenderWindowInteractor(self)
+        self._mainLayout = QVBoxLayout()
+        self._renderWindow = self._vtkWidget.GetRenderWindow()
+
+        self._iStyle = vtkInteractionStyle.vtkInteractorStyleTrackballCamera()
+
+        self._primaryImageLayer = PrimaryImage3DLayer_3D(self._renderer, self._renderWindow, self._iStyle)
+        self._secondaryImageLayer = SecondaryImage3DLayer_3D(self._renderer, self._renderWindow, self._iStyle)
+        self._contourLayer = ContourLayer_3D(self._renderer, self._renderWindow, self._iStyle)
+        self._rtPlanLayer = RTPlanLayer_3D(self._renderer, self._renderWindow)
+
+
+        self.setLayout(self._mainLayout)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+        self._mainLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._renderer.SetBackground(0, 0, 0)
+        self._renderer.GetActiveCamera().SetParallelProjection(True)
+
+        self._renderWindow.GetInteractor().SetInteractorStyle(self._iStyle)
+        self._renderWindow.AddRenderer(self._renderer)
+
+        self._closed = False
+
+    def closeEvent(self, QCloseEvent):
+        if self._closed:
+            return
+
+        self._closed = True
+        self.reset()
+        self._renderWindow.Finalize()
+        self._vtkWidget.close()
+        del self._renderWindow, self._vtkWidget
+        super().closeEvent(QCloseEvent)
+
+    def reset(self):
+        self._rtPlanLayer.close()
+        self._contourLayer.close()
+        self._primaryImageLayer.close()
+        self._secondaryImageLayer.close()
+
+    def show(self):
+        super(Image3DViewer_3D, self).show()
+        self.update()
+        self._primaryImageLayer.update()
+        self._secondaryImageLayer.update()
+        self._rtPlanLayer.update()
+        self._contourLayer.update()
+
+    def update(self):
+        self._primaryImageLayer.update()
+        self._secondaryImageLayer.update()
+        self._rtPlanLayer.update()
+
+
+    @property
+    def primaryImage(self) -> Optional[Image3D]:
+        if self._primaryImageLayer.image is None:
+            return None
+        return self._primaryImageLayer.image.data
+
+    @primaryImage.setter
+    def primaryImage(self, image: Image3D):
+        self._setPrimaryImageForViewer(Image3DForViewer(image))
+        if self.isVisible():
+            self.update()
+
+        self.primaryImageSignal.emit(self.primaryImage)
+
+    def _resetPrimaryImageLayer(self):
+        self._primaryImageLayer.image = None
+        self._mainLayout.removeWidget(self._vtkWidget)
+        self._vtkWidget.hide()
+        self._mainLayout.addWidget(self._blackWidget)
+        self._blackWidget.show()
+
+    def _setPrimaryImageForViewer(self, image:GenericImageForViewer):
+        self._primaryImageLayer.image = image
+
+        self._blackWidget.hide()
+        self._mainLayout.removeWidget(self._blackWidget)
+        self._mainLayout.addWidget(self._vtkWidget)
+        self._vtkWidget.show()
+
+    @property
+    def secondaryImage(self) -> Optional[Image3D]:
+        if self._secondaryImageLayer.image is None:
+            return None
+        return self._secondaryImageLayer.image.data
+
+    @secondaryImage.setter
+    def secondaryImage(self, image: Image3D):
+        if self.primaryImage is None:
+            return
+
+        if image is None:
+            self._secondaryImageLayer.image = None
+            if self.isVisible():
+                self.update()
+
+            self.secondaryImageSignal.emit(self.secondaryImage)
+            return
+        else:
+            self._secondaryImageLayer.image = Image3DForViewer(image)
+
+        if self.isVisible():
+            self.update()
+
+        self._renderWindow.Render()
+
+        self.secondaryImageSignal.emit(self.secondaryImage)
+
+    @property
+    def rtPlan(self) -> RTPlan:
+        raise NotImplementedError
+
+    @rtPlan.setter
+    def rtPlan(self, plan: RTPlan):
+        self._rtPlanLayer.setPlan(plan)
+
+        if self.isVisible():
+            self.update()
+
+    def setNewContour(self, contour:Union[ROIContour, ROIMask]):
+        self._contourLayer.setNewContour(contour)
+
+        if self.isVisible():
+            self._contourLayer.update()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageFusionPropEditor.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageFusionPropEditor.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from PyQt5.QtWidgets import QMainWindow, QGroupBox, QHBoxLayout, QWidget, QVBoxLayout, QLabel, QLineEdit
-from matplotlib import pyplot as plt
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
-from matplotlib.widgets import RangeSlider
-
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-from opentps.gui.viewer.dataViewerComponents.patientDataPropertyEditor import PatientDataPropertyEditor
-
-
-class ImageFusionPropEditor(QMainWindow):
-    def __init__(self, image, parent=None):
-        super().__init__(parent)
-
-        self.setWindowTitle('Secondary image')
-        self.resize(800, 600)
-
-        centralWidget = QWidget()
-        self.setCentralWidget(centralWidget)
-        self._layout = QHBoxLayout()
-        centralWidget.setLayout(self._layout)
-
-        self._imageInfoGroup = QGroupBox(title='Image info')
-        self._layout.addWidget(self._imageInfoGroup)
-        vbox = QVBoxLayout()
-        self._imageInfoGroup.setLayout(vbox)
-        vbox.addWidget(PatientDataPropertyEditor(image, parent=self))
-
-        self._imageProperties = QGroupBox(title='Image properties')
-        self._layout.addWidget(self._imageProperties)
-        vbox = QVBoxLayout()
-        self._imageProperties.setLayout(vbox)
-
-
-        image = Image3DForViewer(image)
-
-        self._figure = plt.figure()
-
-        axs = plt.axes([0.20, 0.3, 0.60, 0.6])
-        n, bins, patches = axs.hist(image.imageArray.flatten(), bins=200)
-        axs.set_title('Histogram of pixel intensities')
-        axs.set_yscale('log')
-
-        # Create the RangeSlider
-        self._slider_ax = plt.axes([0.20, 0.1, 0.60, 0.03])
-        self.slider = RangeSlider(self._slider_ax, "Range", bins[0], bins[-1], valinit=image.range, dragging=True)
-
-        self.cm = plt.cm.get_cmap(image.lookupTableName)
-
-        bin_centers = 0.5 * (bins[:-1] + bins[1:])
-        col = (bin_centers - image.range[0]) / (image.range[1] - image.range[0])
-        for c, p in zip(col, patches):
-            plt.setp(p, 'facecolor', self.cm(c))
-
-        self.bin_centers = bin_centers
-        self._image = image
-        self.patches = patches
-        self.slider.on_changed(self._update)
-
-        self._canvas = FigureCanvasQTAgg(self._figure)
-        vbox.addWidget(self._canvas)
-
-        self._rangeEditor = RangeEditor(image)
-        vbox.addWidget(self._rangeEditor)
-
-        self._image.rangeChangedSignal.connect(self._updateSliderRange)
-
-    def _updateSliderRange(self, range):
-        self.slider.set_val(range)
-
-    def _update(self, val):
-        self._image.range = val
-        col = (self.bin_centers - val[0]) / (val[1] - val[0])
-        for c, p in zip(col, self.patches):
-            plt.setp(p, 'facecolor', self.cm(c))
-
-class RangeEditor(QWidget):
-    def __init__(self, image, parent=None):
-        super().__init__(parent)
-
-        self._image = image
-
-        self._mainLayout = QHBoxLayout(self)
-        self.setLayout(self._mainLayout)
-
-        self._txt = QLabel(self)
-        self._txt.setText('Range: ')
-
-        self._rangeEdit0 = QLineEdit(self)
-        self._rangeEdit1 = QLineEdit(self)
-
-        self._mainLayout.addWidget(self._txt)
-        self._mainLayout.addWidget(self._rangeEdit0)
-        self._mainLayout.addWidget(self._rangeEdit1)
-
-        self._rangeEdit0.setText(str(self._image.range[0]))
-        self._rangeEdit1.setText(str(self._image.range[1]))
-
-        self._rangeEdit0.textEdited.connect(self._handleTextEdited)
-        self._rangeEdit1.textEdited.connect(self._handleTextEdited)
-        self._image.rangeChangedSignal.connect(self.setRangeValue)
-
-    def setRangeValue(self, range):
-        if float(self._rangeEdit0.text()) != range[0]:
-            self._rangeEdit0.setText(str(range[0]))
-        if float(self._rangeEdit1.text()) != range[1]:
-            self._rangeEdit1.setText(str(range[1]))
-
-    def _handleTextEdited(self, *args):
+from PyQt5.QtWidgets import QMainWindow, QGroupBox, QHBoxLayout, QWidget, QVBoxLayout, QLabel, QLineEdit
+from matplotlib import pyplot as plt
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
+from matplotlib.widgets import RangeSlider
+
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.patientDataPropertyEditor import PatientDataPropertyEditor
+
+
+class ImageFusionPropEditor(QMainWindow):
+    def __init__(self, image, parent=None):
+        super().__init__(parent)
+
+        self.setWindowTitle('Secondary image')
+        self.resize(800, 600)
+
+        centralWidget = QWidget()
+        self.setCentralWidget(centralWidget)
+        self._layout = QHBoxLayout()
+        centralWidget.setLayout(self._layout)
+
+        self._imageInfoGroup = QGroupBox(title='Image info')
+        self._layout.addWidget(self._imageInfoGroup)
+        vbox = QVBoxLayout()
+        self._imageInfoGroup.setLayout(vbox)
+        vbox.addWidget(PatientDataPropertyEditor(image, parent=self))
+
+        self._imageProperties = QGroupBox(title='Image properties')
+        self._layout.addWidget(self._imageProperties)
+        vbox = QVBoxLayout()
+        self._imageProperties.setLayout(vbox)
+
+
+        image = Image3DForViewer(image)
+
+        self._figure = plt.figure()
+
+        axs = plt.axes([0.20, 0.3, 0.60, 0.6])
+        n, bins, patches = axs.hist(image.imageArray.flatten(), bins=200)
+        axs.set_title('Histogram of pixel intensities')
+        axs.set_yscale('log')
+
+        # Create the RangeSlider
+        self._slider_ax = plt.axes([0.20, 0.1, 0.60, 0.03])
+        self.slider = RangeSlider(self._slider_ax, "Range", bins[0], bins[-1], valinit=image.range, dragging=True)
+
+        self.cm = plt.cm.get_cmap(image.lookupTableName)
+
+        bin_centers = 0.5 * (bins[:-1] + bins[1:])
+        col = (bin_centers - image.range[0]) / (image.range[1] - image.range[0])
+        for c, p in zip(col, patches):
+            plt.setp(p, 'facecolor', self.cm(c))
+
+        self.bin_centers = bin_centers
+        self._image = image
+        self.patches = patches
+        self.slider.on_changed(self._update)
+
+        self._canvas = FigureCanvasQTAgg(self._figure)
+        vbox.addWidget(self._canvas)
+
+        self._rangeEditor = RangeEditor(image)
+        vbox.addWidget(self._rangeEditor)
+
+        self._image.rangeChangedSignal.connect(self._updateSliderRange)
+
+    def _updateSliderRange(self, range):
+        self.slider.set_val(range)
+
+    def _update(self, val):
+        self._image.range = val
+        col = (self.bin_centers - val[0]) / (val[1] - val[0])
+        for c, p in zip(col, self.patches):
+            plt.setp(p, 'facecolor', self.cm(c))
+
+class RangeEditor(QWidget):
+    def __init__(self, image, parent=None):
+        super().__init__(parent)
+
+        self._image = image
+
+        self._mainLayout = QHBoxLayout(self)
+        self.setLayout(self._mainLayout)
+
+        self._txt = QLabel(self)
+        self._txt.setText('Range: ')
+
+        self._rangeEdit0 = QLineEdit(self)
+        self._rangeEdit1 = QLineEdit(self)
+
+        self._mainLayout.addWidget(self._txt)
+        self._mainLayout.addWidget(self._rangeEdit0)
+        self._mainLayout.addWidget(self._rangeEdit1)
+
+        self._rangeEdit0.setText(str(self._image.range[0]))
+        self._rangeEdit1.setText(str(self._image.range[1]))
+
+        self._rangeEdit0.textEdited.connect(self._handleTextEdited)
+        self._rangeEdit1.textEdited.connect(self._handleTextEdited)
+        self._image.rangeChangedSignal.connect(self.setRangeValue)
+
+    def setRangeValue(self, range):
+        if float(self._rangeEdit0.text()) != range[0]:
+            self._rangeEdit0.setText(str(range[0]))
+        if float(self._rangeEdit1.text()) != range[1]:
+            self._rangeEdit1.setText(str(range[1]))
+
+    def _handleTextEdited(self, *args):
         self._image.range = (float(self._rangeEdit0.text()), float(self._rangeEdit1.text()))
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerActions.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerActions.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-import functools
-from typing import Sequence
-
-import matplotlib
-from PyQt5.QtWidgets import QComboBox, QWidgetAction, QMenu, QAction
-
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
-from opentps.gui.viewer.dataViewerComponents.doseComparisonImageProvider import DoseComparisonImageProvider
-from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
-from opentps.gui.viewer.dataViewerComponents.imageFusionPropEditor import ImageFusionPropEditor
-
-
-class ImageViewerActions:
-    def __init__(self, imageViewer:Image3DViewer):
-        self._imageViewer = imageViewer
-
-        self._viewTypeToStr = {self._imageViewer.ViewerTypes.AXIAL: 'Axial',
-                               self._imageViewer.ViewerTypes.CORONAL: 'Coronal',
-                               self._imageViewer.ViewerTypes.SAGITTAL: 'Sagittal'}
-        self._strToViewType = {v: k for k, v in self._viewTypeToStr.items()}
-
-        self._separator = None
-
-        self._viewTypeCombo = QComboBox()
-        self._viewTypeCombo.setFixedSize(80, 16)
-        self._viewTypeCombo.addItems(list(self._viewTypeToStr.values()))
-
-        self._viewTypeAction = QWidgetAction(None)
-        self._viewTypeAction.setDefaultWidget(self._viewTypeCombo)
-
-        self._primaryImageMenu = PrimaryImageMenu(self._imageViewer)
-        self._secondaryImageMenu = SecondaryImageMenu(self._imageViewer)
-        self._doseComparisonMenu = DoseComparisonMenu(self._imageViewer)
-        self._rtPlanMenu = RTPlanMenu(self._imageViewer)
-
-        self.hide()
-
-        self._viewTypeCombo.setCurrentIndex(self._viewTypeToIndex(self._imageViewer.viewType))
-        self._viewTypeCombo.currentIndexChanged.connect(self._handleViewTypeSelection)
-        self._imageViewer.viewTypeChangedSignal.connect(self._handleExternalViewTypeChange)
-
-    @property
-    def doseComparisonDataViewer(self):
-        return self._doseComparisonMenu.dataViewer
-
-    @doseComparisonDataViewer.setter
-    def doseComparisonDataViewer(self, dataViewer):
-        self._doseComparisonMenu.dataViewer = dataViewer
-
-
-    def _viewTypeToIndex(self, viewType):
-        return list(self._viewTypeToStr.keys()).index(viewType)
-
-    def setImageViewer(self, imageViewer):
-        self._imageViewer = imageViewer
-
-    def addToToolbar(self, toolbar:DataViewerToolbar):
-        self._separator = toolbar.addSeparator()
-        toolbar.addAction(self._viewTypeAction)
-        toolbar.toolsMenu.addMenu(self._primaryImageMenu)
-        toolbar.toolsMenu.addMenu(self._secondaryImageMenu)
-        toolbar.toolsMenu.addMenu(self._doseComparisonMenu)
-        toolbar.toolsMenu.addMenu(self._rtPlanMenu)
-
-    def hide(self):
-        if not self._separator is None:
-            self._separator.setVisible(False)
-        self._viewTypeAction.setVisible(False)
-
-    def show(self):
-        self._separator.setVisible(True)
-        self._viewTypeAction.setVisible(True)
-
-    def _handleViewTypeSelection(self, selectionIndex):
-        selectionText = self._viewTypeCombo.itemText(selectionIndex)
-        self._imageViewer.viewType = self._strToViewType[selectionText]
-
-    def _handleExternalViewTypeChange(self, viewType):
-        self._viewTypeCombo.setCurrentIndex(self._viewTypeToIndex(viewType))
-
-
-class PrimaryImageMenu(QMenu):
-    def __init__(self, imageViewer:Image3DViewer):
-        super().__init__("Primary image")
-
-        self._imageViewer = imageViewer
-
-        self._wwlMenu = QMenu("Window level/width", self)
-        self.addMenu(self._wwlMenu)
-
-        self._presetMenu = QMenu("Presets", self)
-        self._wwlMenu.addMenu(self._presetMenu)
-
-        self._wwlActions = []
-        for ps in presets():
-            wwlAction = QAction(ps.name + ' ' + str((ps.wwl[1], ps.wwl[0])), self)
-            wwlAction.triggered.connect(functools.partial(self._setPreset, ps))
-
-            self._wwlActions.append(wwlAction)
-
-            self._presetMenu.addAction(wwlAction)
-
-    def _setPreset(self, ps):
-        Image3DForViewer(self._imageViewer.primaryImage).wwlValue = ps.wwl
-
-class SecondaryImageMenu(QMenu):
-    def __init__(self, imageViewer:Image3DViewer):
-        super().__init__("Secondary image")
-
-        self._imageViewer = imageViewer
-        self._secondaryImageLayer = self._imageViewer.secondaryImageLayer
-
-        self._resetAction = QAction("Reset", self)
-        self._resetAction.triggered.connect(self._resetImage)
-        self.addAction(self._resetAction)
-
-        self._colorMapMenu = QMenu("Colormap", self)
-        self.addMenu(self._colorMapMenu)
-
-        self._colormapActions = []
-        cms = matplotlib.pyplot.colormaps()
-
-        for cm in cms:
-            cmAction = QAction(cm, self._colorMapMenu)
-            cmAction.triggered.connect(functools.partial(self.setFusion, cm))
-            self._colorMapMenu.addAction(cmAction)
-            self._colormapActions.append(cmAction)
-
-        self._colorbarAction = QAction("Show/hide colorbar", self)
-        self._colorbarAction.triggered.connect(self._setColorbarOnOff)
-        self.addAction(self._colorbarAction)
-
-        self._wwlAction = QAction("Window level/width", self)
-        self._wwlAction.triggered.connect(self._showImageProperties)
-        self.addAction(self._wwlAction)
-
-    def _resetImage(self):
-        self._imageViewer.secondaryImage = None
-
-    def _setColorbarOnOff(self):
-        self._secondaryImageLayer.colorbarOn = not self._secondaryImageLayer.colorbarOn
-
-    def _showImageProperties(self):
-        self._imageFusionProp = ImageFusionPropEditor(self._secondaryImageLayer.image.data)
-        self._imageFusionProp.show()
-
-    def setFusion(self, name:str):
-        self._imageViewer.secondaryImageLayer.image.lookupTableName = name
-
-class DoseComparisonMenu(QMenu):
-    def __init__(self, imageViewer:Image3DViewer):
-        super().__init__("Dose comparison")
-
-        self.dataViewer = None
-
-        self._imageViewer = imageViewer
-        self._secondaryImageLayer = self._imageViewer.secondaryImageLayer
-
-        self._metricsMenu = QMenu("Metrics", self)
-        self.addMenu(self._metricsMenu)
-
-        self._diffAction = QAction("Difference", self._metricsMenu)
-        self._diffAction.triggered.connect(self._setDiffMetric)
-        self._metricsMenu.addAction(self._diffAction)
-        self._absDiffAction = QAction("Absolute difference", self._metricsMenu)
-        self._absDiffAction.triggered.connect(self._setAbsDiffMetric)
-        self._metricsMenu.addAction(self._absDiffAction)
-        self._gammaAction = QAction("Gamma", self._metricsMenu)
-        self._gammaAction.triggered.connect(self._setGammaMetric)
-        self._metricsMenu.addAction(self._gammaAction)
-
-        self._colorMapMenu = QMenu("Colormap", self)
-        self.addMenu(self._colorMapMenu)
-
-        self._colormapActions = []
-        cms = matplotlib.pyplot.colormaps()
-
-        for cm in cms:
-            cmAction = QAction(cm, self._colorMapMenu)
-            cmAction.triggered.connect(functools.partial(self.setFusion, cm))
-            self._colorMapMenu.addAction(cmAction)
-            self._colormapActions.append(cmAction)
-
-        self._colorbarAction = QAction("Show/hide colorbar", self)
-        self._colorbarAction.triggered.connect(self._setColorbarOnOff)
-        self.addAction(self._colorbarAction)
-
-        self._wwlAction = QAction("Window level/width", self)
-        self._wwlAction.triggered.connect(self._showImageProperties)
-        self.addAction(self._wwlAction)
-
-    def _setColorbarOnOff(self):
-        self._secondaryImageLayer.colorbarOn = not self._secondaryImageLayer.colorbarOn
-
-    def _showImageProperties(self):
-        self._imageFusionProp = ImageFusionPropEditor(self._secondaryImageLayer.image.data)
-        self._imageFusionProp.show()
-
-    def _setDiffMetric(self):
-        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.DIFFERENCE
-    def _setAbsDiffMetric(self):
-        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.ABSOLUTE_DIFFERENCE
-    def _setGammaMetric(self):
-        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.GAMMA
-
-    def setFusion(self, name:str):
-        self._imageViewer.secondaryImageLayer.lookupTableName = name
-
-class RTPlanMenu(QMenu):
-    def __init__(self, imageViewer:Image3DViewer):
-        super().__init__("RT plan")
-
-        self._imageViewer = imageViewer
-
-        self._resetAction = QAction("Reset", self)
-        self._resetAction.triggered.connect(self._resetPlan)
-        self.addAction(self._resetAction)
-
-    def _resetPlan(self):
-        self._imageViewer.rtPlan = None
-
-class WWLPreset:
-    def __init__(self, name:str, wwl:Sequence[float]):
-        self.name:str = name
-        self.wwl:Sequence[float] = wwl
-
-def presets() -> Sequence[WWLPreset]:
-    presets = []
-
-    ps = WWLPreset("Bone", (1600, 450))
-    presets.append(ps)
-    ps = WWLPreset("Brain", (100, 35))
-    presets.append(ps)
-    ps = WWLPreset("Dental", (2000, 400))
-    presets.append(ps)
-    ps = WWLPreset("Inner ear", (4000, 700))
-    presets.append(ps)
-    ps = WWLPreset("Larynx", (250, 40))
-    presets.append(ps)
-    ps = WWLPreset("Liver", (350, 50))
-    presets.append(ps)
-    ps = WWLPreset("Lung", (1600, -600))
-    presets.append(ps)
-    ps = WWLPreset("Mediastinum", (400, 40))
-    presets.append(ps)
-    ps = WWLPreset("Pelvis", (1000, 250))
-    presets.append(ps)
-    ps = WWLPreset("Soft tissue", (350, 40))
-    presets.append(ps)
-    ps = WWLPreset("Spine", (300, 35))
-    presets.append(ps)
-    ps = WWLPreset("Vertebrae", (2000, 350))
-    presets.append(ps)
-
-    return presets
+import functools
+from typing import Sequence
+
+import matplotlib
+from PyQt5.QtWidgets import QComboBox, QWidgetAction, QMenu, QAction
+
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.dataViewerToolbar import DataViewerToolbar
+from opentps.gui.viewer.dataViewerComponents.doseComparisonImageProvider import DoseComparisonImageProvider
+from opentps.gui.viewer.dataViewerComponents.image3DViewer import Image3DViewer
+from opentps.gui.viewer.dataViewerComponents.imageFusionPropEditor import ImageFusionPropEditor
+
+
+class ImageViewerActions:
+    def __init__(self, imageViewer:Image3DViewer):
+        self._imageViewer = imageViewer
+
+        self._viewTypeToStr = {self._imageViewer.ViewerTypes.AXIAL: 'Axial',
+                               self._imageViewer.ViewerTypes.CORONAL: 'Coronal',
+                               self._imageViewer.ViewerTypes.SAGITTAL: 'Sagittal'}
+        self._strToViewType = {v: k for k, v in self._viewTypeToStr.items()}
+
+        self._separator = None
+
+        self._viewTypeCombo = QComboBox()
+        self._viewTypeCombo.setFixedSize(80, 16)
+        self._viewTypeCombo.addItems(list(self._viewTypeToStr.values()))
+
+        self._viewTypeAction = QWidgetAction(None)
+        self._viewTypeAction.setDefaultWidget(self._viewTypeCombo)
+
+        self._primaryImageMenu = PrimaryImageMenu(self._imageViewer)
+        self._secondaryImageMenu = SecondaryImageMenu(self._imageViewer)
+        self._doseComparisonMenu = DoseComparisonMenu(self._imageViewer)
+        self._rtPlanMenu = RTPlanMenu(self._imageViewer)
+
+        self.hide()
+
+        self._viewTypeCombo.setCurrentIndex(self._viewTypeToIndex(self._imageViewer.viewType))
+        self._viewTypeCombo.currentIndexChanged.connect(self._handleViewTypeSelection)
+        self._imageViewer.viewTypeChangedSignal.connect(self._handleExternalViewTypeChange)
+
+    @property
+    def doseComparisonDataViewer(self):
+        return self._doseComparisonMenu.dataViewer
+
+    @doseComparisonDataViewer.setter
+    def doseComparisonDataViewer(self, dataViewer):
+        self._doseComparisonMenu.dataViewer = dataViewer
+
+
+    def _viewTypeToIndex(self, viewType):
+        return list(self._viewTypeToStr.keys()).index(viewType)
+
+    def setImageViewer(self, imageViewer):
+        self._imageViewer = imageViewer
+
+    def addToToolbar(self, toolbar:DataViewerToolbar):
+        self._separator = toolbar.addSeparator()
+        toolbar.addAction(self._viewTypeAction)
+        toolbar.toolsMenu.addMenu(self._primaryImageMenu)
+        toolbar.toolsMenu.addMenu(self._secondaryImageMenu)
+        toolbar.toolsMenu.addMenu(self._doseComparisonMenu)
+        toolbar.toolsMenu.addMenu(self._rtPlanMenu)
+
+    def hide(self):
+        if not self._separator is None:
+            self._separator.setVisible(False)
+        self._viewTypeAction.setVisible(False)
+
+    def show(self):
+        self._separator.setVisible(True)
+        self._viewTypeAction.setVisible(True)
+
+    def _handleViewTypeSelection(self, selectionIndex):
+        selectionText = self._viewTypeCombo.itemText(selectionIndex)
+        self._imageViewer.viewType = self._strToViewType[selectionText]
+
+    def _handleExternalViewTypeChange(self, viewType):
+        self._viewTypeCombo.setCurrentIndex(self._viewTypeToIndex(viewType))
+
+
+class PrimaryImageMenu(QMenu):
+    def __init__(self, imageViewer:Image3DViewer):
+        super().__init__("Primary image")
+
+        self._imageViewer = imageViewer
+
+        self._wwlMenu = QMenu("Window level/width", self)
+        self.addMenu(self._wwlMenu)
+
+        self._presetMenu = QMenu("Presets", self)
+        self._wwlMenu.addMenu(self._presetMenu)
+
+        self._wwlActions = []
+        for ps in presets():
+            wwlAction = QAction(ps.name + ' ' + str((ps.wwl[1], ps.wwl[0])), self)
+            wwlAction.triggered.connect(functools.partial(self._setPreset, ps))
+
+            self._wwlActions.append(wwlAction)
+
+            self._presetMenu.addAction(wwlAction)
+
+    def _setPreset(self, ps):
+        Image3DForViewer(self._imageViewer.primaryImage).wwlValue = ps.wwl
+
+class SecondaryImageMenu(QMenu):
+    def __init__(self, imageViewer:Image3DViewer):
+        super().__init__("Secondary image")
+
+        self._imageViewer = imageViewer
+        self._secondaryImageLayer = self._imageViewer.secondaryImageLayer
+
+        self._resetAction = QAction("Reset", self)
+        self._resetAction.triggered.connect(self._resetImage)
+        self.addAction(self._resetAction)
+
+        self._colorMapMenu = QMenu("Colormap", self)
+        self.addMenu(self._colorMapMenu)
+
+        self._colormapActions = []
+        cms = matplotlib.pyplot.colormaps()
+
+        for cm in cms:
+            cmAction = QAction(cm, self._colorMapMenu)
+            cmAction.triggered.connect(functools.partial(self.setFusion, cm))
+            self._colorMapMenu.addAction(cmAction)
+            self._colormapActions.append(cmAction)
+
+        self._colorbarAction = QAction("Show/hide colorbar", self)
+        self._colorbarAction.triggered.connect(self._setColorbarOnOff)
+        self.addAction(self._colorbarAction)
+
+        self._wwlAction = QAction("Window level/width", self)
+        self._wwlAction.triggered.connect(self._showImageProperties)
+        self.addAction(self._wwlAction)
+
+    def _resetImage(self):
+        self._imageViewer.secondaryImage = None
+
+    def _setColorbarOnOff(self):
+        self._secondaryImageLayer.colorbarOn = not self._secondaryImageLayer.colorbarOn
+
+    def _showImageProperties(self):
+        self._imageFusionProp = ImageFusionPropEditor(self._secondaryImageLayer.image.data)
+        self._imageFusionProp.show()
+
+    def setFusion(self, name:str):
+        self._imageViewer.secondaryImageLayer.image.lookupTableName = name
+
+class DoseComparisonMenu(QMenu):
+    def __init__(self, imageViewer:Image3DViewer):
+        super().__init__("Dose comparison")
+
+        self.dataViewer = None
+
+        self._imageViewer = imageViewer
+        self._secondaryImageLayer = self._imageViewer.secondaryImageLayer
+
+        self._metricsMenu = QMenu("Metrics", self)
+        self.addMenu(self._metricsMenu)
+
+        self._diffAction = QAction("Difference", self._metricsMenu)
+        self._diffAction.triggered.connect(self._setDiffMetric)
+        self._metricsMenu.addAction(self._diffAction)
+        self._absDiffAction = QAction("Absolute difference", self._metricsMenu)
+        self._absDiffAction.triggered.connect(self._setAbsDiffMetric)
+        self._metricsMenu.addAction(self._absDiffAction)
+        self._gammaAction = QAction("Gamma", self._metricsMenu)
+        self._gammaAction.triggered.connect(self._setGammaMetric)
+        self._metricsMenu.addAction(self._gammaAction)
+
+        self._colorMapMenu = QMenu("Colormap", self)
+        self.addMenu(self._colorMapMenu)
+
+        self._colormapActions = []
+        cms = matplotlib.pyplot.colormaps()
+
+        for cm in cms:
+            cmAction = QAction(cm, self._colorMapMenu)
+            cmAction.triggered.connect(functools.partial(self.setFusion, cm))
+            self._colorMapMenu.addAction(cmAction)
+            self._colormapActions.append(cmAction)
+
+        self._colorbarAction = QAction("Show/hide colorbar", self)
+        self._colorbarAction.triggered.connect(self._setColorbarOnOff)
+        self.addAction(self._colorbarAction)
+
+        self._wwlAction = QAction("Window level/width", self)
+        self._wwlAction.triggered.connect(self._showImageProperties)
+        self.addAction(self._wwlAction)
+
+    def _setColorbarOnOff(self):
+        self._secondaryImageLayer.colorbarOn = not self._secondaryImageLayer.colorbarOn
+
+    def _showImageProperties(self):
+        self._imageFusionProp = ImageFusionPropEditor(self._secondaryImageLayer.image.data)
+        self._imageFusionProp.show()
+
+    def _setDiffMetric(self):
+        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.DIFFERENCE
+    def _setAbsDiffMetric(self):
+        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.ABSOLUTE_DIFFERENCE
+    def _setGammaMetric(self):
+        self.dataViewer.comparisonMetric = DoseComparisonImageProvider.Metric.GAMMA
+
+    def setFusion(self, name:str):
+        self._imageViewer.secondaryImageLayer.lookupTableName = name
+
+class RTPlanMenu(QMenu):
+    def __init__(self, imageViewer:Image3DViewer):
+        super().__init__("RT plan")
+
+        self._imageViewer = imageViewer
+
+        self._resetAction = QAction("Reset", self)
+        self._resetAction.triggered.connect(self._resetPlan)
+        self.addAction(self._resetAction)
+
+    def _resetPlan(self):
+        self._imageViewer.rtPlan = None
+
+class WWLPreset:
+    def __init__(self, name:str, wwl:Sequence[float]):
+        self.name:str = name
+        self.wwl:Sequence[float] = wwl
+
+def presets() -> Sequence[WWLPreset]:
+    presets = []
+
+    ps = WWLPreset("Bone", (1600, 450))
+    presets.append(ps)
+    ps = WWLPreset("Brain", (100, 35))
+    presets.append(ps)
+    ps = WWLPreset("Dental", (2000, 400))
+    presets.append(ps)
+    ps = WWLPreset("Inner ear", (4000, 700))
+    presets.append(ps)
+    ps = WWLPreset("Larynx", (250, 40))
+    presets.append(ps)
+    ps = WWLPreset("Liver", (350, 50))
+    presets.append(ps)
+    ps = WWLPreset("Lung", (1600, -600))
+    presets.append(ps)
+    ps = WWLPreset("Mediastinum", (400, 40))
+    presets.append(ps)
+    ps = WWLPreset("Pelvis", (1000, 250))
+    presets.append(ps)
+    ps = WWLPreset("Soft tissue", (350, 40))
+    presets.append(ps)
+    ps = WWLPreset("Spine", (300, 35))
+    presets.append(ps)
+    ps = WWLPreset("Vertebrae", (2000, 350))
+    presets.append(ps)
+
+    return presets
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/contourLayer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/contourLayer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-from functools import partial
-from typing import Optional, Union, Sequence
-
-from vtkmodules import vtkImagingCore, vtkCommonCore
-from vtkmodules.vtkFiltersCore import vtkContourFilter
-from vtkmodules.vtkRenderingCore import vtkActor, vtkPolyDataMapper
-
-from opentps.core.data.images._image3D import Image3D
-from opentps.core.data.images import ROIMask
-from opentps.core.data._roiContour import ROIContour
-from opentps.gui.viewer.dataForViewer.ROIContourForViewer import ROIContourForViewer
-from opentps.gui.viewer.dataForViewer.ROIMaskForViewer import ROIMaskForViewer
-
-
-class ContourLayer:
-    def __init__(self, renderer, renderWindow):
-        self._contours = [] # Acts as a cache
-        self._referenceImage = None
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-        self._resliceAxes = None
-        self._vtkContours = []
-        self._partialHandlers = []
-
-    def close(self):
-        for vtkContour in self._vtkContours:
-            vtkContour.close()
-
-    @property
-    def contours(self) -> Sequence[Union[ROIContourForViewer, ROIMaskForViewer]]:
-        return [contour for contour in self._contours]
-
-    def setNewContour(self, contour:Union[ROIContour, ROIMask]):
-        if isinstance(contour, ROIContour):
-            contour = ROIContourForViewer(contour)
-        elif isinstance(contour, ROIMask):
-            contour = ROIMaskForViewer(contour)
-        else:
-            raise ValueError(str(type(contour)) + ' is not a valid type for a contour.')
-
-        if contour in self._contours:
-            return
-
-        if not contour.visible:
-            return
-
-        contour.referenceImage = self.referenceImage
-
-        self._contours.append(contour)
-
-        vtkContourObj = vtkContour(contour, self._renderWindow)
-
-        self._renderer.AddActor(vtkContourObj.actor)
-        vtkContourObj.resliceAxes = self._resliceAxes
-        self._vtkContours.append(vtkContourObj)
-
-        partialHandler = partial(self._handleVisibilityChange, contour)
-        self._partialHandlers.append(partialHandler)
-        contour.visibleChangedSignal.connect(partialHandler)
-
-        self._renderWindow.Render()
-
-    def _handleVisibilityChange(self, contour:Union[ROIContourForViewer, ROIMaskForViewer], visible):
-        if not contour.visible:
-            self._removeContour(contour)
-
-    def _removeContour(self, contour:Union[ROIContourForViewer, ROIMaskForViewer]):
-        contourIndex = self._contours.index(contour)
-        vtkContourObj = self._vtkContours[contourIndex]
-        partialHandler = self._partialHandlers[contourIndex]
-        self._renderer.RemoveActor(vtkContourObj.actor)
-
-        self._contours.remove(contour)
-        self._vtkContours.remove(vtkContourObj)
-        self._partialHandlers.remove(partialHandler)
-
-        contour.visibleChangedSignal.disconnect(partialHandler)
-
-
-    @property
-    def referenceImage(self) -> Optional[Image3D]:
-        return self._referenceImage
-
-    @referenceImage.setter
-    def referenceImage(self, image: Image3D):
-        self._referenceImage = image
-
-        for contour in self._contours:
-            contour.referenceImage = self._referenceImage
-
-    @property
-    def resliceAxes(self):
-        return self._resliceAxes
-
-    @resliceAxes.setter
-    def resliceAxes(self, resliceAxes):
-        self._resliceAxes = resliceAxes
-        self._updateContoursResliceAxes()
-
-    def _updateContoursResliceAxes(self):
-        for vtkContour in self._vtkContours:
-            vtkContour.resliceAxes = self._resliceAxes
-
-    def resliceDataFromPhysicalPoint(self, point):
-        return [contour.resliceDataFromPhysicalPoint(point) for contour in self._vtkContours]
-
-class vtkContour:
-    def __init__(self, contour, renderWindow):
-        self.actor = vtkActor()
-        self._contour = contour
-        self.contourFilter = vtkContourFilter()
-        self.mapper = vtkPolyDataMapper()
-        self.renderWindow = renderWindow  # Not very beautiful to pass renderWindow but fewer lines of code than trigering a render event
-        self.reslice = vtkImagingCore.vtkImageReslice()
-
-        self.actor.SetMapper(self.mapper)
-
-        self.reslice.SetOutputDimensionality(2)
-        self.reslice.SetInterpolationModeToNearestNeighbor()
-
-        self.reslice.SetInputConnection(self._contour.vtkOutputPort)
-        self.contourFilter.SetInputConnection(self.reslice.GetOutputPort())
-        self.mapper.SetInputConnection(self.contourFilter.GetOutputPort())
-
-        self.contourFilter.SetValue(0, 0.1)
-        self.contourFilter.Update()
-
-        self.actor.GetProperty().SetLineWidth(3)
-
-        self.reloadColor()
-
-        self.setVisible(self._contour.visible)
-
-        self._contour.visibleChangedSignal.connect(self.setVisible)
-        self._contour.colorChangedSignal.connect(self.reloadColor)
-
-    def close(self):
-        self._contour.visibleChangedSignal.disconnect(self.setVisible)
-        self._contour.colorChangedSignal.disconnect(self.reloadColor)
-
-    @property
-    def resliceAxes(self):
-        return self.reslice.GetResliceAxes()
-
-    @resliceAxes.setter
-    def resliceAxes(self, resliceAxes):
-        self.reslice.SetResliceAxes(resliceAxes)
-
-    def reloadColor(self):
-        imageColor = self._contour.color
-
-        # Create a greyscale lookup table
-        table = vtkCommonCore.vtkLookupTable()
-        table.SetRange(0, 1)  # image intensity range
-        table.SetValueRange(0.0, 1.0)  # from black to white
-        table.SetSaturationRange(0.0, 0.0)  # no color saturation
-        table.SetRampToLinear()
-
-        table.SetNumberOfTableValues(2)
-        table.SetTableValue(0, (imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1))
-        table.SetTableValue(1, (imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1))
-        table.SetBelowRangeColor(0, 0, 0, 0)
-        table.SetUseBelowRangeColor(True)
-        table.SetAboveRangeColor(imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1)
-        table.SetUseAboveRangeColor(True)
-        table.Build()
-
-        # contourActor.GetProperty().SetColor(imageColor[0], imageColor[1], imageColor[2])
-        self.mapper.SetLookupTable(table)
-
-    def setVisible(self, visible: bool):
-        self.actor.SetVisibility(visible)
-        self.renderWindow.Render()
-
-    def resliceDataFromPhysicalPoint(self, point):
-        imageData = self.reslice.GetInput(0)
-
-        ind = [0, 0, 0]
-        imageData.TransformPhysicalPointToContinuousIndex(point, ind)
-        return imageData.GetScalarComponentAsFloat(int(ind[0]), int(ind[1]), int(ind[2]), 0)
+from functools import partial
+from typing import Optional, Union, Sequence
+
+from vtkmodules import vtkImagingCore, vtkCommonCore
+from vtkmodules.vtkFiltersCore import vtkContourFilter
+from vtkmodules.vtkRenderingCore import vtkActor, vtkPolyDataMapper
+
+from opentps.core.data.images._image3D import Image3D
+from opentps.core.data.images import ROIMask
+from opentps.core.data._roiContour import ROIContour
+from opentps.gui.viewer.dataForViewer.ROIContourForViewer import ROIContourForViewer
+from opentps.gui.viewer.dataForViewer.ROIMaskForViewer import ROIMaskForViewer
+
+
+class ContourLayer:
+    def __init__(self, renderer, renderWindow):
+        self._contours = [] # Acts as a cache
+        self._referenceImage = None
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+        self._resliceAxes = None
+        self._vtkContours = []
+        self._partialHandlers = []
+
+    def close(self):
+        for vtkContour in self._vtkContours:
+            vtkContour.close()
+
+    @property
+    def contours(self) -> Sequence[Union[ROIContourForViewer, ROIMaskForViewer]]:
+        return [contour for contour in self._contours]
+
+    def setNewContour(self, contour:Union[ROIContour, ROIMask]):
+        if isinstance(contour, ROIContour):
+            contour = ROIContourForViewer(contour)
+        elif isinstance(contour, ROIMask):
+            contour = ROIMaskForViewer(contour)
+        else:
+            raise ValueError(str(type(contour)) + ' is not a valid type for a contour.')
+
+        if contour in self._contours:
+            return
+
+        if not contour.visible:
+            return
+
+        contour.referenceImage = self.referenceImage
+
+        self._contours.append(contour)
+
+        vtkContourObj = vtkContour(contour, self._renderWindow)
+
+        self._renderer.AddActor(vtkContourObj.actor)
+        vtkContourObj.resliceAxes = self._resliceAxes
+        self._vtkContours.append(vtkContourObj)
+
+        partialHandler = partial(self._handleVisibilityChange, contour)
+        self._partialHandlers.append(partialHandler)
+        contour.visibleChangedSignal.connect(partialHandler)
+
+        self._renderWindow.Render()
+
+    def _handleVisibilityChange(self, contour:Union[ROIContourForViewer, ROIMaskForViewer], visible):
+        if not contour.visible:
+            self._removeContour(contour)
+
+    def _removeContour(self, contour:Union[ROIContourForViewer, ROIMaskForViewer]):
+        contourIndex = self._contours.index(contour)
+        vtkContourObj = self._vtkContours[contourIndex]
+        partialHandler = self._partialHandlers[contourIndex]
+        self._renderer.RemoveActor(vtkContourObj.actor)
+
+        self._contours.remove(contour)
+        self._vtkContours.remove(vtkContourObj)
+        self._partialHandlers.remove(partialHandler)
+
+        contour.visibleChangedSignal.disconnect(partialHandler)
+
+
+    @property
+    def referenceImage(self) -> Optional[Image3D]:
+        return self._referenceImage
+
+    @referenceImage.setter
+    def referenceImage(self, image: Image3D):
+        self._referenceImage = image
+
+        for contour in self._contours:
+            contour.referenceImage = self._referenceImage
+
+    @property
+    def resliceAxes(self):
+        return self._resliceAxes
+
+    @resliceAxes.setter
+    def resliceAxes(self, resliceAxes):
+        self._resliceAxes = resliceAxes
+        self._updateContoursResliceAxes()
+
+    def _updateContoursResliceAxes(self):
+        for vtkContour in self._vtkContours:
+            vtkContour.resliceAxes = self._resliceAxes
+
+    def resliceDataFromPhysicalPoint(self, point):
+        return [contour.resliceDataFromPhysicalPoint(point) for contour in self._vtkContours]
+
+class vtkContour:
+    def __init__(self, contour, renderWindow):
+        self.actor = vtkActor()
+        self._contour = contour
+        self.contourFilter = vtkContourFilter()
+        self.mapper = vtkPolyDataMapper()
+        self.renderWindow = renderWindow  # Not very beautiful to pass renderWindow but fewer lines of code than trigering a render event
+        self.reslice = vtkImagingCore.vtkImageReslice()
+
+        self.actor.SetMapper(self.mapper)
+
+        self.reslice.SetOutputDimensionality(2)
+        self.reslice.SetInterpolationModeToNearestNeighbor()
+
+        self.reslice.SetInputConnection(self._contour.vtkOutputPort)
+        self.contourFilter.SetInputConnection(self.reslice.GetOutputPort())
+        self.mapper.SetInputConnection(self.contourFilter.GetOutputPort())
+
+        self.contourFilter.SetValue(0, 0.1)
+        self.contourFilter.Update()
+
+        self.actor.GetProperty().SetLineWidth(3)
+
+        self.reloadColor()
+
+        self.setVisible(self._contour.visible)
+
+        self._contour.visibleChangedSignal.connect(self.setVisible)
+        self._contour.colorChangedSignal.connect(self.reloadColor)
+
+    def close(self):
+        self._contour.visibleChangedSignal.disconnect(self.setVisible)
+        self._contour.colorChangedSignal.disconnect(self.reloadColor)
+
+    @property
+    def resliceAxes(self):
+        return self.reslice.GetResliceAxes()
+
+    @resliceAxes.setter
+    def resliceAxes(self, resliceAxes):
+        self.reslice.SetResliceAxes(resliceAxes)
+
+    def reloadColor(self):
+        imageColor = self._contour.color
+
+        # Create a greyscale lookup table
+        table = vtkCommonCore.vtkLookupTable()
+        table.SetRange(0, 1)  # image intensity range
+        table.SetValueRange(0.0, 1.0)  # from black to white
+        table.SetSaturationRange(0.0, 0.0)  # no color saturation
+        table.SetRampToLinear()
+
+        table.SetNumberOfTableValues(2)
+        table.SetTableValue(0, (imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1))
+        table.SetTableValue(1, (imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1))
+        table.SetBelowRangeColor(0, 0, 0, 0)
+        table.SetUseBelowRangeColor(True)
+        table.SetAboveRangeColor(imageColor[0] / 255.0, imageColor[1] / 255.0, imageColor[2] / 255.0, 1)
+        table.SetUseAboveRangeColor(True)
+        table.Build()
+
+        # contourActor.GetProperty().SetColor(imageColor[0], imageColor[1], imageColor[2])
+        self.mapper.SetLookupTable(table)
+
+    def setVisible(self, visible: bool):
+        self.actor.SetVisibility(visible)
+        self.renderWindow.Render()
+
+    def resliceDataFromPhysicalPoint(self, point):
+        imageData = self.reslice.GetInput(0)
+
+        ind = [0, 0, 0]
+        imageData.TransformPhysicalPointToContinuousIndex(point, ind)
+        return imageData.GetScalarComponentAsFloat(int(ind[0]), int(ind[1]), int(ind[2]), 0)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/crossHairLayer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/crossHairLayer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import typing
-
-import vtkmodules.vtkRenderingOpenGL2 #This is necessary to avoid a seg fault
-import vtkmodules.vtkRenderingFreeType  #This is necessary to avoid a seg fault
-from vtkmodules.vtkCommonColor import vtkNamedColors
-from vtkmodules.vtkCommonCore import vtkPoints
-from vtkmodules.vtkCommonDataModel import vtkPolyLine, vtkCellArray, vtkPolyData
-from vtkmodules.vtkRenderingCore import vtkPolyDataMapper, vtkActor
-
-
-class CrossHairLayer:
-    def __init__(self, renderer, renderWindow):
-        self._crossHairActor = vtkActor()
-        self._crossHairEnabled = False
-        self._crossHairMapper = vtkPolyDataMapper()
-        self._position = (0, 0)
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-        self._visible = False
-
-        colors = vtkNamedColors()
-
-        self._crossHairActor.SetMapper(self._crossHairMapper)
-        self._crossHairActor.GetProperty().SetColor(colors.GetColor3d('Tomato'))
-        self._renderer.AddActor(self._crossHairActor)
-        self._crossHairActor.VisibilityOff()
-
-    def close(self):
-        pass
-
-    @property
-    def position(self) -> typing.Sequence:
-        return self._position
-
-    @position.setter
-    def position(self, position: typing.Sequence):
-        points = vtkPoints()
-        points.InsertNextPoint((position[0] - 10, position[1], 0.01))
-        points.InsertNextPoint((position[0] + 10, position[1], 0.01))
-        points.InsertNextPoint((position[0], position[1] - 10, 0.01))
-        points.InsertNextPoint((position[0], position[1] + 10, 0.01))
-
-        polyLine = vtkPolyLine()
-        polyLine.GetPointIds().SetNumberOfIds(2)
-        polyLine2 = vtkPolyLine()
-        polyLine2.GetPointIds().SetNumberOfIds(2)
-        for i in range(0, 2):
-            polyLine.GetPointIds().SetId(i, i)
-            polyLine2.GetPointIds().SetId(i, i + 2)
-
-        cells = vtkCellArray()
-        cells.InsertNextCell(polyLine)
-        cells.InsertNextCell(polyLine2)
-
-        polyData = vtkPolyData()
-        polyData.SetPoints(points)
-        polyData.SetLines(cells)
-
-        self._crossHairMapper.SetInputData(polyData)
-        self._position = position
-
-        self._renderWindow.Render()
-
-    @property
-    def visible(self) -> bool:
-        return self._visible
-
-    @visible.setter
-    def visible(self, visible: bool):
-        self._crossHairActor.SetVisibility(visible)
-        self._visible = visible
+import typing
+
+import vtkmodules.vtkRenderingOpenGL2 #This is necessary to avoid a seg fault
+import vtkmodules.vtkRenderingFreeType  #This is necessary to avoid a seg fault
+from vtkmodules.vtkCommonColor import vtkNamedColors
+from vtkmodules.vtkCommonCore import vtkPoints
+from vtkmodules.vtkCommonDataModel import vtkPolyLine, vtkCellArray, vtkPolyData
+from vtkmodules.vtkRenderingCore import vtkPolyDataMapper, vtkActor
+
+
+class CrossHairLayer:
+    def __init__(self, renderer, renderWindow):
+        self._crossHairActor = vtkActor()
+        self._crossHairEnabled = False
+        self._crossHairMapper = vtkPolyDataMapper()
+        self._position = (0, 0)
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+        self._visible = False
+
+        colors = vtkNamedColors()
+
+        self._crossHairActor.SetMapper(self._crossHairMapper)
+        self._crossHairActor.GetProperty().SetColor(colors.GetColor3d('Tomato'))
+        self._renderer.AddActor(self._crossHairActor)
+        self._crossHairActor.VisibilityOff()
+
+    def close(self):
+        pass
+
+    @property
+    def position(self) -> typing.Sequence:
+        return self._position
+
+    @position.setter
+    def position(self, position: typing.Sequence):
+        points = vtkPoints()
+        points.InsertNextPoint((position[0] - 10, position[1], 0.01))
+        points.InsertNextPoint((position[0] + 10, position[1], 0.01))
+        points.InsertNextPoint((position[0], position[1] - 10, 0.01))
+        points.InsertNextPoint((position[0], position[1] + 10, 0.01))
+
+        polyLine = vtkPolyLine()
+        polyLine.GetPointIds().SetNumberOfIds(2)
+        polyLine2 = vtkPolyLine()
+        polyLine2.GetPointIds().SetNumberOfIds(2)
+        for i in range(0, 2):
+            polyLine.GetPointIds().SetId(i, i)
+            polyLine2.GetPointIds().SetId(i, i + 2)
+
+        cells = vtkCellArray()
+        cells.InsertNextCell(polyLine)
+        cells.InsertNextCell(polyLine2)
+
+        polyData = vtkPolyData()
+        polyData.SetPoints(points)
+        polyData.SetLines(cells)
+
+        self._crossHairMapper.SetInputData(polyData)
+        self._position = position
+
+        self._renderWindow.Render()
+
+    @property
+    def visible(self) -> bool:
+        return self._visible
+
+    @visible.setter
+    def visible(self, visible: bool):
+        self._crossHairActor.SetVisibility(visible)
+        self._visible = visible
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/lookupTables.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/lookupTables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,148 @@
-from typing import Sequence, Tuple
-
-import numpy as np
-import vtkmodules.vtkCommonCore as vtkCommonCore
-from matplotlib import pyplot as plt
-from vtkmodules.vtkCommonDataModel import vtkPiecewiseFunction
-from vtkmodules.vtkRenderingCore import vtkColorTransferFunction
-
-
-def fusionLT(range:Sequence[float], opacity:float, colormap:str) -> vtkCommonCore.vtkLookupTable:
-    table = vtkCommonCore.vtkLookupTable()
-    table.SetRange(range[0], range[1])  # image intensity range
-    table.SetValueRange(0.0, 1.0)  # from black to white
-    table.SetSaturationRange(0.0, 0.0)  # no color saturation
-    table.SetRampToLinear()
-
-    cm = plt.cm.get_cmap(colormap)
-    linInd = list(np.arange(0, 1.01, 0.01))
-
-    table.SetNumberOfTableValues(len(linInd))
-    LastCMVal = (0, 0, 0)
-    for i, ind in enumerate(linInd):
-        cmVal = cm(ind)
-        LastCMVal = cmVal
-        if i==0:
-            table.SetTableValue(i, (cmVal[0], cmVal[1], cmVal[2], 0))
-        else:
-            table.SetTableValue(i, (cmVal[0], cmVal[1], cmVal[2], opacity))
-
-    table.SetBelowRangeColor(0, 0, 0, 0)
-    table.SetUseBelowRangeColor(True)
-    table.SetAboveRangeColor(LastCMVal[0], LastCMVal[1], LastCMVal[2], opacity)
-    table.SetUseAboveRangeColor(True)
-    table.Build()
-
-    return table
-
-def grayLT(range) -> vtkCommonCore.vtkLookupTable:
-    table = vtkCommonCore.vtkLookupTable()
-    table.SetRange(range[0], range[1])  # image intensity range
-    table.SetTableRange(range[0], range[1])  # image intensity range
-    table.SetValueRange(0.0, 1.0)  # from black to white
-    table.SetSaturationRange(0.0, 0.0)  # no color saturation
-    table.SetRampToLinear()
-    table.SetAlpha(1.)
-    table.SetAboveRangeColor(1., 1., 1., 1.)
-    table.SetBelowRangeColor(0., 0., 0., 1.)
-    table.SetUseAboveRangeColor(True)
-    table.SetUseBelowRangeColor(True)
-    table.Build()
-
-    return table
-
-
-def fusionLTTo3DLT(lt:vtkCommonCore.vtkLookupTable) -> Tuple[vtkColorTransferFunction, vtkPiecewiseFunction, vtkPiecewiseFunction]:
-    rangeVal = lt.GetRange()
-
-    volumeColor = vtkColorTransferFunction()
-    volumeScalarOpacity = vtkPiecewiseFunction()
-    volumeGradientOpacity = vtkPiecewiseFunction()
-
-    volumeScalarOpacity.AddPoint(rangeVal[0], 0)
-    volumeScalarOpacity.AddPoint((rangeVal[0]+rangeVal[1])/.2, 0.0)
-    volumeScalarOpacity.AddPoint(3*(rangeVal[0] + rangeVal[1]) /4. , 0.5)
-    volumeScalarOpacity.AddPoint(rangeVal[1], 1.)
-
-    volumeGradientOpacity.AddPoint(rangeVal[0], 0.1)
-    volumeGradientOpacity.AddPoint((rangeVal[0]+rangeVal[1])/2, 0.25)
-    volumeGradientOpacity.AddPoint(3*(rangeVal[0] + rangeVal[1]) /4. , 0.5)
-    volumeGradientOpacity.AddPoint(rangeVal[1], 1.)
-
-    tableVals = np.linspace(rangeVal[0], rangeVal[1], lt.GetNumberOfTableValues())
-    for i in range(lt.GetNumberOfTableValues()):
-        tbVal = lt.GetTableValue(i)
-        volumeColor.AddRGBPoint(tableVals[i], tbVal[0], tbVal[1], tbVal[2])
-
-    return volumeColor, volumeScalarOpacity, volumeGradientOpacity
-
-def ct3DLT() -> Tuple[vtkColorTransferFunction, vtkPiecewiseFunction, vtkPiecewiseFunction]:
-    volumeColor = vtkColorTransferFunction()
-    volumeScalarOpacity = vtkPiecewiseFunction()
-    volumeGradientOpacity = vtkPiecewiseFunction()
-
-    volumeColor.AddRGBPoint(-1000, 0.0, 0.0, 0.0)
-    volumeColor.AddRGBPoint(-500, 240.0/255.0, 184.0/255.0, 160.0/255.0)
-    volumeColor.AddRGBPoint(0, 232/255, 147/255, 132/255)
-    volumeColor.AddRGBPoint(500, 1.0, 1.0, 240.0 / 255.0)
-    volumeColor.AddRGBPoint(700,  242/255, 220/255, 172/255)
-    volumeColor.AddRGBPoint(1800, 173/255, 166/255, 166/255)
-    volumeColor.AddRGBPoint(2500, 237/255, 171/255, 64/255)
-
-    volumeScalarOpacity.AddPoint(-1000, 0.00)
-    volumeScalarOpacity.AddPoint(-500, 0.05)
-    volumeScalarOpacity.AddPoint(-200, 0.5)
-    volumeScalarOpacity.AddPoint(-100, 0.85)
-    volumeScalarOpacity.AddPoint(0, 0.85)
-    volumeScalarOpacity.AddPoint(500, 0.85)
-    volumeScalarOpacity.AddPoint(700, 0.85)
-
-    volumeGradientOpacity.AddPoint(-1000, 0.0)
-    volumeGradientOpacity.AddPoint(-500, 0.0)
-    volumeGradientOpacity.AddPoint(0, 0.6)
-    volumeGradientOpacity.AddPoint(500, 0.85)
-
+from typing import Sequence, Tuple
+
+import numpy as np
+import vtkmodules.vtkCommonCore as vtkCommonCore
+from matplotlib import pyplot as plt
+from vtkmodules.vtkCommonDataModel import vtkPiecewiseFunction
+from vtkmodules.vtkRenderingCore import vtkColorTransferFunction
+
+
+def uniqueColorLT(threshold:float, opacity:float, color:Sequence[float]) -> vtkCommonCore.vtkLookupTable:
+    table = vtkCommonCore.vtkLookupTable()
+    table.SetRange(threshold-1., threshold)  # image intensity range
+    table.SetValueRange(0.0, 1.0)  # from black to white
+    table.SetSaturationRange(0.0, 0.0)  # no color saturation
+    table.SetRampToLinear()
+
+    table.SetNumberOfTableValues(2)
+    table.SetTableValue(0, (0, 0, 0, 0))
+    table.SetTableValue(1, (color[0], color[1], color[2], opacity))
+
+    table.SetBelowRangeColor(0, 0, 0, 0)
+    table.SetUseBelowRangeColor(True)
+    table.SetAboveRangeColor(color[0], color[1], color[2], opacity)
+    table.SetUseAboveRangeColor(True)
+    table.Build()
+
+    return table
+
+def uniqueColorLTTo3DLT(lt:vtkCommonCore.vtkLookupTable) -> Tuple[vtkColorTransferFunction, vtkPiecewiseFunction, vtkPiecewiseFunction]:
+    rangeVal = lt.GetRange()
+    opacity = lt.GetOpacity(rangeVal[1])
+
+    volumeColor = vtkColorTransferFunction()
+    volumeScalarOpacity = vtkPiecewiseFunction()
+    volumeGradientOpacity = vtkPiecewiseFunction()
+
+    volumeScalarOpacity.AddPoint(rangeVal[0], 0.)
+    volumeScalarOpacity.AddPoint(rangeVal[1], opacity)
+
+    volumeGradientOpacity.AddPoint(rangeVal[0], 0.)
+    volumeGradientOpacity.AddPoint(rangeVal[1], opacity)
+
+    tableVals = np.linspace(rangeVal[0], rangeVal[1], lt.GetNumberOfTableValues())
+    for i in range(lt.GetNumberOfTableValues()):
+        tbVal = lt.GetTableValue(i)
+        volumeColor.AddRGBPoint(tableVals[i], tbVal[0], tbVal[1], tbVal[2])
+
+    return volumeColor, volumeScalarOpacity, volumeGradientOpacity
+
+
+def fusionLT(range:Sequence[float], opacity:float, colormap:str) -> vtkCommonCore.vtkLookupTable:
+    table = vtkCommonCore.vtkLookupTable()
+    table.SetRange(range[0], range[1])  # image intensity range
+    table.SetValueRange(0.0, 1.0)  # from black to white
+    table.SetSaturationRange(0.0, 0.0)  # no color saturation
+    table.SetRampToLinear()
+
+    cm = plt.cm.get_cmap(colormap)
+    linInd = list(np.arange(0, 1.01, 0.01))
+
+    table.SetNumberOfTableValues(len(linInd))
+    LastCMVal = (0, 0, 0)
+    for i, ind in enumerate(linInd):
+        cmVal = cm(ind)
+        LastCMVal = cmVal
+        if i==0:
+            table.SetTableValue(i, (cmVal[0], cmVal[1], cmVal[2], 0))
+        else:
+            table.SetTableValue(i, (cmVal[0], cmVal[1], cmVal[2], opacity))
+
+    table.SetBelowRangeColor(0, 0, 0, 0)
+    table.SetUseBelowRangeColor(True)
+    table.SetAboveRangeColor(LastCMVal[0], LastCMVal[1], LastCMVal[2], opacity)
+    table.SetUseAboveRangeColor(True)
+    table.Build()
+
+    return table
+
+def grayLT(range) -> vtkCommonCore.vtkLookupTable:
+    table = vtkCommonCore.vtkLookupTable()
+    table.SetRange(range[0], range[1])  # image intensity range
+    table.SetTableRange(range[0], range[1])  # image intensity range
+    table.SetValueRange(0.0, 1.0)  # from black to white
+    table.SetSaturationRange(0.0, 0.0)  # no color saturation
+    table.SetRampToLinear()
+    table.SetAlpha(1.)
+    table.SetAboveRangeColor(1., 1., 1., 1.)
+    table.SetBelowRangeColor(0., 0., 0., 1.)
+    table.SetUseAboveRangeColor(True)
+    table.SetUseBelowRangeColor(True)
+    table.Build()
+
+    return table
+
+
+def fusionLTTo3DLT(lt:vtkCommonCore.vtkLookupTable) -> Tuple[vtkColorTransferFunction, vtkPiecewiseFunction, vtkPiecewiseFunction]:
+    rangeVal = lt.GetRange()
+    opacity0 = lt.GetOpacity(0)
+    opacity1 = lt.GetOpacity(1)
+
+    volumeColor = vtkColorTransferFunction()
+    volumeScalarOpacity = vtkPiecewiseFunction()
+    volumeGradientOpacity = vtkPiecewiseFunction()
+
+    volumeScalarOpacity.AddPoint(rangeVal[0], opacity0)
+    volumeScalarOpacity.AddPoint((rangeVal[0]+rangeVal[1])/.2, opacity0)
+    volumeScalarOpacity.AddPoint(3*(rangeVal[0] + rangeVal[1]) /4. , opacity1/2.)
+    volumeScalarOpacity.AddPoint(rangeVal[1], opacity1)
+
+    volumeGradientOpacity.AddPoint(rangeVal[0], opacity1)
+    volumeGradientOpacity.AddPoint((rangeVal[0]+rangeVal[1])/2, opacity1/4.)
+    volumeGradientOpacity.AddPoint(3*(rangeVal[0] + rangeVal[1]) /4. , opacity1/2.)
+    volumeGradientOpacity.AddPoint(rangeVal[1], opacity1)
+
+    tableVals = np.linspace(rangeVal[0], rangeVal[1], lt.GetNumberOfTableValues())
+    for i in range(lt.GetNumberOfTableValues()):
+        tbVal = lt.GetTableValue(i)
+        volumeColor.AddRGBPoint(tableVals[i], tbVal[0], tbVal[1], tbVal[2])
+
+    return volumeColor, volumeScalarOpacity, volumeGradientOpacity
+
+def ct3DLT() -> Tuple[vtkColorTransferFunction, vtkPiecewiseFunction, vtkPiecewiseFunction]:
+    volumeColor = vtkColorTransferFunction()
+    volumeScalarOpacity = vtkPiecewiseFunction()
+    volumeGradientOpacity = vtkPiecewiseFunction()
+
+    volumeColor.AddRGBPoint(-1000, 0.0, 0.0, 0.0)
+    volumeColor.AddRGBPoint(-500, 240.0/255.0, 184.0/255.0, 160.0/255.0)
+    volumeColor.AddRGBPoint(0, 232/255, 147/255, 132/255)
+    volumeColor.AddRGBPoint(500, 1.0, 1.0, 240.0 / 255.0)
+    volumeColor.AddRGBPoint(700,  242/255, 220/255, 172/255)
+    volumeColor.AddRGBPoint(1800, 173/255, 166/255, 166/255)
+    volumeColor.AddRGBPoint(2500, 237/255, 171/255, 64/255)
+
+    volumeScalarOpacity.AddPoint(-1000, 0.00)
+    volumeScalarOpacity.AddPoint(-500, 0.05)
+    volumeScalarOpacity.AddPoint(-200, 0.5)
+    volumeScalarOpacity.AddPoint(-100, 0.85)
+    volumeScalarOpacity.AddPoint(0, 0.85)
+    volumeScalarOpacity.AddPoint(500, 0.85)
+    volumeScalarOpacity.AddPoint(700, 0.85)
+
+    volumeGradientOpacity.AddPoint(-1000, 0.0)
+    volumeGradientOpacity.AddPoint(-500, 0.0)
+    volumeGradientOpacity.AddPoint(0, 0.6)
+    volumeGradientOpacity.AddPoint(500, 0.85)
+
     return volumeColor, volumeScalarOpacity, volumeGradientOpacity
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/polyData3DLayer_3D.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/polyData3DLayer_3D.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from typing import Optional
-
-from vtkmodules.vtkCommonColor import vtkNamedColors
-from vtkmodules.vtkRenderingCore import vtkPolyDataMapper, vtkActor
-
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-
-
-class PolyData3DLayer_3D:
-    def __init__(self, renderer, renderWindow):
-        self.imageChangedSignal = Event(object)
-
-        self._image = None
-        self._imageToBeSet = None
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-
-        self._mainActor = vtkActor()
-        self._mainMapper = vtkPolyDataMapper()
-        self._mainActor.SetMapper(self._mainMapper)
-
-    def close(self):
-        self._disconnectAll()
-        self._renderer.RemoveActor(self._mainActor)
-        self._mainMapper.RemoveAllInputs()
-
-    def update(self):
-        self._setImage(self._imageToBeSet)
-
-    @property
-    def image(self) -> Optional[Image3DForViewer]:
-        """
-        Image displayed
-        :type:Optional[Image3DForViewer]
-        """
-        if self._image is None:
-            return None
-
-        return self._image
-
-    @image.setter
-    def image(self, image:Optional[GenericImageForViewer]):
-        if image == self._image:
-            return
-
-        if not (isinstance(image, GenericImageForViewer) or (image is None)):
-            return
-
-        self._imageToBeSet = image
-
-    def _setImage(self, image:Optional[GenericImageForViewer]):
-        self._image = image
-
-        self._disconnectAll()
-        self._renderer.RemoveActor(self._mainActor)
-        self._mainMapper.RemoveAllInputs()
-
-        if not (self._image is None):
-            self._mainMapper.SetInputConnection(self._image.vtkOutputPort)
-
-            self._renderer.AddActor(self._mainActor)
-
-            colors = vtkNamedColors()
-            #backFaceProp = vtkProperty()
-            #backFaceProp.SetDiffuseColor(colors.GetColor3d("Silver"))
-            #self._mainActor.SetBackfaceProperty(backFaceProp)
-            self._mainActor.GetProperty().SetDiffuseColor(colors.GetColor3d("NavajoWhite"))
-
-            self._connectAll()
-
-        self.imageChangedSignal.emit(self._image)
-
-        self._renderWindow.Render()
-
-
-    def _connectAll(self):
-        self._image.dataChangedSignal.connect(self._render)
-
-    def _disconnectAll(self):
-        if self._image is None:
-            return
-
-        self._image.dataChangedSignal.disconnect(self._render)
-
-    def _render(self, *args):
-        self._renderWindow.Render()
+from typing import Optional
+
+from vtkmodules.vtkCommonColor import vtkNamedColors
+from vtkmodules.vtkRenderingCore import vtkPolyDataMapper, vtkActor
+
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+
+
+class PolyData3DLayer_3D:
+    def __init__(self, renderer, renderWindow):
+        self.imageChangedSignal = Event(object)
+
+        self._image = None
+        self._imageToBeSet = None
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+
+        self._mainActor = vtkActor()
+        self._mainMapper = vtkPolyDataMapper()
+        self._mainActor.SetMapper(self._mainMapper)
+
+    def close(self):
+        self._disconnectAll()
+        self._renderer.RemoveActor(self._mainActor)
+        self._mainMapper.RemoveAllInputs()
+
+    def update(self):
+        self._setImage(self._imageToBeSet)
+
+    @property
+    def image(self) -> Optional[Image3DForViewer]:
+        """
+        Image displayed
+        :type:Optional[Image3DForViewer]
+        """
+        if self._image is None:
+            return None
+
+        return self._image
+
+    @image.setter
+    def image(self, image:Optional[GenericImageForViewer]):
+        if image == self._image:
+            return
+
+        if not (isinstance(image, GenericImageForViewer) or (image is None)):
+            return
+
+        self._imageToBeSet = image
+
+    def _setImage(self, image:Optional[GenericImageForViewer]):
+        self._image = image
+
+        self._disconnectAll()
+        self._renderer.RemoveActor(self._mainActor)
+        self._mainMapper.RemoveAllInputs()
+
+        if not (self._image is None):
+            self._mainMapper.SetInputConnection(self._image.vtkOutputPort)
+
+            self._renderer.AddActor(self._mainActor)
+
+            colors = vtkNamedColors()
+            #backFaceProp = vtkProperty()
+            #backFaceProp.SetDiffuseColor(colors.GetColor3d("Silver"))
+            #self._mainActor.SetBackfaceProperty(backFaceProp)
+            self._mainActor.GetProperty().SetDiffuseColor(colors.GetColor3d("NavajoWhite"))
+
+            self._connectAll()
+
+        self.imageChangedSignal.emit(self._image)
+
+        self._renderWindow.Render()
+
+
+    def _connectAll(self):
+        self._image.dataChangedSignal.connect(self._render)
+
+    def _disconnectAll(self):
+        if self._image is None:
+            return
+
+        self._image.dataChangedSignal.disconnect(self._render)
+
+    def _render(self, *args):
+        self._renderWindow.Render()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer_3D.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/primaryImage3DLayer_3D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-from typing import Optional
-
-import vtkmodules.vtkRenderingCore as vtkRenderingCore
-from vtkmodules.vtkRenderingVolumeOpenGL2 import vtkSmartVolumeMapper
-
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables import ct3DLT
-
-
-class PrimaryImage3DLayer_3D:
-    def __init__(self, renderer, renderWindow, iStyle):
-        self.imageChangedSignal = Event(object)
-
-        self._image = None
-        self._imageToBeSet = None
-        self._iStyle = iStyle
-        self._mainActor = vtkRenderingCore.vtkVolume()
-        self._mainMapper = vtkSmartVolumeMapper()
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-
-        self._mainActor.SetMapper(self._mainMapper)
-
-        self._volumeColor, self._volumeScalarOpacity, self._volumeGradientOpacity = ct3DLT()
-
-        self._volumeProperty = vtkRenderingCore.vtkVolumeProperty()
-        self._volumeProperty.SetColor(self._volumeColor)
-        self._volumeProperty.SetScalarOpacity(self._volumeScalarOpacity)
-        self._volumeProperty.SetGradientOpacity(self._volumeGradientOpacity)
-        self._volumeProperty.SetInterpolationTypeToLinear()
-        self._volumeProperty.ShadeOn()
-        self._volumeProperty.SetAmbient(0.4)
-        self._volumeProperty.SetDiffuse(0.6)
-        self._volumeProperty.SetSpecular(0.2)
-
-    def close(self):
-        self._disconnectAll()
-        self._renderer.RemoveActor(self._mainActor)
-        self._mainMapper.RemoveAllInputs()
-
-    def update(self):
-        self._setImage(self._imageToBeSet)
-
-    @property
-    def image(self) -> Optional[Image3DForViewer]:
-        return self._imageToBeSet
-
-    @image.setter
-    def image(self, image:Optional[GenericImageForViewer]):
-        if image == self._imageToBeSet:
-            return
-
-        self._imageToBeSet = image
-
-    def _setImage(self, image:Optional[GenericImageForViewer]):
-        self._image = image
-
-        self._disconnectAll()
-        self._renderer.RemoveActor(self._mainActor)
-        self._mainMapper.RemoveAllInputs()
-
-        if not (self._image is None):
-            self._mainMapper.SetInputConnection(self._image.vtkOutputPort)
-
-            self._renderer.AddActor(self._mainActor)
-
-            self._mainActor.SetProperty(self._volumeProperty)
-
-            self._connectAll()
-
-            self._renderer.ResetCamera()
-
-        self.imageChangedSignal.emit(self._image)
-
-        self._renderWindow.Render()
-
-    def _connectAll(self):
-        self._image.dataChangedSignal.connect(self._render)
-        self._image.lookupTableChangedSignal.connect(self._updateLookupTable)
-
-    def _disconnectAll(self):
-        if self._image is None:
-            return
-
-        self._image.dataChangedSignal.disconnect(self._render)
-        self._image.lookupTableChangedSignal.disconnect(self._updateLookupTable)
-
-    def _render(self, *args):
-        self._renderWindow.Render()
-
-    def _updateLookupTable(self, lt):
-        pass
+from typing import Optional
+
+import vtkmodules.vtkRenderingCore as vtkRenderingCore
+from vtkmodules.vtkRenderingVolumeOpenGL2 import vtkSmartVolumeMapper
+
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables import ct3DLT
+
+
+class PrimaryImage3DLayer_3D:
+    def __init__(self, renderer, renderWindow, iStyle):
+        self.imageChangedSignal = Event(object)
+
+        self._image = None
+        self._imageToBeSet = None
+        self._iStyle = iStyle
+        self._mainActor = vtkRenderingCore.vtkVolume()
+        self._mainMapper = vtkSmartVolumeMapper()
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+
+        self._mainActor.SetMapper(self._mainMapper)
+
+        self._volumeColor, self._volumeScalarOpacity, self._volumeGradientOpacity = ct3DLT()
+
+        self._volumeProperty = vtkRenderingCore.vtkVolumeProperty()
+        self._volumeProperty.SetColor(self._volumeColor)
+        self._volumeProperty.SetScalarOpacity(self._volumeScalarOpacity)
+        self._volumeProperty.SetGradientOpacity(self._volumeGradientOpacity)
+        self._volumeProperty.SetInterpolationTypeToLinear()
+        self._volumeProperty.ShadeOn()
+        self._volumeProperty.SetAmbient(0.4)
+        self._volumeProperty.SetDiffuse(0.6)
+        self._volumeProperty.SetSpecular(0.2)
+
+    def close(self):
+        self._disconnectAll()
+        self._renderer.RemoveActor(self._mainActor)
+        self._mainMapper.RemoveAllInputs()
+
+    def update(self):
+        self._setImage(self._imageToBeSet)
+
+    @property
+    def image(self) -> Optional[Image3DForViewer]:
+        return self._imageToBeSet
+
+    @image.setter
+    def image(self, image:Optional[GenericImageForViewer]):
+        if image == self._imageToBeSet:
+            return
+
+        self._imageToBeSet = image
+
+    def _setImage(self, image:Optional[GenericImageForViewer]):
+        if self._image == self._imageToBeSet:
+            return
+
+        self._image = image
+
+        self._disconnectAll()
+        self._renderer.RemoveActor(self._mainActor)
+        self._mainMapper.RemoveAllInputs()
+
+        if not (self._image is None):
+            self._mainMapper.SetInputConnection(self._image.vtkOutputPort)
+
+            self._renderer.AddActor(self._mainActor)
+
+            self._mainActor.SetProperty(self._volumeProperty)
+
+            self._connectAll()
+
+            self._renderer.ResetCamera()
+
+        self.imageChangedSignal.emit(self._image)
+
+        self._renderWindow.Render()
+
+    def _connectAll(self):
+        self._image.dataChangedSignal.connect(self._render)
+        self._image.lookupTableChangedSignal.connect(self._updateLookupTable)
+
+    def _disconnectAll(self):
+        if self._image is None:
+            return
+
+        self._image.dataChangedSignal.disconnect(self._render)
+        self._image.lookupTableChangedSignal.disconnect(self._updateLookupTable)
+
+    def _render(self, *args):
+        self._renderWindow.Render()
+
+    def _updateLookupTable(self, lt):
+        pass
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtplanLayer_3D.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/rtplanLayer_3D.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import os.path
-from typing import Optional
-
-from vtkmodules.vtkCommonTransforms import vtkTransform
-from vtkmodules.vtkFiltersGeneral import vtkTransformPolyDataFilter
-from vtkmodules.vtkIOGeometry import vtkSTLReader
-
-from opentps.core.data.plan import RTPlan, PlanIonBeam
-from opentps.gui.viewer.dataForViewer.polyDataForViewer import PolyDataForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.polyData3DLayer_3D import PolyData3DLayer_3D
-
-
-class BeamLayer_3D:
-    def __init__(self, renderer, renderWindow):
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-
-        self._nozzleLayer = PolyData3DLayer_3D(self._renderer, self._renderWindow)
-
-        altPath = '/home/sylvain/Downloads/Universal_nozzle_cover.stl'
-        filePath = os.path.join(altPath) #iconModule.__path__[0], 'iba_nozzle.stl')
-        self._stlReader = vtkSTLReader()
-        self._stlReader.SetFileName(filePath)
-        self._tformFilter = vtkTransformPolyDataFilter()
-        self._tformFilter.SetTransform(self._tform(0, 0))
-        self._tformFilter.SetInputConnection(self._stlReader.GetOutputPort())
-        self._image = PolyDataForViewer(self._tformFilter)
-
-    def close(self):
-        self._nozzleLayer.close()
-        self._tformFilter.RemoveAllInputs()
-
-    def update(self):
-        self._nozzleLayer.update()
-
-    def _tform(self, gantryAngle, couchAngle):
-        #TODO couchAngle
-        tform = vtkTransform()
-        tform.RotateY(-90)
-        #tform.RotateY(90)
-        tform.RotateZ(180)
-        #tform.RotateX(90 + gantryAngle)
-        tform.RotateX(180-gantryAngle)
-        tform.Translate(0, 0, 0)
-
-        return tform
-
-    def setBeam(self, beam:PlanIonBeam):
-        self._tformFilter.SetTransform(self._tform(beam.gantryAngle, beam.couchAngle))
-        self._nozzleLayer.image = self._image
-
-class RTPlanLayer_3D:
-    def __init__(self, renderer, renderWindow):
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-
-        self._beamLayers = []
-        self._plan = None
-
-    def close(self):
-        for bLayer in self._beamLayers:
-            bLayer.close()
-
-        self._beamLayers = []
-
-        self._renderWindow.Render()
-
-    def update(self):
-        for bl in self._beamLayers:
-            bl.update()
-
-    @property
-    def plan(self) -> Optional[RTPlan]:
-        return self._plan
-
-    def setPlan(self, plan:RTPlan):
-        #TODO connect to plan.dataChangedSignal
-        if plan is None:
-            self._plan = None
-            self.close()
-            return
-        elif self._plan == plan:
-            return
-
-        self._plan = plan
-
-        self.close()
-
-        for beam in plan:
-            bLayer = BeamLayer_3D(self._renderer, self._renderWindow)
-            bLayer.setBeam(beam)
-            self._beamLayers.append(bLayer)
-
-        self._renderer.ResetCamera()
+import os.path
+from typing import Optional
+
+from vtkmodules.vtkCommonTransforms import vtkTransform
+from vtkmodules.vtkFiltersGeneral import vtkTransformPolyDataFilter
+from vtkmodules.vtkIOGeometry import vtkSTLReader
+
+from opentps.core.data.plan import RTPlan, PlanIonBeam
+from opentps.gui.viewer.dataForViewer.polyDataForViewer import PolyDataForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.polyData3DLayer_3D import PolyData3DLayer_3D
+
+
+class BeamLayer_3D:
+    def __init__(self, renderer, renderWindow):
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+
+        self._nozzleLayer = PolyData3DLayer_3D(self._renderer, self._renderWindow)
+
+        altPath = '/home/sylvain/Downloads/Universal_nozzle_cover.stl'
+        filePath = os.path.join(altPath) #iconModule.__path__[0], 'iba_nozzle.stl')
+        self._stlReader = vtkSTLReader()
+        self._stlReader.SetFileName(filePath)
+        self._tformFilter = vtkTransformPolyDataFilter()
+        self._tformFilter.SetTransform(self._tform(0, 0))
+        self._tformFilter.SetInputConnection(self._stlReader.GetOutputPort())
+        self._image = PolyDataForViewer(self._tformFilter)
+
+    def close(self):
+        self._nozzleLayer.close()
+        self._tformFilter.RemoveAllInputs()
+
+    def update(self):
+        self._nozzleLayer.update()
+
+    def _tform(self, gantryAngle, couchAngle):
+        #TODO couchAngle
+        tform = vtkTransform()
+        tform.RotateY(-90)
+        #tform.RotateY(90)
+        tform.RotateZ(180)
+        #tform.RotateX(90 + gantryAngle)
+        tform.RotateX(180-gantryAngle)
+        tform.Translate(0, 0, 0)
+
+        return tform
+
+    def setBeam(self, beam:PlanIonBeam):
+        self._tformFilter.SetTransform(self._tform(beam.gantryAngle, beam.couchAngle))
+        self._nozzleLayer.image = self._image
+
+class RTPlanLayer_3D:
+    def __init__(self, renderer, renderWindow):
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+
+        self._beamLayers = []
+        self._plan = None
+
+    def close(self):
+        for bLayer in self._beamLayers:
+            bLayer.close()
+
+        self._beamLayers = []
+
+        self._renderWindow.Render()
+
+    def update(self):
+        for bl in self._beamLayers:
+            bl.update()
+
+    @property
+    def plan(self) -> Optional[RTPlan]:
+        return self._plan
+
+    def setPlan(self, plan:RTPlan):
+        #TODO connect to plan.dataChangedSignal
+        if plan is None:
+            self._plan = None
+            self.close()
+            return
+        elif self._plan == plan:
+            return
+
+        self._plan = plan
+
+        self.close()
+
+        for beam in plan:
+            bLayer = BeamLayer_3D(self._renderer, self._renderWindow)
+            bLayer.setBeam(beam)
+            self._beamLayers.append(bLayer)
+
+        self._renderer.ResetCamera()
         self._renderWindow.Render()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage2DLayer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,99 +1,98 @@
-from typing import Optional, Sequence
-
-from vtkmodules import vtkImagingCore
-from vtkmodules.vtkInteractionWidgets import vtkScalarBarWidget
-from vtkmodules.vtkRenderingAnnotation import vtkScalarBarActor
-
-from opentps.core import Event
-from opentps.gui.viewer.dataForViewer.image2DForViewer import Image2DForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage2DLayer import PrimaryImage2DLayer
-
-
-class SecondaryImage2DLayer(PrimaryImage2DLayer):
-    def __init__(self, renderer, renderWindow, iStyle):
-        self._colorMapper = vtkImagingCore.vtkImageMapToColors()
-
-        super().__init__(renderer, renderWindow, iStyle)
-
-        self.colorbarVisibilitySignal = Event(bool)
-        self.lookupTableChangedSignal = Event(bool)
-
-        self._colorbarActor = vtkScalarBarActor()
-        self._colorbarWidget = vtkScalarBarWidget()
-
-        self._colorbarActor.SetNumberOfLabels(5)
-        self._colorbarActor.SetOrientationToVertical()
-        self._colorbarActor.SetVisibility(False)
-        self._colorbarActor.SetUnconstrainedFontSize(14)
-        self._colorbarActor.SetMaximumWidthInPixels(20)
-
-        self._colorbarWidget.SetInteractor(self._renderWindow.GetInteractor())
-        self._colorbarWidget.SetScalarBarActor(self._colorbarActor)
-
-    def _setMainMapperInputConnection(self):
-        # self._colorMapper.SetInputConnection(self._reslice.GetOutputPort())
-        self._mainMapper.SetInputConnection(self._colorMapper.GetOutputPort())
-
-    def close(self):
-        super().close()
-
-    def _setImage(self, image: Optional[Image2DForViewer]):
-        if image == self._image:
-            return
-
-        super()._setImage(image)
-
-        if image is None:
-            self.colorbarOn = False
-        else:
-            self.colorbarOn = True # TODO: Get this from parent
-
-        self._renderWindow.Render()
-
-    @property
-    def colorbarOn(self) -> bool:
-        """
-        Colorbar visibility
-        :type: bool
-        """
-        return self._colorbarActor.GetVisibility()
-
-    @colorbarOn.setter
-    def colorbarOn(self, visible: bool):
-        if visible==self._colorbarActor.GetVisibility():
-            return
-
-        if visible:
-            self._colorbarActor.SetVisibility(True)
-            self._colorbarWidget.On()
-        else:
-            self._colorbarActor.SetVisibility(False)
-            self._colorbarWidget.Off()
-
-        self.colorbarVisibilitySignal.emit(visible)
-
-        self._renderWindow.Render()
-
-    def _connectAll(self):
-        super()._connectAll()
-
-    def _disconnectAll(self):
-        super()._disconnectAll()
-
-        if self._image is None:
-            return
-
-    def _setLookupTable(self):
-        self._image.lookupTableName = 'jet'
-        self._colorMapper.SetLookupTable(self._image.lookupTable)
-        self._colorbarActor.SetLookupTable(self._image.lookupTable)
-
-    def _updateLookupTable(self, lt):
-        self._colorMapper.SetLookupTable(lt)
-        self._colorbarActor.SetLookupTable(lt)
-
-        self._renderWindow.Render()
-
-    def _setWWL(self, wwl: Sequence):
-        # WWL is changed via iStyle. It is only working on the primary image.
-        pass
+from typing import Optional, Sequence
+
+from vtkmodules import vtkImagingCore
+from vtkmodules.vtkInteractionWidgets import vtkScalarBarWidget
+from vtkmodules.vtkRenderingAnnotation import vtkScalarBarActor
+
+from opentps.core import Event
+from opentps.gui.viewer.dataForViewer.image3DForViewer import Image3DForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer import PrimaryImage3DLayer
+
+
+class SecondaryImage3DLayer(PrimaryImage3DLayer):
+    def __init__(self, renderer, renderWindow, iStyle):
+        self._colorMapper = vtkImagingCore.vtkImageMapToColors()
+
+        super().__init__(renderer, renderWindow, iStyle)
+
+        self.colorbarVisibilitySignal = Event(bool)
+        self.lookupTableChangedSignal = Event(bool)
+
+        self._colorbarActor = vtkScalarBarActor()
+        self._colorbarWidget = vtkScalarBarWidget()
+
+        self._colorbarActor.SetNumberOfLabels(5)
+        self._colorbarActor.SetOrientationToVertical()
+        self._colorbarActor.SetVisibility(False)
+        self._colorbarActor.SetUnconstrainedFontSize(14)
+        self._colorbarActor.SetMaximumWidthInPixels(20)
+
+        self._colorbarWidget.SetInteractor(self._renderWindow.GetInteractor())
+        self._colorbarWidget.SetScalarBarActor(self._colorbarActor)
+
+    def _setMainMapperInputConnection(self):
+        self._colorMapper.SetInputConnection(self._reslice.GetOutputPort())
+        self._mainMapper.SetInputConnection(self._colorMapper.GetOutputPort())
+
+    def close(self):
+        super().close()
+
+    def _setImage(self, image: Optional[Image3DForViewer]):
+        if image == self._image:
+            return
+
+        super()._setImage(image)
+
+        if image is None:
+            self.colorbarOn = False
+        else:
+            self._image.lookupTableName = 'jet'
+            self.colorbarOn = True # TODO: Get this from parent
+
+        self._renderWindow.Render()
+
+    @property
+    def colorbarOn(self) -> bool:
+        """
+        Colorbar visibility
+        :type: bool
+        """
+        return self._colorbarActor.GetVisibility()
+
+    @colorbarOn.setter
+    def colorbarOn(self, visible: bool):
+        if visible==self._colorbarActor.GetVisibility():
+            return
+
+        if visible:
+            self._colorbarActor.SetVisibility(True)
+            self._colorbarWidget.On()
+        else:
+            self._colorbarActor.SetVisibility(False)
+            self._colorbarWidget.Off()
+
+        self.colorbarVisibilitySignal.emit(visible)
+
+        self._renderWindow.Render()
+
+    def _connectAll(self):
+        super()._connectAll()
+
+    def _disconnectAll(self):
+        super()._disconnectAll()
+
+        if self._image is None:
+            return
+
+    def _setLookupTable(self):
+        self._updateLookupTable(self._image.lookupTable)
+
+    def _updateLookupTable(self, lt):
+        self._colorMapper.SetLookupTable(lt)
+        self._colorbarActor.SetLookupTable(lt)
+
+        self._renderWindow.Render()
+
+    def _setWWL(self, wwl: Sequence):
+        # WWL is changed via iStyle. It is only working on the primary image.
+        pass
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer_3D.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/imageViewerComponents/secondaryImage3DLayer_3D.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Optional
-
-import vtkmodules.vtkRenderingCore as vtkRenderingCore
-
-from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables import fusionLTTo3DLT
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer_3D import PrimaryImage3DLayer_3D
-
-
-class SecondaryImage3DLayer_3D(PrimaryImage3DLayer_3D):
-    def __init__(self, renderer, renderWindow, iStyle):
-        super().__init__(renderer, renderWindow, iStyle)
-
-        self._volumeProperty = vtkRenderingCore.vtkVolumeProperty()
-        self._volumeProperty.SetInterpolationTypeToLinear()
-        self._volumeProperty.ShadeOn()
-        self._volumeProperty.SetAmbient(0.4)
-        self._volumeProperty.SetDiffuse(0.6)
-        self._volumeProperty.SetSpecular(0.2)
-
-
-    def _setImage(self, image:Optional[GenericImageForViewer]):
-        super()._setImage(image)
-
-        if not (self._image is None):
-            self._updateLookupTable(self._image.lookupTable)
-
-    def _updateLookupTable(self, lt):
-        volumeColor, volumeScalarOpacity, volumeGradientOpacity = fusionLTTo3DLT(lt)
-        self._volumeProperty.SetColor(volumeColor)
-        self._volumeProperty.SetScalarOpacity(volumeScalarOpacity)
-        self._volumeProperty.SetGradientOpacity(volumeGradientOpacity)
-
-        self._renderWindow.Render()
+from typing import Optional
+
+import vtkmodules.vtkRenderingCore as vtkRenderingCore
+
+from opentps.gui.viewer.dataForViewer.genericImageForViewer import GenericImageForViewer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.lookupTables import fusionLTTo3DLT
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer_3D import PrimaryImage3DLayer_3D
+
+
+class SecondaryImage3DLayer_3D(PrimaryImage3DLayer_3D):
+    def __init__(self, renderer, renderWindow, iStyle):
+        super().__init__(renderer, renderWindow, iStyle)
+
+        self._volumeProperty = vtkRenderingCore.vtkVolumeProperty()
+        self._volumeProperty.SetInterpolationTypeToLinear()
+        self._volumeProperty.ShadeOn()
+        self._volumeProperty.SetAmbient(0.4)
+        self._volumeProperty.SetDiffuse(0.6)
+        self._volumeProperty.SetSpecular(0.2)
+
+
+    def _setImage(self, image:Optional[GenericImageForViewer]):
+        super()._setImage(image)
+
+        if not (self._image is None):
+            self._updateLookupTable(self._image.lookupTable)
+
+    def _updateLookupTable(self, lt):
+        volumeColor, volumeScalarOpacity, volumeGradientOpacity = fusionLTTo3DLT(lt)
+        self._volumeProperty.SetColor(volumeColor)
+        self._volumeProperty.SetScalarOpacity(volumeScalarOpacity)
+        self._volumeProperty.SetGradientOpacity(volumeGradientOpacity)
+
+        self._renderWindow.Render()
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/patientDataPropertyEditor.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/patientDataPropertyEditor.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import functools
-import inspect
-import typing
-
-from PyQt5.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, QPushButton, QMainWindow
-
-from opentps.core.data.plan import PlanIonBeam
-from opentps.core.data.plan import PlanIonLayer
-from opentps.core.data.plan import PlanIonSpot
-from opentps.core.data.plan import RangeShifter
-from opentps.core.data import PatientData
-from opentps.core import Event
-
-class PatientDataPropertyEditor(QWidget):
-    def __init__(self, image, parent=None):
-        super().__init__(parent=parent)
-
-        self._mainLayout = QVBoxLayout(self)
-        self.setLayout(self._mainLayout)
-
-        for property in inspect.getmembers(image):
-            # to remove private and protected
-            # functions
-            if not property[0].startswith('_'):
-                # To remove other methods that
-                # does not start with an underscore
-                if not inspect.ismethod(property[1]):
-                    if not isinstance(property[1], Event):
-                        self._mainLayout.addWidget(TwoRowElement(property, parent=self))
-
-
-class TwoRowElement(QWidget):
-    def __init__(self, property, parent=None):
-        super().__init__(parent)
-
-        self._mainLayout = QHBoxLayout(self)
-        self.setLayout(self._mainLayout)
-
-        self._txt = QLabel(self)
-        self._txt.setText(property[0])
-
-        self._mainLayout.addWidget(self._txt)
-
-        val = property[1]
-
-        if isinstance(val, self.supportedTypes()):
-            val = [val]
-
-        if isinstance(val, typing.Sequence) and len(val)>0 and isinstance(val[0], self.supportedTypes()):
-            for valElement in val:
-                patientDataButton = QPushButton(self)
-                patientDataButton.setText(str(valElement.__class__.__name__))
-                patientDataButton.clicked.connect(functools.partial(self._openPatientData, valElement))
-                self._mainLayout.addWidget(patientDataButton)
-        else:
-            self._nameLineEdit = QLineEdit(self)
-            self._nameLineEdit.setText(str(val))
-            self._txt.setBuddy(self._nameLineEdit)
-            self._mainLayout.addWidget(self._nameLineEdit)
-
-        self._mainLayout.addStretch()
-
-    def _openPatientData(self, patientData:PatientData):
-        w = QMainWindow(self.parent().parent())
-        w.setWindowTitle('Image info')
-        w.resize(400, 400)
-        w.setCentralWidget(PatientDataPropertyEditor(patientData, self.parent().parent()))
-        w.show()
-
-    def supportedTypes(self):
+import functools
+import inspect
+import typing
+
+from PyQt5.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, QPushButton, QMainWindow
+
+from opentps.core.data.plan import PlanIonBeam
+from opentps.core.data.plan import PlanIonLayer
+from opentps.core.data.plan import PlanIonSpot
+from opentps.core.data.plan import RangeShifter
+from opentps.core.data import PatientData
+from opentps.core import Event
+
+class PatientDataPropertyEditor(QWidget):
+    def __init__(self, image, parent=None):
+        super().__init__(parent=parent)
+
+        self._mainLayout = QVBoxLayout(self)
+        self.setLayout(self._mainLayout)
+
+        for property in inspect.getmembers(image):
+            # to remove private and protected
+            # functions
+            if not property[0].startswith('_'):
+                # To remove other methods that
+                # does not start with an underscore
+                if not inspect.ismethod(property[1]):
+                    if not isinstance(property[1], Event):
+                        self._mainLayout.addWidget(TwoRowElement(property, parent=self))
+
+
+class TwoRowElement(QWidget):
+    def __init__(self, property, parent=None):
+        super().__init__(parent)
+
+        self._mainLayout = QHBoxLayout(self)
+        self.setLayout(self._mainLayout)
+
+        self._txt = QLabel(self)
+        self._txt.setText(property[0])
+
+        self._mainLayout.addWidget(self._txt)
+
+        val = property[1]
+
+        if isinstance(val, self.supportedTypes()):
+            val = [val]
+
+        if isinstance(val, typing.Sequence) and len(val)>0 and isinstance(val[0], self.supportedTypes()):
+            for valElement in val:
+                patientDataButton = QPushButton(self)
+                patientDataButton.setText(str(valElement.__class__.__name__))
+                patientDataButton.clicked.connect(functools.partial(self._openPatientData, valElement))
+                self._mainLayout.addWidget(patientDataButton)
+        else:
+            self._nameLineEdit = QLineEdit(self)
+            self._nameLineEdit.setText(str(val))
+            self._txt.setBuddy(self._nameLineEdit)
+            self._mainLayout.addWidget(self._nameLineEdit)
+
+        self._mainLayout.addStretch()
+
+    def _openPatientData(self, patientData:PatientData):
+        w = QMainWindow(self.parent().parent())
+        w.setWindowTitle('Image info')
+        w.resize(400, 400)
+        w.setCentralWidget(PatientDataPropertyEditor(patientData, self.parent().parent()))
+        w.show()
+
+    def supportedTypes(self):
         return typing.Union[PatientData, PlanIonBeam, PlanIonLayer, PlanIonSpot, RangeShifter].__args__
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dataViewerComponents/profileWidget.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dataViewerComponents/profileWidget.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import typing
-from math import sqrt
-
-import numpy as np
-from pyqtgraph import mkPen
-from vtkmodules.vtkInteractionWidgets import vtkLineWidget2
-
-from opentps.core import Event
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
-from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer import PrimaryImage3DLayer
-
-
-class ProfileWidget:
-    class ProfileWidgetCallback:
-        def __init__(self):
-            self._setPrimaryImageData = lambda *args, **kwargs: None
-            self._setSecondaryImageData = lambda *args, **kwargs: None
-            self._setContourData = lambda *args, **kwargs: None
-
-        @property
-        def setPrimaryImageData(self):
-            return self._setPrimaryImageData
-
-        @setPrimaryImageData.setter
-        def setPrimaryImageData(self, func):
-            self._setPrimaryImageData = func
-
-        @property
-        def setSecondaryImageData(self):
-            return self._setSecondaryImageData
-
-        @setSecondaryImageData.setter
-        def setSecondaryImageData(self, func):
-            self._setSecondaryImageData = func
-
-        @property
-        def setContourData(self):
-            return self._setContourData
-
-        @setContourData.setter
-        def setContourData(self, func):
-            self._setContourData = func
-
-    def __init__(self, renderer, renderWindow):
-        self.lineWidgeEnabledSignal = Event(bool)
-
-        self._lineWidget = vtkLineWidget2()
-        self._lineWidgetCallback = None
-        self._lineWidgetEnabled = False
-        self._primaryLayer = None
-        self._secondaryLayer = None
-        self._contourLayer = None
-        self._renderer = renderer
-        self._renderWindow = renderWindow
-
-        self._lineWidget.SetCurrentRenderer(self._renderer)
-        self._lineWidget.AddObserver("InteractionEvent", self.onProfileWidgetInteraction)
-        self._lineWidget.AddObserver("EndInteractionEvent", self.onProfileWidgetInteraction)
-        self._lineWidget.SetInteractor(self._renderWindow.GetInteractor())
-
-    @property
-    def enabled(self) -> bool:
-        return self._lineWidgetEnabled
-
-    @enabled.setter
-    def enabled(self, enabled: bool):
-        if enabled == self._lineWidgetEnabled:
-            return
-
-        if enabled:
-            self._lineWidget.On()
-            self._lineWidget.GetLineRepresentation().SetLineColor(1, 0, 0)
-            self._lineWidgetEnabled = True
-        else:
-            self._lineWidget.Off()
-            self._lineWidgetEnabled = False
-            self._renderWindow.Render()
-
-        self.lineWidgeEnabledSignal.emit(self._lineWidgetEnabled)
-
-    @property
-    def callback(self):
-        return self._lineWidgetCallback
-
-    @callback.setter
-    def callback(self, method):
-        self._lineWidgetCallback = method
-
-    @property
-    def primaryLayer(self):
-        return self._primaryLayer
-
-    @primaryLayer.setter
-    def primaryLayer(self, layer):
-        self._primaryLayer = layer
-
-        if isinstance(self._primaryLayer, PrimaryImage3DLayer):
-            if not self._primaryLayer.image is None:
-                self._primaryLayer._reslice.RemoveObserver(self._endEventObserver)
-
-            self._endEventObserver = self._primaryLayer._reslice.AddObserver("EndEvent", self.onProfileWidgetInteraction)
-
-    @property
-    def secondaryLayer(self):
-        return self._secondaryLayer
-
-    @secondaryLayer.setter
-    def secondaryLayer(self, layer):
-        self._secondaryLayer = layer
-
-    @property
-    def contourLayer(self):
-        return self._secondaryLayer
-
-    @contourLayer.setter
-    def contourLayer(self, layer):
-        self._contourLayer = layer
-
-    def setInitialPosition(self, worldPos: typing.Sequence):
-        self._lineWidget.GetLineRepresentation().SetPoint1WorldPosition((worldPos[0], worldPos[1], 0.01))
-        self._lineWidget.GetLineRepresentation().SetPoint2WorldPosition((worldPos[0], worldPos[1], 0.01))
-
-    def onProfileWidgetInteraction(self, obj, event):
-        if not self.enabled:
-            return
-
-        point1 = self._lineWidget.GetLineRepresentation().GetPoint1WorldPosition()
-        point2 = self._lineWidget.GetLineRepresentation().GetPoint2WorldPosition()
-
-        if point1[1]==point1[2]==point2[1]==point2[2]:
-            return
-
-        matrix = self._primaryLayer.resliceAxes
-        point1 = matrix.MultiplyPoint((point1[0], point1[1], 0, 1))
-        point2 = matrix.MultiplyPoint((point2[0], point2[1], 0, 1))
-
-        x, y = self._resliceLayerDataBewteenTwoPoints(self._primaryLayer, point1, point2)
-        self._lineWidgetCallback.setPrimaryImageData(x, y, name=self._layerImageName(self._primaryLayer))
-
-        x, y = self._resliceLayerDataBewteenTwoPoints(self._secondaryLayer, point1, point2)
-        self._lineWidgetCallback.setSecondaryImageData(x, y, name=self._layerImageName(self._secondaryLayer))
-
-        contourNames = [contour.name for contour in self._contourLayer.contours]
-        contourData = self._resliceContoursBetweenTwoPoints(self._contourLayer, point1, point2)
-        pen = [mkPen(color=contour.color, width=1) for contour in self._contourLayer.contours]
-        self._lineWidgetCallback.setContourData(contourData, name=contourNames, pen=pen)
-
-    def _resliceLayerDataBewteenTwoPoints(self, layer, point1, point2):
-        if layer.image is None:
-            return ([0, 0], [0, 0])
-
-        num = 1000
-        points0 = np.linspace(point1[0], point2[0], num)
-        points1 = np.linspace(point1[1], point2[1], num)
-        points2 = np.linspace(point1[2], point2[2], num)
-        data = np.array(points1)
-
-        x = np.linspace(0, sqrt((point2[0] - point1[0]) * (point2[0] - point1[0]) + (point2[1] - point1[1]) * (
-                point2[1] - point1[1]) + (point2[2] - point1[2]) * (point2[2] - point1[2])), num)
-
-        for i, p0 in enumerate(points0):
-            data[i] = layer.resliceDataFromPhysicalPoint((p0, points1[i], points2[i]))
-
-        return (x, data)
-
-    def _layerImageName(self, layer):
-        if layer.image is None:
-            return None
-
-        return layer.image.name
-
-
-    def _resliceContoursBetweenTwoPoints(self, layer:ContourLayer, point1:typing.Sequence[float], point2:typing.Sequence[float]):
-        contours = layer.contours
-
-        res = []
-        if len(contours)<=0:
-            for contour in contours:
-                res.append(([0, 0], [0, 0]))
-            return res
-
-        num = 1000
-        points0 = np.linspace(point1[0], point2[0], num)
-        points1 = np.linspace(point1[1], point2[1], num)
-        points2 = np.linspace(point1[2], point2[2], num)
-
-
-        data = np.zeros((len(contours), num))
-        x = np.linspace(0, sqrt((point2[0] - point1[0]) * (point2[0] - point1[0]) + (point2[1] - point1[1]) * (
-                point2[1] - point1[1]) + (point2[2] - point1[2]) * (point2[2] - point1[2])), num)
-
-
-        for i, p0 in enumerate(points0):
-            contoursData = layer.resliceDataFromPhysicalPoint((p0, points1[i], points2[i]))
-            for c, contour in enumerate(contours):
-                data[c, i] = -10000+contoursData[c]*20000
-
-        for c, contour in enumerate(contours):
-            res.append((x, data[c, :]))
-
-        return res
+import typing
+from math import sqrt
+
+import numpy as np
+from pyqtgraph import mkPen
+from vtkmodules.vtkInteractionWidgets import vtkLineWidget2
+
+from opentps.core import Event
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.contourLayer import ContourLayer
+from opentps.gui.viewer.dataViewerComponents.imageViewerComponents.primaryImage3DLayer import PrimaryImage3DLayer
+
+
+class ProfileWidget:
+    class ProfileWidgetCallback:
+        def __init__(self):
+            self._setPrimaryImageData = lambda *args, **kwargs: None
+            self._setSecondaryImageData = lambda *args, **kwargs: None
+            self._setContourData = lambda *args, **kwargs: None
+
+        @property
+        def setPrimaryImageData(self):
+            return self._setPrimaryImageData
+
+        @setPrimaryImageData.setter
+        def setPrimaryImageData(self, func):
+            self._setPrimaryImageData = func
+
+        @property
+        def setSecondaryImageData(self):
+            return self._setSecondaryImageData
+
+        @setSecondaryImageData.setter
+        def setSecondaryImageData(self, func):
+            self._setSecondaryImageData = func
+
+        @property
+        def setContourData(self):
+            return self._setContourData
+
+        @setContourData.setter
+        def setContourData(self, func):
+            self._setContourData = func
+
+    def __init__(self, renderer, renderWindow):
+        self.lineWidgeEnabledSignal = Event(bool)
+
+        self._lineWidget = vtkLineWidget2()
+        self._lineWidgetCallback = None
+        self._lineWidgetEnabled = False
+        self._primaryLayer = None
+        self._secondaryLayer = None
+        self._contourLayer = None
+        self._renderer = renderer
+        self._renderWindow = renderWindow
+
+        self._lineWidget.SetCurrentRenderer(self._renderer)
+        self._lineWidget.AddObserver("InteractionEvent", self.onProfileWidgetInteraction)
+        self._lineWidget.AddObserver("EndInteractionEvent", self.onProfileWidgetInteraction)
+        self._lineWidget.SetInteractor(self._renderWindow.GetInteractor())
+
+    @property
+    def enabled(self) -> bool:
+        return self._lineWidgetEnabled
+
+    @enabled.setter
+    def enabled(self, enabled: bool):
+        if enabled == self._lineWidgetEnabled:
+            return
+
+        if enabled:
+            self._lineWidget.On()
+            self._lineWidget.GetLineRepresentation().SetLineColor(1, 0, 0)
+            self._lineWidgetEnabled = True
+        else:
+            self._lineWidget.Off()
+            self._lineWidgetEnabled = False
+            self._renderWindow.Render()
+
+        self.lineWidgeEnabledSignal.emit(self._lineWidgetEnabled)
+
+    @property
+    def callback(self):
+        return self._lineWidgetCallback
+
+    @callback.setter
+    def callback(self, method):
+        self._lineWidgetCallback = method
+
+    @property
+    def primaryLayer(self):
+        return self._primaryLayer
+
+    @primaryLayer.setter
+    def primaryLayer(self, layer):
+        self._primaryLayer = layer
+
+        if isinstance(self._primaryLayer, PrimaryImage3DLayer):
+            if not self._primaryLayer.image is None:
+                self._primaryLayer._reslice.RemoveObserver(self._endEventObserver)
+
+            self._endEventObserver = self._primaryLayer._reslice.AddObserver("EndEvent", self.onProfileWidgetInteraction)
+
+    @property
+    def secondaryLayer(self):
+        return self._secondaryLayer
+
+    @secondaryLayer.setter
+    def secondaryLayer(self, layer):
+        self._secondaryLayer = layer
+
+    @property
+    def contourLayer(self):
+        return self._secondaryLayer
+
+    @contourLayer.setter
+    def contourLayer(self, layer):
+        self._contourLayer = layer
+
+    def setInitialPosition(self, worldPos: typing.Sequence):
+        self._lineWidget.GetLineRepresentation().SetPoint1WorldPosition((worldPos[0], worldPos[1], 0.01))
+        self._lineWidget.GetLineRepresentation().SetPoint2WorldPosition((worldPos[0], worldPos[1], 0.01))
+
+    def onProfileWidgetInteraction(self, obj, event):
+        if not self.enabled:
+            return
+
+        point1 = self._lineWidget.GetLineRepresentation().GetPoint1WorldPosition()
+        point2 = self._lineWidget.GetLineRepresentation().GetPoint2WorldPosition()
+
+        if point1[1]==point1[2]==point2[1]==point2[2]:
+            return
+
+        matrix = self._primaryLayer.resliceAxes
+        point1 = matrix.MultiplyPoint((point1[0], point1[1], 0, 1))
+        point2 = matrix.MultiplyPoint((point2[0], point2[1], 0, 1))
+
+        x, y = self._resliceLayerDataBewteenTwoPoints(self._primaryLayer, point1, point2)
+        self._lineWidgetCallback.setPrimaryImageData(x, y, name=self._layerImageName(self._primaryLayer))
+
+        x, y = self._resliceLayerDataBewteenTwoPoints(self._secondaryLayer, point1, point2)
+        self._lineWidgetCallback.setSecondaryImageData(x, y, name=self._layerImageName(self._secondaryLayer))
+
+        contourNames = [contour.name for contour in self._contourLayer.contours]
+        contourData = self._resliceContoursBetweenTwoPoints(self._contourLayer, point1, point2)
+        pen = [mkPen(color=contour.color, width=1) for contour in self._contourLayer.contours]
+        self._lineWidgetCallback.setContourData(contourData, name=contourNames, pen=pen)
+
+    def _resliceLayerDataBewteenTwoPoints(self, layer, point1, point2):
+        if layer.image is None:
+            return ([0, 0], [0, 0])
+
+        num = 1000
+        points0 = np.linspace(point1[0], point2[0], num)
+        points1 = np.linspace(point1[1], point2[1], num)
+        points2 = np.linspace(point1[2], point2[2], num)
+        data = np.array(points1)
+
+        x = np.linspace(0, sqrt((point2[0] - point1[0]) * (point2[0] - point1[0]) + (point2[1] - point1[1]) * (
+                point2[1] - point1[1]) + (point2[2] - point1[2]) * (point2[2] - point1[2])), num)
+
+        for i, p0 in enumerate(points0):
+            data[i] = layer.resliceDataFromPhysicalPoint((p0, points1[i], points2[i]))
+
+        return (x, data)
+
+    def _layerImageName(self, layer):
+        if layer.image is None:
+            return None
+
+        return layer.image.name
+
+
+    def _resliceContoursBetweenTwoPoints(self, layer:ContourLayer, point1:typing.Sequence[float], point2:typing.Sequence[float]):
+        contours = layer.contours
+
+        res = []
+        if len(contours)<=0:
+            for contour in contours:
+                res.append(([0, 0], [0, 0]))
+            return res
+
+        num = 1000
+        points0 = np.linspace(point1[0], point2[0], num)
+        points1 = np.linspace(point1[1], point2[1], num)
+        points2 = np.linspace(point1[2], point2[2], num)
+
+
+        data = np.zeros((len(contours), num))
+        x = np.linspace(0, sqrt((point2[0] - point1[0]) * (point2[0] - point1[0]) + (point2[1] - point1[1]) * (
+                point2[1] - point1[1]) + (point2[2] - point1[2]) * (point2[2] - point1[2])), num)
+
+
+        for i, p0 in enumerate(points0):
+            contoursData = layer.resliceDataFromPhysicalPoint((p0, points1[i], points2[i]))
+            for c, contour in enumerate(contours):
+                data[c, i] = -10000+contoursData[c]*20000
+
+        for c, contour in enumerate(contours):
+            res.append((x, data[c, :]))
+
+        return res
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/doseComparisonDataViewer.py` & `opentps_gui-1.0.5/opentps/gui/viewer/doseComparisonDataViewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,97 @@
-from typing import Optional
-
-from opentps.core.data.images import DoseImage
-from opentps.core.data.images._image3D import Image3D
-from opentps.gui.viewer.dataViewerComponents.doseComparisonImageProvider import DoseComparisonImageProvider
-from opentps.gui.viewer.dataViewer import DataViewer
-
-
-class DoseComparisonDataViewer(DataViewer):
-    def __init__(self, viewController):
-        self._displayDoseComparison = False
-        self._doseComparisonImageProvider = DoseComparisonImageProvider()
-
-        super().__init__(viewController)
-
-
-    ####################################################################################################################
-    # This is the logical part of the viewer. Should we migrate this to a dedicated controller?
-    def _initializeControl(self):
-        super()._initializeControl()
-
-        self._imageViewerActions.doseComparisonDataViewer = self
-
-        self.displayTypeChangedSignal.connect(self._handleDisplayTypeChange)
-
-        self._viewController.dose1ChangedSignal.connect(self._setDose1)
-        self._viewController.dose2ChangedSignal.connect(self._setDose2)
-
-    @property
-    def comparisonMetric(self):
-        return self._doseComparisonImageProvider.comparisonMetric
-
-    @comparisonMetric.setter
-    def comparisonMetric(self, metric):
-        self._doseComparisonImageProvider.comparisonMetric = metric
-
-    def _handleDisplayTypeChange(self, displayType):
-        super()._handleDisplayTypeChange(displayType)
-
-        if not self._displayDoseComparison:
-            self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
-
-    def _handleNewDoseComparisonImage(self, *ags):
-        self._setSecondaryImage(self._doseComparisonImageProvider.doseComparisonImage)
-
-    def _setSecondaryImage(self, image:Optional[Image3D]):
-        if not self._displayDoseComparison:
-            super()._setSecondaryImage(image)
-
-        if image != self._doseComparisonImageProvider.doseComparisonImage:
-            self._displayDoseComparison = False
-
-        if image is None:
-            oldImage = self.cachedStaticImage3DViewer.secondaryImage
-            if oldImage is None:
-                return
-        elif not (image.patient is None):
-            image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
-
-        self.cachedStaticImage3DViewer.secondaryImage = image
-
-        if self._displayDoseComparison:
-            self._imageViewerActions.setImageViewer(self._currentViewer)
-            self._imageViewerActions.hide()
-
-    def _setDose1(self, image:Optional[DoseImage]):
-        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
-
-        self._displayDoseComparison = True
-        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.connect(self._handleNewDoseComparisonImage)
-        self._handleNewDoseComparisonImage()
-
-        image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
-
-        self._doseComparisonImageProvider.dose1 = image
-        self._dvhViewer.dose = image
-
-    def _setDose2(self, image:Optional[DoseImage]):
-        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
-
-        self._displayDoseComparison = True
-        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.connect(self._handleNewDoseComparisonImage)
-        self._handleNewDoseComparisonImage()
-
-        image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
-
-        self._doseComparisonImageProvider.dose2 = image
-        self._dvhViewer.dose2 = image
-
-    def _setDVHDose(self, image:Optional[DoseImage]):
-        if not self._displayDoseComparison:
-            self.cachedStaticDVHViewer.clear()
-            super()._setDVHDose(image)
-        else:
-            return
+from typing import Optional
+
+from opentps.core.data.images import DoseImage
+from opentps.core.data.images._image3D import Image3D
+from opentps.gui.viewer.dataViewerComponents.doseComparisonImageProvider import DoseComparisonImageProvider
+from opentps.gui.viewer.dataViewer import DataViewer
+
+
+class DoseComparisonDataViewer(DataViewer):
+    def __init__(self, viewController):
+        self._displayDoseComparison = False
+        self._doseComparisonImageProvider = DoseComparisonImageProvider()
+
+        super().__init__(viewController)
+
+
+    ####################################################################################################################
+    # This is the logical part of the viewer. Should we migrate this to a dedicated controller?
+    def _initializeControl(self):
+        super()._initializeControl()
+
+        self._imageViewerActions.doseComparisonDataViewer = self
+
+        self.displayTypeChangedSignal.connect(self._handleDisplayTypeChange)
+
+        self._viewController.dose1ChangedSignal.connect(self._setDose1)
+        self._viewController.dose2ChangedSignal.connect(self._setDose2)
+
+    @property
+    def comparisonMetric(self):
+        return self._doseComparisonImageProvider.comparisonMetric
+
+    @comparisonMetric.setter
+    def comparisonMetric(self, metric):
+        self._doseComparisonImageProvider.comparisonMetric = metric
+
+    def _handleDisplayTypeChange(self, displayType):
+        super()._handleDisplayTypeChange(displayType)
+
+        if not self._displayDoseComparison:
+            self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
+
+    def _handleNewDoseComparisonImage(self, *ags):
+        self._setSecondaryImage(self._doseComparisonImageProvider.doseComparisonImage)
+
+    def _setSecondaryImage(self, image:Optional[Image3D]):
+        if not self._displayDoseComparison:
+            super()._setSecondaryImage(image)
+
+        if image != self._doseComparisonImageProvider.doseComparisonImage:
+            self._displayDoseComparison = False
+
+        if image is None:
+            oldImage = self.cachedStaticImage3DViewer.secondaryImage
+            if oldImage is None:
+                return
+        elif not (image.patient is None):
+            image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
+
+        self.cachedStaticImage3DViewer.secondaryImage = image
+
+        if self._displayDoseComparison:
+            self._imageViewerActions.setImageViewer(self._currentViewer)
+            self._imageViewerActions.hide()
+        else:
+            self.cachedStaticDVHViewer.dose2 = None
+
+    def _setDose1(self, image:Optional[DoseImage]):
+        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
+
+        self._displayDoseComparison = True
+        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.connect(self._handleNewDoseComparisonImage)
+        self._handleNewDoseComparisonImage()
+
+        image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
+
+        self._doseComparisonImageProvider.dose1 = image
+        self._dvhViewer.dose = image
+
+    def _setDose2(self, image:Optional[DoseImage]):
+        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.disconnect(self._handleNewDoseComparisonImage)
+
+        self._displayDoseComparison = True
+        self._doseComparisonImageProvider.doseComparisonImageChangedSignal.connect(self._handleNewDoseComparisonImage)
+        self._handleNewDoseComparisonImage()
+
+        image.patient.imageRemovedSignal.connect(self._removeImageFromViewers)
+
+        self._doseComparisonImageProvider.dose2 = image
+        self._dvhViewer.dose2 = image
+
+    def _setDVHDose(self, image:Optional[DoseImage]):
+        if not self._displayDoseComparison:
+            self.cachedStaticDVHViewer.dose2 = None
+            super()._setDVHDose(image)
+        else:
+            return
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/dynamicDisplayController.py` & `opentps_gui-1.0.5/opentps/gui/viewer/dynamicDisplayController.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from PyQt5.QtCore import QTimer
-
-
-class DynamicDisplayController():
-
-    # MODE_DYNAMIC = 'DYNAMIC'
-    # MODE_STATIC = 'STATIC'
-
-    def __init__(self, viewController):
-
-        self._viewController = viewController
-        self._viewerPanelToolBar = None
-
-        self.isDynamic = False
-        self.dynamicViewerUnitList = []
-
-        self.currentSpeedCoef = 1
-        self.refreshRateInFramePerSec = 24
-        self.refreshRateInMS = int(round(1000 / self.refreshRateInFramePerSec))
-        self.timerStepNumber = 0
-        self.time = 0
-        self.timer = QTimer()
-        self.timer.timeout.connect(self.checkIfUpdate)
-
-
-    def setToolBar(self, viewerPanelToolBar):
-        self._viewerPanelToolBar = viewerPanelToolBar
-        self.connectToolBar()
-
-
-    def connectToolBar(self):
-        self._viewerPanelToolBar.playPauseSignal.connect(self.playOrPause)
-        self._viewerPanelToolBar.fasterSignal.connect(self.playFaster)
-        self._viewerPanelToolBar.slowerSignal.connect(self.playSlower)
-        self._viewerPanelToolBar.refreshRateChangedSignal.connect(self.setRefreshRate)
-
-
-    def addDynamicViewer(self, viewer):
-        # print('in displayController addDynViewer', type(viewer))
-        if viewer not in self.dynamicViewerUnitList:
-            self.dynamicViewerUnitList.append(viewer)
-        else:
-            return
-        if self.isDynamic == False:
-            self.switchDynamicMode()
-
-
-    def removeDynamicViewer(self, viewer):
-        # print('in displayController removeDynamicViewer', type(viewer))
-        if viewer in self.dynamicViewerUnitList:
-            viewer.resetDynamicParameters()
-            self.dynamicViewerUnitList.remove(viewer)
-        else:
-            return
-        if not self.dynamicViewerUnitList:
-            self.switchDynamicMode()
-
-
-    def switchDynamicMode(self):
-        """
-        This function switches the mode from dynamic to static and inversely. It starts or stops the timer accordingly.
-        """
-        self.isDynamic = not self.isDynamic
-        if self.isDynamic == True:
-            print('Switch to dynamic mode')
-            self.time = 0
-            self.timer.start(self.refreshRateInMS)
-            self._viewerPanelToolBar.addDynamicButtons()
-
-        elif self.isDynamic == False:
-            self.timer.stop()
-            self._viewerPanelToolBar.removeDynamicButtons()
-            print('Switch to static mode')
-
-
-    def checkIfUpdate(self):
-        """
-        This function checks if an update must occur at this time.
-        It only works for dynamic3DSequences for now.
-        """
-        self.time += self.refreshRateInMS * self.currentSpeedCoef
-        for dynamicViewerUnit in self.dynamicViewerUnitList:
-
-            # print(type(dynamicViewerUnit))
-
-            dyn3DSeqForViewer = dynamicViewerUnit.primaryImage
-            timingsList = dyn3DSeqForViewer.data.timingsList
-            loopShift = timingsList[-1] * dynamicViewerUnit.loopStepNumber
-            curIndex = dynamicViewerUnit.curPrimaryImgIdx
-
-            # print('in dynamicDisplayController, checkIfUpdate', timingsList)
-
-            if self.time - loopShift > timingsList[curIndex + 1]:
-                newIndex = self.lookForClosestIndex(self.time - loopShift, curIndex, timingsList, dynamicViewerUnit)
-                dynamicViewerUnit.nextImage(newIndex)
-
-
-    def lookForClosestIndex(self, time, curIndex, timingsList, dataViewer):
-        """
-        This function return the index of the last position in timingList lower than time,
-        meaning the time has passed this event and an update must occur.
-        If the curIndex has reached the end of the timingsList, it returns 0
-        """
-        while timingsList[curIndex + 1] < time:
-            curIndex += 1
-            if curIndex == len(timingsList) - 1:  # has reach the end
-                dataViewer.loopStepNumber += 1
-                return 0
-
-        return curIndex
-
-
-    def playOrPause(self, playPauseBool):
-        if playPauseBool:
-            self.currentSpeedCoef = 1
-        else:
-            self.currentSpeedCoef = 0
-
-
-    def playFaster(self):
-        self.currentSpeedCoef *= 2
-
-
-    def playSlower(self):
-        self.currentSpeedCoef /= 2
-
-
-    def setRefreshRate(self, refreshRate):
-        self.refreshRateInFramePerSec = refreshRate
-        if self.refreshRateInFramePerSec < 0.2:
-            self.refreshRateInFramePerSec = 0.2
-        if self.refreshRateInFramePerSec > 200:
-            self.refreshRateInFramePerSec = 200
-        self.refreshRateInMS = int(round(1000 / self.refreshRateInFramePerSec))
-        self.timer.stop()
-        self.timer.start(self.refreshRateInMS)
+from PyQt5.QtCore import QTimer
+
+
+class DynamicDisplayController():
+
+    # MODE_DYNAMIC = 'DYNAMIC'
+    # MODE_STATIC = 'STATIC'
+
+    def __init__(self, viewController):
+
+        self._viewController = viewController
+        self._viewerPanelToolBar = None
+
+        self.isDynamic = False
+        self.dynamicViewerUnitList = []
+
+        self.currentSpeedCoef = 1
+        self.refreshRateInFramePerSec = 24
+        self.refreshRateInMS = int(round(1000 / self.refreshRateInFramePerSec))
+        self.timerStepNumber = 0
+        self.time = 0
+        self.timer = QTimer()
+        self.timer.timeout.connect(self.checkIfUpdate)
+
+
+    def setToolBar(self, viewerPanelToolBar):
+        self._viewerPanelToolBar = viewerPanelToolBar
+        self.connectToolBar()
+
+
+    def connectToolBar(self):
+        self._viewerPanelToolBar.playPauseSignal.connect(self.playOrPause)
+        self._viewerPanelToolBar.fasterSignal.connect(self.playFaster)
+        self._viewerPanelToolBar.slowerSignal.connect(self.playSlower)
+        self._viewerPanelToolBar.refreshRateChangedSignal.connect(self.setRefreshRate)
+
+
+    def addDynamicViewer(self, viewer):
+        # print('in displayController addDynViewer', type(viewer))
+        if viewer not in self.dynamicViewerUnitList:
+            self.dynamicViewerUnitList.append(viewer)
+        else:
+            return
+        if self.isDynamic == False:
+            self.switchDynamicMode()
+
+
+    def removeDynamicViewer(self, viewer):
+        # print('in displayController removeDynamicViewer', type(viewer))
+        if viewer in self.dynamicViewerUnitList:
+            viewer.resetDynamicParameters()
+            self.dynamicViewerUnitList.remove(viewer)
+        else:
+            return
+        if not self.dynamicViewerUnitList:
+            self.switchDynamicMode()
+
+
+    def switchDynamicMode(self):
+        """
+        This function switches the mode from dynamic to static and inversely. It starts or stops the timer accordingly.
+        """
+        self.isDynamic = not self.isDynamic
+        if self.isDynamic == True:
+            print('Switch to dynamic mode')
+            self.time = 0
+            self.timer.start(self.refreshRateInMS)
+            self._viewerPanelToolBar.addDynamicButtons()
+
+        elif self.isDynamic == False:
+            self.timer.stop()
+            self._viewerPanelToolBar.removeDynamicButtons()
+            print('Switch to static mode')
+
+
+    def checkIfUpdate(self):
+        """
+        This function checks if an update must occur at this time.
+        It only works for dynamic3DSequences for now.
+        """
+        self.time += self.refreshRateInMS * self.currentSpeedCoef
+        for dynamicViewerUnit in self.dynamicViewerUnitList:
+
+            # print(type(dynamicViewerUnit))
+
+            dyn3DSeqForViewer = dynamicViewerUnit.primaryImage
+            timingsList = dyn3DSeqForViewer.data.timingsList
+            loopShift = timingsList[-1] * dynamicViewerUnit.loopStepNumber
+            curIndex = dynamicViewerUnit.curPrimaryImgIdx
+
+            # print('in dynamicDisplayController, checkIfUpdate', timingsList)
+
+            if self.time - loopShift > timingsList[curIndex + 1]:
+                newIndex = self.lookForClosestIndex(self.time - loopShift, curIndex, timingsList, dynamicViewerUnit)
+                dynamicViewerUnit.nextImage(newIndex)
+
+
+    def lookForClosestIndex(self, time, curIndex, timingsList, dataViewer):
+        """
+        This function return the index of the last position in timingList lower than time,
+        meaning the time has passed this event and an update must occur.
+        If the curIndex has reached the end of the timingsList, it returns 0
+        """
+        while timingsList[curIndex + 1] < time:
+            curIndex += 1
+            if curIndex == len(timingsList) - 1:  # has reach the end
+                dataViewer.loopStepNumber += 1
+                return 0
+
+        return curIndex
+
+
+    def playOrPause(self, playPauseBool):
+        if playPauseBool:
+            self.currentSpeedCoef = 1
+        else:
+            self.currentSpeedCoef = 0
+
+
+    def playFaster(self):
+        self.currentSpeedCoef *= 2
+
+
+    def playSlower(self):
+        self.currentSpeedCoef /= 2
+
+
+    def setRefreshRate(self, refreshRate):
+        self.refreshRateInFramePerSec = refreshRate
+        if self.refreshRateInFramePerSec < 0.2:
+            self.refreshRateInFramePerSec = 0.2
+        if self.refreshRateInFramePerSec > 200:
+            self.refreshRateInFramePerSec = 200
+        self.refreshRateInMS = int(round(1000 / self.refreshRateInFramePerSec))
+        self.timer.stop()
+        self.timer.start(self.refreshRateInMS)
         print('Refresh Rate Set to', self.refreshRateInFramePerSec, 'frames/sec --> Check every', self.refreshRateInMS, 'ms')
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/exportWindow.py` & `opentps_gui-1.0.5/opentps/gui/viewer/exportWindow.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from PyQt5.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QButtonGroup, QRadioButton, QTableWidget, \
-    QFileDialog, QPushButton
-
-from opentps.core.io.dataExporter import ExportTypes, ExportConfig, exportPatient
-
-
-class ExportWindow(QMainWindow):
-    def __init__(self, viewController):
-        super().__init__()
-
-        self._viewController = viewController
-
-        self.setWindowTitle('Export settings')
-        self.resize(400, 400)
-
-        centralWidget = QWidget()
-        self.setCentralWidget(centralWidget)
-        self._layout = QVBoxLayout()
-        centralWidget.setLayout(self._layout)
-
-        self._exportTable = ExportTable(parent=self)
-        self._layout.addWidget(self._exportTable)
-
-        self._exportButton = QPushButton("Select folder and export")
-        self._exportButton.clicked.connect(self._handleExport)
-        self._layout.addWidget(self._exportButton)
-
-        self._layout.addStretch()
-        self.adjustSize()
-        self.setFixedSize(self.size())
-
-    def _handleExport(self):
-        # TODO: Use export options defined in ExportTable
-
-        folderpath = QFileDialog.getExistingDirectory(self, 'Select folder')
-
-        if folderpath == "":
-            return
-
-        exportPatient(self._viewController.currentPatient, folderpath, self._exportTable.exportConfig)
-
-class ExportTable(QWidget):
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-        dataTypes = ExportConfig()
-        self._exportTypes = [ExportTypes.DICOM, ExportTypes.MHD, ExportTypes.MCSQUARE, ExportTypes.PICKLE]
-        self._buttonGroups = []
-
-        rowNb = len(dataTypes)
-        colNb = len(self._exportTypes)
-
-        self.table = QTableWidget()
-        self.table.setRowCount(rowNb)
-        self.table.setColumnCount(colNb)
-        self.table.setHorizontalHeaderLabels([exportType.value for exportType in self._exportTypes])
-        self.table.setVerticalHeaderLabels([dataType.name for dataType in dataTypes])
-
-        self.table.setFixedWidth((colNb+1)*self.table.columnWidth(0))
-
-        self._layout = QHBoxLayout(self)
-        self._layout.addWidget(self.table)
-
-        for row, dataType in enumerate(dataTypes):
-            button_group = QButtonGroup(self)
-            button_group.setExclusive(True)
-            self._buttonGroups.append(button_group)
-
-            dataTypeHasOneOptionChecked = False
-            for col, exportType in enumerate(self._exportTypes):
-                checkbox = QRadioButton()
-                button_group.addButton(checkbox, col)
-                self.table.setCellWidget(row, col, checkbox)
-
-                if exportType in dataType.exportTypes:
-                    checkbox.setEnabled(True)
-                    if not dataTypeHasOneOptionChecked:
-                        checkbox.setChecked(True)
-                        dataTypeHasOneOptionChecked = True
-                    else:
-                        checkbox.setChecked(False)
-                else:
-                    checkbox.setChecked(False)
-                    checkbox.setEnabled(False)
-
-    @property
-    def exportConfig(self) -> ExportConfig:
-        config = ExportConfig()
-
-        for i, dataType in enumerate(config):
-            dataType.exportType = self._exportTypes[self._buttonGroups[i].checkedId()]
-            print(dataType.exportType)
-
+from PyQt5.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QButtonGroup, QRadioButton, QTableWidget, \
+    QFileDialog, QPushButton
+
+from opentps.core.io.dataExporter import ExportTypes, ExportConfig, exportPatient
+
+
+class ExportWindow(QMainWindow):
+    def __init__(self, viewController):
+        super().__init__()
+
+        self._viewController = viewController
+
+        self.setWindowTitle('Export settings')
+        self.resize(400, 400)
+
+        centralWidget = QWidget()
+        self.setCentralWidget(centralWidget)
+        self._layout = QVBoxLayout()
+        centralWidget.setLayout(self._layout)
+
+        self._exportTable = ExportTable(parent=self)
+        self._layout.addWidget(self._exportTable)
+
+        self._exportButton = QPushButton("Select folder and export")
+        self._exportButton.clicked.connect(self._handleExport)
+        self._layout.addWidget(self._exportButton)
+
+        self._layout.addStretch()
+        self.adjustSize()
+        self.setFixedSize(self.size())
+
+    def _handleExport(self):
+        # TODO: Use export options defined in ExportTable
+
+        folderpath = QFileDialog.getExistingDirectory(self, 'Select folder')
+
+        if folderpath == "":
+            return
+
+        exportPatient(self._viewController.currentPatient, folderpath, self._exportTable.exportConfig)
+
+class ExportTable(QWidget):
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        dataTypes = ExportConfig()
+        self._exportTypes = [ExportTypes.DICOM, ExportTypes.MHD, ExportTypes.MCSQUARE, ExportTypes.PICKLE]
+        self._buttonGroups = []
+
+        rowNb = len(dataTypes)
+        colNb = len(self._exportTypes)
+
+        self.table = QTableWidget()
+        self.table.setRowCount(rowNb)
+        self.table.setColumnCount(colNb)
+        self.table.setHorizontalHeaderLabels([exportType.value for exportType in self._exportTypes])
+        self.table.setVerticalHeaderLabels([dataType.name for dataType in dataTypes])
+
+        self.table.setFixedWidth((colNb+1)*self.table.columnWidth(0))
+
+        self._layout = QHBoxLayout(self)
+        self._layout.addWidget(self.table)
+
+        for row, dataType in enumerate(dataTypes):
+            button_group = QButtonGroup(self)
+            button_group.setExclusive(True)
+            self._buttonGroups.append(button_group)
+
+            dataTypeHasOneOptionChecked = False
+            for col, exportType in enumerate(self._exportTypes):
+                checkbox = QRadioButton()
+                button_group.addButton(checkbox, col)
+                self.table.setCellWidget(row, col, checkbox)
+
+                if exportType in dataType.exportTypes:
+                    checkbox.setEnabled(True)
+                    if not dataTypeHasOneOptionChecked:
+                        checkbox.setChecked(True)
+                        dataTypeHasOneOptionChecked = True
+                    else:
+                        checkbox.setChecked(False)
+                else:
+                    checkbox.setChecked(False)
+                    checkbox.setEnabled(False)
+
+    @property
+    def exportConfig(self) -> ExportConfig:
+        config = ExportConfig()
+
+        for i, dataType in enumerate(config):
+            dataType.exportType = self._exportTypes[self._buttonGroups[i].checkedId()]
+            print(dataType.exportType)
+
         return config
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/grid.py` & `opentps_gui-1.0.5/opentps/gui/viewer/grid.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from PyQt5.QtWidgets import QWidget
-
-
-class Grid(QWidget):
-    def __init__(self, viewController, parent):
-        super().__init__(parent)
-
-        self._gridElements = []
-        self._viewController = viewController
-
-    @property
-    def gridElements(self):
-        # Prevent from appending/removing to/from _gridElements
-        return [element for element in self._gridElements]
-
-    def appendGridElement(self, gridElement):
-        self._gridElements.append(gridElement)
-
-    def removeGridElement(self, gridElement):
-        self._gridElements.remove(gridElement)
+from PyQt5.QtWidgets import QWidget
+
+
+class Grid(QWidget):
+    def __init__(self, viewController, parent):
+        super().__init__(parent)
+
+        self._gridElements = []
+        self._viewController = viewController
+
+    @property
+    def gridElements(self):
+        # Prevent from appending/removing to/from _gridElements
+        return [element for element in self._gridElements]
+
+    def appendGridElement(self, gridElement):
+        self._gridElements.append(gridElement)
+
+    def removeGridElement(self, gridElement):
+        self._gridElements.remove(gridElement)
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/gridFourElements.py` & `opentps_gui-1.0.5/opentps/gui/viewer/gridFourElements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,171 @@
-from PyQt5 import QtCore
-from PyQt5.QtCore import QSize
-from PyQt5.QtWidgets import QHBoxLayout, QFrame, QSplitter, QVBoxLayout
-
-from opentps.gui.viewer.doseComparisonDataViewer import DoseComparisonDataViewer
-from opentps.gui.viewer.grid import Grid
-
-
-class GridFourElements(Grid):
-    def __init__(self, viewController, parent):
-        super().__init__(viewController, parent)
-
-        self._minimumSize = QSize(200, 200)
-        self._setEqualSize = False #Use to set equal size before qwidget is effectively shown
-
-        # Horizontal splitting
-        self._mainLayout = QHBoxLayout(self)
-
-        self._horizontalSplitter = QSplitter(QtCore.Qt.Horizontal, self)
-        self._leftPart = QFrame(self._horizontalSplitter)
-        self._leftPart.setFrameShape(QFrame.StyledPanel)
-        self._rightPart = QFrame(self._horizontalSplitter)
-        self._rightPart.setFrameShape(QFrame.StyledPanel)
-        self._horizontalSplitter.addWidget(self._leftPart)
-        self._horizontalSplitter.addWidget(self._rightPart)
-        self._horizontalSplitter.setStretchFactor(1, 1)
-
-        self._mainLayout.addWidget(self._horizontalSplitter)
-        self._mainLayout.setContentsMargins(0, 0, 0, 0)
-
-        # Vertical splitting
-        leftPartLayout = QVBoxLayout(self._leftPart)
-        leftPartLayout.setContentsMargins(0, 0, 0, 0)
-        rightPartLayout = QVBoxLayout(self._rightPart)
-        rightPartLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._leftPartSplitter = VerticalSplitter(self)
-        self._botLeftGridElementContainer = self._leftPartSplitter.botGridElementContainer
-        self._topLeftGridElementContainer = self._leftPartSplitter.topGridElementContainer
-        leftPartLayout.addWidget(self._leftPartSplitter)
-
-        self._rightPartSplitter = VerticalSplitter(self)
-        self._botRightGridElementContainer = self._rightPartSplitter.botGridElementContainer
-        self._topRightGridElementContainer = self._rightPartSplitter.topGridElementContainer
-        rightPartLayout.addWidget(self._rightPartSplitter)
-
-        self._botLeftGridElementContainer.setMinimumSize(self._minimumSize)
-        self._botRightGridElementContainer.setMinimumSize(self._minimumSize)
-        self._topLeftGridElementContainer.setMinimumSize(self._minimumSize)
-        self._topRightGridElementContainer.setMinimumSize(self._minimumSize)
-
-        self._botLeftLayout = QVBoxLayout(self._botLeftGridElementContainer)
-        self._botRightLayout = QVBoxLayout(self._botRightGridElementContainer)
-        self._topLeftLayout = QVBoxLayout(self._topLeftGridElementContainer)
-        self._topRightLayout = QVBoxLayout(self._topRightGridElementContainer)
-
-        self._botLeftLayout.setContentsMargins(0, 0, 0, 0)
-        self._botRightLayout.setContentsMargins(0, 0, 0, 0)
-        self._topLeftLayout.setContentsMargins(0, 0, 0, 0)
-        self._topRightLayout.setContentsMargins(0, 0, 0, 0)
-
-        self._initializeViewers()
-
-    def _initializeViewers(self):
-        # Fill grid elements with data viewers
-        gridElement = DoseComparisonDataViewer(self._viewController)
-        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.AXIAL
-        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.AXIAL
-        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.AXIAL
-        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.AXIAL
-        self.appendGridElement(gridElement)
-        self._topLeftLayout.addWidget(gridElement)
-        gridElement = DoseComparisonDataViewer(self._viewController)
-        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.CORONAL
-        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.CORONAL
-        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.CORONAL
-        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.CORONAL
-        self.appendGridElement(gridElement)
-        self._topRightLayout.addWidget(gridElement)
-        gridElement = DoseComparisonDataViewer(self._viewController)
-        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.SAGITTAL
-        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.SAGITTAL
-        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.SAGITTAL
-        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.SAGITTAL
-        self.appendGridElement(gridElement)
-        self._botLeftLayout.addWidget(gridElement)
-        gridElement = DoseComparisonDataViewer(self._viewController)
-        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.SAGITTAL
-        self.appendGridElement(gridElement)
-        self._botRightLayout.addWidget(gridElement)
-
-
-    def resizeEvent(self, event):
-        if self._setEqualSize:
-            self.setEqualSize()
-        self._setEqualSize = False
-
-        self._oldWidth = event.oldSize().width()
-        self._newWidth = event.size().width()
-        self._leftWidth = self._horizontalSplitter.sizes()[0]
-
-        if self._oldWidth<=0 or self._oldWidth==self.width():
-            super().resizeEvent(event)
-            return
-
-        oldWidthRatio = self._leftWidth / self._oldWidth
-
-        leftPartWidth = int(oldWidthRatio * self._newWidth)
-        rightPartWidth = int(self._newWidth - oldWidthRatio * self._newWidth)
-
-        self._horizontalSplitter.setSizes([leftPartWidth, rightPartWidth])
-
-        super().resizeEvent(event)
-
-
-    def setEqualSize(self):
-        if not self.isVisible():
-            self._setEqualSize = True
-
-        leftPartWidth = int(self.width()/2)
-        self._horizontalSplitter.setSizes([leftPartWidth, leftPartWidth])
-
-        self._leftPartSplitter.setEqualSize()
-        self._rightPartSplitter.setEqualSize()
-
-
-class VerticalSplitter(QSplitter):
-    def __init__(self, parent):
-        super().__init__(QtCore.Qt.Vertical, parent)
-
-        self._setEqualSize = False  # Use to set equal size before qwidget is effectively shown
-
-        self.botGridElementContainer = QFrame(self)
-        self.topGridElementContainer = QFrame(self)
-        self.addWidget(self.topGridElementContainer)
-        self.addWidget(self.botGridElementContainer)
-        self.setStretchFactor(1, 1)
-
-        self.botGridElementContainer.setFrameShape(QFrame.StyledPanel)
-        self.topGridElementContainer.setFrameShape(QFrame.StyledPanel)
-
-    def resizeEvent(self, event):
-        if self._setEqualSize:
-            self.setEqualSize()
-        self._setEqualSize = False
-
-        self._oldHeight = event.oldSize().height()
-        self._newHeight = event.size().height()
-        self._topHeight = self.sizes()[0]
-
-        if self._oldHeight<=0 or self._oldHeight==self._newHeight:
-            super().resizeEvent(event)
-            return
-
-        oldHeightRatio = self._topHeight/self._oldHeight
-
-        topHeight = int(oldHeightRatio * self._newHeight)
-        botHeight = int(self._newHeight - oldHeightRatio*self._newHeight)
-
-        self.setSizes([topHeight, botHeight])
-
-    def setEqualSize(self):
-        if not self.isVisible():
-            self._setEqualSize = True
-
-        topHeight = int(self.height()/2)
-        self.setSizes([topHeight, topHeight])
+from PyQt5 import QtCore
+from PyQt5.QtCore import QSize
+from PyQt5.QtWidgets import QHBoxLayout, QFrame, QSplitter, QVBoxLayout
+
+from opentps.gui.viewer.doseComparisonDataViewer import DoseComparisonDataViewer
+from opentps.gui.viewer.grid import Grid
+
+
+class GridFourElements(Grid):
+    def __init__(self, viewController, parent):
+        super().__init__(viewController, parent)
+
+        self._minimumSize = QSize(200, 200)
+        self._setEqualSize = False #Use to set equal size before qwidget is effectively shown
+
+        # Horizontal splitting
+        self._mainLayout = QHBoxLayout(self)
+
+        self._horizontalSplitter = QSplitter(QtCore.Qt.Horizontal, self)
+        self._leftPart = QFrame(self._horizontalSplitter)
+        self._leftPart.setFrameShape(QFrame.StyledPanel)
+        self._rightPart = QFrame(self._horizontalSplitter)
+        self._rightPart.setFrameShape(QFrame.StyledPanel)
+        self._horizontalSplitter.addWidget(self._leftPart)
+        self._horizontalSplitter.addWidget(self._rightPart)
+        self._horizontalSplitter.setStretchFactor(1, 1)
+
+        self._mainLayout.addWidget(self._horizontalSplitter)
+        self._mainLayout.setContentsMargins(0, 0, 0, 0)
+
+        # Vertical splitting
+        leftPartLayout = QVBoxLayout(self._leftPart)
+        leftPartLayout.setContentsMargins(0, 0, 0, 0)
+        rightPartLayout = QVBoxLayout(self._rightPart)
+        rightPartLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._leftPartSplitter = VerticalSplitter(self)
+        self._botLeftGridElementContainer = self._leftPartSplitter.botGridElementContainer
+        self._topLeftGridElementContainer = self._leftPartSplitter.topGridElementContainer
+        leftPartLayout.addWidget(self._leftPartSplitter)
+
+        self._rightPartSplitter = VerticalSplitter(self)
+        self._botRightGridElementContainer = self._rightPartSplitter.botGridElementContainer
+        self._topRightGridElementContainer = self._rightPartSplitter.topGridElementContainer
+        rightPartLayout.addWidget(self._rightPartSplitter)
+
+        self._botLeftGridElementContainer.setMinimumSize(self._minimumSize)
+        self._botRightGridElementContainer.setMinimumSize(self._minimumSize)
+        self._topLeftGridElementContainer.setMinimumSize(self._minimumSize)
+        self._topRightGridElementContainer.setMinimumSize(self._minimumSize)
+
+        self._botLeftLayout = QVBoxLayout(self._botLeftGridElementContainer)
+        self._botRightLayout = QVBoxLayout(self._botRightGridElementContainer)
+        self._topLeftLayout = QVBoxLayout(self._topLeftGridElementContainer)
+        self._topRightLayout = QVBoxLayout(self._topRightGridElementContainer)
+
+        self._botLeftLayout.setContentsMargins(0, 0, 0, 0)
+        self._botRightLayout.setContentsMargins(0, 0, 0, 0)
+        self._topLeftLayout.setContentsMargins(0, 0, 0, 0)
+        self._topRightLayout.setContentsMargins(0, 0, 0, 0)
+
+        self._initializeViewers()
+
+    def closeEvent(self, QCloseEvent):
+
+        super().closeEvent(QCloseEvent)
+
+    def _initializeViewers(self):
+        # Fill grid elements with data viewers
+        gridElement = DoseComparisonDataViewer(self._viewController)
+        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.AXIAL
+        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.AXIAL
+        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.AXIAL
+        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.AXIAL
+        self.appendGridElement(gridElement)
+        self._topLeftLayout.addWidget(gridElement)
+        gridElement = DoseComparisonDataViewer(self._viewController)
+        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.CORONAL
+        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.CORONAL
+        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.CORONAL
+        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.CORONAL
+        self.appendGridElement(gridElement)
+        self._topRightLayout.addWidget(gridElement)
+        gridElement = DoseComparisonDataViewer(self._viewController)
+        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.SAGITTAL
+        # gridElement.cachedStaticImage2DViewer.viewType = gridElement.cachedStaticImage2DViewer.ViewerTypes.SAGITTAL
+        gridElement.cachedDynamicImage3DViewer.viewType = gridElement.cachedDynamicImage3DViewer.ViewerTypes.SAGITTAL
+        # gridElement.cachedDynamicImage2DViewer.viewType = gridElement.cachedDynamicImage2DViewer.ViewerTypes.SAGITTAL
+        self.appendGridElement(gridElement)
+        self._botLeftLayout.addWidget(gridElement)
+        gridElement = DoseComparisonDataViewer(self._viewController)
+        gridElement.cachedStaticImage3DViewer.viewType = gridElement.cachedStaticImage3DViewer.ViewerTypes.SAGITTAL
+        self.appendGridElement(gridElement)
+        self._botRightLayout.addWidget(gridElement)
+
+
+    def resizeEvent(self, event):
+        if self._setEqualSize:
+            self.setEqualSize()
+        self._setEqualSize = False
+
+        self._oldWidth = event.oldSize().width()
+        self._newWidth = event.size().width()
+        self._leftWidth = self._horizontalSplitter.sizes()[0]
+
+        if self._oldWidth<=0 or self._oldWidth==self.width():
+            super().resizeEvent(event)
+            return
+
+        oldWidthRatio = self._leftWidth / self._oldWidth
+
+        leftPartWidth = int(oldWidthRatio * self._newWidth)
+        rightPartWidth = int(self._newWidth - oldWidthRatio * self._newWidth)
+
+        self._horizontalSplitter.setSizes([leftPartWidth, rightPartWidth])
+
+        super().resizeEvent(event)
+
+
+    def setEqualSize(self):
+        if not self.isVisible():
+            self._setEqualSize = True
+
+        leftPartWidth = int(self.width()/2)
+        self._horizontalSplitter.setSizes([leftPartWidth, leftPartWidth])
+
+        self._leftPartSplitter.setEqualSize()
+        self._rightPartSplitter.setEqualSize()
+
+
+class VerticalSplitter(QSplitter):
+    def __init__(self, parent):
+        super().__init__(QtCore.Qt.Vertical, parent)
+
+        self._setEqualSize = False  # Use to set equal size before qwidget is effectively shown
+
+        self.botGridElementContainer = QFrame(self)
+        self.topGridElementContainer = QFrame(self)
+        self.addWidget(self.topGridElementContainer)
+        self.addWidget(self.botGridElementContainer)
+        self.setStretchFactor(1, 1)
+
+        self.botGridElementContainer.setFrameShape(QFrame.StyledPanel)
+        self.topGridElementContainer.setFrameShape(QFrame.StyledPanel)
+
+    def resizeEvent(self, event):
+        if self._setEqualSize:
+            self.setEqualSize()
+        self._setEqualSize = False
+
+        self._oldHeight = event.oldSize().height()
+        self._newHeight = event.size().height()
+        self._topHeight = self.sizes()[0]
+
+        if self._oldHeight<=0 or self._oldHeight==self._newHeight:
+            super().resizeEvent(event)
+            return
+
+        oldHeightRatio = self._topHeight/self._oldHeight
+
+        topHeight = int(oldHeightRatio * self._newHeight)
+        botHeight = int(self._newHeight - oldHeightRatio*self._newHeight)
+
+        self.setSizes([topHeight, botHeight])
+
+    def setEqualSize(self):
+        if not self.isVisible():
+            self._setEqualSize = True
+
+        topHeight = int(self.height()/2)
+        self.setSizes([topHeight, topHeight])
```

### Comparing `opentps-gui-1.0.4/opentps/gui/viewer/viewerToolbar.py` & `opentps_gui-1.0.5/opentps/gui/viewer/viewerToolbar.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-
-import os
-
-from PyQt5.QtCore import QSize, QDir
-from PyQt5.QtGui import QIcon
-from PyQt5.QtWidgets import QToolBar, QAction, QDialog, QPushButton, QLineEdit, QVBoxLayout, QFileDialog, \
-    QStackedWidget, QListView, QComboBox, QWidgetAction
-
-from opentps.core.io import dataLoader
-from opentps.core import Event
-from opentps.gui.viewer.dataViewer import DataViewer
-from opentps.gui.viewer.exportWindow import ExportWindow
-from opentps.gui.tools._cropTool import CropWidget
-from opentps.gui.tools._resampleTool import ResampleWidget
-from opentps.gui.programSettingEditor import ProgramSettingEditor
-
-import opentps.gui.res.icons as IconModule
-
-class ViewerToolbar(QToolBar):
-
-    PLAY_STATUS = 1
-    PAUSE_STATUS = 0
-
-    def __init__(self, viewController, parent=None):
-        super().__init__(parent)
-
-        self._viewController = viewController
-        self._cropWidgets = []
-        self._resampleWidgets = []
-
-        self.setIconSize(QSize(16, 16))
-
-        self.iconPath = str(IconModule.__path__[0]) + os.path.sep
-
-        self._buttonSettings = QAction(QIcon(self.iconPath + "settings-5-line.png"), "Settings", self)
-        self._buttonSettings.triggered.connect(self._openSettings)
-
-        self._buttonOpen = QAction(QIcon(self.iconPath + "folder-open.png"), "Open files or folder", self)
-        self._buttonOpen.setStatusTip("Open files or folder")
-        self._buttonOpen.triggered.connect(self._handleLoadData)
-        self._buttonOpen.setCheckable(False)
-
-        self._buttonSave = QAction(QIcon(self.iconPath + "save.png"), "Export", self)
-        self._buttonSave.triggered.connect(self._handleExportData)
-
-        self._buttonIndependentViews = QAction(QIcon(self.iconPath + "independent_views.png"), "Independent views", self)
-        self._buttonIndependentViews.setStatusTip("Independent views")
-        self._buttonIndependentViews.triggered.connect(self._handleButtonIndependentViews)
-        self._buttonIndependentViews.setCheckable(True)
-        self._buttonIndependentViews.setChecked(self._viewController.independentViewsEnabled)
-
-        self._buttonWindowLevel = QAction(QIcon(self.iconPath + "contrast.png"), "Window level", self)
-        self._buttonWindowLevel.setStatusTip("Window level")
-        self._buttonWindowLevel.triggered.connect(self._handleWindowLevel)
-        self._buttonWindowLevel.setCheckable(True)
-
-        self._buttonCrossHair = QAction(QIcon(self.iconPath + "geolocation.png"), "Crosshair", self)
-        self._buttonCrossHair.setStatusTip("Crosshair")
-        self._buttonCrossHair.triggered.connect(self._handleCrossHair)
-        self._buttonCrossHair.setCheckable(True)
-
-        self._buttonCrop = QAction(QIcon(self.iconPath + "crop.png"), "Crop", self)
-        self._buttonCrop.setStatusTip("Crop")
-        self._buttonCrop.triggered.connect(self._handleCrop)
-        self._buttonCrop.setCheckable(False)
-
-        self._buttonResample = QAction(QIcon(self.iconPath + "resample.png"), "Resample", self)
-        self._buttonResample.setStatusTip("Resample")
-        self._buttonResample.triggered.connect(self._handleResample)
-        self._buttonResample.setCheckable(False)
-
-        self._dropModeCombo = QComboBox()
-        self._dropModeToStr = {DataViewer.DropModes.AUTO: 'Drop mode: auto',
-                               DataViewer.DropModes.PRIMARY: 'Drop as primary image',
-                               DataViewer.DropModes.SECONDARY: 'Drop as secondaryImage'}
-        self._strToDropMode = {v: k for k, v in self._dropModeToStr.items()}
-        self._dropModeCombo.addItems(list(self._dropModeToStr.values()))
-        self._dropModeCombo.setCurrentIndex(self._dropModeToIndex(self._viewController.dropMode))
-        self._dropModeCombo.currentIndexChanged.connect(self._handleDropModeSelection)
-        self._dropModeAction = QWidgetAction(None)
-        self._dropModeAction.setDefaultWidget(self._dropModeCombo)
-
-        self.addAction(self._buttonSettings)
-        self.addAction(self._buttonOpen)
-        self.addAction(self._buttonSave)
-        self.addAction(self._buttonIndependentViews)
-        self.addAction(self._buttonCrossHair)
-        self.addAction(self._buttonWindowLevel)
-        self.addAction(self._buttonCrop)
-        self.addAction(self._buttonResample)
-        self.addAction(self._dropModeAction)
-
-        self.addSeparator()
-
-        ## dynamic options buttons
-        self._buttonFaster = QAction(QIcon(self.iconPath + "fast.png"), "Faster", self)
-        self._buttonFaster.setStatusTip("Speed up the dynamic viewers evolution")
-        self._buttonFaster.triggered.connect(self._handleFaster)
-
-        self._buttonSlower = QAction(QIcon(self.iconPath + "slow.png"), "Slower", self)
-        self._buttonSlower.setStatusTip("Slows the dynamic viewers evolution")
-        self._buttonSlower.triggered.connect(self._handleSlower)
-
-        self._buttonPlayPause = QAction(QIcon(self.iconPath + "play.png"), "Play/Pause", self)
-        self._buttonPlayPause.setStatusTip("Classical Play Pause of course")
-        self._buttonPlayPause.triggered.connect(self._handlePlayPause)
-        self.playPauseStatus = self.PLAY_STATUS
-
-        self._buttonRefreshRate = QAction('RR', self)
-        self._buttonRefreshRate.setStatusTip("Change the refresh rate of the dynamic viewers")
-        self._buttonRefreshRate.triggered.connect(self._handleRefreshRate)
-
-        self.fasterSignal = Event()
-        self.slowerSignal = Event()
-        self.playPauseSignal = Event(bool)
-        self.refreshRateChangedSignal = Event(float)
-        self.refreshRateValue = 24
-        # self.addDynamicButtons()
-
-        self._viewController.independentViewsEnabledSignal.connect(self._handleButtonIndependentViews)
-        self._viewController.windowLevelEnabledSignal.connect(self._handleWindowLevel)
-        self._viewController.crossHairEnabledSignal.connect(self._handleCrossHair)
-
-    def _dropModeToIndex(self, dropMode):
-        return list(self._dropModeToStr.keys()).index(dropMode)
-
-    def _indexToDropMode(self, index):
-        return list(self._dropModeToStr.keys())[index]
-
-    def _handleDropModeSelection(self, selectionIndex):
-        self._viewController.dropMode = self._indexToDropMode(selectionIndex)
-
-    def _openSettings(self, pressed):
-        self._settingEditor = ProgramSettingEditor()
-        self._settingEditor.show()
-
-    def _handleButtonIndependentViews(self, pressed):
-        # This is useful if controller emit a signal:
-        if self._buttonIndependentViews.isChecked() != pressed:
-            self._buttonIndependentViews.setChecked(pressed)
-            return
-
-        self._viewController.independentViewsEnabled = pressed
-
-    def _handleCrossHair(self, pressed):
-        # This is useful if controller emit a signal:
-        if self._buttonCrossHair.isChecked() != pressed:
-            self._buttonCrossHair.setChecked(pressed)
-            return
-
-        self._viewController.crossHairEnabled = pressed
-
-    def _handleCrop(self):
-        cw = CropWidget(self._viewController)
-        # TODO
-        # I don't know why but we must keep the reference to any CropWidget created even if we close it
-        # This is an issue because _cropWidgets might become huge
-        self._cropWidgets.append(cw)
-        cw.show()
-
-    def _handleResample(self):
-        rw = ResampleWidget(self._viewController)
-        self._resampleWidgets.append(rw)
-        rw.show()
-
-    def _handleLoadData(self):
-        filesOrFoldersList = self._getOpenFilesAndDirs(caption="Open patient data files or folders",
-                                                  directory=QDir.currentPath())
-        if len(filesOrFoldersList) < 1:
-            return
-
-        splitPath = filesOrFoldersList[0].split('/')
-        withoutLastElementPath = ''
-        for element in splitPath[:-1]:
-            withoutLastElementPath += element + '/'
-        self.dataPath = withoutLastElementPath
-
-        dataLoader.loadData(self._viewController._patientList, filesOrFoldersList)
-
-    def _handleExportData(self):
-        self._exportWindow = ExportWindow(self._viewController)
-        self._exportWindow.show()
-
-    def _handleWindowLevel(self, pressed):
-        # This is useful if controller emit a signal:
-        if self._buttonWindowLevel.isChecked() != pressed:
-            self._buttonWindowLevel.setChecked(pressed)
-            return
-
-        self._viewController.windowLevelEnabled = pressed
-
-    def addDynamicButtons(self):
-
-        self.addAction(self._buttonSlower)
-        self.addAction(self._buttonPlayPause)
-        self._buttonPlayPause.setIcon(QIcon(self.iconPath + "pause.jpg"))
-        self.addAction(self._buttonFaster)
-        self.addAction(self._buttonRefreshRate)
-
-    def removeDynamicButtons(self):
-
-        self.removeAction(self._buttonSlower)
-        self.removeAction(self._buttonPlayPause)
-        self.removeAction(self._buttonFaster)
-        self.removeAction(self._buttonRefreshRate)
-
-    def _handleFaster(self):
-        self.fasterSignal.emit()
-
-
-    def _handleSlower(self):
-        self.slowerSignal.emit()
-
-
-    def _handlePlayPause(self):
-        self.playPauseStatus = not self.playPauseStatus
-
-        if self.playPauseStatus:
-            self._buttonPlayPause.setIcon(QIcon(self.iconPath + "pause.jpg"))
-        elif not self.playPauseStatus:
-            self._buttonPlayPause.setIcon(QIcon(self.iconPath + "play.png"))
-
-        self.playPauseSignal.emit(self.playPauseStatus)
-
-
-    def _handleRefreshRate(self):
-
-        refreshRateDialog = RefreshRateDialog(self.refreshRateValue)
-
-        if (refreshRateDialog.exec()):
-            self.refreshRateValue = float(refreshRateDialog.rRValueLine.text())
-            self.refreshRateChangedSignal.emit(self.refreshRateValue)
-
-    # TODO : this is duplicated from patientDataPanel
-    def _getOpenFilesAndDirs(self, parent=None, caption='', directory='',
-                             filter='', initialFilter='', options=None):
-        def updateText():
-            # update the contents of the line edit widget with the selected files
-            selected = []
-            for index in view.selectionModel().selectedRows():
-                selected.append('"{}"'.format(index.data()))
-            lineEdit.setText(' '.join(selected))
-
-        dialog = QFileDialog(parent, windowTitle=caption)
-        dialog.setFileMode(dialog.ExistingFiles)
-        if options:
-            dialog.setOptions(options)
-        dialog.setOption(dialog.DontUseNativeDialog, True)
-        if directory:
-            dialog.setDirectory(directory)
-        if filter:
-            dialog.setNameFilter(filter)
-            if initialFilter:
-                dialog.selectNameFilter(initialFilter)
-
-        # by default, if a directory is opened in file listing mode,
-        # QFileDialog.accept() shows the contents of that directory, but we
-        # need to be able to "open" directories as we can do with files, so we
-        # just override accept() with the default QDialog implementation which
-        # will just return exec_()
-        dialog.accept = lambda: QDialog.accept(dialog)
-
-        # there are many item views in a non-native dialog, but the ones displaying
-        # the actual contents are created inside a QStackedWidget; they are a
-        # QTreeView and a QListView, and the tree is only used when the
-        # viewMode is set to QFileDialog.Details, which is not this case
-        stackedWidget = dialog.findChild(QStackedWidget)
-        view = stackedWidget.findChild(QListView)
-        view.selectionModel().selectionChanged.connect(updateText)
-
-        lineEdit = dialog.findChild(QLineEdit)
-        # clear the line edit contents whenever the current directory changes
-        dialog.directoryEntered.connect(lambda: lineEdit.setText(''))
-
-        dialog.exec_()
-        return dialog.selectedFiles()
-
-
-class RefreshRateDialog(QDialog):
-
-    def __init__(self, refreshRateValue):
-        QDialog.__init__(self)
-
-        self.RRVal = refreshRateValue
-
-        self.main_layout = QVBoxLayout()
-        self.setLayout(self.main_layout)
-
-        # self.slider = QScrollBar(self)   ## to select the refresh rate with a scroll bar, not used for now
-        # self.slider.setOrientation(Qt.Horizontal)
-        # self.slider.sliderMoved.connect(self.sliderval)
-        # self.main_layout.addWidget(self.slider)
-
-        self.rRValueLine = QLineEdit(str(self.RRVal))
-        self.main_layout.addWidget(self.rRValueLine)
-
-        okButton = QPushButton("ok", self)
-        okButton.clicked.connect(self.accept)
-        self.main_layout.addWidget(okButton)
-
-
-    def sliderval(self):
-        # getting current position of the slider
-        value = self.slider.sliderPosition()
+
+import os
+
+from PyQt5.QtCore import QSize, QDir
+from PyQt5.QtGui import QIcon
+from PyQt5.QtWidgets import QToolBar, QAction, QDialog, QPushButton, QLineEdit, QVBoxLayout, QFileDialog, \
+    QStackedWidget, QListView, QComboBox, QWidgetAction
+
+from opentps.core.io import dataLoader
+from opentps.core import Event
+from opentps.gui.viewer.dataViewer import DataViewer
+from opentps.gui.viewer.exportWindow import ExportWindow
+from opentps.gui.tools._cropTool import CropWidget
+from opentps.gui.tools._resampleTool import ResampleWidget
+from opentps.gui.programSettingEditor import ProgramSettingEditor
+
+import opentps.gui.res.icons as IconModule
+
+class ViewerToolbar(QToolBar):
+
+    PLAY_STATUS = 1
+    PAUSE_STATUS = 0
+
+    def __init__(self, viewController, parent=None):
+        super().__init__(parent)
+
+        self._viewController = viewController
+        self._cropWidgets = []
+        self._resampleWidgets = []
+
+        self.setIconSize(QSize(16, 16))
+
+        self.iconPath = str(IconModule.__path__[0]) + os.path.sep
+
+        self._buttonSettings = QAction(QIcon(self.iconPath + "settings-5-line.png"), "Settings", self)
+        self._buttonSettings.triggered.connect(self._openSettings)
+
+        self._buttonOpen = QAction(QIcon(self.iconPath + "folder-open.png"), "Open files or folder", self)
+        self._buttonOpen.setStatusTip("Open files or folder")
+        self._buttonOpen.triggered.connect(self._handleLoadData)
+        self._buttonOpen.setCheckable(False)
+
+        self._buttonSave = QAction(QIcon(self.iconPath + "save.png"), "Export", self)
+        self._buttonSave.triggered.connect(self._handleExportData)
+
+        self._buttonIndependentViews = QAction(QIcon(self.iconPath + "independent_views.png"), "Independent views", self)
+        self._buttonIndependentViews.setStatusTip("Independent views")
+        self._buttonIndependentViews.triggered.connect(self._handleButtonIndependentViews)
+        self._buttonIndependentViews.setCheckable(True)
+        self._buttonIndependentViews.setChecked(self._viewController.independentViewsEnabled)
+
+        self._buttonWindowLevel = QAction(QIcon(self.iconPath + "contrast.png"), "Window level", self)
+        self._buttonWindowLevel.setStatusTip("Window level")
+        self._buttonWindowLevel.triggered.connect(self._handleWindowLevel)
+        self._buttonWindowLevel.setCheckable(True)
+
+        self._buttonCrossHair = QAction(QIcon(self.iconPath + "geolocation.png"), "Crosshair", self)
+        self._buttonCrossHair.setStatusTip("Crosshair")
+        self._buttonCrossHair.triggered.connect(self._handleCrossHair)
+        self._buttonCrossHair.setCheckable(True)
+
+        self._buttonCrop = QAction(QIcon(self.iconPath + "crop.png"), "Crop", self)
+        self._buttonCrop.setStatusTip("Crop")
+        self._buttonCrop.triggered.connect(self._handleCrop)
+        self._buttonCrop.setCheckable(False)
+
+        self._buttonResample = QAction(QIcon(self.iconPath + "resample.png"), "Resample", self)
+        self._buttonResample.setStatusTip("Resample")
+        self._buttonResample.triggered.connect(self._handleResample)
+        self._buttonResample.setCheckable(False)
+
+        self._dropModeCombo = QComboBox()
+        self._dropModeToStr = {DataViewer.DropModes.AUTO: 'Drop mode: auto',
+                               DataViewer.DropModes.PRIMARY: 'Drop as primary image',
+                               DataViewer.DropModes.SECONDARY: 'Drop as secondaryImage'}
+        self._strToDropMode = {v: k for k, v in self._dropModeToStr.items()}
+        self._dropModeCombo.addItems(list(self._dropModeToStr.values()))
+        self._dropModeCombo.setCurrentIndex(self._dropModeToIndex(self._viewController.dropMode))
+        self._dropModeCombo.currentIndexChanged.connect(self._handleDropModeSelection)
+        self._dropModeAction = QWidgetAction(None)
+        self._dropModeAction.setDefaultWidget(self._dropModeCombo)
+
+        self.addAction(self._buttonSettings)
+        self.addAction(self._buttonOpen)
+        self.addAction(self._buttonSave)
+        self.addAction(self._buttonIndependentViews)
+        self.addAction(self._buttonCrossHair)
+        self.addAction(self._buttonWindowLevel)
+        self.addAction(self._buttonCrop)
+        self.addAction(self._buttonResample)
+        self.addAction(self._dropModeAction)
+
+        self.addSeparator()
+
+        ## dynamic options buttons
+        self._buttonFaster = QAction(QIcon(self.iconPath + "fast.png"), "Faster", self)
+        self._buttonFaster.setStatusTip("Speed up the dynamic viewers evolution")
+        self._buttonFaster.triggered.connect(self._handleFaster)
+
+        self._buttonSlower = QAction(QIcon(self.iconPath + "slow.png"), "Slower", self)
+        self._buttonSlower.setStatusTip("Slows the dynamic viewers evolution")
+        self._buttonSlower.triggered.connect(self._handleSlower)
+
+        self._buttonPlayPause = QAction(QIcon(self.iconPath + "play.png"), "Play/Pause", self)
+        self._buttonPlayPause.setStatusTip("Classical Play Pause of course")
+        self._buttonPlayPause.triggered.connect(self._handlePlayPause)
+        self.playPauseStatus = self.PLAY_STATUS
+
+        self._buttonRefreshRate = QAction('RR', self)
+        self._buttonRefreshRate.setStatusTip("Change the refresh rate of the dynamic viewers")
+        self._buttonRefreshRate.triggered.connect(self._handleRefreshRate)
+
+        self.fasterSignal = Event()
+        self.slowerSignal = Event()
+        self.playPauseSignal = Event(bool)
+        self.refreshRateChangedSignal = Event(float)
+        self.refreshRateValue = 24
+        # self.addDynamicButtons()
+
+        self._viewController.independentViewsEnabledSignal.connect(self._handleButtonIndependentViews)
+        self._viewController.windowLevelEnabledSignal.connect(self._handleWindowLevel)
+        self._viewController.crossHairEnabledSignal.connect(self._handleCrossHair)
+
+    def _dropModeToIndex(self, dropMode):
+        return list(self._dropModeToStr.keys()).index(dropMode)
+
+    def _indexToDropMode(self, index):
+        return list(self._dropModeToStr.keys())[index]
+
+    def _handleDropModeSelection(self, selectionIndex):
+        self._viewController.dropMode = self._indexToDropMode(selectionIndex)
+
+    def _openSettings(self, pressed):
+        self._settingEditor = ProgramSettingEditor()
+        self._settingEditor.show()
+
+    def _handleButtonIndependentViews(self, pressed):
+        # This is useful if controller emit a signal:
+        if self._buttonIndependentViews.isChecked() != pressed:
+            self._buttonIndependentViews.setChecked(pressed)
+            return
+
+        self._viewController.independentViewsEnabled = pressed
+
+    def _handleCrossHair(self, pressed):
+        # This is useful if controller emit a signal:
+        if self._buttonCrossHair.isChecked() != pressed:
+            self._buttonCrossHair.setChecked(pressed)
+            return
+
+        self._viewController.crossHairEnabled = pressed
+
+    def _handleCrop(self):
+        cw = CropWidget(self._viewController)
+        # TODO
+        # I don't know why but we must keep the reference to any CropWidget created even if we close it
+        # This is an issue because _cropWidgets might become huge
+        self._cropWidgets.append(cw)
+        cw.show()
+
+    def _handleResample(self):
+        rw = ResampleWidget(self._viewController)
+        self._resampleWidgets.append(rw)
+        rw.show()
+
+    def _handleLoadData(self):
+        filesOrFoldersList = self._getOpenFilesAndDirs(caption="Open patient data files or folders",
+                                                  directory=QDir.currentPath())
+        if len(filesOrFoldersList) < 1:
+            return
+
+        splitPath = filesOrFoldersList[0].split('/')
+        withoutLastElementPath = ''
+        for element in splitPath[:-1]:
+            withoutLastElementPath += element + '/'
+        self.dataPath = withoutLastElementPath
+
+        dataLoader.loadData(self._viewController._patientList, filesOrFoldersList)
+
+    def _handleExportData(self):
+        self._exportWindow = ExportWindow(self._viewController)
+        self._exportWindow.show()
+
+    def _handleWindowLevel(self, pressed):
+        # This is useful if controller emit a signal:
+        if self._buttonWindowLevel.isChecked() != pressed:
+            self._buttonWindowLevel.setChecked(pressed)
+            return
+
+        self._viewController.windowLevelEnabled = pressed
+
+    def addDynamicButtons(self):
+
+        self.addAction(self._buttonSlower)
+        self.addAction(self._buttonPlayPause)
+        self._buttonPlayPause.setIcon(QIcon(self.iconPath + "pause.jpg"))
+        self.addAction(self._buttonFaster)
+        self.addAction(self._buttonRefreshRate)
+
+    def removeDynamicButtons(self):
+
+        self.removeAction(self._buttonSlower)
+        self.removeAction(self._buttonPlayPause)
+        self.removeAction(self._buttonFaster)
+        self.removeAction(self._buttonRefreshRate)
+
+    def _handleFaster(self):
+        self.fasterSignal.emit()
+
+
+    def _handleSlower(self):
+        self.slowerSignal.emit()
+
+
+    def _handlePlayPause(self):
+        self.playPauseStatus = not self.playPauseStatus
+
+        if self.playPauseStatus:
+            self._buttonPlayPause.setIcon(QIcon(self.iconPath + "pause.jpg"))
+        elif not self.playPauseStatus:
+            self._buttonPlayPause.setIcon(QIcon(self.iconPath + "play.png"))
+
+        self.playPauseSignal.emit(self.playPauseStatus)
+
+
+    def _handleRefreshRate(self):
+
+        refreshRateDialog = RefreshRateDialog(self.refreshRateValue)
+
+        if (refreshRateDialog.exec()):
+            self.refreshRateValue = float(refreshRateDialog.rRValueLine.text())
+            self.refreshRateChangedSignal.emit(self.refreshRateValue)
+
+    # TODO : this is duplicated from patientDataPanel
+    def _getOpenFilesAndDirs(self, parent=None, caption='', directory='',
+                             filter='', initialFilter='', options=None):
+        def updateText():
+            # update the contents of the line edit widget with the selected files
+            selected = []
+            for index in view.selectionModel().selectedRows():
+                selected.append('"{}"'.format(index.data()))
+            lineEdit.setText(' '.join(selected))
+
+        dialog = QFileDialog(parent, windowTitle=caption)
+        dialog.setFileMode(dialog.ExistingFiles)
+        if options:
+            dialog.setOptions(options)
+        dialog.setOption(dialog.DontUseNativeDialog, True)
+        if directory:
+            dialog.setDirectory(directory)
+        if filter:
+            dialog.setNameFilter(filter)
+            if initialFilter:
+                dialog.selectNameFilter(initialFilter)
+
+        # by default, if a directory is opened in file listing mode,
+        # QFileDialog.accept() shows the contents of that directory, but we
+        # need to be able to "open" directories as we can do with files, so we
+        # just override accept() with the default QDialog implementation which
+        # will just return exec_()
+        dialog.accept = lambda: QDialog.accept(dialog)
+
+        # there are many item views in a non-native dialog, but the ones displaying
+        # the actual contents are created inside a QStackedWidget; they are a
+        # QTreeView and a QListView, and the tree is only used when the
+        # viewMode is set to QFileDialog.Details, which is not this case
+        stackedWidget = dialog.findChild(QStackedWidget)
+        view = stackedWidget.findChild(QListView)
+        view.selectionModel().selectionChanged.connect(updateText)
+
+        lineEdit = dialog.findChild(QLineEdit)
+        # clear the line edit contents whenever the current directory changes
+        dialog.directoryEntered.connect(lambda: lineEdit.setText(''))
+
+        dialog.exec_()
+        return dialog.selectedFiles()
+
+
+class RefreshRateDialog(QDialog):
+
+    def __init__(self, refreshRateValue):
+        QDialog.__init__(self)
+
+        self.RRVal = refreshRateValue
+
+        self.main_layout = QVBoxLayout()
+        self.setLayout(self.main_layout)
+
+        # self.slider = QScrollBar(self)   ## to select the refresh rate with a scroll bar, not used for now
+        # self.slider.setOrientation(Qt.Horizontal)
+        # self.slider.sliderMoved.connect(self.sliderval)
+        # self.main_layout.addWidget(self.slider)
+
+        self.rRValueLine = QLineEdit(str(self.RRVal))
+        self.main_layout.addWidget(self.rRValueLine)
+
+        okButton = QPushButton("ok", self)
+        okButton.clicked.connect(self.accept)
+        self.main_layout.addWidget(okButton)
+
+
+    def sliderval(self):
+        # getting current position of the slider
+        value = self.slider.sliderPosition()
```

### Comparing `opentps-gui-1.0.4/PKG-INFO` & `opentps_gui-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,102 @@
 Metadata-Version: 2.1
 Name: opentps-gui
-Version: 1.0.4
+Version: 1.0.5
 Summary: Open source TPS for advanced proton therapy
 Home-page: http://opentps.org/
 License: GPLv3
 Author: Sylvain Deffet
 Author-email: sylvaindeffet@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: PyQt5 (==5.14)
-Requires-Dist: SimpleITK (>=2.1.1,<3.0.0)
-Requires-Dist: numpy (>=1.23.2,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: pydicom (>=2.3.0,<3.0.0)
-Requires-Dist: pyqtgraph (>=0.12.4,<0.13.0)
-Requires-Dist: setuptools (>=61.0.0,<62.0.0)
-Requires-Dist: sparse-dot-mkl (>=0.8.2,<0.9.0)
-Requires-Dist: vtk (>=9.1.0,<10.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.4.0,<10.0.0)
+Requires-Dist: PyQt5 (>=5.15.7,<6.0.0)
+Requires-Dist: SimpleITK (>=2.2.1,<3.0.0)
+Requires-Dist: cachecontrol
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pydicom (>=2.4.1,<3.0.0)
+Requires-Dist: pyqtgraph (>=0.13.1,<0.14.0)
+Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: sparse-dot-mkl (>=0.8.3,<0.9.0)
+Requires-Dist: vtk (>=9.2.6,<10.0.0)
 Description-Content-Type: text/markdown
 
 # opentps-gui
 
 GUI of opentps, a Python application for treatment planning in proton therapy, based on the MCsquare Monte Carlo dose engine.
 
-
 ## Installation (Linux):
+
 Requirements are listed in pyproject.toml.
 To install all required dependencies:
-``` 
+
+```
 poetry install
-``` 
+```
 
 Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
 
-
 ## Installation (Windows):
+
 Note: VTK is only compatible with Python version <= 3.9. Do not use Python 3.10
 
-1) Install anaconda on your Windows computer
+1. Install anaconda on your Windows computer
 
-2) Open Anaconda Prompt (via the Anaconda application)
+2. Open Anaconda Prompt (via the Anaconda application)
 
-3) Create a new Anaconda environment:
-``` 
+3. Create a new Anaconda environment:
+
+```
 conda create --name OpenTPS python=3.8
-``` 
+```
+
+4. Activate the new environment:
 
-4) Activate the new environment:
-``` 
+```
 conda activate OpenTPS
-``` 
+```
+
+5. Install the following python modules:
+   Python modules:
 
-5) Install the following python modules:
-Python modules:
-``` 
-pip3 install --upgrade --user pip
-pip3 install --user pydicom
-pip3 install --user numpy
-pip3 install --user scipy
-pip3 install --user matplotlib
-pip3 install --user Pillow
-pip3 install --user PyQt5==5.14
-pip3 install --user pyqtgraph
-pip3 install --user sparse_dot_mkl
-pip3 install --user vtk
-pip3 install --user SimpleITK
-pip3 install --user pandas
+```
+pip3 install --upgrade pip
+pip3 install pydicom
+pip3 install numpy
+pip3 install scipy
+pip3 install matplotlib
+pip3 install Pillow
+pip3 install PyQt5==5.15.7
+pip3 install pyqtgraph
+pip3 install sparse_dot_mkl
+pip3 install vtk
+pip3 install SimpleITK
+pip3 install pandas
 pip3
 ```
 
 Optional python modules:
-``` 
-pip3 install --user tensorflow
-pip3 install --user keras
-pip3 install --user cupy
-```
 
+```
+pip3 install tensorflow
+pip3 install keras
+pip3 install cupy
+```
 
 ## Run:
+
 ```
 python3 main.py
 ```
 
 or from a python script:
 
 ```python
 import opentps.gui as opentps_gui
 opentps_gui.run()
 ```
 
-
```

