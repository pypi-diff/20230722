# Comparing `tmp/fastestimator-nightly-1.6.0.dev202307191402.tar.gz` & `tmp/fastestimator-nightly-1.6.0.dev202307220133.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastestimator-nightly-1.6.0.dev202307191402.tar", last modified: Wed Jul 19 14:02:18 2023, max compression
+gzip compressed data, was "fastestimator-nightly-1.6.0.dev202307220133.tar", last modified: Sat Jul 22 01:33:21 2023, max compression
```

## Comparing `fastestimator-nightly-1.6.0.dev202307191402.tar` & `fastestimator-nightly-1.6.0.dev202307220133.tar`

### file list

```diff
@@ -1,801 +1,804 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/
--rw-r--r--   0 root         (0) root         (0)    11356 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/LICENSE
--rw-r--r--   0 root         (0) root         (0)      628 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6271 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.757131 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/
--rw-r--r--   0 root         (0) root         (0)     3093 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.757131 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.761131 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1609 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7452 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/lenet.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/unet.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.761131 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/lenet.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/unet.py
--rw-r--r--   0 root         (0) root         (0)     5580 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.781130 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/
--rw-r--r--   0 root         (0) root         (0)    10420 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_abs.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_argmax.py
--rw-r--r--   0 root         (0) root         (0)     4853 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_cast.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_concat.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_convert_tensor_precision.py
--rw-r--r--   0 root         (0) root         (0)     7866 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_exp.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_flip.py
--rw-r--r--   0 root         (0) root         (0)     6816 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_gather_from_batch.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_shape.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_huber.py
--rw-r--r--   0 root         (0) root         (0)     4476 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_iwd.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     4558 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_load_model.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_maximum.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_permute.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_pow.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_roll.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_save_model.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_sign.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_smooth_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     5742 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5214 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_update_model.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_watch.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_where.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.785130 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/
--rw-r--r--   0 root         (0) root         (0)     1618 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/history.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/logs.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/plot.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.789130 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/
--rw-r--r--   0 root         (0) root         (0)     2189 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16450 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/combined_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4517 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/csv_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.797129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifair10.py
--rw-r--r--   0 root         (0) root         (0)     3118 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifair100.py
--rw-r--r--   0 root         (0) root         (0)     3447 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifar10.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifar100.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cub200.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/em_3d.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/food101.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/horse2zebra.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/imdb_review.py
--rw-r--r--   0 root         (0) root         (0)     4488 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/medmnist.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mendeley.py
--rw-r--r--   0 root         (0) root         (0)     4039 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mitmovie_ner.py
--rw-r--r--   0 root         (0) root         (0)     1338 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mnist.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/montgomery.py
--rw-r--r--   0 root         (0) root         (0)    12377 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mscoco.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/nih_chestxray.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/omniglot.py
--rw-r--r--   0 root         (0) root         (0)     9767 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/pascal_voc.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/penn_treebank.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/shakespeare.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/skl_digits.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/svhn.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/svhn_cropped.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/tednmt.py
--rw-r--r--   0 root         (0) root         (0)     4183 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/tiny_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/usps.py
--rw-r--r--   0 root         (0) root         (0)    20743 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    26711 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10140 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/op_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9011 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/siamese_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    33059 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.797129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.797129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1200 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.801129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/reflection_padding_2d.py
--rw-r--r--   0 root         (0) root         (0)    55423 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.801129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.801129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.801129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     5847 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.813129 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)     5956 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/affine.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/center_crop.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/crop.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     4920 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     4302 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/flip.py
--rw-r--r--   0 root         (0) root         (0)     4555 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     4807 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/multivariate.py
--rw-r--r--   0 root         (0) root         (0)     4654 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     5222 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_crop.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_scale.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     5023 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/read_mat.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/resize.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/rotate.py
--rw-r--r--   0 root         (0) root         (0)     6186 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/transpose.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)    16598 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.833128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)    10320 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/binarize.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/blur.py
--rw-r--r--   0 root         (0) root         (0)     3497 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/brightness.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/calibate.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/clahe.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/color.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/contrast.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/downscale.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/equalize.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/from_float.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/median_blur.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/minmax.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2978 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/normalize.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/onehot.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/posterize.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_rain.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_snow.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/read_image.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/rua.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/sharpness.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/shear_x.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/solarize.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_array.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_float.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_gray.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/translate_x.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/translate_y.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/univariate.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/word_to_id.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.833128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/argmax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.837128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7214 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/cutmix_batch.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/mixup_batch.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/average.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.837128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/fgsm.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/gradient.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.841128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)     2300 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5748 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/dice_loss.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/hinge.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     9186 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.841128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)     1454 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.841128 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10480 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/model.py
--rw-r--r--   0 root         (0) root         (0)    12067 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/update.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/normalize.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/permute.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/resize3d.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/tensorop.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)    36605 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.845127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)    10488 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.845127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/
--rw-r--r--   0 root         (0) root         (0)     1386 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/golden_section.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/grid_search.py
--rw-r--r--   0 root         (0) root         (0)     9239 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.845127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/cartesian.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/heatmap.py
--rw-r--r--   0 root         (0) root         (0)     4789 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/parallel_coordinate_plot.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/vis_util.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.849127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/
--rw-r--r--   0 root         (0) root         (0)     1412 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3554 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/axis_slicer.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/mean_unslicer.py
--rw-r--r--   0 root         (0) root         (0)    10974 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/slicer.py
--rw-r--r--   0 root         (0) root         (0)    13977 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/sliding_slicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.849127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41454 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.853127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/log_parse.py
--rw-r--r--   0 root         (0) root         (0)    33817 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/log_plot.py
--rw-r--r--   0 root         (0) root         (0)     9909 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/summary.py
--rw-r--r--   0 root         (0) root         (0)    18385 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.853127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/nightly_util.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.853127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.857127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)     1678 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3867 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.861127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/
--rw-r--r--   0 root         (0) root         (0)     2539 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7889 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     9018 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/grid_display.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/image_saver.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)    23746 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    22579 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/test_report.py
--rw-r--r--   0 root         (0) root         (0)    43469 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.861127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/meta/
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/meta/_per_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.865127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/accuracy.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/auc.py
--rw-r--r--   0 root         (0) root         (0)    10591 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/bleu_score.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/dice.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/f1_score.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/mcc.py
--rw-r--r--   0 root         (0) root         (0)    18372 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/precision.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/recall.py
--rw-r--r--   0 root         (0) root         (0)    21156 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/trace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.869127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10667 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/eigen_cam.py
--rw-r--r--   0 root         (0) root         (0)     7808 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/grad_cam.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     6905 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/label_tracker.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.869127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/types/
--rw-r--r--   0 root         (0) root         (0)     5119 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.873127 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/
--rw-r--r--   0 root         (0) root         (0)     4218 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27829 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/base_util.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/cli_util.py
--rw-r--r--   0 root         (0) root         (0)     4347 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/data.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/google_download_util.py
--rw-r--r--   0 root         (0) root         (0)    31984 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/img_data.py
--rw-r--r--   0 root         (0) root         (0)     8260 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/latex_util.py
--rw-r--r--   0 root         (0) root         (0)    58481 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    19812 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/util.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.877126 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/xai/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12171 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      628 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35887 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      718 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-19 14:02:18.000000 fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4700 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.877126 fastestimator-nightly-1.6.0.dev202307191402/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.877126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.877126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.881126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_save_model_load_model.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_update_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.881126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4980 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.881126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/dataset/test_batch_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.881126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.881126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.885126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.885126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.885126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.885126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.889126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.889126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.889126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)    10341 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     8292 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.893126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.893126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
--rw-r--r--   0 root         (0) root         (0)    22429 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_average.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.897126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_arc.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14280 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.897126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.897126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/visualize/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/visualize/test_visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.897126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_axis_slicer.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_slicer.py
--rw-r--r--   0 root         (0) root         (0)     4719 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_sliding_slicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.897126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11980 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/test_system.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_estimator.py
--rw-r--r--   0 root         (0) root         (0)    28311 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_network.py
--rw-r--r--   0 root         (0) root         (0)    98463 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.901126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.901126 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.905125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     7106 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_image_saver.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     8180 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)     3146 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_test_report.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.909125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_accuracy.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_dice.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_f1_score.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_mcc.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_precision.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_recall.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_eval_essential.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_test_essential.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_trace.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_train_essential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.913125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/
--rw-r--r--   0 root         (0) root         (0)      702 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/test_label_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.913125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_img_data.py
--rw-r--r--   0 root         (0) root         (0)    11100 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.913125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.913125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.913125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.917125 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.933124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_abs.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     6396 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_cast.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     8362 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_exp.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_gather.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_gather_from_batch.py
--rwxr-xr-x   0 root         (0) root         (0)     3742 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_iwd.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_maximum.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_permute.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_pow.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_roll.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_sign.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_watch.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_where.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.933124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/cli/test_cli_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.937124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_combine_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_csv_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_data.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13000 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.937124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.937124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.937124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.941124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.941124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/loss/test_focal_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.941124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.941124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.949124 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/test_numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.965123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.969123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.969123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.969123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     7142 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     3686 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_tensorop.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.969123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.973123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_golden_section_search.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_grid_search.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.973123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7315 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_axis_slicer.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_mean_slicer.py
--rw-r--r--   0 root         (0) root         (0)     4196 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_slicer.py
--rw-r--r--   0 root         (0) root         (0)    22534 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_sliding_slicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.973123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.977123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/logs/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/logs/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/test_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.977123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/test/test_unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.977123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.977123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/test_auc_score.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/test_bleu_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.977123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/types/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/types/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    19505 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:02:18.981123 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/xai/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/xai/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-07-19 13:53:58.000000 fastestimator-nightly-1.6.0.dev202307191402/test/run_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.180957 fastestimator-nightly-1.6.0.dev202307220133/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-22 01:33:21.180957 fastestimator-nightly-1.6.0.dev202307220133/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.944965 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.944965 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.944965 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7452 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/unet.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.948965 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/unet.py
+-rw-r--r--   0 root         (0) root         (0)     5580 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.968965 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/
+-rw-r--r--   0 root         (0) root         (0)    10420 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_cast.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_concat.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_convert_tensor_precision.py
+-rw-r--r--   0 root         (0) root         (0)     7866 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_flip.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_gather_from_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_shape.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_huber.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_roll.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_save_model.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_smooth_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     5742 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_update_model.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_watch.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_where.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.972964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/history.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.976964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16882 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/combined_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/csv_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.988964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifair10.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifair100.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifar10.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifar100.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/em_3d.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/food101.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/horse2zebra.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/imdb_review.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/medmnist.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mendeley.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mitmovie_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/montgomery.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mscoco.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/nih_chestxray.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/omniglot.py
+-rw-r--r--   0 root         (0) root         (0)     9767 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/pascal_voc.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/penn_treebank.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/shakespeare.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/skl_digits.py
+-rw-r--r--   0 root         (0) root         (0)     6097 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/svhn.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/svhn_cropped.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/tednmt.py
+-rw-r--r--   0 root         (0) root         (0)     4183 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/tiny_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/usps.py
+-rw-r--r--   0 root         (0) root         (0)    22543 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    26711 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16321 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/interleave_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10140 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/op_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/siamese_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    33059 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.988964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.988964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.988964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/reflection_padding_2d.py
+-rw-r--r--   0 root         (0) root         (0)    55423 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.988964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.992964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:20.992964 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5847 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.004963 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/affine.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/crop.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/flip.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/multivariate.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/read_mat.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/resize.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     6186 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/transpose.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)    16598 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.020963 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/binarize.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/blur.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/brightness.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/calibate.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/clahe.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/color.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/equalize.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/from_float.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/onehot.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/posterize.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/read_image.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/rua.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/solarize.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/univariate.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/word_to_id.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.024963 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/argmax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.024963 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/cutmix_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/mixup_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/average.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.028962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.028962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/dice_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/hinge.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     9186 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.032962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.032962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10480 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    12067 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/update.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/permute.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)    41667 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.032962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10918 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.036962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/golden_section.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     9239 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.036962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/cartesian.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/parallel_coordinate_plot.py
+-rw-r--r--   0 root         (0) root         (0)     5115 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/vis_util.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.040962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/mean_unslicer.py
+-rw-r--r--   0 root         (0) root         (0)    10974 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    13977 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.040962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41454 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.044962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/log_parse.py
+-rw-r--r--   0 root         (0) root         (0)    33817 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/log_plot.py
+-rw-r--r--   0 root         (0) root         (0)     9909 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/summary.py
+-rw-r--r--   0 root         (0) root         (0)    18385 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.044962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/nightly_util.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.044962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.048962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.052962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/grid_display.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)    23746 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    22579 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/test_report.py
+-rw-r--r--   0 root         (0) root         (0)    43469 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.052962 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/meta/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/meta/_per_ds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.060961 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/auc.py
+-rw-r--r--   0 root         (0) root         (0)    10591 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/bleu_score.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/dice.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/mcc.py
+-rw-r--r--   0 root         (0) root         (0)    18372 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/precision.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/recall.py
+-rw-r--r--   0 root         (0) root         (0)    21156 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/trace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.060961 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10667 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/eigen_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7808 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/grad_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/label_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.060961 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/types/
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.068961 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/
+-rw-r--r--   0 root         (0) root         (0)     4218 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27829 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/base_util.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/cli_util.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/data.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/google_download_util.py
+-rw-r--r--   0 root         (0) root         (0)    31984 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/img_data.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/latex_util.py
+-rw-r--r--   0 root         (0) root         (0)    58481 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    19845 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/util.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.068961 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/xai/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.180957 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36060 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-22 01:33:20.000000 fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 01:33:21.180957 fastestimator-nightly-1.6.0.dev202307220133/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4700 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.068961 fastestimator-nightly-1.6.0.dev202307220133/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.068961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.072961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.072961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_save_model_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_update_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.072961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.076961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/dataset/test_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11055 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/dataset/test_interleave_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.076961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.076961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.080961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.080961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.080961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.080961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.084961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.084961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.084961 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)    10341 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.088960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.088960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
+-rw-r--r--   0 root         (0) root         (0)    22429 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_average.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.092960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_arc.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    14280 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.092960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.092960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/visualize/test_visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.092960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     4719 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.096960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)    17978 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/test_system.py
+-rw-r--r--   0 root         (0) root         (0)    23833 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    28311 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_network.py
+-rw-r--r--   0 root         (0) root         (0)   100833 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.096960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.100960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.104960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4498 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     8180 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_test_report.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.108960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_dice.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_mcc.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_recall.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_eval_essential.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-07-22 01:25:25.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_test_essential.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_train_essential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.108960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/test_label_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.108960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_img_data.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.108960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.108960 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.112959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.112959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.128959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_cast.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_concat.py
+-rw-r--r--   0 root         (0) root         (0)     8362 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_gather_from_batch.py
+-rwxr-xr-x   0 root         (0) root         (0)     3742 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_roll.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_watch.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_where.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.128959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/cli/test_cli_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.132959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_combine_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_csv_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     7131 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_interleave_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.132959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.132959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.136959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.136959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.136959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/loss/test_focal_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.136959 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.140958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.148958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/test_numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.164958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.164958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.164958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.168958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     7142 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.168958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.168958 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_golden_section_search.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.172957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_mean_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_slicer.py
+-rw-r--r--   0 root         (0) root         (0)    22534 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.172957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.172957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/logs/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/test_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.172957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/test/test_unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.172957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.176957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/test_auc_score.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/test_bleu_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.176957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/types/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/types/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.176957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    19505 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 01:33:21.176957 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/xai/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/xai/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-07-22 01:25:26.000000 fastestimator-nightly-1.6.0.dev202307220133/test/run_pr_test.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/LICENSE` & `fastestimator-nightly-1.6.0.dev202307220133/LICENSE`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202307220133/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202307191402
+Version: 1.6.0.dev202307220133
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/README.md` & `fastestimator-nightly-1.6.0.dev202307220133/README.md`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/lenet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/resnet9.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/pytorch/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/pytorch/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/lenet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/resnet9.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/architecture/tensorflow/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/architecture/tensorflow/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_abs.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_argmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_cast.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_check_nan.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_concat.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_convert_tensor_precision.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_convert_tensor_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_dice_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_exp.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_gather.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_lr.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_get_shape.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_get_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_hinge.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_huber.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_huber.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_iwd.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_lambertw.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_load_model.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_matmul.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_maximum.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_ones_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_percentile.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_permute.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_pow.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_roll.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_save_model.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_save_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_set_lr.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_sign.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_smooth_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_squeeze.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_shape.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_to_type.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_update_model.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_watch.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_where.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/backend/_zscore.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/backend/_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/history.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/logs.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/logs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/main.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/plot.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/run.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/run.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/cli/train.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "generator_dataset": ["GeneratorDataset"],
         "labeled_dir_dataset": ["LabeledDirDataset"],
         "numpy_dataset": ["NumpyDataset"],
         "pickle_dataset": ["PickleDataset"],
         "siamese_dir_dataset": ["SiameseDirDataset"],
         "extend_dataset": ["ExtendDataset"],
         "combined_dataset": ["CombinedDataset"],
+        "interleave_dataset": ["InterleaveDataset"]
     },
 )
 
 if TYPE_CHECKING:
     from fastestimator.dataset import data
     from fastestimator.dataset.batch_dataset import BatchDataset
     from fastestimator.dataset.combined_dataset import CombinedDataset
@@ -42,7 +43,8 @@
     from fastestimator.dataset.dir_dataset import DirDataset
     from fastestimator.dataset.extend_dataset import ExtendDataset
     from fastestimator.dataset.generator_dataset import GeneratorDataset
     from fastestimator.dataset.labeled_dir_dataset import LabeledDirDataset
     from fastestimator.dataset.numpy_dataset import NumpyDataset
     from fastestimator.dataset.pickle_dataset import PickleDataset
     from fastestimator.dataset.siamese_dir_dataset import SiameseDirDataset
+    from fastestimator.dataset.interleave_dataset import InterleaveDataset
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/batch_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import random
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
 import numpy as np
 
 from fastestimator.dataset.dataset import DatasetSummary, FEDataset
 from fastestimator.dataset.extend_dataset import ExtendDataset
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.util.base_util import to_list, warn
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class BatchDataset(FEDataset):
     """BatchDataset extracts a list (batch) of data from a single dataset or multiple datasets.
@@ -120,14 +121,15 @@
         else:
             assert len(set(num_examples)) == 1, "the number of output samples must be the same for disjoint features"
             self.fe_batch = num_examples[0]
         self.all_fe_datasets = all([isinstance(dataset, FEDataset) for dataset in self.datasets])
         # Check ExtendDataset
         for idx, dataset in enumerate(self.datasets):
             assert not isinstance(dataset, ExtendDataset), "Input Dataset cannot be an ExtendDataset object"
+            assert not isinstance(dataset, InterleaveDataset), "Input Dataset cannot be an InterleaveDataset object"
 
     def _do_split(self, splits: Sequence[Iterable[int]]) -> List['BatchDataset']:
         """This class overwrites the .split() method instead of _do_split().
 
         Args:
             splits: Which indices to remove from the current dataset in order to create new dataset(s). One dataset will
                 be generated for every element of the `splits` sequence.
@@ -303,18 +305,20 @@
         # Don't bother re-initializing if shuffle is False
         if shuffle is False and self.index_maps:
             return
         num_samples = self.num_samples
         if self.probability:
             num_samples = num_samples * len(self.datasets)
         self.index_maps = []
-        for dataset, num_sample in zip(self.datasets, num_samples):
+        for idx, (dataset, num_sample) in enumerate(zip(self.datasets, num_samples)):
             index_map = [list(range(len(dataset))) for _ in range(math.ceil(len(self) * num_sample / len(dataset)))]
             for mapping in index_map:
                 if seed is not None:
-                    random.Random(seed).shuffle(mapping)
+                    # adding idx to the seed because we need to make sure different datasets have different index
+                    # orders, in the meantime, their random behavior should still be conditioned on seed.
+                    random.Random(seed + idx).shuffle(mapping)
                 else:
                     random.shuffle(mapping)
             if hasattr(dataset, "fe_batch_indices"):
                 self.index_maps.append([dataset.fe_batch_indices(item) for sublist in index_map for item in sublist])
             else:
                 self.index_maps.append([item for sublist in index_map for item in sublist])
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/combined_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/combined_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,33 +13,36 @@
 # limitations under the License.
 # ==============================================================================
 
 from typing import List
 
 from torch.utils.data import ConcatDataset, Dataset
 
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class CombinedDataset(ConcatDataset):
-    def __init__(self, datasets: List[Dataset]) -> None:
-        """Combines a list of PyTorch Datasets,
+    """Combines a list of PyTorch Datasets.
 
-        Args:
-            datasets: Pytorch (or FE) Datasets to be combined.
+    Args:
+        datasets: Pytorch (or FE) Datasets to be combined.
 
-        Raises:
-            AssertionError: raise exception when the input list has less than 2 datasets.
-            KeyError: raise exception when the datasets does not have same keys.
-        """
+    Raises:
+        AssertionError: raise exception when the input list has less than 2 datasets.
+        KeyError: raise exception when the datasets does not have same keys.
+    """
+    def __init__(self, datasets: List[Dataset]) -> None:
         super().__init__(datasets)
         keys = None
 
         for ds in datasets:
+            if isinstance(ds, InterleaveDataset):
+                raise AssertionError("CombinedDataset does not support InterleaveDataset")
             if isinstance(ds, Dataset) and isinstance(ds[0], dict):
                 if keys is None:
                     keys = ds[0].keys()
                 elif ds[0].keys() != keys:
                     raise KeyError("All datasets should have the same keys.")
             else:
                 raise AssertionError("Each dataset should be a type of PyTorch Dataset and should return a dictionary.")
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/breast_cancer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifair10.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifair10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifair100.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifair100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifar10.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifar10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cifar100.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cifar100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/cub200.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/cub200.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/em_3d.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/em_3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/food101.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/food101.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/horse2zebra.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/imdb_review.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/imdb_review.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/medmnist.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/medmnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mendeley.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mendeley.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mitmovie_ner.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mitmovie_ner.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mnist.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/montgomery.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/montgomery.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/mscoco.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/mscoco.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/nih_chestxray.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/nih_chestxray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/omniglot.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/omniglot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/pascal_voc.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/penn_treebank.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/penn_treebank.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/shakespeare.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/skl_digits.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/skl_digits.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/svhn.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/svhn.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/svhn_cropped.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/svhn_cropped.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/tednmt.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/tednmt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/tiny_imagenet.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/data/usps.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/data/usps.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dataloader.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from torch.utils.data import DataLoader, Sampler, _DatasetKind
 from torch.utils.data._utils.collate import default_collate, default_convert
 from torch.utils.data._utils.fetch import _MapDatasetFetcher
 from torch.utils.data.dataloader import _BaseDataLoaderIter, _MultiProcessingDataLoaderIter, \
     _SingleProcessDataLoaderIter
 
 from fastestimator.dataset.extend_dataset import ExtendDataset
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.dataset.op_dataset import OpDataset
 from fastestimator.types import FilteredData, MapDataset
 from fastestimator.util.util import Suppressor
 
 
 class PostProcessFunction(Protocol):
     def __call__(self, data: Dict[str, Any], shared: bool = True) -> Union[Dict[str, Any], FilteredData]:
@@ -105,15 +106,15 @@
                 to_yield = len(dataset)
             if drop_last:
                 to_yield -= to_yield % (batch_size or 1)
         self.fe_samples_to_yield = to_yield
         self.fe_drop_last = drop_last
         self.fe_collate_fn = collate_fn or default_collate
         if self.fe_batch_size in (0, None) and batch_size is None and self.fe_collate_fn == default_collate:
-            # The user did not provide a batch dataset nor a batch size, so default collate won't work. Have to try
+            # The user did not provide a batched dataset nor a batch size, so default collate won't work. Have to try
             # convert instead.
             self.fe_collate_fn = default_convert
         self.fe_postprocess_fn = postprocess_fn
 
         # We could disable pre-collating when num_workers=0, but this would lead to inconsistent batch ordering between
         # single- and multi-processing.
 
@@ -302,31 +303,53 @@
     while self.fe_samples_yielded < self.fe_samples_to_yield:
         collated, candidate_batch = self._next_data()
         if collated is True:  # Not regular if check since collated might be FilteredData
             self.fe_samples_yielded += 1
             return candidate_batch
         if isinstance(collated, FilteredData):
             # The batch was filtered during the forward_batch pass
-            if not collated.replacement:
-                self.fe_samples_yielded += 1
+            if isinstance(self._dataset, InterleaveDataset):
+                # We have to burn an entire cycle of data in order to ensure that the next sample comes from the desired
+                # dataset again without messing up any interactions between a fancy pattern and merge_grad
+                for _ in range(len(self._dataset.pattern) - 1):
+                    self._next_data()
+                if not collated.replacement:
+                    self.fe_samples_yielded += len(self._dataset.pattern)  # You burned this one + the rest of the cycle
+            else:
+                if not collated.replacement:
+                    self.fe_samples_yielded += 1
         else:
             # The filtered data appeared before batching, need to find it
             for instance in candidate_batch:
                 if isinstance(instance, FilteredData):
-                    if not instance.replacement:
-                        self.fe_samples_yielded += 1
+                    if isinstance(self._dataset, InterleaveDataset):
+                        # Burn data
+                        for _ in range(len(self._dataset.pattern) - 1):
+                            self._next_data()
+                        if not instance.replacement:
+                            self.fe_samples_yielded += len(self._dataset.pattern)
+                    else:
+                        if not instance.replacement:
+                            self.fe_samples_yielded += 1
                     break
             else:
                 # The else block is reached iff the for loop never breaks (probably should never get here)
                 collated = self.fe_collate_fn(candidate_batch)
                 if self.fe_postprocess_fn is not None:
                     collated = self.fe_postprocess_fn(collated, shared=False)
                     if isinstance(collated, FilteredData):
-                        if not collated.replacement:
-                            self.fe_samples_yielded += 1
+                        if isinstance(self._dataset, InterleaveDataset):
+                            # Burn data
+                            for _ in range(len(self._dataset.pattern) - 1):
+                                self._next_data()
+                            if not collated.replacement:
+                                self.fe_samples_yielded += len(self._dataset.pattern)
+                        else:
+                            if not collated.replacement:
+                                self.fe_samples_yielded += 1
                         return _next_post_batch(self)
                 self.fe_samples_yielded += 1
                 return collated
     raise StopIteration
 
 
 class _SPPreBatchIter(_BaseFELoaderIter, _SingleProcessDataLoaderIter):
@@ -358,14 +381,15 @@
     """
     def __init__(self,
                  data_source: Sized,
                  shuffle: bool = True,
                  reset_fn: Optional[Callable[[bool], None]] = None,
                  convert_fn: Optional[Callable[[int], Any]] = None):
         super().__init__(data_source=None)  # Arg is unused and triggers a warning in torch 2.1
+        self.interleave_ds = isinstance(data_source, InterleaveDataset)
         self.ds_len = len(data_source)
         if self.ds_len < 1:
             raise ValueError("dataset length must be at least 1")
         self.indices = [i for i in range(self.ds_len)]
         self.shuffle = shuffle
         self.reset_fn = reset_fn
         self.convert_fn = convert_fn
@@ -374,24 +398,26 @@
     def __len__(self):
         return self.ds_len
 
     def __iter__(self):
         self.idx = 0
         if self.reset_fn:
             self.reset_fn(self.shuffle)
-        if self.shuffle:
+        if self.shuffle and not self.interleave_ds:
+            # interleave_ds requires unshuffled indices to work correctly with its repeating pattern
             random.shuffle(self.indices)
         return self
 
     def __next__(self):
         if self.idx == self.ds_len:
             self.idx = 0
             if self.reset_fn:
                 self.reset_fn(self.shuffle)
-            if self.shuffle:
+            if self.shuffle and not self.interleave_ds:
+                # interleave_ds requires unshuffled indices to work correctly with its repeating pattern
                 random.shuffle(self.indices)
         elem = self.indices[self.idx]
         self.idx += 1
         if self.convert_fn:
             elem = self.convert_fn(elem)
         return elem
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/extend_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from torch.utils.data import Dataset
 
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.util.traceability_util import traceable
 
 
 @traceable()
 class ExtendDataset(Dataset):
     """ExtendDataset either extends or contracts the length of provided Dataset.
 
@@ -43,10 +44,11 @@
         """Verify that the given input values are valid.
         Raises:
             AssertionError: If any of the parameters are found to by unacceptable for a variety of reasons.
         """
         assert isinstance(self.spoof_length, int), "Only accept positive integer type as spoof_length"
         assert self.spoof_length > 0, "Invalid spoof_length. Expand Length cannot be less than or equal to 0"
         assert not isinstance(self.dataset, ExtendDataset), "Input Dataset cannot be an ExtendDataset object"
+        assert not isinstance(self.dataset, InterleaveDataset), "Input Dataset cannot be an InterleaveDataset object"
 
     def __getitem__(self, index):
         return self.dataset[index]
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/op_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/op_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/dataset/siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/dataset/siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/estimator.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/pytorch/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/pytorch/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/instance_norm.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/layers/tensorflow/reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/layers/tensorflow/reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/network.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/affine.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/center_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/multivariate.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/multivariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_scale.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/read_mat.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/resize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/rotate.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/multivariate/vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/multivariate/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/numpyop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/autocontrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/binarize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/brightness.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/calibate.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/calibate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/clahe.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/color.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/color_jitter.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/contrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/downscale.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/equalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/from_float.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/from_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/image_compression.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/invert_img.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/iso_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/median_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/minmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/motion_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/onehot.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/posterize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_fog.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_gamma.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_rain.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_shadow.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_shapes.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_snow.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/read_image.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/rua.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/sharpness.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/shear_x.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/shear_y.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/solarize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_array.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_float.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_gray.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/to_sepia.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/tokenize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/translate_x.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/translate_y.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/univariate.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/univariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/numpyop/univariate/word_to_id.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/numpyop/univariate/word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/op.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/argmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/augmentation/mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/augmentation/mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/average.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gather.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/fgsm.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/gradient.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/gradient/watch.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/gradient/watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/dice_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/dice_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/hinge.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/loss/super_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/loss/super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/model.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/model/update.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/model/update.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/permute.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/resize3d.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/tensorop.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/op/tensorop/un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/op/tensorop/un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/pipeline.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 import gc
 import multiprocessing as mp
 import os
 import time
 from copy import deepcopy
 from operator import mul
 from threading import Lock
-from typing import Any, Dict, List, Literal, Optional, Set, Tuple, Type, TypeVar, Union, cast, overload
+from typing import Any, Dict, Iterable, List, Literal, Optional, Set, Tuple, Type, TypeVar, Union, cast, overload
 
 import numpy as np
 import tensorflow as tf
 from torch.utils.data import DataLoader, Dataset
 from typing_extensions import Self
 
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.dataset.dataloader import FEDataLoader
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.dataset.op_dataset import OpDataset
 from fastestimator.op.numpyop.meta.fuse import Fuse
 from fastestimator.op.numpyop.meta.one_of import OneOf
 from fastestimator.op.numpyop.meta.repeat import Repeat
 from fastestimator.op.numpyop.meta.sometimes import Sometimes
 from fastestimator.op.numpyop.numpyop import Batch, NumpyOp, forward_numpyop
 from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
@@ -220,21 +221,22 @@
                 warn("ops will only be used for built-in dataset")
             if kwargs['num_process'] is not None:
                 warn("num_process will only be used for built-in dataset")
             return False
         else:
             raise ValueError("Unsupported dataset type: {}".format(type(dataset)))
 
-    def _get_op_split(self, mode: str, epoch: int, ds_id: str) -> Tuple[List[NumpyOp], Batch, List[NumpyOp]]:
+    def _get_op_split(self, mode: str, epoch: int,
+                      ds_id: Union[str, Iterable[str]]) -> Tuple[List[NumpyOp], Batch, List[NumpyOp]]:
         """Figure out which ops are pre-batch vs post-batch.
 
         Args:
             mode: The current mode.
             epoch: The current epoch.
-            ds_id: The current dataset.
+            ds_id: The current dataset id(s).
 
         Returns:
             (instance ops, batch info, batch ops).
         """
         batch_info = Batch()
         instance_ops = []
         batch_ops = []
@@ -606,29 +608,72 @@
             raise ValueError("You cannot invoke a Pipeline's __call__ method while it already has an active loader.")
         self.ctx_mode = mode
         self.ctx_epoch = epoch
         self.ctx_ds_id = ds_id
         self.ctx_shuffle = mode == 'train' if shuffle is None else shuffle
         self.ctx_steps_per_epoch = steps_per_epoch
         self.ctx_output_keys = output_keys or set()
-        self.ctx_ops, self.ctx_batch_info, self.ctx_batch_ops = self._get_op_split(mode=mode, epoch=epoch, ds_id=ds_id)
+        dataset = self.data[self.ctx_mode][self.ctx_ds_id]
+        if isinstance(dataset, Scheduler):
+            dataset = dataset.get_current_value(self.ctx_epoch)
+        self.ctx_dataset = dataset
+        if isinstance(dataset, InterleaveDataset):
+            # if this is InterleaveDataset, then build multiple ops, batch_info, and batch_ops.
+            self.ctx_ops = []
+            ctx_batch_infos: List[Batch] = []
+            ctx_batch_ops_lists: List[List[NumpyOp]] = []
+            for tag in dataset.tags:
+                id_tags = {ds_id, tag} if isinstance(tag, str) else ds_id
+                ctx_ops, ctx_batch_info, ctx_batch_ops = self._get_op_split(mode=mode, epoch=epoch, ds_id=id_tags)
+                self.ctx_ops.append(ctx_ops)
+                ctx_batch_infos.append(ctx_batch_info)
+                ctx_batch_ops_lists.append(ctx_batch_ops)
+            # Decide on the batch size (this might still be ignored later if the user is using a BatchDataset)
+            self.ctx_batch_size = [ctx_batch_info.batch_size for ctx_batch_info in ctx_batch_infos]
+            # drop_last and collate_fn for different dataset must be the same, since it is the same dataloader.
+            same_drop_last = len(set(ctx_batch_info.drop_last for ctx_batch_info in ctx_batch_infos)) == 1
+            same_collate = len(set(ctx_batch_info.collate_fn for ctx_batch_info in ctx_batch_infos)) == 1
+            if not same_collate:
+                pad_val_0 = ctx_batch_infos[0]._pad_value
+                if pad_val_0 is not None and all([pad_val_0 == pv._pad_value for pv in ctx_batch_infos[1:]]):
+                    # If the user is using pad values and all the pad values are the same, then even though the
+                    # collate functions are bound to different instances, they are all effectively the same function
+                    same_collate = True
+            assert same_drop_last and same_collate, \
+                "when using InterleaveDataset, the drop_last and collate behavior for all datasets must be the same"
+            # Interleave dataset at current scope does not support batch level, need to make sure batchops are the same
+            assert all(ctx_batch_ops_lists[0] == batch_ops for batch_ops in ctx_batch_ops_lists[1:]), \
+                "Current InterleaveDataset does not support different dataset behaviors after the BatchOp."
+            self.ctx_batch_ops = ctx_batch_ops_lists[0]
+            self.ctx_batch_info = ctx_batch_infos[0]
+            # fill in the correct batch sizes
+            for idx, batch_size in enumerate(self.ctx_batch_size):
+                if batch_size is None:
+                    batch_size = self.batch_size
+                    if isinstance(batch_size, Scheduler):
+                        batch_size = batch_size.get_current_value(self.ctx_epoch)
+                    self.ctx_batch_size[idx] = batch_size
+        else:
+            self.ctx_ops, self.ctx_batch_info, self.ctx_batch_ops = self._get_op_split(mode=mode,
+                                                                                       epoch=epoch,
+                                                                                       ds_id=ds_id)
+            # Decide on the batch size (this might still be ignored later if the user is using a BatchDataset)
+            self.ctx_batch_size = self.ctx_batch_info.batch_size
+            if self.ctx_batch_size is None:
+                # batch size
+                batch_size = self.batch_size
+                if isinstance(batch_size, Scheduler):
+                    batch_size = batch_size.get_current_value(self.ctx_epoch)
+                self.ctx_batch_size = batch_size
         # Figure out which input keys are required by the batch ops (so they don't get pruned too early)
         self.ctx_batch_input_keys = set()
         batch_produced_keys = set()
         for op in get_current_items(self.ctx_batch_ops, mode, epoch, ds_id=ds_id):
             self.ctx_batch_input_keys.update(set(key for key in op.inputs if key not in batch_produced_keys))
             batch_produced_keys.update(op.outputs)
-        # Decide on the batch size (this might still be ignored later if the user is using a BatchDataset)
-        self.ctx_batch_size = self.ctx_batch_info.batch_size
-        if self.ctx_batch_size is None:
-            # batch size
-            batch_size = self.batch_size
-            if isinstance(batch_size, Scheduler):
-                batch_size = batch_size.get_current_value(self.ctx_epoch)
-            self.ctx_batch_size = batch_size
         self.ctx_lock.release()
         return self
 
     def __enter__(self) -> Union[DataLoader, tf.data.Dataset]:
         """Get a data loader from the Pipeline for the current epoch and mode.
 
         A given pipeline can only provide one loader at a time. This helps to prevent issues with multi-threading.
@@ -652,20 +697,49 @@
         # Release the lock if arguments are invalid so that people in Jupyter / debug consoles don't get stuck
         if self.ctx_mode not in self.data:
             self.ctx_lock.release()
             raise KeyError(f"Pipeline has no data for mode '{self.ctx_mode}'")
         if self.ctx_ds_id not in self.data[self.ctx_mode]:
             self.ctx_lock.release()
             raise KeyError(f"The dataset id '{self.ctx_ds_id}' is not present in {self.ctx_mode} mode")
-        data = self.data[self.ctx_mode][self.ctx_ds_id]
-        if isinstance(data, Scheduler):
-            data = data.get_current_value(self.ctx_epoch)
-        if isinstance(data, Dataset):
+        if isinstance(self.ctx_dataset, InterleaveDataset):
+            # Results will be immediately converted to tensors, so don't need deep_remainder
+            op_datasets = [
+                OpDataset(ds,
+                          ctx_ops,
+                          self.ctx_mode,
+                          self.ctx_output_keys | self.ctx_batch_input_keys if self.ctx_output_keys else None,
+                          deep_remainder=False) for ds,
+                ctx_ops in zip(self.ctx_dataset.datasets, self.ctx_ops)
+            ]
+            self.ctx_dataset.op_datasets = op_datasets
+            # when batch_size is None, then it indicates each sample is a batch
+            self.ctx_dataset.set_batch_sizes([batch_size or 1 for batch_size in self.ctx_batch_size])
+            postprocess_fn = None
+            if self.ctx_batch_ops:
+                postprocess_fn = functools.partial(_batch_postprocess,
+                                                   ops=self.ctx_batch_ops,
+                                                   output_keys=self.ctx_output_keys,
+                                                   mode=self.ctx_mode)
+            try:
+                data = FEDataLoader(self.ctx_dataset,
+                                    postprocess_fn=postprocess_fn,
+                                    batch_size=None,
+                                    shuffle=self.ctx_shuffle,
+                                    steps_per_epoch=self.ctx_steps_per_epoch,
+                                    num_workers=self.num_process,
+                                    drop_last=self.ctx_batch_info.drop_last,
+                                    collate_fn=self.ctx_batch_info.collate_fn)
+            except ValueError as err:
+                self.ctx_lock.release()
+                raise err
+            self.ctx_loader = data
+        elif isinstance(self.ctx_dataset, Dataset):
             # Results will be immediately converted to tensors, so don't need deep_remainder
-            op_dataset = OpDataset(data,
+            op_dataset = OpDataset(self.ctx_dataset,
                                    self.ctx_ops,
                                    self.ctx_mode,
                                    self.ctx_output_keys | self.ctx_batch_input_keys if self.ctx_output_keys else None,
                                    deep_remainder=False)
             # check whether to batch the data
             batch_size = None if op_dataset.fe_batch else self.ctx_batch_size
             # Figure out whether a postprocessing function is needed (for batched ops)
@@ -684,18 +758,20 @@
                                     num_workers=self.num_process,
                                     drop_last=self.ctx_batch_info.drop_last,
                                     collate_fn=self.ctx_batch_info.collate_fn)
             except ValueError as err:
                 self.ctx_lock.release()
                 raise err
             self.ctx_loader = data
-        return data
+        else:
+            self.ctx_loader = self.ctx_dataset
+        return self.ctx_loader
 
     def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
-        if self.ctx_loader is not None:
+        if self.ctx_loader is not None and hasattr(self.ctx_loader, 'shutdown'):
             self.ctx_loader.shutdown()
             self.ctx_loader = None
         # Manually triggering gc here seems to be necessary in order to avoid problems with repeated invocations of FE
         # killing one another through multi-processing.
         gc.collect()
         self.ctx_lock.release()
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/schedule/schedule.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/schedule/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,38 +194,47 @@
     ...
 
 
 @overload
 def get_current_items(items: Iterable[Union[T, Scheduler[T]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
-                      ds_id: Optional[str] = None) -> List[T]:
+                      ds_id: Optional[Union[str, Iterable[str]]] = None) -> List[T]:
+    ...
+
+
+@overload
+def get_current_items(items: Iterable[Union[T, T2, Scheduler[T], Scheduler[T2]]],
+                      run_modes: Optional[Union[str, Iterable[str]]] = None,
+                      epoch: Optional[int] = None,
+                      ds_id: Optional[Union[str, Iterable[str]]] = None) -> List[Union[T, T2]]:
     ...
 
 
 def get_current_items(items: Iterable[Union[Any, Scheduler[Any]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
-                      ds_id: Optional[str] = None) -> List[Any]:
-    """Select items which should be executed for given mode and epoch.
+                      ds_id: Optional[Union[str, Iterable[str]]] = None) -> List[Any]:
+    """Select items which should be executed for given mode, epoch, and ds_id.
 
     Args:
         items: A list of possible items or Schedulers of items to choose from.
         run_modes: The desired execution mode. One or more of "train", "eval", "test", or "infer". If None, items of
             all modes will be returned.
         epoch: The desired execution epoch. If None, items across all epochs will be returned.
-        ds_id: The desired execution dataset id. If None, items across all ds_ids will be returned. An empty string
-            indicates that positive matches should be excluded ('' != 'ds1'), but that negative matches are satisfied
-            ('' == '!ds1').
+        ds_id: The desired one or more execution dataset id(s). If None, items across all ds_ids will be returned. An
+            empty string indicates that positive matches should be excluded ('' != 'ds1'), but that negative matches are
+            satisfied ('' == '!ds1').
 
     Returns:
         The items which should be executed.
     """
     selected_items = []
     run_modes = to_set(run_modes)
+    ds_id = to_set(ds_id)
     for item in items:
         if isinstance(item, Scheduler):
             if epoch is None:
                 item = item.get_all_values()
             else:
                 item = [item.get_current_value(epoch)]
         else:
@@ -241,25 +250,25 @@
                 if not item_.mode:
                     mode_match = True
                 elif item_.mode.intersection(run_modes):
                     mode_match = True
 
             # ds_id matching
             ds_id_match = False
-            if ds_id is None:
+            if not ds_id:
                 ds_id_match = True
             if not hasattr(item_, "ds_id"):
                 ds_id_match = True
             else:
                 # If the object has no requirements, then allow it
                 if not item_.ds_id:
                     ds_id_match = True
                 # blacklist check (before whitelist due to desired empty string behavior)
                 # if any of ds_id starts with "!", then they will all start with "!"
-                elif any([x.startswith("!") for x in item_.ds_id]) and all([ds_id != x[1:] for x in item_.ds_id]):
+                elif any([x.startswith("!") for x in item_.ds_id]) and all([x[1:] not in ds_id for x in item_.ds_id]):
                     ds_id_match = True  # Note that empty string will pass this check (unless target is literally "!")
                 # whitelist check
-                elif ds_id in item_.ds_id:
+                elif item_.ds_id.intersection(ds_id):
                     ds_id_match = True  # Note that empty string will fail this check
             if item_ and mode_match and ds_id_match:
                 selected_items.append(item_)
     return selected_items
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/golden_section.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/golden_section.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/grid_search.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/search.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/cartesian.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/cartesian.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/heatmap.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/heatmap.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/parallel_coordinate_plot.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/parallel_coordinate_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/vis_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/vis_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
         self.results = set(example_item['result'].keys())
 
         ignore_keys = to_set(ignore_keys) | {'search_idx'}
         for key in ignore_keys:
             self.params.discard(key)
             self.results.discard(key)
 
+        # Check if any results left to use
+        assert len(self.results) != 0, f"No results found after ignoring keys: {ignore_keys}"
+
         # Keep a sample parameter value to catch boring parameters
         param_samples = {}
 
         for elem in search:
             pars = elem['param']
             for k, v in pars.items():
                 if k in ignore_keys:
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/search/visualize/visualize.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/search/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/axis_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/axis_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/mean_unslicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/mean_unslicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/slicer/sliding_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/slicer/sliding_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/history.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/log_parse.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/log_parse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/logs/log_plot.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/logs/log_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/summary.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/summary/system.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/summary/system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/nightly_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/nightly_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/test/unittest_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/test/unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/early_stopping.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/adapt/terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/adapt/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/batch_display.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/csv_logger.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/grid_display.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/grid_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/image_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/image_viewer.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/model_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/tensorboard.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/test_report.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/io/traceability.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/io/traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/meta/_per_ds.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/meta/_per_ds.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/accuracy.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/auc.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/auc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/bleu_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/calibration_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/dice.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/f1_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/mcc.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/precision.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/metric/recall.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/metric/recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/trace.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/eigen_cam.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/grad_cam.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/grad_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/label_tracker.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/trace/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/trace/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/types/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/base_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/base_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/cli_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/data.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/google_download_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/google_download_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/img_data.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/latex_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/latex_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,16 +176,17 @@
             os.close(fd)
         os.close(self.fake)
         if self.show_if_exception:
             # Clear the file
             open(self.stash_name, 'w').close()
         if self.allow_pyprint:
             tf.print = print_v2
-            for line in open(self.tf_print_name, 'r'):
-                print(line, end='')  # Endings already included from tf.print
+            with open(self.tf_print_name, 'r') as f:
+                for line in f:
+                    print(line, end='')  # Endings already included from tf.print
             open(self.tf_print_name, 'w').close()
 
     def write(self, dummy: str) -> None:
         """A function which is invoked during print calls.
 
         Args:
             dummy: The string which wanted to be printed.
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/util/wget_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/util/wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202307191402
+Version: 1.6.0.dev202307220133
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/SOURCES.txt` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 ./fastestimator/dataset/combined_dataset.py
 ./fastestimator/dataset/csv_dataset.py
 ./fastestimator/dataset/dataloader.py
 ./fastestimator/dataset/dataset.py
 ./fastestimator/dataset/dir_dataset.py
 ./fastestimator/dataset/extend_dataset.py
 ./fastestimator/dataset/generator_dataset.py
+./fastestimator/dataset/interleave_dataset.py
 ./fastestimator/dataset/labeled_dir_dataset.py
 ./fastestimator/dataset/numpy_dataset.py
 ./fastestimator/dataset/op_dataset.py
 ./fastestimator/dataset/pickle_dataset.py
 ./fastestimator/dataset/siamese_dir_dataset.py
 ./fastestimator/dataset/data/__init__.py
 ./fastestimator/dataset/data/breast_cancer.py
@@ -367,14 +368,15 @@
 ./test/PR_test/integration_test/backend/test_set_lr.py
 ./test/PR_test/integration_test/backend/test_update_model.py
 ./test/PR_test/integration_test/cli/__init__.py
 ./test/PR_test/integration_test/cli/test_main.py
 ./test/PR_test/integration_test/cli/test_train.py
 ./test/PR_test/integration_test/dataset/__init__.py
 ./test/PR_test/integration_test/dataset/test_batch_dataset.py
+./test/PR_test/integration_test/dataset/test_interleave_dataset.py
 ./test/PR_test/integration_test/op/__init__.py
 ./test/PR_test/integration_test/op/test_op.py
 ./test/PR_test/integration_test/op/numpyop/__init__.py
 ./test/PR_test/integration_test/op/numpyop/meta/__init__.py
 ./test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
 ./test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
 ./test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
@@ -538,14 +540,15 @@
 ./test/PR_test/unit_test/dataset/test_batch_dataset.py
 ./test/PR_test/unit_test/dataset/test_combine_dataset.py
 ./test/PR_test/unit_test/dataset/test_csv_dataset.py
 ./test/PR_test/unit_test/dataset/test_data.py
 ./test/PR_test/unit_test/dataset/test_dir_dataset.py
 ./test/PR_test/unit_test/dataset/test_extend_dataset.py
 ./test/PR_test/unit_test/dataset/test_generator_dataset.py
+./test/PR_test/unit_test/dataset/test_interleave_dataset.py
 ./test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
 ./test/PR_test/unit_test/dataset/test_numpy_dataset.py
 ./test/PR_test/unit_test/dataset/test_pickle_dataset.py
 ./test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
 ./test/PR_test/unit_test/layers/__init__.py
 ./test/PR_test/unit_test/layers/pytorch/__init__.py
 ./test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/fastestimator_nightly.egg-info/requires.txt` & `fastestimator-nightly-1.6.0.dev202307220133/fastestimator_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/setup.py` & `fastestimator-nightly-1.6.0.dev202307220133/setup.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_get_lr.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_save_model_load_model.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_save_model_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_set_lr.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/backend/test_update_model.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/backend/test_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/test_main.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/cli/test_train.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/cli/test_train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/test_modelop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/test_modelop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/model/test_updateop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/model/test_updateop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_average.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_arc.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_arc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/schedule/test_schedule.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/schedule/test_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/search/visualize/test_visualize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/search/visualize/test_visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_axis_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_axis_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/slicer/test_sliding_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/slicer/test_sliding_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/summary/test_system.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/summary/test_system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_estimator.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_network.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/test_pipeline.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import tensorflow as tf
 import torch
 from torch.utils.data import DataLoader, Dataset
 
 import fastestimator as fe
 from fastestimator.dataset.batch_dataset import BatchDataset
 from fastestimator.dataset.extend_dataset import ExtendDataset
+from fastestimator.dataset.interleave_dataset import InterleaveDataset
 from fastestimator.dataset.numpy_dataset import NumpyDataset
 from fastestimator.op.numpyop import NumpyOp, RemoveIf
 from fastestimator.op.numpyop.numpyop import Batch
 from fastestimator.op.numpyop.univariate import Minmax
 from fastestimator.op.tensorop import TensorOp
 from fastestimator.schedule import EpochScheduler, RepeatScheduler
 from fastestimator.test.unittest_util import is_equal
@@ -232,24 +233,27 @@
             with self.assertRaises(AssertionError):
                 fe.Pipeline(train_data=data, ops=[Batch(mode='train'), Batch(mode='train')])
         with self.subTest("Simple DS Conflict"):
             with self.assertRaises(AssertionError):
                 fe.Pipeline(train_data={'ds1': data}, ops=[Batch(ds_id='ds1'), Batch(ds_id='ds1')])
         with self.subTest("Scheduler Conflict"):
             with self.assertRaises(AssertionError):
-                fe.Pipeline(train_data=data,
-                            eval_data={'ds1': data, 'ds2': data, 'ds3': data, 'ds4': data},
-                            test_data=data,
-                            ops=[EpochScheduler({1: Batch(mode='train'),
-                                                 50: Batch(mode='eval', ds_id='ds4'),
-                                                 10000: Batch(mode='test')}),
-                                 RepeatScheduler([Batch(ds_id='ds1'),
-                                                  Batch(ds_id='ds2'),
-                                                  Batch(ds_id='ds3'),
-                                                  Batch(ds_id='ds4')])])
+                fe.Pipeline(
+                    train_data=data,
+                    eval_data={
+                        'ds1': data, 'ds2': data, 'ds3': data, 'ds4': data
+                    },
+                    test_data=data,
+                    ops=[
+                        EpochScheduler({
+                            1: Batch(mode='train'), 50: Batch(mode='eval', ds_id='ds4'), 10000: Batch(mode='test')
+                        }),
+                        RepeatScheduler(
+                            [Batch(ds_id='ds1'), Batch(ds_id='ds2'), Batch(ds_id='ds3'), Batch(ds_id='ds4')])
+                    ])
 
     def test_init_with_permissible_batch_ops(self):
         data = self.sample_torch_dataset
         with self.subTest("Simple Mode Non-Conflict"):
             try:
                 fe.Pipeline(train_data=data, ops=[Batch(mode='train'), Batch(mode='eval')])
             except (AssertionError, ValueError):
@@ -262,53 +266,71 @@
         with self.subTest("Simple DS Non-Conflict (2)"):
             try:
                 fe.Pipeline(train_data={'ds1': data, 'ds2': data}, ops=[Batch(ds_id="ds1"), Batch(ds_id="ds2")])
             except (AssertionError, ValueError):
                 self.fail("Exception Occurred")
         with self.subTest("Mode/DS Non Conflict (1)"):
             try:
-                fe.Pipeline(train_data={'ds1': data, 'ds2': data},
-                            eval_data={'ds1': data, 'ds2': data},
-                            ops=[Batch(mode="train", ds_id="ds1"),
-                                 Batch(mode="eval", ds_id="ds1")])
+                fe.Pipeline(train_data={
+                    'ds1': data, 'ds2': data
+                },
+                            eval_data={
+                                'ds1': data, 'ds2': data
+                            },
+                            ops=[Batch(mode="train", ds_id="ds1"), Batch(mode="eval", ds_id="ds1")])
             except (AssertionError, ValueError):
                 self.fail("Exception Occurred")
         with self.subTest("Mode/DS Non Conflict (2)"):
             try:
-                fe.Pipeline(train_data={'ds1': data, 'ds2': data},
-                            eval_data={'ds1': data, 'ds2': data},
-                            ops=[Batch(mode="train", ds_id="ds1"),
-                                 Batch(mode="train", ds_id="ds2")])
+                fe.Pipeline(train_data={
+                    'ds1': data, 'ds2': data
+                },
+                            eval_data={
+                                'ds1': data, 'ds2': data
+                            },
+                            ops=[Batch(mode="train", ds_id="ds1"), Batch(mode="train", ds_id="ds2")])
             except (AssertionError, ValueError):
                 self.fail("Exception Occurred")
         with self.subTest("Scheduler Non Conflict"):
             try:
-                fe.Pipeline(train_data={'ds1': data, 'ds2': data},
-                            eval_data={'ds1': data, 'ds2': data},
-                            ops=[EpochScheduler({1: Batch(mode="train", ds_id="ds1"),
-                                                 5: Batch(mode="eval")}),
-                                 EpochScheduler({1: Batch(mode="eval"),
-                                                 5: Batch(mode="train", ds_id="ds1")})])
+                fe.Pipeline(
+                    train_data={
+                        'ds1': data, 'ds2': data
+                    },
+                    eval_data={
+                        'ds1': data, 'ds2': data
+                    },
+                    ops=[
+                        EpochScheduler({
+                            1: Batch(mode="train", ds_id="ds1"), 5: Batch(mode="eval")
+                        }),
+                        EpochScheduler({
+                            1: Batch(mode="eval"), 5: Batch(mode="train", ds_id="ds1")
+                        })
+                    ])
             except (AssertionError, ValueError):
                 self.fail("Exception Occurred")
         with self.subTest("Scheduler Non Conflict (2)"):
             try:
-                fe.Pipeline(train_data=data,
-                            eval_data={'ds1': data, 'ds2': data, 'ds3': data, 'ds4': data},
-                            test_data=data,
-                            ops=[EpochScheduler({1: Batch(mode='train'),
-                                                 50: Batch(mode='eval', ds_id='ds4'),
-                                                 100: Batch(mode='test')}),
-                                 RepeatScheduler([Batch(ds_id='ds1'),
-                                                  Batch(ds_id='ds2'),
-                                                  Batch(ds_id='ds3')])
-                                 ])
+                fe.Pipeline(
+                    train_data=data,
+                    eval_data={
+                        'ds1': data, 'ds2': data, 'ds3': data, 'ds4': data
+                    },
+                    test_data=data,
+                    ops=[
+                        EpochScheduler({
+                            1: Batch(mode='train'), 50: Batch(mode='eval', ds_id='ds4'), 100: Batch(mode='test')
+                        }),
+                        RepeatScheduler([Batch(ds_id='ds1'), Batch(ds_id='ds2'), Batch(ds_id='ds3')])
+                    ])
             except (AssertionError, ValueError):
                 self.fail("Exception Occurred")
 
+
 class TestPipelineGetModes(unittest.TestCase):
     """This test include:
     * fe.pipeline.Pipeline.get_modes
     * fe.schedule.schedule.EpochScheduler
     """
     def setUp(self):
         self.sample_torch_dataset = get_sample_torch_dataset()
@@ -427,16 +449,15 @@
         data = pipeline.transform(data=self.sample_data, mode="train")
         ans = {"x": np.array([[1, 2, 3]], dtype=np.float32)}
         self.assertTrue(is_equal(data, ans))
 
     def test_pipeline_transform_with_ops(self):
         pipeline = fe.Pipeline(train_data=self.sample_dataset, ops=[NumpyOpAdd1(inputs="x", outputs="y")])
         data = pipeline.transform(data=self.sample_data, mode="train")
-        ans = {"x": np.array([[1, 2, 3]], dtype=np.float32),
-               "y": np.array([[2, 3, 4]], dtype=np.float32)}
+        ans = {"x": np.array([[1, 2, 3]], dtype=np.float32), "y": np.array([[2, 3, 4]], dtype=np.float32)}
         self.assertTrue(is_equal(data, ans))
 
     def test_multi_train(self):
         pipeline = fe.Pipeline(train_data=self.sample_dataset,
                                ops=Minmax(inputs="x", outputs="x", ds_id=("ds_1", "ds_2")))
         sample_data = {"x": np.array([0, 255], dtype=np.float32)}
         data1 = pipeline.transform(data=sample_data, mode="train", ds_id="ds_1")
@@ -522,29 +543,32 @@
         data = pipeline.get_results(mode="train", epoch=1)
         data["x"] = data["x"].numpy()
         data["y"] = data["y"].numpy()
         ans = {"x": np.array([[0]], dtype=np.float32), "y": np.array([[1]], dtype=np.float32)}
         self.assertTrue(is_equal(data, ans))
 
     def test_pipeline_get_result_dict_batch_size_scheduler(self):
-        pipeline = fe.Pipeline(train_data=self.sample_torch_dataset,
-                               ops=[NumpyOpAdd1(inputs="x", outputs="y"),
-                                    EpochScheduler({1: Batch(batch_size=1, mode='train')})])
+        pipeline = fe.Pipeline(
+            train_data=self.sample_torch_dataset,
+            ops=[NumpyOpAdd1(inputs="x", outputs="y"), EpochScheduler({1: Batch(batch_size=1, mode='train')})])
         data = pipeline.get_results(mode="train", epoch=1)
         data["x"] = data["x"].numpy()
         data["y"] = data["y"].numpy()
         ans = {"x": np.array([[0]], dtype=np.float32), "y": np.array([[1]], dtype=np.float32)}
         self.assertTrue(is_equal(data, ans))
 
     def test_pipeline_get_result_dict_batch_size_train_eval(self):
-        pipeline = fe.Pipeline(train_data=self.sample_torch_dataset,
-                               eval_data=self.sample_torch_dataset,
-                               ops=[NumpyOpAdd1(inputs="x", outputs="y"),
-                                    Batch(batch_size=2, mode='train'),
-                                    Batch(batch_size=1, mode='eval')])
+        pipeline = fe.Pipeline(
+            train_data=self.sample_torch_dataset,
+            eval_data=self.sample_torch_dataset,
+            ops=[
+                NumpyOpAdd1(inputs="x", outputs="y"),
+                Batch(batch_size=2, mode='train'),
+                Batch(batch_size=1, mode='eval')
+            ])
         data_train = pipeline.get_results(mode="train", epoch=1)
         data_eval = pipeline.get_results(mode="eval", epoch=1)
         data_train["x"] = data_train["x"].numpy()
         data_train["y"] = data_train["y"].numpy()
         data_eval["x"] = data_eval["x"].numpy()
         data_eval["y"] = data_eval["y"].numpy()
         ans_train = {"x": np.array([[0], [1]], dtype=np.float32), "y": np.array([[1], [2]], dtype=np.float32)}
@@ -810,24 +834,26 @@
         data = NumpyDataset({"x": np.array([[0, 255], [255, 0]])})
         train_ds = {"ds|ds1": data}
         with self.assertRaises(AssertionError):
             fe.Pipeline(train_data=train_ds)
 
 
 class TestPipelineFilter(unittest.TestCase):
-
     def test_unbatched_no_drop_multi_filter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(10)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       num_process=n_process,
-                                       ops=[RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [6, 7]),
-                                            Batch(batch_size=4),
-                                            RemoveIf(inputs="idx", replacement=False, fn=lambda x: 0 in x)])
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    num_process=n_process,
+                    ops=[
+                        RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [6, 7]),
+                        Batch(batch_size=4),
+                        RemoveIf(inputs="idx", replacement=False, fn=lambda x: 0 in x)
+                    ])
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -843,31 +869,29 @@
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
-                    self.assertListEqual([i+1 for i in range(39)], composite_list)
+                    self.assertListEqual([i + 1 for i in range(39)], composite_list)
                 with self.subTest("shuffle True"):
                     with pipeline(mode="train", shuffle=True) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
-                    self.assertSetEqual(set([i+1 for i in range(39)]), set(composite_list))
+                    self.assertSetEqual(set([i + 1 for i in range(39)]), set(composite_list))
 
     def test_unbatched_nodrop_nofilter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -908,20 +932,19 @@
                     self.assertEqual(23, len(composite_list))
                     self.assertSetEqual(set(target), set(composite_list))  # Should visit all the data at least once
 
     def test_unbatched_nodrop_cutfilter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [2, 6, 9, 10, 11],
-                                                    inputs="idx",
-                                                    replacement=False))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [2, 6, 9, 10, 11], inputs="idx", replacement=False))
                 target = [0, 1, 3, 4, 5, 7, 8, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22]
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
@@ -938,18 +961,15 @@
                     self.assertEqual(18, len(composite_list))
                     self.assertSetEqual(set(target), set(composite_list))  # Should visit all the data at least once
 
     def test_unbatched_drop_nofilter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=Batch(drop_last=True))
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process, ops=Batch(drop_last=True))
                 with self.subTest("shuffle false"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -963,19 +983,19 @@
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
                     self.assertEqual(20, len(composite_list))  # Since shuffling don't know which will be kept
 
     def test_unbatched_drop_replacementfilter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=[RemoveIf(inputs="idx", fn=lambda x: x in [2, 6, 9, 10, 11]),
-                                            Batch(drop_last=True)])
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=[RemoveIf(inputs="idx", fn=lambda x: x in [2, 6, 9, 10, 11]), Batch(drop_last=True)])
                 target = [0, 1, 3, 4, 5, 7, 8, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 0, 1]
                 with self.subTest("shuffle false"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
@@ -991,21 +1011,22 @@
                     self.assertEqual(20, len(composite_list))  # Since shuffling don't know which will be kept
                     self.assertSetEqual(set(target), set(composite_list))  # Everything should be visited at least once
 
     def test_unbatched_drop_cutfilter(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=[RemoveIf(fn=lambda x: x in [2, 6, 9, 10, 11],
-                                                    inputs="idx",
-                                                    replacement=False),
-                                            Batch(drop_last=True)])
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=[
+                        RemoveIf(fn=lambda x: x in [2, 6, 9, 10, 11], inputs="idx", replacement=False),
+                        Batch(drop_last=True)
+                    ])
                 target = [0, 1, 3, 4, 5, 7, 8, 12, 13, 14, 15, 16, 17, 18, 19]
                 with self.subTest("shuffle false"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
@@ -1022,25 +1043,23 @@
                     # Don't know which ones, but should be no repeats at least
                     self.assertEqual(15, len(set(composite_list)))
 
     def test_unbatched_nofilter_expand(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
-                    self.assertListEqual([i for i in range(23)]*2+[i for i in range(9)], composite_list)
+                    self.assertListEqual([i for i in range(23)] * 2 + [i for i in range(9)], composite_list)
                 with self.subTest("shuffle True"):
                     with pipeline(mode="train", shuffle=True, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1048,17 +1067,15 @@
                     for i in range(23):
                         self.assertGreaterEqual(composite_list.count(i), 2)
 
     def test_unbatched_nofilter_contract(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1083,35 +1100,35 @@
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
-                    self.assertListEqual(([0, 1, 3, 4, 5, 7, 8]+list(range(12, 23)))*3+[0], composite_list)
+                    self.assertListEqual(([0, 1, 3, 4, 5, 7, 8] + list(range(12, 23))) * 3 + [0], composite_list)
                 with self.subTest("shuffle True"):
                     with pipeline(mode="train", shuffle=True, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
                     self.assertEqual(55, len(composite_list))
-                    for i in [0, 1, 3, 4, 5, 7, 8]+list(range(12, 23)):
+                    for i in [0, 1, 3, 4, 5, 7, 8] + list(range(12, 23)):
                         self.assertGreaterEqual(composite_list.count(i), 3)
 
     def test_unbatched_replacementfilter_contract(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13],
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13], inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1126,50 +1143,48 @@
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
                     self.assertEqual(10, len(set(composite_list)))  # All the elements should be unique
 
     def test_unbatched_cutfilter_expand(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(inputs="idx",
-                                                    replacement=False,
-                                                    fn=lambda x: x in [2, 6, 9, 10, 11]))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [2, 6, 9, 10, 11]))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
-                    self.assertListEqual((([0, 1, 3, 4, 5, 7, 8]+list(range(12, 23)))*3)[:43], composite_list)
+                    self.assertListEqual((([0, 1, 3, 4, 5, 7, 8] + list(range(12, 23))) * 3)[:43], composite_list)
                 with self.subTest("shuffle True"):
                     with pipeline(mode="train", shuffle=True, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
                     self.assertGreaterEqual(len(composite_list), 40)
                     self.assertLessEqual(len(composite_list), 45)
-                    for i in [0, 1, 3, 4, 5, 7, 8]+list(range(12, 23)):
+                    for i in [0, 1, 3, 4, 5, 7, 8] + list(range(12, 23)):
                         self.assertGreaterEqual(composite_list.count(i), 2)
 
     def test_unbatched_cutfilter_contract(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10],
-                                                    replacement=False,
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10], replacement=False, inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1184,17 +1199,15 @@
                     self.assertGreaterEqual(len(set(composite_list)), 2)
 
     def test_unbatched_nofilter_expandds(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data = ExtendDataset(data, spoof_length=55)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1211,17 +1224,15 @@
                         self.assertGreaterEqual(composite_list.count(i), 2)
 
     def test_unbatched_nofilter_contractds(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data = ExtendDataset(data, spoof_length=10)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1264,19 +1275,19 @@
                         self.assertGreaterEqual(composite_list.count(i), 3)
 
     def test_unbatched_replacementfilter_contractds(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data = ExtendDataset(data, spoof_length=10)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13],
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13], inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1292,20 +1303,19 @@
                     self.assertEqual(10, len(set(composite_list)))  # All the elements should be unique
 
     def test_unbatched_cutfilter_expandds(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data = ExtendDataset(data, spoof_length=55)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(inputs="idx",
-                                                    replacement=False,
-                                                    fn=lambda x: x in [2, 6, 9, 10, 11]))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [2, 6, 9, 10, 11]))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1323,20 +1333,19 @@
                         self.assertGreaterEqual(composite_list.count(i), 2)
 
     def test_unbatched_cutfilter_contractds(self):
         data = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data = ExtendDataset(data, spoof_length=10)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10],
-                                                    replacement=False,
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10], replacement=False, inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1357,33 +1366,28 @@
     def test_batched_nofilter(self):
         data_a = NumpyDataset({"a": np.array([i for i in range(23)])})
         data_b = NumpyDataset({"b": np.array([i for i in range(23)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 with self.subTest("shuffle False"):
                     data = BatchDataset(datasets=[data_a, data_b], num_samples=[3, 3])
-                    pipeline = fe.Pipeline(train_data=data,
-                                           batch_size=5,
-                                           num_process=n_process)
+                    pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_a = list(np.concatenate([batch['a'] for batch in batches]))
                     composite_b = list(np.concatenate([batch['b'] for batch in batches]))
                     self.assertEqual(24, len(composite_a))  # batch dataset will fill up the final batch
-                    self.assertListEqual(composite_a, composite_b)  # make sure that the index orders are consistent
                     self.assertEqual(23, len(set(composite_a)))  # make sure all the elements got visited
                 with self.subTest("shuffle True"):
                     # have to re-create the dataset since shuffle pollutes the state of the index maps
                     data = BatchDataset(datasets=[data_a, data_b], num_samples=[3, 3])
-                    pipeline = fe.Pipeline(train_data=data,
-                                           batch_size=5,
-                                           num_process=n_process)
+                    pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                     with pipeline(mode="train", shuffle=True) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_a = list(np.concatenate([batch['a'] for batch in batches]))
                     composite_b = list(np.concatenate([batch['b'] for batch in batches]))
@@ -1408,15 +1412,14 @@
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_a = list(np.concatenate([batch['a'] for batch in batches]))
                     composite_b = list(np.concatenate([batch['b'] for batch in batches]))
                     self.assertEqual(30, len(composite_a))  # batch dataset will fill up the final batch
-                    self.assertListEqual(composite_a, composite_b)  # make sure that the index orders are consistent
                     self.assertGreaterEqual(len(set(composite_a)), 12)  # There should be at least 4 unique batches
                 with self.subTest("shuffle True"):
                     # have to re-create the dataset since shuffle pollutes the state of the index maps
                     data = BatchDataset(datasets=[data_a, data_b], num_samples=[5, 5])
                     pipeline = fe.Pipeline(train_data=data,
                                            batch_size=5,
                                            num_process=n_process,
@@ -1445,37 +1448,32 @@
         data_b = NumpyDataset({"b": np.array([i for i in range(29)])})
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 data = BatchDataset(datasets=[data_a, data_b], num_samples=[3, 3])
                 pipeline = fe.Pipeline(train_data=data,
                                        batch_size=5,
                                        num_process=n_process,
-                                       ops=RemoveIf(inputs="a",
-                                                    replacement=False,
-                                                    fn=lambda x: x in [2, 6, 9, 10, 11]))
+                                       ops=RemoveIf(inputs="a", replacement=False, fn=lambda x: x in [2, 6, 9, 10, 11]))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_a = list(np.concatenate([batch['a'] for batch in batches]))
                     composite_b = list(np.concatenate([batch['b'] for batch in batches]))
-                    self.assertListEqual(composite_a, composite_b)  # make sure that the index orders are consistent
                     self.assertGreaterEqual(len(set(composite_a)), 12)  # There should be at least 4 unique batches
                     self.assertGreaterEqual(len(composite_a), 15)  # There should be at least 5 batches
                 with self.subTest("shuffle True"):
                     # have to re-create the dataset since shuffle pollutes the state of the index maps
                     data = BatchDataset(datasets=[data_a, data_b], num_samples=[5, 5])
                     pipeline = fe.Pipeline(train_data=data,
                                            batch_size=5,
                                            num_process=n_process,
-                                           ops=RemoveIf(inputs="a",
-                                                        replacement=False,
-                                                        fn=lambda x: x in [2, 6, 9]))
+                                           ops=RemoveIf(inputs="a", replacement=False, fn=lambda x: x in [2, 6, 9]))
                     with pipeline(mode="train", shuffle=True) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_a = list(np.concatenate([batch['a'] for batch in batches]))
                     composite_b = list(np.concatenate([batch['b'] for batch in batches]))
@@ -1492,16 +1490,15 @@
 
     def test_batched_nofilter_expand(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1521,17 +1518,15 @@
 
     def test_batched_nofilter_contract(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(25)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(25)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1574,18 +1569,18 @@
 
     def test_batched_replacementfilter_contract(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13],
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13], inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1604,17 +1599,15 @@
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 pipeline = fe.Pipeline(train_data=data,
                                        batch_size=5,
                                        num_process=n_process,
-                                       ops=RemoveIf(inputs="idx",
-                                                    replacement=False,
-                                                    fn=lambda x: x in [2, 6, 9]))
+                                       ops=RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [2, 6, 9]))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=11) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1634,17 +1627,15 @@
         data_x = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 pipeline = fe.Pipeline(train_data=data,
                                        num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in list(range(19)),
-                                                    replacement=False,
-                                                    inputs="idx"))
+                                       ops=RemoveIf(fn=lambda x: x in list(range(19)), replacement=False, inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False, steps_per_epoch=2) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     self.assertEqual(0, len(batches))
@@ -1659,17 +1650,15 @@
     def test_batched_nofilter_expandds(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         data = ExtendDataset(data, spoof_length=11)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1690,17 +1679,15 @@
     def test_batched_nofilter_contractds(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(25)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(25)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         data = ExtendDataset(data, spoof_length=2)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process)
+                pipeline = fe.Pipeline(train_data=data, batch_size=5, num_process=n_process)
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1745,19 +1732,19 @@
     def test_batched_replacementfilter_contractds(self):
         data_x = NumpyDataset({"idx": np.array([i for i in range(23)])})
         data_y = NumpyDataset({"y": np.array([i for i in range(23)])})
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         data = ExtendDataset(data, spoof_length=2)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
-                pipeline = fe.Pipeline(train_data=data,
-                                       batch_size=5,
-                                       num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13],
-                                                    inputs="idx"))
+                pipeline = fe.Pipeline(
+                    train_data=data,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=RemoveIf(fn=lambda x: x in [1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 13], inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1777,17 +1764,15 @@
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         data = ExtendDataset(data, spoof_length=11)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 pipeline = fe.Pipeline(train_data=data,
                                        batch_size=5,
                                        num_process=n_process,
-                                       ops=RemoveIf(inputs="idx",
-                                                    replacement=False,
-                                                    fn=lambda x: x in [2, 6, 9]))
+                                       ops=RemoveIf(inputs="idx", replacement=False, fn=lambda x: x in [2, 6, 9]))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     composite_list = list(np.concatenate([batch['idx'] for batch in batches]))
@@ -1809,24 +1794,123 @@
         data = BatchDataset(datasets=[data_x, data_y], num_samples=[5, 5])
         data = ExtendDataset(data, spoof_length=2)
         for n_process in [0, 7]:
             with self.subTest("proc status", workers=n_process):
                 pipeline = fe.Pipeline(train_data=data,
                                        batch_size=5,
                                        num_process=n_process,
-                                       ops=RemoveIf(fn=lambda x: x in list(range(18)),
-                                                    replacement=False,
-                                                    inputs="idx"))
+                                       ops=RemoveIf(fn=lambda x: x in list(range(18)), replacement=False, inputs="idx"))
                 with self.subTest("shuffle False"):
                     with pipeline(mode="train", shuffle=False) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     self.assertEqual(0, len(batches))
                 with self.subTest("shuffle True"):
                     with pipeline(mode="train", shuffle=True) as loader:
                         itr = iter(loader)
                         batches = []
                         for elem in itr:
                             batches.append(elem)
                     self.assertEqual(0, len(batches))
+
+    # ### Interleaved Tests ### #
+    # For now we are wasting a ton of data due to implementation of InterleaveDataset. If Torch ever resolves
+    # https://github.com/pytorch/pytorch/issues/104761 then we should switch to a data-loader based implementation and
+    # update these tests accordingly.
+    # ###               ### #
+
+    def test_interleave_drop_replacementfilter(self):
+        data1 = NumpyDataset({"idx": [f'ds1_{idx}' for idx in range(50)]})
+        data2 = NumpyDataset({"idx": [f'ds2_{idx}' for idx in range(50)]})
+        data3 = NumpyDataset({"idx": [f'ds3_{idx}' for idx in range(50)]})
+
+        interleaved = InterleaveDataset(datasets=[data1, data2, data3], pattern=[1, 0, 2, 2])
+        self.assertEqual(len(interleaved), 100)  # 25 + 25 + 50
+        for n_process in [0, 7]:
+            with self.subTest("proc status", workers=n_process):
+                pipeline = fe.Pipeline(
+                    train_data=interleaved,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=[
+                        RemoveIf(inputs="idx", fn=lambda x: x in ['ds2_5', 'ds1_10', 'ds2_20']), Batch(drop_last=True)
+                    ])
+                target = [
+                    ['ds2_0', 'ds2_1', 'ds2_2', 'ds2_3', 'ds2_4'],
+                    ['ds1_0', 'ds1_1', 'ds1_2', 'ds1_3', 'ds1_4'],
+                    ['ds3_0', 'ds3_1', 'ds3_2', 'ds3_3', 'ds3_4'],
+                    ['ds3_5', 'ds3_6', 'ds3_7', 'ds3_8', 'ds3_9'],
+                    ['ds2_10', 'ds2_11', 'ds2_12', 'ds2_13', 'ds2_14'],
+                    ['ds1_15', 'ds1_16', 'ds1_17', 'ds1_18', 'ds1_19'],
+                    ['ds3_30', 'ds3_31', 'ds3_32', 'ds3_33', 'ds3_34'],
+                    ['ds3_35', 'ds3_36', 'ds3_37', 'ds3_38', 'ds3_39'],
+                ]
+                target = target * 3
+                target = target[:20]
+                with self.subTest("shuffle false"):
+                    with pipeline(mode="train", shuffle=False) as loader:
+                        itr = iter(loader)
+                        batches = []
+                        for elem in itr:
+                            batches.append(elem)
+                    batches = [batch['idx'] for batch in batches]
+                    self.assertEqual(len(target), len(batches))
+                    for ti, bi in zip(target, batches):
+                        self.assertListEqual(ti, bi)
+                with self.subTest("shuffle true"):
+                    with pipeline(mode="train", shuffle=True) as loader:
+                        itr = iter(loader)
+                        batches = []
+                        for elem in itr:
+                            batches.append(elem)
+                    batches = [batch['idx'] for batch in batches]
+                    self.assertEqual(20, len(batches))  # Since shuffling don't know which will be kept
+
+    def test_interleave_drop_cutfilter(self):
+        data1 = NumpyDataset({"idx": [f'ds1_{idx}' for idx in range(50)]})
+        data2 = NumpyDataset({"idx": [f'ds2_{idx}' for idx in range(50)]})
+        data3 = NumpyDataset({"idx": [f'ds3_{idx}' for idx in range(50)]})
+
+        interleaved = InterleaveDataset(datasets=[data1, data2, data3], pattern=[1, 0, 2, 2])
+        self.assertEqual(len(interleaved), 100)  # 25 + 25 + 50
+        for n_process in [0, 7]:
+            with self.subTest("proc status", workers=n_process):
+                pipeline = fe.Pipeline(
+                    train_data=interleaved,
+                    batch_size=5,
+                    num_process=n_process,
+                    ops=[
+                        RemoveIf(inputs="idx",
+                                 fn=lambda x: x in ['ds2_5', 'ds1_10', 'ds2_20', 'ds3_49'],
+                                 replacement=False),
+                        Batch(drop_last=True)
+                    ])
+                target = [
+                    ['ds2_0', 'ds2_1', 'ds2_2', 'ds2_3', 'ds2_4'],
+                    ['ds1_0', 'ds1_1', 'ds1_2', 'ds1_3', 'ds1_4'],
+                    ['ds3_0', 'ds3_1', 'ds3_2', 'ds3_3', 'ds3_4'],
+                    ['ds3_5', 'ds3_6', 'ds3_7', 'ds3_8', 'ds3_9'],
+                    ['ds2_10', 'ds2_11', 'ds2_12', 'ds2_13', 'ds2_14'],
+                    ['ds1_15', 'ds1_16', 'ds1_17', 'ds1_18', 'ds1_19'],
+                    ['ds3_30', 'ds3_31', 'ds3_32', 'ds3_33', 'ds3_34'],
+                    ['ds3_35', 'ds3_36', 'ds3_37', 'ds3_38', 'ds3_39'],
+                ]
+                with self.subTest("shuffle false"):
+                    with pipeline(mode="train", shuffle=False) as loader:
+                        itr = iter(loader)
+                        batches = []
+                        for elem in itr:
+                            batches.append(elem)
+                    batches = [batch['idx'] for batch in batches]
+                    self.assertEqual(len(target), len(batches))
+                    for ti, bi in zip(target, batches):
+                        self.assertListEqual(ti, bi)
+                with self.subTest("shuffle true"):
+                    with pipeline(mode="train", shuffle=True) as loader:
+                        itr = iter(loader)
+                        batches = []
+                        for elem in itr:
+                            batches.append(elem)
+                    batches = [batch['idx'] for batch in batches]
+                    self.assertLess(len(batches), 20)  # Since shuffling don't know which will be kept
```

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_early_stopping.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_batch_display.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_csv_logger.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_image_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_image_viewer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_tensorboard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_test_report.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/io/test_traceability.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/io/test_traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_accuracy.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_calibration_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_dice.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_f1_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_mcc.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_precision.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/metric/test_recall.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/metric/test_recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_eval_essential.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_eval_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_logger.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_test_essential.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_test_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_trace.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/test_train_essential.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/test_train_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/test_instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/test_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/trace/xai/test_label_tracker.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/trace/xai/test_label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_img_data.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/integration_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/integration_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_unet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_abs.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_cast.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_check_nan.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_concat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_dice_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_exp.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_gather.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_iwd.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_lambertw.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_matmul.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_maximum.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_ones_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_percentile.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_permute.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_pow.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_roll.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_sign.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_squeeze.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_shape.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_to_type.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_watch.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_where.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/backend/test_zscore.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/backend/test_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/cli/test_cli_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_combine_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_combine_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_data.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/pytorch/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/pytorch/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/loss/test_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/loss/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/test_numpyop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/test_numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_color.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/tensorop/test_tensorop.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/tensorop/test_tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_golden_section_search.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_golden_section_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_grid_search.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/search/test_search.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/search/test_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_axis_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_axis_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_mean_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_mean_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/slicer/test_sliding_slicer.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/slicer/test_sliding_slicer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/logs/test_metrics.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/summary/test_summary.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/summary/test_summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/test/test_unittest_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/test/test_unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/test_auc_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/test_auc_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/trace/metric/test_bleu_score.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/trace/metric/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/types/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/types/test_types.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/types/test_types.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_data.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/util/test_wget_util.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/util/test_wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/PR_test/unit_test/xai/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/PR_test/unit_test/xai/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202307191402/test/run_pr_test.py` & `fastestimator-nightly-1.6.0.dev202307220133/test/run_pr_test.py`

 * *Files identical despite different names*

