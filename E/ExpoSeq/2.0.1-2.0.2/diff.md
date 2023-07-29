# Comparing `tmp/ExpoSeq-2.0.1.tar.gz` & `tmp/ExpoSeq-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-2.0.1.tar", last modified: Sat Jul 29 09:13:23 2023, max compression
+gzip compressed data, was "ExpoSeq-2.0.2.tar", last modified: Sat Jul 29 09:26:41 2023, max compression
```

## Comparing `ExpoSeq-2.0.1.tar` & `ExpoSeq-2.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.069360 ExpoSeq-2.0.1/
--rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7611 2023-07-29 09:13:23.068360 ExpoSeq-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 09:13:23.069360 ExpoSeq-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-07-29 09:08:42.000000 ExpoSeq-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.245892 ExpoSeq-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.411939 ExpoSeq-2.0.1/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.515143 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-07-29 09:01:16.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    21027 2023-07-29 07:17:35.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    41988 2023-07-29 09:12:18.000000 ExpoSeq-2.0.1/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.655911 ExpoSeq-2.0.1/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7812 2023-07-29 09:06:08.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4607 2023-07-29 08:02:03.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1171 2023-07-29 08:02:14.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.752762 ExpoSeq-2.0.1/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.790457 ExpoSeq-2.0.1/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.863681 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.003345 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1142 2023-07-29 07:45:22.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.062364 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.464137 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     7611 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.775496 ExpoSeq-2.0.2/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7611 2023-07-29 09:26:41.774562 ExpoSeq-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:26:41.775496 ExpoSeq-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-07-29 09:26:17.000000 ExpoSeq-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.217673 ExpoSeq-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.267675 ExpoSeq-2.0.2/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.367945 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-07-29 09:01:16.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    21027 2023-07-29 07:17:35.000000 ExpoSeq-2.0.2/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    41988 2023-07-29 09:12:18.000000 ExpoSeq-2.0.2/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.563519 ExpoSeq-2.0.2/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7812 2023-07-29 09:06:08.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4641 2023-07-29 09:26:08.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1171 2023-07-29 08:02:14.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.2/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.588216 ExpoSeq-2.0.2/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.594219 ExpoSeq-2.0.2/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.640618 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.740570 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1142 2023-07-29 07:45:22.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.769477 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:26:41.279684 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     7611 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 09:26:41.000000 ExpoSeq-2.0.2/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-2.0.1/LICENSE` & `ExpoSeq-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/PKG-INFO` & `ExpoSeq-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.1
+Version: 2.0.2
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.1/README.md` & `ExpoSeq-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/setup.py` & `ExpoSeq-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "2.0.1",
+    version = "2.0.2",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-2.0.2/src/ExpoSeq/augment_data/uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/full_pipe.py` & `ExpoSeq-2.0.2/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/pipeline.py` & `ExpoSeq-2.0.2/src/ExpoSeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/logo_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                                show_spines=False,
                                ax=ax,
                                )
     logo_plot.style_xticks(anchor=0,
                            spacing=1,
                            rotation=0)
     original_fontsize = font_settings["fontsize"]
-    ax.set_xlabel("Frequency")
-    ax.set_ylabel("Position on sequence")
+    ax.set_xlabel("Frequency", **font_settings)
+    ax.set_ylabel("Position on sequence", **font_settings)
     font_settings["fontsize"] = 22
     plt.title("Logo Plot of " + sample + " with sequence length " + str(chosen_seq_length), **font_settings)
     font_settings["fontsize"] = original_fontsize
     if highlight_specific_pos != False:
         logo_plot.highlight_position(p=5,
                                      color='gold',
                                      alpha=.5)
```

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-2.0.2/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/reset.py` & `ExpoSeq-2.0.2/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-2.0.2/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-2.0.2/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-2.0.2/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-2.0.2/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/test_uploader.py` & `ExpoSeq-2.0.2/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-2.0.2/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-2.0.2/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.1
+Version: 2.0.2
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.1/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-2.0.2/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

