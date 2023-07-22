# Comparing `tmp/bren-0.1.4.tar.gz` & `tmp/bren-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bren-0.1.4.tar", last modified: Sat Jul 22 17:04:10 2023, max compression
+gzip compressed data, was "bren-0.1.5.tar", last modified: Sat Jul 22 17:31:33 2023, max compression
```

## Comparing `bren-0.1.4.tar` & `bren-0.1.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.125925 bren-0.1.4/
--rw-rw-rw-   0        0        0     3726 2023-07-14 18:16:17.000000 bren-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1347 2023-07-22 17:04:10.124227 bren-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4895 2023-07-22 17:03:04.000000 bren-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.790101 bren-0.1.4/bren/
--rw-rw-rw-   0        0        0     1923 2023-07-15 20:46:11.000000 bren-0.1.4/bren/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.826124 bren-0.1.4/bren/autodiff/
--rw-rw-rw-   0        0        0        0 2023-01-04 21:18:47.000000 bren-0.1.4/bren/autodiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.855776 bren-0.1.4/bren/autodiff/nodes/
--rw-rw-rw-   0        0        0      442 2023-01-07 21:45:46.000000 bren-0.1.4/bren/autodiff/nodes/Const.py
--rw-rw-rw-   0        0        0     1632 2023-07-11 18:40:11.000000 bren-0.1.4/bren/autodiff/nodes/Graph.py
--rw-rw-rw-   0        0        0      343 2023-01-15 20:42:35.000000 bren-0.1.4/bren/autodiff/nodes/Node.py
--rw-rw-rw-   0        0        0      542 2023-07-10 15:39:02.000000 bren-0.1.4/bren/autodiff/nodes/Operator.py
--rw-rw-rw-   0        0        0      369 2023-01-03 21:07:13.000000 bren-0.1.4/bren/autodiff/nodes/Var.py
--rw-rw-rw-   0        0        0      276 2023-01-03 21:39:06.000000 bren-0.1.4/bren/autodiff/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.868767 bren-0.1.4/bren/autodiff/operations/
--rw-rw-rw-   0        0        0        0 2023-07-21 17:41:51.000000 bren-0.1.4/bren/autodiff/operations/__init__.py
--rw-rw-rw-   0        0        0     4916 2023-07-11 15:10:50.000000 bren-0.1.4/bren/autodiff/operations/ops.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.884136 bren-0.1.4/bren/core/
--rw-rw-rw-   0        0        0     4387 2023-07-18 18:33:41.000000 bren-0.1.4/bren/core/Array.py
--rw-rw-rw-   0        0        0      121 2023-07-21 17:23:23.000000 bren-0.1.4/bren/core/__init__.py
--rw-rw-rw-   0        0        0     1128 2023-07-21 15:02:52.000000 bren-0.1.4/bren/core/core.py
--rw-rw-rw-   0        0        0    11560 2023-07-14 18:16:17.000000 bren-0.1.4/bren/keras_LICENCE_copy
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.895544 bren-0.1.4/bren/nn/
--rw-rw-rw-   0        0        0      458 2023-03-15 22:57:21.000000 bren-0.1.4/bren/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.928143 bren-0.1.4/bren/nn/activations/
--rw-rw-rw-   0        0        0      641 2023-07-22 16:42:43.000000 bren-0.1.4/bren/nn/activations/Activation.py
--rw-rw-rw-   0        0        0     1123 2023-07-22 16:41:58.000000 bren-0.1.4/bren/nn/activations/ELU.py
--rw-rw-rw-   0        0        0      402 2023-07-22 16:40:24.000000 bren-0.1.4/bren/nn/activations/Linear.py
--rw-rw-rw-   0        0        0     1129 2023-07-22 16:44:18.000000 bren-0.1.4/bren/nn/activations/ReLU.py
--rw-rw-rw-   0        0        0      397 2023-07-22 16:02:02.000000 bren-0.1.4/bren/nn/activations/Tanh.py
--rw-rw-rw-   0        0        0      648 2023-07-08 17:47:09.000000 bren-0.1.4/bren/nn/activations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.936253 bren-0.1.4/bren/nn/datasets/
--rw-rw-rw-   0        0        0       73 2023-03-15 22:57:55.000000 bren-0.1.4/bren/nn/datasets/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-07-21 17:56:16.000000 bren-0.1.4/bren/nn/datasets/mnist.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.971896 bren-0.1.4/bren/nn/initialisers/
--rw-rw-rw-   0        0        0      707 2023-07-13 20:06:12.000000 bren-0.1.4/bren/nn/initialisers/GlorotNormal.py
--rw-rw-rw-   0        0        0      676 2023-07-14 18:18:10.000000 bren-0.1.4/bren/nn/initialisers/GlorotUniform.py
--rw-rw-rw-   0        0        0      605 2023-07-14 18:17:50.000000 bren-0.1.4/bren/nn/initialisers/HeNormal.py
--rw-rw-rw-   0        0        0      576 2023-07-14 18:18:02.000000 bren-0.1.4/bren/nn/initialisers/HeUniform.py
--rw-rw-rw-   0        0        0      916 2023-07-15 21:06:02.000000 bren-0.1.4/bren/nn/initialisers/Initialiser.py
--rw-rw-rw-   0        0        0      884 2023-01-22 20:44:45.000000 bren-0.1.4/bren/nn/initialisers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.003380 bren-0.1.4/bren/nn/layers/
--rw-rw-rw-   0        0        0      460 2023-07-14 18:46:16.000000 bren-0.1.4/bren/nn/layers/Flatten.py
--rw-rw-rw-   0        0        0     3621 2023-07-22 16:15:34.000000 bren-0.1.4/bren/nn/layers/FullyConnected.py
--rw-rw-rw-   0        0        0     2115 2023-07-15 16:42:56.000000 bren-0.1.4/bren/nn/layers/Layer.py
--rw-rw-rw-   0        0        0      537 2023-07-14 18:51:56.000000 bren-0.1.4/bren/nn/layers/Softmax.py
--rw-rw-rw-   0        0        0      265 2023-07-14 18:26:44.000000 bren-0.1.4/bren/nn/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.029090 bren-0.1.4/bren/nn/losses/
--rw-rw-rw-   0        0        0      485 2023-07-20 21:16:06.000000 bren-0.1.4/bren/nn/losses/CatrgoricalCrossEntropy.py
--rw-rw-rw-   0        0        0      460 2023-07-20 16:45:14.000000 bren-0.1.4/bren/nn/losses/Loss.py
--rw-rw-rw-   0        0        0      406 2023-07-20 16:42:39.000000 bren-0.1.4/bren/nn/losses/MeanSquaredError.py
--rw-rw-rw-   0        0        0      538 2023-03-11 22:55:20.000000 bren-0.1.4/bren/nn/losses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.058405 bren-0.1.4/bren/nn/metrics/
--rw-rw-rw-   0        0        0      963 2023-07-14 22:13:36.000000 bren-0.1.4/bren/nn/metrics/Accuracy.py
--rw-rw-rw-   0        0        0      696 2023-07-14 21:23:20.000000 bren-0.1.4/bren/nn/metrics/CategoricalCrossEntropy.py
--rw-rw-rw-   0        0        0      580 2023-07-14 21:24:06.000000 bren-0.1.4/bren/nn/metrics/MeanSquaredError.py
--rw-rw-rw-   0        0        0     1123 2023-07-20 21:08:15.000000 bren-0.1.4/bren/nn/metrics/Metric.py
--rw-rw-rw-   0        0        0     1179 2023-07-20 21:04:44.000000 bren-0.1.4/bren/nn/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.077199 bren-0.1.4/bren/nn/models/
--rw-rw-rw-   0        0        0     6944 2023-07-22 15:42:20.000000 bren-0.1.4/bren/nn/models/Model.py
--rw-rw-rw-   0        0        0      975 2023-07-20 16:02:19.000000 bren-0.1.4/bren/nn/models/Sequential.py
--rw-rw-rw-   0        0        0     1293 2023-07-22 16:12:15.000000 bren-0.1.4/bren/nn/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.110717 bren-0.1.4/bren/nn/optimisers/
--rw-rw-rw-   0        0        0      667 2023-07-15 20:30:49.000000 bren-0.1.4/bren/nn/optimisers/AdaGrad.py
--rw-rw-rw-   0        0        0      999 2023-06-25 20:52:03.000000 bren-0.1.4/bren/nn/optimisers/Adam.py
--rw-rw-rw-   0        0        0      716 2023-07-15 17:49:17.000000 bren-0.1.4/bren/nn/optimisers/Optimiser.py
--rw-rw-rw-   0        0        0      748 2023-02-04 22:07:59.000000 bren-0.1.4/bren/nn/optimisers/RMSProp.py
--rw-rw-rw-   0        0        0      647 2023-07-10 16:19:29.000000 bren-0.1.4/bren/nn/optimisers/SGD.py
--rw-rw-rw-   0        0        0      730 2023-03-11 23:14:11.000000 bren-0.1.4/bren/nn/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:10.119215 bren-0.1.4/bren/nn/preprocessing/
--rw-rw-rw-   0        0        0      138 2023-03-15 21:55:23.000000 bren-0.1.4/bren/nn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-07-15 18:27:34.000000 bren-0.1.4/bren/nn/preprocessing/utils.py
--rw-rw-rw-   0        0        0     1026 2023-07-15 20:34:41.000000 bren-0.1.4/bren/nn/utils.py
--rw-rw-rw-   0        0        0    13827 2023-07-14 18:16:17.000000 bren-0.1.4/bren/tensorflow_LICENCE_copy
-drwxrwxrwx   0        0        0        0 2023-07-22 17:04:09.820011 bren-0.1.4/bren.egg-info/
--rw-rw-rw-   0        0        0     1347 2023-07-22 17:04:09.000000 bren-0.1.4/bren.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1793 2023-07-22 17:04:09.000000 bren-0.1.4/bren.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 17:04:09.000000 bren-0.1.4/bren.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-22 17:04:09.000000 bren-0.1.4/bren.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 17:04:09.000000 bren-0.1.4/bren.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 17:04:10.126924 bren-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-07-22 17:03:49.000000 bren-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.867618 bren-0.1.5/
+-rw-rw-rw-   0        0        0     3726 2023-07-14 18:16:17.000000 bren-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5465 2023-07-22 17:31:33.865385 bren-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4926 2023-07-22 17:20:04.000000 bren-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.582511 bren-0.1.5/bren/
+-rw-rw-rw-   0        0        0     1923 2023-07-15 20:46:11.000000 bren-0.1.5/bren/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.608914 bren-0.1.5/bren/autodiff/
+-rw-rw-rw-   0        0        0        0 2023-01-04 21:18:47.000000 bren-0.1.5/bren/autodiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.637974 bren-0.1.5/bren/autodiff/nodes/
+-rw-rw-rw-   0        0        0      442 2023-01-07 21:45:46.000000 bren-0.1.5/bren/autodiff/nodes/Const.py
+-rw-rw-rw-   0        0        0     1632 2023-07-11 18:40:11.000000 bren-0.1.5/bren/autodiff/nodes/Graph.py
+-rw-rw-rw-   0        0        0      343 2023-01-15 20:42:35.000000 bren-0.1.5/bren/autodiff/nodes/Node.py
+-rw-rw-rw-   0        0        0      542 2023-07-10 15:39:02.000000 bren-0.1.5/bren/autodiff/nodes/Operator.py
+-rw-rw-rw-   0        0        0      369 2023-01-03 21:07:13.000000 bren-0.1.5/bren/autodiff/nodes/Var.py
+-rw-rw-rw-   0        0        0      276 2023-01-03 21:39:06.000000 bren-0.1.5/bren/autodiff/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.646506 bren-0.1.5/bren/autodiff/operations/
+-rw-rw-rw-   0        0        0        0 2023-07-21 17:41:51.000000 bren-0.1.5/bren/autodiff/operations/__init__.py
+-rw-rw-rw-   0        0        0     4916 2023-07-11 15:10:50.000000 bren-0.1.5/bren/autodiff/operations/ops.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.662838 bren-0.1.5/bren/core/
+-rw-rw-rw-   0        0        0     4387 2023-07-18 18:33:41.000000 bren-0.1.5/bren/core/Array.py
+-rw-rw-rw-   0        0        0      121 2023-07-21 17:23:23.000000 bren-0.1.5/bren/core/__init__.py
+-rw-rw-rw-   0        0        0     1128 2023-07-21 15:02:52.000000 bren-0.1.5/bren/core/core.py
+-rw-rw-rw-   0        0        0    11560 2023-07-14 18:16:17.000000 bren-0.1.5/bren/keras_LICENCE_copy
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.671651 bren-0.1.5/bren/nn/
+-rw-rw-rw-   0        0        0      458 2023-03-15 22:57:21.000000 bren-0.1.5/bren/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.703443 bren-0.1.5/bren/nn/activations/
+-rw-rw-rw-   0        0        0      641 2023-07-22 16:42:43.000000 bren-0.1.5/bren/nn/activations/Activation.py
+-rw-rw-rw-   0        0        0     1123 2023-07-22 16:41:58.000000 bren-0.1.5/bren/nn/activations/ELU.py
+-rw-rw-rw-   0        0        0      402 2023-07-22 16:40:24.000000 bren-0.1.5/bren/nn/activations/Linear.py
+-rw-rw-rw-   0        0        0     1129 2023-07-22 16:44:18.000000 bren-0.1.5/bren/nn/activations/ReLU.py
+-rw-rw-rw-   0        0        0      397 2023-07-22 16:02:02.000000 bren-0.1.5/bren/nn/activations/Tanh.py
+-rw-rw-rw-   0        0        0      648 2023-07-08 17:47:09.000000 bren-0.1.5/bren/nn/activations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.711190 bren-0.1.5/bren/nn/datasets/
+-rw-rw-rw-   0        0        0       73 2023-03-15 22:57:55.000000 bren-0.1.5/bren/nn/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-07-21 17:56:16.000000 bren-0.1.5/bren/nn/datasets/mnist.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.743152 bren-0.1.5/bren/nn/initialisers/
+-rw-rw-rw-   0        0        0      707 2023-07-13 20:06:12.000000 bren-0.1.5/bren/nn/initialisers/GlorotNormal.py
+-rw-rw-rw-   0        0        0      676 2023-07-14 18:18:10.000000 bren-0.1.5/bren/nn/initialisers/GlorotUniform.py
+-rw-rw-rw-   0        0        0      605 2023-07-14 18:17:50.000000 bren-0.1.5/bren/nn/initialisers/HeNormal.py
+-rw-rw-rw-   0        0        0      576 2023-07-14 18:18:02.000000 bren-0.1.5/bren/nn/initialisers/HeUniform.py
+-rw-rw-rw-   0        0        0      916 2023-07-15 21:06:02.000000 bren-0.1.5/bren/nn/initialisers/Initialiser.py
+-rw-rw-rw-   0        0        0      884 2023-01-22 20:44:45.000000 bren-0.1.5/bren/nn/initialisers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.767129 bren-0.1.5/bren/nn/layers/
+-rw-rw-rw-   0        0        0      460 2023-07-14 18:46:16.000000 bren-0.1.5/bren/nn/layers/Flatten.py
+-rw-rw-rw-   0        0        0     3576 2023-07-22 17:28:27.000000 bren-0.1.5/bren/nn/layers/FullyConnected.py
+-rw-rw-rw-   0        0        0     2115 2023-07-15 16:42:56.000000 bren-0.1.5/bren/nn/layers/Layer.py
+-rw-rw-rw-   0        0        0      537 2023-07-14 18:51:56.000000 bren-0.1.5/bren/nn/layers/Softmax.py
+-rw-rw-rw-   0        0        0      265 2023-07-14 18:26:44.000000 bren-0.1.5/bren/nn/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.782113 bren-0.1.5/bren/nn/losses/
+-rw-rw-rw-   0        0        0      485 2023-07-20 21:16:06.000000 bren-0.1.5/bren/nn/losses/CatrgoricalCrossEntropy.py
+-rw-rw-rw-   0        0        0      460 2023-07-20 16:45:14.000000 bren-0.1.5/bren/nn/losses/Loss.py
+-rw-rw-rw-   0        0        0      406 2023-07-20 16:42:39.000000 bren-0.1.5/bren/nn/losses/MeanSquaredError.py
+-rw-rw-rw-   0        0        0      538 2023-03-11 22:55:20.000000 bren-0.1.5/bren/nn/losses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.808758 bren-0.1.5/bren/nn/metrics/
+-rw-rw-rw-   0        0        0      963 2023-07-14 22:13:36.000000 bren-0.1.5/bren/nn/metrics/Accuracy.py
+-rw-rw-rw-   0        0        0      696 2023-07-14 21:23:20.000000 bren-0.1.5/bren/nn/metrics/CategoricalCrossEntropy.py
+-rw-rw-rw-   0        0        0      580 2023-07-14 21:24:06.000000 bren-0.1.5/bren/nn/metrics/MeanSquaredError.py
+-rw-rw-rw-   0        0        0     1123 2023-07-20 21:08:15.000000 bren-0.1.5/bren/nn/metrics/Metric.py
+-rw-rw-rw-   0        0        0     1179 2023-07-20 21:04:44.000000 bren-0.1.5/bren/nn/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.825071 bren-0.1.5/bren/nn/models/
+-rw-rw-rw-   0        0        0     6944 2023-07-22 15:42:20.000000 bren-0.1.5/bren/nn/models/Model.py
+-rw-rw-rw-   0        0        0      975 2023-07-20 16:02:19.000000 bren-0.1.5/bren/nn/models/Sequential.py
+-rw-rw-rw-   0        0        0     1293 2023-07-22 16:12:15.000000 bren-0.1.5/bren/nn/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.852168 bren-0.1.5/bren/nn/optimisers/
+-rw-rw-rw-   0        0        0      667 2023-07-15 20:30:49.000000 bren-0.1.5/bren/nn/optimisers/AdaGrad.py
+-rw-rw-rw-   0        0        0      999 2023-06-25 20:52:03.000000 bren-0.1.5/bren/nn/optimisers/Adam.py
+-rw-rw-rw-   0        0        0      716 2023-07-15 17:49:17.000000 bren-0.1.5/bren/nn/optimisers/Optimiser.py
+-rw-rw-rw-   0        0        0      748 2023-02-04 22:07:59.000000 bren-0.1.5/bren/nn/optimisers/RMSProp.py
+-rw-rw-rw-   0        0        0      647 2023-07-10 16:19:29.000000 bren-0.1.5/bren/nn/optimisers/SGD.py
+-rw-rw-rw-   0        0        0      730 2023-03-11 23:14:11.000000 bren-0.1.5/bren/nn/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.859788 bren-0.1.5/bren/nn/preprocessing/
+-rw-rw-rw-   0        0        0      138 2023-03-15 21:55:23.000000 bren-0.1.5/bren/nn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-07-15 18:27:34.000000 bren-0.1.5/bren/nn/preprocessing/utils.py
+-rw-rw-rw-   0        0        0     1026 2023-07-15 20:34:41.000000 bren-0.1.5/bren/nn/utils.py
+-rw-rw-rw-   0        0        0    13827 2023-07-14 18:16:17.000000 bren-0.1.5/bren/tensorflow_LICENCE_copy
+drwxrwxrwx   0        0        0        0 2023-07-22 17:31:33.605129 bren-0.1.5/bren.egg-info/
+-rw-rw-rw-   0        0        0     5465 2023-07-22 17:31:33.000000 bren-0.1.5/bren.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1793 2023-07-22 17:31:33.000000 bren-0.1.5/bren.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 17:31:33.000000 bren-0.1.5/bren.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-22 17:31:33.000000 bren-0.1.5/bren.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-22 17:31:33.000000 bren-0.1.5/bren.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 17:31:33.869017 bren-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-07-22 17:31:18.000000 bren-0.1.5/setup.py
```

### Comparing `bren-0.1.4/LICENSE` & `bren-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/README.md` & `bren-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,98 @@
   <div id="header" align="center">
     <img id="logo" src="https://github.com/OmPanchal/Bren/blob/main/bren/B.png" ></img>   
   </div>
 
-[bren](https://pypi.org/project/bren/) is a custom [numpy](https://numpy.org) based library, powered by automatic differentiation, inspired by [Tensorflow](https://www.tensorflow.org)/[Keras](https://keras.io), which allows users to build small scale simple neural networks. It's analogous yet simpler design to the Keras API allows users to produce, train and save their own models, with custom components, without having to learn an entirely new structure. 
+[bren](https://pypi.org/project/bren/) is a custom [numpy](https://numpy.org) based library, powered by automatic differentiation, inspired by [Tensorflow](https://www.tensorflow.org)/[Keras](https://keras.io), which allows users to build small scale simple neural networks. It's analogous yet simpler design to the Keras API allows users to produce, train and save their own models, with custom components, without having to learn an entirely new structure.
 
 bren is part of a sequence of neural network from scratch projects and a successor to the [neural-network-from-scratch-v2](https://github.com/OmPanchal/nn-from-scratch-2), with one major update being the integration of automatic differentitation. Automatic differentiation allows for the real-time determination of derivatives during backpropagation (through the use of computation graphs produced by `br.autodiff` and `br.Variable`) and reduces the need for users to couple mathematical computation with pre-written derivatives as was required in the previous projects.
 
 ## Install
-To install the latest version of bren, run: 
+
+To install the latest version of bren, run:
+
 ```
 pip install bren
 ```
 
 **Your first bren program**. (Examples tend to import `bren` as `br`)
+
 ```python
 import bren as br
 
 A = br.Variable([1, 2, 3])
 print(A + 2) # <Variable value=[3. 4. 5.] dtype=float64>
 ```
 
 ## `br.autodiff` (Automatic Differentiation)
-bren is an automatic differentiation driven neural network library, with backpropagation making use of `br.Graph` to find the derivatives of the trainable parameters with respect to the loss. This is governed by `br.Variable` which keeps track of any operation which have been performed on the `Variable` object. `br.autodiff` is used to produce a computation graph of these recorded operations, this graph can be back tracked to determine the derivatives of a given *dy* value with respect to a given *dx* value. As a gradient, a `br.Constant` is returned (the derivative of a `br.Constant` is always 0). The functionings of `br.Variable` and `br.Constant` are a result of the swift array computation of [numpy](https://numpy.org).
+
+bren is an automatic differentiation driven neural network library, with backpropagation making use of `br.Graph` to find the derivatives of the trainable parameters with respect to the loss. This is governed by `br.Variable` which keeps track of any operation which have been performed on the `Variable` object. `br.autodiff` is used to produce a computation graph of these recorded operations, this graph can be back tracked to determine the derivatives of a given _dy_ value with respect to a given _dx_ value. As a gradient, a `br.Constant` is returned (the derivative of a `br.Constant` is always 0). The functionings of `br.Variable` and `br.Constant` are a result of the swift array computation of [numpy](https://numpy.org).
 
 ```python
 import bren as br
 
 A = br.Variable([1, 2, 3], dtype="float64")
 
 with br.Graph() as g:
-	B = A ** 2 # any computation performed on a Variable will be tracked 
+	B = A ** 2 # any computation performed on a Variable will be tracked
 	print(g.grad(B, [A])) # [<Constant value=[2. 4. 6.] dtype=float64>]
 ```
 
 ## `br.nn` (Neural Networks)
+
 bren's modular design is heavily inspired by the [Keras](https://keras.io) API, allowing users to produce networks comprised of a variety of customisable components. Users are also capable of producing their own custom components such as (layers, activations, initialisers, losses, metrics) through the use of the respective base classes. `br.nn` allows ready made components to be imported and custom components to be produced.
 
 **Your first neural network with bren**: First prepare the dataset
+
 ```python
 import bren as br
 
 # Test data - The XOR dataset
 X = br.Variable([[0, 0], [0, 1], [1, 0], [1, 1]])
 Y = br.Variable([0, 1, 1, 0])
 ```
+
 Next initialise the `Sequential` model which will be trained to fit the data. It will take in a list of layers through which the data will be passed through consecutively. In the example below, a three fully connected (`FC`) layer neural network is initialised, with activation "tanh".
+
 ```python
 # Initialise the model
 model = br.nn.models.Sequential(layers=[
 	br.nn.layers.FC(2, activation="tanh"),
 	br.nn.layers.FC(32, activation="tanh"),
 	br.nn.layers.FC(1, activation="tanh"),
 ])
 ```
+
 `model.assemble` will then be called to establish the optimiser used during gradient descent, the loss function, and metrics to be displayed during training.
+
 ```python
 model.assemble(
 	optimiser="Adam",
  	loss=br.nn.losses.MeanSquaredError(),
 	metrics=["accuracy"]
 )
 ```
+
 To train the model, `model.fit` will be called. Here the training features and lables will be specified, as well other arguments such as epochs (the number of iterations of the data while training the metwork).
+
 ```python
 model.fit(X, Y, epochs=100)
 ```
+
 Now that the model is trained, you can test it on test data to evaluate its performance, and also save it to a file for future use.
+
 ```python
 pred = model.predict(X) # Test data would be inputted
 model.save("model")
 ```
+
 ### Custom Components
+
 Custom components can be produced by using the base class of the component or can be in the form of a function, both methods are compatible with the existing components which `br.nn` provides.
+
 ```python
 # Custom activation as a function
 def linear(x): return x
 
 # Custom activation as a class
 class Linear(br.nn.activations.Activation):
 	def __init__(self, name="linear", **kwargs):
```

### Comparing `bren-0.1.4/bren/__init__.py` & `bren-0.1.5/bren/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/autodiff/nodes/Graph.py` & `bren-0.1.5/bren/autodiff/nodes/Graph.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/autodiff/nodes/Operator.py` & `bren-0.1.5/bren/autodiff/nodes/Operator.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/autodiff/operations/ops.py` & `bren-0.1.5/bren/autodiff/operations/ops.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/core/Array.py` & `bren-0.1.5/bren/core/Array.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/core/core.py` & `bren-0.1.5/bren/core/core.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/keras_LICENCE_copy` & `bren-0.1.5/bren/keras_LICENCE_copy`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/activations/Activation.py` & `bren-0.1.5/bren/nn/activations/Activation.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/activations/ELU.py` & `bren-0.1.5/bren/nn/activations/ELU.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/activations/ReLU.py` & `bren-0.1.5/bren/nn/activations/ReLU.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/activations/__init__.py` & `bren-0.1.5/bren/nn/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/datasets/mnist.py` & `bren-0.1.5/bren/nn/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/GlorotNormal.py` & `bren-0.1.5/bren/nn/initialisers/GlorotNormal.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/GlorotUniform.py` & `bren-0.1.5/bren/nn/initialisers/GlorotUniform.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/HeNormal.py` & `bren-0.1.5/bren/nn/initialisers/HeNormal.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/HeUniform.py` & `bren-0.1.5/bren/nn/initialisers/HeUniform.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/Initialiser.py` & `bren-0.1.5/bren/nn/initialisers/Initialiser.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/initialisers/__init__.py` & `bren-0.1.5/bren/nn/initialisers/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/layers/FullyConnected.py` & `bren-0.1.5/bren/nn/layers/FullyConnected.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
 	def call(self, x):
 		output = (self.weights @ x) + self.bias
 		
 		return self.activation(output)
 	
 	def config(self):
-		print(self.activation.__class__.__name__)
 		self.set_config(rename_key(super().config(), "_units", "units"))
 		self.__dict__["bias_initialiser"] = self.bias_initialiser.__name__
 		self.__dict__["weights_initialiser"] = self.weights_initialiser.__name__
 		self.__dict__["activation"] = self.activation.__class__.__name__
 		return self.__dict__
 
 # aliases
```

### Comparing `bren-0.1.4/bren/nn/layers/Layer.py` & `bren-0.1.5/bren/nn/layers/Layer.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/layers/Softmax.py` & `bren-0.1.5/bren/nn/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/losses/__init__.py` & `bren-0.1.5/bren/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/metrics/Accuracy.py` & `bren-0.1.5/bren/nn/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/metrics/CategoricalCrossEntropy.py` & `bren-0.1.5/bren/nn/metrics/CategoricalCrossEntropy.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/metrics/MeanSquaredError.py` & `bren-0.1.5/bren/nn/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/metrics/Metric.py` & `bren-0.1.5/bren/nn/metrics/Metric.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/metrics/__init__.py` & `bren-0.1.5/bren/nn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/models/Model.py` & `bren-0.1.5/bren/nn/models/Model.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/models/Sequential.py` & `bren-0.1.5/bren/nn/models/Sequential.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/models/__init__.py` & `bren-0.1.5/bren/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/AdaGrad.py` & `bren-0.1.5/bren/nn/optimisers/AdaGrad.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/Adam.py` & `bren-0.1.5/bren/nn/optimisers/Adam.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/Optimiser.py` & `bren-0.1.5/bren/nn/optimisers/Optimiser.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/RMSProp.py` & `bren-0.1.5/bren/nn/optimisers/RMSProp.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/SGD.py` & `bren-0.1.5/bren/nn/optimisers/SGD.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/optimisers/__init__.py` & `bren-0.1.5/bren/nn/optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/preprocessing/utils.py` & `bren-0.1.5/bren/nn/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/nn/utils.py` & `bren-0.1.5/bren/nn/utils.py`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren/tensorflow_LICENCE_copy` & `bren-0.1.5/bren/tensorflow_LICENCE_copy`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/bren.egg-info/SOURCES.txt` & `bren-0.1.5/bren.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bren-0.1.4/setup.py` & `bren-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 from codecs import open
 from os import path
 
 HERE = path.abspath(path.dirname(__file__))
 
-with open(path.join(HERE, 'PACKAGE.md'), encoding='utf-8') as f:
+with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="bren",
-    version="0.1.4",
+    version="0.1.5",
     description="A simple numpy based neural network library inspired by Tensorflow/Keras.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Om Panchal",
     author_email="om.panchal2022@gmail.com",
     maintainer="Om Panchal",
     maintainer_email="om.panchal2022@gmail.com",
```

