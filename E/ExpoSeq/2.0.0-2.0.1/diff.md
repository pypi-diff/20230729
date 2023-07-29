# Comparing `tmp/ExpoSeq-2.0.0.tar.gz` & `tmp/ExpoSeq-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-2.0.0.tar", last modified: Sat Jul 22 10:02:14 2023, max compression
+gzip compressed data, was "ExpoSeq-2.0.1.tar", last modified: Sat Jul 29 09:13:23 2023, max compression
```

## Comparing `ExpoSeq-2.0.0.tar` & `ExpoSeq-2.0.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.930553 ExpoSeq-2.0.0/
--rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7611 2023-07-22 10:02:14.929556 ExpoSeq-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-22 10:02:14.930553 ExpoSeq-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-07-22 10:02:06.000000 ExpoSeq-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.576110 ExpoSeq-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.608386 ExpoSeq-2.0.0/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.660349 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    20837 2023-07-22 10:01:16.000000 ExpoSeq-2.0.0/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    41099 2023-07-22 10:00:24.000000 ExpoSeq-2.0.0/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.762964 ExpoSeq-2.0.0/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1134 2023-07-16 08:58:43.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.0/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.788961 ExpoSeq-2.0.0/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.794960 ExpoSeq-2.0.0/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.852260 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.900073 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.924555 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:02:14.619395 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     7611 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 10:02:14.000000 ExpoSeq-2.0.0/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.069360 ExpoSeq-2.0.1/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7611 2023-07-29 09:13:23.068360 ExpoSeq-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7230 2023-07-22 09:38:55.000000 ExpoSeq-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 09:13:23.069360 ExpoSeq-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-07-29 09:08:42.000000 ExpoSeq-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.245892 ExpoSeq-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.411939 ExpoSeq-2.0.1/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.515143 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-07-29 09:01:16.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6813 2023-07-16 09:18:38.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    21027 2023-07-29 07:17:35.000000 ExpoSeq-2.0.1/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    41988 2023-07-29 09:12:18.000000 ExpoSeq-2.0.1/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.655911 ExpoSeq-2.0.1/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3292 2023-07-16 08:59:57.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7812 2023-07-29 09:06:08.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4607 2023-07-29 08:02:03.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1171 2023-07-29 08:02:14.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2540 2023-07-16 09:10:35.000000 ExpoSeq-2.0.1/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.752762 ExpoSeq-2.0.1/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.790457 ExpoSeq-2.0.1/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.863681 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.003345 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1142 2023-07-29 07:45:22.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:23.062364 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-29 09:13:22.464137 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     7611 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 09:13:22.000000 ExpoSeq-2.0.1/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-2.0.0/LICENSE` & `ExpoSeq-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/PKG-INFO` & `ExpoSeq-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.0
+Version: 2.0.1
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.0/README.md` & `ExpoSeq-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/setup.py` & `ExpoSeq-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "2.0.0",
+    version = "2.0.1",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/binding_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 try:
     import tkinter as tk
     from tkinter import filedialog
 except:
     pass
 
 def collect_binding_data(binding_data = None):
-    if binding_data == None:
+    if binding_data is None:
         binding_data = pd.DataFrame([])
     else:
         pass
     while True:
         # prompt the user to add a file
-        print("add your excel sheet with the binding data with the file chooser")
+        print("add your excel sheet as csv file with the binding data with the file chooser")
 
         try:
             binding_file = filedialog.askopenfilename()
         except:
             while True:
                 binding_file = input("copy and paste the path to your binding report")
                 if os.path.isfile(os.path.abspath(binding_file)):
                     break
                 else:
                     print("Please enter a valid filepath. ")
         if binding_file.endswith(".xlsx"):
             binding_new = pd.read_excel(binding_file)
         elif binding_file.endswith(".csv"):
             binding_new = pd.read_csv(binding_file)
+        assert binding_new.columns.to_list()[0] == "aaSeqCDR3", "Please change the header of the first column in your csv file to aaSeqCDR3"
         binding_data = pd.concat([binding_data, binding_new])
         response = input("Do you want to continue adding files? (Y/n) ")
         if response.lower() == "n":
             break
     return binding_data
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-2.0.1/src/ExpoSeq/augment_data/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,19 @@
             if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
                 replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
                 if replace in ["Y", "y", "n", "N"]:
                     break
                 else:
                     print("Please enter another name.")
             else:
+                replace = "n"
                 break
         if replace in ["Y", "y"]:
             shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
-            os.mkdir(os.path.join(module_dir, "my_experiments", experiment))
+
     else: 
         experiment = get_random_string(10)
     
     os.mkdir(os.path.join(module_dir,
                     "my_experiments",
                     experiment))
     return experiment
@@ -231,15 +232,18 @@
                     pickle.dump(experiment_dic, f)
                 break
             else:
                 print("Sorry, but we could not find the column Experiment in your sequencing report. Please check if you have this")
         else:
             print("Sorry, but the filepath you entered is invalid.")
     all_alignment_reports = None
-
+    sequencing_report.to_csv(os.path.join(module_dir,
+                                         "my_experiments",
+                                         experiment,
+                                         "sequencing_report.csv"))
     return sequencing_report,all_alignment_reports, experiment
 
 
 def find_file_in_subdirectories(directory, filename):
     for dirpath, dirnames, files in os.walk(directory):
         if filename in files:
             if os.path.basename(dirpath) != "test_directory":
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/full_pipe.py` & `ExpoSeq-2.0.1/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/pipeline.py` & `ExpoSeq-2.0.1/src/ExpoSeq/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,15 +169,16 @@
 
     def change_experiment_names(self, specific = None, change_whole_dic = False):
         """
         :param specific: optional parameter. You can use this function to change the names of a specific sample.
         :param change_whole_dic: optional Parameter. The renaming can be done by using a dictionary and map it to the labels. You can change multiple or all labels by adding the new dictionary for this parameter.
         :return:You can use this function to change the name of your samples. Thus, you can change the labels of your plots.
         """
-
+        self.unique_experiments = self.sequencing_report["Experiment"].unique().tolist()
+        self.unique_experiments = dict(zip(self.unique_experiments, self.unique_experiments))
         if specific != None:
             assert type(specific) == str, "You have to give a string (inside: "") as input for the specific sample you want to change"
         if change_whole_dic != False:
             assert type(change_whole_dic) == dict, "You have to give a dictionary as input for the specific sample you want to change"
         if change_whole_dic == False:
             if specific == None:
                 for key in self.unique_experiments:
@@ -374,15 +375,15 @@
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
 
     def lengthDistribution_multi(self,num_cols, samples = "all"):
         """
         :param num_cols: number of columns you want to have in your figure.
         :param samples: You analyze ExpoSeq samples per default. If you want to analyze specific samples it has to be a list with the corresponding sample names
-        :return: Outputs one figurewith one subplot per sample which shows you the distribution of sequence length
+        :return: Outputs one figure with one subplot per sample which shows you the distribution of the sequence length
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         if samples != "all":
             assert type(samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
@@ -405,15 +406,15 @@
     def rel_seq_abundance(self, samples, max_levenshtein_distance = 0, length_filter = 0, batch = 3000):
         """
 
         :param samples: For a qualitative analysis choose samples from the same panning experiment. Input is a list
         :param max_levenshtein_distance: Default is 0. You can change it to see increased fraction with increased variability of certain sequences
         :param length_filter: Default is 0. You should change it if you change the levenshtein distance. Otherwise your results will be biased.
         :param batch: Default is 3000. The size of the sample which is chosen. The higher it is, the more computational intense.
-        :return: Shows you a Bar Plot of the frequences of the most abundant sequences. You can introduce the levenshtein distance to see how the frequency changes with higher variability of the sequences.
+        :return: Shows you a bar plot of the frequencies of the most abundant sequences. You can introduce the levenshtein distance to see how the frequency changes with higher variability of the sequences.
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         incorrect_samples = [x for x in samples if x not in self.experiments_list]
         assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(samples) == list, "You have to give a list with the samples you want to analyze"
@@ -436,14 +437,17 @@
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
 
 
     def basic_cluster(self, sample,max_ld = 1, min_ld = 0, second_figure = False):
         """
         :param sample: type in a sample name you want to analyze
+        :max_ld: optional Parameter where its default is 1. Is the maximum Levenshtein distance you allow per cluster
+        :min_ld: optional Parameter where its default is 0. Is the minimum Levenshtein distance between sequences you allow
+        :second_figure: optional Parameter. Default is False. If you want to see the a histogram with the levenshtein distances, set it to True
         :return:
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(sample) == str, "You have to give a string as input for the sample"
@@ -469,20 +473,21 @@
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
         if second_figure == True:
             print("close the second window before you continue")
 
 
 
-    def cluster_one_AG(self, antigen,max_ld = 1, min_ld = 0, specific_experiments=False):
+    def cluster_one_AG(self, antigen,max_ld = 1, min_ld = 0,batch_size = 1000, specific_experiments=False):
         """
 
         :param antigen: is the name of the antigen you would like to analyze
         :param max_ld: optional Parameter where its default is 1. Is the maximum Levenshtein distance you allow per cluster
         :param min_ld: optional Parameter where its default is 0. Is the minimum Levenshtein distance between sequences you allow
+        :param batch_size: optional Parameter where its default is 1000. Is the batch size you want to use for the analysis
         :param specific_experiments: optional Parameter. You can give the names of specific samples in a list if you want
         :return: Creates a figure where sequences are clustered based on Levenshtein distance. Additionally the binding data of the sequences against a specific antigen is given.
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         assert self.binding_data is not None, "You have not given binding data. You can add it with the add_binding_data function"
@@ -493,15 +498,15 @@
         self.fig.clear()
         cluster_single_AG(self.fig,
                           self.sequencing_report,
                           antigen,
                           self.binding_data,
                           max_ld,
                           min_ld,
-                          self.batch_size,
+                          batch_size,
                           specific_experiments,
                           )
         self.plot_type = "multi"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
@@ -554,21 +559,23 @@
             tsne_results.to_csv(path_save_embedding, index=False)
 
     def embedding_tsne(self,
                        samples,
                        strands = True,
                        pca_components = 80,
                        perplexity = 30,
-                       iterations_tsne = 2500):
+                       iterations_tsne = 2500,
+                       batch_size = 1000):
         """
         :param samples: the samples you would like to compare towards their sequences
         :param strands: Default is True. It means that you will plot a batch of the strands in your plot
         :param pca_components: Default is 80. Has to be applied for better accuracy of t-SNE. You can indirectly change the described variance with this.
         :param perplexity: Default is 30. It roughly determines the number of nearest neighbors that are considered in the embedding. A higher perplexity value results in a more global structure in the low-dimensional embedding, while a lower perplexity value emphasizes local structure. The optimal perplexity value for a given dataset depends on the dataset's intrinsic dimensionality, and it is usually determined by trial and err
         :param iterations_tsne: Default is 2500. number of times that the algorithm will repeat the optimization process for reducing the cost function. The optimization process aims to minimize the difference between the high-dimensional and low-dimensional representations of the data. More iterations result in a more optimized low-dimensional representation, but also increases the computational cost.
+        :param batch_size: Default is 1000. The size of the sample which is chosen. The higher it is, the more computational intense.
         :return: Returns a plot where the sequences of the input samples are transformed in a vector space. Dimension reduction such as PCA and following t-SNE is used to plot it on a two dimensional space. The different colors indicate the different samples.
         """
         if not plt.fignum_exists(1):
             self.fig = plt.figure(1)
             print("Please do not close the window for the figure while the plot is loading")
         incorrect_samples = [x for x in samples if x not in self.experiments_list]
         assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
@@ -578,15 +585,15 @@
         assert type(perplexity) == int, "You have to give an integer as input for the perplexity"
         assert type(iterations_tsne) == int, "You have to give an integer as input for the iterations_tsne"
         self.fig.clear()
         self.ax = self.fig.gca()
         show_difference(self.sequencing_report,
                         samples,
                         strands,
-                        self.batch_size,
+                        batch_size,
                         pca_components,
                         perplexity,
                         iterations_tsne,
                         self.ax,
                         self.legend_settings,
                         self.font_settings)
         self.plot_type = "single"
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,21 @@
         ax2.set_xlabel("Degree", **font_settings)
         ax2.set_ylabel("# of Nodes", font_settings)
         return fig2
     else:
         return
 
 def cluster_single_AG(fig, sequencing_report, antigen, binding_data, max_ld, min_ld, batch_size, specific_experiments = False, ):
+    assert antigen in binding_data.columns, "it seems like your antigen does not exist in the binding data. Please enter the correct value"
     report_batch = sequencing_report.groupby("Experiment").head(batch_size)
     if specific_experiments != False:
         report_batch = report_batch[report_batch['Experiment'].isin(specific_experiments)]
     else:
         pass
+
     experiments = report_batch["Experiment"].unique()
     Tot = experiments.shape[0]
     Cols = int(input("How many Columns for the Plots do you want?"))
     Rows = Tot // Cols
     if Tot % Cols != 0:
         Rows += 1
     # Create a Position index
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/logo_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,24 @@
     aa_distribution, sequence_length, length_filtered_seqs = cleaning(sample,
                                                                       sequencing_report,
                                                                       chosen_seq_length)
     logo_plot = logomaker.Logo(aa_distribution,
                                shade_below=.5,
                                fade_below=.5,
                                font_name='Arial Rounded MT Bold',
+                               color_scheme="skylign_protein",
+                               show_spines=False,
                                ax=ax,
                                )
     logo_plot.style_xticks(anchor=0,
                            spacing=1,
                            rotation=0)
     original_fontsize = font_settings["fontsize"]
+    ax.set_xlabel("Frequency")
+    ax.set_ylabel("Position on sequence")
     font_settings["fontsize"] = 22
     plt.title("Logo Plot of " + sample + " with sequence length " + str(chosen_seq_length), **font_settings)
     font_settings["fontsize"] = original_fontsize
     if highlight_specific_pos != False:
         logo_plot.highlight_position(p=5,
                                      color='gold',
                                      alpha=.5)
@@ -62,14 +66,16 @@
                                  Cols,
                                  Position[n],
                                  xticks = (np.arange(0, chosen_seq_length, step = 1)))
             logo_plot = logomaker.Logo(aa_distribution,
                                         shade_below=.5,
                                         fade_below=.5,
                                         font_name='Arial Rounded MT Bold',
+                                        color_scheme="skylign_protein",
+                                        show_spines=False,
                                         ax=ax,
                                         )
             #logo_plot.set_xticks(range(aa_distribution.shape[0]))
             logo_plot.style_xticks(anchor=0,
                                    spacing=1,
                                    rotation=0,)
             plt.title(i, **font_settings) # check out https://matplotlib.org/3.1.0/api/_as_gen/matplotlib.pyplot.title.html
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     ax.set_xlabel('Position on amino acid sequence', **font_settings)
     if protein == True:
         ax.set_ylabel('Relatvie Proportion of Amino Acid', **font_settings)
     else:
         ax.set_ylabel('Relatvie Proportion of Nucleotide', **font_settings)
 
 #    ax.set_xticks(rotation = 360)
-    ax.legend(**legend_settings)
+    ax.legend(bbox_to_anchor=(1.05, 1), loc='upper left')
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 22
     if protein == True:
         ax.set_title("Distribution of Aminoacids per Position for your sequences",pad = 12, **font_settings)
     else:
         ax.set_title("Distribution of Nucleotides per Position for your sequences",pad = 12, **font_settings)
-    ax.set_xticklabels(ax.get_xticklabels(), rotation=0, ha='center')
+    ax.set_xticklabels([*range(region[0], region[1]+1)], rotation=0, ha='center')
     font_settings["fontsize"] = original_fontsize
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-2.0.1/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/reset.py` & `ExpoSeq-2.0.1/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-2.0.1/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-2.0.1/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-2.0.1/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-2.0.1/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/test_uploader.py` & `ExpoSeq-2.0.1/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def cleaning(report, max_ld, min_ld):
     aa = list(report["aaSeqCDR3"])
     num_strings = len(aa)
     string_index = [*range(0, num_strings, 1)]
     max_ld = max_ld
     min_ld = min_ld
     collect_coordinates = np.array([0, 0, 0]).reshape(1,3)
-    for i in range(len(string_index)):
+    for i in range(len(aa)):
         string1 = aa[i]
         index_1 = i
         for index in range(index_1):
             string2 = aa[index]
             distance = editdistance.distance(string1, string2)
             if distance>= min_ld and distance <= max_ld:
                 collect_coordinates = np.concatenate((collect_coordinates,
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-2.0.1/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-2.0.1/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 2.0.0
+Version: 2.0.1
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ExpoSeq-2.0.0/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-2.0.1/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

