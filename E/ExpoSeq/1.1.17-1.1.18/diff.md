# Comparing `tmp/ExpoSeq-1.1.17.tar.gz` & `tmp/ExpoSeq-1.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.17.tar", last modified: Sun Jul 16 08:48:13 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.18.tar", last modified: Sat Jul 22 08:57:04 2023, max compression
```

## Comparing `ExpoSeq-1.1.17.tar` & `ExpoSeq-1.1.18.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/
--rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/MANIFEST.in
--rw-rw-rw-   0        0        0     5527 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/PKG-INFO
--rw-rw-rw-   0        0        0     5145 2023-07-15 16:34:55.000000 ExpoSeq-1.1.17/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-07-16 08:47:58.000000 ExpoSeq-1.1.17/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.063291 ExpoSeq-1.1.17/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.228323 ExpoSeq-1.1.17/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.382409 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6814 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    19695 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    40816 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.649602 ExpoSeq-1.1.17/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3295 2023-07-16 08:45:22.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1134 2023-07-16 08:42:06.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.754157 ExpoSeq-1.1.17/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.794589 ExpoSeq-1.1.17/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.900318 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.997740 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.292604 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     5527 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:04.672268 ExpoSeq-1.1.18/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/MANIFEST.in
+-rw-rw-rw-   0        0        0     7135 2023-07-22 08:57:04.671380 ExpoSeq-1.1.18/PKG-INFO
+-rw-rw-rw-   0        0        0     6753 2023-07-16 09:56:41.000000 ExpoSeq-1.1.18/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:57:04.673267 ExpoSeq-1.1.18/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-07-22 08:56:26.000000 ExpoSeq-1.1.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:02.505832 ExpoSeq-1.1.18/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:02.681195 ExpoSeq-1.1.18/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:03.133553 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    20375 2023-07-22 08:55:26.000000 ExpoSeq-1.1.18/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    40851 2023-07-16 09:24:37.000000 ExpoSeq-1.1.18/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:03.682277 ExpoSeq-1.1.18/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1134 2023-07-16 08:58:43.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-1.1.18/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:03.789225 ExpoSeq-1.1.18/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:03.795997 ExpoSeq-1.1.18/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:03.852969 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:04.369593 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:04.622619 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:57:02.693182 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     7135 2023-07-22 08:57:02.000000 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-22 08:57:02.000000 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:57:02.000000 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-22 08:57:02.000000 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 08:57:02.000000 ExpoSeq-1.1.18/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.17/LICENSE` & `ExpoSeq-1.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/PKG-INFO` & `ExpoSeq-1.1.18/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,67 @@
-Metadata-Version: 2.1
-Name: ExpoSeq
-Version: 1.1.17
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
-Home-page: https://github.com/nilshof01/ExpoSeq
-Author: Nils Hofmann
-Author-email: n.hofmann.99@web.de
-License: Apache License 2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples. It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
-You can also only use the test version without installing it.
+You can also only use the test version of ExpoSeq without installing it.
 
 ## Importing the Plotting Tool
 
 To access the plotting tool, you will need to import it into your console by running the following command:
+<br>
 ```from ExpoSeq.pipeline import PlotManager```
-
+<br>
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
+<br>
 ```import ExpoSeq.run```
+<br>
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
+<br>
 ```plot = PlotManager()```
+<br>
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
+<br>
 ![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
-If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
+<br>
+If you just want to test the pipeline and see its functions you can call:
+<br>
+ ```plot = PlotManager(test_version = True)```
+ <br>
+  Alternatively you can take a look in the [Jupyter script](ExpoSeq_handsOn.ipynb)
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
+<br>
 ```plot.jaccard()```
-If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
+<br>
+If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following:
+<br>
+ ```plot.style.title_xaxis("your_title")``` 
+ <br>
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
+<br>
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
+<br>
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
+## Upload binding data 
 
-# Processing on a server with multithreading
+If you have conducted DELFIA or other techniques to receive binding data for certain sequences (usually sanger sequenced), you can upload these in a certain format and use these for clustering to potentially find other suitable sequences with high binding.  You need to import the data as csv file where the first column starts in the first row with the header: aaSeqCDR3 which are the sequences. It is very important to keep the header at this position. In the second column you can put the binding data for your epitope which you can name in the first row however you prefer. You can have a look in [this csv file](src/ExpoSeq/test_data/test_files/binding_data.csv) to see the general structure of the file. Moreover, you can download it and import it in Excel. Therefore, open Excel and choose under "Data" in the Excel header "From Text/CSV". Then make sure to delete the first column which contains the row number. After that you can delete the random data in that excel sheet and add your own. Finally you can export the data as a csv and import it with the pipeline either in the initial uploading process which will be prompted or with the command 
+<br>
+```plot.add_binding_data()```
+<br>
+Note: If you decide to add more binding data to your analysis you can just use the same command and choose the new file with the filechooser and it will be added to the existing data.
+## Processing on a server with multithreading
 
 If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
 
 Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
 
 ### Required Inputs
 
@@ -67,15 +79,15 @@
 
 
 
 ## References
 [1] Dmitriy A. Bolotin, Stanislav Poslavsky, Igor Mitrophanov, Mikhail Shugay, Ilgar Z. Mamedov, Ekaterina V. Putintseva, and Dmitriy M. Chudakov. "MiXCR: software for comprehensive adaptive immunity profiling." Nature methods 12, no. 5 (2015): 380-381.
 
 
-[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908â€“911 (2017)
+[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908–911 (2017)
 
 [3] (1, 2) Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.
```

### Comparing `ExpoSeq-1.1.17/README.md` & `ExpoSeq-1.1.18/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,79 @@
+Metadata-Version: 2.1
+Name: ExpoSeq
+Version: 1.1.18
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
+Home-page: https://github.com/nilshof01/ExpoSeq
+Author: Nils Hofmann
+Author-email: n.hofmann.99@web.de
+License: Apache License 2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples. It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
-You can also only use the test version without installing it.
+You can also only use the test version of ExpoSeq without installing it.
 
 ## Importing the Plotting Tool
 
 To access the plotting tool, you will need to import it into your console by running the following command:
+<br>
 ```from ExpoSeq.pipeline import PlotManager```
-
+<br>
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
+<br>
 ```import ExpoSeq.run```
+<br>
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
+<br>
 ```plot = PlotManager()```
+<br>
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
+<br>
 ![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
-If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
+<br>
+If you just want to test the pipeline and see its functions you can call:
+<br>
+ ```plot = PlotManager(test_version = True)```
+ <br>
+  Alternatively you can take a look in the [Jupyter script](ExpoSeq_handsOn.ipynb)
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
+<br>
 ```plot.jaccard()```
-If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
+<br>
+If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following:
+<br>
+ ```plot.style.title_xaxis("your_title")``` 
+ <br>
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
+<br>
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
+<br>
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
+## Upload binding data 
 
-# Processing on a server with multithreading
+If you have conducted DELFIA or other techniques to receive binding data for certain sequences (usually sanger sequenced), you can upload these in a certain format and use these for clustering to potentially find other suitable sequences with high binding.  You need to import the data as csv file where the first column starts in the first row with the header: aaSeqCDR3 which are the sequences. It is very important to keep the header at this position. In the second column you can put the binding data for your epitope which you can name in the first row however you prefer. You can have a look in [this csv file](src/ExpoSeq/test_data/test_files/binding_data.csv) to see the general structure of the file. Moreover, you can download it and import it in Excel. Therefore, open Excel and choose under "Data" in the Excel header "From Text/CSV". Then make sure to delete the first column which contains the row number. After that you can delete the random data in that excel sheet and add your own. Finally you can export the data as a csv and import it with the pipeline either in the initial uploading process which will be prompted or with the command 
+<br>
+```plot.add_binding_data()```
+<br>
+Note: If you decide to add more binding data to your analysis you can just use the same command and choose the new file with the filechooser and it will be added to the existing data.
+## Processing on a server with multithreading
 
 If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
 
 Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
 
 ### Required Inputs
 
@@ -55,15 +91,15 @@
 
 
 
 ## References
 [1] Dmitriy A. Bolotin, Stanislav Poslavsky, Igor Mitrophanov, Mikhail Shugay, Ilgar Z. Mamedov, Ekaterina V. Putintseva, and Dmitriy M. Chudakov. "MiXCR: software for comprehensive adaptive immunity profiling." Nature methods 12, no. 5 (2015): 380-381.
 
 
-[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908–911 (2017)
+[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908â€“911 (2017)
 
 [3] (1, 2) Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.
```

### Comparing `ExpoSeq-1.1.17/setup.py` & `ExpoSeq-1.1.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.17",
+    version = "1.1.18",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/randomizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     # generate random indices where the splits should occur
     split_indices = np.sort(np.random.choice(range(1, len(binding_values)), num_splits, replace=False))
     # split the list into random parts
     split_lists = [(binding_values[i:j], aaSeq[i:j]) for i, j in zip([0]+split_indices, split_indices+[len(binding_values)])]
     for i in range(len(split_lists)):
         part_binding = split_lists[i][0]
         part_aaSeq = split_lists[i][1]
-        data = {"aaSeqCDR3": part_aaSeq, "Antibody " + str(i): part_binding}
+        data = {"aaSeqCDR3": part_aaSeq, "Epitope " + str(i): part_binding}
         intermediate_binding = pd.DataFrame(data)
         if i == 0:
             binding_data = intermediate_binding
         else:
             binding_data = pd.merge(binding_data, intermediate_binding,how = "left",on = "aaSeqCDR3")
     
     return binding_data
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.18/src/ExpoSeq/augment_data/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,26 +250,39 @@
     with open(glob_vars, "r") as f:
         data = f.read()
     data = literal_eval(data)
     data["last_experiment"] = experiment
     with open(glob_vars, "w") as f:
         f.write(str(data))
 
+def find_file_in_subdirectories(directory, filename):
+    for dirpath, dirnames, files in os.walk(directory):
+        if filename in files:
+            return os.path.join(dirpath, filename)
+    return None
+
 def check_last_exp(pkg_path, module_dir, testing):
     if not testing:
         glob_vars = os.path.join(pkg_path,
                                 "settings",
                                 "global_vars.txt")
         with open(glob_vars, "r") as f:
             data = f.read()
         data = literal_eval(data)
 
         last_experiment = data["last_experiment"]
         if last_experiment == "":
-            print("You have no experiments in your folder.")
+            if not bool(os.listdir(os.path.join(module_dir, "my_experiments"))):
+                print("You have no experiments in your folder.")
+            else:
+                subdirectory = find_file_in_subdirectories(os.path.join(module_dir, "my_experiments"), "sequencing_report.csv")
+                if subdirectory is not None:
+                    last_experiment = os.path.dirname(subdirectory)
+                else:
+                    print("The experiments in my experiment do not contain the sequencing report. You need to upload a new experiment.")
             repo_path = ""
         else:
             repo_path = os.path.join(module_dir,
                                    "my_experiments",
                                     last_experiment,
                                     "sequencing_report.csv")
     else:
@@ -291,15 +304,15 @@
         next_step = input("If you want to upload a new experiment press 1. If you want to choose another experiment press 2. ")
     else:
         next_step = testing_value
     return next_step
 
 def get_choose_method_input(testing, testing_value = None):
     if not testing:
-        processing = input("If you want to process your fastq files with mixcr press 1. If you want to upload already processed txt files with unique clones, press 2. If you want to upload an already processed sequencing report in table format, press 3.")
+        processing = input("If you want to process your fastq files with mixcr press 1. If you want to upload an already processed sequencing report in table format, press 2.")
     else:
         processing = testing_value
     return processing
 
 def get_experiment_name_input(testing = False):
     if not testing:
         experiment_name = input("Enter the name of the experiment you want to analyze")
@@ -312,17 +325,17 @@
     choose_method = get_choose_method_input(testing, testing_value)
     
     while True:
         if choose_method in ["1", "2", "3"]:
             if choose_method == "1":
             
                 sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
+         #   elif choose_method == "2":
+          #      sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
             elif choose_method == "2":
-                sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
-            elif choose_method == "3":
                 sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
             break
         else:
             print("Please enter a correct value.")
 
         
 
@@ -370,15 +383,14 @@
 
 def process_data_with_last_experiment(module_dir, last_experiment, testing):
     experiment = last_experiment
     sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
     return sequencing_report, all_alignment_reports, experiment
 
 def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
-   # module_dir = os.path.abspath("")
     module_dir = os.getcwd()
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
     
     if os.path.isfile(repo_path):
         continue_analysis = get_continue_analysis_input(last_experiment,
                                                         testing,
@@ -408,12 +420,14 @@
         sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,
                                                                                      repo_path,
                                                                                      testing,
                                                                                      upload_type,
                                                                                      paired_end_test,
                                                                                      experiment_column)
     if testing and experiment != "test_directory":
-        shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
+        shutil.rmtree(os.path.join(module_dir,
+                                   "my_experiments",
+                                   experiment))
     
     if not testing and experiment != "test_directory":
         write_last_exp(pkg_path, experiment)
     return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.18/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.18/src/ExpoSeq/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,14 @@
                      legend_settings = self.legend_settings)
             self.plot_type = "single"
             self.ax = self.fig.gca()
             self.style = PlotStyle(self.ax, self.plot_type)
             figManager = plt.get_current_fig_manager()
             figManager.window.showMaximized()
 
-
     def logoPlot_single(self,
                         sample,
                         highlight_specific_pos = False,
                         highlight_pos_range = False,
                         chosen_seq_length = 16):
         """
         :param sample: insert the sample name
@@ -507,15 +506,15 @@
         """
         :param sample: the sample you would like to analyze
         :param antigen: the toxins you would like to cluster
         :param antigen_names: Default is True. Prints the name of the toxin for the corresponding embedded sequence in the plot
         :param pca_components: optional. Default is 70
         :param perplexity: optional. Default 25
         :param iterations_tsne: optional. Default is 2500
-        :return: It first embeds the sequences in a vector space and then clusters them with PCA and TSNE. The sequences with the binding data are processed with the input sequences, to enable the plotting of the binding data.
+        :return: It first embeds the sequences in a vector space and then reduces the dimensions and clusters them with PCA and TSNE. The sequences with the binding data are processed with the input sequences, to enable the plotting of the binding data.
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         assert self.binding_data is not None, "You have not given binding data. You can add it with the add_binding_data function"
         assert type(sample) == str, "You have to give a string as input for the sample"
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
@@ -587,14 +586,15 @@
                         self.legend_settings,
                         self.font_settings)
         self.plot_type = "single"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
+        
     def morosita_horn(self, specific_experiments = False):
         """
         :param specific_experiments: you can give a list with specific experiments
         :return: Returns a matrix of the identity between your samples based on the Morosita Horn Index
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/length_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     ax.title.set_text(sample)
     ax.title.set_size(10)
     ax.set_ylabel("Read Count",
                     **font_settings)  # Y label
     ax.set_xlabel('Read Length',
                 **font_settings)  # X label
 
-#    original_fontsize = font_settings["fontsize"]
- #   font_settings["fontsize"] = 22
+    original_fontsize = font_settings["fontsize"]
+    font_settings["fontsize"] = 20
     plt.title("Length Distribution of " + sample,
               pad=12,
               **font_settings)
-  #  font_settings["fontsize"] = original_fontsize
+    font_settings["fontsize"] = original_fontsize
 
 
 
 def length_distribution_multi(fig, sequencing_report, samples,num_cols, font_settings, test_version = False):
     if samples == "all":
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.sort(unique_experiments)
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.18/src/ExpoSeq/plots/usq_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
     plt.xlabel("Total sampled sequences", **font_settings)
     plt.ylabel("Total Unique Sequences", **font_settings)
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 22
     plt.title("Sequencing depth of the given samples ",pad = 12, **font_settings)
     font_settings["fontsize"] = original_fontsize
     fig.tight_layout()
-
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.18/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.18/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.18/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.18/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.18/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.18/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.18/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.18/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,79 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.17
+Version: 1.1.18
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
 
-ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
+ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples. It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
 
 To get started, please download and follow the instructions for MiXCR under the following link: https://docs.milaboratories.com/mixcr/getting-started/installation/ 
-You can also only use the test version without installing it.
+You can also only use the test version of ExpoSeq without installing it.
 
 ## Importing the Plotting Tool
 
 To access the plotting tool, you will need to import it into your console by running the following command:
+<br>
 ```from ExpoSeq.pipeline import PlotManager```
-
+<br>
 If you want to use the fast and easy version you can ignore the rest of the instructions and just import in your Console:
+<br>
 ```import ExpoSeq.run```
+<br>
 ## Using the PlotManager
 
 The PlotManager is the main interface for creating various plots using your FASTQ data. You can create an instance of the PlotManager by running the following command:
+<br>
 ```plot = PlotManager()```
+<br>
 To use the PlotManager to create plots, you will need to upload your FASTQ data to the pipeline. This will automatically happen as soon as you have called the PlotManager. In the following you can obtain an insight in the worklow of the pipeline after the initial call. There, the blue boxes indicate your input, gray are optional inputs while black and red are processing steps and output, respectively.
+<br>
 ![relative_path_to_image](pictures_gen/workflow_ExpoSeq.png)
-If you just want to test the pipeline and see its functions you can call: ```plot = PlotManager(test_version = True)```
+<br>
+If you just want to test the pipeline and see its functions you can call:
+<br>
+ ```plot = PlotManager(test_version = True)```
+ <br>
+  Alternatively you can take a look in the [Jupyter script](ExpoSeq_handsOn.ipynb)
 
 Once you have called the test version or have finished the data processing, you can use the PlotManager to create a variety of plots, such as an identity plot based on the jaccard similarity. Here is an example of how to create this type of plot:
+<br>
 ```plot.jaccard()```
-If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
+<br>
+If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following:
+<br>
+ ```plot.style.title_xaxis("your_title")``` 
+ <br>
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
+<br>
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
+<br>
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
+## Upload binding data 
 
-# Processing on a server with multithreading
+If you have conducted DELFIA or other techniques to receive binding data for certain sequences (usually sanger sequenced), you can upload these in a certain format and use these for clustering to potentially find other suitable sequences with high binding.  You need to import the data as csv file where the first column starts in the first row with the header: aaSeqCDR3 which are the sequences. It is very important to keep the header at this position. In the second column you can put the binding data for your epitope which you can name in the first row however you prefer. You can have a look in [this csv file](src/ExpoSeq/test_data/test_files/binding_data.csv) to see the general structure of the file. Moreover, you can download it and import it in Excel. Therefore, open Excel and choose under "Data" in the Excel header "From Text/CSV". Then make sure to delete the first column which contains the row number. After that you can delete the random data in that excel sheet and add your own. Finally you can export the data as a csv and import it with the pipeline either in the initial uploading process which will be prompted or with the command 
+<br>
+```plot.add_binding_data()```
+<br>
+Note: If you decide to add more binding data to your analysis you can just use the same command and choose the new file with the filechooser and it will be added to the existing data.
+## Processing on a server with multithreading
 
 If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
 
 Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
 
 ### Required Inputs
```

### Comparing `ExpoSeq-1.1.17/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.18/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

