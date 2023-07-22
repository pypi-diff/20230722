# Comparing `tmp/score_models-0.4.5.tar.gz` & `tmp/score_models-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.4.5.tar", last modified: Mon Jul 17 22:55:06 2023, max compression
+gzip compressed data, was "dist/score_models-0.4.6.tar", last modified: Sat Jul 22 03:22:26 2023, max compression
```

## Comparing `score_models-0.4.5.tar` & `score_models-0.4.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.790813 score_models-0.4.5/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.5/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 22:55:06.790813 score_models-0.4.5/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.5/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.5/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20765 2023-07-17 22:53:49.000000 score_models-0.4.5/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1647 2023-07-17 04:57:57.000000 score_models-0.4.5/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-17 18:30:38.000000 score_models-0.4.5/score_models/sliced_score_matching.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-17 22:55:06.790813 score_models-0.4.5/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-17 22:54:35.000000 score_models-0.4.5/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.4.5/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.5/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.5/tests/test_score_models.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.5/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.6/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7415 2023-07-22 03:22:26.000000 score_models-0.4.6/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.6/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.6/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20765 2023-07-22 03:21:43.000000 score_models-0.4.6/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1647 2023-07-17 04:57:57.000000 score_models-0.4.6/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-18 01:20:38.000000 score_models-0.4.6/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-07-22 03:19:51.000000 score_models-0.4.6/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7415 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-22 03:22:26.000000 score_models-0.4.6/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-22 03:22:04.000000 score_models-0.4.6/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.6/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.6/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.6/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.6/tests/test_training.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `score_models-0.4.5/LICENSE.txt` & `score_models-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/PKG-INFO` & `score_models-0.4.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,159 +1,160 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: score_models
-Version: 0.4.5
+Version: 0.4.6
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
+License: UNKNOWN
+Description: =========================
+        Score Models for Pytorch
+        =========================
+        
+        .. image:: https://badge.fury.io/py/score_models.svg
+           :target: https://badge.fury.io/py/score_models
+        .. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
+           :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
+        
+        A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
+        
+        - Simple initialization of MLP, NCSN++ and DDPM neural network architectures
+        - A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
+        - A sampling method based on an Euler-Maruyama discretization of an SDE.
+        - A simple interface to train an energy model using DSM
+        
+        This repository is mainly intended for personal use.
+        You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
+        
+        Installation
+        ------------
+        
+        To install the package, you can use pip:
+        
+        .. code-block:: bash
+        
+           pip install torch-score-models
+        
+        Usage
+        -----
+        
+        ScoreModel
+        ~~~~~~~~~~
+        
+        The `ScoreModel` class is the main interface for training and using score models, defined as
+        
+        .. math::
+        
+           \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
+        
+        where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
+        of an SDE.
+        
+        The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
+        
+        .. code-block:: python
+        
+           from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
+        
+           # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
+           model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
+           # ... or the VPSDE
+           model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
+        
+           # NN Architectures support a Unet with 1D convolutions for time series input data
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
+           # ... or 3D convolutions for videos/voxels
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
+           # You can also use a simpler MLP architecture
+           net = MLP(dimensions=dim, layers=4, units=100)
+           # ... or Jonathan Ho's DDPM architecture
+           net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
+        
+           # Train the model
+           model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
+        
+           # Generate samples from the trained model
+           samples = model.sample(size=[batch_size, *dimensions], N=1000)
+        
+           # Compute the score for a given input
+           score = model.score(t, x)
+        
+           # Initialize the score model and its neural network from a path to a checkpoint directory
+           score = ScoreModel(checkpoint_directory)
+        
+        EnergyModel
+        ~~~~~~~~~~~
+        
+        The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
+        automatic differentiation of an energy model
+        
+        .. math::
+        
+           E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
+        
+        This is to say that the score is defined as
+        
+        .. math::
+        
+           \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
+        
+        **Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
+        neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
+        architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
+        can also be specified to make the energy positive or bounded from below.
+        
+        Training Parameters
+        ~~~~~~~~~~~~~~~~~~~
+        
+        When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
+        
+        - `dataset`: The training dataset (`torch.utils.data.Dataset`).
+        - `epochs`: The number of training epochs.
+        - `learning_rate`: The learning rate for the ADAM optimizer.
+        - `batch_size`: The batch size for training.
+        - `checkpoints_directory`: The directory to save model checkpoints (default: None).
+        - `seed`: The random seed for numpy and torch.
+        
+        Refer to the method's docstring or the class definition for more details on available parameters.
+        
+        Citations
+        ---------
+        
+        If you use this package in your research, please consider citing the following papers:
+        
+        .. code-block:: bibtex
+        
+           @inproceedings{NEURIPS2020_4c5bcfec,
+               author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
+               booktitle   = {Advances in Neural Information Processing Systems},
+               editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
+               pages       = {6840--6851},
+               publisher   = {Curran Associates, Inc.},
+               title       = {Denoising Diffusion Probabilistic Models},
+               url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
+               volume      = {33},
+               year        = {2020}
+           }
+        
+           @inproceedings{song2021scorebased,
+             title={Score-Based Generative Modeling through Stochastic Differential Equations},
+             author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
+             booktitle={International Conference on Learning Representations},
+             year={2021},
+             url={https://openreview.net/forum?id=PxTIG12RRHS}
+           }
+        
+        License
+        -------
+        
+        This package is licensed under the MIT License.
+        
+        You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
-License-File: LICENSE.txt
-
-=========================
-Score Models for Pytorch
-=========================
-
-.. image:: https://badge.fury.io/py/score_models.svg
-   :target: https://badge.fury.io/py/score_models
-.. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
-   :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
-
-A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
-
-- Simple initialization of MLP, NCSN++ and DDPM neural network architectures
-- A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
-- A sampling method based on an Euler-Maruyama discretization of an SDE.
-- A simple interface to train an energy model using DSM
-
-This repository is mainly intended for personal use.
-You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
-
-Installation
-------------
-
-To install the package, you can use pip:
-
-.. code-block:: bash
-
-   pip install torch-score-models
-
-Usage
------
-
-ScoreModel
-~~~~~~~~~~
-
-The `ScoreModel` class is the main interface for training and using score models, defined as
-
-.. math::
-
-   \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
-
-where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
-of an SDE.
-
-The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
-
-.. code-block:: python
-
-   from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
-
-   # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
-   model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
-   # ... or the VPSDE
-   model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
-
-   # NN Architectures support a Unet with 1D convolutions for time series input data
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
-   # ... or 3D convolutions for videos/voxels
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
-   # You can also use a simpler MLP architecture
-   net = MLP(dimensions=dim, layers=4, units=100)
-   # ... or Jonathan Ho's DDPM architecture
-   net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
-
-   # Train the model
-   model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
-
-   # Generate samples from the trained model
-   samples = model.sample(size=[batch_size, *dimensions], N=1000)
-
-   # Compute the score for a given input
-   score = model.score(t, x)
-
-   # Initialize the score model and its neural network from a path to a checkpoint directory
-   score = ScoreModel(checkpoint_directory)
-
-EnergyModel
-~~~~~~~~~~~
-
-The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
-automatic differentiation of an energy model
-
-.. math::
-
-   E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
-
-This is to say that the score is defined as
-
-.. math::
-
-   \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
-
-**Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
-neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
-architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
-can also be specified to make the energy positive or bounded from below.
-
-Training Parameters
-~~~~~~~~~~~~~~~~~~~
-
-When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
-
-- `dataset`: The training dataset (`torch.utils.data.Dataset`).
-- `epochs`: The number of training epochs.
-- `learning_rate`: The learning rate for the ADAM optimizer.
-- `batch_size`: The batch size for training.
-- `checkpoints_directory`: The directory to save model checkpoints (default: None).
-- `seed`: The random seed for numpy and torch.
-
-Refer to the method's docstring or the class definition for more details on available parameters.
-
-Citations
----------
-
-If you use this package in your research, please consider citing the following papers:
-
-.. code-block:: bibtex
-
-   @inproceedings{NEURIPS2020_4c5bcfec,
-       author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
-       booktitle   = {Advances in Neural Information Processing Systems},
-       editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
-       pages       = {6840--6851},
-       publisher   = {Curran Associates, Inc.},
-       title       = {Denoising Diffusion Probabilistic Models},
-       url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
-       volume      = {33},
-       year        = {2020}
-   }
-
-   @inproceedings{song2021scorebased,
-     title={Score-Based Generative Modeling through Stochastic Differential Equations},
-     author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
-     booktitle={International Conference on Learning Representations},
-     year={2021},
-     url={https://openreview.net/forum?id=PxTIG12RRHS}
-   }
-
-License
--------
-
-This package is licensed under the MIT License.
-
-You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
-
```

### Comparing `score_models-0.4.5/README.md` & `score_models-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/architectures/ddpm.py` & `score_models-0.4.6/score_models/architectures/ddpm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/architectures/mlp.py` & `score_models-0.4.6/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/architectures/ncsnpp.py` & `score_models-0.4.6/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/base.py` & `score_models-0.4.6/score_models/base.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/definitions.py` & `score_models-0.4.6/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/__init__.py` & `score_models-0.4.6/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/attention_block.py` & `score_models-0.4.6/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/combine.py` & `score_models-0.4.6/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.6/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.6/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.6/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conv1dsame.py` & `score_models-0.4.6/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conv2dsame.py` & `score_models-0.4.6/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conv3dsame.py` & `score_models-0.4.6/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/conv_layers.py` & `score_models-0.4.6/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.6/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/downsample.py` & `score_models-0.4.6/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.6/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/projection_embedding.py` & `score_models-0.4.6/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.6/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/spectral_normalization.py` & `score_models-0.4.6/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.6/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/style_gan_conv.py` & `score_models-0.4.6/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/up_or_downsampling.py` & `score_models-0.4.6/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.6/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.6/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.6/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/upfirdn1d.py` & `score_models-0.4.6/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/upfirdn2d.py` & `score_models-0.4.6/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/upfirdn3d.py` & `score_models-0.4.6/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/layers/upsample.py` & `score_models-0.4.6/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/score_model.py` & `score_models-0.4.6/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/sde/sde.py` & `score_models-0.4.6/score_models/sde/sde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/sde/vesde.py` & `score_models-0.4.6/score_models/sde/vesde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/sde/vpsde.py` & `score_models-0.4.6/score_models/sde/vpsde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/sliced_score_matching.py` & `score_models-0.4.6/score_models/sliced_score_matching.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/score_models/utils.py` & `score_models-0.4.6/score_models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,9 +84,16 @@
         else:
             raise ValueError(f"{model} not supported")
     else:
         hparams = model.hyperparameters
     paths = glob(os.path.join(checkpoints_directory, "checkpoint*.pt"))
     checkpoints = [int(re.findall('[0-9]+', os.path.split(path)[-1])[-1]) for path in paths]
     if paths:
-        model.load_state_dict(torch.load(paths[np.argmax(checkpoints)], map_location=device))
+        try:
+            model.load_state_dict(torch.load(paths[np.argmax(checkpoints)], map_location=device))
+        except (KeyError, RuntimeError):
+            # Maybe the ScoreModel instance was used when saving the weights, in which case we hack the loading process
+            from score_models import ScoreModel
+            model = ScoreModel(model, **hparams)
+            model.load_state_dict(torch.load(paths[np.argmax(checkpoints)], map_location=device))
+            model = model.model # Remove the ScoreModel wrapping to extract the nn
     return model, hparams
```

### Comparing `score_models-0.4.5/score_models.egg-info/PKG-INFO` & `score_models-0.4.6/score_models.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,159 +1,160 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: score-models
-Version: 0.4.5
+Version: 0.4.6
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
+License: UNKNOWN
+Description: =========================
+        Score Models for Pytorch
+        =========================
+        
+        .. image:: https://badge.fury.io/py/score_models.svg
+           :target: https://badge.fury.io/py/score_models
+        .. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
+           :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
+        
+        A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
+        
+        - Simple initialization of MLP, NCSN++ and DDPM neural network architectures
+        - A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
+        - A sampling method based on an Euler-Maruyama discretization of an SDE.
+        - A simple interface to train an energy model using DSM
+        
+        This repository is mainly intended for personal use.
+        You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
+        
+        Installation
+        ------------
+        
+        To install the package, you can use pip:
+        
+        .. code-block:: bash
+        
+           pip install torch-score-models
+        
+        Usage
+        -----
+        
+        ScoreModel
+        ~~~~~~~~~~
+        
+        The `ScoreModel` class is the main interface for training and using score models, defined as
+        
+        .. math::
+        
+           \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
+        
+        where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
+        of an SDE.
+        
+        The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
+        
+        .. code-block:: python
+        
+           from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
+        
+           # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
+           model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
+           # ... or the VPSDE
+           model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
+        
+           # NN Architectures support a Unet with 1D convolutions for time series input data
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
+           # ... or 3D convolutions for videos/voxels
+           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
+           # You can also use a simpler MLP architecture
+           net = MLP(dimensions=dim, layers=4, units=100)
+           # ... or Jonathan Ho's DDPM architecture
+           net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
+        
+           # Train the model
+           model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
+        
+           # Generate samples from the trained model
+           samples = model.sample(size=[batch_size, *dimensions], N=1000)
+        
+           # Compute the score for a given input
+           score = model.score(t, x)
+        
+           # Initialize the score model and its neural network from a path to a checkpoint directory
+           score = ScoreModel(checkpoint_directory)
+        
+        EnergyModel
+        ~~~~~~~~~~~
+        
+        The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
+        automatic differentiation of an energy model
+        
+        .. math::
+        
+           E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
+        
+        This is to say that the score is defined as
+        
+        .. math::
+        
+           \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
+        
+        **Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
+        neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
+        architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
+        can also be specified to make the energy positive or bounded from below.
+        
+        Training Parameters
+        ~~~~~~~~~~~~~~~~~~~
+        
+        When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
+        
+        - `dataset`: The training dataset (`torch.utils.data.Dataset`).
+        - `epochs`: The number of training epochs.
+        - `learning_rate`: The learning rate for the ADAM optimizer.
+        - `batch_size`: The batch size for training.
+        - `checkpoints_directory`: The directory to save model checkpoints (default: None).
+        - `seed`: The random seed for numpy and torch.
+        
+        Refer to the method's docstring or the class definition for more details on available parameters.
+        
+        Citations
+        ---------
+        
+        If you use this package in your research, please consider citing the following papers:
+        
+        .. code-block:: bibtex
+        
+           @inproceedings{NEURIPS2020_4c5bcfec,
+               author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
+               booktitle   = {Advances in Neural Information Processing Systems},
+               editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
+               pages       = {6840--6851},
+               publisher   = {Curran Associates, Inc.},
+               title       = {Denoising Diffusion Probabilistic Models},
+               url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
+               volume      = {33},
+               year        = {2020}
+           }
+        
+           @inproceedings{song2021scorebased,
+             title={Score-Based Generative Modeling through Stochastic Differential Equations},
+             author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
+             booktitle={International Conference on Learning Representations},
+             year={2021},
+             url={https://openreview.net/forum?id=PxTIG12RRHS}
+           }
+        
+        License
+        -------
+        
+        This package is licensed under the MIT License.
+        
+        You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
-License-File: LICENSE.txt
-
-=========================
-Score Models for Pytorch
-=========================
-
-.. image:: https://badge.fury.io/py/score_models.svg
-   :target: https://badge.fury.io/py/score_models
-.. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
-   :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
-
-A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
-
-- Simple initialization of MLP, NCSN++ and DDPM neural network architectures
-- A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
-- A sampling method based on an Euler-Maruyama discretization of an SDE.
-- A simple interface to train an energy model using DSM
-
-This repository is mainly intended for personal use.
-You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
-
-Installation
-------------
-
-To install the package, you can use pip:
-
-.. code-block:: bash
-
-   pip install torch-score-models
-
-Usage
------
-
-ScoreModel
-~~~~~~~~~~
-
-The `ScoreModel` class is the main interface for training and using score models, defined as
-
-.. math::
-
-   \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
-
-where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
-of an SDE.
-
-The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
-
-.. code-block:: python
-
-   from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
-
-   # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
-   model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
-   # ... or the VPSDE
-   model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
-
-   # NN Architectures support a Unet with 1D convolutions for time series input data
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
-   # ... or 3D convolutions for videos/voxels
-   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
-   # You can also use a simpler MLP architecture
-   net = MLP(dimensions=dim, layers=4, units=100)
-   # ... or Jonathan Ho's DDPM architecture
-   net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
-
-   # Train the model
-   model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
-
-   # Generate samples from the trained model
-   samples = model.sample(size=[batch_size, *dimensions], N=1000)
-
-   # Compute the score for a given input
-   score = model.score(t, x)
-
-   # Initialize the score model and its neural network from a path to a checkpoint directory
-   score = ScoreModel(checkpoint_directory)
-
-EnergyModel
-~~~~~~~~~~~
-
-The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
-automatic differentiation of an energy model
-
-.. math::
-
-   E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
-
-This is to say that the score is defined as
-
-.. math::
-
-   \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
-
-**Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
-neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
-architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
-can also be specified to make the energy positive or bounded from below.
-
-Training Parameters
-~~~~~~~~~~~~~~~~~~~
-
-When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
-
-- `dataset`: The training dataset (`torch.utils.data.Dataset`).
-- `epochs`: The number of training epochs.
-- `learning_rate`: The learning rate for the ADAM optimizer.
-- `batch_size`: The batch size for training.
-- `checkpoints_directory`: The directory to save model checkpoints (default: None).
-- `seed`: The random seed for numpy and torch.
-
-Refer to the method's docstring or the class definition for more details on available parameters.
-
-Citations
----------
-
-If you use this package in your research, please consider citing the following papers:
-
-.. code-block:: bibtex
-
-   @inproceedings{NEURIPS2020_4c5bcfec,
-       author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
-       booktitle   = {Advances in Neural Information Processing Systems},
-       editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
-       pages       = {6840--6851},
-       publisher   = {Curran Associates, Inc.},
-       title       = {Denoising Diffusion Probabilistic Models},
-       url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
-       volume      = {33},
-       year        = {2020}
-   }
-
-   @inproceedings{song2021scorebased,
-     title={Score-Based Generative Modeling through Stochastic Differential Equations},
-     author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
-     booktitle={International Conference on Learning Representations},
-     year={2021},
-     url={https://openreview.net/forum?id=PxTIG12RRHS}
-   }
-
-License
--------
-
-This package is licensed under the MIT License.
-
-You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
-
```

### Comparing `score_models-0.4.5/score_models.egg-info/SOURCES.txt` & `score_models-0.4.6/score_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/setup.py` & `score_models-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.4.5",
+	version="0.4.6",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.4.5/tests/test_architectures.py` & `score_models-0.4.6/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/tests/test_layers.py` & `score_models-0.4.6/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/tests/test_score_models.py` & `score_models-0.4.6/tests/test_score_models.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.5/tests/test_training.py` & `score_models-0.4.6/tests/test_training.py`

 * *Files identical despite different names*

