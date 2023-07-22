# Comparing `tmp/imbalanced-ensemble-0.2.0.tar.gz` & `tmp/imbalanced-ensemble-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbalanced-ensemble-0.2.0.tar", last modified: Mon Feb 13 23:39:55 2023, max compression
+gzip compressed data, was "imbalanced-ensemble-0.2.1.tar", last modified: Sat Jul 22 07:41:08 2023, max compression
```

## Comparing `imbalanced-ensemble-0.2.0.tar` & `imbalanced-ensemble-0.2.1.tar`

### file list

```diff
@@ -1,991 +1,338 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.138647 imbalanced-ensemble-0.2.0/
--rw-rw-rw-   0        0        0     1089 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       90 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    39743 2023-02-13 23:39:55.137614 imbalanced-ensemble-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    38108 2023-02-13 23:07:24.000000 imbalanced-ensemble-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.254336 imbalanced-ensemble-0.2.0/docs/
--rw-rw-rw-   0        0        0    53248 2023-02-10 07:28:25.000000 imbalanced-ensemble-0.2.0/docs/.coverage
--rw-rw-rw-   0        0        0      658 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0    27378 2023-02-13 23:06:57.000000 imbalanced-ensemble-0.2.0/docs/README_CN.md
--rwxrwxrwx   0        0        0      799 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0      229 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.259319 imbalanced-ensemble-0.2.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.261330 imbalanced-ensemble-0.2.0/docs/source/_static/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.262333 imbalanced-ensemble-0.2.0/docs/source/_static/css/
--rw-rw-rw-   0        0        0       59 2021-06-13 23:32:47.000000 imbalanced-ensemble-0.2.0/docs/source/_static/css/my_theme.css
--rw-rw-rw-   0        0        0    31873 2021-06-11 04:52:45.000000 imbalanced-ensemble-0.2.0/docs/source/_static/thumbnail.png
--rw-rw-rw-   0        0        0    20254 2021-06-10 17:33:31.000000 imbalanced-ensemble-0.2.0/docs/source/_static/training_log_thumbnail.png
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.266320 imbalanced-ensemble-0.2.0/docs/source/_templates/
--rw-rw-rw-   0        0        0      508 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/_templates/class.rst
--rw-rw-rw-   0        0        0      435 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/_templates/ensemble_class.rst
--rw-rw-rw-   0        0        0      248 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/_templates/function.rst
--rw-rw-rw-   0        0        0      228 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/_templates/numpydoc_docstring.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.224785 imbalanced-ensemble-0.2.0/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.268314 imbalanced-ensemble-0.2.0/docs/source/api/datasets/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.270957 imbalanced-ensemble-0.2.0/docs/source/api/datasets/_autosummary/
--rw-rw-rw-   0        0        0      279 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/datasets/_autosummary/imbens.datasets.fetch_datasets.rst
--rw-rw-rw-   0        0        0      315 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/datasets/_autosummary/imbens.datasets.generate_imbalance_data.rst
--rw-rw-rw-   0        0        0      279 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/datasets/_autosummary/imbens.datasets.make_imbalance.rst
--rw-rw-rw-   0        0        0      175 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/datasets/api.rst
--rw-rw-rw-   0        0        0      325 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/datasets/datasets.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.276092 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.290409 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/
--rw-rw-rw-   0        0        0     1058 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaCostClassifier.rst
--rw-rw-rw-   0        0        0     1090 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaUBoostClassifier.rst
--rw-rw-rw-   0        0        0     1090 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AsymBoostClassifier.rst
--rw-rw-rw-   0        0        0      823 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalanceCascadeClassifier.rst
--rw-rw-rw-   0        0        0     1023 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalancedRandomForestClassifier.rst
--rw-rw-rw-   0        0        0     1234 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleAdaBoostClassifier.rst
--rw-rw-rw-   0        0        0      928 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleBaggingClassifier.rst
--rw-rw-rw-   0        0        0      868 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.EasyEnsembleClassifier.rst
--rw-rw-rw-   0        0        0     1202 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.KmeansSMOTEBoostClassifier.rst
--rw-rw-rw-   0        0        0      856 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBaggingClassifier.rst
--rw-rw-rw-   0        0        0     1090 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBoostClassifier.rst
--rw-rw-rw-   0        0        0     1074 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.RUSBoostClassifier.rst
--rw-rw-rw-   0        0        0      868 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBaggingClassifier.rst
--rw-rw-rw-   0        0        0     1106 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBoostClassifier.rst
--rw-rw-rw-   0        0        0      856 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.SelfPacedEnsembleClassifier.rst
--rw-rw-rw-   0        0        0      868 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.UnderBaggingClassifier.rst
--rw-rw-rw-   0        0        0      228 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/api.rst
--rw-rw-rw-   0        0        0      327 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/compatible.rst
--rw-rw-rw-   0        0        0      415 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/over-sampling.rst
--rw-rw-rw-   0        0        0      348 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/reweighting.rst
--rw-rw-rw-   0        0        0      457 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/ensemble/under-sampling.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.294051 imbalanced-ensemble-0.2.0/docs/source/api/metrics/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.300696 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/
--rw-rw-rw-   0        0        0      606 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.ValueDifferenceMetric.rst
--rw-rw-rw-   0        0        0      348 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.classification_report_imbalanced.rst
--rw-rw-rw-   0        0        0      300 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.geometric_mean_score.rst
--rw-rw-rw-   0        0        0      356 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.macro_averaged_mean_absolute_error.rst
--rw-rw-rw-   0        0        0      332 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.make_index_balanced_accuracy.rst
--rw-rw-rw-   0        0        0      288 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.sensitivity_score.rst
--rw-rw-rw-   0        0        0      344 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.sensitivity_specificity_support.rst
--rw-rw-rw-   0        0        0      288 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/_autosummary/imbens.metrics.specificity_score.rst
--rw-rw-rw-   0        0        0      192 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/api.rst
--rw-rw-rw-   0        0        0      484 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/classification.rst
--rw-rw-rw-   0        0        0      287 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/metrics/pairwise.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.302118 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.304142 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/_autosummary/
--rw-rw-rw-   0        0        0     1094 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/_autosummary/imbens.pipeline.Pipeline.rst
--rw-rw-rw-   0        0        0      275 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/_autosummary/imbens.pipeline.make_pipeline.rst
--rw-rw-rw-   0        0        0      175 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/api.rst
--rw-rw-rw-   0        0        0      364 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/pipeline/pipeline.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.307403 imbalanced-ensemble-0.2.0/docs/source/api/sampler/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.332718 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/
--rw-rw-rw-   0        0        0      490 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.ADASYN.rst
--rw-rw-rw-   0        0        0      490 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.AllKNN.rst
--rw-rw-rw-   0        0        0      650 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.BalanceCascadeUnderSampler.rst
--rw-rw-rw-   0        0        0      562 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.BorderlineSMOTE.rst
--rw-rw-rw-   0        0        0      570 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.ClusterCentroids.rst
--rw-rw-rw-   0        0        0      642 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.CondensedNearestNeighbour.rst
--rw-rw-rw-   0        0        0      626 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.EditedNearestNeighbours.rst
--rw-rw-rw-   0        0        0      642 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.InstanceHardnessThreshold.rst
--rw-rw-rw-   0        0        0      530 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.KMeansSMOTE.rst
--rw-rw-rw-   0        0        0      506 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.NearMiss.rst
--rw-rw-rw-   0        0        0      642 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.NeighbourhoodCleaningRule.rst
--rw-rw-rw-   0        0        0      578 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.OneSidedSelection.rst
--rw-rw-rw-   0        0        0      578 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RandomOverSampler.rst
--rw-rw-rw-   0        0        0      586 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RandomUnderSampler.rst
--rw-rw-rw-   0        0        0      690 2023-02-13 19:30:53.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RepeatedEditedNearestNeighbours.rst
--rw-rw-rw-   0        0        0      482 2023-02-13 19:30:54.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.SMOTE.rst
--rw-rw-rw-   0        0        0      506 2023-02-13 19:30:54.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.SVMSMOTE.rst
--rw-rw-rw-   0        0        0      610 2023-02-13 19:30:54.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.SelfPacedUnderSampler.rst
--rw-rw-rw-   0        0        0      568 2023-02-13 19:30:54.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.TomekLinks.rst
--rw-rw-rw-   0        0        0      197 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/api.rst
--rw-rw-rw-   0        0        0      373 2023-02-13 19:30:14.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/over-samplers.rst
--rw-rw-rw-   0        0        0      599 2023-02-13 19:30:10.000000 imbalanced-ensemble-0.2.0/docs/source/api/sampler/under-samplers.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.338081 imbalanced-ensemble-0.2.0/docs/source/api/utils/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.347173 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/
--rw-rw-rw-   0        0        0      310 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_balancing_schedule.rst
--rw-rw-rw-   0        0        0      290 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_eval_datasets.rst
--rw-rw-rw-   0        0        0      286 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_eval_metrics.rst
--rw-rw-rw-   0        0        0      302 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_neighbors_object.rst
--rw-rw-rw-   0        0        0      306 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_sampling_strategy.rst
--rw-rw-rw-   0        0        0      370 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_target_label_and_n_target_samples.rst
--rw-rw-rw-   0        0        0      282 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.check_target_type.rst
--rw-rw-rw-   0        0        0      270 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/_autosummary/imbens.utils.evaluate_print.rst
--rw-rw-rw-   0        0        0      216 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/api.rst
--rw-rw-rw-   0        0        0      293 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/evaluation.rst
--rw-rw-rw-   0        0        0      409 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/validation_ensemble.rst
--rw-rw-rw-   0        0        0      363 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/utils/validation_sampler.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.349166 imbalanced-ensemble-0.2.0/docs/source/api/visualizer/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.350163 imbalanced-ensemble-0.2.0/docs/source/api/visualizer/_autosummary/
--rw-rw-rw-   0        0        0      631 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.0/docs/source/api/visualizer/_autosummary/imbens.visualizer.ImbalancedEnsembleVisualizer.rst
--rw-rw-rw-   0        0        0      183 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/visualizer/api.rst
--rw-rw-rw-   0        0        0      297 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.0/docs/source/api/visualizer/visualizer.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.355746 imbalanced-ensemble-0.2.0/docs/source/auto_examples/
--rw-rw-rw-   0        0        0   124355 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/auto_examples_jupyter.zip
--rw-rw-rw-   0        0        0    75544 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/auto_examples_python.zip
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.371186 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.374870 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/
--rw-rw-rw-   0        0        0   118028 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/sphx_glr_plot_basic_example_001.png
--rw-rw-rw-   0        0        0    79546 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/sphx_glr_plot_basic_visualize_001.png
--rw-rw-rw-   0        0        0    21619 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/sphx_glr_plot_basic_visualize_002.png
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.377202 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/thumb/
--rw-rw-rw-   0        0        0    55190 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/thumb/sphx_glr_plot_basic_example_thumb.png
--rw-rw-rw-   0        0        0    24388 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/thumb/sphx_glr_plot_basic_visualize_thumb.png
--rw-rw-rw-   0        0        0    51974 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/images/thumb/sphx_glr_plot_training_log_thumb.png
--rw-rw-rw-   0        0        0     1866 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/index.rst
--rw-rw-rw-   0        0        0     6102 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example.ipynb
--rw-rw-rw-   0        0        0     3759 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example.py.md5
--rw-rw-rw-   0        0        0     9029 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example.rst
--rw-rw-rw-   0        0        0    11793 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example_codeobj.pickle
--rw-rw-rw-   0        0        0     4745 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize.ipynb
--rw-rw-rw-   0        0        0     2385 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize.py.md5
--rw-rw-rw-   0        0        0     6783 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize.rst
--rw-rw-rw-   0        0        0     4583 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize_codeobj.pickle
--rw-rw-rw-   0        0        0     6238 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log.ipynb
--rw-rw-rw-   0        0        0     3299 2023-02-13 21:22:08.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log.py.md5
--rw-rw-rw-   0        0        0    40829 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log.rst
--rw-rw-rw-   0        0        0     4091 2023-02-13 21:22:09.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log_codeobj.pickle
--rw-rw-rw-   0        0        0      977 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.407755 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.435683 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/
--rw-rw-rw-   0        0        0   760610 2023-02-13 21:22:15.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_classifier_comparison_001.png
--rw-rw-rw-   0        0        0   554993 2023-02-13 21:22:17.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_classifier_comparison_002.png
--rw-rw-rw-   0        0        0   429277 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_classifier_comparison_003.png
--rw-rw-rw-   0        0        0    33174 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_cost_matrix_001.png
--rw-rw-rw-   0        0        0    38726 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_cost_matrix_002.png
--rw-rw-rw-   0        0        0    20040 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_cost_matrix_003.png
--rw-rw-rw-   0        0        0    22240 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_cost_matrix_004.png
--rw-rw-rw-   0        0        0    48138 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_cost_matrix_005.png
--rw-rw-rw-   0        0        0    15815 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_digits_001.png
--rw-rw-rw-   0        0        0   196261 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_digits_002.png
--rw-rw-rw-   0        0        0   143979 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_digits_003.png
--rw-rw-rw-   0        0        0     5969 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_digits_004.png
--rw-rw-rw-   0        0        0    34910 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_digits_005.png
--rw-rw-rw-   0        0        0    98379 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_probability_001.png
--rw-rw-rw-   0        0        0    44530 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_001.png
--rw-rw-rw-   0        0        0    46482 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_002.png
--rw-rw-rw-   0        0        0    47413 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_003.png
--rw-rw-rw-   0        0        0    51072 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_004.png
--rw-rw-rw-   0        0        0    46497 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_005.png
--rw-rw-rw-   0        0        0    45431 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_006.png
--rw-rw-rw-   0        0        0    47882 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_007.png
--rw-rw-rw-   0        0        0    51836 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_008.png
--rw-rw-rw-   0        0        0   100646 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_resampling_target_009.png
--rw-rw-rw-   0        0        0    23278 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_sampling_schedule_001.png
--rw-rw-rw-   0        0        0    27348 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_sampling_schedule_002.png
--rw-rw-rw-   0        0        0    45913 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/sphx_glr_plot_sampling_schedule_003.png
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.441601 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/
--rw-rw-rw-   0        0        0    96754 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_classifier_comparison_thumb.png
--rw-rw-rw-   0        0        0    17780 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_cost_matrix_thumb.png
--rw-rw-rw-   0        0        0    20316 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_digits_thumb.png
--rw-rw-rw-   0        0        0    44278 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_probability_thumb.png
--rw-rw-rw-   0        0        0    30832 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_resampling_target_thumb.png
--rw-rw-rw-   0        0        0    41791 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/images/thumb/sphx_glr_plot_sampling_schedule_thumb.png
--rw-rw-rw-   0        0        0     3689 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/index.rst
--rw-rw-rw-   0        0        0    10280 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.ipynb
--rw-rw-rw-   0        0        0     7661 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.py.md5
--rw-rw-rw-   0        0        0    13115 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.rst
--rw-rw-rw-   0        0        0     7968 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison_codeobj.pickle
--rw-rw-rw-   0        0        0    10367 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix.ipynb
--rw-rw-rw-   0        0        0     5807 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix.py.md5
--rw-rw-rw-   0        0        0    10881 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix.rst
--rw-rw-rw-   0        0        0     8833 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix_codeobj.pickle
--rw-rw-rw-   0        0        0     7697 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits.ipynb
--rw-rw-rw-   0        0        0     4579 2023-02-13 21:22:10.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits.py.md5
--rw-rw-rw-   0        0        0    10253 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits.rst
--rw-rw-rw-   0        0        0    12211 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits_codeobj.pickle
--rw-rw-rw-   0        0        0     5614 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability.ipynb
--rw-rw-rw-   0        0        0     3730 2023-02-13 21:22:11.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability.py.md5
--rw-rw-rw-   0        0        0     6219 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability.rst
--rw-rw-rw-   0        0        0    13972 2023-02-13 21:22:12.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability_codeobj.pickle
--rw-rw-rw-   0        0        0    13679 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target.ipynb
--rw-rw-rw-   0        0        0     8979 2023-02-13 21:22:18.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target.py.md5
--rw-rw-rw-   0        0        0    22100 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target.rst
--rw-rw-rw-   0        0        0    14026 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target_codeobj.pickle
--rw-rw-rw-   0        0        0    14480 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule.ipynb
--rw-rw-rw-   0        0        0     8679 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule.py.md5
--rw-rw-rw-   0        0        0    62380 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule.rst
--rw-rw-rw-   0        0        0    17634 2023-02-13 21:22:13.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule_codeobj.pickle
--rw-rw-rw-   0        0        0     1958 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.457207 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.464559 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/
--rw-rw-rw-   0        0        0   135977 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_generate_imbalance_001.png
--rw-rw-rw-   0        0        0    74417 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_001.png
--rw-rw-rw-   0        0        0   348420 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_002.png
--rw-rw-rw-   0        0        0    15815 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_digits_001.png
--rw-rw-rw-   0        0        0   196261 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_digits_002.png
--rw-rw-rw-   0        0        0   143979 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_digits_003.png
--rw-rw-rw-   0        0        0   392258 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/sphx_glr_plot_make_imbalance_digits_004.png
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.468546 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/thumb/
--rw-rw-rw-   0        0        0    45779 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/thumb/sphx_glr_plot_generate_imbalance_thumb.png
--rw-rw-rw-   0        0        0    82300 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/thumb/sphx_glr_plot_make_imbalance_digits_thumb.png
--rw-rw-rw-   0        0        0    43434 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/images/thumb/sphx_glr_plot_make_imbalance_thumb.png
--rw-rw-rw-   0        0        0     1931 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/index.rst
--rw-rw-rw-   0        0        0     2635 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance.ipynb
--rw-rw-rw-   0        0        0      979 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance.py.md5
--rw-rw-rw-   0        0        0     3286 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance.rst
--rw-rw-rw-   0        0        0      914 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance_codeobj.pickle
--rw-rw-rw-   0        0        0     4369 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance.ipynb
--rw-rw-rw-   0        0        0     2516 2023-02-13 21:22:19.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance.py.md5
--rw-rw-rw-   0        0        0     4810 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance.rst
--rw-rw-rw-   0        0        0     4422 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_codeobj.pickle
--rw-rw-rw-   0        0        0     5399 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits.ipynb
--rw-rw-rw-   0        0        0     3258 2023-02-13 21:22:20.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits.py.md5
--rw-rw-rw-   0        0        0     6344 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits.rst
--rw-rw-rw-   0        0        0     8600 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits_codeobj.pickle
--rw-rw-rw-   0        0        0     1088 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.479923 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.230765 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/images/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.481812 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/images/thumb/
--rw-rw-rw-   0        0        0    24159 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/images/thumb/sphx_glr_plot_classification_report_thumb.png
--rw-rw-rw-   0        0        0    24159 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/images/thumb/sphx_glr_plot_metrics_thumb.png
--rw-rw-rw-   0        0        0     1437 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/index.rst
--rw-rw-rw-   0        0        0     2613 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report.ipynb
--rw-rw-rw-   0        0        0     1676 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report.py.md5
--rw-rw-rw-   0        0        0     3537 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report.rst
--rw-rw-rw-   0        0        0     4782 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report_codeobj.pickle
--rw-rw-rw-   0        0        0     6006 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics.ipynb
--rw-rw-rw-   0        0        0     3028 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics.py.md5
--rw-rw-rw-   0        0        0     5406 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics.rst
--rw-rw-rw-   0        0        0     5282 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics_codeobj.pickle
--rw-rw-rw-   0        0        0      842 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/sg_execution_times.rst
--rw-rw-rw-   0        0        0    10963 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/index.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.487792 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.231517 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/images/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.488789 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/images/thumb/
--rw-rw-rw-   0        0        0    24159 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/images/thumb/sphx_glr_plot_pipeline_classification_thumb.png
--rw-rw-rw-   0        0        0      891 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/index.rst
--rw-rw-rw-   0        0        0     4583 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification.ipynb
--rw-rw-rw-   0        0        0     2345 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification.py.md5
--rw-rw-rw-   0        0        0     4640 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification.rst
--rw-rw-rw-   0        0        0     8972 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification_codeobj.pickle
--rw-rw-rw-   0        0        0      580 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/sg_execution_times.rst
--rw-rw-rw-   0        0        0      340 2023-02-13 21:22:50.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/searchindex.bak
--rw-rw-rw-   0        0        0   155783 2023-02-13 21:22:50.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/searchindex.dat
--rw-rw-rw-   0        0        0      340 2023-02-13 21:22:50.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/searchindex.dir
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.499372 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.509998 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/
--rw-rw-rw-   0        0        0    84374 2023-02-13 21:22:32.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_confusion_matrix_001.png
--rw-rw-rw-   0        0        0    83767 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_confusion_matrix_002.png
--rw-rw-rw-   0        0        0    34378 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_confusion_matrix_003.png
--rw-rw-rw-   0        0        0    59337 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_confusion_matrix_004.png
--rw-rw-rw-   0        0        0   110250 2023-02-13 21:22:37.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_001.png
--rw-rw-rw-   0        0        0    89898 2023-02-13 21:22:37.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_002.png
--rw-rw-rw-   0        0        0    63029 2023-02-13 21:22:37.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_003.png
--rw-rw-rw-   0        0        0    74244 2023-02-13 21:22:37.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_004.png
--rw-rw-rw-   0        0        0    84295 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_005.png
--rw-rw-rw-   0        0        0   128242 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/sphx_glr_plot_performance_curve_006.png
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.511502 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/thumb/
--rw-rw-rw-   0        0        0    33004 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/thumb/sphx_glr_plot_confusion_matrix_thumb.png
--rw-rw-rw-   0        0        0    68165 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/images/thumb/sphx_glr_plot_performance_curve_thumb.png
--rw-rw-rw-   0        0        0     1388 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/index.rst
--rw-rw-rw-   0        0        0     7523 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix.ipynb
--rw-rw-rw-   0        0        0     4602 2023-02-13 21:22:27.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix.py.md5
--rw-rw-rw-   0        0        0    16200 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix.rst
--rw-rw-rw-   0        0        0    12899 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix_codeobj.pickle
--rw-rw-rw-   0        0        0     9441 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve.ipynb
--rw-rw-rw-   0        0        0     5780 2023-02-13 21:22:33.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve.py
--rw-rw-rw-   0        0        0       32 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve.py.md5
--rw-rw-rw-   0        0        0    18164 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve.rst
--rw-rw-rw-   0        0        0    12883 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve_codeobj.pickle
--rw-rw-rw-   0        0        0      802 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.956304 imbalanced-ensemble-0.2.0/docs/source/back_references/
--rw-rw-rw-   0        0        0      766 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.AdaCostClassifier.examples
--rw-rw-rw-   0        0        0      774 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.AdaCostClassifier.fit.examples
--rw-rw-rw-   0        0        0     1374 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BalancedRandomForestClassifier.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseCleaningSampler.examples
--rw-rw-rw-   0        0        0      800 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseImbalancedEnsemble.estimator_.examples
--rw-rw-rw-   0        0        0     5464 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseImbalancedEnsemble.examples
--rw-rw-rw-   0        0        0     3757 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseImbalancedEnsemble.fit.examples
--rw-rw-rw-   0        0        0     2006 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseImbalancedEnsemble.predict.examples
--rw-rw-rw-   0        0        0     1420 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseImbalancedEnsemble.predict_proba.examples
--rw-rw-rw-   0        0        0     2022 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseOverSampler.examples
--rw-rw-rw-   0        0        0     2010 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseSMOTE.examples
--rw-rw-rw-   0        0        0     2014 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.BaseSampler.examples
--rw-rw-rw-   0        0        0     1358 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.EasyEnsembleClassifier.examples
--rw-rw-rw-   0        0        0      830 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.EditedNearestNeighbours.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleClassifierMixin.estimator_.examples
--rw-rw-rw-   0        0        0     6642 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleClassifierMixin.examples
--rw-rw-rw-   0        0        0     5483 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleClassifierMixin.fit.examples
--rw-rw-rw-   0        0        0     2028 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleClassifierMixin.predict.examples
--rw-rw-rw-   0        0        0     1442 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleClassifierMixin.predict_proba.examples
--rw-rw-rw-   0        0        0     2015 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleVisualizer.confusion_matrix_heatmap.examples
--rw-rw-rw-   0        0        0     2540 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleVisualizer.examples
--rw-rw-rw-   0        0        0     1950 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleVisualizer.fit.examples
--rw-rw-rw-   0        0        0     1416 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ImbalancedEnsembleVisualizer.performance_lineplot.examples
--rw-rw-rw-   0        0        0     2008 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.Pipeline.examples
--rw-rw-rw-   0        0        0     2016 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.Pipeline.fit.examples
--rw-rw-rw-   0        0        0     2024 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.Pipeline.predict.examples
--rw-rw-rw-   0        0        0     1959 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ResampleBaggingClassifier.examples
--rw-rw-rw-   0        0        0     1372 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ResampleBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0     1415 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ResampleBoostClassifier.examples
--rw-rw-rw-   0        0        0     1423 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ResampleBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0      778 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ReweightBoostClassifier.examples
--rw-rw-rw-   0        0        0      786 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ReweightBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0     2002 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SMOTE.examples
--rw-rw-rw-   0        0        0     1358 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SMOTEBaggingClassifier.examples
--rw-rw-rw-   0        0        0     1366 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SMOTEBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0     1409 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SMOTEBoostClassifier.examples
--rw-rw-rw-   0        0        0     1417 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SMOTEBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0     2016 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SamplerMixin.examples
--rw-rw-rw-   0        0        0      810 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SelfPacedEnsembleClassifier.estimator_.examples
--rw-rw-rw-   0        0        0     5474 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SelfPacedEnsembleClassifier.examples
--rw-rw-rw-   0        0        0     3767 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SelfPacedEnsembleClassifier.fit.examples
--rw-rw-rw-   0        0        0     2016 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SelfPacedEnsembleClassifier.predict.examples
--rw-rw-rw-   0        0        0     1430 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.SelfPacedEnsembleClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0      810 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.UnderBaggingClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.datasets.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.datasets.fetch_datasets.examples
--rw-rw-rw-   0        0        0      821 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.datasets.generate_imbalance_data.examples
--rw-rw-rw-   0        0        0     3207 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.datasets.make_imbalance.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0     1379 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0      792 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaCostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AdaUBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.AsymBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      832 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalanceCascadeClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.apply.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.decision_path.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.estimator_.examples
--rw-rw-rw-   0        0        0     1987 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:39.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BalancedRandomForestClassifier.set_params.examples
--rw-rw-rw-   0        0        0      818 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BaseImbalancedEnsemble.estimator_.examples
--rw-rw-rw-   0        0        0     5482 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BaseImbalancedEnsemble.examples
--rw-rw-rw-   0        0        0     3775 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BaseImbalancedEnsemble.fit.examples
--rw-rw-rw-   0        0        0     2024 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BaseImbalancedEnsemble.predict.examples
--rw-rw-rw-   0        0        0     1438 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.BaseImbalancedEnsemble.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleAdaBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.estimators_samples_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.CompatibleBaggingClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.estimators_samples_.examples
--rw-rw-rw-   0        0        0     1971 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.EasyEnsembleClassifier.set_params.examples
--rw-rw-rw-   0        0        0      840 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ImbalancedEnsembleClassifierMixin.estimator_.examples
--rw-rw-rw-   0        0        0     6660 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ImbalancedEnsembleClassifierMixin.examples
--rw-rw-rw-   0        0        0     5501 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ImbalancedEnsembleClassifierMixin.fit.examples
--rw-rw-rw-   0        0        0     2046 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ImbalancedEnsembleClassifierMixin.predict.examples
--rw-rw-rw-   0        0        0     1460 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ImbalancedEnsembleClassifierMixin.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      836 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.KmeansSMOTEBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.estimators_samples_.examples
--rw-rw-rw-   0        0        0      826 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:40.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBaggingClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.OverBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0      820 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.RUSBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0     1977 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ResampleBaggingClassifier.examples
--rw-rw-rw-   0        0        0     1390 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ResampleBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0     1433 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ResampleBoostClassifier.examples
--rw-rw-rw-   0        0        0     1441 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ResampleBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0      796 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ReweightBoostClassifier.examples
--rw-rw-rw-   0        0        0      804 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.ReweightBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.estimators_samples_.examples
--rw-rw-rw-   0        0        0     1971 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.examples
--rw-rw-rw-   0        0        0     1384 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBaggingClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.estimator_.examples
--rw-rw-rw-   0        0        0     2022 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0     1435 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.staged_decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.staged_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.staged_predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:41.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SMOTEBoostClassifier.staged_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.decision_function.examples
--rw-rw-rw-   0        0        0      828 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.estimator_.examples
--rw-rw-rw-   0        0        0     6087 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.feature_importances_.examples
--rw-rw-rw-   0        0        0     3785 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.get_params.examples
--rw-rw-rw-   0        0        0     2034 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.predict.examples
--rw-rw-rw-   0        0        0     1448 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.SelfPacedEnsembleClassifier.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.base_estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.decision_function.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.estimator_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.estimators_samples_.examples
--rw-rw-rw-   0        0        0      828 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.UnderBaggingClassifier.set_params.examples
--rw-rw-rw-   0        0        0     1995 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._bagging.ResampleBaggingClassifier.examples
--rw-rw-rw-   0        0        0     1408 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._bagging.ResampleBaggingClassifier.fit.examples
--rw-rw-rw-   0        0        0     1447 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._boost.ResampleBoostClassifier.examples
--rw-rw-rw-   0        0        0     1455 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._boost.ResampleBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0      810 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._boost.ReweightBoostClassifier.examples
--rw-rw-rw-   0        0        0      818 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._boost.ReweightBoostClassifier.fit.examples
--rw-rw-rw-   0        0        0      842 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble._reweighting.__init__.__all__.examples
--rw-rw-rw-   0        0        0      828 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.BaseImbalancedEnsemble.estimator_.examples
--rw-rw-rw-   0        0        0     5492 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.BaseImbalancedEnsemble.examples
--rw-rw-rw-   0        0        0     3785 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.BaseImbalancedEnsemble.fit.examples
--rw-rw-rw-   0        0        0     2034 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.BaseImbalancedEnsemble.predict.examples
--rw-rw-rw-   0        0        0     1448 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.BaseImbalancedEnsemble.predict_proba.examples
--rw-rw-rw-   0        0        0      850 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.ImbalancedEnsembleClassifierMixin.estimator_.examples
--rw-rw-rw-   0        0        0     6670 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.ImbalancedEnsembleClassifierMixin.examples
--rw-rw-rw-   0        0        0     5511 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.ImbalancedEnsembleClassifierMixin.fit.examples
--rw-rw-rw-   0        0        0     2056 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.ImbalancedEnsembleClassifierMixin.predict.examples
--rw-rw-rw-   0        0        0     1470 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.ImbalancedEnsembleClassifierMixin.predict_proba.examples
--rw-rw-rw-   0        0        0     3167 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.base.sort_dict_by_key.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.ensemble.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.ValueDifferenceMetric.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.ValueDifferenceMetric.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.ValueDifferenceMetric.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.ValueDifferenceMetric.pairwise.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.ValueDifferenceMetric.set_params.examples
--rw-rw-rw-   0        0        0      882 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.classification_report_imbalanced.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.examples
--rw-rw-rw-   0        0        0      804 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.geometric_mean_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.macro_averaged_mean_absolute_error.examples
--rw-rw-rw-   0        0        0      820 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.make_index_balanced_accuracy.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.sensitivity_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.sensitivity_specificity_support.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.metrics.specificity_score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.classes_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.decision_function.examples
--rw-rw-rw-   0        0        0     2026 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.feature_names_in_.examples
--rw-rw-rw-   0        0        0     2034 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.fit_predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.fit_transform.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.get_feature_names_out.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.inverse_transform.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.n_features_in_.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.named_steps.examples
--rw-rw-rw-   0        0        0     2042 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.predict.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.predict_log_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.predict_proba.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.score.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.score_samples.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.set_output.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:42.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.Pipeline.transform.examples
--rw-rw-rw-   0        0        0     2036 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.pipeline.make_pipeline.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ADASYN.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ADASYN.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ADASYN.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ADASYN.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ADASYN.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.AllKNN.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.AllKNN.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.AllKNN.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.AllKNN.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.AllKNN.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BalanceCascadeUnderSampler.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BalanceCascadeUnderSampler.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BalanceCascadeUnderSampler.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BalanceCascadeUnderSampler.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BalanceCascadeUnderSampler.set_params.examples
--rw-rw-rw-   0        0        0      838 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BaseCleaningSampler.examples
--rw-rw-rw-   0        0        0     2038 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BaseOverSampler.examples
--rw-rw-rw-   0        0        0     2026 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BaseSMOTE.examples
--rw-rw-rw-   0        0        0     2030 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BaseSampler.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BorderlineSMOTE.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BorderlineSMOTE.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BorderlineSMOTE.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BorderlineSMOTE.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.BorderlineSMOTE.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ClusterCentroids.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ClusterCentroids.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ClusterCentroids.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ClusterCentroids.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.ClusterCentroids.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.CondensedNearestNeighbour.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.CondensedNearestNeighbour.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.CondensedNearestNeighbour.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.CondensedNearestNeighbour.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.CondensedNearestNeighbour.set_params.examples
--rw-rw-rw-   0        0        0      846 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.EditedNearestNeighbours.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.EditedNearestNeighbours.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.EditedNearestNeighbours.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.EditedNearestNeighbours.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.EditedNearestNeighbours.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.InstanceHardnessThreshold.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.InstanceHardnessThreshold.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.InstanceHardnessThreshold.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.InstanceHardnessThreshold.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:43.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.InstanceHardnessThreshold.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.KMeansSMOTE.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.KMeansSMOTE.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.KMeansSMOTE.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.KMeansSMOTE.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.KMeansSMOTE.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NearMiss.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NearMiss.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NearMiss.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NearMiss.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NearMiss.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NeighbourhoodCleaningRule.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NeighbourhoodCleaningRule.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NeighbourhoodCleaningRule.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NeighbourhoodCleaningRule.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.NeighbourhoodCleaningRule.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.OneSidedSelection.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.OneSidedSelection.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.OneSidedSelection.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.OneSidedSelection.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.OneSidedSelection.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomOverSampler.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomOverSampler.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomOverSampler.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomOverSampler.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomOverSampler.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomUnderSampler.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomUnderSampler.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomUnderSampler.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomUnderSampler.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RandomUnderSampler.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RepeatedEditedNearestNeighbours.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RepeatedEditedNearestNeighbours.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RepeatedEditedNearestNeighbours.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RepeatedEditedNearestNeighbours.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.RepeatedEditedNearestNeighbours.set_params.examples
--rw-rw-rw-   0        0        0     2018 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SMOTE.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SMOTE.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SMOTE.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SMOTE.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SMOTE.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SVMSMOTE.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SVMSMOTE.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SVMSMOTE.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SVMSMOTE.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SVMSMOTE.set_params.examples
--rw-rw-rw-   0        0        0     2032 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SamplerMixin.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SelfPacedUnderSampler.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:44.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SelfPacedUnderSampler.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SelfPacedUnderSampler.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SelfPacedUnderSampler.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.SelfPacedUnderSampler.set_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.fit.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.fit_resample.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.get_params.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.is_tomek.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.TomekLinks.set_params.examples
--rw-rw-rw-   0        0        0     2068 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._over_sampling.BaseOverSampler.examples
--rw-rw-rw-   0        0        0     2056 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._over_sampling.BaseSMOTE.examples
--rw-rw-rw-   0        0        0     2070 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._over_sampling._smote.BaseSMOTE.examples
--rw-rw-rw-   0        0        0     2080 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._over_sampling._smote.base.BaseSMOTE.examples
--rw-rw-rw-   0        0        0     2078 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._over_sampling.base.BaseOverSampler.examples
--rw-rw-rw-   0        0        0      870 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._under_sampling.BaseCleaningSampler.examples
--rw-rw-rw-   0        0        0      880 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler._under_sampling.base.BaseCleaningSampler.examples
--rw-rw-rw-   0        0        0     2040 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.base.BaseSampler.examples
--rw-rw-rw-   0        0        0     2042 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.base.SamplerMixin.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.sampler.examples
--rw-rw-rw-   0        0        0     2615 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils._plot.plot_2Dprojection_and_cardinality.examples
--rw-rw-rw-   0        0        0      826 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils._plot.plot_scatter.examples
--rw-rw-rw-   0        0        0     1419 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils._plot.set_ax_border.examples
--rw-rw-rw-   0        0        0      864 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils._validation_param._progressive_schedule.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_balancing_schedule.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_eval_datasets.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_eval_metrics.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_neighbors_object.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_sampling_strategy.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_target_label_and_n_target_samples.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.check_target_type.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.evaluate_print.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.examples
--rw-rw-rw-   0        0        0      822 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.utils.testing.all_estimators.examples
--rw-rw-rw-   0        0        0     2037 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.visualizer.ImbalancedEnsembleVisualizer.confusion_matrix_heatmap.examples
--rw-rw-rw-   0        0        0     2562 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.visualizer.ImbalancedEnsembleVisualizer.examples
--rw-rw-rw-   0        0        0     1972 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.visualizer.ImbalancedEnsembleVisualizer.fit.examples
--rw-rw-rw-   0        0        0     1438 2023-02-13 21:22:38.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.visualizer.ImbalancedEnsembleVisualizer.performance_lineplot.examples
--rw-rw-rw-   0        0        0        0 2023-02-13 21:22:45.000000 imbalanced-ensemble-0.2.0/docs/source/back_references/imbens.visualizer.examples
--rw-rw-rw-   0        0        0     4047 2023-02-13 18:58:24.000000 imbalanced-ensemble-0.2.0/docs/source/conf.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 18:58:25.000000 imbalanced-ensemble-0.2.0/docs/source/get_start.rst
--rw-rw-rw-   0        0        0     7580 2023-02-13 23:08:00.000000 imbalanced-ensemble-0.2.0/docs/source/index.rst
--rw-rw-rw-   0        0        0      917 2021-11-25 14:01:00.000000 imbalanced-ensemble-0.2.0/docs/source/install.rst
--rw-rw-rw-   0        0        0     5945 2023-02-13 19:19:35.000000 imbalanced-ensemble-0.2.0/docs/source/release_history.rst
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.961865 imbalanced-ensemble-0.2.0/docs/source/sphinxext/
--rw-rw-rw-   0        0        0     6132 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/sphinxext/LICENSE.txt
--rw-rw-rw-   0        0        0       45 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/sphinxext/MANIFEST.in
--rw-rw-rw-   0        0        0     1748 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/sphinxext/README.txt
--rw-rw-rw-   0        0        0     2699 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/sphinxext/github_link.py
--rw-rw-rw-   0        0        0     8338 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.0/docs/source/sphinxext/sphinx_issues.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.961865 imbalanced-ensemble-0.2.0/examples/
--rw-rw-rw-   0        0        0      244 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.965589 imbalanced-ensemble-0.2.0/examples/basic/
--rw-rw-rw-   0        0        0      137 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/basic/README.txt
--rw-rw-rw-   0        0        0     3759 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/basic/plot_basic_example.py
--rw-rw-rw-   0        0        0     2385 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/basic/plot_basic_visualize.py
--rw-rw-rw-   0        0        0     3299 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/basic/plot_training_log.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.971925 imbalanced-ensemble-0.2.0/examples/classification/
--rw-rw-rw-   0        0        0      198 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/classification/README.txt
--rw-rw-rw-   0        0        0     7661 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_classifier_comparison.py
--rw-rw-rw-   0        0        0     5807 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_cost_matrix.py
--rw-rw-rw-   0        0        0     4579 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_digits.py
--rw-rw-rw-   0        0        0     3730 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_probability.py
--rw-rw-rw-   0        0        0     8979 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_resampling_target.py
--rw-rw-rw-   0        0        0     8679 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/classification/plot_sampling_schedule.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.975686 imbalanced-ensemble-0.2.0/examples/datasets/
--rw-rw-rw-   0        0        0      126 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/datasets/README.txt
--rw-rw-rw-   0        0        0      979 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/datasets/plot_generate_imbalance.py
--rw-rw-rw-   0        0        0     2516 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/datasets/plot_make_imbalance.py
--rw-rw-rw-   0        0        0     3258 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/datasets/plot_make_imbalance_digits.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.978452 imbalanced-ensemble-0.2.0/examples/evaluation/
--rw-rw-rw-   0        0        0      152 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/examples/evaluation/README.txt
--rw-rw-rw-   0        0        0     1676 2023-02-13 19:14:31.000000 imbalanced-ensemble-0.2.0/examples/evaluation/plot_classification_report.py
--rw-rw-rw-   0        0        0     3028 2023-02-13 19:14:48.000000 imbalanced-ensemble-0.2.0/examples/evaluation/plot_metrics.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.980598 imbalanced-ensemble-0.2.0/examples/pipeline/
--rw-rw-rw-   0        0        0      164 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/examples/pipeline/README.txt
--rw-rw-rw-   0        0        0     2345 2023-02-13 19:15:14.000000 imbalanced-ensemble-0.2.0/examples/pipeline/plot_pipeline_classification.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:54.982772 imbalanced-ensemble-0.2.0/examples/visualizer/
--rw-rw-rw-   0        0        0      168 2023-02-13 18:52:58.000000 imbalanced-ensemble-0.2.0/examples/visualizer/README.txt
--rw-rw-rw-   0        0        0     4602 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/visualizer/plot_confusion_matrix.py
--rw-rw-rw-   0        0        0     5780 2023-02-13 19:52:57.000000 imbalanced-ensemble-0.2.0/examples/visualizer/plot_performance_curve.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.007794 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/
--rw-rw-rw-   0        0        0    39743 2023-02-13 23:39:53.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    64771 2023-02-13 23:39:54.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 23:39:53.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-13 18:34:33.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      263 2023-02-13 23:39:53.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-13 23:39:53.000000 imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.012693 imbalanced-ensemble-0.2.0/imbens/
--rw-rw-rw-   0        0        0     1370 2023-02-13 21:29:29.000000 imbalanced-ensemble-0.2.0/imbens/__init__.py
--rw-rw-rw-   0        0        0      694 2023-02-13 23:36:42.000000 imbalanced-ensemble-0.2.0/imbens/_version.py
--rw-rw-rw-   0        0        0      373 2023-02-13 21:28:51.000000 imbalanced-ensemble-0.2.0/imbens/base.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.015031 imbalanced-ensemble-0.2.0/imbens/datasets/
--rw-rw-rw-   0        0        0      311 2023-02-13 22:19:01.000000 imbalanced-ensemble-0.2.0/imbens/datasets/__init__.py
--rw-rw-rw-   0        0        0     6637 2023-02-13 22:18:55.000000 imbalanced-ensemble-0.2.0/imbens/datasets/_imbalance.py
--rw-rw-rw-   0        0        0    13016 2023-02-13 22:18:50.000000 imbalanced-ensemble-0.2.0/imbens/datasets/_zenodo.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.019161 imbalanced-ensemble-0.2.0/imbens/datasets/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:32:10.000000 imbalanced-ensemble-0.2.0/imbens/datasets/tests/__init__.py
--rw-rw-rw-   0        0        0     2545 2023-02-13 22:19:10.000000 imbalanced-ensemble-0.2.0/imbens/datasets/tests/test_imbalance.py
--rw-rw-rw-   0        0        0     2846 2023-02-13 22:19:07.000000 imbalanced-ensemble-0.2.0/imbens/datasets/tests/test_zenodo.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.023319 imbalanced-ensemble-0.2.0/imbens/ensemble/
--rw-rw-rw-   0        0        0     1693 2023-02-13 19:53:03.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/__init__.py
--rw-rw-rw-   0        0        0    17511 2023-02-13 21:47:52.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_bagging.py
--rw-rw-rw-   0        0        0    38014 2023-02-13 21:47:42.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_boost.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.026190 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/
--rw-rw-rw-   0        0        0      378 2023-02-13 18:20:06.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/__init__.py
--rw-rw-rw-   0        0        0    15392 2023-02-13 22:18:22.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/adaboost_compatible.py
--rw-rw-rw-   0        0        0    17946 2023-02-13 22:18:18.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/bagging_compatible.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.029362 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:16:01.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/__init__.py
--rw-rw-rw-   0        0        0     3162 2023-02-13 22:18:37.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/test_adabost_compatible.py
--rw-rw-rw-   0        0        0    14414 2023-02-13 22:18:33.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/test_bagging_compatible.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.035239 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/
--rw-rw-rw-   0        0        0      566 2023-02-13 22:14:03.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/__init__.py
--rw-rw-rw-   0        0        0    14015 2023-02-13 22:17:40.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/kmeans_smote_boost.py
--rw-rw-rw-   0        0        0    12163 2023-02-13 22:17:23.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/over_bagging.py
--rw-rw-rw-   0        0        0    11415 2023-02-13 22:17:20.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/over_boost.py
--rw-rw-rw-   0        0        0    12771 2023-02-13 22:17:18.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/smote_bagging.py
--rw-rw-rw-   0        0        0    12546 2023-02-13 22:17:12.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/smote_boost.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.040879 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:15:56.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/__init__.py
--rw-rw-rw-   0        0        0     4851 2023-02-13 22:18:08.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_kmeans_smote_boost.py
--rw-rw-rw-   0        0        0    14446 2023-02-13 22:18:05.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_over_bagging.py
--rw-rw-rw-   0        0        0     3354 2023-02-13 22:17:59.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_over_boost.py
--rw-rw-rw-   0        0        0    14604 2023-02-13 22:17:57.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_smote_bagging.py
--rw-rw-rw-   0        0        0     4777 2023-02-13 22:17:47.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_smote_boost.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.044855 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/
--rw-rw-rw-   0        0        0      374 2023-02-13 22:13:54.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/__init__.py
--rw-rw-rw-   0        0        0    12992 2023-02-13 22:16:44.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/adacost.py
--rw-rw-rw-   0        0        0    15732 2023-02-13 22:16:40.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/adauboost.py
--rw-rw-rw-   0        0        0    13010 2023-02-13 22:16:36.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/asymmetric_boost.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.048572 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:15:53.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/__init__.py
--rw-rw-rw-   0        0        0     6529 2023-02-13 22:17:01.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_adacost.py
--rw-rw-rw-   0        0        0     5771 2023-02-13 22:16:58.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_adauboost.py
--rw-rw-rw-   0        0        0     6778 2023-02-13 22:16:53.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_asymmetric_boost.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.054938 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/
--rw-rw-rw-   0        0        0      690 2023-02-13 22:13:45.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/__init__.py
--rw-rw-rw-   0        0        0    16738 2023-02-13 22:13:20.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/balance_cascade.py
--rw-rw-rw-   0        0        0    31879 2023-02-13 22:13:11.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/balanced_random_forest.py
--rw-rw-rw-   0        0        0    13018 2023-02-13 22:12:57.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/easy_ensemble.py
--rw-rw-rw-   0        0        0    11681 2023-02-13 22:12:52.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/rus_boost.py
--rw-rw-rw-   0        0        0    17272 2023-02-13 22:12:46.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/self_paced_ensemble.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.061481 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:15:50.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/__init__.py
--rw-rw-rw-   0        0        0     9401 2023-02-13 22:14:59.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_balance_cascade.py
--rw-rw-rw-   0        0        0     6393 2023-02-13 22:14:53.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_balanced_random_forest.py
--rw-rw-rw-   0        0        0    16218 2023-02-13 22:14:50.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_easy_ensemble.py
--rw-rw-rw-   0        0        0     3388 2023-02-13 22:14:41.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_rus_boost.py
--rw-rw-rw-   0        0        0     7366 2023-02-13 22:14:38.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_self_paced_ensemble.py
--rw-rw-rw-   0        0        0    14475 2023-02-13 22:14:31.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_under_bagging.py
--rw-rw-rw-   0        0        0    12174 2023-02-13 22:12:39.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/under_bagging.py
--rw-rw-rw-   0        0        0    27925 2023-02-13 21:47:28.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/base.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.063481 imbalanced-ensemble-0.2.0/imbens/ensemble/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:15:45.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/tests/__init__.py
--rw-rw-rw-   0        0        0     3865 2023-02-13 21:48:07.000000 imbalanced-ensemble-0.2.0/imbens/ensemble/tests/test_base_ensemble.py
--rw-rw-rw-   0        0        0      429 2023-02-13 21:28:47.000000 imbalanced-ensemble-0.2.0/imbens/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.066472 imbalanced-ensemble-0.2.0/imbens/metrics/
--rw-rw-rw-   0        0        0      874 2023-02-13 21:46:48.000000 imbalanced-ensemble-0.2.0/imbens/metrics/__init__.py
--rw-rw-rw-   0        0        0    38415 2023-02-13 21:46:44.000000 imbalanced-ensemble-0.2.0/imbens/metrics/_classification.py
--rw-rw-rw-   0        0        0     7954 2023-02-13 21:46:38.000000 imbalanced-ensemble-0.2.0/imbens/metrics/pairwise.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.069461 imbalanced-ensemble-0.2.0/imbens/metrics/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/metrics/tests/__init__.py
--rw-rw-rw-   0        0        0    17511 2023-02-13 21:47:11.000000 imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_classification.py
--rw-rw-rw-   0        0        0     6540 2023-02-13 21:47:05.000000 imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_pairwise.py
--rw-rw-rw-   0        0        0     2322 2023-02-13 21:46:58.000000 imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_score_objects.py
--rw-rw-rw-   0        0        0    20641 2023-02-13 21:28:09.000000 imbalanced-ensemble-0.2.0/imbens/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.071455 imbalanced-ensemble-0.2.0/imbens/sampler/
--rw-rw-rw-   0        0        0     1620 2023-02-13 19:49:38.000000 imbalanced-ensemble-0.2.0/imbens/sampler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.074975 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/
--rw-rw-rw-   0        0        0      557 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/__init__.py
--rw-rw-rw-   0        0        0     8906 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_adasyn.py
--rw-rw-rw-   0        0        0    10747 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_random_over_sampler.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.078662 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/
--rw-rw-rw-   0        0        0      224 2023-02-07 23:44:57.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/__init__.py
--rw-rw-rw-   0        0        0    13034 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/base.py
--rw-rw-rw-   0        0        0    13433 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/cluster.py
--rw-rw-rw-   0        0        0    18005 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/filter.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.083646 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/__init__.py
--rw-rw-rw-   0        0        0     1988 2023-02-13 19:55:18.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_borderline_smote.py
--rw-rw-rw-   0        0        0     4002 2023-02-13 19:50:31.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_kmeans_smote.py
--rw-rw-rw-   0        0        0     5745 2023-02-13 19:50:16.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_smote.py
--rw-rw-rw-   0        0        0     2435 2023-02-13 19:50:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_svm_smote.py
--rw-rw-rw-   0        0        0     2385 2023-02-12 04:30:52.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/base.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.086383 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/__init__.py
--rw-rw-rw-   0        0        0     4515 2023-02-13 19:50:12.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/test_adasyn.py
--rw-rw-rw-   0        0        0     8608 2023-02-13 19:50:09.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/test_random_over_sampler.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.087380 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/
--rw-rw-rw-   0        0        0     1219 2023-02-13 21:39:01.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.089373 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/
--rw-rw-rw-   0        0        0      250 2023-02-13 21:44:57.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/__init__.py
--rw-rw-rw-   0        0        0     8489 2023-02-13 21:44:53.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/_cluster_centroids.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.091406 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/tests/__init__.py
--rw-rw-rw-   0        0        0     4497 2023-02-13 21:45:56.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/tests/test_cluster_centroids.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.101377 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/
--rw-rw-rw-   0        0        0     1222 2023-02-13 20:22:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/__init__.py
--rw-rw-rw-   0        0        0    15176 2023-02-13 21:41:43.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_balance_cascade_under_sampler.py
--rw-rw-rw-   0        0        0     9832 2023-02-13 21:41:37.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_condensed_nearest_neighbour.py
--rw-rw-rw-   0        0        0    20575 2023-02-13 21:41:28.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_edited_nearest_neighbours.py
--rw-rw-rw-   0        0        0     8034 2023-02-13 21:41:23.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_instance_hardness_threshold.py
--rw-rw-rw-   0        0        0    12198 2023-02-13 21:41:15.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_nearmiss.py
--rw-rw-rw-   0        0        0     9026 2023-02-13 21:40:26.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_neighbourhood_cleaning_rule.py
--rw-rw-rw-   0        0        0     8651 2023-02-13 21:40:17.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_one_sided_selection.py
--rw-rw-rw-   0        0        0     7201 2023-02-13 21:40:02.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_random_under_sampler.py
--rw-rw-rw-   0        0        0    18110 2023-02-13 21:39:49.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_self_paced_under_sampler.py
--rw-rw-rw-   0        0        0     6336 2023-02-13 21:39:57.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_tomek_links.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.113867 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/__init__.py
--rw-rw-rw-   0        0        0     9112 2023-02-13 21:44:23.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_allknn.py
--rw-rw-rw-   0        0        0     7904 2023-02-13 21:44:15.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_balance_cascade_under_sampler.py
--rw-rw-rw-   0        0        0     3337 2023-02-13 21:44:09.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_condensed_nearest_neighbour.py
--rw-rw-rw-   0        0        0     4565 2023-02-13 21:44:02.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_edited_nearest_neighbours.py
--rw-rw-rw-   0        0        0     3192 2023-02-13 21:43:57.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_instance_hardness_threshold.py
--rw-rw-rw-   0        0        0     7798 2023-02-13 21:43:49.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_nearmiss.py
--rw-rw-rw-   0        0        0     2815 2023-02-13 21:42:38.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_neighbourhood_cleaning_rule.py
--rw-rw-rw-   0        0        0     3299 2023-02-13 21:42:18.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_one_sided_selection.py
--rw-rw-rw-   0        0        0     3900 2023-02-13 21:42:11.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_random_under_sampler.py
--rw-rw-rw-   0        0        0     9248 2023-02-13 21:42:04.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_repeated_edited_nearest_neighbours.py
--rw-rw-rw-   0        0        0     8114 2023-02-13 21:41:58.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_self_paced_under_sampler.py
--rw-rw-rw-   0        0        0     2148 2023-02-13 21:41:52.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_tomek_links.py
--rw-rw-rw-   0        0        0     3537 2023-02-13 21:38:54.000000 imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/base.py
--rw-rw-rw-   0        0        0    11624 2023-02-13 21:46:25.000000 imbalanced-ensemble-0.2.0/imbens/sampler/base.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.114865 imbalanced-ensemble-0.2.0/imbens/sampler/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/sampler/tests/__init__.py
--rw-rw-rw-   0        0        0     4538 2023-02-13 21:38:44.000000 imbalanced-ensemble-0.2.0/imbens/sampler/tests/test_base_sampler.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.124734 imbalanced-ensemble-0.2.0/imbens/utils/
--rw-rw-rw-   0        0        0      818 2023-02-13 21:35:12.000000 imbalanced-ensemble-0.2.0/imbens/utils/__init__.py
--rw-rw-rw-   0        0        0    22720 2023-02-13 21:35:09.000000 imbalanced-ensemble-0.2.0/imbens/utils/_docstring.py
--rw-rw-rw-   0        0        0     4209 2023-02-13 21:34:56.000000 imbalanced-ensemble-0.2.0/imbens/utils/_evaluate.py
--rw-rw-rw-   0        0        0     3706 2023-02-13 21:34:44.000000 imbalanced-ensemble-0.2.0/imbens/utils/_plot.py
--rw-rw-rw-   0        0        0     2369 2023-02-13 21:34:34.000000 imbalanced-ensemble-0.2.0/imbens/utils/_show_versions.py
--rw-rw-rw-   0        0        0    22920 2023-02-13 21:33:45.000000 imbalanced-ensemble-0.2.0/imbens/utils/_validation.py
--rw-rw-rw-   0        0        0     4189 2023-02-13 21:34:11.000000 imbalanced-ensemble-0.2.0/imbens/utils/_validation_data.py
--rw-rw-rw-   0        0        0    30409 2023-02-13 21:33:56.000000 imbalanced-ensemble-0.2.0/imbens/utils/_validation_param.py
--rw-rw-rw-   0        0        0     1736 2023-02-13 21:32:43.000000 imbalanced-ensemble-0.2.0/imbens/utils/deprecation.py
--rw-rw-rw-   0        0        0    14539 2023-02-13 21:33:14.000000 imbalanced-ensemble-0.2.0/imbens/utils/estimator_checks.py
--rw-rw-rw-   0        0        0     4001 2023-02-13 21:33:31.000000 imbalanced-ensemble-0.2.0/imbens/utils/testing.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.133485 imbalanced-ensemble-0.2.0/imbens/utils/tests/
--rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/__init__.py
--rw-rw-rw-   0        0        0      558 2023-02-13 21:38:04.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_deprecation.py
--rw-rw-rw-   0        0        0     1218 2023-02-13 21:37:58.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_docstring.py
--rw-rw-rw-   0        0        0     4789 2023-02-13 21:37:47.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_estimator_checks.py
--rw-rw-rw-   0        0        0     1087 2023-02-13 21:36:49.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_plot.py
--rw-rw-rw-   0        0        0     1808 2023-02-13 21:36:59.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_show_versions.py
--rw-rw-rw-   0        0        0      853 2023-02-13 21:35:54.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_testing.py
--rw-rw-rw-   0        0        0    14047 2023-02-13 21:35:33.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_validation.py
--rw-rw-rw-   0        0        0     6449 2023-02-13 21:37:18.000000 imbalanced-ensemble-0.2.0/imbens/utils/tests/test_validation_param.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.135479 imbalanced-ensemble-0.2.0/imbens/visualizer/
--rw-rw-rw-   0        0        0      218 2023-02-13 21:32:25.000000 imbalanced-ensemble-0.2.0/imbens/visualizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 23:39:55.136475 imbalanced-ensemble-0.2.0/imbens/visualizer/tests/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:19:52.000000 imbalanced-ensemble-0.2.0/imbens/visualizer/tests/__init__.py
--rw-rw-rw-   0        0        0     5699 2023-02-13 21:32:06.000000 imbalanced-ensemble-0.2.0/imbens/visualizer/tests/test_visualizer.py
--rw-rw-rw-   0        0        0    40684 2023-02-13 21:31:03.000000 imbalanced-ensemble-0.2.0/imbens/visualizer/visualizer.py
--rw-rw-rw-   0        0        0       42 2023-02-13 23:39:55.138647 imbalanced-ensemble-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3268 2023-02-13 20:03:38.000000 imbalanced-ensemble-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.979190 imbalanced-ensemble-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       90 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    39797 2023-07-22 07:41:08.977601 imbalanced-ensemble-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    38139 2023-02-26 06:32:19.000000 imbalanced-ensemble-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.828475 imbalanced-ensemble-0.2.1/docs/
+-rw-rw-rw-   0        0        0    53248 2023-02-10 07:28:25.000000 imbalanced-ensemble-0.2.1/docs/.coverage
+-rw-rw-rw-   0        0        0      658 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0    27378 2023-02-13 23:06:57.000000 imbalanced-ensemble-0.2.1/docs/README_CN.md
+-rwxrwxrwx   0        0        0      799 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0      269 2023-07-22 07:20:09.000000 imbalanced-ensemble-0.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.844272 imbalanced-ensemble-0.2.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.852349 imbalanced-ensemble-0.2.1/docs/source/_static/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.852349 imbalanced-ensemble-0.2.1/docs/source/_static/css/
+-rw-rw-rw-   0        0        0       59 2021-06-13 23:32:47.000000 imbalanced-ensemble-0.2.1/docs/source/_static/css/my_theme.css
+-rw-rw-rw-   0        0        0    31873 2021-06-11 04:52:45.000000 imbalanced-ensemble-0.2.1/docs/source/_static/thumbnail.png
+-rw-rw-rw-   0        0        0    20254 2021-06-10 17:33:31.000000 imbalanced-ensemble-0.2.1/docs/source/_static/training_log_thumbnail.png
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.868376 imbalanced-ensemble-0.2.1/docs/source/_templates/
+-rw-rw-rw-   0        0        0      508 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/_templates/class.rst
+-rw-rw-rw-   0        0        0      435 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/_templates/ensemble_class.rst
+-rw-rw-rw-   0        0        0      248 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/_templates/function.rst
+-rw-rw-rw-   0        0        0      228 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/_templates/numpydoc_docstring.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.740974 imbalanced-ensemble-0.2.1/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.876376 imbalanced-ensemble-0.2.1/docs/source/api/datasets/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.892379 imbalanced-ensemble-0.2.1/docs/source/api/datasets/_autosummary/
+-rw-rw-rw-   0        0        0      279 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/datasets/_autosummary/imbens.datasets.fetch_datasets.rst
+-rw-rw-rw-   0        0        0      315 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/datasets/_autosummary/imbens.datasets.generate_imbalance_data.rst
+-rw-rw-rw-   0        0        0      279 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/datasets/_autosummary/imbens.datasets.make_imbalance.rst
+-rw-rw-rw-   0        0        0      175 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/datasets/api.rst
+-rw-rw-rw-   0        0        0      325 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/datasets/datasets.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.908377 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.972506 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/
+-rw-rw-rw-   0        0        0     1245 2023-07-22 07:02:31.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaCostClassifier.rst
+-rw-rw-rw-   0        0        0     1283 2023-07-22 07:02:31.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaUBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1283 2023-07-22 07:02:31.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AsymBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1031 2023-07-22 07:02:31.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalanceCascadeClassifier.rst
+-rw-rw-rw-   0        0        0     1249 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalancedRandomForestClassifier.rst
+-rw-rw-rw-   0        0        0     1454 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleAdaBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1145 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleBaggingClassifier.rst
+-rw-rw-rw-   0        0        0     1070 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.EasyEnsembleClassifier.rst
+-rw-rw-rw-   0        0        0     1416 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.KmeansSMOTEBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1055 2023-07-22 07:02:32.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBaggingClassifier.rst
+-rw-rw-rw-   0        0        0     1283 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1264 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.RUSBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1070 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBaggingClassifier.rst
+-rw-rw-rw-   0        0        0     1302 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBoostClassifier.rst
+-rw-rw-rw-   0        0        0     1073 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.SelfPacedEnsembleClassifier.rst
+-rw-rw-rw-   0        0        0     1070 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.UnderBaggingClassifier.rst
+-rw-rw-rw-   0        0        0      228 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/api.rst
+-rw-rw-rw-   0        0        0      327 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/compatible.rst
+-rw-rw-rw-   0        0        0      415 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/over-sampling.rst
+-rw-rw-rw-   0        0        0      348 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/reweighting.rst
+-rw-rw-rw-   0        0        0      457 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/ensemble/under-sampling.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:07.988504 imbalanced-ensemble-0.2.1/docs/source/api/metrics/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.020509 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/
+-rw-rw-rw-   0        0        0      675 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.ValueDifferenceMetric.rst
+-rw-rw-rw-   0        0        0      348 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.classification_report_imbalanced.rst
+-rw-rw-rw-   0        0        0      300 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.geometric_mean_score.rst
+-rw-rw-rw-   0        0        0      356 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.macro_averaged_mean_absolute_error.rst
+-rw-rw-rw-   0        0        0      332 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.make_index_balanced_accuracy.rst
+-rw-rw-rw-   0        0        0      288 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.sensitivity_score.rst
+-rw-rw-rw-   0        0        0      344 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.sensitivity_specificity_support.rst
+-rw-rw-rw-   0        0        0      288 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/_autosummary/imbens.metrics.specificity_score.rst
+-rw-rw-rw-   0        0        0      192 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/api.rst
+-rw-rw-rw-   0        0        0      484 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/classification.rst
+-rw-rw-rw-   0        0        0      287 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/metrics/pairwise.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.028506 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.036482 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/_autosummary/
+-rw-rw-rw-   0        0        0     1254 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/_autosummary/imbens.pipeline.Pipeline.rst
+-rw-rw-rw-   0        0        0      275 2023-02-13 18:59:45.000000 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/_autosummary/imbens.pipeline.make_pipeline.rst
+-rw-rw-rw-   0        0        0      175 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/api.rst
+-rw-rw-rw-   0        0        0      364 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/pipeline/pipeline.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.044509 imbalanced-ensemble-0.2.1/docs/source/api/sampler/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.125044 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/
+-rw-rw-rw-   0        0        0      544 2023-07-22 07:02:33.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.ADASYN.rst
+-rw-rw-rw-   0        0        0      544 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.AllKNN.rst
+-rw-rw-rw-   0        0        0      724 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.BalanceCascadeUnderSampler.rst
+-rw-rw-rw-   0        0        0      625 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.BorderlineSMOTE.rst
+-rw-rw-rw-   0        0        0      634 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.ClusterCentroids.rst
+-rw-rw-rw-   0        0        0      715 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.CondensedNearestNeighbour.rst
+-rw-rw-rw-   0        0        0      697 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.EditedNearestNeighbours.rst
+-rw-rw-rw-   0        0        0      715 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.InstanceHardnessThreshold.rst
+-rw-rw-rw-   0        0        0      589 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.KMeansSMOTE.rst
+-rw-rw-rw-   0        0        0      562 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.NearMiss.rst
+-rw-rw-rw-   0        0        0      715 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.NeighbourhoodCleaningRule.rst
+-rw-rw-rw-   0        0        0      643 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.OneSidedSelection.rst
+-rw-rw-rw-   0        0        0      643 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RandomOverSampler.rst
+-rw-rw-rw-   0        0        0      652 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RandomUnderSampler.rst
+-rw-rw-rw-   0        0        0      769 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RepeatedEditedNearestNeighbours.rst
+-rw-rw-rw-   0        0        0      535 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.SMOTE.rst
+-rw-rw-rw-   0        0        0      562 2023-07-22 07:02:34.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.SVMSMOTE.rst
+-rw-rw-rw-   0        0        0      679 2023-07-22 07:02:35.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.SelfPacedUnderSampler.rst
+-rw-rw-rw-   0        0        0      626 2023-07-22 07:02:35.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.TomekLinks.rst
+-rw-rw-rw-   0        0        0      197 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/api.rst
+-rw-rw-rw-   0        0        0      373 2023-02-13 19:30:14.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/over-samplers.rst
+-rw-rw-rw-   0        0        0      599 2023-02-13 19:30:10.000000 imbalanced-ensemble-0.2.1/docs/source/api/sampler/under-samplers.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.141074 imbalanced-ensemble-0.2.1/docs/source/api/utils/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.173204 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/
+-rw-rw-rw-   0        0        0      310 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_balancing_schedule.rst
+-rw-rw-rw-   0        0        0      290 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_eval_datasets.rst
+-rw-rw-rw-   0        0        0      286 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_eval_metrics.rst
+-rw-rw-rw-   0        0        0      302 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_neighbors_object.rst
+-rw-rw-rw-   0        0        0      306 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_sampling_strategy.rst
+-rw-rw-rw-   0        0        0      370 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_target_label_and_n_target_samples.rst
+-rw-rw-rw-   0        0        0      282 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.check_target_type.rst
+-rw-rw-rw-   0        0        0      270 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/_autosummary/imbens.utils.evaluate_print.rst
+-rw-rw-rw-   0        0        0      216 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/api.rst
+-rw-rw-rw-   0        0        0      293 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/evaluation.rst
+-rw-rw-rw-   0        0        0      409 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/validation_ensemble.rst
+-rw-rw-rw-   0        0        0      363 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/utils/validation_sampler.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.181205 imbalanced-ensemble-0.2.1/docs/source/api/visualizer/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.189205 imbalanced-ensemble-0.2.1/docs/source/api/visualizer/_autosummary/
+-rw-rw-rw-   0        0        0      631 2023-02-13 18:59:46.000000 imbalanced-ensemble-0.2.1/docs/source/api/visualizer/_autosummary/imbens.visualizer.ImbalancedEnsembleVisualizer.rst
+-rw-rw-rw-   0        0        0      183 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/visualizer/api.rst
+-rw-rw-rw-   0        0        0      297 2023-02-13 18:58:26.000000 imbalanced-ensemble-0.2.1/docs/source/api/visualizer/visualizer.rst
+-rw-rw-rw-   0        0        0     4043 2023-03-03 21:30:08.000000 imbalanced-ensemble-0.2.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 18:58:25.000000 imbalanced-ensemble-0.2.1/docs/source/get_start.rst
+-rw-rw-rw-   0        0        0     7460 2023-03-03 21:22:57.000000 imbalanced-ensemble-0.2.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0      917 2021-11-25 14:01:00.000000 imbalanced-ensemble-0.2.1/docs/source/install.rst
+-rw-rw-rw-   0        0        0     6552 2023-07-22 07:38:37.000000 imbalanced-ensemble-0.2.1/docs/source/release_history.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.205188 imbalanced-ensemble-0.2.1/docs/source/sphinxext/
+-rw-rw-rw-   0        0        0     6132 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/LICENSE.txt
+-rw-rw-rw-   0        0        0       45 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/MANIFEST.in
+-rw-rw-rw-   0        0        0     1748 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.221202 imbalanced-ensemble-0.2.1/docs/source/sphinxext/__pycache__/
+-rw-rw-rw-   0        0        0     2830 2023-03-03 22:11:40.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/__pycache__/github_link.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6139 2023-03-03 21:25:19.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/__pycache__/sphinx_issues.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3234 2023-03-03 22:11:31.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/github_link.py
+-rw-rw-rw-   0        0        0     8338 2021-05-30 16:51:37.000000 imbalanced-ensemble-0.2.1/docs/source/sphinxext/sphinx_issues.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.221202 imbalanced-ensemble-0.2.1/examples/
+-rw-rw-rw-   0        0        0      240 2023-03-03 20:46:49.000000 imbalanced-ensemble-0.2.1/examples/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.237204 imbalanced-ensemble-0.2.1/examples/basic/
+-rw-rw-rw-   0        0        0      102 2023-03-03 19:57:34.000000 imbalanced-ensemble-0.2.1/examples/basic/README.txt
+-rw-rw-rw-   0        0        0     3808 2023-03-03 21:08:50.000000 imbalanced-ensemble-0.2.1/examples/basic/plot_basic_example.py
+-rw-rw-rw-   0        0        0     2430 2023-03-03 21:08:52.000000 imbalanced-ensemble-0.2.1/examples/basic/plot_basic_visualize.py
+-rw-rw-rw-   0        0        0     3348 2023-03-03 21:08:54.000000 imbalanced-ensemble-0.2.1/examples/basic/plot_training_log.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.269344 imbalanced-ensemble-0.2.1/examples/classification/
+-rw-rw-rw-   0        0        0      166 2023-03-03 19:57:30.000000 imbalanced-ensemble-0.2.1/examples/classification/README.txt
+-rw-rw-rw-   0        0        0     7998 2023-03-03 21:09:01.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_classifier_comparison.py
+-rw-rw-rw-   0        0        0     5791 2023-03-03 21:09:08.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_cost_matrix.py
+-rw-rw-rw-   0        0        0     4641 2023-03-03 21:09:11.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_digits.py
+-rw-rw-rw-   0        0        0     3711 2023-03-03 21:09:13.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_probability.py
+-rw-rw-rw-   0        0        0     8717 2023-03-03 21:09:15.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_resampling_target.py
+-rw-rw-rw-   0        0        0     8718 2023-03-03 21:09:19.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_sampling_schedule.py
+-rw-rw-rw-   0        0        0     7319 2023-03-03 21:09:21.000000 imbalanced-ensemble-0.2.1/examples/classification/plot_torch.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.285346 imbalanced-ensemble-0.2.1/examples/datasets/
+-rw-rw-rw-   0        0        0      119 2023-03-03 19:57:23.000000 imbalanced-ensemble-0.2.1/examples/datasets/README.txt
+-rw-rw-rw-   0        0        0      993 2023-03-03 21:09:24.000000 imbalanced-ensemble-0.2.1/examples/datasets/plot_generate_imbalance.py
+-rw-rw-rw-   0        0        0     2511 2023-03-03 21:09:27.000000 imbalanced-ensemble-0.2.1/examples/datasets/plot_make_imbalance.py
+-rw-rw-rw-   0        0        0     3416 2023-03-03 21:09:25.000000 imbalanced-ensemble-0.2.1/examples/datasets/plot_make_imbalance_digits.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.293348 imbalanced-ensemble-0.2.1/examples/evaluation/
+-rw-rw-rw-   0        0        0      152 2023-03-03 21:09:33.000000 imbalanced-ensemble-0.2.1/examples/evaluation/README.txt
+-rw-rw-rw-   0        0        0     1675 2023-03-03 21:09:29.000000 imbalanced-ensemble-0.2.1/examples/evaluation/plot_classification_report.py
+-rw-rw-rw-   0        0        0     3027 2023-03-03 21:09:31.000000 imbalanced-ensemble-0.2.1/examples/evaluation/plot_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.301347 imbalanced-ensemble-0.2.1/examples/pipeline/
+-rw-rw-rw-   0        0        0      160 2023-03-03 19:57:13.000000 imbalanced-ensemble-0.2.1/examples/pipeline/README.txt
+-rw-rw-rw-   0        0        0     2343 2023-03-03 21:09:35.000000 imbalanced-ensemble-0.2.1/examples/pipeline/plot_pipeline_classification.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.317346 imbalanced-ensemble-0.2.1/examples/visualizer/
+-rw-rw-rw-   0        0        0      132 2023-03-03 19:57:09.000000 imbalanced-ensemble-0.2.1/examples/visualizer/README.txt
+-rw-rw-rw-   0        0        0     4623 2023-03-03 21:09:36.000000 imbalanced-ensemble-0.2.1/examples/visualizer/plot_confusion_matrix.py
+-rw-rw-rw-   0        0        0     5793 2023-03-03 21:09:36.000000 imbalanced-ensemble-0.2.1/examples/visualizer/plot_performance_curve.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.397795 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/
+-rw-rw-rw-   0        0        0    39797 2023-07-22 07:41:05.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14212 2023-07-22 07:41:07.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 07:41:05.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-13 18:34:33.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      276 2023-07-22 07:41:06.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-22 07:41:06.000000 imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.421794 imbalanced-ensemble-0.2.1/imbens/
+-rw-rw-rw-   0        0        0     1370 2023-02-13 21:29:29.000000 imbalanced-ensemble-0.2.1/imbens/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-07-22 07:29:59.000000 imbalanced-ensemble-0.2.1/imbens/_version.py
+-rw-rw-rw-   0        0        0      373 2023-02-13 21:28:51.000000 imbalanced-ensemble-0.2.1/imbens/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.429794 imbalanced-ensemble-0.2.1/imbens/datasets/
+-rw-rw-rw-   0        0        0      311 2023-02-13 22:19:01.000000 imbalanced-ensemble-0.2.1/imbens/datasets/__init__.py
+-rw-rw-rw-   0        0        0     6637 2023-02-13 22:18:55.000000 imbalanced-ensemble-0.2.1/imbens/datasets/_imbalance.py
+-rw-rw-rw-   0        0        0    13016 2023-02-13 22:18:50.000000 imbalanced-ensemble-0.2.1/imbens/datasets/_zenodo.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.437791 imbalanced-ensemble-0.2.1/imbens/datasets/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:32:10.000000 imbalanced-ensemble-0.2.1/imbens/datasets/tests/__init__.py
+-rw-rw-rw-   0        0        0     2545 2023-02-13 22:19:10.000000 imbalanced-ensemble-0.2.1/imbens/datasets/tests/test_imbalance.py
+-rw-rw-rw-   0        0        0     2846 2023-02-13 22:19:07.000000 imbalanced-ensemble-0.2.1/imbens/datasets/tests/test_zenodo.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.453931 imbalanced-ensemble-0.2.1/imbens/ensemble/
+-rw-rw-rw-   0        0        0     1693 2023-02-13 19:53:03.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/__init__.py
+-rw-rw-rw-   0        0        0    17511 2023-02-13 21:47:52.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_bagging.py
+-rw-rw-rw-   0        0        0    38014 2023-02-13 21:47:42.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_boost.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.469979 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/
+-rw-rw-rw-   0        0        0      378 2023-02-13 18:20:06.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/__init__.py
+-rw-rw-rw-   0        0        0    15392 2023-02-13 22:18:22.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/adaboost_compatible.py
+-rw-rw-rw-   0        0        0    17946 2023-02-13 22:18:18.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/bagging_compatible.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.477962 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:16:01.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/__init__.py
+-rw-rw-rw-   0        0        0     3162 2023-02-13 22:18:37.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/test_adabost_compatible.py
+-rw-rw-rw-   0        0        0    14414 2023-02-13 22:18:33.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/test_bagging_compatible.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.502101 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/
+-rw-rw-rw-   0        0        0      566 2023-02-13 22:14:03.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/__init__.py
+-rw-rw-rw-   0        0        0    14015 2023-02-13 22:17:40.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/kmeans_smote_boost.py
+-rw-rw-rw-   0        0        0    12163 2023-02-13 22:17:23.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/over_bagging.py
+-rw-rw-rw-   0        0        0    11415 2023-02-13 22:17:20.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/over_boost.py
+-rw-rw-rw-   0        0        0    12771 2023-02-13 22:17:18.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/smote_bagging.py
+-rw-rw-rw-   0        0        0    12546 2023-02-13 22:17:12.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/smote_boost.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.526104 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:15:56.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/__init__.py
+-rw-rw-rw-   0        0        0     4851 2023-02-13 22:18:08.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_kmeans_smote_boost.py
+-rw-rw-rw-   0        0        0    14446 2023-02-13 22:18:05.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_over_bagging.py
+-rw-rw-rw-   0        0        0     3354 2023-02-13 22:17:59.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_over_boost.py
+-rw-rw-rw-   0        0        0    14604 2023-02-13 22:17:57.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_smote_bagging.py
+-rw-rw-rw-   0        0        0     4777 2023-02-13 22:17:47.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_smote_boost.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.542104 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/
+-rw-rw-rw-   0        0        0      374 2023-02-13 22:13:54.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/__init__.py
+-rw-rw-rw-   0        0        0    12992 2023-02-13 22:16:44.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/adacost.py
+-rw-rw-rw-   0        0        0    15732 2023-02-13 22:16:40.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/adauboost.py
+-rw-rw-rw-   0        0        0    13010 2023-02-13 22:16:36.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/asymmetric_boost.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.566238 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:15:53.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/__init__.py
+-rw-rw-rw-   0        0        0     6529 2023-02-13 22:17:01.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_adacost.py
+-rw-rw-rw-   0        0        0     5771 2023-02-13 22:16:58.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_adauboost.py
+-rw-rw-rw-   0        0        0     6778 2023-02-13 22:16:53.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_asymmetric_boost.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.590240 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/
+-rw-rw-rw-   0        0        0      690 2023-02-13 22:13:45.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/__init__.py
+-rw-rw-rw-   0        0        0    16738 2023-02-13 22:13:20.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/balance_cascade.py
+-rw-rw-rw-   0        0        0    31877 2023-07-22 05:34:11.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/balanced_random_forest.py
+-rw-rw-rw-   0        0        0    13018 2023-02-13 22:12:57.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/easy_ensemble.py
+-rw-rw-rw-   0        0        0    11681 2023-02-13 22:12:52.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/rus_boost.py
+-rw-rw-rw-   0        0        0    17272 2023-02-13 22:12:46.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/self_paced_ensemble.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.622236 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:15:50.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/__init__.py
+-rw-rw-rw-   0        0        0     9401 2023-02-13 22:14:59.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_balance_cascade.py
+-rw-rw-rw-   0        0        0     6393 2023-02-13 22:14:53.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_balanced_random_forest.py
+-rw-rw-rw-   0        0        0    16218 2023-02-13 22:14:50.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_easy_ensemble.py
+-rw-rw-rw-   0        0        0     3388 2023-02-13 22:14:41.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_rus_boost.py
+-rw-rw-rw-   0        0        0     7366 2023-02-13 22:14:38.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_self_paced_ensemble.py
+-rw-rw-rw-   0        0        0    14475 2023-02-13 22:14:31.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_under_bagging.py
+-rw-rw-rw-   0        0        0    12174 2023-02-13 22:12:39.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/under_bagging.py
+-rw-rw-rw-   0        0        0    27925 2023-02-13 21:47:28.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.630240 imbalanced-ensemble-0.2.1/imbens/ensemble/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:15:45.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/tests/__init__.py
+-rw-rw-rw-   0        0        0     3865 2023-02-13 21:48:07.000000 imbalanced-ensemble-0.2.1/imbens/ensemble/tests/test_base_ensemble.py
+-rw-rw-rw-   0        0        0      429 2023-02-13 21:28:47.000000 imbalanced-ensemble-0.2.1/imbens/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.638238 imbalanced-ensemble-0.2.1/imbens/metrics/
+-rw-rw-rw-   0        0        0      874 2023-02-13 21:46:48.000000 imbalanced-ensemble-0.2.1/imbens/metrics/__init__.py
+-rw-rw-rw-   0        0        0    38415 2023-02-13 21:46:44.000000 imbalanced-ensemble-0.2.1/imbens/metrics/_classification.py
+-rw-rw-rw-   0        0        0     7954 2023-02-13 21:46:38.000000 imbalanced-ensemble-0.2.1/imbens/metrics/pairwise.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.654359 imbalanced-ensemble-0.2.1/imbens/metrics/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/metrics/tests/__init__.py
+-rw-rw-rw-   0        0        0    17511 2023-02-13 21:47:11.000000 imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_classification.py
+-rw-rw-rw-   0        0        0     6540 2023-02-13 21:47:05.000000 imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_pairwise.py
+-rw-rw-rw-   0        0        0     2322 2023-02-13 21:46:58.000000 imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_score_objects.py
+-rw-rw-rw-   0        0        0    20632 2023-07-22 01:08:30.000000 imbalanced-ensemble-0.2.1/imbens/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.668780 imbalanced-ensemble-0.2.1/imbens/sampler/
+-rw-rw-rw-   0        0        0     1620 2023-02-13 19:49:38.000000 imbalanced-ensemble-0.2.1/imbens/sampler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.678892 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/
+-rw-rw-rw-   0        0        0      557 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/__init__.py
+-rw-rw-rw-   0        0        0     8906 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_adasyn.py
+-rw-rw-rw-   0        0        0    10747 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_random_over_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.694892 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/
+-rw-rw-rw-   0        0        0      224 2023-02-07 23:44:57.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/__init__.py
+-rw-rw-rw-   0        0        0    13034 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/base.py
+-rw-rw-rw-   0        0        0    13433 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/cluster.py
+-rw-rw-rw-   0        0        0    18005 2023-02-13 20:22:34.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/filter.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.718893 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/__init__.py
+-rw-rw-rw-   0        0        0     1988 2023-02-13 19:55:18.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_borderline_smote.py
+-rw-rw-rw-   0        0        0     4002 2023-02-13 19:50:31.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_kmeans_smote.py
+-rw-rw-rw-   0        0        0     5745 2023-02-13 19:50:16.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_smote.py
+-rw-rw-rw-   0        0        0     2435 2023-02-13 19:50:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_svm_smote.py
+-rw-rw-rw-   0        0        0     2385 2023-02-12 04:30:52.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.734892 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/__init__.py
+-rw-rw-rw-   0        0        0     4515 2023-02-13 19:50:12.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/test_adasyn.py
+-rw-rw-rw-   0        0        0     8608 2023-02-13 19:50:09.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/test_random_over_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.742890 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/
+-rw-rw-rw-   0        0        0     1219 2023-02-13 21:39:01.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.752456 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/
+-rw-rw-rw-   0        0        0      250 2023-02-13 21:44:57.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/__init__.py
+-rw-rw-rw-   0        0        0     8489 2023-02-13 21:44:53.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/_cluster_centroids.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.758993 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/tests/__init__.py
+-rw-rw-rw-   0        0        0     4497 2023-02-13 21:45:56.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/tests/test_cluster_centroids.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.807023 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/
+-rw-rw-rw-   0        0        0     1222 2023-02-13 20:22:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/__init__.py
+-rw-rw-rw-   0        0        0    15176 2023-02-13 21:41:43.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_balance_cascade_under_sampler.py
+-rw-rw-rw-   0        0        0     9832 2023-02-13 21:41:37.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_condensed_nearest_neighbour.py
+-rw-rw-rw-   0        0        0    20575 2023-02-13 21:41:28.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_edited_nearest_neighbours.py
+-rw-rw-rw-   0        0        0     8034 2023-02-13 21:41:23.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_instance_hardness_threshold.py
+-rw-rw-rw-   0        0        0    12198 2023-02-13 21:41:15.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_nearmiss.py
+-rw-rw-rw-   0        0        0     9026 2023-02-13 21:40:26.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_neighbourhood_cleaning_rule.py
+-rw-rw-rw-   0        0        0     8651 2023-02-13 21:40:17.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_one_sided_selection.py
+-rw-rw-rw-   0        0        0     7201 2023-02-13 21:40:02.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_random_under_sampler.py
+-rw-rw-rw-   0        0        0    18110 2023-02-13 21:39:49.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_self_paced_under_sampler.py
+-rw-rw-rw-   0        0        0     6336 2023-02-13 21:39:57.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_tomek_links.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.863155 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/__init__.py
+-rw-rw-rw-   0        0        0     9112 2023-02-13 21:44:23.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_allknn.py
+-rw-rw-rw-   0        0        0     7904 2023-02-13 21:44:15.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_balance_cascade_under_sampler.py
+-rw-rw-rw-   0        0        0     3337 2023-02-13 21:44:09.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_condensed_nearest_neighbour.py
+-rw-rw-rw-   0        0        0     4565 2023-02-13 21:44:02.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_edited_nearest_neighbours.py
+-rw-rw-rw-   0        0        0     3192 2023-02-13 21:43:57.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_instance_hardness_threshold.py
+-rw-rw-rw-   0        0        0     7798 2023-02-13 21:43:49.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_nearmiss.py
+-rw-rw-rw-   0        0        0     2815 2023-02-13 21:42:38.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_neighbourhood_cleaning_rule.py
+-rw-rw-rw-   0        0        0     3299 2023-02-13 21:42:18.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_one_sided_selection.py
+-rw-rw-rw-   0        0        0     3900 2023-02-13 21:42:11.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_random_under_sampler.py
+-rw-rw-rw-   0        0        0     9248 2023-02-13 21:42:04.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_repeated_edited_nearest_neighbours.py
+-rw-rw-rw-   0        0        0     8114 2023-02-13 21:41:58.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_self_paced_under_sampler.py
+-rw-rw-rw-   0        0        0     2148 2023-02-13 21:41:52.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_tomek_links.py
+-rw-rw-rw-   0        0        0     3537 2023-02-13 21:38:54.000000 imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/base.py
+-rw-rw-rw-   0        0        0    11624 2023-02-13 21:46:25.000000 imbalanced-ensemble-0.2.1/imbens/sampler/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.863155 imbalanced-ensemble-0.2.1/imbens/sampler/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/sampler/tests/__init__.py
+-rw-rw-rw-   0        0        0     4538 2023-02-13 21:38:44.000000 imbalanced-ensemble-0.2.1/imbens/sampler/tests/test_base_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.913102 imbalanced-ensemble-0.2.1/imbens/utils/
+-rw-rw-rw-   0        0        0      818 2023-02-13 21:35:12.000000 imbalanced-ensemble-0.2.1/imbens/utils/__init__.py
+-rw-rw-rw-   0        0        0    22720 2023-02-13 21:35:09.000000 imbalanced-ensemble-0.2.1/imbens/utils/_docstring.py
+-rw-rw-rw-   0        0        0     4209 2023-02-13 21:34:56.000000 imbalanced-ensemble-0.2.1/imbens/utils/_evaluate.py
+-rw-rw-rw-   0        0        0     3706 2023-03-03 05:36:54.000000 imbalanced-ensemble-0.2.1/imbens/utils/_plot.py
+-rw-rw-rw-   0        0        0     2269 2023-07-22 06:18:24.000000 imbalanced-ensemble-0.2.1/imbens/utils/_show_versions.py
+-rw-rw-rw-   0        0        0    22920 2023-02-13 21:33:45.000000 imbalanced-ensemble-0.2.1/imbens/utils/_validation.py
+-rw-rw-rw-   0        0        0     4189 2023-02-13 21:34:11.000000 imbalanced-ensemble-0.2.1/imbens/utils/_validation_data.py
+-rw-rw-rw-   0        0        0    30409 2023-02-13 21:33:56.000000 imbalanced-ensemble-0.2.1/imbens/utils/_validation_param.py
+-rw-rw-rw-   0        0        0     1736 2023-02-13 21:32:43.000000 imbalanced-ensemble-0.2.1/imbens/utils/deprecation.py
+-rw-rw-rw-   0        0        0    14537 2023-07-22 05:46:20.000000 imbalanced-ensemble-0.2.1/imbens/utils/estimator_checks.py
+-rw-rw-rw-   0        0        0     4001 2023-02-13 21:33:31.000000 imbalanced-ensemble-0.2.1/imbens/utils/testing.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.954182 imbalanced-ensemble-0.2.1/imbens/utils/tests/
+-rw-rw-rw-   0        0        0        0 2021-05-27 19:38:14.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-02-13 21:38:04.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_deprecation.py
+-rw-rw-rw-   0        0        0     1218 2023-02-13 21:37:58.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_docstring.py
+-rw-rw-rw-   0        0        0     4789 2023-07-22 05:46:24.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_estimator_checks.py
+-rw-rw-rw-   0        0        0     1087 2023-02-13 21:36:49.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1826 2023-07-22 01:47:30.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_show_versions.py
+-rw-rw-rw-   0        0        0      853 2023-02-13 21:35:54.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_testing.py
+-rw-rw-rw-   0        0        0    14047 2023-02-13 21:35:33.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_validation.py
+-rw-rw-rw-   0        0        0     6449 2023-02-13 21:37:18.000000 imbalanced-ensemble-0.2.1/imbens/utils/tests/test_validation_param.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.960217 imbalanced-ensemble-0.2.1/imbens/visualizer/
+-rw-rw-rw-   0        0        0      218 2023-02-13 21:32:25.000000 imbalanced-ensemble-0.2.1/imbens/visualizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:41:08.970940 imbalanced-ensemble-0.2.1/imbens/visualizer/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:19:52.000000 imbalanced-ensemble-0.2.1/imbens/visualizer/tests/__init__.py
+-rw-rw-rw-   0        0        0     5699 2023-02-13 21:32:06.000000 imbalanced-ensemble-0.2.1/imbens/visualizer/tests/test_visualizer.py
+-rw-rw-rw-   0        0        0    40684 2023-02-13 21:31:03.000000 imbalanced-ensemble-0.2.1/imbens/visualizer/visualizer.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 07:41:08.979190 imbalanced-ensemble-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3307 2023-07-22 07:32:23.000000 imbalanced-ensemble-0.2.1/setup.py
```

### Comparing `imbalanced-ensemble-0.2.0/LICENSE` & `imbalanced-ensemble-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/PKG-INFO` & `imbalanced-ensemble-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: imbalanced-ensemble
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolbox for ensemble learning on class-imbalanced dataset.
 Home-page: https://github.com/ZhiningLiu1998/imbalanced-ensemble
 Author: Zhining Liu
 Author-email: zhining.liu@outlook.com
 Maintainer: Zhining Liu
 Maintainer-email: zhining.liu@outlook.com
 License: MIT
 Project-URL: Documentation, https://imbalanced-ensemble.readthedocs.io/
 Project-URL: Source, https://github.com/ZhiningLiu1998/imbalanced-ensemble
 Project-URL: Tracker, https://github.com/ZhiningLiu1998/imbalanced-ensemble/issues
 Project-URL: Changelog, https://imbalanced-ensemble.readthedocs.io/en/latest/release_history.html
 Project-URL: Download, https://pypi.org/project/imbalanced-ensemble/#files
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -110,15 +111,15 @@
   Links: 
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#5-min-quick-start-with-imbens">Getting Started</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/">API Reference</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#">Examples</a> |
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#related-projects">Related Projects</a> |
   <a href="https://zhuanlan.zhihu.com/p/376572330">知乎/Zhihu</a>  
   Paper:
-  <a href="https://arxiv.org/abs/2111.12776">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
+  <a href="https://arxiv.org/pdf/2111.12776.pdf">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
   <br>**
 
 ***IMBENS*** (imported as `imbens`) is a Python library for quick implementation, modification, evaluation, and visualization of **ensemble [learning from class-imbalanced data](https://github.com/ZhiningLiu1998/awesome-imbalanced-learning)**. 
 Currently, IMBENS includes more than **[15 ensemble imbalanced learning algorithms](#list-of-implemented-methods)**, from the classical *SMOTEBoost* (2003), *RUSBoost* (2010) to recent [*Self-paced Ensemble*](https://github.com/ZhiningLiu1998/self-paced-ensemble) (2020), from *resampling* to *cost-sensitive learning*.
 
 ***IMBENS*** is developed on top of [imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn) (imblearn) and follows the API design of [scikit-learn](https://github.com/scikit-learn/scikit-learn). Compared to imblearn, IMBENS provides more powerful ensemble learning algorithms with ***multi-class learning*** support and many other **advanced features**:
 
@@ -133,34 +134,40 @@
 - &#x1F34E; Unified, easy-to-use APIs, detailed [documentation](https://imbalanced-ensemble.readthedocs.io/) and [examples](https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#).
 - &#x1F34E; Capable for out-of-the-box ***multi-class*** imbalanced (long-tailed) learning.
 - &#x1F34E; Optimized performance with parallelization when possible using [joblib](https://github.com/joblib/joblib).
 - &#x1F34E; Powerful, customizable, interactive training logging and visualizer.
 - &#x1F34E; Full compatibility with other popular packages like [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https://imbalanced-learn.org/stable/).
 
 **Ensemble Imbalanced Learning with 4 Lines of Code:**
+
 ```python
 # Train an SPE classifier
 from imbens.ensemble import SelfPacedEnsembleClassifier
 clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train)
 
 # Predict with an SPE classifier
 y_pred = clf.predict(X_test)
 ```
+
+**Contributing to IMBENS**
+
+Please refer to the [contributing guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/CONTRIBUTING.md).
+
 **Citing IMBENS**
 
 The [IMBENS paper](https://arxiv.org/pdf/2111.12776.pdf) is available on arxiv.
 If you use IMBENS in a scientific publication, we would appreciate citations to the following paper:
 
 ```bib
-@article{liu2021imbens,
+@article{liu2023imbens,
   title={IMBENS: Ensemble Class-imbalanced Learning in Python},
-  author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi},
+  author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
   journal={arXiv preprint arXiv:2111.12776},
-  year={2021}
+  year={2023}
 }
 ```
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
@@ -524,7 +531,9 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: imbalanced-ensemble Version: 0.2.0 Summary: Toolbox
+Metadata-Version: 2.1 Name: imbalanced-ensemble Version: 0.2.1 Summary: Toolbox
 for ensemble learning on class-imbalanced dataset. Home-page: https://
 github.com/ZhiningLiu1998/imbalanced-ensemble Author: Zhining Liu Author-email:
 zhining.liu@outlook.com Maintainer: Zhining Liu Maintainer-email:
 zhining.liu@outlook.com License: MIT Project-URL: Documentation, https://
 imbalanced-ensemble.readthedocs.io/ Project-URL: Source, https://github.com/
 ZhiningLiu1998/imbalanced-ensemble Project-URL: Tracker, https://github.com/
 ZhiningLiu1998/imbalanced-ensemble/issues Project-URL: Changelog, https://
 imbalanced-ensemble.readthedocs.io/en/latest/release_history.html Project-URL:
-Download, https://pypi.org/project/imbalanced-ensemble/#files Classifier:
-Intended Audience :: Science/Research Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Download, https://pypi.org/project/imbalanced-ensemble/#files Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: C Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
 Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -61,47 +61,47 @@
 - &#x1F34E; Powerful, customizable, interactive training logging and
 visualizer. - &#x1F34E; Full compatibility with other popular packages like
 [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https:/
 /imbalanced-learn.org/stable/). **Ensemble Imbalanced Learning with 4 Lines of
 Code:** ```python # Train an SPE classifier from imbens.ensemble import
 SelfPacedEnsembleClassifier clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train) # Predict with an SPE classifier y_pred = clf.predict
-(X_test) ``` **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
+(X_test) ``` **Contributing to IMBENS** Please refer to the [contributing
+guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/
+CONTRIBUTING.md). **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
 2111.12776.pdf) is available on arxiv. If you use IMBENS in a scientific
 publication, we would appreciate citations to the following paper: ```bib
-@article{liu2021imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
-Python}, author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang
-and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and
-Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi}, journal={arXiv
-preprint arXiv:2111.12776}, year={2021} } ``` ## Table of Contents - [Table of
-Contents](#table-of-contents) - [Installation](#installation) - [Highlights]
-(#highlights) - [List of implemented methods](#list-of-implemented-methods) -
-[5-min Quick Start with IMBENS](#5-min-quick-start-with-imbens) - [A minimal
-working example](#a-minimal-working-example) - [Visualize ensemble classifiers]
-(#visualize-ensemble-classifiers) - [Customizing training log](#customizing-
-training-log) - [About imbalanced learning](#about-imbalanced-learning) -
-[Acknowledgements](#acknowledgements) - [References](#references) - [Related
-Projects](#related-projects) - [Contributors â¨](#contributors-) ##
-Installation It is recommended to use **pip** for installation. Please make
-sure the **latest version** is installed to avoid potential problems: ```shell
-$ pip install imbalanced-ensemble # normal install $ pip install --upgrade
-imbalanced-ensemble # update if needed ``` Or you can install imbalanced-
-ensemble by clone this repository: ```shell $ git clone https://github.com/
-ZhiningLiu1998/imbalanced-ensemble.git $ cd imbalanced-ensemble $ pip install .
-``` imbalanced-ensemble requires following dependencies: - [Python](https://
-www.python.org/) (>=3.6) - [numpy](https://numpy.org/) (>=1.16.0) - [pandas]
-(https://pandas.pydata.org/) (>=1.1.3) - [scipy](https://www.scipy.org/)
-(>=1.9.1) - [joblib](https://pypi.org/project/joblib/) (>=0.11) - [scikit-
-learn](https://scikit-learn.org/stable/) (>=1.2.0) - [matplotlib](https://
-matplotlib.org/) (>=3.3.2) - [seaborn](https://seaborn.pydata.org/) (>=0.11.0)
-- [tqdm](https://tqdm.github.io/) (>=4.50.2) ## Highlights - &#x1F34E;
-***Unified, easy-to-use API design.*** All ensemble learning methods
-implemented in IMBENS share a unified API design. Similar to sklearn, all
-methods have functions (e.g., `fit()`, `predict()`, `predict_proba()`) that
-allow users to deploy them with only a few lines of code. - &#x1F34E;
+@article{liu2023imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
+Python}, author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
+journal={arXiv preprint arXiv:2111.12776}, year={2023} } ``` ## Table of
+Contents - [Table of Contents](#table-of-contents) - [Installation]
+(#installation) - [Highlights](#highlights) - [List of implemented methods]
+(#list-of-implemented-methods) - [5-min Quick Start with IMBENS](#5-min-quick-
+start-with-imbens) - [A minimal working example](#a-minimal-working-example) -
+[Visualize ensemble classifiers](#visualize-ensemble-classifiers) -
+[Customizing training log](#customizing-training-log) - [About imbalanced
+learning](#about-imbalanced-learning) - [Acknowledgements](#acknowledgements) -
+[References](#references) - [Related Projects](#related-projects) -
+[Contributors â¨](#contributors-) ## Installation It is recommended to use
+**pip** for installation. Please make sure the **latest version** is installed
+to avoid potential problems: ```shell $ pip install imbalanced-ensemble #
+normal install $ pip install --upgrade imbalanced-ensemble # update if needed
+``` Or you can install imbalanced-ensemble by clone this repository: ```shell $
+git clone https://github.com/ZhiningLiu1998/imbalanced-ensemble.git $ cd
+imbalanced-ensemble $ pip install . ``` imbalanced-ensemble requires following
+dependencies: - [Python](https://www.python.org/) (>=3.6) - [numpy](https://
+numpy.org/) (>=1.16.0) - [pandas](https://pandas.pydata.org/) (>=1.1.3) -
+[scipy](https://www.scipy.org/) (>=1.9.1) - [joblib](https://pypi.org/project/
+joblib/) (>=0.11) - [scikit-learn](https://scikit-learn.org/stable/) (>=1.2.0)
+- [matplotlib](https://matplotlib.org/) (>=3.3.2) - [seaborn](https://
+seaborn.pydata.org/) (>=0.11.0) - [tqdm](https://tqdm.github.io/) (>=4.50.2) ##
+Highlights - &#x1F34E; ***Unified, easy-to-use API design.*** All ensemble
+learning methods implemented in IMBENS share a unified API design. Similar to
+sklearn, all methods have functions (e.g., `fit()`, `predict()`, `predict_proba
+()`) that allow users to deploy them with only a few lines of code. - &#x1F34E;
 ***Extended functionalities, wider application scenarios.*** *All methods in
 IMBENS are ready for **multi-class imbalanced classification**.* We extend
 binary ensemble imbalanced learning methods to get them to work under the
 multi-class scenario. Additionally, for supported methods, we provide more
 training options like class-wise resampling control, balancing scheduler during
 the ensemble training process, etc. - &#x1F34E; ***Detailed training log, quick
 intuitive visualization.*** We provide additional parameters (e.g.,
```

### Comparing `imbalanced-ensemble-0.2.0/README.md` & `imbalanced-ensemble-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   Links: 
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#5-min-quick-start-with-imbens">Getting Started</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/">API Reference</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#">Examples</a> |
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#related-projects">Related Projects</a> |
   <a href="https://zhuanlan.zhihu.com/p/376572330">知乎/Zhihu</a>  
   Paper:
-  <a href="https://arxiv.org/abs/2111.12776">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
+  <a href="https://arxiv.org/pdf/2111.12776.pdf">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
   <br>**
 
 ***IMBENS*** (imported as `imbens`) is a Python library for quick implementation, modification, evaluation, and visualization of **ensemble [learning from class-imbalanced data](https://github.com/ZhiningLiu1998/awesome-imbalanced-learning)**. 
 Currently, IMBENS includes more than **[15 ensemble imbalanced learning algorithms](#list-of-implemented-methods)**, from the classical *SMOTEBoost* (2003), *RUSBoost* (2010) to recent [*Self-paced Ensemble*](https://github.com/ZhiningLiu1998/self-paced-ensemble) (2020), from *resampling* to *cost-sensitive learning*.
 
 ***IMBENS*** is developed on top of [imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn) (imblearn) and follows the API design of [scikit-learn](https://github.com/scikit-learn/scikit-learn). Compared to imblearn, IMBENS provides more powerful ensemble learning algorithms with ***multi-class learning*** support and many other **advanced features**:
 
@@ -95,34 +95,40 @@
 - &#x1F34E; Unified, easy-to-use APIs, detailed [documentation](https://imbalanced-ensemble.readthedocs.io/) and [examples](https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#).
 - &#x1F34E; Capable for out-of-the-box ***multi-class*** imbalanced (long-tailed) learning.
 - &#x1F34E; Optimized performance with parallelization when possible using [joblib](https://github.com/joblib/joblib).
 - &#x1F34E; Powerful, customizable, interactive training logging and visualizer.
 - &#x1F34E; Full compatibility with other popular packages like [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https://imbalanced-learn.org/stable/).
 
 **Ensemble Imbalanced Learning with 4 Lines of Code:**
+
 ```python
 # Train an SPE classifier
 from imbens.ensemble import SelfPacedEnsembleClassifier
 clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train)
 
 # Predict with an SPE classifier
 y_pred = clf.predict(X_test)
 ```
+
+**Contributing to IMBENS**
+
+Please refer to the [contributing guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/CONTRIBUTING.md).
+
 **Citing IMBENS**
 
 The [IMBENS paper](https://arxiv.org/pdf/2111.12776.pdf) is available on arxiv.
 If you use IMBENS in a scientific publication, we would appreciate citations to the following paper:
 
 ```bib
-@article{liu2021imbens,
+@article{liu2023imbens,
   title={IMBENS: Ensemble Class-imbalanced Learning in Python},
-  author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi},
+  author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
   journal={arXiv preprint arXiv:2111.12776},
-  year={2021}
+  year={2023}
 }
 ```
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
```

#### html2text {}

```diff
@@ -40,47 +40,47 @@
 - &#x1F34E; Powerful, customizable, interactive training logging and
 visualizer. - &#x1F34E; Full compatibility with other popular packages like
 [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https:/
 /imbalanced-learn.org/stable/). **Ensemble Imbalanced Learning with 4 Lines of
 Code:** ```python # Train an SPE classifier from imbens.ensemble import
 SelfPacedEnsembleClassifier clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train) # Predict with an SPE classifier y_pred = clf.predict
-(X_test) ``` **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
+(X_test) ``` **Contributing to IMBENS** Please refer to the [contributing
+guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/
+CONTRIBUTING.md). **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
 2111.12776.pdf) is available on arxiv. If you use IMBENS in a scientific
 publication, we would appreciate citations to the following paper: ```bib
-@article{liu2021imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
-Python}, author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang
-and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and
-Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi}, journal={arXiv
-preprint arXiv:2111.12776}, year={2021} } ``` ## Table of Contents - [Table of
-Contents](#table-of-contents) - [Installation](#installation) - [Highlights]
-(#highlights) - [List of implemented methods](#list-of-implemented-methods) -
-[5-min Quick Start with IMBENS](#5-min-quick-start-with-imbens) - [A minimal
-working example](#a-minimal-working-example) - [Visualize ensemble classifiers]
-(#visualize-ensemble-classifiers) - [Customizing training log](#customizing-
-training-log) - [About imbalanced learning](#about-imbalanced-learning) -
-[Acknowledgements](#acknowledgements) - [References](#references) - [Related
-Projects](#related-projects) - [Contributors â¨](#contributors-) ##
-Installation It is recommended to use **pip** for installation. Please make
-sure the **latest version** is installed to avoid potential problems: ```shell
-$ pip install imbalanced-ensemble # normal install $ pip install --upgrade
-imbalanced-ensemble # update if needed ``` Or you can install imbalanced-
-ensemble by clone this repository: ```shell $ git clone https://github.com/
-ZhiningLiu1998/imbalanced-ensemble.git $ cd imbalanced-ensemble $ pip install .
-``` imbalanced-ensemble requires following dependencies: - [Python](https://
-www.python.org/) (>=3.6) - [numpy](https://numpy.org/) (>=1.16.0) - [pandas]
-(https://pandas.pydata.org/) (>=1.1.3) - [scipy](https://www.scipy.org/)
-(>=1.9.1) - [joblib](https://pypi.org/project/joblib/) (>=0.11) - [scikit-
-learn](https://scikit-learn.org/stable/) (>=1.2.0) - [matplotlib](https://
-matplotlib.org/) (>=3.3.2) - [seaborn](https://seaborn.pydata.org/) (>=0.11.0)
-- [tqdm](https://tqdm.github.io/) (>=4.50.2) ## Highlights - &#x1F34E;
-***Unified, easy-to-use API design.*** All ensemble learning methods
-implemented in IMBENS share a unified API design. Similar to sklearn, all
-methods have functions (e.g., `fit()`, `predict()`, `predict_proba()`) that
-allow users to deploy them with only a few lines of code. - &#x1F34E;
+@article{liu2023imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
+Python}, author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
+journal={arXiv preprint arXiv:2111.12776}, year={2023} } ``` ## Table of
+Contents - [Table of Contents](#table-of-contents) - [Installation]
+(#installation) - [Highlights](#highlights) - [List of implemented methods]
+(#list-of-implemented-methods) - [5-min Quick Start with IMBENS](#5-min-quick-
+start-with-imbens) - [A minimal working example](#a-minimal-working-example) -
+[Visualize ensemble classifiers](#visualize-ensemble-classifiers) -
+[Customizing training log](#customizing-training-log) - [About imbalanced
+learning](#about-imbalanced-learning) - [Acknowledgements](#acknowledgements) -
+[References](#references) - [Related Projects](#related-projects) -
+[Contributors â¨](#contributors-) ## Installation It is recommended to use
+**pip** for installation. Please make sure the **latest version** is installed
+to avoid potential problems: ```shell $ pip install imbalanced-ensemble #
+normal install $ pip install --upgrade imbalanced-ensemble # update if needed
+``` Or you can install imbalanced-ensemble by clone this repository: ```shell $
+git clone https://github.com/ZhiningLiu1998/imbalanced-ensemble.git $ cd
+imbalanced-ensemble $ pip install . ``` imbalanced-ensemble requires following
+dependencies: - [Python](https://www.python.org/) (>=3.6) - [numpy](https://
+numpy.org/) (>=1.16.0) - [pandas](https://pandas.pydata.org/) (>=1.1.3) -
+[scipy](https://www.scipy.org/) (>=1.9.1) - [joblib](https://pypi.org/project/
+joblib/) (>=0.11) - [scikit-learn](https://scikit-learn.org/stable/) (>=1.2.0)
+- [matplotlib](https://matplotlib.org/) (>=3.3.2) - [seaborn](https://
+seaborn.pydata.org/) (>=0.11.0) - [tqdm](https://tqdm.github.io/) (>=4.50.2) ##
+Highlights - &#x1F34E; ***Unified, easy-to-use API design.*** All ensemble
+learning methods implemented in IMBENS share a unified API design. Similar to
+sklearn, all methods have functions (e.g., `fit()`, `predict()`, `predict_proba
+()`) that allow users to deploy them with only a few lines of code. - &#x1F34E;
 ***Extended functionalities, wider application scenarios.*** *All methods in
 IMBENS are ready for **multi-class imbalanced classification**.* We extend
 binary ensemble imbalanced learning methods to get them to work under the
 multi-class scenario. Additionally, for supported methods, we provide more
 training options like class-wise resampling control, balancing scheduler during
 the ensemble training process, etc. - &#x1F34E; ***Detailed training log, quick
 intuitive visualization.*** We provide additional parameters (e.g.,
```

### Comparing `imbalanced-ensemble-0.2.0/docs/.coverage` & `imbalanced-ensemble-0.2.1/docs/.coverage`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/Makefile` & `imbalanced-ensemble-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/README_CN.md` & `imbalanced-ensemble-0.2.1/docs/README_CN.md`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/make.bat` & `imbalanced-ensemble-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/_static/thumbnail.png` & `imbalanced-ensemble-0.2.1/docs/source/_static/thumbnail.png`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/_static/training_log_thumbnail.png` & `imbalanced-ensemble-0.2.1/docs/source/_static/training_log_thumbnail.png`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaCostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaUBoostClassifier.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-﻿AdaCostClassifier
-===============================================
+﻿AdaUBoostClassifier
+=================================================
 
 .. currentmodule:: imbens.ensemble
 
-.. autoclass:: AdaCostClassifier
+.. autoclass:: AdaUBoostClassifier
 
    
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       
       
-        ~AdaCostClassifier.decision_function
+        ~AdaUBoostClassifier.decision_function
       
       
-        ~AdaCostClassifier.fit
+        ~AdaUBoostClassifier.fit
       
       
-        ~AdaCostClassifier.get_params
+        ~AdaUBoostClassifier.get_metadata_routing
       
       
-        ~AdaCostClassifier.predict
+        ~AdaUBoostClassifier.get_params
       
       
-        ~AdaCostClassifier.predict_log_proba
+        ~AdaUBoostClassifier.predict
       
       
-        ~AdaCostClassifier.predict_proba
+        ~AdaUBoostClassifier.predict_log_proba
       
       
-        ~AdaCostClassifier.score
+        ~AdaUBoostClassifier.predict_proba
       
       
-        ~AdaCostClassifier.set_params
+        ~AdaUBoostClassifier.score
       
       
-        ~AdaCostClassifier.staged_decision_function
+        ~AdaUBoostClassifier.set_fit_request
       
       
-        ~AdaCostClassifier.staged_predict
+        ~AdaUBoostClassifier.set_params
       
       
-        ~AdaCostClassifier.staged_predict_proba
+        ~AdaUBoostClassifier.set_score_request
       
       
-        ~AdaCostClassifier.staged_score
+        ~AdaUBoostClassifier.staged_decision_function
+      
+      
+        ~AdaUBoostClassifier.staged_predict
+      
+      
+        ~AdaUBoostClassifier.staged_predict_proba
+      
+      
+        ~AdaUBoostClassifier.staged_score
       
    
    
 
-.. include:: ../../../back_references/imbens.ensemble.AdaCostClassifier.examples
+.. include:: ../../../back_references/imbens.ensemble.AdaUBoostClassifier.examples
 
 .. raw:: html
 
     <div style='clear:both'></div>
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaUBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AsymBoostClassifier.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-﻿AdaUBoostClassifier
+﻿AsymBoostClassifier
 =================================================
 
 .. currentmodule:: imbens.ensemble
 
-.. autoclass:: AdaUBoostClassifier
+.. autoclass:: AsymBoostClassifier
 
    
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       
       
-        ~AdaUBoostClassifier.decision_function
+        ~AsymBoostClassifier.decision_function
       
       
-        ~AdaUBoostClassifier.fit
+        ~AsymBoostClassifier.fit
       
       
-        ~AdaUBoostClassifier.get_params
+        ~AsymBoostClassifier.get_metadata_routing
       
       
-        ~AdaUBoostClassifier.predict
+        ~AsymBoostClassifier.get_params
       
       
-        ~AdaUBoostClassifier.predict_log_proba
+        ~AsymBoostClassifier.predict
       
       
-        ~AdaUBoostClassifier.predict_proba
+        ~AsymBoostClassifier.predict_log_proba
       
       
-        ~AdaUBoostClassifier.score
+        ~AsymBoostClassifier.predict_proba
       
       
-        ~AdaUBoostClassifier.set_params
+        ~AsymBoostClassifier.score
       
       
-        ~AdaUBoostClassifier.staged_decision_function
+        ~AsymBoostClassifier.set_fit_request
       
       
-        ~AdaUBoostClassifier.staged_predict
+        ~AsymBoostClassifier.set_params
       
       
-        ~AdaUBoostClassifier.staged_predict_proba
+        ~AsymBoostClassifier.set_score_request
       
       
-        ~AdaUBoostClassifier.staged_score
+        ~AsymBoostClassifier.staged_decision_function
+      
+      
+        ~AsymBoostClassifier.staged_predict
+      
+      
+        ~AsymBoostClassifier.staged_predict_proba
+      
+      
+        ~AsymBoostClassifier.staged_score
       
    
    
 
-.. include:: ../../../back_references/imbens.ensemble.AdaUBoostClassifier.examples
+.. include:: ../../../back_references/imbens.ensemble.AsymBoostClassifier.examples
 
 .. raw:: html
 
     <div style='clear:both'></div>
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.AsymBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.AdaCostClassifier.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-﻿AsymBoostClassifier
-=================================================
+﻿AdaCostClassifier
+===============================================
 
 .. currentmodule:: imbens.ensemble
 
-.. autoclass:: AsymBoostClassifier
+.. autoclass:: AdaCostClassifier
 
    
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       
       
-        ~AsymBoostClassifier.decision_function
+        ~AdaCostClassifier.decision_function
       
       
-        ~AsymBoostClassifier.fit
+        ~AdaCostClassifier.fit
       
       
-        ~AsymBoostClassifier.get_params
+        ~AdaCostClassifier.get_metadata_routing
       
       
-        ~AsymBoostClassifier.predict
+        ~AdaCostClassifier.get_params
       
       
-        ~AsymBoostClassifier.predict_log_proba
+        ~AdaCostClassifier.predict
       
       
-        ~AsymBoostClassifier.predict_proba
+        ~AdaCostClassifier.predict_log_proba
       
       
-        ~AsymBoostClassifier.score
+        ~AdaCostClassifier.predict_proba
       
       
-        ~AsymBoostClassifier.set_params
+        ~AdaCostClassifier.score
       
       
-        ~AsymBoostClassifier.staged_decision_function
+        ~AdaCostClassifier.set_fit_request
       
       
-        ~AsymBoostClassifier.staged_predict
+        ~AdaCostClassifier.set_params
       
       
-        ~AsymBoostClassifier.staged_predict_proba
+        ~AdaCostClassifier.set_score_request
       
       
-        ~AsymBoostClassifier.staged_score
+        ~AdaCostClassifier.staged_decision_function
+      
+      
+        ~AdaCostClassifier.staged_predict
+      
+      
+        ~AdaCostClassifier.staged_predict_proba
+      
+      
+        ~AdaCostClassifier.staged_score
       
    
    
 
-.. include:: ../../../back_references/imbens.ensemble.AsymBoostClassifier.examples
+.. include:: ../../../back_references/imbens.ensemble.AdaCostClassifier.examples
 
 .. raw:: html
 
     <div style='clear:both'></div>
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalancedRandomForestClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.BalancedRandomForestClassifier.rst`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,17 @@
       
         ~BalancedRandomForestClassifier.decision_path
       
       
         ~BalancedRandomForestClassifier.fit
       
       
+        ~BalancedRandomForestClassifier.get_metadata_routing
+      
+      
         ~BalancedRandomForestClassifier.get_params
       
       
         ~BalancedRandomForestClassifier.predict
       
       
         ~BalancedRandomForestClassifier.predict_log_proba
@@ -34,16 +37,22 @@
       
         ~BalancedRandomForestClassifier.predict_proba
       
       
         ~BalancedRandomForestClassifier.score
       
       
+        ~BalancedRandomForestClassifier.set_fit_request
+      
+      
         ~BalancedRandomForestClassifier.set_params
       
+      
+        ~BalancedRandomForestClassifier.set_score_request
+      
    
    
 
 .. include:: ../../../back_references/imbens.ensemble.BalancedRandomForestClassifier.examples
 
 .. raw:: html
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleAdaBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleAdaBoostClassifier.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~CompatibleAdaBoostClassifier.decision_function
       
       
         ~CompatibleAdaBoostClassifier.fit
       
       
+        ~CompatibleAdaBoostClassifier.get_metadata_routing
+      
+      
         ~CompatibleAdaBoostClassifier.get_params
       
       
         ~CompatibleAdaBoostClassifier.predict
       
       
         ~CompatibleAdaBoostClassifier.predict_log_proba
@@ -31,17 +34,23 @@
       
         ~CompatibleAdaBoostClassifier.predict_proba
       
       
         ~CompatibleAdaBoostClassifier.score
       
       
+        ~CompatibleAdaBoostClassifier.set_fit_request
+      
+      
         ~CompatibleAdaBoostClassifier.set_params
       
       
+        ~CompatibleAdaBoostClassifier.set_score_request
+      
+      
         ~CompatibleAdaBoostClassifier.staged_decision_function
       
       
         ~CompatibleAdaBoostClassifier.staged_predict
       
       
         ~CompatibleAdaBoostClassifier.staged_predict_proba
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleBaggingClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.CompatibleBaggingClassifier.rst`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~CompatibleBaggingClassifier.decision_function
       
       
         ~CompatibleBaggingClassifier.fit
       
       
+        ~CompatibleBaggingClassifier.get_metadata_routing
+      
+      
         ~CompatibleBaggingClassifier.get_params
       
       
         ~CompatibleBaggingClassifier.predict
       
       
         ~CompatibleBaggingClassifier.predict_log_proba
@@ -31,16 +34,22 @@
       
         ~CompatibleBaggingClassifier.predict_proba
       
       
         ~CompatibleBaggingClassifier.score
       
       
+        ~CompatibleBaggingClassifier.set_fit_request
+      
+      
         ~CompatibleBaggingClassifier.set_params
       
+      
+        ~CompatibleBaggingClassifier.set_score_request
+      
    
    
 
 .. include:: ../../../back_references/imbens.ensemble.CompatibleBaggingClassifier.examples
 
 .. raw:: html
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.KmeansSMOTEBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.KmeansSMOTEBoostClassifier.rst`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~KmeansSMOTEBoostClassifier.decision_function
       
       
         ~KmeansSMOTEBoostClassifier.fit
       
       
+        ~KmeansSMOTEBoostClassifier.get_metadata_routing
+      
+      
         ~KmeansSMOTEBoostClassifier.get_params
       
       
         ~KmeansSMOTEBoostClassifier.predict
       
       
         ~KmeansSMOTEBoostClassifier.predict_log_proba
@@ -31,17 +34,23 @@
       
         ~KmeansSMOTEBoostClassifier.predict_proba
       
       
         ~KmeansSMOTEBoostClassifier.score
       
       
+        ~KmeansSMOTEBoostClassifier.set_fit_request
+      
+      
         ~KmeansSMOTEBoostClassifier.set_params
       
       
+        ~KmeansSMOTEBoostClassifier.set_score_request
+      
+      
         ~KmeansSMOTEBoostClassifier.staged_decision_function
       
       
         ~KmeansSMOTEBoostClassifier.staged_predict
       
       
         ~KmeansSMOTEBoostClassifier.staged_predict_proba
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBaggingClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.OverBaggingClassifier.rst`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~OverBaggingClassifier.decision_function
       
       
         ~OverBaggingClassifier.fit
       
       
+        ~OverBaggingClassifier.get_metadata_routing
+      
+      
         ~OverBaggingClassifier.get_params
       
       
         ~OverBaggingClassifier.predict
       
       
         ~OverBaggingClassifier.predict_log_proba
@@ -31,16 +34,22 @@
       
         ~OverBaggingClassifier.predict_proba
       
       
         ~OverBaggingClassifier.score
       
       
+        ~OverBaggingClassifier.set_fit_request
+      
+      
         ~OverBaggingClassifier.set_params
       
+      
+        ~OverBaggingClassifier.set_score_request
+      
    
    
 
 .. include:: ../../../back_references/imbens.ensemble.OverBaggingClassifier.examples
 
 .. raw:: html
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.RUSBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.RUSBoostClassifier.rst`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~RUSBoostClassifier.decision_function
       
       
         ~RUSBoostClassifier.fit
       
       
+        ~RUSBoostClassifier.get_metadata_routing
+      
+      
         ~RUSBoostClassifier.get_params
       
       
         ~RUSBoostClassifier.predict
       
       
         ~RUSBoostClassifier.predict_log_proba
@@ -31,17 +34,23 @@
       
         ~RUSBoostClassifier.predict_proba
       
       
         ~RUSBoostClassifier.score
       
       
+        ~RUSBoostClassifier.set_fit_request
+      
+      
         ~RUSBoostClassifier.set_params
       
       
+        ~RUSBoostClassifier.set_score_request
+      
+      
         ~RUSBoostClassifier.staged_decision_function
       
       
         ~RUSBoostClassifier.staged_predict
       
       
         ~RUSBoostClassifier.staged_predict_proba
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBaggingClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBaggingClassifier.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~SMOTEBaggingClassifier.decision_function
       
       
         ~SMOTEBaggingClassifier.fit
       
       
+        ~SMOTEBaggingClassifier.get_metadata_routing
+      
+      
         ~SMOTEBaggingClassifier.get_params
       
       
         ~SMOTEBaggingClassifier.predict
       
       
         ~SMOTEBaggingClassifier.predict_log_proba
@@ -31,16 +34,22 @@
       
         ~SMOTEBaggingClassifier.predict_proba
       
       
         ~SMOTEBaggingClassifier.score
       
       
+        ~SMOTEBaggingClassifier.set_fit_request
+      
+      
         ~SMOTEBaggingClassifier.set_params
       
+      
+        ~SMOTEBaggingClassifier.set_score_request
+      
    
    
 
 .. include:: ../../../back_references/imbens.ensemble.SMOTEBaggingClassifier.examples
 
 .. raw:: html
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBoostClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.SMOTEBoostClassifier.rst`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~SMOTEBoostClassifier.decision_function
       
       
         ~SMOTEBoostClassifier.fit
       
       
+        ~SMOTEBoostClassifier.get_metadata_routing
+      
+      
         ~SMOTEBoostClassifier.get_params
       
       
         ~SMOTEBoostClassifier.predict
       
       
         ~SMOTEBoostClassifier.predict_log_proba
@@ -31,17 +34,23 @@
       
         ~SMOTEBoostClassifier.predict_proba
       
       
         ~SMOTEBoostClassifier.score
       
       
+        ~SMOTEBoostClassifier.set_fit_request
+      
+      
         ~SMOTEBoostClassifier.set_params
       
       
+        ~SMOTEBoostClassifier.set_score_request
+      
+      
         ~SMOTEBoostClassifier.staged_decision_function
       
       
         ~SMOTEBoostClassifier.staged_predict
       
       
         ~SMOTEBoostClassifier.staged_predict_proba
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/ensemble/_autosummary/imbens.ensemble.UnderBaggingClassifier.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/ensemble/_autosummary/imbens.ensemble.UnderBaggingClassifier.rst`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~UnderBaggingClassifier.decision_function
       
       
         ~UnderBaggingClassifier.fit
       
       
+        ~UnderBaggingClassifier.get_metadata_routing
+      
+      
         ~UnderBaggingClassifier.get_params
       
       
         ~UnderBaggingClassifier.predict
       
       
         ~UnderBaggingClassifier.predict_log_proba
@@ -31,16 +34,22 @@
       
         ~UnderBaggingClassifier.predict_proba
       
       
         ~UnderBaggingClassifier.score
       
       
+        ~UnderBaggingClassifier.set_fit_request
+      
+      
         ~UnderBaggingClassifier.set_params
       
+      
+        ~UnderBaggingClassifier.set_score_request
+      
    
    
 
 .. include:: ../../../back_references/imbens.ensemble.UnderBaggingClassifier.examples
 
 .. raw:: html
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/pipeline/_autosummary/imbens.pipeline.Pipeline.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/pipeline/_autosummary/imbens.pipeline.Pipeline.rst`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
       
         ~Pipeline.fit_transform
       
       
         ~Pipeline.get_feature_names_out
       
       
+        ~Pipeline.get_metadata_routing
+      
+      
         ~Pipeline.get_params
       
       
         ~Pipeline.inverse_transform
       
       
         ~Pipeline.predict
@@ -49,20 +52,26 @@
       
         ~Pipeline.score
       
       
         ~Pipeline.score_samples
       
       
+        ~Pipeline.set_fit_request
+      
+      
         ~Pipeline.set_output
       
       
         ~Pipeline.set_params
       
       
+        ~Pipeline.set_score_request
+      
+      
         ~Pipeline.transform
       
    
    
 
 .. include:: ../../../back_references/imbens.pipeline.Pipeline.examples
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.BalanceCascadeUnderSampler.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.BalanceCascadeUnderSampler.rst`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~BalanceCascadeUnderSampler.fit
       
       
         ~BalanceCascadeUnderSampler.fit_resample
       
       
+        ~BalanceCascadeUnderSampler.get_metadata_routing
+      
+      
         ~BalanceCascadeUnderSampler.get_params
       
       
         ~BalanceCascadeUnderSampler.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.BorderlineSMOTE.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.BorderlineSMOTE.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~BorderlineSMOTE.fit
       
       
         ~BorderlineSMOTE.fit_resample
       
       
+        ~BorderlineSMOTE.get_metadata_routing
+      
+      
         ~BorderlineSMOTE.get_params
       
       
         ~BorderlineSMOTE.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.ClusterCentroids.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.ClusterCentroids.rst`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~ClusterCentroids.fit
       
       
         ~ClusterCentroids.fit_resample
       
       
+        ~ClusterCentroids.get_metadata_routing
+      
+      
         ~ClusterCentroids.get_params
       
       
         ~ClusterCentroids.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.CondensedNearestNeighbour.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.CondensedNearestNeighbour.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~CondensedNearestNeighbour.fit
       
       
         ~CondensedNearestNeighbour.fit_resample
       
       
+        ~CondensedNearestNeighbour.get_metadata_routing
+      
+      
         ~CondensedNearestNeighbour.get_params
       
       
         ~CondensedNearestNeighbour.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.EditedNearestNeighbours.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.EditedNearestNeighbours.rst`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~EditedNearestNeighbours.fit
       
       
         ~EditedNearestNeighbours.fit_resample
       
       
+        ~EditedNearestNeighbours.get_metadata_routing
+      
+      
         ~EditedNearestNeighbours.get_params
       
       
         ~EditedNearestNeighbours.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.InstanceHardnessThreshold.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.InstanceHardnessThreshold.rst`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~InstanceHardnessThreshold.fit
       
       
         ~InstanceHardnessThreshold.fit_resample
       
       
+        ~InstanceHardnessThreshold.get_metadata_routing
+      
+      
         ~InstanceHardnessThreshold.get_params
       
       
         ~InstanceHardnessThreshold.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.KMeansSMOTE.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.KMeansSMOTE.rst`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~KMeansSMOTE.fit
       
       
         ~KMeansSMOTE.fit_resample
       
       
+        ~KMeansSMOTE.get_metadata_routing
+      
+      
         ~KMeansSMOTE.get_params
       
       
         ~KMeansSMOTE.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.NeighbourhoodCleaningRule.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.NeighbourhoodCleaningRule.rst`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~NeighbourhoodCleaningRule.fit
       
       
         ~NeighbourhoodCleaningRule.fit_resample
       
       
+        ~NeighbourhoodCleaningRule.get_metadata_routing
+      
+      
         ~NeighbourhoodCleaningRule.get_params
       
       
         ~NeighbourhoodCleaningRule.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.OneSidedSelection.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.OneSidedSelection.rst`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~OneSidedSelection.fit
       
       
         ~OneSidedSelection.fit_resample
       
       
+        ~OneSidedSelection.get_metadata_routing
+      
+      
         ~OneSidedSelection.get_params
       
       
         ~OneSidedSelection.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RandomOverSampler.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RandomOverSampler.rst`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~RandomOverSampler.fit
       
       
         ~RandomOverSampler.fit_resample
       
       
+        ~RandomOverSampler.get_metadata_routing
+      
+      
         ~RandomOverSampler.get_params
       
       
         ~RandomOverSampler.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RandomUnderSampler.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RandomUnderSampler.rst`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~RandomUnderSampler.fit
       
       
         ~RandomUnderSampler.fit_resample
       
       
+        ~RandomUnderSampler.get_metadata_routing
+      
+      
         ~RandomUnderSampler.get_params
       
       
         ~RandomUnderSampler.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.RepeatedEditedNearestNeighbours.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.RepeatedEditedNearestNeighbours.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~RepeatedEditedNearestNeighbours.fit
       
       
         ~RepeatedEditedNearestNeighbours.fit_resample
       
       
+        ~RepeatedEditedNearestNeighbours.get_metadata_routing
+      
+      
         ~RepeatedEditedNearestNeighbours.get_params
       
       
         ~RepeatedEditedNearestNeighbours.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.SelfPacedUnderSampler.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.SelfPacedUnderSampler.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~SelfPacedUnderSampler.fit
       
       
         ~SelfPacedUnderSampler.fit_resample
       
       
+        ~SelfPacedUnderSampler.get_metadata_routing
+      
+      
         ~SelfPacedUnderSampler.get_params
       
       
         ~SelfPacedUnderSampler.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/_autosummary/imbens.sampler.TomekLinks.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/_autosummary/imbens.sampler.TomekLinks.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       
         ~TomekLinks.fit
       
       
         ~TomekLinks.fit_resample
       
       
+        ~TomekLinks.get_metadata_routing
+      
+      
         ~TomekLinks.get_params
       
       
         ~TomekLinks.is_tomek
       
       
         ~TomekLinks.set_params
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/sampler/under-samplers.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/sampler/under-samplers.rst`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/api/visualizer/_autosummary/imbens.visualizer.ImbalancedEnsembleVisualizer.rst` & `imbalanced-ensemble-0.2.1/docs/source/api/visualizer/_autosummary/imbens.visualizer.ImbalancedEnsembleVisualizer.rst`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_example.py` & `imbalanced-ensemble-0.2.1/examples/basic/plot_basic_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,29 @@
 
 # %% [markdown]
 # Prepare & visualize the data
 # ----------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # Generate and split a synthetic dataset
-X, y = make_classification(n_classes=3, n_samples=2000, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, random_state=RANDOM_STATE)
-X_train, X_valid, y_train, y_valid = train_test_split(X, y, 
-    test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+X, y = make_classification(
+    n_classes=3,
+    n_samples=2000,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    random_state=RANDOM_STATE,
+)
+X_train, X_valid, y_train, y_valid = train_test_split(
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # Visualize the training dataset
 fig = plot_2Dprojection_and_cardinality(X_train, y_train, figsize=(8, 4))
 plt.show()
 
 # Print class distribution
 print('Training dataset distribution    %s' % sort_dict_by_key(Counter(y_train)))
@@ -67,58 +77,59 @@
 
 # Make predictions
 y_pred_proba = clf.predict_proba(X_valid)
 y_pred = clf.predict(X_valid)
 
 # Evaluate
 balanced_acc_score = sklearn.metrics.balanced_accuracy_score(y_valid, y_pred)
-print (f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
-print ('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
+print(f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
+print('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
 
 
 # %% [markdown]
 # Set the ensemble size
 # ---------------------
 # (parameter ``n_estimators``: int)
 
 from imbens.ensemble import SelfPacedEnsembleClassifier as SPE
 from sklearn.metrics import balanced_accuracy_score
 
 clf = SPE(
-    n_estimators=5, # Set ensemble size to 5
+    n_estimators=5,  # Set ensemble size to 5
     random_state=RANDOM_STATE,
 ).fit(X_train, y_train)
 
 # Evaluate
 balanced_acc_score = balanced_accuracy_score(y_valid, clf.predict(X_valid))
-print (f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
-print ('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
+print(f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
+print('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
 
 
 # %% [markdown]
 # Use different base estimator
 # ----------------------------
 # (parameter ``estimator``: estimator object)
 
 from sklearn.svm import SVC
 
 clf = SPE(
     n_estimators=5,
-    estimator=SVC(probability=True), # Use SVM as the base estimator
+    estimator=SVC(probability=True),  # Use SVM as the base estimator
     random_state=RANDOM_STATE,
 ).fit(X_train, y_train)
 
 # Evaluate
 balanced_acc_score = balanced_accuracy_score(y_valid, clf.predict(X_valid))
-print (f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
-print ('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
+print(f'SPE: ensemble of {clf.n_estimators} {clf.estimator_}')
+print('Validation Balanced Accuracy: {:.3f}'.format(balanced_acc_score))
 
 
 # %% [markdown]
 # Enable training log
 # -------------------
 # (``fit()`` parameter ``train_verbose``: bool, int or dict)
 
 clf = SPE(random_state=RANDOM_STATE).fit(
-    X_train, y_train, 
-    train_verbose=True, # Enable training log
-)
+    X_train,
+    y_train,
+    train_verbose=True,  # Enable training log
+)
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_basic_visualize.py` & `imbalanced-ensemble-0.2.1/examples/basic/plot_basic_visualize.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,46 +34,56 @@
 
 # %% [markdown]
 # Prepare data
 # ------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 
 # %% [markdown]
 # Train an ensemble classifier
 # ----------------------------
 # Take ``SelfPacedEnsembleClassifier`` as example
 
 # Initialize and train an SPE classifier
-clf = imbens.ensemble.SelfPacedEnsembleClassifier(
-    random_state=RANDOM_STATE
-).fit(X_train, y_train)
+clf = imbens.ensemble.SelfPacedEnsembleClassifier(random_state=RANDOM_STATE).fit(
+    X_train, y_train
+)
 
 # Store the fitted SelfPacedEnsembleClassifier
 fitted_ensembles = {'SPE': clf}
 
 
 # %% [markdown]
 # Fit an ImbalancedEnsembleVisualizer
 # -----------------------------------------------------
 
 # Initialize visualizer
 visualizer = imbens.visualizer.ImbalancedEnsembleVisualizer(
-    eval_datasets = {
-        'training' : (X_train, y_train),
-        'validation' : (X_valid, y_valid),
+    eval_datasets={
+        'training': (X_train, y_train),
+        'validation': (X_valid, y_valid),
     },
 )
 
 # Fit visualizer
 visualizer.fit(fitted_ensembles)
 
 
@@ -85,10 +95,10 @@
 fig, axes = visualizer.performance_lineplot()
 
 # %% [markdown]
 # Plot confusion matrix
 # ---------------------
 
 fig, axes = visualizer.confusion_matrix_heatmap(
-    on_datasets=['validation'], # only on validation set
+    on_datasets=['validation'],  # only on validation set
     sup_title=False,
-)
+)
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/basic/plot_training_log.py` & `imbalanced-ensemble-0.2.1/examples/basic/plot_training_log.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,90 +32,117 @@
 
 # %% [markdown]
 # Prepare data
 # ----------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # %% [markdown]
 # Customize training log
 # ---------------------------------------------------------------------------
 # Take ``SelfPacedEnsembleClassifier`` as example, training log is controlled by 3 parameters of the ``fit()`` method:
-# 
+#
 #   - ``eval_datasets``: Dataset(s) used for evaluation during the ensemble training.
 #   - ``eval_metrics``: Metric(s) used for evaluation during the ensemble training.
 #   - ``train_verbose``: Controls the granularity and content of the training log.
 
 clf = imbens.ensemble.SelfPacedEnsembleClassifier(random_state=RANDOM_STATE)
 
 # %% [markdown]
 # Set training log format
 # -----------------------
 # (``fit()`` parameter: ``train_verbose``: bool, int or dict)
 
 # %% [markdown]
-# **Enable auto training log** 
+# **Enable auto training log**
 
-clf.fit(X_train, y_train,
-        train_verbose=True,
-       )
+clf.fit(
+    X_train,
+    y_train,
+    train_verbose=True,
+)
 
 
 # %% [markdown]
 # **Customize training log granularity**
 
-clf.fit(X_train, y_train,
-        train_verbose={
-            'granularity': 10,
-        })
+clf.fit(
+    X_train,
+    y_train,
+    train_verbose={
+        'granularity': 10,
+    },
+)
 
 
 # %% [markdown]
 # **Customize training log content column**
 
-clf.fit(X_train, y_train,
-        train_verbose={
-            'granularity': 10,
-            'print_distribution': False,
-            'print_metrics': True,
-        })
+clf.fit(
+    X_train,
+    y_train,
+    train_verbose={
+        'granularity': 10,
+        'print_distribution': False,
+        'print_metrics': True,
+    },
+)
 
 
 # %% [markdown]
 # Add additional evaluation dataset(s)
 # ------------------------------------
 # (``fit()`` parameter: ``eval_datasets``: dict)
 
-clf.fit(X_train, y_train,
-        eval_datasets={
-            'valid': (X_valid, y_valid), # add validation data
-        },
-        train_verbose={
-            'granularity': 10,
-        })
+clf.fit(
+    X_train,
+    y_train,
+    eval_datasets={
+        'valid': (X_valid, y_valid),  # add validation data
+    },
+    train_verbose={
+        'granularity': 10,
+    },
+)
 
 
 # %% [markdown]
 # Specify evaluation metric(s)
 # ----------------------------
 # (``fit()`` parameter: ``eval_metrics``: dict)
 
-clf.fit(X_train, y_train,
-        eval_datasets={
-            'valid': (X_valid, y_valid),
-        },
-        eval_metrics={
-            'weighted_f1': (sklearn.metrics.f1_score, {'average':'weighted'}), # use weighted_f1
-        },
-        train_verbose={
-            'granularity': 10,
-        })
+clf.fit(
+    X_train,
+    y_train,
+    eval_datasets={
+        'valid': (X_valid, y_valid),
+    },
+    eval_metrics={
+        'weighted_f1': (
+            sklearn.metrics.f1_score,
+            {'average': 'weighted'},
+        ),  # use weighted_f1
+    },
+    train_verbose={
+        'granularity': 10,
+    },
+)
 
 # %%
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_classifier_comparison.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,74 +61,96 @@
 # -----------
 # **Make 3 imbalanced toy classification tasks.**
 
 distribution = {0: 100, 1: 50}
 
 # dataset 1
 X, y = make_moons(200, noise=0.2, random_state=RANDOM_STATE)
-dataset1 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
+dataset1 = make_imbalance(
+    X, y, sampling_strategy=distribution, random_state=RANDOM_STATE
+)
 # dataset 2
 X, y = make_circles(200, noise=0.2, factor=0.5, random_state=RANDOM_STATE)
-dataset2 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
+dataset2 = make_imbalance(
+    X, y, sampling_strategy=distribution, random_state=RANDOM_STATE
+)
 # dataset 3
-X, y = make_classification(200, n_features=2, n_redundant=0, n_informative=2,
-                           random_state=1, n_clusters_per_class=1)
+X, y = make_classification(
+    200,
+    n_features=2,
+    n_redundant=0,
+    n_informative=2,
+    random_state=1,
+    n_clusters_per_class=1,
+)
 X += 2 * np.random.RandomState(RANDOM_STATE).uniform(size=X.shape)
-dataset3 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
+dataset3 = make_imbalance(
+    X, y, sampling_strategy=distribution, random_state=RANDOM_STATE
+)
 
 datasets = [dataset1, dataset2, dataset3]
 
 
 # %% [markdown]
 # **Load all ensemble classifiers**
 
 from imbens.utils.testing import all_estimators
 
 init_kwargs = {'n_estimators': 5, 'random_state': RANDOM_STATE}
-all_ensembles_clf = {name: ensemble(**init_kwargs) for (name, ensemble) in all_estimators('ensemble')}
+all_ensembles_clf = {
+    name: ensemble(**init_kwargs) for (name, ensemble) in all_estimators('ensemble')
+}
 
-print ('{:<30s} | Class \n{:=<120s}'.format('Method', ''))
+print('{:<30s} | Class \n{:=<120s}'.format('Method', ''))
 for (name, ensemble) in all_estimators('ensemble'):
-    print ('{:<30s} | {}'.format(name, ensemble))
+    print('{:<30s} | {}'.format(name, ensemble))
 
 
 # %% [markdown]
 # **Function for classifier comparison**
 
+
 def plot_classifier_comparison(classifiers, names, datasets, figsize):
 
-    h = .02  # step size in the mesh
+    h = 0.02  # step size in the mesh
 
     figure = plt.figure(figsize=figsize)
     i = 1
     # iterate over datasets
     for ds_cnt, ds in enumerate(datasets):
         # preprocess dataset, split into training and test part
         X, y = ds
         X = StandardScaler().fit_transform(X)
-        X_train, X_test, y_train, y_test = \
-            train_test_split(X, y, test_size=.4, random_state=42)
-
-        x_min, x_max = X[:, 0].min() - .5, X[:, 0].max() + .5
-        y_min, y_max = X[:, 1].min() - .5, X[:, 1].max() + .5
-        xx, yy = np.meshgrid(np.arange(x_min, x_max, h),
-                             np.arange(y_min, y_max, h))
+        X_train, X_test, y_train, y_test = train_test_split(
+            X, y, test_size=0.4, random_state=42
+        )
+
+        x_min, x_max = X[:, 0].min() - 0.5, X[:, 0].max() + 0.5
+        y_min, y_max = X[:, 1].min() - 0.5, X[:, 1].max() + 0.5
+        xx, yy = np.meshgrid(np.arange(x_min, x_max, h), np.arange(y_min, y_max, h))
 
         # just plot the dataset first
         cm = plt.cm.RdBu
         cm_bright = ListedColormap(['#FF0000', '#0000FF'])
         ax = plt.subplot(len(datasets), len(classifiers) + 1, i)
         if ds_cnt == 0:
             ax.set_title("Input data")
         # Plot the training points
-        ax.scatter(X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright,
-                   edgecolors='k')
+        ax.scatter(
+            X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright, edgecolors='k'
+        )
         # Plot the testing points
-        ax.scatter(X_test[:, 0], X_test[:, 1], c=y_test, cmap=cm_bright, alpha=0.6,
-                   edgecolors='k')
+        ax.scatter(
+            X_test[:, 0],
+            X_test[:, 1],
+            c=y_test,
+            cmap=cm_bright,
+            alpha=0.6,
+            edgecolors='k',
+        )
         ax.set_xlim(xx.min(), xx.max())
         ax.set_ylim(yy.min(), yy.max())
         ax.set_xticks(())
         ax.set_yticks(())
         i += 1
 
         # iterate over classifiers
@@ -142,59 +164,78 @@
             if hasattr(clf, "decision_function"):
                 Z = clf.decision_function(np.c_[xx.ravel(), yy.ravel()])
             else:
                 Z = clf.predict_proba(np.c_[xx.ravel(), yy.ravel()])[:, 1]
 
             # Put the result into a color plot
             Z = Z.reshape(xx.shape)
-            ax.contourf(xx, yy, Z, cmap=cm, alpha=.8)
+            ax.contourf(xx, yy, Z, cmap=cm, alpha=0.8)
 
             # Plot the training points
-            ax.scatter(X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright,
-                       edgecolors='k')
+            ax.scatter(
+                X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright, edgecolors='k'
+            )
             # Plot the testing points
-            ax.scatter(X_test[:, 0], X_test[:, 1], c=y_test, cmap=cm_bright,
-                       edgecolors='k', alpha=0.6)
+            ax.scatter(
+                X_test[:, 0],
+                X_test[:, 1],
+                c=y_test,
+                cmap=cm_bright,
+                edgecolors='k',
+                alpha=0.6,
+            )
 
             ax.set_xlim(xx.min(), xx.max())
             ax.set_ylim(yy.min(), yy.max())
             ax.set_xticks(())
             ax.set_yticks(())
             if ds_cnt == 0:
                 ax.set_title(name)
-            ax.text(0.95, 0.06, ('%.2f' % score).lstrip('0'), size=15,
+            ax.text(
+                0.95,
+                0.06,
+                ('%.2f' % score).lstrip('0'),
+                size=15,
                 bbox=dict(boxstyle='round', alpha=0.8, facecolor='white'),
-                transform=ax.transAxes, horizontalalignment='right')
+                transform=ax.transAxes,
+                horizontalalignment='right',
+            )
             i += 1
 
     plt.tight_layout()
     plt.show()
 
 
 # %% [markdown]
 # Compare all under-sampling-based ensemble algorithms
 # ----------------------------------------------------
 
 from imbens.ensemble._under_sampling.__init__ import __all__ as names
 
 classifiers = [all_ensembles_clf[name] for name in names]
-plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
+plot_classifier_comparison(
+    classifiers, names, datasets, figsize=(len(names) * 3 + 3, 9)
+)
 
 
 # %% [markdown]
 # Compare all over-sampling-based ensemble algorithms
 # ----------------------------------------------------
 
 from imbens.ensemble._over_sampling.__init__ import __all__ as names
 
 classifiers = [all_ensembles_clf[name] for name in names]
-plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
+plot_classifier_comparison(
+    classifiers, names, datasets, figsize=(len(names) * 3 + 3, 9)
+)
 
 
 # %% [markdown]
 # Compare all reweighting-based ensemble algorithms
 # ----------------------------------------------------
 
 from imbens.ensemble._reweighting.__init__ import __all__ as names
 
 classifiers = [all_ensembles_clf[name] for name in names]
-plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
+plot_classifier_comparison(
+    classifiers, names, datasets, figsize=(len(names) * 3 + 3, 9)
+)
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_classifier_comparison.rst` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/asymmetric_boost.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,383 +1,393 @@
-
-.. DO NOT EDIT.
-.. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
-.. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\classification\plot_classifier_comparison.py"
-.. LINE NUMBERS ARE GIVEN BELOW.
-
-.. only:: html
-
-    .. note::
-        :class: sphx-glr-download-link-note
-
-        Click :ref:`here <sphx_glr_download_auto_examples_classification_plot_classifier_comparison.py>`
-        to download the full example code
-
-.. rst-class:: sphx-glr-example-title
-
-.. _sphx_glr_auto_examples_classification_plot_classifier_comparison.py:
-
-
-=========================================================
-Classifier comparison
-=========================================================
-
-A comparison of a several classifiers in :mod:`imbens.ensemble` 
-on synthetic datasets. The point of this example is to illustrate the nature 
-of decision boundaries of different imbalanced ensmeble classifiers. 
-This should be taken with a grain of salt, as the intuition conveyed by these 
-examples does not necessarily carry over to real datasets.
-
-The plots show training points in solid colors and testing points semi-transparent. 
-The lower right shows the average precision score (AUPRC) on the test set.
-
-This example uses:
-    
-    - Reweighting-based method
-        - :class:`imbens.ensemble.AdaCostClassifier`
-        - :class:`imbens.ensemble.AdaUBoostClassifier`
-        - :class:`imbens.ensemble.AsymBoostClassifier`
-    - Under-sampling-based method
-        - :class:`imbens.ensemble.SelfPacedEnsembleClassifier`
-        - :class:`imbens.ensemble.BalanceCascadeClassifier`
-        - :class:`imbens.ensemble.BalancedRandomForestClassifier`
-        - :class:`imbens.ensemble.EasyEnsembleClassifier`
-        - :class:`imbens.ensemble.RUSBoostClassifier`
-        - :class:`imbens.ensemble.UnderBaggingClassifier`
-    - Over-sampling-based method
-        - :class:`imbens.ensemble.OverBoostClassifier`
-        - :class:`imbens.ensemble.SMOTEBoostClassifier`
-        - :class:`imbens.ensemble.KmeansSMOTEBoostClassifier`
-        - :class:`imbens.ensemble.OverBaggingClassifier`
-        - :class:`imbens.ensemble.SMOTEBaggingClassifier`
-
-.. GENERATED FROM PYTHON SOURCE LINES 35-39
-
-.. code-block:: default
-
-
-    # Authors: Zhining Liu <zhining.liu@outlook.com>
-    # License: MIT
-
-
-
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 40-59
-
-.. code-block:: default
-
-    print(__doc__)
-
-    # Import imbalanced-ensemble
-    import imbens
-
-    # Import utilities
-    import numpy as np
-    import sklearn
-    from sklearn.model_selection import train_test_split
-    from sklearn.preprocessing import StandardScaler
-    from sklearn.datasets import make_moons, make_circles, make_classification
-    from imbens.datasets import make_imbalance
-
-    # Import plot utilities
-    import matplotlib.pyplot as plt
-    from matplotlib.colors import ListedColormap
-
-    RANDOM_STATE = 42
-
-
-
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 60-63
-
-Preparation
------------
-**Make 3 imbalanced toy classification tasks.**
-
-.. GENERATED FROM PYTHON SOURCE LINES 63-81
-
-.. code-block:: default
-
-
-    distribution = {0: 100, 1: 50}
-
-    # dataset 1
-    X, y = make_moons(200, noise=0.2, random_state=RANDOM_STATE)
-    dataset1 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
-    # dataset 2
-    X, y = make_circles(200, noise=0.2, factor=0.5, random_state=RANDOM_STATE)
-    dataset2 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
-    # dataset 3
-    X, y = make_classification(200, n_features=2, n_redundant=0, n_informative=2,
-                               random_state=1, n_clusters_per_class=1)
-    X += 2 * np.random.RandomState(RANDOM_STATE).uniform(size=X.shape)
-    dataset3 = make_imbalance(X, y, sampling_strategy=distribution, random_state=RANDOM_STATE)
-
-    datasets = [dataset1, dataset2, dataset3]
-
-
-
-
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 82-83
-
-**Load all ensemble classifiers**
-
-.. GENERATED FROM PYTHON SOURCE LINES 83-94
-
-.. code-block:: default
-
-
-    from imbens.utils.testing import all_estimators
-
-    init_kwargs = {'n_estimators': 5, 'random_state': RANDOM_STATE}
-    all_ensembles_clf = {name: ensemble(**init_kwargs) for (name, ensemble) in all_estimators('ensemble')}
-
-    print ('{:<30s} | Class \n{:=<120s}'.format('Method', ''))
-    for (name, ensemble) in all_estimators('ensemble'):
-        print ('{:<30s} | {}'.format(name, ensemble))
-
-
-
-
-
-
-.. rst-class:: sphx-glr-script-out
-
- .. code-block:: none
-
-    Method                         | Class 
-    ========================================================================================================================
-    AdaCostClassifier              | <class 'imbens.ensemble._reweighting.adacost.AdaCostClassifier'>
-    AdaUBoostClassifier            | <class 'imbens.ensemble._reweighting.adauboost.AdaUBoostClassifier'>
-    AsymBoostClassifier            | <class 'imbens.ensemble._reweighting.asymmetric_boost.AsymBoostClassifier'>
-    BalanceCascadeClassifier       | <class 'imbens.ensemble._under_sampling.balance_cascade.BalanceCascadeClassifier'>
-    BalancedRandomForestClassifier | <class 'imbens.ensemble._under_sampling.balanced_random_forest.BalancedRandomForestClassifier'>
-    CompatibleAdaBoostClassifier   | <class 'imbens.ensemble._compatible.adaboost_compatible.CompatibleAdaBoostClassifier'>
-    CompatibleBaggingClassifier    | <class 'imbens.ensemble._compatible.bagging_compatible.CompatibleBaggingClassifier'>
-    EasyEnsembleClassifier         | <class 'imbens.ensemble._under_sampling.easy_ensemble.EasyEnsembleClassifier'>
-    KmeansSMOTEBoostClassifier     | <class 'imbens.ensemble._over_sampling.kmeans_smote_boost.KmeansSMOTEBoostClassifier'>
-    OverBaggingClassifier          | <class 'imbens.ensemble._over_sampling.over_bagging.OverBaggingClassifier'>
-    OverBoostClassifier            | <class 'imbens.ensemble._over_sampling.over_boost.OverBoostClassifier'>
-    RUSBoostClassifier             | <class 'imbens.ensemble._under_sampling.rus_boost.RUSBoostClassifier'>
-    SMOTEBaggingClassifier         | <class 'imbens.ensemble._over_sampling.smote_bagging.SMOTEBaggingClassifier'>
-    SMOTEBoostClassifier           | <class 'imbens.ensemble._over_sampling.smote_boost.SMOTEBoostClassifier'>
-    SelfPacedEnsembleClassifier    | <class 'imbens.ensemble._under_sampling.self_paced_ensemble.SelfPacedEnsembleClassifier'>
-    UnderBaggingClassifier         | <class 'imbens.ensemble._under_sampling.under_bagging.UnderBaggingClassifier'>
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 95-96
-
-**Function for classifier comparison**
-
-.. GENERATED FROM PYTHON SOURCE LINES 96-173
-
-.. code-block:: default
-
-
-    def plot_classifier_comparison(classifiers, names, datasets, figsize):
-
-        h = .02  # step size in the mesh
-
-        figure = plt.figure(figsize=figsize)
-        i = 1
-        # iterate over datasets
-        for ds_cnt, ds in enumerate(datasets):
-            # preprocess dataset, split into training and test part
-            X, y = ds
-            X = StandardScaler().fit_transform(X)
-            X_train, X_test, y_train, y_test = \
-                train_test_split(X, y, test_size=.4, random_state=42)
-
-            x_min, x_max = X[:, 0].min() - .5, X[:, 0].max() + .5
-            y_min, y_max = X[:, 1].min() - .5, X[:, 1].max() + .5
-            xx, yy = np.meshgrid(np.arange(x_min, x_max, h),
-                                 np.arange(y_min, y_max, h))
-
-            # just plot the dataset first
-            cm = plt.cm.RdBu
-            cm_bright = ListedColormap(['#FF0000', '#0000FF'])
-            ax = plt.subplot(len(datasets), len(classifiers) + 1, i)
-            if ds_cnt == 0:
-                ax.set_title("Input data")
-            # Plot the training points
-            ax.scatter(X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright,
-                       edgecolors='k')
-            # Plot the testing points
-            ax.scatter(X_test[:, 0], X_test[:, 1], c=y_test, cmap=cm_bright, alpha=0.6,
-                       edgecolors='k')
-            ax.set_xlim(xx.min(), xx.max())
-            ax.set_ylim(yy.min(), yy.max())
-            ax.set_xticks(())
-            ax.set_yticks(())
-            i += 1
-
-            # iterate over classifiers
-            for name, clf in zip(names, classifiers):
-                ax = plt.subplot(len(datasets), len(classifiers) + 1, i)
-                clf.fit(X_train, y_train)
-                score = sklearn.metrics.average_precision_score(y_test, clf.predict(X_test))
-
-                # Plot the decision boundary. For that, we will assign a color to each
-                # point in the mesh [x_min, x_max]x[y_min, y_max].
-                if hasattr(clf, "decision_function"):
-                    Z = clf.decision_function(np.c_[xx.ravel(), yy.ravel()])
-                else:
-                    Z = clf.predict_proba(np.c_[xx.ravel(), yy.ravel()])[:, 1]
-
-                # Put the result into a color plot
-                Z = Z.reshape(xx.shape)
-                ax.contourf(xx, yy, Z, cmap=cm, alpha=.8)
-
-                # Plot the training points
-                ax.scatter(X_train[:, 0], X_train[:, 1], c=y_train, cmap=cm_bright,
-                           edgecolors='k')
-                # Plot the testing points
-                ax.scatter(X_test[:, 0], X_test[:, 1], c=y_test, cmap=cm_bright,
-                           edgecolors='k', alpha=0.6)
-
-                ax.set_xlim(xx.min(), xx.max())
-                ax.set_ylim(yy.min(), yy.max())
-                ax.set_xticks(())
-                ax.set_yticks(())
-                if ds_cnt == 0:
-                    ax.set_title(name)
-                ax.text(0.95, 0.06, ('%.2f' % score).lstrip('0'), size=15,
-                    bbox=dict(boxstyle='round', alpha=0.8, facecolor='white'),
-                    transform=ax.transAxes, horizontalalignment='right')
-                i += 1
-
-        plt.tight_layout()
-        plt.show()
-
-
-
-
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 174-176
-
-Compare all under-sampling-based ensemble algorithms
-----------------------------------------------------
-
-.. GENERATED FROM PYTHON SOURCE LINES 176-183
-
-.. code-block:: default
-
-
-    from imbens.ensemble._under_sampling.__init__ import __all__ as names
-
-    classifiers = [all_ensembles_clf[name] for name in names]
-    plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
-
-
-
-
-
-.. image-sg:: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_001.png
-   :alt: Input data, SelfPacedEnsembleClassifier, BalanceCascadeClassifier, BalancedRandomForestClassifier, EasyEnsembleClassifier, RUSBoostClassifier, UnderBaggingClassifier
-   :srcset: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_001.png
-   :class: sphx-glr-single-img
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 184-186
-
-Compare all over-sampling-based ensemble algorithms
-----------------------------------------------------
-
-.. GENERATED FROM PYTHON SOURCE LINES 186-193
-
-.. code-block:: default
-
-
-    from imbens.ensemble._over_sampling.__init__ import __all__ as names
-
-    classifiers = [all_ensembles_clf[name] for name in names]
-    plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
-
-
-
-
-
-.. image-sg:: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_002.png
-   :alt: Input data, OverBoostClassifier, SMOTEBoostClassifier, KmeansSMOTEBoostClassifier, OverBaggingClassifier, SMOTEBaggingClassifier
-   :srcset: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_002.png
-   :class: sphx-glr-single-img
-
-
-
-
-
-.. GENERATED FROM PYTHON SOURCE LINES 194-196
-
-Compare all reweighting-based ensemble algorithms
-----------------------------------------------------
-
-.. GENERATED FROM PYTHON SOURCE LINES 196-201
-
-.. code-block:: default
-
-
-    from imbens.ensemble._reweighting.__init__ import __all__ as names
-
-    classifiers = [all_ensembles_clf[name] for name in names]
-    plot_classifier_comparison(classifiers, names, datasets, figsize=(len(names)*3+3, 9))
-
-
-
-.. image-sg:: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_003.png
-   :alt: Input data, AdaCostClassifier, AdaUBoostClassifier, AsymBoostClassifier
-   :srcset: /auto_examples/classification/images/sphx_glr_plot_classifier_comparison_003.png
-   :class: sphx-glr-single-img
-
-
-
-
-
-
-.. rst-class:: sphx-glr-timing
-
-   **Total running time of the script:** ( 0 minutes  4.204 seconds)
-
-
-.. _sphx_glr_download_auto_examples_classification_plot_classifier_comparison.py:
-
-.. only:: html
-
-  .. container:: sphx-glr-footer sphx-glr-footer-example
-
-
-    .. container:: sphx-glr-download sphx-glr-download-python
-
-      :download:`Download Python source code: plot_classifier_comparison.py <plot_classifier_comparison.py>`
-
-    .. container:: sphx-glr-download sphx-glr-download-jupyter
-
-      :download:`Download Jupyter notebook: plot_classifier_comparison.ipynb <plot_classifier_comparison.ipynb>`
-
-
-.. only:: html
-
- .. rst-class:: sphx-glr-signature
-
-    `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
+"""AsymBoostClassifier: An Asymmetric Boosting classifier.
+"""
+
+# Authors: Zhining Liu <zhining.liu@outlook.com>
+# License: MIT
+
+# %%
+LOCAL_DEBUG = False
+
+if not LOCAL_DEBUG:
+    from ...utils._docstring import (
+        FuncSubstitution,
+        Substitution,
+        _get_example_docstring,
+        _get_parameter_docstring,
+    )
+    from ...utils._validation import _deprecate_positional_args
+    from .._boost import ReweightBoostClassifier
+else:  # pragma: no cover
+    import sys  # For local test
+
+    sys.path.append("../..")
+    from ensemble._boost import ReweightBoostClassifier
+    from utils._validation import _deprecate_positional_args
+    from utils._docstring import (
+        Substitution,
+        FuncSubstitution,
+        _get_parameter_docstring,
+        _get_example_docstring,
+    )
+
+import numpy as np
+import pandas as pd
+
+# Properties
+_method_name = 'AsymBoostClassifier'
+
+_solution_type = ReweightBoostClassifier._solution_type
+_ensemble_type = ReweightBoostClassifier._ensemble_type
+_training_type = ReweightBoostClassifier._training_type
+
+_properties = {
+    'solution_type': _solution_type,
+    'ensemble_type': _ensemble_type,
+    'training_type': _training_type,
+}
+
+
+@Substitution(
+    early_termination=_get_parameter_docstring('early_termination', **_properties),
+    random_state=_get_parameter_docstring('random_state', **_properties),
+    example=_get_example_docstring(_method_name),
+)
+class AsymBoostClassifier(ReweightBoostClassifier):
+    """An Asymmetric Boosting classifier.
+
+    Asymmetric Boosting (AsymBoost) [1]_, a variant of AdaBoost, is a
+    cost-sensitive boosting method. It uses the asymmetric misclassication
+    cost to update the training distribution on successive boosting rounds.
+
+    This AsymBoost implementation supports multi-class classification.
+
+    Parameters
+    ----------
+    estimator : estimator object, default=None
+        The base estimator from which the boosted ensemble is built.
+        Support for sample weighting is required, as well as proper
+        ``classes_`` and ``n_classes_`` attributes. If ``None``, then
+        the base estimator is ``DecisionTreeClassifier(max_depth=1)``.
+
+    n_estimators : int, default=50
+        The maximum number of estimators at which boosting is terminated.
+        In case of perfect fit, the learning procedure is stopped early.
+
+    learning_rate : float, default=1.
+        Learning rate shrinks the contribution of each classifier by
+        ``learning_rate``. There is a trade-off between ``learning_rate`` and
+        ``n_estimators``.
+
+    algorithm : {{'SAMME', 'SAMME.R'}}, default='SAMME.R'
+        If 'SAMME.R' then use the SAMME.R real boosting algorithm.
+        ``estimator`` must support calculation of class probabilities.
+        If 'SAMME' then use the SAMME discrete boosting algorithm.
+        The SAMME.R algorithm typically converges faster than SAMME,
+        achieving a lower test error with fewer boosting iterations.
+
+    {early_termination}
+
+    {random_state}
+
+    Attributes
+    ----------
+    estimators_ : list of classifiers
+        The collection of fitted sub-estimators.
+
+    cost_matrix_ : array of shape = [n_classes, n_classes]
+        The used cost matrix. The rows represent the predicted class and
+        columns represent the actual class. The order of the classes
+        corresponds to that in the attribute ``classes_``.
+
+    cost_table_asymboost_ : DataFrame of shape = [n_classes*n_classes, 3]
+        The used cost map table.
+
+    classes_ : array of shape = [n_classes]
+        The classes labels.
+
+    n_classes_ : int
+        The number of classes.
+
+    estimator_weights_ : array of floats
+        Weights for each estimator in the boosted ensemble.
+
+    estimator_errors_ : array of floats
+        Classification error for each estimator in the boosted
+        ensemble.
+
+    estimators_n_training_samples_ : list of ints
+        The number of training samples for each fitted
+        base estimators.
+
+    feature_importances_ : array of shape = [n_features]
+        The feature importances if supported by the ``estimator``.
+
+    See also
+    --------
+    AdaUBoostClassifier : An AdaUBoost cost-sensitive classifier.
+
+    AdaCostClassifier : An AdaCost cost-sensitive boosting classifier.
+
+    References
+    ----------
+    .. [1] Viola, P., & Jones, M. "Fast and robust classification using
+       asymmetric adaboost and a detector cascade." Advances in Neural
+       Information Processing System 14 (2001).
+
+    Examples
+    --------
+    {example}
+    """
+
+    @_deprecate_positional_args
+    def __init__(
+        self,
+        estimator=None,
+        n_estimators: int = 50,
+        *,
+        learning_rate: float = 1.0,
+        algorithm: str = 'SAMME.R',
+        early_termination: bool = False,
+        random_state=None,
+    ):
+
+        super(AsymBoostClassifier, self).__init__(
+            estimator=estimator,
+            n_estimators=n_estimators,
+            learning_rate=learning_rate,
+            algorithm=algorithm,
+            early_termination=early_termination,
+            random_state=random_state,
+        )
+
+        self.__name__ = _method_name
+        self._properties = _properties
+
+    def _compute_mult_out_exp_weights_array(self, y_true, y_pred):
+        """Return the asymmetric weights of shape = (n_samples,).
+
+        Parameters
+        ----------
+        y_true : array-like of shape = [n_samples, 1]
+                 True class values.
+
+        y_pred : array-like of shape = [n_samples, 1]
+                 Predicted class values.
+        """
+        df = pd.DataFrame({'y_pred': y_pred, 'y_true': y_true})
+        df = df.merge(self.cost_table_asymboost_, how='left', on=['y_pred', 'y_true'])
+
+        return df['asym_weight'].values
+
+    def _cost_matrix_to_asymmetric_weights(self, cost_matrix):
+        """Creates a table of asymmetric weight map table from the cost matrix.
+
+        Parameters
+        ----------
+        cost_matrix : array-like of shape = [n_classes, n_classes]
+
+        Returns
+        -------
+        df : pd.DataFrame of shape = [n_classes, 2]
+
+        """
+        table = np.empty((0, 3))
+
+        for (x, y), value in np.ndenumerate(cost_matrix):
+            # Section 4 of [1]
+            table = np.vstack(
+                (
+                    table,
+                    np.array(
+                        [x, y, np.exp(1 / self.n_estimators * np.log(np.sqrt(value)))]
+                    ),
+                )
+            )
+
+        return pd.DataFrame(table, columns=['y_pred', 'y_true', 'asym_weight'])
+
+    def _validate_cost_matrix(self, cost_matrix, n_classes):
+        """validate the cost matrix & set the cost map table."""
+
+        cost_matrix = super()._validate_cost_matrix(cost_matrix, n_classes)
+        self.cost_table_asymboost_ = self._cost_matrix_to_asymmetric_weights(
+            cost_matrix
+        )
+
+        return cost_matrix
+
+    @_deprecate_positional_args
+    @FuncSubstitution(
+        eval_datasets=_get_parameter_docstring('eval_datasets'),
+        eval_metrics=_get_parameter_docstring('eval_metrics'),
+        train_verbose=_get_parameter_docstring('train_verbose', **_properties),
+    )
+    def fit(
+        self,
+        X,
+        y,
+        *,
+        sample_weight=None,
+        cost_matrix='inverse',
+        eval_datasets: dict = None,
+        eval_metrics: dict = None,
+        train_verbose: bool or int or dict = False,
+    ):
+        """Build a AsymBoost classifier from the training set (X, y).
+
+        Parameters
+        ----------
+        X : {array-like, sparse matrix} of shape (n_samples, n_features)
+            The training input samples. Sparse matrix can be CSC, CSR, COO,
+            DOK, or LIL. DOK and LIL are converted to CSR.
+
+        y : array-like of shape (n_samples,)
+            The target values (class labels).
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, the sample weights are initialized to
+            ``1 / n_samples``.
+
+        cost_matrix : str or numpy.ndarray, default=None
+            A matrix representing the cost of misclassification.
+
+            - If ``None``, equivalent to ``'inverse'``.
+            - If ``'uniform'``, set misclassification cost to be equal.
+            - If ``'inverse'``, set misclassification cost by inverse class frequency.
+            - If ``numpy.ndarray`` of shape (n_classes, n_classes), the rows
+              represent the predicted class and columns represent the actual class.
+              Thus the value at :math:`i`-th row :math:`j`-th column (:math:`C_{ij}`)
+              represents the cost of classifying a sample from class :math:`j` to
+              class :math:`i`.
+              Note: the cost matrix must satisfy that :math:`C_{ij} * C_{ji} = 1`.
+
+        %(eval_datasets)s
+
+        %(eval_metrics)s
+
+        %(train_verbose)s
+
+        Returns
+        -------
+        self : object
+        """
+
+        # Note that AsymBoost requires the cost matrix to satisfy
+        # C_{ij} * C_{ji} = 1, thus the 'log1p-inverse' option is not
+        # available in this situation.
+        if type(cost_matrix) == str and cost_matrix == 'log1p-inverse':
+            raise ValueError(
+                "'log1p-inverse' option is not available for "
+                "AsymBoostClassifier. Please use 'inverse' instead."
+            )
+
+        return self._fit(
+            X,
+            y,
+            sample_weight=sample_weight,
+            cost_matrix=cost_matrix,
+            eval_datasets=eval_datasets,
+            eval_metrics=eval_metrics,
+            train_verbose=train_verbose,
+        )
+
+
+# %%
+
+if __name__ == "__main__":  # pragma: no cover
+    from collections import Counter
+    from copy import copy
+
+    from sklearn.datasets import make_classification
+    from sklearn.metrics import accuracy_score, balanced_accuracy_score, f1_score
+    from sklearn.model_selection import train_test_split
+    from sklearn.tree import DecisionTreeClassifier
+
+    # X, y = make_classification(n_classes=2, class_sep=2, # 2-class
+    #     weights=[0.1, 0.9], n_informative=3, n_redundant=1, flip_y=0,
+    #     n_features=20, n_clusters_per_class=1, n_samples=1000, random_state=10)
+    X, y = make_classification(
+        n_classes=3,
+        class_sep=2,  # 3-class
+        weights=[0.1, 0.3, 0.6],
+        n_informative=3,
+        n_redundant=1,
+        flip_y=0,
+        n_features=20,
+        n_clusters_per_class=1,
+        n_samples=2000,
+        random_state=10,
+    )
+
+    X_train, X_valid, y_train, y_valid = train_test_split(
+        X, y, test_size=0.5, random_state=42
+    )
+
+    origin_distr = dict(Counter(y_train))  # {2: 600, 1: 300, 0: 100}
+    print('Original training dataset shape %s' % origin_distr)
+
+    init_kwargs_default = {
+        'estimator': None,
+        'n_estimators': 100,
+        'learning_rate': 1.0,
+        'algorithm': 'SAMME.R',
+        'random_state': 42,
+        # 'random_state': None,
+    }
+    fit_kwargs_default = {
+        'X': X_train,
+        'y': y_train,
+        'sample_weight': None,
+        'eval_datasets': {'valid': (X_valid, y_valid)},
+        'eval_metrics': {
+            'acc': (accuracy_score, {}),
+            'balanced_acc': (balanced_accuracy_score, {}),
+            'weighted_f1': (f1_score, {'average': 'weighted'}),
+        },
+        'train_verbose': {
+            'granularity': 10,
+            'print_distribution': True,
+            'print_metrics': True,
+        },
+    }
+
+    ensembles = {}
+
+    init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
+    asymboost = AsymBoostClassifier(**init_kwargs).fit(**fit_kwargs)
+    ensembles['asymboost'] = asymboost
+
+    init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
+    fit_kwargs.update(
+        {
+            'cost_matrix': 'uniform',
+        }
+    )
+    asymboost_uniform = AsymBoostClassifier(**init_kwargs).fit(**fit_kwargs)
+    ensembles['asymboost_uniform'] = asymboost_uniform
+
+    # %%
+    from imbens.visualizer import ImbalancedEnsembleVisualizer
+
+    visualizer = ImbalancedEnsembleVisualizer(
+        eval_datasets=None,
+        eval_metrics=None,
+    ).fit(
+        ensembles=ensembles,
+        granularity=5,
+    )
+    fig, axes = visualizer.performance_lineplot(
+        on_ensembles=None,
+        on_datasets=None,
+        split_by=[],
+        n_samples_as_x_axis=False,
+        sub_figsize=(4, 3.3),
+        sup_title=True,
+        alpha=0.8,
+    )
+    fig, axes = visualizer.confusion_matrix_heatmap(
+        on_ensembles=None,
+        on_datasets=None,
+        sub_figsize=(4, 3.3),
+    )
+
+    # %%
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_cost_matrix.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_cost_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from sklearn.model_selection import train_test_split
 from imbens.ensemble.base import sort_dict_by_key
 from collections import Counter
 
 # Import plot utilities
 import matplotlib.pyplot as plt
 import seaborn as sns
+
 sns.set_context('talk')
 
 RANDOM_STATE = 42
 
 init_kwargs = {
     'n_estimators': 5,
     'random_state': RANDOM_STATE,
@@ -43,47 +44,58 @@
 
 # %% [markdown]
 # Prepare data
 # ------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # Print class distribution
 print('Training dataset distribution    %s' % sort_dict_by_key(Counter(y_train)))
 print('Validation dataset distribution  %s' % sort_dict_by_key(Counter(y_valid)))
 
 
 # %% [markdown]
 # Implement some plot utilities
 
 cost_matrices = {}
 
-def plot_cost_matrix(cost_matrix, title:str, **kwargs):
+
+def plot_cost_matrix(cost_matrix, title: str, **kwargs):
     ax = sns.heatmap(data=cost_matrix, **kwargs)
     ax.set_ylabel("Predicted Label")
     ax.set_xlabel("Ground Truth")
     ax.set_title(title)
 
 
 # %% [markdown]
 # Default Cost Matrix
 # ----------------------------
 # By default, cost-sensitive ensemble methods will set misclassification cost by inverse class frequency.
 
 # %% [markdown]
-# **You can access the ``clf.cost_matrix_`` attribute (``clf`` is a fitted cost-sensitive ensemble classifier) to view the cost matrix used for training.**  
-# The rows represent the predicted class and columns represent the actual class.  
+# **You can access the ``clf.cost_matrix_`` attribute (``clf`` is a fitted cost-sensitive ensemble classifier) to view the cost matrix used for training.**
+# The rows represent the predicted class and columns represent the actual class.
 # Note that the order of the classes corresponds to that in the attribute ``clf.classes_``.
 
 # %% [markdown]
 # Take ``AdaCostClassifier`` as example
 
 adacost_clf = imbens.ensemble.AdaCostClassifier(**init_kwargs)
 
@@ -103,20 +115,22 @@
 cost_matrices[title] = adacost_clf.cost_matrix_
 plot_cost_matrix(adacost_clf.cost_matrix_, title, annot=True, cmap='YlOrRd', vmax=6)
 
 
 # %% [markdown]
 # ``log1p-inverse`` Cost Matrix
 # -----------------------------
-# You can set misclassification cost by log inverse class frequency by set ``cost_matrix`` = ``'log1p-inverse'``.  
+# You can set misclassification cost by log inverse class frequency by set ``cost_matrix`` = ``'log1p-inverse'``.
 # This usually leads to a "softer" cost matrix, that is, less penalty for misclassification of minority class samples into the majority class.
 
-adacost_clf.fit(X_train, y_train,
-               cost_matrix = 'log1p-inverse', # set cost matrix by log inverse class frequency
-               )
+adacost_clf.fit(
+    X_train,
+    y_train,
+    cost_matrix='log1p-inverse',  # set cost matrix by log inverse class frequency
+)
 
 adacost_clf.cost_matrix_
 
 
 # %% [markdown]
 # **Visualize the log1p-inverse cost matrix**
 
@@ -124,21 +138,23 @@
 cost_matrices[title] = adacost_clf.cost_matrix_
 plot_cost_matrix(adacost_clf.cost_matrix_, title, annot=True, cmap='YlOrRd', vmax=6)
 
 
 # %% [markdown]
 # Use Uniform Cost Matrix
 # ----------------------------
-# You can set misclassification cost by log inverse class frequency by set ``cost_matrix`` = ``'uniform'``.  
+# You can set misclassification cost by log inverse class frequency by set ``cost_matrix`` = ``'uniform'``.
 
 # Note that this will set all misclassification cost to be equal, i.e., model will not be cost-sensitive.
 
-adacost_clf.fit(X_train, y_train,
-               cost_matrix = 'uniform', # set cost matrix to be uniform
-               )
+adacost_clf.fit(
+    X_train,
+    y_train,
+    cost_matrix='uniform',  # set cost matrix to be uniform
+)
 
 adacost_clf.cost_matrix_
 
 
 # %% [markdown]
 # **Visualize the uniform cost matrix**
 
@@ -146,30 +162,32 @@
 cost_matrices[title] = adacost_clf.cost_matrix_
 plot_cost_matrix(adacost_clf.cost_matrix_, title, annot=True, cmap='YlOrRd', vmax=6)
 
 
 # %% [markdown]
 # Use Your Own Cost Matrix
 # ------------------------
-# You can also set misclassification cost by explicitly passing your cost matrix to ``cost_matrix``.  
+# You can also set misclassification cost by explicitly passing your cost matrix to ``cost_matrix``.
 
 # %% [markdown]
-# Your cost matrix must be a ``numpy.2darray`` of shape (n_classes, n_classes), the rows represent the predicted class and columns represent the actual class.  
+# Your cost matrix must be a ``numpy.2darray`` of shape (n_classes, n_classes), the rows represent the predicted class and columns represent the actual class.
 # Thus the value at :math:`i`-th row :math:`j`-th column represents the cost of classifying a sample from class :math:`j` to class :math:`i`.
 
 # set your own cost matrix
 my_cost_matrix = [
     [1, 1, 1],
     [2, 1, 1],
     [5, 2, 1],
 ]
 
-adacost_clf.fit(X_train, y_train,
-               cost_matrix = my_cost_matrix, # use your cost matrix
-               )
+adacost_clf.fit(
+    X_train,
+    y_train,
+    cost_matrix=my_cost_matrix,  # use your cost matrix
+)
 
 adacost_clf.cost_matrix_
 
 
 # %% [markdown]
 # **Visualize the user-define cost matrix**
 
@@ -181,9 +199,10 @@
 # %% [markdown]
 # Visualize All Used Cost Matrices
 # --------------------------------
 
 sns.set_context('notebook')
 fig, axes = plt.subplots(1, 4, figsize=(20, 4))
 for ax, title in zip(axes, cost_matrices.keys()):
-    plot_cost_matrix(cost_matrices[title], title, 
-                     annot=True, cmap='YlOrRd', vmax=6, ax=ax)
+    plot_cost_matrix(
+        cost_matrices[title], title, annot=True, cmap='YlOrRd', vmax=6, ax=ax
+    )
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_digits.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_digits.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,75 +56,88 @@
 
 # %% [markdown]
 # **The original digits dataset**
 
 fig = plot_2Dprojection_and_cardinality(X, y, figsize=(8, 4))
 
 
-
 # %% [markdown]
 # **Make class-imbalanced digits dataset**
 
-imbalance_distr = {0: 178, 1: 120, 2: 80, 3: 60, 4: 50, 5: 44, 6: 40, 7: 40, 8: 40, 9: 40}
+imbalance_distr = {
+    0: 178,
+    1: 120,
+    2: 80,
+    3: 60,
+    4: 50,
+    5: 44,
+    6: 40,
+    7: 40,
+    8: 40,
+    9: 40,
+}
 
-X, y = make_imbalance(X, y, sampling_strategy=imbalance_distr, random_state=RANDOM_STATE)
+X, y = make_imbalance(
+    X, y, sampling_strategy=imbalance_distr, random_state=RANDOM_STATE
+)
 
 fig = plot_2Dprojection_and_cardinality(X, y, figsize=(8, 4))
 
 
-
 # %% [markdown]
 # Classification
 # --------------
-# We split the data into train and test subsets and fit a ``SelfPacedEnsembleClassifier`` (with support vector machine as base classifier) on the train samples.  
+# We split the data into train and test subsets and fit a ``SelfPacedEnsembleClassifier`` (with support vector machine as base classifier) on the train samples.
 # The fitted classifier can subsequently be used to predict the value of the digit for the samples in the test subset.
 
 # Split data into 50% train and 50% test subsets
 X_train, X_test, y_train, y_test = train_test_split(
-    X, y, test_size=0.5, shuffle=True, stratify=y, random_state=0)
+    X, y, test_size=0.5, shuffle=True, stratify=y, random_state=0
+)
 
 # Create a classifier: a SPE with support vector base classifier
 base_clf = sklearn.svm.SVC(gamma=0.001, probability=True)
 clf = imbens.ensemble.SelfPacedEnsembleClassifier(
-    n_estimators=5, estimator=base_clf,
+    n_estimators=5,
+    estimator=base_clf,
 )
 
 # Learn the digits on the train subset
 clf.fit(X_train, y_train)
 
 # Predict the value of the digit on the test subset
 predicted = clf.predict(X_test)
 
 
-
 # %% [markdown]
 # ``sklearn.metrics.classification_report`` builds a text report showing the main classification metrics.
 
-print(f"Classification report for classifier {clf}:\n"
-      f"{sklearn.metrics.classification_report(y_test, predicted)}\n")
+print(
+    f"Classification report for classifier {clf}:\n"
+    f"{sklearn.metrics.classification_report(y_test, predicted)}\n"
+)
 
 
 # %% [markdown]
 # Below we visualize the first 4 test samples and show their predicted digit value in the title.
 
 _, axes = plt.subplots(nrows=1, ncols=4, figsize=(10, 3))
 for ax, image, prediction in zip(axes, X_test, predicted):
     ax.set_axis_off()
     image = image.reshape(8, 8)
     ax.imshow(image, cmap=plt.cm.gray_r, interpolation='nearest')
     ax.set_title(f'Prediction: {prediction}')
 
 
-
 # %% [markdown]
 # We can also plot a confusion matrix of the true digit values and the predicted digit values using the ``ImbalancedEnsembleVisualizer``.
 
 visualizer = imbens.visualizer.ImbalancedEnsembleVisualizer(
-    eval_datasets = {
-        'test' : (X_test, y_test),
+    eval_datasets={
+        'test': (X_test, y_test),
     },
 ).fit({'SPE': clf})
 
 fig, axes = visualizer.confusion_matrix_heatmap(
     sub_figsize=(8, 7),
     false_pred_only=True,
 )
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_probability.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_probability.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,38 +38,42 @@
 # -----------
 # **Make 3 imbalanced iris classification tasks.**
 
 iris = sklearn.datasets.load_iris()
 X = iris.data[:, 0:2]  # we only take the first two features for visualization
 y = iris.target
 
-X, y = make_imbalance(X, y, 
-                      sampling_strategy={0: 50, 1: 30, 2: 10}, 
-                      random_state=RANDOM_STATE)
-print('Class distribution of imbalanced iris dataset: \n%s' % sort_dict_by_key(Counter(y)))
-
+X, y = make_imbalance(
+    X, y, sampling_strategy={0: 50, 1: 30, 2: 10}, random_state=RANDOM_STATE
+)
+print(
+    'Class distribution of imbalanced iris dataset: \n%s' % sort_dict_by_key(Counter(y))
+)
 
 
 # %% [markdown]
 # **Create SPE (ensemble size = 5) with different base classifiers.**
 
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.gaussian_process.kernels import RBF
 
 classifiers = {
     'SPE-DT': imbens.ensemble.SelfPacedEnsembleClassifier(
-        n_estimators=5, estimator=DecisionTreeClassifier(),
+        n_estimators=5,
+        estimator=DecisionTreeClassifier(),
     ),
     'SPE-SVM-rbf': imbens.ensemble.SelfPacedEnsembleClassifier(
-        n_estimators=5, estimator=SVC(kernel='rbf', probability=True),
+        n_estimators=5,
+        estimator=SVC(kernel='rbf', probability=True),
     ),
     'SPE-GPC': imbens.ensemble.SelfPacedEnsembleClassifier(
-        n_estimators=5, estimator=GaussianProcessClassifier(1.0 * RBF([1.0, 1.0])),
+        n_estimators=5,
+        estimator=GaussianProcessClassifier(1.0 * RBF([1.0, 1.0])),
     ),
 }
 
 n_classifiers = len(classifiers)
 
 
 # %% [markdown]
@@ -77,15 +81,15 @@
 # ---------------------------------
 
 import matplotlib.pyplot as plt
 
 n_features = X.shape[1]
 
 plt.figure(figsize=(3 * 2, n_classifiers * 2))
-plt.subplots_adjust(bottom=.2, top=.95)
+plt.subplots_adjust(bottom=0.2, top=0.95)
 
 xx = np.linspace(3, 9, 100)
 yy = np.linspace(1, 5, 100).T
 xx, yy = np.meshgrid(xx, yy)
 Xfull = np.c_[xx.ravel(), yy.ravel()]
 
 for index, (name, classifier) in enumerate(classifiers.items()):
@@ -99,19 +103,20 @@
     probas = classifier.predict_proba(Xfull)
     n_classes = np.unique(y_pred).size
     for k in range(n_classes):
         plt.subplot(n_classifiers, n_classes, index * n_classes + k + 1)
         plt.title("Class %d" % k)
         if k == 0:
             plt.ylabel(name)
-        imshow_handle = plt.imshow(probas[:, k].reshape((100, 100)),
-                                   extent=(3, 9, 1, 5), origin='lower')
+        imshow_handle = plt.imshow(
+            probas[:, k].reshape((100, 100)), extent=(3, 9, 1, 5), origin='lower'
+        )
         plt.xticks(())
         plt.yticks(())
-        idx = (y_pred == k)
+        idx = y_pred == k
         if idx.any():
             plt.scatter(X[idx, 0], X[idx, 1], marker='o', c='w', edgecolor='k')
 
 ax = plt.axes([0.15, 0.04, 0.7, 0.05])
 plt.title("Probability")
 plt.colorbar(imshow_handle, cax=ax, orientation='horizontal')
 plt.show()
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_resampling_target.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_resampling_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from imbens.ensemble.base import sort_dict_by_key
 from collections import Counter
 
 # Import plot utilities
 from imbens.utils._plot import set_ax_border
 import matplotlib.pyplot as plt
 import seaborn as sns
+
 sns.set_context('talk')
 
 RANDOM_STATE = 42
 
 init_kwargs = {
     'n_estimators': 1,
     'random_state': RANDOM_STATE,
@@ -51,135 +52,152 @@
 
 # %% [markdown]
 # Prepare data
 # ------------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # Generate and split a synthetic dataset
-X, y = make_classification(n_classes=3, n_samples=2000, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, random_state=RANDOM_STATE)
-X_train, X_valid, y_train, y_valid = train_test_split(X, y, 
-    test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+X, y = make_classification(
+    n_classes=3,
+    n_samples=2000,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    random_state=RANDOM_STATE,
+)
+X_train, X_valid, y_train, y_valid = train_test_split(
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # Print class distribution
 print('Training dataset distribution    %s' % sort_dict_by_key(Counter(y_train)))
 print('Validation dataset distribution  %s' % sort_dict_by_key(Counter(y_valid)))
 
 # %% [markdown]
 # Implement some plot utilities
 
 ylim = (0, 630)
 
 all_distribution = {}
 
-def plot_class_distribution(distr:dict, xlabel:str='Class Label', 
-                            ylabel:str='Number of samples', **kwargs):
+
+def plot_class_distribution(
+    distr: dict,
+    xlabel: str = 'Class Label',
+    ylabel: str = 'Number of samples',
+    **kwargs
+):
     distr = dict(sorted(distr.items(), key=lambda k: k[0], reverse=True))
     ax = sns.barplot(
-        x=list(distr.keys()), 
-        y=list(distr.values()),
-        order=list(distr.keys()),
-        **kwargs
+        x=list(distr.keys()), y=list(distr.values()), order=list(distr.keys()), **kwargs
     )
     set_ax_border(ax)
     ax.grid(axis='y', alpha=0.5, ls='-.')
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     return ax
 
-def plot_class_distribution_comparison(clf, 
-                                       title1='Original imbalanced class distribution', 
-                                       title2='After resampling', figsize=(12, 6)):
+
+def plot_class_distribution_comparison(
+    clf,
+    title1='Original imbalanced class distribution',
+    title2='After resampling',
+    figsize=(12, 6),
+):
     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
     plot_class_distribution(clf.origin_distr_, ax=ax1)
     ax1.set(ylim=ylim, title=title1)
     plot_class_distribution(clf.target_distr_, ax=ax2)
     ax2.set(ylim=ylim, title=title2)
     fig.tight_layout()
 
 
 # %% [markdown]
 # Default under-sampling
 # ----------------------------
-# By default, under-sampling-based ensemble methods will consider the smallest class as the minority class (class 0 with 100 samples).  
-# All other classes (class 1 and 2) will be considered as majority classes and will be under-sampled until the number of samples is equalized.  
+# By default, under-sampling-based ensemble methods will consider the smallest class as the minority class (class 0 with 100 samples).
+# All other classes (class 1 and 2) will be considered as majority classes and will be under-sampled until the number of samples is equalized.
 
 # %% [markdown]
 # Take ``SelfPacedEnsembleClassifier`` as example
 
 spe_clf = imbens.ensemble.SelfPacedEnsembleClassifier(**init_kwargs)
 
 
 # %% [markdown]
 # **Train with the default under-sampling setting**
 
 spe_clf.fit(X_train, y_train, **fit_kwargs)
 
 all_distribution['Before under-sampling'] = spe_clf.origin_distr_
-resampling_type='After default under-sampling'
+resampling_type = 'After default under-sampling'
 all_distribution[resampling_type] = spe_clf.target_distr_
 plot_class_distribution_comparison(spe_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # Specify the class targeted by the under-sampling
 # -------------------------------------------------
-# **Set parameter ``target_label``: int**  
-# All other classes that have more samples than the target class will be considered as majority classes.  
-# They will be under-sampled until the number of samples is equalized.  
+# **Set parameter ``target_label``: int**
+# All other classes that have more samples than the target class will be considered as majority classes.
+# They will be under-sampled until the number of samples is equalized.
 # The remaining minority classes (if any) will stay unchanged.
 
-spe_clf.fit(X_train, y_train, 
-            target_label=1, # target class 1
-            **fit_kwargs)
+spe_clf.fit(X_train, y_train, target_label=1, **fit_kwargs)  # target class 1
 
-resampling_type='After under-sampling (target class 1)'
+resampling_type = 'After under-sampling (target class 1)'
 all_distribution[resampling_type] = spe_clf.target_distr_
 plot_class_distribution_comparison(spe_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # Specify the desired number of samples after under-sampling
 # -----------------------------------------------------------
-# **Set parameter ``n_target_samples``: int or dict**  
+# **Set parameter ``n_target_samples``: int or dict**
 # If int, all classes that have more than the n_target_samples samples will be under-sampled until the number of samples is equalized.
 
-spe_clf.fit(X_train, y_train, 
-            n_target_samples=200, # target number of samples 200
-            **fit_kwargs)
+spe_clf.fit(
+    X_train, y_train, n_target_samples=200, **fit_kwargs  # target number of samples 200
+)
 
-resampling_type='After under-sampling (target number 200)'
+resampling_type = 'After under-sampling (target number 200)'
 all_distribution[resampling_type] = spe_clf.target_distr_
 plot_class_distribution_comparison(spe_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # Specify the desired number of samples of each class after under-sampling
 # ------------------------------------------------------------------------
-# **Set parameter ``n_target_samples``: int or dict**  
+# **Set parameter ``n_target_samples``: int or dict**
 # If dict, the keys correspond to the targeted classes. The values correspond to the desired number of samples for each targeted class.
 
-spe_clf.fit(X_train, y_train, 
-            n_target_samples={
-                0: 80,
-                1: 200,
-                2: 400,
-            }, # target number of samples
-            **fit_kwargs)
+spe_clf.fit(
+    X_train,
+    y_train,
+    n_target_samples={
+        0: 80,
+        1: 200,
+        2: 400,
+    },  # target number of samples
+    **fit_kwargs
+)
 
-resampling_type='After under-sampling \n(target number {0: 80, 1: 200, 2: 400})'
+resampling_type = 'After under-sampling \n(target number {0: 80, 1: 200, 2: 400})'
 all_distribution[resampling_type] = spe_clf.target_distr_
 plot_class_distribution_comparison(spe_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # Over-sampling
 # ----------------------------
-# By default, over-sampling-based ensemble methods will consider the largest class as the majority class (class 2 with 600 samples).  
+# By default, over-sampling-based ensemble methods will consider the largest class as the majority class (class 2 with 600 samples).
 # All other classes (class 0 and 1) will be considered as minority classes and will be over-sampled until the number of samples is equalized.
 
 # %% [markdown]
 # **The over-sampling schedule can be customized in the same way as under-sampling.**
 
 # %% [markdown]
 # Take ``SMOTEBoostClassifier`` as example
@@ -189,55 +207,56 @@
 
 # %% [markdown]
 # **Train with the default under-sampling setting**
 
 smoteboost_clf.fit(X_train, y_train, **fit_kwargs)
 
 all_distribution['Before over-sampling'] = smoteboost_clf.origin_distr_
-resampling_type='After default over-sampling'
+resampling_type = 'After default over-sampling'
 all_distribution[resampling_type] = smoteboost_clf.target_distr_
 plot_class_distribution_comparison(smoteboost_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # **Specify the class targeted by the over-sampling**
 
-smoteboost_clf.fit(X_train, y_train, 
-                   target_label=1, # target class 1
-                   **fit_kwargs)
+smoteboost_clf.fit(X_train, y_train, target_label=1, **fit_kwargs)  # target class 1
 
-resampling_type='After over-sampling (target class 1)'
+resampling_type = 'After over-sampling (target class 1)'
 all_distribution[resampling_type] = smoteboost_clf.target_distr_
 plot_class_distribution_comparison(smoteboost_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # **Specify the desired number of samples after over-sampling**
 
-smoteboost_clf.fit(X_train, y_train, 
-                   n_target_samples=400, # target number of samples 400
-                   **fit_kwargs)
+smoteboost_clf.fit(
+    X_train, y_train, n_target_samples=400, **fit_kwargs  # target number of samples 400
+)
 
-resampling_type='After over-sampling (target number 400)'
+resampling_type = 'After over-sampling (target number 400)'
 all_distribution[resampling_type] = smoteboost_clf.target_distr_
 plot_class_distribution_comparison(smoteboost_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # **Specify the desired number of samples of each class after over-sampling**
 
-smoteboost_clf.fit(X_train, y_train, 
-                   n_target_samples={
-                       0: 200,
-                       1: 400,
-                       2: 600,
-                   }, # target number of samples
-                   **fit_kwargs)
+smoteboost_clf.fit(
+    X_train,
+    y_train,
+    n_target_samples={
+        0: 200,
+        1: 400,
+        2: 600,
+    },  # target number of samples
+    **fit_kwargs
+)
 
-resampling_type='After over-sampling \n(target number {0: 200, 1: 400, 2: 600})'
+resampling_type = 'After over-sampling \n(target number {0: 200, 1: 400, 2: 600})'
 all_distribution[resampling_type] = smoteboost_clf.target_distr_
 plot_class_distribution_comparison(smoteboost_clf, title2=resampling_type)
 
 
 # %% [markdown]
 # Visualize different resampling target
 # ---------------------------------------
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/classification/plot_sampling_schedule.py` & `imbalanced-ensemble-0.2.1/examples/classification/plot_sampling_schedule.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,34 +48,44 @@
 
 # %% [markdown]
 # Prepare data
 # ----------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 
 # %% [markdown]
 # Print the original class/marginal distribution P(Y) of the training data
 
 print('Original training dataset distribution %s' % sort_dict_by_key(Counter(y_train)))
 
 
 # %% [markdown]
 # Uniform under-sampling
 # ----------------------------
-# By default, under-sampling-based ensemble methods will consider the smallest class as the minority class (class 0 with 100 samples).  
-# All other classes (class 1 and 2) will be considered as majority classes and will be under-sampled until the number of samples is equalized.  
+# By default, under-sampling-based ensemble methods will consider the smallest class as the minority class (class 0 with 100 samples).
+# All other classes (class 1 and 2) will be considered as majority classes and will be under-sampled until the number of samples is equalized.
 
 # %% [markdown]
 # Take ``SelfPacedEnsembleClassifier`` as example
 
 spe_clf = imbens.ensemble.SelfPacedEnsembleClassifier(**init_kwargs)
 
 
@@ -84,81 +94,94 @@
 
 spe_clf.fit(X_train, y_train, **fit_kwargs)
 
 
 # %% [markdown]
 # Progressive under-sampling
 # ---------------------------
-# The resample class distributions are progressive 
+# The resample class distributions are progressive
 # interpolation between the original and the target class distribution.
-# Example: For a class :math:`c`, say the number of samples is :math:`N_{c}` 
-# and the target number of samples is :math:`N'_{c}`. Suppose that we are 
-# training the :math:`t`-th base estimator of a :math:`T`-estimator ensemble, then 
-# we expect to get :math:`(1-\frac{t}{T}) \cdot N_{c} + \frac{t}{T} \cdot N'_{c}` 
+# Example: For a class :math:`c`, say the number of samples is :math:`N_{c}`
+# and the target number of samples is :math:`N'_{c}`. Suppose that we are
+# training the :math:`t`-th base estimator of a :math:`T`-estimator ensemble, then
+# we expect to get :math:`(1-\frac{t}{T}) \cdot N_{c} + \frac{t}{T} \cdot N'_{c}`
 # samples after resampling;
 
 # %% [markdown]
 # **Train with progressive under-sampling schedule**
 
-spe_clf.fit(X_train, y_train,
-    balancing_schedule='progressive', # Progeressive under-sampling
-    **fit_kwargs
+spe_clf.fit(
+    X_train,
+    y_train,
+    balancing_schedule='progressive',  # Progeressive under-sampling
+    **fit_kwargs,
 )
 
 
 # %% [markdown]
-# Define your own resampling schedule. 
+# Define your own resampling schedule.
 # ------------------------------------
-# Your schedule function should take 4 positional arguments with order (``'origin_distr'``: 
-# ``dict``, ``'target_distr'``: ``dict``, ``'i_estimator'``: ``int``, ``'total_estimator'``: 
-# ``int``), and returns a ``'result_distr'``: ``dict``. For all parameters of type ``dict``, 
-# the keys of type ``int`` correspond to the targeted classes, and the values of type ``str`` 
+# Your schedule function should take 4 positional arguments with order (``'origin_distr'``:
+# ``dict``, ``'target_distr'``: ``dict``, ``'i_estimator'``: ``int``, ``'total_estimator'``:
+# ``int``), and returns a ``'result_distr'``: ``dict``. For all parameters of type ``dict``,
+# the keys of type ``int`` correspond to the targeted classes, and the values of type ``str``
 # correspond to the (desired) number of samples for each class.
 
 # %% [markdown]
 # **Train with user-defined dummy resampling schedule**
 
-def my_dummy_schedule(origin_distr:dict, target_distr:dict, 
-                      i_estimator:int, total_estimator:int):
+
+def my_dummy_schedule(
+    origin_distr: dict, target_distr: dict, i_estimator: int, total_estimator: int
+):
     '''A dummy resampling schedule'''
     return origin_distr
 
-spe_clf.fit(X_train, y_train,
-    balancing_schedule=my_dummy_schedule, # Use your progressive resampling schedule
-    **fit_kwargs
+
+spe_clf.fit(
+    X_train,
+    y_train,
+    balancing_schedule=my_dummy_schedule,  # Use your progressive resampling schedule
+    **fit_kwargs,
 )
 
 
 # %% [markdown]
 # **Train with user-defined progressive resampling schedule**
 
-def my_progressive_schedule(origin_distr:dict, target_distr:dict, 
-                            i_estimator:int, total_estimator:int):
+
+def my_progressive_schedule(
+    origin_distr: dict, target_distr: dict, i_estimator: int, total_estimator: int
+):
     '''A user-defined progressive resampling schedule'''
     # compute training progress
-    p = i_estimator / (total_estimator-1) if total_estimator >= 1 else 1
+    p = i_estimator / (total_estimator - 1) if total_estimator >= 1 else 1
     result_distr = {}
     # compute expected number of samples for each class
     for label in origin_distr.keys():
         result_distr[label] = math.ceil(
-            origin_distr[label] * (1-p) + target_distr[label] * p - 1e-10 # for numerical stability
+            origin_distr[label] * (1 - p)
+            + target_distr[label] * p
+            - 1e-10  # for numerical stability
         )
     return result_distr
 
 
-spe_clf.fit(X_train, y_train,
-    balancing_schedule=my_progressive_schedule, # Use your progressive resampling schedule
-    **fit_kwargs
+spe_clf.fit(
+    X_train,
+    y_train,
+    balancing_schedule=my_progressive_schedule,  # Use your progressive resampling schedule
+    **fit_kwargs,
 )
 
 
 # %% [markdown]
 # Over-sampling
 # ----------------------------
-# By default, over-sampling-based ensemble methods will consider the largest class as the majority class (class 2 with 600 samples).  
+# By default, over-sampling-based ensemble methods will consider the largest class as the majority class (class 2 with 600 samples).
 # All other classes (class 0 and 1) will be considered as minority classes and will be over-sampled until the number of samples is equalized.
 
 # %% [markdown]
 # **The over-sampling schedule can be customized in the same way as under-sampling.**
 
 # %% [markdown]
 # Take ``SMOTEBoostClassifier`` as example
@@ -176,48 +199,46 @@
 
 smoteboost_clf.fit(X_train, y_train, balancing_schedule='progressive', **fit_kwargs)
 
 
 # %% [markdown]
 # **Train with user-defined dummy resampling schedule**
 
-smoteboost_clf.fit(X_train, y_train,
-    balancing_schedule=my_dummy_schedule,
-    **fit_kwargs
-)
+smoteboost_clf.fit(X_train, y_train, balancing_schedule=my_dummy_schedule, **fit_kwargs)
 
 
 # %% [markdown]
 # **Train with user-defined progressive resampling schedule**
 
-smoteboost_clf.fit(X_train, y_train,
-    balancing_schedule=my_progressive_schedule,
-    **fit_kwargs
+smoteboost_clf.fit(
+    X_train, y_train, balancing_schedule=my_progressive_schedule, **fit_kwargs
 )
 
 
 # %% [markdown]
 # Visualize different resampling schedule
 # ---------------------------------------
 # Implement some plot utilities
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 from imbens.utils._plot import set_ax_border
 
 ylim = (0, 630)
 
-def plot_class_distribution(distr:dict, xlabel:str='Class Label', 
-                            ylabel:str='Number of samples', **kwargs):
+
+def plot_class_distribution(
+    distr: dict,
+    xlabel: str = 'Class Label',
+    ylabel: str = 'Number of samples',
+    **kwargs,
+):
     distr = dict(sorted(distr.items(), key=lambda k: k[0], reverse=True))
     ax = sns.barplot(
-        x=list(distr.keys()), 
-        y=list(distr.values()),
-        order=list(distr.keys()),
-        **kwargs
+        x=list(distr.keys()), y=list(distr.values()), order=list(distr.keys()), **kwargs
     )
     set_ax_border(ax)
     ax.grid(axis='y', alpha=0.5, ls='-.')
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     return ax
 
@@ -262,10 +283,13 @@
 
 # Progressive over-sampling
 for ax, i in zip(axes[1], i_estimators):
     resample_distr = _progressive_schedule(origin_distr, over_distr, i, N)
     plot_class_distribution(resample_distr, ax=ax)
     ax.set(ylim=ylim, title=f'After prog OS @Iter {i+1}/{N}')
 
-fig.suptitle("Abbreviation: prog: progressive; US: under-sampling; OS: over-sampling; Iter: iteration.", 
-             y=0.02, style='italic')
+fig.suptitle(
+    "Abbreviation: prog: progressive; US: under-sampling; OS: over-sampling; Iter: iteration.",
+    y=0.02,
+    style='italic',
+)
 fig.tight_layout()
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_generate_imbalance.py` & `imbalanced-ensemble-0.2.1/examples/datasets/plot_generate_imbalance.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 # %% [markdown]
 # Generate the dataset
 # --------------------
 #
 
 # %%
 X_train, X_test, y_train, y_test = generate_imbalance_data(
-    n_samples=1000, weights=[.7,.2,.1], test_size=.5,
+    n_samples=1000,
+    weights=[0.7, 0.2, 0.1],
+    test_size=0.5,
     kwargs={'n_informative': 3},
 )
 
-print ("Train class distribution: ", Counter(y_train))
-print ("Test class distribution:  ", Counter(y_test))
+print("Train class distribution: ", Counter(y_train))
+print("Test class distribution:  ", Counter(y_test))
 
 # %% [markdown]
 # Plot the generated (training) data
 # ----------------------------------
 #
 
 plot_2Dprojection_and_cardinality(X_train, y_train)
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance.py` & `imbalanced-ensemble-0.2.1/examples/datasets/plot_make_imbalance.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # License: MIT
 
 # %%
 print(__doc__)
 
 import matplotlib.pyplot as plt
 import seaborn as sns
+
 sns.set_context("poster")
 
 # %% [markdown]
 # Generate the dataset
 # --------------------
 #
 # First, we will generate a dataset and convert it to a
@@ -35,15 +36,15 @@
 from sklearn.datasets import make_moons
 
 X, y = make_moons(n_samples=200, shuffle=True, noise=0.25, random_state=10)
 X = pd.DataFrame(X, columns=["feature 1", "feature 2"])
 
 fig = plt.figure(figsize=(6, 5))
 ax = sns.scatterplot(
-    data=X, 
+    data=X,
     x="feature 1",
     y="feature 2",
     hue=y,
     style=y,
 )
 
 # %% [markdown]
@@ -65,15 +66,15 @@
 
 # %%
 from imbens.datasets import make_imbalance
 
 fig, axs = plt.subplots(nrows=2, ncols=3, figsize=(15, 10))
 
 sns.scatterplot(
-    data=X, 
+    data=X,
     x="feature 1",
     y="feature 2",
     hue=y,
     style=y,
     ax=axs[0, 0],
 )
 axs[0, 0].set_title("Original set")
@@ -82,17 +83,17 @@
 for ax, multiplier in zip(axs.ravel()[1:], multipliers):
     X_resampled, y_resampled = make_imbalance(
         X,
         y,
         sampling_strategy=ratio_func,
         **{"multiplier": multiplier, "minority_class": 1},
     )
-    
+
     sns.scatterplot(
-        data=X_resampled, 
+        data=X_resampled,
         x="feature 1",
         y="feature 2",
         hue=y_resampled,
         style=y_resampled,
         ax=ax,
     )
     ax.set_title(f"Sampling ratio = {multiplier}")
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/datasets/plot_make_imbalance_digits.py` & `imbalanced-ensemble-0.2.1/examples/datasets/plot_make_imbalance_digits.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,39 +50,80 @@
 
 fig = plot_2Dprojection_and_cardinality(X, y, figsize=(8, 4))
 
 
 # %% [markdown]
 # **Make class-imbalanced digits dataset**
 
-imbalance_distr = {0: 178, 1: 120, 2: 80, 3: 60, 4: 50, 5: 44, 6: 40, 7: 40, 8: 40, 9: 40}
-
-X_imb, y_imb = make_imbalance(X, y, sampling_strategy=imbalance_distr, random_state=RANDOM_STATE)
+imbalance_distr = {
+    0: 178,
+    1: 120,
+    2: 80,
+    3: 60,
+    4: 50,
+    5: 44,
+    6: 40,
+    7: 40,
+    8: 40,
+    9: 40,
+}
+
+X_imb, y_imb = make_imbalance(
+    X, y, sampling_strategy=imbalance_distr, random_state=RANDOM_STATE
+)
 
 fig = plot_2Dprojection_and_cardinality(X_imb, y_imb, figsize=(8, 4))
 
 
 # %% [markdown]
 # Use TSNE to compare the original & imbalanced Digits datasets
 # -------------------------------------------------------------
-# We can observe that it is more difficult to distinguish the tail classes from each other in the imbalanced Digits dataset.  
+# We can observe that it is more difficult to distinguish the tail classes from each other in the imbalanced Digits dataset.
 # These tailed classes are not well represented, thus it is harder for a learning model to learn their patterns.
 
 sns.set_context('talk')
 
-tsne = sklearn.manifold.TSNE(n_components=2, perplexity=100, n_iter=500, random_state=RANDOM_STATE)
+tsne = sklearn.manifold.TSNE(
+    n_components=2, perplexity=100, n_iter=500, random_state=RANDOM_STATE
+)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
 
 # Plot original digits data
-plot_scatter(tsne.fit_transform(X), y, title='Original Digits Data', weights=100, 
-             vis_params={'edgecolor': 'black', 'alpha': 0.8}, ax=ax1)
-ax1.legend(ncol=2, loc=2, columnspacing=0.01, borderaxespad=0.1, handletextpad=0.01, 
-           labelspacing=0.01, handlelength=None)
+plot_scatter(
+    tsne.fit_transform(X),
+    y,
+    title='Original Digits Data',
+    weights=100,
+    vis_params={'edgecolor': 'black', 'alpha': 0.8},
+    ax=ax1,
+)
+ax1.legend(
+    ncol=2,
+    loc=2,
+    columnspacing=0.01,
+    borderaxespad=0.1,
+    handletextpad=0.01,
+    labelspacing=0.01,
+    handlelength=None,
+)
 
 # Plot imbalanced digits data
-plot_scatter(tsne.fit_transform(X_imb), y_imb, title='Imbalanced Digits Data', weights=100, 
-             vis_params={'edgecolor': 'black', 'alpha': 0.8}, ax=ax2)
-ax2.legend(ncol=2, loc=2, columnspacing=0.01, borderaxespad=0.1, handletextpad=0.01, 
-           labelspacing=0.01, handlelength=None)
+plot_scatter(
+    tsne.fit_transform(X_imb),
+    y_imb,
+    title='Imbalanced Digits Data',
+    weights=100,
+    vis_params={'edgecolor': 'black', 'alpha': 0.8},
+    ax=ax2,
+)
+ax2.legend(
+    ncol=2,
+    loc=2,
+    columnspacing=0.01,
+    borderaxespad=0.1,
+    handletextpad=0.01,
+    labelspacing=0.01,
+    handlelength=None,
+)
 
 fig.tight_layout()
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_classification_report.py` & `imbalanced-ensemble-0.2.1/examples/evaluation/plot_classification_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Specific metrics have been developed to evaluate classifier which has been
 trained using imbalanced data. "mod:`imbens` provides a classification report
 (:func:`imbens.metrics.classification_report_imbalanced`) 
 similar to :mod:`sklearn`, with additional metrics specific to imbalanced
 learning problem.
 """
 
-# Adapted from imbalanced-learn 
+# Adapted from imbalanced-learn
 # Authors: Guillaume Lemaitre
 # License: MIT
 
 from sklearn import datasets
 from sklearn.svm import LinearSVC
 from sklearn.model_selection import train_test_split
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/evaluation/plot_metrics.py` & `imbalanced-ensemble-0.2.1/examples/evaluation/plot_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Specific metrics have been developed to evaluate classifier which
 has been trained using imbalanced data. :mod:`imbens` provides mainly
 two additional metrics which are not implemented in :mod:`sklearn`: (i)
 geometric mean (:func:`imbens.metrics.geometric_mean_score`) 
 and (ii) index balanced accuracy (:func:`imbens.metrics.make_index_balanced_accuracy`).
 """
 
-# Adapted from imbalanced-learn 
+# Adapted from imbalanced-learn
 # Authors: Guillaume Lemaitre
 # License: MIT
 
 # %%
 print(__doc__)
 
 RANDOM_STATE = 42
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/pipeline/plot_pipeline_classification.py` & `imbalanced-ensemble-0.2.1/examples/pipeline/plot_pipeline_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 :func:`~imbens.pipeline.make_pipeline` helper function) working with
 transformers (:class:`~sklearn.decomposition.PCA`, 
 :class:`~sklearn.neighbors.KNeighborsClassifier` from *scikit-learn*) and resamplers
 (:class:`~imbens.sampler.EditedNearestNeighbours`, 
 :class:`~imbens.sampler.SMOTE`).
 """
 
-# Adapted from imbalanced-learn 
+# Adapted from imbalanced-learn
 # Authors: Christos Aridas
 #          Guillaume Lemaitre
 # License: MIT
 
 # %%
 print(__doc__)
 
@@ -40,15 +40,15 @@
     n_samples=5000,
     random_state=10,
 )
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, stratify=y, random_state=42)
 
 # %% [markdown]
-# Now, we will create each individual steps 
+# Now, we will create each individual steps
 # that we would like later to combine
 
 # %%
 from sklearn.decomposition import PCA
 from sklearn.neighbors import KNeighborsClassifier
 from imbens.sampler import EditedNearestNeighbours
 from imbens.sampler import SMOTE
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_confusion_matrix.py` & `imbalanced-ensemble-0.2.1/examples/visualizer/plot_confusion_matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,21 +39,31 @@
 
 # %% [markdown]
 # Prepare data
 # ----------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # %% [markdown]
 # Train ensemble classifiers
 # --------------------------
 # 4 different ensemble classifiers are used.
 
 init_kwargs = {'n_estimators': 50, 'random_state': RANDOM_STATE}
@@ -70,60 +80,58 @@
 # Train all ensemble classifiers, store the results in fitted_ensembles
 fitted_ensembles = {}
 for clf_name, clf in ensemble_dict.items():
     start_time = time()
     clf.fit(**fit_kwargs)
     fit_time = time() - start_time
     fitted_ensembles[clf_name] = clf
-    print ('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
+    print('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
 
 
 # %% [markdown]
 # Fit an ``ImbalancedEnsembleVisualizer``
 # -----------------------------------------------------
-# The visualizer fits on a ``dictionary`` like {..., ensemble_name: ensemble_classifier, ...}  
-# The keys should be strings corresponding to ensemble names.   
+# The visualizer fits on a ``dictionary`` like {..., ensemble_name: ensemble_classifier, ...}
+# The keys should be strings corresponding to ensemble names.
 # The values should be fitted ``imbalance_ensemble.ensemble`` or ``sklearn.ensemble`` estimator objects.
 
 # Initialize visualizer
 visualizer = imbens.visualizer.ImbalancedEnsembleVisualizer(
-    eval_datasets = {
-        'training' : (X_train, y_train),
-        'validation' : (X_valid, y_valid),
+    eval_datasets={
+        'training': (X_train, y_train),
+        'validation': (X_valid, y_valid),
     },
-    eval_metrics = {
+    eval_metrics={
         'acc': (sklearn.metrics.accuracy_score, {}),
         'balanced_acc': (sklearn.metrics.balanced_accuracy_score, {}),
-        'weighted_f1': (sklearn.metrics.f1_score, {'average':'weighted'}),
+        'weighted_f1': (sklearn.metrics.f1_score, {'average': 'weighted'}),
     },
 )
 
 # Fit visualizer
 visualizer.fit(fitted_ensembles)
 
 
 # %% [markdown]
 # Plot confusion matrices
 # -----------------------
 
 fig, axes = visualizer.confusion_matrix_heatmap()
 
 
-
 # %% [markdown]
 # False predictions only
 # -----------------------
 # (parameter ``false_pred_only``: bool)
 
 fig, axes = visualizer.confusion_matrix_heatmap(
     false_pred_only=True,
 )
 
 
-
 # %% [markdown]
 # Select results for visualization
 # --------------------------------
 # (parameter ``on_ensembles``: list of ensemble name, ``on_datasets``: list of dataset name)
 
 # %% [markdown]
 # **Select: method ('SPE', 'BalanceForest'), data ('validation')**
@@ -138,18 +146,16 @@
 # Customize visual appearance
 # ---------------------------
 # (parameter ``sub_figsize``: tuple, ``sup_title``: bool or string, kwargs of ``seaborn.heatmap()``)
 
 fig, axes = visualizer.confusion_matrix_heatmap(
     on_ensembles=['SPE', 'BalanceForest'],
     on_datasets=['training', 'validation'],
-    
     # Customize visual appearance
     sub_figsize=(4, 3.3),
     sup_title='My Suptitle',
-    
     # arguments pass down to seaborn.heatmap()
     cmap='YlOrRd',
     cbar=True,
     linewidths=10,
     vmax=20,
-)
+)
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/auto_examples/visualizer/plot_performance_curve.py` & `imbalanced-ensemble-0.2.1/examples/visualizer/plot_performance_curve.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,21 +40,31 @@
 
 # %% [markdown]
 # Prepare data
 # ----------------------------
 # Make a toy 3-class imbalanced classification task.
 
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 
 # train valid split
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
 # %% [markdown]
 # Train ensemble classifiers
 # --------------------------
 # 4 different ensemble classifiers are used.
 
 init_kwargs = {'n_estimators': 50, 'random_state': RANDOM_STATE}
@@ -71,34 +81,34 @@
 # Train all ensemble classifiers, store the results in fitted_ensembles
 fitted_ensembles = {}
 for clf_name, clf in ensemble_dict.items():
     start_time = time()
     clf.fit(**fit_kwargs)
     fit_time = time() - start_time
     fitted_ensembles[clf_name] = clf
-    print ('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
+    print('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
 
 
 # %% [markdown]
 # Fit an ``ImbalancedEnsembleVisualizer``
 # -----------------------------------------------------
-# The visualizer fits on a ``dictionary`` like {..., ensemble_name: ensemble_classifier, ...}  
-# The keys should be strings corresponding to ensemble names.   
+# The visualizer fits on a ``dictionary`` like {..., ensemble_name: ensemble_classifier, ...}
+# The keys should be strings corresponding to ensemble names.
 # The values should be fitted ``imbalance_ensemble.ensemble`` or ``sklearn.ensemble`` estimator objects.
 
 # Initialize visualizer
 visualizer = imbens.visualizer.ImbalancedEnsembleVisualizer(
-    eval_datasets = {
-        'training' : (X_train, y_train),
-        'validation' : (X_valid, y_valid),
+    eval_datasets={
+        'training': (X_train, y_train),
+        'validation': (X_valid, y_valid),
     },
-    eval_metrics = {
+    eval_metrics={
         'acc': (sklearn.metrics.accuracy_score, {}),
         'balanced_acc': (sklearn.metrics.balanced_accuracy_score, {}),
-        'weighted_f1': (sklearn.metrics.f1_score, {'average':'weighted'}),
+        'weighted_f1': (sklearn.metrics.f1_score, {'average': 'weighted'}),
     },
 )
 
 # Fit visualizer
 visualizer.fit(fitted_ensembles)
 
 
@@ -145,19 +155,17 @@
 # (parameter ``sub_figsize``: tuple, ``sup_title``: bool or string, kwargs of ``seaborn.lineplot()``)
 
 fig, axes = visualizer.performance_lineplot(
     on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
     on_datasets=['training', 'validation'],
     on_metrics=['balanced_acc', 'weighted_f1'],
     n_samples_as_x_axis=True,
-    
     # Customize visual appearance
     sub_figsize=(3, 4),
     sup_title='My Suptitle',
-    
     # arguments pass down to seaborn.lineplot()
     linewidth=3,
     markers=True,
     alpha=0.8,
 )
 
 
@@ -171,24 +179,22 @@
 
 fig, axes = visualizer.performance_lineplot(
     on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
     on_datasets=['training', 'validation'],
     on_metrics=['balanced_acc', 'weighted_f1'],
     n_samples_as_x_axis=True,
     sub_figsize=(3, 2.3),
-    
-    split_by=['dataset'], # Group results by dataset
+    split_by=['dataset'],  # Group results by dataset
 )
 
 
 # %% [markdown]
 # **Group results by method**
 
 fig, axes = visualizer.performance_lineplot(
     on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
     on_datasets=['training', 'validation'],
     on_metrics=['balanced_acc', 'weighted_f1'],
     n_samples_as_x_axis=True,
     sub_figsize=(3, 2.3),
-    
-    split_by=['method'], # Group results by method
+    split_by=['method'],  # Group results by method
 )
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/conf.py` & `imbalanced-ensemble-0.2.1/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 import os
 import sys
 from os.path import abspath, dirname
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-
 sys.path.insert(0, dirname(dirname(dirname(abspath(__file__)))))
-# sys.path.insert(0, abspath("sphinxext"))
-# from github_link import make_linkcode_resolve
+sys.path.insert(0, abspath("sphinxext"))
+from github_link import make_linkcode_resolve
 
 # -- Project information -----------------------------------------------------
 
 project = 'imbalanced-ensemble'
 copyright = '2021, Zhining Liu'
 author = 'Zhining Liu'
 
@@ -37,15 +36,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     "sphinx.ext.autosummary",
     # "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
-    # "sphinx.ext.linkcode",
+    "sphinx.ext.linkcode",
     # "sphinxcontrib.bibtex",
     "numpydoc",
     # "sphinx_issues",
     "sphinx_gallery.gen_gallery",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
@@ -66,56 +65,58 @@
 # generate autosummary even if no references
 autosummary_generate = True
 
 # -- Options for numpydoc -----------------------------------------------------
 
 # this is needed for some reason...
 # see https://github.com/numpy/numpydoc/issues/69
-numpydoc_show_class_members = False 
+numpydoc_show_class_members = False
 
 # -- Options for sphinx-gallery -----------------------------------------------
 
 # Generate the plot for the gallery
 plot_gallery = True
 
 # sphinx-gallery configuration
 sphinx_gallery_conf = {
-    'examples_dirs': ['../../examples'],
-    'gallery_dirs': ['auto_examples'],
+    "examples_dirs": ["../../examples"],
+    "gallery_dirs": ["auto_examples"],
     "doc_module": (
-        "imbens", 
+        "imbens",
         "imbens.ensemble",
     ),
     "backreferences_dir": os.path.join("back_references"),
     "show_memory": True,
     "reference_url": {"imbalanced-ensemble": None},
+    "nested_sections": False,
 }
 
 # # -- Options for github link for what's new -----------------------------------
 
-# # Config for sphinx_issues
+# Config for sphinx_issues
 # issues_uri = "https://github.com/ZhiningLiu1998/imbalanced-ensemble/issues/{issue}"
 # issues_github_path = "ZhiningLiu1998/imbalanced-ensemble"
 # issues_user_uri = "https://github.com/{user}"
 
-# # The following is used by sphinx.ext.linkcode to provide links to github
-# linkcode_resolve = make_linkcode_resolve(
-#     "imbalanced-ensemble",
-#     "https://github.com/ZhiningLiu1998/"
-#     "imbalanced-ensemble/blob/{revision}/"
-#     "{package}/{path}#L{lineno}",
-# )
+# The following is used by sphinx.ext.linkcode to provide links to github
+linkcode_resolve = make_linkcode_resolve(
+    "imbens",
+    "https://github.com/ZhiningLiu1998/"
+    "imbalanced-ensemble/blob/{revision}/"
+    "{package}/{path}#L{lineno}",
+)
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+
 def setup(app):
-    app.add_css_file('css/my_theme.css')
+    app.add_css_file('css/my_theme.css')
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/get_start.rst` & `imbalanced-ensemble-0.2.1/docs/source/get_start.rst`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/index.rst` & `imbalanced-ensemble-0.2.1/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -73,20 +73,20 @@
 **Date**: |today| **Version**: |version|
 
 **Paper**: `IMBENS: Ensemble Class-imbalanced Learning in Python <https://arxiv.org/abs/2111.12776>`_
 
 **Citing US**
 
 If you find IMBENS helpful in your work or research, we would greatly appreciate citations to the following paper [`PDF <(https://arxiv.org/pdf/2111.12776.pdf>`_]::
-
-   @article{liu2021imbens,
+   
+   @article{liu2023imbens,
       title={IMBENS: Ensemble Class-imbalanced Learning in Python},
-      author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi},
+      author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
       journal={arXiv preprint arXiv:2111.12776},
-      year={2021}
+      year={2023}
    }
 
 
 **imbalanced-ensemble** (IMBENS, imported as ``imbens``) is a Python toolbox 
 for quick implementation, modification, evaluation, and visualization of ensemble learning 
 algorithms for class-imbalanced data.
 It was built on the basis of `scikit-learn <https://scikit-learn.org/stable/index.html>`__
@@ -148,16 +148,18 @@
    api/sampler/api
    api/visualizer/api
    api/pipeline/api
    api/datasets/api
    api/metrics/api
    api/utils/api
 
+
 .. toctree::
-   :maxdepth: 3
+   :hidden:
+   :maxdepth: 0
    :caption: Examples
 
    auto_examples/index
 
 .. toctree::
    :maxdepth: 3
    :caption: History
```

#### html2text {}

```diff
@@ -21,23 +21,21 @@
 .. raw:: html
 **** [Github] [Gallery] [PyPI] [Changelog] [Source] [Download] [ç¥ä¹/Zhihu]
 [ä¸­æREADME] [arXiv] ****
 **Date**: |today| **Version**: |version| **Paper**: `IMBENS: Ensemble Class-
 imbalanced Learning in Python
 arxiv.org/abs/2111.12776>`_ **Citing US** If you find IMBENS helpful in your
 work or research, we would greatly appreciate citations to the following paper
-[`PDF <(https://arxiv.org/pdf/2111.12776.pdf>`_]:: @article{liu2021imbens,
+[`PDF <(https://arxiv.org/pdf/2111.12776.pdf>`_]:: @article{liu2023imbens,
 title={IMBENS: Ensemble Class-imbalanced Learning in Python}, author={Liu,
-Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang and Guo, Kai and Yu,
-Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and Bian, Jiang and Wei,
-Pengfei and Jiang, Jing and Chang, Yi}, journal={arXiv preprint arXiv:
-2111.12776}, year={2021} } **imbalanced-ensemble** (IMBENS, imported as
-``imbens``) is a Python toolbox for quick implementation, modification,
-evaluation, and visualization of ensemble learning algorithms for class-
-imbalanced data. It was built on the basis of `scikit-learn
+Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi}, journal={arXiv
+preprint arXiv:2111.12776}, year={2023} } **imbalanced-ensemble** (IMBENS,
+imported as ``imbens``) is a Python toolbox for quick implementation,
+modification, evaluation, and visualization of ensemble learning algorithms for
+class-imbalanced data. It was built on the basis of `scikit-learn
 scikit-learn.org/stable/index.html>`__ and `imbalanced-learn
 imbalanced-learn.org/stable/>`__. IMBENS includes more than 15 ensemble
 imbalanced learning (EIL) algorithms, from the classical SMOTEBoost (2003) and
 RUSBoost (2010) to recent SPE (2020), from resampling-based methods to cost-
 sensitive ensemble learning. **IMBENS is featured for:** - Unified, easy-to-use
 APIs, detailed `documentation
 imbalanced-ensemble.readthedocs.io/>`_ and `examples
@@ -61,9 +59,9 @@
 Gmean: 0.972 >>> >>> visualizer = ImbalancedEnsembleVisualizer() # initialize
 visualizer >>> visualizer.fit({'SPE': clf}) >>> >>>
 visualizer.performance_lineplot() # performance visualization >>>
 visualizer.confusion_matrix_heatmap() # prediction visualization .. toctree:: :
 maxdepth: 3 :caption: Getting Started get_start install .. toctree:: :maxdepth:
 2 :caption: API api/ensemble/api api/sampler/api api/visualizer/api api/
 pipeline/api api/datasets/api api/metrics/api api/utils/api .. toctree:: :
-maxdepth: 3 :caption: Examples auto_examples/index .. toctree:: :maxdepth: 3 :
-caption: History release_history
+hidden: :maxdepth: 0 :caption: Examples auto_examples/index .. toctree:: :
+maxdepth: 3 :caption: History release_history
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/install.rst` & `imbalanced-ensemble-0.2.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/release_history.rst` & `imbalanced-ensemble-0.2.1/docs/source/release_history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 Release History
 ***************
 
-Version 0.1.8 (2023.02)
+Version 0.2.1 (2023.07)
 =========================
 
-Enhancement:
+Maintenance:
 
-- Add unit test for all ensemble classifiers and samplers.
-- Following sklearn version >1.2, for all ensemble classifiers, 
+- Bump supported scikit-learn version to ``1.3.0``.
+- Update requirements for building documentation with ``sphinx``.
+- Remove redundant doc (``auto_examples`` and ``back_references``) files in the source distribution.
 
-  - the parameter ``base_estimator`` is renamed to ``estimator``.
-  - the attribute ``base_estimator_`` is renamed to ``estimator_``.
+Bug Fixes:
+
+- Fix ``AttributeError`` in :class:`imbens.ensemble.BalancedRandomForestClassifier`.
+- Fix several bugs encountered in CI.
+
+Version 0.2.0 (2023.02)
+=========================
+
+Enhancement:
+
+- Enable CircleCI with CodeCov report.
+- Easier usage:
+  
+  - the package is now imported as ``imbens``
+  - all samplers can be directly accessed in ``imbens.sampler``
 
 Maintenance:
 
+- Complement unit tests (59% -> 96% coverage).
 - Set default ``k_neighbors=1`` for SMOTEBagging to prevent error in few-shot cases.
 - Set default ``cluster_balance_threshold=0.1`` for KmeansSMOTEBoost to prevent error in few-shot cases.
-- Add ``decision_function()`` for supported ensembles.
+- Add ``decision_function()`` for supported ensemble classifiers.
 - The parameter ``base_sampler`` is renamed to ``sampler``.
 - The attribute ``base_sampler_`` is renamed to ``sampler_``.
 - Bump supported Python version to ``3.8, 3.9, 3.10, 3.11``.
+- Following sklearn version >1.2, for all ensemble classifiers, 
+
+  - the parameter ``base_estimator`` is renamed to ``estimator``.
+  - the attribute ``base_estimator_`` is renamed to ``estimator_``.
 
 Bug Fixes:
 
 - Add missing comma in the INSTALL_REQUIRES list which breaks ``conda env export``.
 - Fix ``BalanceCascade`` and ``SelfPacedEnsemble``'s ``_make_sampler()`` behaviour.
 - Fix ``BalanceCascade`` and ``SelfPacedEnsemble`` parameter check.
 - Fix cost_matrix type check for cost-sensitive methods
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/sphinxext/LICENSE.txt` & `imbalanced-ensemble-0.2.1/docs/source/sphinxext/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/sphinxext/README.txt` & `imbalanced-ensemble-0.2.1/docs/source/sphinxext/README.txt`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/docs/source/sphinxext/github_link.py` & `imbalanced-ensemble-0.2.1/docs/source/sphinxext/github_link.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+# %%
+
 from operator import attrgetter
 import inspect
 import subprocess
 import os
 import sys
 from functools import partial
 
 REVISION_CMD = "git rev-parse --short HEAD"
 
+# %%
+
 
 def _get_git_revision():
     try:
         revision = subprocess.check_output(REVISION_CMD.split()).strip()
     except (subprocess.CalledProcessError, OSError):
         print("Failed to execute git to get revision")
         return None
@@ -42,29 +46,39 @@
     class_name = info["fullname"].split(".")[0]
     if type(class_name) != str:
         # Python 2 only
         class_name = class_name.encode("utf-8")
     module = __import__(info["module"], fromlist=[class_name])
     obj = attrgetter(info["fullname"])(module)
 
+    # try:
+    #     fn = inspect.getsourcefile(obj)
+    # except Exception:
+    #     fn = None
+    # if not fn:
+    #     try:
+    #         fn = inspect.getsourcefile(sys.modules[obj.__module__])
+    #     except Exception:
+    #         fn = None
     try:
-        fn = inspect.getsourcefile(obj)
+        fn = inspect.getsourcefile(sys.modules[obj.__module__])
     except Exception:
         fn = None
     if not fn:
-        try:
-            fn = inspect.getsourcefile(sys.modules[obj.__module__])
-        except Exception:
-            fn = None
-    if not fn:
         return
 
     fn = os.path.relpath(fn, start=os.path.dirname(__import__(package).__file__))
     try:
-        lineno = inspect.getsourcelines(obj)[1]
+        src_code_lines, lineno = inspect.getsourcelines(obj)
+        i = 0
+        for l in src_code_lines:
+            if 'def' in l or 'class' in l:
+                break
+            i += 1
+        lineno += i
     except Exception:
         lineno = ""
     return url_fmt.format(revision=revision, package=package, path=fn, lineno=lineno)
 
 
 def make_linkcode_resolve(package, url_fmt):
     """Returns a linkcode_resolve function for the given URL format
@@ -77,7 +91,19 @@
                                    'blob/{revision}/{package}/'
                                    '{path}#L{lineno}')
     """
     revision = _get_git_revision()
     return partial(
         _linkcode_resolve, revision=revision, package=package, url_fmt=url_fmt
     )
+
+
+# %%
+
+linkcode_resolve = make_linkcode_resolve(
+    "imbens",
+    "https://github.com/ZhiningLiu1998/"
+    "imbalanced-ensemble/blob/{revision}/"
+    "{package}/{path}#L{lineno}",
+)
+
+linkcode_resolve
```

### Comparing `imbalanced-ensemble-0.2.0/docs/source/sphinxext/sphinx_issues.py` & `imbalanced-ensemble-0.2.1/docs/source/sphinxext/sphinx_issues.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/examples/visualizer/plot_performance_curve.py` & `imbalanced-ensemble-0.2.1/imbens/visualizer/tests/test_visualizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,183 @@
-"""
-=========================================================
-Plot performance curves
-=========================================================
-
-This example illustrates how to use the 
-:mod:`imbens.visualizer` module to visualize or 
-compare :mod:`imbens.ensemble` classifier(s).
-
-This example uses:
-
-    - :class:`imbens.ensemble.SelfPacedEnsembleClassifier`
-    - :class:`imbens.ensemble.EasyEnsembleClassifier`
-    - :class:`imbens.ensemble.BalancedRandomForestClassifier`
-    - :class:`imbens.ensemble.SMOTEBaggingClassifier`
-    - :class:`imbens.visualizer.ImbalancedEnsembleVisualizer`
-"""
+"""Test visualizer."""
 
 # Authors: Zhining Liu <zhining.liu@outlook.com>
 # License: MIT
 
 
-# %%
-print(__doc__)
-
+import pytest
+import numpy as np
+import matplotlib.pyplot as plt
 from time import time
-
-# Import imbalanced-ensemble
-import imbens
-
-# Import utilities from sklearn
 import sklearn
 from sklearn.datasets import make_classification
-from sklearn.model_selection import train_test_split
-
-RANDOM_STATE = 42
-
-# sphinx_gallery_thumbnail_number = 4
+from sklearn.model_selection import ParameterGrid, train_test_split
 
+import imbens
 
-# %% [markdown]
-# Prepare data
-# ----------------------------
-# Make a toy 3-class imbalanced classification task.
 
+RANDOM_STATE = 42
 # make dataset
-X, y = make_classification(n_classes=3, class_sep=2,
-    weights=[0.1, 0.3, 0.6], n_informative=3, n_redundant=1, flip_y=0,
-    n_features=20, n_clusters_per_class=2, n_samples=2000, random_state=0)
-
-# train valid split
+X, y = make_classification(
+    n_classes=3,
+    class_sep=2,
+    weights=[0.1, 0.3, 0.6],
+    n_informative=3,
+    n_redundant=1,
+    flip_y=0,
+    n_features=20,
+    n_clusters_per_class=2,
+    n_samples=2000,
+    random_state=0,
+)
 X_train, X_valid, y_train, y_valid = train_test_split(
-    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE)
+    X, y, test_size=0.5, stratify=y, random_state=RANDOM_STATE
+)
 
-# %% [markdown]
-# Train ensemble classifiers
-# --------------------------
-# 4 different ensemble classifiers are used.
 
+# Train all ensemble classifiers, store the results in fitted_ensembles
 init_kwargs = {'n_estimators': 50, 'random_state': RANDOM_STATE}
 fit_kwargs = {'X': X_train, 'y': y_train}
-
-# imbens.ensemble classifiers
 ensemble_dict = {
     'SPE': imbens.ensemble.SelfPacedEnsembleClassifier(**init_kwargs),
     'EasyEns': imbens.ensemble.EasyEnsembleClassifier(**init_kwargs),
     'BalanceForest': imbens.ensemble.BalancedRandomForestClassifier(**init_kwargs),
     'SMOTEBagging': imbens.ensemble.SMOTEBaggingClassifier(**init_kwargs),
 }
-
-# Train all ensemble classifiers, store the results in fitted_ensembles
 fitted_ensembles = {}
 for clf_name, clf in ensemble_dict.items():
     start_time = time()
     clf.fit(**fit_kwargs)
     fit_time = time() - start_time
     fitted_ensembles[clf_name] = clf
-    print ('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
-
+    print('Training {:^30s} | Time used: {:.3f}s'.format(clf.__name__, fit_time))
 
-# %% [markdown]
-# Fit an ``ImbalancedEnsembleVisualizer``
-# -----------------------------------------------------
-# The visualizer fits on a ``dictionary`` like {..., ensemble_name: ensemble_classifier, ...}  
-# The keys should be strings corresponding to ensemble names.   
-# The values should be fitted ``imbalance_ensemble.ensemble`` or ``sklearn.ensemble`` estimator objects.
-
-# Initialize visualizer
 visualizer = imbens.visualizer.ImbalancedEnsembleVisualizer(
-    eval_datasets = {
-        'training' : (X_train, y_train),
-        'validation' : (X_valid, y_valid),
+    eval_datasets={
+        'training': (X_train, y_train),
+        'validation': (X_valid, y_valid),
     },
-    eval_metrics = {
+    eval_metrics={
         'acc': (sklearn.metrics.accuracy_score, {}),
         'balanced_acc': (sklearn.metrics.balanced_accuracy_score, {}),
-        'weighted_f1': (sklearn.metrics.f1_score, {'average':'weighted'}),
+        'weighted_f1': (sklearn.metrics.f1_score, {'average': 'weighted'}),
     },
 )
-
 # Fit visualizer
 visualizer.fit(fitted_ensembles)
 
 
-# %% [markdown]
-# Plot performance curve
-# ----------------------
-# **Performance w.r.t. number of base estimators**
-
-fig, axes = visualizer.performance_lineplot()
-
-
-# %% [markdown]
-# Set x-axis
-# ----------
-# (parameter ``n_samples_as_x_axis``: bool)
-
-# %% [markdown]
-# **Performance w.r.t. number of training samples**
-
-fig, axes = visualizer.performance_lineplot(
-    n_samples_as_x_axis=True,
-)
-
-
-# %% [markdown]
-# Select results for visualization
-# --------------------------------
-# (parameter ``on_ensembles``: list of ensemble name, ``on_datasets``: list of dataset name, ``on_metrics``: list of metric name)
-
-# %% [markdown]
-# **Select: method ('SPE', 'SMOTEBagging'), data ('validation'), metric ('balanced_acc', 'weighted_f1')**
-
-fig, axes = visualizer.performance_lineplot(
-    on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
-    on_datasets=['validation'],
-    on_metrics=['balanced_acc', 'weighted_f1'],
-    n_samples_as_x_axis=True,
-)
-
-
-# %% [markdown]
-# Customize visual appearance
-# ---------------------------
-# (parameter ``sub_figsize``: tuple, ``sup_title``: bool or string, kwargs of ``seaborn.lineplot()``)
-
-fig, axes = visualizer.performance_lineplot(
-    on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
-    on_datasets=['training', 'validation'],
-    on_metrics=['balanced_acc', 'weighted_f1'],
-    n_samples_as_x_axis=True,
-    
+def test_performance_curve():
+    # Performance w.r.t. number of base estimators
+    fig, axes = visualizer.performance_lineplot()
+    # Performance w.r.t. number of training samples
+    fig, axes = visualizer.performance_lineplot(
+        n_samples_as_x_axis=True,
+    )
+    # Select results for visualization
+    fig, axes = visualizer.performance_lineplot(
+        on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
+        on_datasets=['validation'],
+        on_metrics=['balanced_acc', 'weighted_f1'],
+        n_samples_as_x_axis=True,
+    )
+    # Custom visualization
+    fig, axes = visualizer.performance_lineplot(
+        on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
+        on_datasets=['training', 'validation'],
+        on_metrics=['balanced_acc', 'weighted_f1'],
+        n_samples_as_x_axis=True,
+        # Customize visual appearance
+        sub_figsize=(3, 4),
+        sup_title='My Suptitle',
+        # arguments pass down to seaborn.lineplot()
+        linewidth=3,
+        markers=True,
+        alpha=0.8,
+    )
+    # Group results by dataset
+    fig, axes = visualizer.performance_lineplot(
+        on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
+        on_datasets=['training', 'validation'],
+        on_metrics=['balanced_acc', 'weighted_f1'],
+        n_samples_as_x_axis=True,
+        sub_figsize=(3, 2.3),
+        split_by=['dataset'],  # Group results by dataset
+    )
+    # Group results by method
+    fig, axes = visualizer.performance_lineplot(
+        on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
+        on_datasets=['training', 'validation'],
+        on_metrics=['balanced_acc', 'weighted_f1'],
+        n_samples_as_x_axis=True,
+        sub_figsize=(3, 2.3),
+        split_by=['method'],  # Group results by method
+    )
+
+
+def test_confusion_matrix_heatmap():
+    fig, axes = visualizer.confusion_matrix_heatmap()
+    # False predictions only
+    fig, axes = visualizer.confusion_matrix_heatmap(
+        false_pred_only=True,
+    )
+    # Select: method ('SPE', 'BalanceForest'), data ('validation')
+    fig, axes = visualizer.confusion_matrix_heatmap(
+        on_ensembles=['SPE', 'BalanceForest'],
+        on_datasets=['validation'],
+    )
     # Customize visual appearance
-    sub_figsize=(3, 4),
-    sup_title='My Suptitle',
-    
-    # arguments pass down to seaborn.lineplot()
-    linewidth=3,
-    markers=True,
-    alpha=0.8,
-)
-
-
-# %% [markdown]
-# Group results
-# -------------
-# (parameter ``split_by``: list of {'method', 'dataset'})
-
-# %% [markdown]
-# **Group results by dataset**
-
-fig, axes = visualizer.performance_lineplot(
-    on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
-    on_datasets=['training', 'validation'],
-    on_metrics=['balanced_acc', 'weighted_f1'],
-    n_samples_as_x_axis=True,
-    sub_figsize=(3, 2.3),
-    
-    split_by=['dataset'], # Group results by dataset
-)
-
-
-# %% [markdown]
-# **Group results by method**
-
-fig, axes = visualizer.performance_lineplot(
-    on_ensembles=['SPE', 'EasyEns', 'BalanceForest'],
-    on_datasets=['training', 'validation'],
-    on_metrics=['balanced_acc', 'weighted_f1'],
-    n_samples_as_x_axis=True,
-    sub_figsize=(3, 2.3),
-    
-    split_by=['method'], # Group results by method
+    fig, axes = visualizer.confusion_matrix_heatmap(
+        on_ensembles=['SPE', 'BalanceForest'],
+        on_datasets=['training', 'validation'],
+        # Customize visual appearance
+        sub_figsize=(4, 3.3),
+        sup_title='My Suptitle',
+        # arguments pass down to seaborn.heatmap()
+        cmap='YlOrRd',
+        cbar=True,
+        linewidths=10,
+        vmax=20,
+    )
+
+
+@pytest.mark.parametrize(
+    "vis_params",
+    ParameterGrid(
+        {
+            "on_ensembles": [
+                ['SPE'],
+            ],
+            "on_datasets": [
+                ['validation'],
+            ],
+            "on_metrics": [
+                ['acc'],
+            ],
+            "n_samples_as_x_axis": [False, True],
+            "split_by": [
+                ['method'],
+                ['method', 'dataset'],
+            ],
+        }
+    ),
+)
+def test_performance_curve_grid(vis_params):
+    fig, axes = visualizer.performance_lineplot(**vis_params)
+
+
+@pytest.mark.parametrize(
+    "vis_params",
+    ParameterGrid(
+        {
+            "on_ensembles": [
+                ['SPE'],
+            ],
+            "on_datasets": [
+                ['validation'],
+            ],
+            "false_pred_only": [False, True],
+        }
+    ),
 )
+def test_confusion_matrix_heatmap_grid(vis_params):
+    fig, axes = visualizer.confusion_matrix_heatmap(**vis_params)
```

### Comparing `imbalanced-ensemble-0.2.0/imbalanced_ensemble.egg-info/PKG-INFO` & `imbalanced-ensemble-0.2.1/imbalanced_ensemble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: imbalanced-ensemble
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolbox for ensemble learning on class-imbalanced dataset.
 Home-page: https://github.com/ZhiningLiu1998/imbalanced-ensemble
 Author: Zhining Liu
 Author-email: zhining.liu@outlook.com
 Maintainer: Zhining Liu
 Maintainer-email: zhining.liu@outlook.com
 License: MIT
 Project-URL: Documentation, https://imbalanced-ensemble.readthedocs.io/
 Project-URL: Source, https://github.com/ZhiningLiu1998/imbalanced-ensemble
 Project-URL: Tracker, https://github.com/ZhiningLiu1998/imbalanced-ensemble/issues
 Project-URL: Changelog, https://imbalanced-ensemble.readthedocs.io/en/latest/release_history.html
 Project-URL: Download, https://pypi.org/project/imbalanced-ensemble/#files
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -110,15 +111,15 @@
   Links: 
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#5-min-quick-start-with-imbens">Getting Started</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/">API Reference</a> |
   <a href="https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#">Examples</a> |
   <a href="https://github.com/ZhiningLiu1998/imbalanced-ensemble#related-projects">Related Projects</a> |
   <a href="https://zhuanlan.zhihu.com/p/376572330">知乎/Zhihu</a>  
   Paper:
-  <a href="https://arxiv.org/abs/2111.12776">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
+  <a href="https://arxiv.org/pdf/2111.12776.pdf">"IMBENS: Ensemble Class-imbalanced Learning in Python"</a>
   <br>**
 
 ***IMBENS*** (imported as `imbens`) is a Python library for quick implementation, modification, evaluation, and visualization of **ensemble [learning from class-imbalanced data](https://github.com/ZhiningLiu1998/awesome-imbalanced-learning)**. 
 Currently, IMBENS includes more than **[15 ensemble imbalanced learning algorithms](#list-of-implemented-methods)**, from the classical *SMOTEBoost* (2003), *RUSBoost* (2010) to recent [*Self-paced Ensemble*](https://github.com/ZhiningLiu1998/self-paced-ensemble) (2020), from *resampling* to *cost-sensitive learning*.
 
 ***IMBENS*** is developed on top of [imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn) (imblearn) and follows the API design of [scikit-learn](https://github.com/scikit-learn/scikit-learn). Compared to imblearn, IMBENS provides more powerful ensemble learning algorithms with ***multi-class learning*** support and many other **advanced features**:
 
@@ -133,34 +134,40 @@
 - &#x1F34E; Unified, easy-to-use APIs, detailed [documentation](https://imbalanced-ensemble.readthedocs.io/) and [examples](https://imbalanced-ensemble.readthedocs.io/en/latest/auto_examples/index.html#).
 - &#x1F34E; Capable for out-of-the-box ***multi-class*** imbalanced (long-tailed) learning.
 - &#x1F34E; Optimized performance with parallelization when possible using [joblib](https://github.com/joblib/joblib).
 - &#x1F34E; Powerful, customizable, interactive training logging and visualizer.
 - &#x1F34E; Full compatibility with other popular packages like [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https://imbalanced-learn.org/stable/).
 
 **Ensemble Imbalanced Learning with 4 Lines of Code:**
+
 ```python
 # Train an SPE classifier
 from imbens.ensemble import SelfPacedEnsembleClassifier
 clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train)
 
 # Predict with an SPE classifier
 y_pred = clf.predict(X_test)
 ```
+
+**Contributing to IMBENS**
+
+Please refer to the [contributing guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/CONTRIBUTING.md).
+
 **Citing IMBENS**
 
 The [IMBENS paper](https://arxiv.org/pdf/2111.12776.pdf) is available on arxiv.
 If you use IMBENS in a scientific publication, we would appreciate citations to the following paper:
 
 ```bib
-@article{liu2021imbens,
+@article{liu2023imbens,
   title={IMBENS: Ensemble Class-imbalanced Learning in Python},
-  author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi},
+  author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
   journal={arXiv preprint arXiv:2111.12776},
-  year={2021}
+  year={2023}
 }
 ```
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
@@ -524,7 +531,9 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: imbalanced-ensemble Version: 0.2.0 Summary: Toolbox
+Metadata-Version: 2.1 Name: imbalanced-ensemble Version: 0.2.1 Summary: Toolbox
 for ensemble learning on class-imbalanced dataset. Home-page: https://
 github.com/ZhiningLiu1998/imbalanced-ensemble Author: Zhining Liu Author-email:
 zhining.liu@outlook.com Maintainer: Zhining Liu Maintainer-email:
 zhining.liu@outlook.com License: MIT Project-URL: Documentation, https://
 imbalanced-ensemble.readthedocs.io/ Project-URL: Source, https://github.com/
 ZhiningLiu1998/imbalanced-ensemble Project-URL: Tracker, https://github.com/
 ZhiningLiu1998/imbalanced-ensemble/issues Project-URL: Changelog, https://
 imbalanced-ensemble.readthedocs.io/en/latest/release_history.html Project-URL:
-Download, https://pypi.org/project/imbalanced-ensemble/#files Classifier:
-Intended Audience :: Science/Research Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Download, https://pypi.org/project/imbalanced-ensemble/#files Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: C Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
 Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -61,47 +61,47 @@
 - &#x1F34E; Powerful, customizable, interactive training logging and
 visualizer. - &#x1F34E; Full compatibility with other popular packages like
 [scikit-learn](https://scikit-learn.org/stable/) and [imbalanced-learn](https:/
 /imbalanced-learn.org/stable/). **Ensemble Imbalanced Learning with 4 Lines of
 Code:** ```python # Train an SPE classifier from imbens.ensemble import
 SelfPacedEnsembleClassifier clf = SelfPacedEnsembleClassifier(random_state=42)
 clf.fit(X_train, y_train) # Predict with an SPE classifier y_pred = clf.predict
-(X_test) ``` **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
+(X_test) ``` **Contributing to IMBENS** Please refer to the [contributing
+guidelines](https://github.com/ZhiningLiu1998/imbalanced-ensemble/blob/main/
+CONTRIBUTING.md). **Citing IMBENS** The [IMBENS paper](https://arxiv.org/pdf/
 2111.12776.pdf) is available on arxiv. If you use IMBENS in a scientific
 publication, we would appreciate citations to the following paper: ```bib
-@article{liu2021imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
-Python}, author={Liu, Zhining and Wei, Zhepei and Yu, Erxin and Huang, Qiang
-and Guo, Kai and Yu, Boyang and Cai, Zhaonian and Ye, Hangting and Cao, Wei and
-Bian, Jiang and Wei, Pengfei and Jiang, Jing and Chang, Yi}, journal={arXiv
-preprint arXiv:2111.12776}, year={2021} } ``` ## Table of Contents - [Table of
-Contents](#table-of-contents) - [Installation](#installation) - [Highlights]
-(#highlights) - [List of implemented methods](#list-of-implemented-methods) -
-[5-min Quick Start with IMBENS](#5-min-quick-start-with-imbens) - [A minimal
-working example](#a-minimal-working-example) - [Visualize ensemble classifiers]
-(#visualize-ensemble-classifiers) - [Customizing training log](#customizing-
-training-log) - [About imbalanced learning](#about-imbalanced-learning) -
-[Acknowledgements](#acknowledgements) - [References](#references) - [Related
-Projects](#related-projects) - [Contributors â¨](#contributors-) ##
-Installation It is recommended to use **pip** for installation. Please make
-sure the **latest version** is installed to avoid potential problems: ```shell
-$ pip install imbalanced-ensemble # normal install $ pip install --upgrade
-imbalanced-ensemble # update if needed ``` Or you can install imbalanced-
-ensemble by clone this repository: ```shell $ git clone https://github.com/
-ZhiningLiu1998/imbalanced-ensemble.git $ cd imbalanced-ensemble $ pip install .
-``` imbalanced-ensemble requires following dependencies: - [Python](https://
-www.python.org/) (>=3.6) - [numpy](https://numpy.org/) (>=1.16.0) - [pandas]
-(https://pandas.pydata.org/) (>=1.1.3) - [scipy](https://www.scipy.org/)
-(>=1.9.1) - [joblib](https://pypi.org/project/joblib/) (>=0.11) - [scikit-
-learn](https://scikit-learn.org/stable/) (>=1.2.0) - [matplotlib](https://
-matplotlib.org/) (>=3.3.2) - [seaborn](https://seaborn.pydata.org/) (>=0.11.0)
-- [tqdm](https://tqdm.github.io/) (>=4.50.2) ## Highlights - &#x1F34E;
-***Unified, easy-to-use API design.*** All ensemble learning methods
-implemented in IMBENS share a unified API design. Similar to sklearn, all
-methods have functions (e.g., `fit()`, `predict()`, `predict_proba()`) that
-allow users to deploy them with only a few lines of code. - &#x1F34E;
+@article{liu2023imbens, title={IMBENS: Ensemble Class-imbalanced Learning in
+Python}, author={Liu, Zhining and Kang, Jian and Tong, Hanghang and Chang, Yi},
+journal={arXiv preprint arXiv:2111.12776}, year={2023} } ``` ## Table of
+Contents - [Table of Contents](#table-of-contents) - [Installation]
+(#installation) - [Highlights](#highlights) - [List of implemented methods]
+(#list-of-implemented-methods) - [5-min Quick Start with IMBENS](#5-min-quick-
+start-with-imbens) - [A minimal working example](#a-minimal-working-example) -
+[Visualize ensemble classifiers](#visualize-ensemble-classifiers) -
+[Customizing training log](#customizing-training-log) - [About imbalanced
+learning](#about-imbalanced-learning) - [Acknowledgements](#acknowledgements) -
+[References](#references) - [Related Projects](#related-projects) -
+[Contributors â¨](#contributors-) ## Installation It is recommended to use
+**pip** for installation. Please make sure the **latest version** is installed
+to avoid potential problems: ```shell $ pip install imbalanced-ensemble #
+normal install $ pip install --upgrade imbalanced-ensemble # update if needed
+``` Or you can install imbalanced-ensemble by clone this repository: ```shell $
+git clone https://github.com/ZhiningLiu1998/imbalanced-ensemble.git $ cd
+imbalanced-ensemble $ pip install . ``` imbalanced-ensemble requires following
+dependencies: - [Python](https://www.python.org/) (>=3.6) - [numpy](https://
+numpy.org/) (>=1.16.0) - [pandas](https://pandas.pydata.org/) (>=1.1.3) -
+[scipy](https://www.scipy.org/) (>=1.9.1) - [joblib](https://pypi.org/project/
+joblib/) (>=0.11) - [scikit-learn](https://scikit-learn.org/stable/) (>=1.2.0)
+- [matplotlib](https://matplotlib.org/) (>=3.3.2) - [seaborn](https://
+seaborn.pydata.org/) (>=0.11.0) - [tqdm](https://tqdm.github.io/) (>=4.50.2) ##
+Highlights - &#x1F34E; ***Unified, easy-to-use API design.*** All ensemble
+learning methods implemented in IMBENS share a unified API design. Similar to
+sklearn, all methods have functions (e.g., `fit()`, `predict()`, `predict_proba
+()`) that allow users to deploy them with only a few lines of code. - &#x1F34E;
 ***Extended functionalities, wider application scenarios.*** *All methods in
 IMBENS are ready for **multi-class imbalanced classification**.* We extend
 binary ensemble imbalanced learning methods to get them to work under the
 multi-class scenario. Additionally, for supported methods, we provide more
 training options like class-wise resampling control, balancing scheduler during
 the ensemble training process, etc. - &#x1F34E; ***Detailed training log, quick
 intuitive visualization.*** We provide additional parameters (e.g.,
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/_version.py` & `imbalanced-ensemble-0.2.1/imbens/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/datasets/_imbalance.py` & `imbalanced-ensemble-0.2.1/imbens/datasets/_imbalance.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/datasets/_zenodo.py` & `imbalanced-ensemble-0.2.1/imbens/datasets/_zenodo.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/datasets/tests/test_imbalance.py` & `imbalanced-ensemble-0.2.1/imbens/datasets/tests/test_imbalance.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/datasets/tests/test_zenodo.py` & `imbalanced-ensemble-0.2.1/imbens/datasets/tests/test_zenodo.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/adaboost_compatible.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/adaboost_compatible.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/bagging_compatible.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/bagging_compatible.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/test_adabost_compatible.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/test_adabost_compatible.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_compatible/tests/test_bagging_compatible.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_compatible/tests/test_bagging_compatible.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/kmeans_smote_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/kmeans_smote_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/over_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/over_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/over_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/over_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/smote_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/smote_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/smote_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/smote_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_kmeans_smote_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_kmeans_smote_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_over_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_over_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_over_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_over_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_smote_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_smote_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_over_sampling/tests/test_smote_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_over_sampling/tests/test_smote_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/adacost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/adacost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/adauboost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/adauboost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/asymmetric_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/easy_ensemble.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,296 @@
-"""AsymBoostClassifier: An Asymmetric Boosting classifier.
+"""EasyEnsembleClassifier: Bag of balanced boosted learners 
+also known as EasyEnsemble.
 """
 
 # Authors: Zhining Liu <zhining.liu@outlook.com>
 # License: MIT
 
 # %%
 LOCAL_DEBUG = False
 
 if not LOCAL_DEBUG:
+    from ...sampler._under_sampling import RandomUnderSampler
     from ...utils._docstring import (
         FuncSubstitution,
         Substitution,
         _get_example_docstring,
         _get_parameter_docstring,
     )
     from ...utils._validation import _deprecate_positional_args
-    from .._boost import ReweightBoostClassifier
+    from .._bagging import ResampleBaggingClassifier
 else:  # pragma: no cover
     import sys  # For local test
 
     sys.path.append("../..")
-    from ensemble._boost import ReweightBoostClassifier
+    from ensemble._bagging import ResampleBaggingClassifier
+    from sampler._under_sampling import RandomUnderSampler
     from utils._validation import _deprecate_positional_args
     from utils._docstring import (
         Substitution,
         FuncSubstitution,
         _get_parameter_docstring,
         _get_example_docstring,
     )
 
-import numpy as np
-import pandas as pd
+from warnings import warn
+
+from sklearn.ensemble import AdaBoostClassifier
 
 # Properties
-_method_name = 'AsymBoostClassifier'
+_method_name = 'EasyEnsembleClassifier'
+_sampler_class = RandomUnderSampler
 
-_solution_type = ReweightBoostClassifier._solution_type
-_ensemble_type = ReweightBoostClassifier._ensemble_type
-_training_type = ReweightBoostClassifier._training_type
+_solution_type = ResampleBaggingClassifier._solution_type
+_sampling_type = 'under-sampling'
+_ensemble_type = ResampleBaggingClassifier._ensemble_type
+_training_type = ResampleBaggingClassifier._training_type
 
 _properties = {
+    'sampling_type': _sampling_type,
     'solution_type': _solution_type,
     'ensemble_type': _ensemble_type,
     'training_type': _training_type,
 }
 
 
 @Substitution(
-    early_termination=_get_parameter_docstring('early_termination', **_properties),
     random_state=_get_parameter_docstring('random_state', **_properties),
+    n_jobs=_get_parameter_docstring('n_jobs', **_properties),
+    warm_start=_get_parameter_docstring('warm_start', **_properties),
     example=_get_example_docstring(_method_name),
 )
-class AsymBoostClassifier(ReweightBoostClassifier):
-    """An Asymmetric Boosting classifier.
+class EasyEnsembleClassifier(ResampleBaggingClassifier):
+    """Bag of balanced boosted learners also known as EasyEnsemble.
 
-    Asymmetric Boosting (AsymBoost) [1]_, a variant of AdaBoost, is a
-    cost-sensitive boosting method. It uses the asymmetric misclassication
-    cost to update the training distribution on successive boosting rounds.
+    This algorithm is known as EasyEnsemble [1]_. The classifier is an
+    ensemble of AdaBoost learners trained on different balanced boostrap
+    samples. The balancing is achieved by random under-sampling.
 
-    This AsymBoost implementation supports multi-class classification.
+    This implementation extends EasyEnsemble to support multi-class classification.
 
     Parameters
     ----------
-    estimator : estimator object, default=None
-        The base estimator from which the boosted ensemble is built.
-        Support for sample weighting is required, as well as proper
-        ``classes_`` and ``n_classes_`` attributes. If ``None``, then
-        the base estimator is ``DecisionTreeClassifier(max_depth=1)``.
-
     n_estimators : int, default=50
-        The maximum number of estimators at which boosting is terminated.
-        In case of perfect fit, the learning procedure is stopped early.
+        Number of AdaBoost learners in the ensemble.
+
+    estimator : estimator object, default=AdaBoostClassifier(n_estimators=10)
+        The base AdaBoost classifier used in the inner ensemble. Note that you
+        can use another classifier as the base estimator, but this will degrades
+        EasyEnsemble to ``UnderBaggingClassifier`` and raise a Warning.
+
+    max_samples : int or float, default=1.0
+        The number of samples to draw from X to train each base estimator (with
+        replacement by default, see `bootstrap` for more details).
+
+        - If ``int``, then draw `max_samples` samples.
+        - If ``float``, then draw `max_samples * X.shape[0]` samples.
+
+    max_features : int or float, default=1.0
+        The number of features to draw from X to train each base estimator (
+        without replacement by default, see `bootstrap_features` for more
+        details).
+
+        - If ``int``, then draw `max_features` features.
+        - If ``float``, then draw `max_features * X.shape[1]` features.
 
-    learning_rate : float, default=1.
-        Learning rate shrinks the contribution of each classifier by
-        ``learning_rate``. There is a trade-off between ``learning_rate`` and
-        ``n_estimators``.
-
-    algorithm : {{'SAMME', 'SAMME.R'}}, default='SAMME.R'
-        If 'SAMME.R' then use the SAMME.R real boosting algorithm.
-        ``estimator`` must support calculation of class probabilities.
-        If 'SAMME' then use the SAMME discrete boosting algorithm.
-        The SAMME.R algorithm typically converges faster than SAMME,
-        achieving a lower test error with fewer boosting iterations.
+    bootstrap : bool, default=True
+        Whether samples are drawn with replacement. If False, sampling
+        without replacement is performed.
 
-    {early_termination}
+    bootstrap_features : bool, default=False
+        Whether features are drawn with replacement.
+
+    oob_score : bool, default=False
+        Whether to use out-of-bag samples to estimate
+        the generalization error.
+
+    {warm_start}
+
+    {n_jobs}
 
     {random_state}
 
+    verbose : int, default=0
+        Controls the verbosity when fitting and predicting.
+
     Attributes
     ----------
-    estimators_ : list of classifiers
-        The collection of fitted sub-estimators.
+    estimator_ : pipeline estimator
+        The base estimator from which the ensemble is grown.
 
-    cost_matrix_ : array of shape = [n_classes, n_classes]
-        The used cost matrix. The rows represent the predicted class and
-        columns represent the actual class. The order of the classes
-        corresponds to that in the attribute ``classes_``.
+    sampler_ : RandomUnderSampler
+        The base sampler.
 
-    cost_table_asymboost_ : DataFrame of shape = [n_classes*n_classes, 3]
-        The used cost map table.
+    estimators_ : list of classifiers
+        The collection of fitted sub-estimators.
 
-    classes_ : array of shape = [n_classes]
-        The classes labels.
+    n_features_in_ : int
+        The number of features when :meth:`fit` is performed.
 
-    n_classes_ : int
-        The number of classes.
+    estimators_ : list of estimators
+        The collection of fitted base estimators.
 
-    estimator_weights_ : array of floats
-        Weights for each estimator in the boosted ensemble.
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
 
-    estimator_errors_ : array of floats
-        Classification error for each estimator in the boosted
-        ensemble.
+    estimators_features_ : list of arrays
+        The subset of drawn features for each base estimator.
 
     estimators_n_training_samples_ : list of ints
         The number of training samples for each fitted
         base estimators.
 
-    feature_importances_ : array of shape = [n_features]
-        The feature importances if supported by the ``estimator``.
+    classes_ : ndarray of shape (n_classes,)
+        The classes labels.
+
+    n_classes_ : int or list
+        The number of classes.
 
-    See also
+    oob_score_ : float
+        Score of the training dataset obtained using an out-of-bag estimate.
+        This attribute exists only when ``oob_score`` is True.
+
+    oob_decision_function_ : ndarray of shape (n_samples, n_classes)
+        Decision function computed with out-of-bag estimate on the training
+        set. If n_estimators is small it might be possible that a data point
+        was never left out during the bootstrap. In this case,
+        `oob_decision_function_` might contain NaN. This attribute exists
+        only when ``oob_score`` is True.
+
+    See Also
     --------
-    AdaUBoostClassifier : An AdaUBoost cost-sensitive classifier.
+    BalanceCascadeClassifier : Ensemble with cascade dynamic under-sampling.
+
+    SelfPacedEnsembleClassifier : Ensemble with self-paced dynamic under-sampling.
 
-    AdaCostClassifier : An AdaCost cost-sensitive boosting classifier.
+    UnderBaggingClassifier : Bagging with intergrated random under-sampling.
 
     References
     ----------
-    .. [1] Viola, P., & Jones, M. "Fast and robust classification using
-       asymmetric adaboost and a detector cascade." Advances in Neural
-       Information Processing System 14 (2001).
+    .. [1] X. Y. Liu, J. Wu and Z. H. Zhou, "Exploratory Undersampling for
+       Class-Imbalance Learning," in IEEE Transactions on Systems, Man, and
+       Cybernetics, Part B (Cybernetics), vol. 39, no. 2, pp. 539-550,
+       April 2009.
 
     Examples
     --------
     {example}
     """
 
     @_deprecate_positional_args
     def __init__(
         self,
         estimator=None,
         n_estimators: int = 50,
         *,
-        learning_rate: float = 1.0,
-        algorithm: str = 'SAMME.R',
-        early_termination: bool = False,
+        max_samples=1.0,
+        max_features=1.0,
+        bootstrap=True,
+        bootstrap_features=False,
+        oob_score=False,
+        warm_start=False,
+        n_jobs=None,
         random_state=None,
+        verbose=0,
     ):
 
-        super(AsymBoostClassifier, self).__init__(
+        sampling_strategy = 'auto'
+        sampler = _sampler_class()
+        sampling_type = _sampling_type
+
+        # Check if the estimator is AdaBoostClassifier
+        if estimator is None:
+            estimator = AdaBoostClassifier(n_estimators=10)
+        elif type(estimator) == AdaBoostClassifier:
+            estimator = estimator
+        else:
+            # if not, raise a Warning
+            warn(
+                f"\nYou are trying to set {type(estimator)} as the"
+                f" base estimator. A typical EasyEnsembleClassifier uses"
+                f" Adaboost as its base estimator, using other base"
+                f" estimators will degrades it to UnderBaggingClassifier."
+            )
+            estimator = estimator
+
+        super().__init__(
             estimator=estimator,
             n_estimators=n_estimators,
-            learning_rate=learning_rate,
-            algorithm=algorithm,
-            early_termination=early_termination,
+            sampler=sampler,
+            sampling_type=sampling_type,
+            sampling_strategy=sampling_strategy,
+            max_samples=max_samples,
+            max_features=max_features,
+            bootstrap=bootstrap,
+            bootstrap_features=bootstrap_features,
+            oob_score=oob_score,
+            warm_start=warm_start,
+            n_jobs=n_jobs,
             random_state=random_state,
+            verbose=verbose,
         )
 
         self.__name__ = _method_name
+        self._sampling_type = _sampling_type
+        self._sampler_class = _sampler_class
         self._properties = _properties
 
-    def _compute_mult_out_exp_weights_array(self, y_true, y_pred):
-        """Return the asymmetric weights of shape = (n_samples,).
-
-        Parameters
-        ----------
-        y_true : array-like of shape = [n_samples, 1]
-                 True class values.
-
-        y_pred : array-like of shape = [n_samples, 1]
-                 Predicted class values.
-        """
-        df = pd.DataFrame({'y_pred': y_pred, 'y_true': y_true})
-        df = df.merge(self.cost_table_asymboost_, how='left', on=['y_pred', 'y_true'])
-
-        return df['asym_weight'].values
-
-    def _cost_matrix_to_asymmetric_weights(self, cost_matrix):
-        """Creates a table of asymmetric weight map table from the cost matrix.
-
-        Parameters
-        ----------
-        cost_matrix : array-like of shape = [n_classes, n_classes]
-
-        Returns
-        -------
-        df : pd.DataFrame of shape = [n_classes, 2]
-
-        """
-        table = np.empty((0, 3))
-
-        for (x, y), value in np.ndenumerate(cost_matrix):
-            # Section 4 of [1]
-            table = np.vstack(
-                (
-                    table,
-                    np.array(
-                        [x, y, np.exp(1 / self.n_estimators * np.log(np.sqrt(value)))]
-                    ),
-                )
-            )
-
-        return pd.DataFrame(table, columns=['y_pred', 'y_true', 'asym_weight'])
-
-    def _validate_cost_matrix(self, cost_matrix, n_classes):
-        """validate the cost matrix & set the cost map table."""
-
-        cost_matrix = super()._validate_cost_matrix(cost_matrix, n_classes)
-        self.cost_table_asymboost_ = self._cost_matrix_to_asymmetric_weights(
-            cost_matrix
-        )
-
-        return cost_matrix
-
     @_deprecate_positional_args
     @FuncSubstitution(
         eval_datasets=_get_parameter_docstring('eval_datasets'),
         eval_metrics=_get_parameter_docstring('eval_metrics'),
         train_verbose=_get_parameter_docstring('train_verbose', **_properties),
     )
     def fit(
         self,
         X,
         y,
         *,
         sample_weight=None,
-        cost_matrix='inverse',
+        max_samples=None,
         eval_datasets: dict = None,
         eval_metrics: dict = None,
         train_verbose: bool or int or dict = False,
     ):
-        """Build a AsymBoost classifier from the training set (X, y).
+        """Build an EasyEnsemble classifier from the training set (X, y).
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The training input samples. Sparse matrix can be CSC, CSR, COO,
             DOK, or LIL. DOK and LIL are converted to CSR.
 
         y : array-like of shape (n_samples,)
             The target values (class labels).
 
         sample_weight : array-like of shape (n_samples,), default=None
             Sample weights. If None, the sample weights are initialized to
             ``1 / n_samples``.
 
-        cost_matrix : str or numpy.ndarray, default=None
-            A matrix representing the cost of misclassification.
-
-            - If ``None``, equivalent to ``'inverse'``.
-            - If ``'uniform'``, set misclassification cost to be equal.
-            - If ``'inverse'``, set misclassification cost by inverse class frequency.
-            - If ``numpy.ndarray`` of shape (n_classes, n_classes), the rows
-              represent the predicted class and columns represent the actual class.
-              Thus the value at :math:`i`-th row :math:`j`-th column (:math:`C_{ij}`)
-              represents the cost of classifying a sample from class :math:`j` to
-              class :math:`i`.
-              Note: the cost matrix must satisfy that :math:`C_{ij} * C_{ji} = 1`.
+        max_samples : int or float, default=None
+            Argument to use instead of self.max_samples.
 
         %(eval_datasets)s
 
         %(eval_metrics)s
 
         %(train_verbose)s
 
         Returns
         -------
         self : object
         """
 
-        # Note that AsymBoost requires the cost matrix to satisfy
-        # C_{ij} * C_{ji} = 1, thus the 'log1p-inverse' option is not
-        # available in this situation.
-        if type(cost_matrix) == str and cost_matrix == 'log1p-inverse':
-            raise ValueError(
-                "'log1p-inverse' option is not available for "
-                "AsymBoostClassifier. Please use 'inverse' instead."
-            )
-
         return self._fit(
             X,
             y,
             sample_weight=sample_weight,
-            cost_matrix=cost_matrix,
+            max_samples=max_samples,
             eval_datasets=eval_datasets,
             eval_metrics=eval_metrics,
             train_verbose=train_verbose,
         )
 
 
 # %%
@@ -321,53 +323,59 @@
     X_train, X_valid, y_train, y_valid = train_test_split(
         X, y, test_size=0.5, random_state=42
     )
 
     origin_distr = dict(Counter(y_train))  # {2: 600, 1: 300, 0: 100}
     print('Original training dataset shape %s' % origin_distr)
 
+    target_distr = {2: 200, 1: 100, 0: 100}
+
     init_kwargs_default = {
         'estimator': None,
+        # 'estimator': DecisionTreeClassifier(),
         'n_estimators': 100,
-        'learning_rate': 1.0,
-        'algorithm': 'SAMME.R',
+        'max_samples': 1.0,
+        'max_features': 1.0,
+        'bootstrap': True,
+        'bootstrap_features': False,
+        'oob_score': False,
+        'warm_start': False,
+        'n_jobs': None,
         'random_state': 42,
         # 'random_state': None,
+        'verbose': 0,
     }
     fit_kwargs_default = {
         'X': X_train,
         'y': y_train,
         'sample_weight': None,
+        'max_samples': None,
         'eval_datasets': {'valid': (X_valid, y_valid)},
         'eval_metrics': {
             'acc': (accuracy_score, {}),
             'balanced_acc': (balanced_accuracy_score, {}),
             'weighted_f1': (f1_score, {'average': 'weighted'}),
         },
-        'train_verbose': {
-            'granularity': 10,
-            'print_distribution': True,
-            'print_metrics': True,
-        },
+        'train_verbose': True,
     }
 
     ensembles = {}
 
     init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
-    asymboost = AsymBoostClassifier(**init_kwargs).fit(**fit_kwargs)
-    ensembles['asymboost'] = asymboost
+    easyens = EasyEnsembleClassifier(**init_kwargs).fit(**fit_kwargs)
+    ensembles['easyens'] = easyens
 
     init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
-    fit_kwargs.update(
+    init_kwargs.update(
         {
-            'cost_matrix': 'uniform',
+            'estimator': DecisionTreeClassifier(),
         }
     )
-    asymboost_uniform = AsymBoostClassifier(**init_kwargs).fit(**fit_kwargs)
-    ensembles['asymboost_uniform'] = asymboost_uniform
+    easyens_fallback = EasyEnsembleClassifier(**init_kwargs).fit(**fit_kwargs)
+    ensembles['easyens_fallback'] = easyens_fallback
 
     # %%
     from imbens.visualizer import ImbalancedEnsembleVisualizer
 
     visualizer = ImbalancedEnsembleVisualizer(
         eval_datasets=None,
         eval_metrics=None,
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_adacost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_adacost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_adauboost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_adauboost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_reweighting/tests/test_asymmetric_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_reweighting/tests/test_asymmetric_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/balance_cascade.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/balance_cascade.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/balanced_random_forest.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/balanced_random_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,14 @@
         random_state=None,
         verbose=0,
         warm_start=False,
         class_weight=None,
         ccp_alpha=0.0,
         max_samples=None,
     ):
-
         super().__init__(
             criterion=criterion,
             max_depth=max_depth,
             n_estimators=n_estimators,
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
@@ -388,29 +387,29 @@
 
         if self.n_estimators <= 0:
             raise ValueError(
                 f"n_estimators must be greater than zero, " f"got {self.n_estimators}."
             )
 
         if self.estimator is not None:
-            self._estimator = clone(self.estimator)
+            self.estimator_ = clone(self.estimator)
         else:
-            self._estimator = clone(default)
+            self.estimator_ = clone(default)
 
         self.sampler_ = RandomUnderSampler(
             sampling_strategy=self._sampling_strategy,
             replacement=self.replacement,
         )
 
     def _make_sampler_estimator(self, random_state=None):
         """Make and configure a copy of the `estimator_` attribute.
         Warning: This method should be used to properly instantiate new
         sub-estimators.
         """
-        estimator = clone(self._estimator)
+        estimator = clone(self.estimator_)
         estimator.set_params(**{p: getattr(self, p) for p in self.estimator_params})
         sampler = clone(self.sampler_)
 
         if random_state is not None:
             _set_random_states(estimator, random_state)
             _set_random_states(sampler, random_state)
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/easy_ensemble.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/under_bagging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,83 @@
-"""EasyEnsembleClassifier: Bag of balanced boosted learners 
-also known as EasyEnsemble.
+"""UnderBaggingClassifier: A Bagging classifier with intergrated 
+random under-sampling.
 """
 
 # Authors: Zhining Liu <zhining.liu@outlook.com>
 # License: MIT
 
 # %%
 LOCAL_DEBUG = False
 
 if not LOCAL_DEBUG:
+    from .._bagging import ResampleBaggingClassifier
     from ...sampler._under_sampling import RandomUnderSampler
+    from ...utils._validation import _deprecate_positional_args
     from ...utils._docstring import (
-        FuncSubstitution,
         Substitution,
-        _get_example_docstring,
+        FuncSubstitution,
         _get_parameter_docstring,
+        _get_example_docstring,
     )
-    from ...utils._validation import _deprecate_positional_args
-    from .._bagging import ResampleBaggingClassifier
 else:  # pragma: no cover
     import sys  # For local test
 
     sys.path.append("../..")
     from ensemble._bagging import ResampleBaggingClassifier
     from sampler._under_sampling import RandomUnderSampler
     from utils._validation import _deprecate_positional_args
     from utils._docstring import (
         Substitution,
         FuncSubstitution,
         _get_parameter_docstring,
         _get_example_docstring,
     )
 
-from warnings import warn
-
-from sklearn.ensemble import AdaBoostClassifier
 
 # Properties
-_method_name = 'EasyEnsembleClassifier'
+_method_name = 'UnderBaggingClassifier'
 _sampler_class = RandomUnderSampler
 
 _solution_type = ResampleBaggingClassifier._solution_type
 _sampling_type = 'under-sampling'
 _ensemble_type = ResampleBaggingClassifier._ensemble_type
 _training_type = ResampleBaggingClassifier._training_type
 
 _properties = {
-    'sampling_type': _sampling_type,
     'solution_type': _solution_type,
+    'sampling_type': _sampling_type,
     'ensemble_type': _ensemble_type,
     'training_type': _training_type,
 }
 
 
 @Substitution(
     random_state=_get_parameter_docstring('random_state', **_properties),
     n_jobs=_get_parameter_docstring('n_jobs', **_properties),
     warm_start=_get_parameter_docstring('warm_start', **_properties),
     example=_get_example_docstring(_method_name),
 )
-class EasyEnsembleClassifier(ResampleBaggingClassifier):
-    """Bag of balanced boosted learners also known as EasyEnsemble.
+class UnderBaggingClassifier(ResampleBaggingClassifier):
+    """A Bagging classifier with intergrated random under-sampling.
 
-    This algorithm is known as EasyEnsemble [1]_. The classifier is an
-    ensemble of AdaBoost learners trained on different balanced boostrap
-    samples. The balancing is achieved by random under-sampling.
+    This implementation of UnderBagging [1]_ is similar to the scikit-learn
+    implementation. It includes an additional step to balance the training set
+    at fit time using a RandomUnderSampler.
 
-    This implementation extends EasyEnsemble to support multi-class classification.
+    This implementation extends UnderBagging to support multi-class classification.
 
     Parameters
     ----------
-    n_estimators : int, default=50
-        Number of AdaBoost learners in the ensemble.
+    estimator : object, default=None
+        The base estimator to fit on random subsets of the dataset.
+        If None, then the base estimator is a
+        ``Pipeline([RandomUnderSampler(), DecisionTreeClassifier()])``.
 
-    estimator : estimator object, default=AdaBoostClassifier(n_estimators=10)
-        The base AdaBoost classifier used in the inner ensemble. Note that you
-        can use another classifier as the base estimator, but this will degrades
-        EasyEnsemble to ``UnderBaggingClassifier`` and raise a Warning.
+    n_estimators : int, default=50
+        The number of base estimators in the ensemble.
 
     max_samples : int or float, default=1.0
         The number of samples to draw from X to train each base estimator (with
         replacement by default, see `bootstrap` for more details).
 
         - If ``int``, then draw `max_samples` samples.
         - If ``float``, then draw `max_samples * X.shape[0]` samples.
@@ -156,26 +153,34 @@
         set. If n_estimators is small it might be possible that a data point
         was never left out during the bootstrap. In this case,
         `oob_decision_function_` might contain NaN. This attribute exists
         only when ``oob_score`` is True.
 
     See Also
     --------
-    BalanceCascadeClassifier : Ensemble with cascade dynamic under-sampling.
+    EasyEnsembleClassifier : Bag of balanced boosted learners.
+
+    BalancedRandomForestClassifier : RandomForest with random under-sampling.
 
-    SelfPacedEnsembleClassifier : Ensemble with self-paced dynamic under-sampling.
+    RUSBoostClassifier : Random under-sampling integrated in AdaBoost.
 
-    UnderBaggingClassifier : Bagging with intergrated random under-sampling.
+    Notes
+    -----
+    This is possible to turn this classifier into a balanced random forest [2]_
+    by passing a :class:`~sklearn.tree.DecisionTreeClassifier` with
+    `max_features='auto'` as a base estimator.
 
     References
     ----------
-    .. [1] X. Y. Liu, J. Wu and Z. H. Zhou, "Exploratory Undersampling for
-       Class-Imbalance Learning," in IEEE Transactions on Systems, Man, and
-       Cybernetics, Part B (Cybernetics), vol. 39, no. 2, pp. 539-550,
-       April 2009.
+    .. [1] R. Maclin, and D. Opitz. "An empirical evaluation of bagging and
+           boosting." AAAI/IAAI 1997 (1997): 546-551.
+
+    .. [2] C. Chen Chao, A. Liaw, and L. Breiman. "Using random forest to
+           learn imbalanced data." University of California, Berkeley 110,
+           2004.
 
     Examples
     --------
     {example}
     """
 
     @_deprecate_positional_args
@@ -195,29 +200,14 @@
         verbose=0,
     ):
 
         sampling_strategy = 'auto'
         sampler = _sampler_class()
         sampling_type = _sampling_type
 
-        # Check if the estimator is AdaBoostClassifier
-        if estimator is None:
-            estimator = AdaBoostClassifier(n_estimators=10)
-        elif type(estimator) == AdaBoostClassifier:
-            estimator = estimator
-        else:
-            # if not, raise a Warning
-            warn(
-                f"\nYou are trying to set {type(estimator)} as the"
-                f" base estimator. A typical EasyEnsembleClassifier uses"
-                f" Adaboost as its base estimator, using other base"
-                f" estimators will degrades it to UnderBaggingClassifier."
-            )
-            estimator = estimator
-
         super().__init__(
             estimator=estimator,
             n_estimators=n_estimators,
             sampler=sampler,
             sampling_type=sampling_type,
             sampling_strategy=sampling_strategy,
             max_samples=max_samples,
@@ -249,28 +239,30 @@
         *,
         sample_weight=None,
         max_samples=None,
         eval_datasets: dict = None,
         eval_metrics: dict = None,
         train_verbose: bool or int or dict = False,
     ):
-        """Build an EasyEnsemble classifier from the training set (X, y).
+        """Build an UnderBagging ensemble of estimators from the training set (X, y).
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
-            The training input samples. Sparse matrix can be CSC, CSR, COO,
-            DOK, or LIL. DOK and LIL are converted to CSR.
+            The training input samples. Sparse matrices are accepted only if
+            they are supported by the base estimator.
 
         y : array-like of shape (n_samples,)
-            The target values (class labels).
+            The target values (class labels in classification, real numbers in
+            regression).
 
         sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, the sample weights are initialized to
-            ``1 / n_samples``.
+            Sample weights. If None, then samples are equally weighted.
+            Note that this is supported only if the base estimator supports
+            sample weighting.
 
         max_samples : int or float, default=None
             Argument to use instead of self.max_samples.
 
         %(eval_datasets)s
 
         %(eval_metrics)s
@@ -294,19 +286,17 @@
 
 
 # %%
 
 if __name__ == "__main__":  # pragma: no cover
     from collections import Counter
     from copy import copy
-
     from sklearn.datasets import make_classification
-    from sklearn.metrics import accuracy_score, balanced_accuracy_score, f1_score
     from sklearn.model_selection import train_test_split
-    from sklearn.tree import DecisionTreeClassifier
+    from sklearn.metrics import accuracy_score, balanced_accuracy_score, f1_score
 
     # X, y = make_classification(n_classes=2, class_sep=2, # 2-class
     #     weights=[0.1, 0.9], n_informative=3, n_redundant=1, flip_y=0,
     #     n_features=20, n_clusters_per_class=1, n_samples=1000, random_state=10)
     X, y = make_classification(
         n_classes=3,
         class_sep=2,  # 3-class
@@ -327,26 +317,25 @@
     origin_distr = dict(Counter(y_train))  # {2: 600, 1: 300, 0: 100}
     print('Original training dataset shape %s' % origin_distr)
 
     target_distr = {2: 200, 1: 100, 0: 100}
 
     init_kwargs_default = {
         'estimator': None,
-        # 'estimator': DecisionTreeClassifier(),
         'n_estimators': 100,
         'max_samples': 1.0,
         'max_features': 1.0,
         'bootstrap': True,
         'bootstrap_features': False,
         'oob_score': False,
         'warm_start': False,
         'n_jobs': None,
         'random_state': 42,
         # 'random_state': None,
-        'verbose': 0,
+        'verbose': 1,
     }
     fit_kwargs_default = {
         'X': X_train,
         'y': y_train,
         'sample_weight': None,
         'max_samples': None,
         'eval_datasets': {'valid': (X_valid, y_valid)},
@@ -357,25 +346,16 @@
         },
         'train_verbose': True,
     }
 
     ensembles = {}
 
     init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
-    easyens = EasyEnsembleClassifier(**init_kwargs).fit(**fit_kwargs)
-    ensembles['easyens'] = easyens
-
-    init_kwargs, fit_kwargs = copy(init_kwargs_default), copy(fit_kwargs_default)
-    init_kwargs.update(
-        {
-            'estimator': DecisionTreeClassifier(),
-        }
-    )
-    easyens_fallback = EasyEnsembleClassifier(**init_kwargs).fit(**fit_kwargs)
-    ensembles['easyens_fallback'] = easyens_fallback
+    underbagging = UnderBaggingClassifier(**init_kwargs).fit(**fit_kwargs)
+    ensembles['underbagging'] = underbagging
 
     # %%
     from imbens.visualizer import ImbalancedEnsembleVisualizer
 
     visualizer = ImbalancedEnsembleVisualizer(
         eval_datasets=None,
         eval_metrics=None,
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/rus_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/rus_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/self_paced_ensemble.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/self_paced_ensemble.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_balance_cascade.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_balance_cascade.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_balanced_random_forest.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_balanced_random_forest.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_easy_ensemble.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_easy_ensemble.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_rus_boost.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_rus_boost.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_self_paced_ensemble.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_self_paced_ensemble.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/_under_sampling/tests/test_under_bagging.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/_under_sampling/tests/test_under_bagging.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/base.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/ensemble/tests/test_base_ensemble.py` & `imbalanced-ensemble-0.2.1/imbens/ensemble/tests/test_base_ensemble.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/_classification.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/pairwise.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_classification.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_pairwise.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_pairwise.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/metrics/tests/test_score_objects.py` & `imbalanced-ensemble-0.2.1/imbens/metrics/tests/test_score_objects.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/pipeline.py` & `imbalanced-ensemble-0.2.1/imbens/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #          Zhining Liu <zhining.liu@outlook.com>
 # License: BSD
 
 from collections import Counter
 from sklearn import pipeline
 from sklearn.base import clone
 from sklearn.utils import _print_elapsed_time
-from sklearn.utils.metaestimators import if_delegate_has_method
+from sklearn.utils.metaestimators import available_if
 from sklearn.utils.validation import check_memory
 
 __all__ = ["Pipeline", "make_pipeline"]
 
 
 class Pipeline(pipeline.Pipeline):
     """Pipeline of transforms and resamples with a final estimator.
@@ -179,24 +179,23 @@
             return filter(lambda x: not hasattr(x[-1], "fit_resample"), it)
         else:
             return it
 
     # Estimator interface
 
     def _fit(self, X, y=None, sample_weight=None, **fit_params_steps):
-
         self.steps = list(self.steps)
         self._validate_steps()
         # Setup the memory
         memory = check_memory(self.memory)
 
         fit_transform_one_cached = memory.cache(pipeline._fit_transform_one)
         fit_resample_one_cached = memory.cache(_fit_resample_one)
 
-        for (step_idx, name, transformer) in self._iter(
+        for step_idx, name, transformer in self._iter(
             with_final=False, filter_passthrough=False, filter_resample=False
         ):
             if transformer is None or transformer == "passthrough":
                 with _print_elapsed_time("Pipeline", self._log_message(step_idx)):
                     continue
 
             try:
@@ -369,15 +368,15 @@
         with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
             if last_step == "passthrough":
                 return Xt
             fit_params_last_step = fit_params_steps[self.steps[-1][0]]
             if hasattr(last_step, "fit_resample"):
                 return last_step.fit_resample(Xt, yt, **fit_params_last_step)
 
-    @if_delegate_has_method(delegate="_final_estimator")
+    @available_if(pipeline._final_estimator_has("fit_predict"))
     def fit_predict(self, X, y=None, **fit_params):
         """Apply `fit_predict` of last step in pipeline after transforms.
 
         Applies fit_transforms of a pipeline to the data, followed by the
         fit_predict method of the final estimator in the pipeline. Valid
         only if the final estimator implements fit_predict.
 
@@ -410,15 +409,14 @@
         return y_pred
 
 
 def _fit_resample_one(
     sampler, X, y, sample_weight=None, message_clsname="", message=None, **fit_params
 ):
     with _print_elapsed_time(message_clsname, message):
-
         out = sampler.fit_resample(X, y, sample_weight=sample_weight, **fit_params)
 
         if sample_weight is None:
             (X_res, y_res) = out
             return X_res, y_res, sampler
         else:
             (X_res, y_res, sample_weight_res) = out
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_adasyn.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_adasyn.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_random_over_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_random_over_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/base.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/base.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/cluster.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/cluster.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/filter.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/filter.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_borderline_smote.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_borderline_smote.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_kmeans_smote.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_kmeans_smote.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_smote.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_smote.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/_smote/tests/test_svm_smote.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/_smote/tests/test_svm_smote.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/base.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/base.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/test_adasyn.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/test_adasyn.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_over_sampling/tests/test_random_over_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_over_sampling/tests/test_random_over_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/_cluster_centroids.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/_cluster_centroids.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_generation/tests/test_cluster_centroids.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_generation/tests/test_cluster_centroids.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_balance_cascade_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_balance_cascade_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_condensed_nearest_neighbour.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_condensed_nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_edited_nearest_neighbours.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_instance_hardness_threshold.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_instance_hardness_threshold.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_nearmiss.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_nearmiss.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_neighbourhood_cleaning_rule.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_neighbourhood_cleaning_rule.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_one_sided_selection.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_one_sided_selection.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_random_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_random_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_self_paced_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_self_paced_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/_tomek_links.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/_tomek_links.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_allknn.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_allknn.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_balance_cascade_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_balance_cascade_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_condensed_nearest_neighbour.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_condensed_nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_edited_nearest_neighbours.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_instance_hardness_threshold.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_instance_hardness_threshold.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_nearmiss.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_nearmiss.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_neighbourhood_cleaning_rule.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_neighbourhood_cleaning_rule.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_one_sided_selection.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_one_sided_selection.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_random_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_random_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_repeated_edited_nearest_neighbours.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_repeated_edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_self_paced_under_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_self_paced_under_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/_prototype_selection/tests/test_tomek_links.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/_prototype_selection/tests/test_tomek_links.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/_under_sampling/base.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/_under_sampling/base.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/base.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/base.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/sampler/tests/test_base_sampler.py` & `imbalanced-ensemble-0.2.1/imbens/sampler/tests/test_base_sampler.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/__init__.py` & `imbalanced-ensemble-0.2.1/imbens/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_docstring.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_docstring.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_evaluate.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_evaluate.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_plot.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_plot.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_show_versions.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_show_versions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 which was adapted from :func:`pandas.show_versions`
 """
 # Adapted from imbalanced-learn
 
 # Author: Alexander L. Hayes <hayesall@iu.edu>
 # License: MIT
 
-import importlib
-import sys
+from .. import __version__
 
 
 def _get_deps_info():
     """Overview of the installed version of main dependencies
     Returns
     -------
     deps_info: dict
@@ -29,36 +28,33 @@
         "numpy",
         "scipy",
         "Cython",
         "pandas",
         "joblib",
     ]
 
-    def get_version(module):
-        return module.__version__
+    deps_info = {
+        "imbalanced-ensemble": __version__,
+    }
 
-    deps_info = {}
+    from importlib.metadata import PackageNotFoundError, version
 
     for modname in deps:
         try:
-            if modname in sys.modules:
-                mod = sys.modules[modname]
-            else:
-                mod = importlib.import_module(modname)
-            ver = get_version(mod)
-            deps_info[modname] = ver
-        except ImportError:
+            deps_info[modname] = version(modname)
+        except PackageNotFoundError:
             deps_info[modname] = None
-
     return deps_info
 
 
 def show_versions(github=False):
     """Print debugging information.
 
+    .. versionadded:: 0.5
+
     Parameters
     ----------
     github : bool,
         If true, wrap system info with GitHub markup.
     """
 
     from sklearn.utils._show_versions import _get_sys_info
@@ -72,27 +68,25 @@
         "{0}\n"
         "**Python Dependencies**\n\n"
         "{1}\n"
         "</details>"
     )
 
     if github:
-
         _sys_markup = ""
         _deps_markup = ""
 
         for k, stat in _sys_info.items():
             _sys_markup += f"* {k:<10}: `{stat}`\n"
         for k, stat in _deps_info.items():
             _deps_markup += f"* {k:<10}: `{stat}`\n"
 
         print(_github_markup.format(_sys_markup, _deps_markup))
 
     else:
-
         print("\nSystem:")
         for k, stat in _sys_info.items():
             print(f"{k:>11}: {stat}")
 
         print("\nPython dependencies:")
         for k, stat in _deps_info.items():
             print(f"{k:>11}: {stat}")
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_validation.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_validation_data.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_validation_data.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/_validation_param.py` & `imbalanced-ensemble-0.2.1/imbens/utils/_validation_param.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/deprecation.py` & `imbalanced-ensemble-0.2.1/imbens/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/estimator_checks.py` & `imbalanced-ensemble-0.2.1/imbens/utils/estimator_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 def check_target_type(name, estimator_orig):
     estimator = clone(estimator_orig)
     # should raise warning if the target is continuous (we cannot raise error)
     X = np.random.random((20, 2))
     y = np.linspace(0, 1, 20)
-    msg = "Unknown label type: 'continuous'"
+    msg = "Unknown label type: continuous"
     assert_raises_regex(
         ValueError,
         msg,
         estimator.fit_resample,
         X,
         y,
     )
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/testing.py` & `imbalanced-ensemble-0.2.1/imbens/utils/testing.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_deprecation.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_docstring.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_estimator_checks.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_estimator_checks.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_plot.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_show_versions.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_show_versions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Test for the show_versions helper. Based on the sklearn tests."""
 # Author: Alexander L. Hayes <hayesall@iu.edu>
 # License: MIT
 
+# %%
 
 from imbens.utils._show_versions import _get_deps_info, show_versions
 
-_deps_info = _get_deps_info()
-
 
 def test_get_deps_info():
+    _deps_info = _get_deps_info()
     assert "pip" in _deps_info
     assert "setuptools" in _deps_info
     assert "imblearn" in _deps_info
     assert "imbens" in _deps_info
     assert "sklearn" in _deps_info
     assert "numpy" in _deps_info
     assert "scipy" in _deps_info
@@ -55,7 +55,10 @@
     assert "* sklearn" in out
     assert "* numpy" in out
     assert "* scipy" in out
     assert "* Cython" in out
     assert "* pandas" in out
     assert "* joblib" in out
     assert "</details>" in out
+
+
+# %%
```

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_testing.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_validation.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/utils/tests/test_validation_param.py` & `imbalanced-ensemble-0.2.1/imbens/utils/tests/test_validation_param.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/imbens/visualizer/visualizer.py` & `imbalanced-ensemble-0.2.1/imbens/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `imbalanced-ensemble-0.2.0/setup.py` & `imbalanced-ensemble-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     "doc": [
         "sphinx",
         "sphinx-gallery",
         "sphinx_rtd_theme",
         "pydata-sphinx-theme",
         "numpydoc",
         "sphinxcontrib-bibtex",
+        "torch",
+        "pytest",
     ],
 }
 
 setup(
     name=DISTNAME,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
@@ -97,8 +99,8 @@
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     zip_safe=False,  # the package can run out of an .egg file
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
-)
+)
```

