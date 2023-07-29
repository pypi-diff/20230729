# Comparing `tmp/pypmc-1.2.1.tar.gz` & `tmp/pypmc-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypmc-1.2.1.tar", last modified: Sat Jul 29 15:20:03 2023, max compression
+gzip compressed data, was "pypmc-1.2.2.tar", last modified: Sat Jul 29 17:50:49 2023, max compression
```

## Comparing `pypmc-1.2.1.tar` & `pypmc-1.2.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.247624 pypmc-1.2.1/
--rw-r--r--   0 root         (0) root         (0)    18026 2023-07-29 15:15:17.000000 pypmc-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 15:15:17.000000 pypmc-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1961 2023-07-29 15:20:03.243625 pypmc-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2481 2023-07-29 15:15:17.000000 pypmc-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.227625 pypmc-1.2.1/pypmc/
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.231624 pypmc-1.2.1/pypmc/density/
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/base.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/base_test.py
--rw-r--r--   0 root         (0) root         (0)  1291350 2023-07-29 15:17:50.000000 pypmc-1.2.1/pypmc/density/gauss.c
--rw-r--r--   0 root         (0) root         (0)     5683 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/gauss.pyx
--rw-r--r--   0 root         (0) root         (0)     6743 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/gauss_test.py
--rw-r--r--   0 root         (0) root         (0)   736213 2023-07-29 15:17:50.000000 pypmc-1.2.1/pypmc/density/mixture.c
--rw-r--r--   0 root         (0) root         (0)    11852 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/mixture.pyx
--rw-r--r--   0 root         (0) root         (0)    11946 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/mixture_test.py
--rw-r--r--   0 root         (0) root         (0)  1289453 2023-07-29 15:17:51.000000 pypmc-1.2.1/pypmc/density/student_t.c
--rw-r--r--   0 root         (0) root         (0)     6022 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/student_t.pyx
--rw-r--r--   0 root         (0) root         (0)     8770 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/density/student_t_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.239625 pypmc-1.2.1/pypmc/mix_adapt/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7688 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/hierarchical.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/hierarchical_test.py
--rw-r--r--   0 root         (0) root         (0)  1648088 2023-07-29 15:17:52.000000 pypmc-1.2.1/pypmc/mix_adapt/pmc.c
--rw-r--r--   0 root         (0) root         (0)    27594 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/pmc.pyx
--rw-r--r--   0 root         (0) root         (0)    40727 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/pmc_test.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/r_value.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/r_value_test.py
--rw-r--r--   0 root         (0) root         (0)  2391866 2023-07-29 15:17:53.000000 pypmc-1.2.1/pypmc/mix_adapt/variational.c
--rw-r--r--   0 root         (0) root         (0)    46823 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/variational.pyx
--rw-r--r--   0 root         (0) root         (0)    30923 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/mix_adapt/variational_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.239625 pypmc-1.2.1/pypmc/sampler/
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/sampler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13342 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/sampler/importance_sampling.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/sampler/importance_sampling_test.py
--rw-r--r--   0 root         (0) root         (0)    16011 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/sampler/markov_chain.py
--rw-r--r--   0 root         (0) root         (0)    13390 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/sampler/markov_chain_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.243625 pypmc-1.2.1/pypmc/tools/
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_doc.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_history.py
--rw-r--r--   0 root         (0) root         (0)  1114612 2023-07-29 15:17:54.000000 pypmc-1.2.1/pypmc/tools/_linalg.c
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_linalg.pxd
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_linalg.pyx
--rw-r--r--   0 root         (0) root         (0)     3104 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_partition.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_plot.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_probability_densities.py
--rw-r--r--   0 root         (0) root         (0)   442415 2023-07-29 15:17:54.000000 pypmc-1.2.1/pypmc/tools/_regularize.c
--rw-r--r--   0 root         (0) root         (0)      278 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_regularize.pxd
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/_regularize.pyx
--rw-r--r--   0 root         (0) root         (0)     1542 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/convergence.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/convergence_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.243625 pypmc-1.2.1/pypmc/tools/indicator/
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/indicator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3088 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/indicator/_indicator_factory.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/indicator/_indicator_merge.py
--rw-r--r--   0 root         (0) root         (0)     5481 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/indicator/indicator_factory_test.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/linalg_test.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/parallel_sampler.py
--rw-r--r--   0 root         (0) root         (0)     5753 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/parallel_sampler_test.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/partition_test.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/plot_test.py
--rw-r--r--   0 root         (0) root         (0)      688 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/regularize_test.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-29 15:15:17.000000 pypmc-1.2.1/pypmc/tools/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:20:03.227625 pypmc-1.2.1/pypmc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1961 2023-07-29 15:20:02.000000 pypmc-1.2.1/pypmc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1780 2023-07-29 15:20:02.000000 pypmc-1.2.1/pypmc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 15:20:02.000000 pypmc-1.2.1/pypmc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-29 15:20:02.000000 pypmc-1.2.1/pypmc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-29 15:20:02.000000 pypmc-1.2.1/pypmc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-07-29 15:15:17.000000 pypmc-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 15:20:03.247624 pypmc-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3051 2023-07-29 15:15:17.000000 pypmc-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.730521 pypmc-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)    18026 2023-07-29 17:46:03.000000 pypmc-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 17:46:03.000000 pypmc-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-07-29 17:50:49.730521 pypmc-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-29 17:46:03.000000 pypmc-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.714521 pypmc-1.2.2/pypmc/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.718520 pypmc-1.2.2/pypmc/density/
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/base.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/base_test.py
+-rw-r--r--   0 root         (0) root         (0)  1291350 2023-07-29 17:48:34.000000 pypmc-1.2.2/pypmc/density/gauss.c
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/gauss.pyx
+-rw-r--r--   0 root         (0) root         (0)     6743 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/gauss_test.py
+-rw-r--r--   0 root         (0) root         (0)   736213 2023-07-29 17:48:34.000000 pypmc-1.2.2/pypmc/density/mixture.c
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/mixture.pyx
+-rw-r--r--   0 root         (0) root         (0)    11946 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/mixture_test.py
+-rw-r--r--   0 root         (0) root         (0)  1289453 2023-07-29 17:48:35.000000 pypmc-1.2.2/pypmc/density/student_t.c
+-rw-r--r--   0 root         (0) root         (0)     6022 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/student_t.pyx
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/density/student_t_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.722520 pypmc-1.2.2/pypmc/mix_adapt/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/hierarchical.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/hierarchical_test.py
+-rw-r--r--   0 root         (0) root         (0)  1648088 2023-07-29 17:48:36.000000 pypmc-1.2.2/pypmc/mix_adapt/pmc.c
+-rw-r--r--   0 root         (0) root         (0)    27594 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/pmc.pyx
+-rw-r--r--   0 root         (0) root         (0)    40636 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/pmc_test.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/r_value.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/r_value_test.py
+-rw-r--r--   0 root         (0) root         (0)  2391866 2023-07-29 17:48:37.000000 pypmc-1.2.2/pypmc/mix_adapt/variational.c
+-rw-r--r--   0 root         (0) root         (0)    46823 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/variational.pyx
+-rw-r--r--   0 root         (0) root         (0)    30832 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/mix_adapt/variational_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.722520 pypmc-1.2.2/pypmc/sampler/
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/sampler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/sampler/importance_sampling.py
+-rw-r--r--   0 root         (0) root         (0)    16906 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/sampler/importance_sampling_test.py
+-rw-r--r--   0 root         (0) root         (0)    16011 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/sampler/markov_chain.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/sampler/markov_chain_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.730521 pypmc-1.2.2/pypmc/tools/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_doc.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_history.py
+-rw-r--r--   0 root         (0) root         (0)  1114612 2023-07-29 17:48:38.000000 pypmc-1.2.2/pypmc/tools/_linalg.c
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_linalg.pxd
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_linalg.pyx
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_partition.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_plot.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_probability_densities.py
+-rw-r--r--   0 root         (0) root         (0)   442415 2023-07-29 17:48:39.000000 pypmc-1.2.2/pypmc/tools/_regularize.c
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_regularize.pxd
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/_regularize.pyx
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/convergence.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/convergence_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.730521 pypmc-1.2.2/pypmc/tools/indicator/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/indicator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/indicator/_indicator_factory.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/indicator/_indicator_merge.py
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/indicator/indicator_factory_test.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/linalg_test.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/parallel_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/parallel_sampler_test.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/partition_test.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/plot_test.py
+-rw-r--r--   0 root         (0) root         (0)      688 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/regularize_test.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-29 17:46:03.000000 pypmc-1.2.2/pypmc/tools/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 17:50:49.714521 pypmc-1.2.2/pypmc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-07-29 17:50:48.000000 pypmc-1.2.2/pypmc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-29 17:50:48.000000 pypmc-1.2.2/pypmc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 17:50:48.000000 pypmc-1.2.2/pypmc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-29 17:50:48.000000 pypmc-1.2.2/pypmc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-29 17:50:48.000000 pypmc-1.2.2/pypmc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-29 17:46:03.000000 pypmc-1.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 17:50:49.730521 pypmc-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-07-29 17:46:03.000000 pypmc-1.2.2/setup.py
```

### Comparing `pypmc-1.2.1/LICENSE` & `pypmc-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/PKG-INFO` & `pypmc-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypmc
-Version: 1.2.1
+Version: 1.2.2
 Summary: A toolkit for adaptive importance sampling featuring implementations of variational Bayes, population Monte Carlo, and Markov chains.
 Home-page: https://github.com/pypmc/pypmc
 Author: Frederik Beaujean, Stephan Jahn
 Author-email: beaujean@mytum.de, stephan.jahn@mytum.de
 License: GPLv2
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pypmc-1.2.1/README.md` & `pypmc-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/base.py` & `pypmc-1.2.2/pypmc/density/base.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/base_test.py` & `pypmc-1.2.2/pypmc/density/base_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/gauss.c` & `pypmc-1.2.2/pypmc/density/gauss.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/gauss.pyx` & `pypmc-1.2.2/pypmc/density/gauss.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/gauss_test.py` & `pypmc-1.2.2/pypmc/density/gauss_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/mixture.c` & `pypmc-1.2.2/pypmc/density/mixture.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/mixture.pyx` & `pypmc-1.2.2/pypmc/density/mixture.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/mixture_test.py` & `pypmc-1.2.2/pypmc/density/mixture_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/student_t.c` & `pypmc-1.2.2/pypmc/density/student_t.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/student_t.pyx` & `pypmc-1.2.2/pypmc/density/student_t.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/density/student_t_test.py` & `pypmc-1.2.2/pypmc/density/student_t_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/hierarchical.py` & `pypmc-1.2.2/pypmc/mix_adapt/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/hierarchical_test.py` & `pypmc-1.2.2/pypmc/mix_adapt/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/pmc.c` & `pypmc-1.2.2/pypmc/mix_adapt/pmc.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/pmc.pyx` & `pypmc-1.2.2/pypmc/mix_adapt/pmc.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/pmc_test.py` & `pypmc-1.2.2/pypmc/mix_adapt/pmc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 '''
 
 from .pmc import *
 from .. import density
 import numpy as np
 import unittest
-from nose.plugins.attrib import attr
 
 class TestGaussianPMCNoOverlap(unittest.TestCase):
     # proposal density
     mu1 = np.array( [ 10., -1.0, 8.0] )
     mu2 = np.array( [-10.,  7.4, 0.5] )
 
     cov1 = np.array([[1.15 , 0.875, 0.0],
@@ -391,15 +390,14 @@
     def test_adaptation(self):
         pmc = PMC(self.samples, self.prop, self.weights, latent=self.latent, rb=False)
         converged = pmc.run()
         outdensity = pmc.density
 
         self.assertEqual(converged, 2)
 
-    @attr('slow')
     def test_with_overlap(self):
         # proposal density
         mu1 = np.array([ 10.5,   1.1,   8.0])
         mu2 = np.array([ 10.3,   1.4,   7.8])
 
         cov1 = np.array([[1.15 , 0.875, 0.0],
                          [0.875, 0.75 ,-0.2],
@@ -434,15 +432,14 @@
         np.testing.assert_allclose(adapted_comp_weights, component_weights, atol=0.01)
         np.testing.assert_allclose(adapted_mu1         , mu1              , rtol=0.01)
         np.testing.assert_allclose(adapted_mu2         , mu2              , rtol=0.01)
         np.testing.assert_allclose(adapted_sigma1      , cov1             , atol=0.03)
         np.testing.assert_allclose(adapted_sigma2      , cov2             , atol=0.06)
         # less samples from second component due to smaller component weight --> estimate less accurate
 
-    @attr('slow')
     def test_prune(self):
         # proposal density
         mu1 = np.array([ 10.5,   1.1,   8.0])
         mu2 = np.array([ 10.3,   1.4,   7.8])
 
         cov1 = np.array([[1.15 , 0.875, 0.0],
                          [0.875, 0.75 ,-0.2],
@@ -485,15 +482,14 @@
         np.testing.assert_allclose(adapted_sigma2      , cov2             , atol=0.06)
         # less samples from second component due to smaller component weight --> estimate less accurate
 
 class TestStudentTPMCMultipleUpdates(unittest.TestCase):
     def setUp(self):
         np.random.mtrand.seed(3026281795684 % 4294967296)
 
-    @attr('slow')
     def test_prune(self):
         # proposal density
         mu1 = np.array([ 10.5,   1.1,   8.0])
         mu2 = np.array([ 10.3,   1.4,   7.8])
 
         sigma1 = np.array([[1.15 , 0.875, 0.0],
                            [0.875, 0.75 ,-0.2],
```

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/r_value.py` & `pypmc-1.2.2/pypmc/mix_adapt/r_value.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/r_value_test.py` & `pypmc-1.2.2/pypmc/mix_adapt/r_value_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/variational.c` & `pypmc-1.2.2/pypmc/mix_adapt/variational.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/variational.pyx` & `pypmc-1.2.2/pypmc/mix_adapt/variational.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/mix_adapt/variational_test.py` & `pypmc-1.2.2/pypmc/mix_adapt/variational_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..density.gauss import Gauss
 from ..density.student_t import StudentT
 from ..density.mixture import MixtureDensity, create_gaussian_mixture, recover_gaussian_mixture
 from ..sampler import importance_sampling
 from ..tools._probability_densities import unnormalized_log_pdf_gauss, normalized_pdf_gauss
 
 import copy
-from nose.plugins.attrib import attr
 import numpy as np
 from scipy.special import digamma
 import unittest
 
 def check_bound(test_case, variational, n=20, prune=True):
     bound = variational.likelihood_bound()
     old_K = variational.K
@@ -287,15 +286,14 @@
 
         # check W
         inv_W = inv_W0 + N_comp[0]*S + (infer.beta0*N_comp[0]) / (infer.beta0 + N_comp[0]) *\
                 np.outer(x_mean_comp[0], x_mean_comp[0])
         W     = np.linalg.inv(inv_W)
         np.testing.assert_allclose(infer.W[0], W)
 
-    @attr('slow')
     def test_weighted(self):
         # this test uses pypmc.pmc.importance_sampling --> before debugging here,
         # first make sure that importance_sampling works
 
         # -------------------------------- generate weighted test data ----------------------------------
         # target
         target_abundances = np.array((.7, .3))
@@ -386,15 +384,14 @@
 
         for key in expected_posterior_as_prior:
             np.testing.assert_allclose(posterior_as_prior[key], expected_posterior_as_prior[key])
 
         # try creation of new GaussianInference instance with these values
         GaussianInference(samples, **posterior_as_prior)
 
-    @attr('slow')
     def test_prune(self):
         # generate test data from two independent gaussians
         target_abundances = np.array((.1, .9))
         target_mean1 = np.array((+1. , -4.))
         target_mean2 = np.array((-5. , +2.))
         target_cov1  = covariance1
         target_cov2  = covariance2
@@ -614,15 +611,14 @@
         self.assertEqual(vb2.likelihood_bound(), vb.likelihood_bound())
 
         # parameters should be identical at fixed point
         params2 = vb2.prior_posterior()
         for k, v in params2.items():
             np.testing.assert_array_equal(v, pripos[k])
 
-    @attr('slow')
     def test_large_prune(self):
         #Compress large number of similar components into a single component.
 
         means = (np.array([5, 0]),)
         cov = np.eye(2)
         N = 500
         N_input = 300
```

### Comparing `pypmc-1.2.1/pypmc/sampler/importance_sampling.py` & `pypmc-1.2.2/pypmc/sampler/importance_sampling.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/sampler/importance_sampling_test.py` & `pypmc-1.2.2/pypmc/sampler/importance_sampling_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 '''
 
 from .importance_sampling import *
 from .. import density
 from ..density.mixture_test import DummyComponent
 from ..tools._probability_densities import unnormalized_log_pdf_gauss, normalized_pdf_gauss
 from ..tools import History
-from nose.plugins.attrib import attr
 import numpy as np
 import unittest
 from math import exp, log
 
 rng_seed   = 215135183 # do not change!
 rng_steps  = 10000
 less_steps = 5
@@ -281,19 +280,17 @@
         with_ind.run()
 
         weights = with_ind.weights[:][:,0]
 
         # samples out of support should have zero weight
         np.testing.assert_allclose(weights, 0.)
 
-    @attr('slow')
     def test_unimodal_sampling(self):
         unimodal_sampling(self, ImportanceSampler)
 
-    @attr('slow')
     def test_bimodal_sampling(self):
         bimodal_sampling(self, ImportanceSampler)
 
     def test_weights(self):
         log_target = lambda x: unnormalized_log_pdf_gauss(x, mu, inv_cov)
 
         target_weights = np.array([5.64485430502, 4.21621342833, 6.19074100415, 6.57693562598, 1.39850240669])
```

### Comparing `pypmc-1.2.1/pypmc/sampler/markov_chain.py` & `pypmc-1.2.2/pypmc/sampler/markov_chain.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/sampler/markov_chain_test.py` & `pypmc-1.2.2/pypmc/sampler/markov_chain_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Unit tests for the MCMC sampler functions.
 
 """
 
 from .markov_chain import *
 from .. import density
 from ..tools._probability_densities import unnormalized_log_pdf_gauss
-from nose.plugins.attrib import attr
 import numpy as np
 import unittest
 
 zero_mean      = np.zeros(2)
 
 offdiag_sigma  = np.array([[0.01 , 0.003 ]
                           ,[0.003, 0.0025]])
@@ -90,15 +89,14 @@
 
         mc = MarkovChain(lambda x: 1., prop, start)
 
         mc.run()
 
         self.assertRaises(NotImplementedError, lambda: prop.evaluate(1.,2.))
 
-    @attr('slow')
     def test_sampling(self):
         delta_mean   = .002
         delta_var0   = .0003
         delta_var1   = .00003
 
         prop_dof   = 5.
         prop_sigma = np.array([[0.1 , 0.  ]
@@ -224,15 +222,14 @@
         self.assertEqual(len(mc.target_values), 0)
         self.assertEqual(len(mc.samples), 0)
 
 class TestAdaptiveMarkovChain(unittest.TestCase):
     def setUp(self):
         np.random.mtrand.seed(rng_seed)
 
-    @attr('slow')
     def test_adapt(self):
         delta_mean   = .005
 
         relative_error_unscaled_sigma = .05
 
         prop_dof   = 50.
         prop_sigma = np.array([[0.1 , 0.  ]
```

### Comparing `pypmc-1.2.1/pypmc/tools/_doc.py` & `pypmc-1.2.2/pypmc/tools/_doc.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_history.py` & `pypmc-1.2.2/pypmc/tools/_history.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_linalg.c` & `pypmc-1.2.2/pypmc/tools/_linalg.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_linalg.pyx` & `pypmc-1.2.2/pypmc/tools/_linalg.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_partition.py` & `pypmc-1.2.2/pypmc/tools/_partition.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_plot.py` & `pypmc-1.2.2/pypmc/tools/_plot.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_regularize.c` & `pypmc-1.2.2/pypmc/tools/_regularize.c`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/_regularize.pyx` & `pypmc-1.2.2/pypmc/tools/_regularize.pyx`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/convergence.py` & `pypmc-1.2.2/pypmc/tools/convergence.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/convergence_test.py` & `pypmc-1.2.2/pypmc/tools/convergence_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/indicator/_indicator_factory.py` & `pypmc-1.2.2/pypmc/tools/indicator/_indicator_factory.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/indicator/_indicator_merge.py` & `pypmc-1.2.2/pypmc/tools/indicator/_indicator_merge.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/indicator/indicator_factory_test.py` & `pypmc-1.2.2/pypmc/tools/indicator/indicator_factory_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/linalg_test.py` & `pypmc-1.2.2/pypmc/tools/linalg_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/parallel_sampler.py` & `pypmc-1.2.2/pypmc/tools/parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/parallel_sampler_test.py` & `pypmc-1.2.2/pypmc/tools/parallel_sampler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''Unit tests for parallel sampler
 In order to run tests in parallel, you have to execute this test with
 "mpirun", for example: "mpirun -n 2 nosetests parallel_sampler_test.py"
 
 '''
 
 import numpy as np
-from nose.plugins.attrib import attr
 from ..sampler.markov_chain import MarkovChain, AdaptiveMarkovChain
 from ..sampler.importance_sampling import ImportanceSampler
 from ..density.mixture_test import DummyComponent
 from .. import density
 from ._probability_densities import unnormalized_log_pdf_gauss
 
 def setUpModule():
@@ -39,15 +38,14 @@
 inv_target_sigma = np.linalg.inv(target_sigma)
 log_target = lambda x: unnormalized_log_pdf_gauss(x, target_mean, inv_target_sigma)
 
 class TestMPISampler(unittest.TestCase):
     def setUp(self):
         np.random.mtrand.seed(rng_seed)
 
-    @attr('slow')
     def test_mc_self_adaptive_sampling(self):
         NumberOfRandomSteps = 20000
         delta_mean = .01
         delta_cov  = .05
 
         prop_dof   = 5.
         prop_sigma = np.array([[0.01, 0.   ]
```

### Comparing `pypmc-1.2.1/pypmc/tools/partition_test.py` & `pypmc-1.2.2/pypmc/tools/partition_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/plot_test.py` & `pypmc-1.2.2/pypmc/tools/plot_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/regularize_test.py` & `pypmc-1.2.2/pypmc/tools/regularize_test.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc/tools/util.py` & `pypmc-1.2.2/pypmc/tools/util.py`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/pypmc.egg-info/PKG-INFO` & `pypmc-1.2.2/pypmc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypmc
-Version: 1.2.1
+Version: 1.2.2
 Summary: A toolkit for adaptive importance sampling featuring implementations of variational Bayes, population Monte Carlo, and Markov chains.
 Home-page: https://github.com/pypmc/pypmc
 Author: Frederik Beaujean, Stephan Jahn
 Author-email: beaujean@mytum.de, stephan.jahn@mytum.de
 License: GPLv2
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pypmc-1.2.1/pypmc.egg-info/SOURCES.txt` & `pypmc-1.2.2/pypmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypmc-1.2.1/setup.py` & `pypmc-1.2.2/setup.py`

 * *Files identical despite different names*

