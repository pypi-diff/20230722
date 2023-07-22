# Comparing `tmp/ExpoSeq-1.1.19.tar.gz` & `tmp/ExpoSeq-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.19.tar", last modified: Sat Jul 22 09:39:39 2023, max compression
+gzip compressed data, was "ExpoSeq-2.0.0.tar", last modified: Sat Jul 22 10:02:14 2023, max compression
```

## Comparing `ExpoSeq-1.1.19.tar` & `ExpoSeq-2.0.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.394540 ExpoSeq-1.1.19/
--rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/MANIFEST.in
--rw-rw-rw-   0        0        0     7612 2023-07-22 09:39:39.393540 ExpoSeq-1.1.19/PKG-INFO
--rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-1.1.19/README.md
--rw-rw-rw-   0        0        0       42 2023-07-22 09:39:39.394540 ExpoSeq-1.1.19/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-07-22 09:39:24.000000 ExpoSeq-1.1.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.039669 ExpoSeq-1.1.19/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.078669 ExpoSeq-1.1.19/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.135937 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17254 2023-07-22 09:38:22.000000 ExpoSeq-1.1.19/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    41099 2023-07-22 09:37:46.000000 ExpoSeq-1.1.19/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.236755 ExpoSeq-1.1.19/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1134 2023-07-16 08:58:43.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-1.1.19/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.259448 ExpoSeq-1.1.19/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.264441 ExpoSeq-1.1.19/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.319848 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.365755 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.389538 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:39:39.090552 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     7612 2023-07-22 09:39:38.000000 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-07-22 09:39:38.000000 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:39:38.000000 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-22 09:39:38.000000 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 09:39:38.000000 ExpoSeq-1.1.19/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.930553 ExpoSeq-2.0.0/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7611 2023-07-22 10:02:14.929556 ExpoSeq-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 10:02:14.930553 ExpoSeq-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-07-22 10:02:06.000000 ExpoSeq-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.576110 ExpoSeq-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.608386 ExpoSeq-2.0.0/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.660349 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    20837 2023-07-22 10:01:16.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    41099 2023-07-22 10:00:24.000000 ExpoSeq-2.0.0/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.762964 ExpoSeq-2.0.0/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1134 2023-07-16 08:58:43.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.788961 ExpoSeq-2.0.0/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.794960 ExpoSeq-2.0.0/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.852260 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.900073 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.924555 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.619395 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     7611 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.19/LICENSE` & `ExpoSeq-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/PKG-INFO` & `ExpoSeq-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.19
+Version: 2.0.0
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.19/README.md` & `ExpoSeq-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/setup.py` & `ExpoSeq-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.19",
+    version = "2.0.0",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/uploader.py`

 * *Files 12% similar despite different names*

```diff
@@ -234,39 +234,60 @@
                 print("Sorry, but we could not find the column Experiment in your sequencing report. Please check if you have this")
         else:
             print("Sorry, but the filepath you entered is invalid.")
     all_alignment_reports = None
 
     return sequencing_report,all_alignment_reports, experiment
 
+
+def find_file_in_subdirectories(directory, filename):
+    for dirpath, dirnames, files in os.walk(directory):
+        if filename in files:
+            if os.path.basename(dirpath) != "test_directory":
+                return os.path.join(dirpath, filename)
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
-            repo_path = ""
+            if not bool(os.listdir(os.path.join(module_dir, "my_experiments"))):
+                repo_path = ""
+                print("You have no experiments in your folder.")
+            else:
+                subdirectory = find_file_in_subdirectories(os.path.join(module_dir, "my_experiments"), "sequencing_report.csv")
+                if subdirectory is not None:
+                    repo_path = subdirectory
+                    dirpath = os.path.dirname(subdirectory)
+                    last_experiment = os.path.basename(dirpath)
+                else:
+                    print("The experiments in my experiment do not contain the sequencing report. You need to upload a new experiment.")
+            
         else:
             repo_path = os.path.join(module_dir,
-                                    "my_experiments",
+                                   "my_experiments",
                                     last_experiment,
                                     "sequencing_report.csv")
     else:
         repo_path = os.path.join(module_dir,
                                 "my_experiments",
                                 "test_directory",
                                 "sequencing_report.csv")
         last_experiment = "test_directory"
     return repo_path, last_experiment
+
+
+
 def get_continue_analysis_input(last_experiment, testing=False, testing_value = None):
     if not testing:
         continue_input = input("Do you want to continue to analyze with " + last_experiment + "? Y/n")
     else:
         continue_input = testing_value
     return continue_input
 
@@ -275,15 +296,15 @@
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
@@ -291,23 +312,28 @@
         experiment_name = get_random_string(10)
     return experiment_name  
 
 def upload_new_experiment(module_dir, repo_path, testing, testing_value, paired_end_test, experiment_column):
     experiment = check_experiment(module_dir, testing)
     choose_method = get_choose_method_input(testing, testing_value)
     
-    if choose_method == "1":
+    while True:
+        if choose_method in ["1", "2", "3"]:
+            if choose_method == "1":
+            
+                sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
+         #   elif choose_method == "2":
+          #      sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
+            elif choose_method == "2":
+                sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
+            break
+        else:
+            print("Please enter a correct value.")
+
         
-        sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
-    elif choose_method == "2":
-        sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
-    elif choose_method == "3":
-        sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
-    else:
-        raise ValueError("Invalid option")
 
     return sequencing_report, all_alignment_reports, experiment
 
 def choose_existing_experiment(module_dir, testing):
     if not testing:
         while True:
             user_input = get_experiment_name_input()
@@ -328,51 +354,97 @@
         align_repo_path = os.path.join(module_dir,
                             "my_experiments",
                             experiment,
                             "alignment_reports", "*")
     else:
         seq_report_path = os.path.join(module_dir, "my_experiments", "test_directory", "sequencing_report.csv")
         align_repo_path = os.path.join(module_dir, "tests", "test_directory", "all_alignment_reports.pickle")
-    with open(seq_report_path, "rb") as f:
-        sequencing_report = pd.read_table(f, sep=",")
-    try:
-        align_repo_path = os.path.join(module_dir,
-                                    "my_experiments",
-                                    experiment,
-                                    "alignment_reports", "*")
-        alignment_reports = glob(align_repo_path)
-        all_alignment_reports = load_alignment_reports(alignment_reports)
-    except:
-        all_alignment_reports = pd.DataFrame([])
-        print("No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+    if os.path.isfile(seq_report_path):
+        with open(seq_report_path, "rb") as f:
+            sequencing_report = pd.read_table(f, sep=",")
+        try:
+            align_repo_path = os.path.join(module_dir,
+                                        "my_experiments",
+                                        experiment,
+                                        "alignment_reports", "*")
+            alignment_reports = glob(align_repo_path)
+            all_alignment_reports = load_alignment_reports(alignment_reports)
+        except:
+            all_alignment_reports = pd.DataFrame([])
+            print("No alignment reports could be found in " + experiment + ". You will continue without being able to analyze the Alignment Quality.")
+    else:
+        print("The sequencing report could not be found in " + experiment + ". Please enter an experiment with an existing sequencing_report.csv file or upload new data.")
+        sequencing_report = None
+        all_alignment_reports = None
+        experiment = None
 
     return sequencing_report, all_alignment_reports, experiment
 
 def process_data_with_last_experiment(module_dir, last_experiment, testing):
     experiment = last_experiment
     sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
     return sequencing_report, all_alignment_reports, experiment
 
+
+
+def write_last_exp(pkg_path, experiment):
+    glob_vars = os.path.join(pkg_path,
+                             "settings",
+                             "global_vars.txt")
+    with open(glob_vars, "r") as f:
+        data = f.read()
+    data = literal_eval(data)
+    data["last_experiment"] = experiment
+    with open(glob_vars, "w") as f:
+        f.write(str(data))
+
 def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
-   # module_dir = os.path.abspath("")
     module_dir = os.getcwd()
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
-
+    
     if os.path.isfile(repo_path):
-        continue_analysis = get_continue_analysis_input(last_experiment, testing,continue_analysis)
+        continue_analysis = get_continue_analysis_input(last_experiment,
+                                                        testing,
+                                                        continue_analysis)
         if continue_analysis.lower() in ["n", "no"]:
             next_step = get_next_step_input(testing, choose_exp)
-            if next_step == "1":
-                sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,repo_path, testing, upload_type, paired_end_test, experiment_column)
-            elif next_step == "2":
-                experiment = choose_existing_experiment(module_dir, testing)
-                sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir, experiment, testing)
-            else:
-                raise ValueError("Invalid option")
+            while True:
+                if next_step == "1":
+                    
+                    sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,
+                                                                                                repo_path,
+                                                                                                testing,
+                                                                                                upload_type,
+                                                                                                paired_end_test,
+                                                                                                experiment_column)
+                elif next_step == "2":
+                    experiment = choose_existing_experiment(module_dir,
+                                                            testing)
+                    sequencing_report, all_alignment_reports, experiment = retrieve_reports(module_dir,
+                                                                                            experiment,
+                                                                                            testing)
+                if isinstance(sequencing_report, pd.DataFrame):
+                    break
+                else:
+                    print("Something went wrong. Please try again.")
+                    
+
         else:
-            sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir, last_experiment, testing)
-    else:
-        sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir, repo_path, testing, upload_type, paired_end_test, experiment_column)
+            sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir,
+                                                                                                     last_experiment,
+                                                                                                     testing)
+    else:
+        sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir,
+                                                                                     repo_path,
+                                                                                     testing,
+                                                                                     upload_type,
+                                                                                     paired_end_test,
+                                                                                     experiment_column)
     if testing and experiment != "test_directory":
-        shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
-    return sequencing_report, all_alignment_reports, experiment
+        shutil.rmtree(os.path.join(module_dir,
+                                   "my_experiments",
+                                   experiment))
+    
+    if not testing and experiment != "test_directory":
+        write_last_exp(pkg_path, experiment)
+    return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/full_pipe.py` & `ExpoSeq-2.0.0/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/pipeline.py` & `ExpoSeq-2.0.0/src/ExpoSeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-2.0.0/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/reset.py` & `ExpoSeq-2.0.0/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-2.0.0/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-2.0.0/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-2.0.0/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/test_uploader.py` & `ExpoSeq-2.0.0/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-2.0.0/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.19
+Version: 2.0.0
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-1.1.19/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-2.0.0/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

