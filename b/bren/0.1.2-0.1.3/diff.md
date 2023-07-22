# Comparing `tmp/bren-0.1.2.tar.gz` & `tmp/bren-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bren-0.1.2.tar", last modified: Fri Jul 21 17:59:48 2023, max compression
+gzip compressed data, was "bren-0.1.3.tar", last modified: Fri Jul 21 21:29:58 2023, max compression
```

## Comparing `bren-0.1.2.tar` & `bren-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.591813 bren-0.1.2/
--rw-rw-rw-   0        0        0     3726 2023-07-14 18:16:17.000000 bren-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1347 2023-07-21 17:59:48.590819 bren-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-07-11 12:31:10.000000 bren-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.365366 bren-0.1.2/bren/
--rw-rw-rw-   0        0        0     1923 2023-07-15 20:46:11.000000 bren-0.1.2/bren/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.413289 bren-0.1.2/bren/autodiff/
--rw-rw-rw-   0        0        0        0 2023-01-04 21:18:47.000000 bren-0.1.2/bren/autodiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.447199 bren-0.1.2/bren/autodiff/nodes/
--rw-rw-rw-   0        0        0      442 2023-01-07 21:45:46.000000 bren-0.1.2/bren/autodiff/nodes/Const.py
--rw-rw-rw-   0        0        0     1632 2023-07-11 18:40:11.000000 bren-0.1.2/bren/autodiff/nodes/Graph.py
--rw-rw-rw-   0        0        0      343 2023-01-15 20:42:35.000000 bren-0.1.2/bren/autodiff/nodes/Node.py
--rw-rw-rw-   0        0        0      542 2023-07-10 15:39:02.000000 bren-0.1.2/bren/autodiff/nodes/Operator.py
--rw-rw-rw-   0        0        0      369 2023-01-03 21:07:13.000000 bren-0.1.2/bren/autodiff/nodes/Var.py
--rw-rw-rw-   0        0        0      276 2023-01-03 21:39:06.000000 bren-0.1.2/bren/autodiff/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.452186 bren-0.1.2/bren/autodiff/operations/
--rw-rw-rw-   0        0        0        0 2023-07-21 17:41:51.000000 bren-0.1.2/bren/autodiff/operations/__init__.py
--rw-rw-rw-   0        0        0     4916 2023-07-11 15:10:50.000000 bren-0.1.2/bren/autodiff/operations/ops.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.461164 bren-0.1.2/bren/core/
--rw-rw-rw-   0        0        0     4387 2023-07-18 18:33:41.000000 bren-0.1.2/bren/core/Array.py
--rw-rw-rw-   0        0        0      121 2023-07-21 17:23:23.000000 bren-0.1.2/bren/core/__init__.py
--rw-rw-rw-   0        0        0     1128 2023-07-21 15:02:52.000000 bren-0.1.2/bren/core/core.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.465151 bren-0.1.2/bren/nn/
--rw-rw-rw-   0        0        0      458 2023-03-15 22:57:21.000000 bren-0.1.2/bren/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.488090 bren-0.1.2/bren/nn/activations/
--rw-rw-rw-   0        0        0      578 2023-07-12 20:33:26.000000 bren-0.1.2/bren/nn/activations/Activation.py
--rw-rw-rw-   0        0        0     1101 2023-07-12 15:17:05.000000 bren-0.1.2/bren/nn/activations/ELU.py
--rw-rw-rw-   0        0        0      375 2023-07-12 15:18:00.000000 bren-0.1.2/bren/nn/activations/Linear.py
--rw-rw-rw-   0        0        0     1103 2023-07-12 15:25:53.000000 bren-0.1.2/bren/nn/activations/ReLU.py
--rw-rw-rw-   0        0        0      405 2023-07-12 15:17:52.000000 bren-0.1.2/bren/nn/activations/Tanh.py
--rw-rw-rw-   0        0        0      648 2023-07-08 17:47:09.000000 bren-0.1.2/bren/nn/activations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.494075 bren-0.1.2/bren/nn/datasets/
--rw-rw-rw-   0        0        0       73 2023-03-15 22:57:55.000000 bren-0.1.2/bren/nn/datasets/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-07-21 17:56:16.000000 bren-0.1.2/bren/nn/datasets/mnist.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.509035 bren-0.1.2/bren/nn/initialisers/
--rw-rw-rw-   0        0        0      707 2023-07-13 20:06:12.000000 bren-0.1.2/bren/nn/initialisers/GlorotNormal.py
--rw-rw-rw-   0        0        0      676 2023-07-14 18:18:10.000000 bren-0.1.2/bren/nn/initialisers/GlorotUniform.py
--rw-rw-rw-   0        0        0      605 2023-07-14 18:17:50.000000 bren-0.1.2/bren/nn/initialisers/HeNormal.py
--rw-rw-rw-   0        0        0      576 2023-07-14 18:18:02.000000 bren-0.1.2/bren/nn/initialisers/HeUniform.py
--rw-rw-rw-   0        0        0      916 2023-07-15 21:06:02.000000 bren-0.1.2/bren/nn/initialisers/Initialiser.py
--rw-rw-rw-   0        0        0      884 2023-01-22 20:44:45.000000 bren-0.1.2/bren/nn/initialisers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.525989 bren-0.1.2/bren/nn/layers/
--rw-rw-rw-   0        0        0      460 2023-07-14 18:46:16.000000 bren-0.1.2/bren/nn/layers/Flatten.py
--rw-rw-rw-   0        0        0     3550 2023-07-14 18:41:54.000000 bren-0.1.2/bren/nn/layers/FullyConnected.py
--rw-rw-rw-   0        0        0     2115 2023-07-15 16:42:56.000000 bren-0.1.2/bren/nn/layers/Layer.py
--rw-rw-rw-   0        0        0      537 2023-07-14 18:51:56.000000 bren-0.1.2/bren/nn/layers/Softmax.py
--rw-rw-rw-   0        0        0      265 2023-07-14 18:26:44.000000 bren-0.1.2/bren/nn/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.535974 bren-0.1.2/bren/nn/losses/
--rw-rw-rw-   0        0        0      485 2023-07-20 21:16:06.000000 bren-0.1.2/bren/nn/losses/CatrgoricalCrossEntropy.py
--rw-rw-rw-   0        0        0      460 2023-07-20 16:45:14.000000 bren-0.1.2/bren/nn/losses/Loss.py
--rw-rw-rw-   0        0        0      406 2023-07-20 16:42:39.000000 bren-0.1.2/bren/nn/losses/MeanSquaredError.py
--rw-rw-rw-   0        0        0      538 2023-03-11 22:55:20.000000 bren-0.1.2/bren/nn/losses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.550922 bren-0.1.2/bren/nn/metrics/
--rw-rw-rw-   0        0        0      963 2023-07-14 22:13:36.000000 bren-0.1.2/bren/nn/metrics/Accuracy.py
--rw-rw-rw-   0        0        0      696 2023-07-14 21:23:20.000000 bren-0.1.2/bren/nn/metrics/CategoricalCrossEntropy.py
--rw-rw-rw-   0        0        0      580 2023-07-14 21:24:06.000000 bren-0.1.2/bren/nn/metrics/MeanSquaredError.py
--rw-rw-rw-   0        0        0     1123 2023-07-20 21:08:15.000000 bren-0.1.2/bren/nn/metrics/Metric.py
--rw-rw-rw-   0        0        0     1179 2023-07-20 21:04:44.000000 bren-0.1.2/bren/nn/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.561895 bren-0.1.2/bren/nn/models/
--rw-rw-rw-   0        0        0     6944 2023-07-20 21:17:00.000000 bren-0.1.2/bren/nn/models/Model.py
--rw-rw-rw-   0        0        0      975 2023-07-20 16:02:19.000000 bren-0.1.2/bren/nn/models/Sequential.py
--rw-rw-rw-   0        0        0     1293 2023-07-21 12:51:34.000000 bren-0.1.2/bren/nn/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.580849 bren-0.1.2/bren/nn/optimisers/
--rw-rw-rw-   0        0        0      667 2023-07-15 20:30:49.000000 bren-0.1.2/bren/nn/optimisers/AdaGrad.py
--rw-rw-rw-   0        0        0      999 2023-06-25 20:52:03.000000 bren-0.1.2/bren/nn/optimisers/Adam.py
--rw-rw-rw-   0        0        0      716 2023-07-15 17:49:17.000000 bren-0.1.2/bren/nn/optimisers/Optimiser.py
--rw-rw-rw-   0        0        0      748 2023-02-04 22:07:59.000000 bren-0.1.2/bren/nn/optimisers/RMSProp.py
--rw-rw-rw-   0        0        0      647 2023-07-10 16:19:29.000000 bren-0.1.2/bren/nn/optimisers/SGD.py
--rw-rw-rw-   0        0        0      730 2023-03-11 23:14:11.000000 bren-0.1.2/bren/nn/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.586829 bren-0.1.2/bren/nn/preprocessing/
--rw-rw-rw-   0        0        0      138 2023-03-15 21:55:23.000000 bren-0.1.2/bren/nn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-07-15 18:27:34.000000 bren-0.1.2/bren/nn/preprocessing/utils.py
--rw-rw-rw-   0        0        0     1026 2023-07-15 20:34:41.000000 bren-0.1.2/bren/nn/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:59:48.410297 bren-0.1.2/bren.egg-info/
--rw-rw-rw-   0        0        0     1347 2023-07-21 17:59:48.000000 bren-0.1.2/bren.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1740 2023-07-21 17:59:48.000000 bren-0.1.2/bren.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 17:59:48.000000 bren-0.1.2/bren.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-21 17:59:48.000000 bren-0.1.2/bren.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-21 17:59:48.000000 bren-0.1.2/bren.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 17:59:48.591813 bren-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-07-21 17:59:39.000000 bren-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.799435 bren-0.1.3/
+-rw-rw-rw-   0        0        0     3726 2023-07-14 18:16:17.000000 bren-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1347 2023-07-21 21:29:58.798206 bren-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-07-11 12:31:10.000000 bren-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.472129 bren-0.1.3/bren/
+-rw-rw-rw-   0        0        0     1923 2023-07-15 20:46:11.000000 bren-0.1.3/bren/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.500608 bren-0.1.3/bren/autodiff/
+-rw-rw-rw-   0        0        0        0 2023-01-04 21:18:47.000000 bren-0.1.3/bren/autodiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.526212 bren-0.1.3/bren/autodiff/nodes/
+-rw-rw-rw-   0        0        0      442 2023-01-07 21:45:46.000000 bren-0.1.3/bren/autodiff/nodes/Const.py
+-rw-rw-rw-   0        0        0     1632 2023-07-11 18:40:11.000000 bren-0.1.3/bren/autodiff/nodes/Graph.py
+-rw-rw-rw-   0        0        0      343 2023-01-15 20:42:35.000000 bren-0.1.3/bren/autodiff/nodes/Node.py
+-rw-rw-rw-   0        0        0      542 2023-07-10 15:39:02.000000 bren-0.1.3/bren/autodiff/nodes/Operator.py
+-rw-rw-rw-   0        0        0      369 2023-01-03 21:07:13.000000 bren-0.1.3/bren/autodiff/nodes/Var.py
+-rw-rw-rw-   0        0        0      276 2023-01-03 21:39:06.000000 bren-0.1.3/bren/autodiff/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.537597 bren-0.1.3/bren/autodiff/operations/
+-rw-rw-rw-   0        0        0        0 2023-07-21 17:41:51.000000 bren-0.1.3/bren/autodiff/operations/__init__.py
+-rw-rw-rw-   0        0        0     4916 2023-07-11 15:10:50.000000 bren-0.1.3/bren/autodiff/operations/ops.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.553820 bren-0.1.3/bren/core/
+-rw-rw-rw-   0        0        0     4387 2023-07-18 18:33:41.000000 bren-0.1.3/bren/core/Array.py
+-rw-rw-rw-   0        0        0      121 2023-07-21 17:23:23.000000 bren-0.1.3/bren/core/__init__.py
+-rw-rw-rw-   0        0        0     1128 2023-07-21 15:02:52.000000 bren-0.1.3/bren/core/core.py
+-rw-rw-rw-   0        0        0    11560 2023-07-14 18:16:17.000000 bren-0.1.3/bren/keras_LICENCE_copy
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.563565 bren-0.1.3/bren/nn/
+-rw-rw-rw-   0        0        0      458 2023-03-15 22:57:21.000000 bren-0.1.3/bren/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.603545 bren-0.1.3/bren/nn/activations/
+-rw-rw-rw-   0        0        0      578 2023-07-12 20:33:26.000000 bren-0.1.3/bren/nn/activations/Activation.py
+-rw-rw-rw-   0        0        0     1101 2023-07-12 15:17:05.000000 bren-0.1.3/bren/nn/activations/ELU.py
+-rw-rw-rw-   0        0        0      375 2023-07-12 15:18:00.000000 bren-0.1.3/bren/nn/activations/Linear.py
+-rw-rw-rw-   0        0        0     1103 2023-07-12 15:25:53.000000 bren-0.1.3/bren/nn/activations/ReLU.py
+-rw-rw-rw-   0        0        0      405 2023-07-12 15:17:52.000000 bren-0.1.3/bren/nn/activations/Tanh.py
+-rw-rw-rw-   0        0        0      648 2023-07-08 17:47:09.000000 bren-0.1.3/bren/nn/activations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.613803 bren-0.1.3/bren/nn/datasets/
+-rw-rw-rw-   0        0        0       73 2023-03-15 22:57:55.000000 bren-0.1.3/bren/nn/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-07-21 17:56:16.000000 bren-0.1.3/bren/nn/datasets/mnist.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.644616 bren-0.1.3/bren/nn/initialisers/
+-rw-rw-rw-   0        0        0      707 2023-07-13 20:06:12.000000 bren-0.1.3/bren/nn/initialisers/GlorotNormal.py
+-rw-rw-rw-   0        0        0      676 2023-07-14 18:18:10.000000 bren-0.1.3/bren/nn/initialisers/GlorotUniform.py
+-rw-rw-rw-   0        0        0      605 2023-07-14 18:17:50.000000 bren-0.1.3/bren/nn/initialisers/HeNormal.py
+-rw-rw-rw-   0        0        0      576 2023-07-14 18:18:02.000000 bren-0.1.3/bren/nn/initialisers/HeUniform.py
+-rw-rw-rw-   0        0        0      916 2023-07-15 21:06:02.000000 bren-0.1.3/bren/nn/initialisers/Initialiser.py
+-rw-rw-rw-   0        0        0      884 2023-01-22 20:44:45.000000 bren-0.1.3/bren/nn/initialisers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.675637 bren-0.1.3/bren/nn/layers/
+-rw-rw-rw-   0        0        0      460 2023-07-14 18:46:16.000000 bren-0.1.3/bren/nn/layers/Flatten.py
+-rw-rw-rw-   0        0        0     3550 2023-07-14 18:41:54.000000 bren-0.1.3/bren/nn/layers/FullyConnected.py
+-rw-rw-rw-   0        0        0     2115 2023-07-15 16:42:56.000000 bren-0.1.3/bren/nn/layers/Layer.py
+-rw-rw-rw-   0        0        0      537 2023-07-14 18:51:56.000000 bren-0.1.3/bren/nn/layers/Softmax.py
+-rw-rw-rw-   0        0        0      265 2023-07-14 18:26:44.000000 bren-0.1.3/bren/nn/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.702548 bren-0.1.3/bren/nn/losses/
+-rw-rw-rw-   0        0        0      485 2023-07-20 21:16:06.000000 bren-0.1.3/bren/nn/losses/CatrgoricalCrossEntropy.py
+-rw-rw-rw-   0        0        0      460 2023-07-20 16:45:14.000000 bren-0.1.3/bren/nn/losses/Loss.py
+-rw-rw-rw-   0        0        0      406 2023-07-20 16:42:39.000000 bren-0.1.3/bren/nn/losses/MeanSquaredError.py
+-rw-rw-rw-   0        0        0      538 2023-03-11 22:55:20.000000 bren-0.1.3/bren/nn/losses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.739578 bren-0.1.3/bren/nn/metrics/
+-rw-rw-rw-   0        0        0      963 2023-07-14 22:13:36.000000 bren-0.1.3/bren/nn/metrics/Accuracy.py
+-rw-rw-rw-   0        0        0      696 2023-07-14 21:23:20.000000 bren-0.1.3/bren/nn/metrics/CategoricalCrossEntropy.py
+-rw-rw-rw-   0        0        0      580 2023-07-14 21:24:06.000000 bren-0.1.3/bren/nn/metrics/MeanSquaredError.py
+-rw-rw-rw-   0        0        0     1123 2023-07-20 21:08:15.000000 bren-0.1.3/bren/nn/metrics/Metric.py
+-rw-rw-rw-   0        0        0     1179 2023-07-20 21:04:44.000000 bren-0.1.3/bren/nn/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.756383 bren-0.1.3/bren/nn/models/
+-rw-rw-rw-   0        0        0     6944 2023-07-20 21:17:00.000000 bren-0.1.3/bren/nn/models/Model.py
+-rw-rw-rw-   0        0        0      975 2023-07-20 16:02:19.000000 bren-0.1.3/bren/nn/models/Sequential.py
+-rw-rw-rw-   0        0        0     1293 2023-07-21 12:51:34.000000 bren-0.1.3/bren/nn/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.786981 bren-0.1.3/bren/nn/optimisers/
+-rw-rw-rw-   0        0        0      667 2023-07-15 20:30:49.000000 bren-0.1.3/bren/nn/optimisers/AdaGrad.py
+-rw-rw-rw-   0        0        0      999 2023-06-25 20:52:03.000000 bren-0.1.3/bren/nn/optimisers/Adam.py
+-rw-rw-rw-   0        0        0      716 2023-07-15 17:49:17.000000 bren-0.1.3/bren/nn/optimisers/Optimiser.py
+-rw-rw-rw-   0        0        0      748 2023-02-04 22:07:59.000000 bren-0.1.3/bren/nn/optimisers/RMSProp.py
+-rw-rw-rw-   0        0        0      647 2023-07-10 16:19:29.000000 bren-0.1.3/bren/nn/optimisers/SGD.py
+-rw-rw-rw-   0        0        0      730 2023-03-11 23:14:11.000000 bren-0.1.3/bren/nn/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.794128 bren-0.1.3/bren/nn/preprocessing/
+-rw-rw-rw-   0        0        0      138 2023-03-15 21:55:23.000000 bren-0.1.3/bren/nn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-07-15 18:27:34.000000 bren-0.1.3/bren/nn/preprocessing/utils.py
+-rw-rw-rw-   0        0        0     1026 2023-07-15 20:34:41.000000 bren-0.1.3/bren/nn/utils.py
+-rw-rw-rw-   0        0        0    13827 2023-07-14 18:16:17.000000 bren-0.1.3/bren/tensorflow_LICENCE_copy
+drwxrwxrwx   0        0        0        0 2023-07-21 21:29:58.494131 bren-0.1.3/bren.egg-info/
+-rw-rw-rw-   0        0        0     1347 2023-07-21 21:29:58.000000 bren-0.1.3/bren.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1793 2023-07-21 21:29:58.000000 bren-0.1.3/bren.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:29:58.000000 bren-0.1.3/bren.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-21 21:29:58.000000 bren-0.1.3/bren.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-21 21:29:58.000000 bren-0.1.3/bren.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 21:29:58.800434 bren-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-07-21 21:29:31.000000 bren-0.1.3/setup.py
```

### Comparing `bren-0.1.2/LICENSE` & `bren-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/PKG-INFO` & `bren-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bren
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple numpy based neural network library inspired by Tensorflow/Keras.
 Author: Om Panchal
 Author-email: om.panchal2022@gmail.com
 Maintainer: Om Panchal
 Maintainer-email: om.panchal2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `bren-0.1.2/README.md` & `bren-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/__init__.py` & `bren-0.1.3/bren/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/autodiff/nodes/Graph.py` & `bren-0.1.3/bren/autodiff/nodes/Graph.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/autodiff/nodes/Operator.py` & `bren-0.1.3/bren/autodiff/nodes/Operator.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/autodiff/operations/ops.py` & `bren-0.1.3/bren/autodiff/operations/ops.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/core/Array.py` & `bren-0.1.3/bren/core/Array.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/core/core.py` & `bren-0.1.3/bren/core/core.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/activations/Activation.py` & `bren-0.1.3/bren/nn/activations/Activation.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/activations/ELU.py` & `bren-0.1.3/bren/nn/activations/ELU.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/activations/ReLU.py` & `bren-0.1.3/bren/nn/activations/ReLU.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/activations/__init__.py` & `bren-0.1.3/bren/nn/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/datasets/mnist.py` & `bren-0.1.3/bren/nn/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/GlorotNormal.py` & `bren-0.1.3/bren/nn/initialisers/GlorotNormal.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/GlorotUniform.py` & `bren-0.1.3/bren/nn/initialisers/GlorotUniform.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/HeNormal.py` & `bren-0.1.3/bren/nn/initialisers/HeNormal.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/HeUniform.py` & `bren-0.1.3/bren/nn/initialisers/HeUniform.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/Initialiser.py` & `bren-0.1.3/bren/nn/initialisers/Initialiser.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/initialisers/__init__.py` & `bren-0.1.3/bren/nn/initialisers/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/layers/FullyConnected.py` & `bren-0.1.3/bren/nn/layers/FullyConnected.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/layers/Layer.py` & `bren-0.1.3/bren/nn/layers/Layer.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/layers/Softmax.py` & `bren-0.1.3/bren/nn/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/losses/__init__.py` & `bren-0.1.3/bren/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/metrics/Accuracy.py` & `bren-0.1.3/bren/nn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/metrics/CategoricalCrossEntropy.py` & `bren-0.1.3/bren/nn/metrics/CategoricalCrossEntropy.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/metrics/MeanSquaredError.py` & `bren-0.1.3/bren/nn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/metrics/Metric.py` & `bren-0.1.3/bren/nn/metrics/Metric.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/metrics/__init__.py` & `bren-0.1.3/bren/nn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/models/Model.py` & `bren-0.1.3/bren/nn/models/Model.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/models/Sequential.py` & `bren-0.1.3/bren/nn/models/Sequential.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/models/__init__.py` & `bren-0.1.3/bren/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/AdaGrad.py` & `bren-0.1.3/bren/nn/optimisers/AdaGrad.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/Adam.py` & `bren-0.1.3/bren/nn/optimisers/Adam.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/Optimiser.py` & `bren-0.1.3/bren/nn/optimisers/Optimiser.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/RMSProp.py` & `bren-0.1.3/bren/nn/optimisers/RMSProp.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/SGD.py` & `bren-0.1.3/bren/nn/optimisers/SGD.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/optimisers/__init__.py` & `bren-0.1.3/bren/nn/optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/preprocessing/utils.py` & `bren-0.1.3/bren/nn/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren/nn/utils.py` & `bren-0.1.3/bren/nn/utils.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.2/bren.egg-info/PKG-INFO` & `bren-0.1.3/bren.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bren
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple numpy based neural network library inspired by Tensorflow/Keras.
 Author: Om Panchal
 Author-email: om.panchal2022@gmail.com
 Maintainer: Om Panchal
 Maintainer-email: om.panchal2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `bren-0.1.2/bren.egg-info/SOURCES.txt` & `bren-0.1.3/bren.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 README.md
 setup.py
 bren/__init__.py
+bren/keras_LICENCE_copy
+bren/tensorflow_LICENCE_copy
 bren.egg-info/PKG-INFO
 bren.egg-info/SOURCES.txt
 bren.egg-info/dependency_links.txt
 bren.egg-info/requires.txt
 bren.egg-info/top_level.txt
 bren/autodiff/__init__.py
 bren/autodiff/nodes/Const.py
```

### Comparing `bren-0.1.2/setup.py` & `bren-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'PACKAGE.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="bren",
-    version="0.1.2",
+    version="0.1.3",
     description="A simple numpy based neural network library inspired by Tensorflow/Keras.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Om Panchal",
     author_email="om.panchal2022@gmail.com",
     maintainer="Om Panchal",
     maintainer_email="om.panchal2022@gmail.com",
     license="MIT",
     packages=find_packages(),
+    package_data={
+        "bren": [
+            "keras_LICENCE_copy",
+            "tensorflow_LICENCE_copy"
+        ]
+    },
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
 	],
     install_requires=["numpy", "requests"]
 )
```

