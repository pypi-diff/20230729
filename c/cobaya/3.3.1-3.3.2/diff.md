# Comparing `tmp/cobaya-3.3.1.tar.gz` & `tmp/cobaya-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobaya-3.3.1.tar", last modified: Tue Apr  4 14:18:47 2023, max compression
+gzip compressed data, was "cobaya-3.3.2.tar", last modified: Sat Jul 29 05:16:40 2023, max compression
```

## Comparing `cobaya-3.3.1.tar` & `cobaya-3.3.2.tar`

### file list

```diff
@@ -1,371 +1,374 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.061753 cobaya-3.3.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66680 2023-04-04 14:06:45.000000 cobaya-3.3.1/LICENCE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7014 2023-04-04 14:18:47.057753 cobaya-3.3.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6623 2023-04-04 14:06:45.000000 cobaya-3.3.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.001749 cobaya-3.3.1/cobaya/
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6273 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/bib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48415 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33529 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12919 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3760 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/conventions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.001749 cobaya-3.3.1/cobaya/cosmo_input/
--rw-rw-r--   0 travis    (2000) travis    (2000)      450 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7463 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/autoselect_covmat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5136 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/convert_cosmomc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5647 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/create_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18110 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36178 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/cosmo_input/input_database.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3709 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/doc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.005749 cobaya-3.3.1/cobaya/grid_tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22870 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/batchjob.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9226 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/batchjob_args.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/conventions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2571 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/delete_jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9923 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/gridconfig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18557 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/jobqueue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/runMPI.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6026 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/runbatch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1921 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/grid_tools/running_jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32000 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/install.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11531 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihood.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.005749 cobaya-3.3.1/cobaya/likelihoods/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.009750 cobaya-3.3.1/cobaya/likelihoods/H0/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      551 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/freedman2020.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/freedman2020.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/freedman2020.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      654 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018a.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      357 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018a.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      654 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018b.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2018b.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess201903.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess201903.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess201903.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      480 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2020.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2020.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2020.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2020Mb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      384 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/H0/riess2020Mb.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.009750 cobaya-3.3.1/cobaya/likelihoods/_test/
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/_test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/_test/_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      487 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/_test/_test.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.017750 cobaya-3.3.1/cobaya/likelihoods/bao/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/generic.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_final.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_final.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      393 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_final.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      390 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      356 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      356 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      564 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr7_mgs.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr7_mgs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr7_mgs.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      678 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sixdf_2011_bao.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sixdf_2011_bao.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bao/sixdf_2011_bao.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.021750 cobaya-3.3.1/cobaya/likelihoods/base_classes/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2949 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/DataSetLikelihood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/H0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/InstallableLikelihood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      698 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/Mb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18663 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/bao.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35805 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/cmblikes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35663 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/des.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck2015.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck2018.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    16732 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_2018_CamSpec_python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_calib.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)    16639 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_clik.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6496 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_pliklite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16584 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/base_classes/sn.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.021750 cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    13092 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2129 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.bibtex
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4181 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.021750 cobaya-3.3.1/cobaya/likelihoods/des_y1/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/clustering.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/clustering.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      689 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/des_y1.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/galaxy_galaxy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4435 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/galaxy_galaxy.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      260 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/joint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4459 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/joint.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/shear.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/des_y1/shear.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.021750 cobaya-3.3.1/cobaya/likelihoods/gaussian_mixture/
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/gaussian_mixture/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10851 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/one/
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/one/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/one/one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/one/one.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      266 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing_cmblikes/
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing_cmblikes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      446 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowTEB/
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowTEB/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowTEB/planck_2015_lowTEB.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      398 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_lowl/planck_2015_lowl.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2865 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/params_TT_2015.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      442 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/planck_2015_plikHM_TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/prior_SZ_2015.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4926 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/params_TEEE_2015.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/planck_2015_plikHM_TTTEEE.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      658 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/planck_2015_plikHM_TTTEEE_unbinned.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.025751 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/planck_2015_plikHM_TT_unbinned.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.029751 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/
--rw-rw-r--   0 travis    (2000) travis    (2000)      296 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      643 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      312 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/params_EE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2656 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec_fixedcalpol.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/prior_SZ_CamSpec.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.033751 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/CamSpec2021.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/EE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/EE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      333 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      307 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      375 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      317 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_EE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec_fixedcalpol.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_fixedcalEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_fixedcalTE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/planck_2018_CamSpec2021_python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/prior_SZ_CamSpec.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.037752 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/EE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      447 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/EE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      229 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      245 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      281 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_lite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      460 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_lite.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      247 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_unbinned.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_unbinned.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1091 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_EE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_TE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_calib_pol.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      429 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_calib_temp.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/prior_SZ.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.041752 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      672 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/CMBMarged.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/PlanckLensing2018.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      890 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/clik.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/clik.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/native.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.041752 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2292 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/EE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/EE_clik.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/EE_clik.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/TT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/TT_clik.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      408 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/TT_clik.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.045752 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/
--rw-rw-r--   0 travis    (2000) travis    (2000)      694 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/CamSpec_NPIPE_2022.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      299 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TT.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TT.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      324 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTEEE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      384 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTEEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_EE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TE_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec_fixedcalpol.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_calib_CamSpec_2021.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_fixedcalEE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_fixedcalTE.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/planck_NPIPE_CamSpec_python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/prior_SZ_CamSpec.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.045752 cobaya-3.3.1/cobaya/likelihoods/sn/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      888 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla_lite.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla_lite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/jla_lite.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      680 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/pantheon.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/pantheon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/likelihoods/sn/pantheon.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)    10683 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/log.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70280 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12407 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/mpi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23906 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22327 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/parameterization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28170 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/post.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32093 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/prior.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11138 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25945 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/sampler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.045752 cobaya-3.3.1/cobaya/samplers/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.049752 cobaya-3.3.1/cobaya/samplers/evaluate/
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/evaluate/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/evaluate/evaluate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/evaluate/evaluate.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.049752 cobaya-3.3.1/cobaya/samplers/mcmc/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/mcmc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    52213 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3330 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)    11618 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/mcmc/proposal.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.049752 cobaya-3.3.1/cobaya/samplers/minimize/
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/minimize/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2889 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/minimize/minimize.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    23148 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/minimize/minimize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1643 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/minimize/minimize.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.049752 cobaya-3.3.1/cobaya/samplers/polychord/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/polychord/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/polychord/polychord.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    23642 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/polychord/polychord.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3745 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/samplers/polychord/polychord.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.049752 cobaya-3.3.1/cobaya/theories/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.053753 cobaya-3.3.1/cobaya/theories/camb/
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/camb/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/camb/camb.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    46670 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/camb/camb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1159 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/camb/camb.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.053753 cobaya-3.3.1/cobaya/theories/classy/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/classy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      635 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/classy/classy.bibtex
--rw-rw-r--   0 travis    (2000) travis    (2000)    35171 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/classy/classy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1636 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/classy/classy.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.053753 cobaya-3.3.1/cobaya/theories/cosmo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/cosmo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33133 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theories/cosmo/boltzmannbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18269 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/theory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51697 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3180 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/typing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9100 2023-04-04 14:06:45.000000 cobaya-3.3.1/cobaya/yaml.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.001749 cobaya-3.3.1/cobaya.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7014 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    14626 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      632 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-04-04 14:18:46.000000 cobaya-3.3.1/cobaya.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-04 14:18:47.061753 cobaya-3.3.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4338 2023-04-04 14:06:45.000000 cobaya-3.3.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-04 14:18:47.057753 cobaya-3.3.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2690 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_H0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10234 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_bao.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_bicep_keck_2018.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4968 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_camb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4168 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_des_y1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1383 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_docs_basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_docs_likelihood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3327 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_docs_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12383 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_multi_theory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_planck_2015.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15668 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_planck_2018.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_planck_NPIPE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9229 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_quantities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9231 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3250 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_cosmo_sn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7968 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2664 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_docs_example_quickstart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      630 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_docs_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3108 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_input.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_likelihood_external.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8420 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_mcmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3321 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_mcmc_initial_covmat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2401 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_minimize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5633 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_parameterization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5352 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_polychord.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2120 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_pools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8342 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_post.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_prior.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      920 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_prior_external.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_ref.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2023-04-04 14:06:45.000000 cobaya-3.3.1/tests/test_scripts.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.287315 cobaya-3.3.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66680 2023-07-29 05:05:04.000000 cobaya-3.3.2/LICENCE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-07-29 05:16:40.287315 cobaya-3.3.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6830 2023-07-29 05:05:04.000000 cobaya-3.3.2/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.207310 cobaya-3.3.2/cobaya/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6273 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/bib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48441 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/collection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33969 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12919 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3760 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/conventions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.211310 cobaya-3.3.2/cobaya/cosmo_input/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      450 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7463 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/autoselect_covmat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5136 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/convert_cosmomc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5647 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/create_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18110 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36133 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/cosmo_input/input_database.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3709 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/doc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.215311 cobaya-3.3.2/cobaya/grid_tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22870 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/batchjob.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9226 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/batchjob_args.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/conventions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2571 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/delete_jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9923 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/gridconfig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18557 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/jobqueue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/runMPI.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6026 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/runbatch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1921 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/grid_tools/running_jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27888 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32000 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/install.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12152 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihood.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.215311 cobaya-3.3.2/cobaya/likelihoods/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.219311 cobaya-3.3.2/cobaya/likelihoods/H0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      551 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/freedman2020.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/freedman2020.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/freedman2020.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      654 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018a.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      357 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018a.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      654 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018b.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2018b.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      780 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess201903.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      153 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess201903.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess201903.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      480 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2020.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2020.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2020.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2020Mb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      384 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/H0/riess2020Mb.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.219311 cobaya-3.3.2/cobaya/likelihoods/_test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/_test/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      248 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/_test/_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      487 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/_test/_test.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.231312 cobaya-3.3.2/cobaya/likelihoods/bao/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/generic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/generic.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      378 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_final.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_final.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      393 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_final.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      190 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      200 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      356 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      356 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      564 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      237 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      727 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr7_mgs.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr7_mgs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr7_mgs.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      678 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sixdf_2011_bao.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sixdf_2011_bao.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      337 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bao/sixdf_2011_bao.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.235312 cobaya-3.3.2/cobaya/likelihoods/base_classes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2949 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/DataSetLikelihood.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/H0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5805 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/InstallableLikelihood.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      698 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/Mb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18663 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/bao.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35805 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/cmblikes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35663 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/des.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck2015.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck2018.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16800 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_2018_CamSpec_python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_calib.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16660 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_clik.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6496 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_pliklite.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16584 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/base_classes/sn.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.235312 cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    13092 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2129 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.bibtex
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4181 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/des_y1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/clustering.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/clustering.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      689 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/des_y1.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/galaxy_galaxy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4435 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/galaxy_galaxy.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      260 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/joint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4459 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/joint.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      223 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/shear.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/des_y1/shear.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/gaussian_mixture/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/gaussian_mixture/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10851 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/one/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      755 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/one/one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/one/one.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      383 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing_cmblikes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing_cmblikes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      446 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.239312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowTEB/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowTEB/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowTEB/planck_2015_lowTEB.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.243312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      398 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_lowl/planck_2015_lowl.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.243312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2865 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/params_TT_2015.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      442 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/planck_2015_plikHM_TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/prior_SZ_2015.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.243312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      243 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4926 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/params_TEEE_2015.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      618 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/planck_2015_plikHM_TTTEEE.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.243312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      658 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/planck_2015_plikHM_TTTEEE_unbinned.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.243312 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      501 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT_unbinned/planck_2015_plikHM_TT_unbinned.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.247313 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      296 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      643 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      312 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      697 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      164 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/params_EE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      164 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2656 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec_fixedcalpol.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/prior_SZ_CamSpec.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.251313 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      699 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/CamSpec2021.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/EE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/EE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      333 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      307 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      361 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      375 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      317 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      378 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/TTTEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_EE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec_fixedcalpol.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_fixedcalEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_fixedcalTE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/planck_2018_CamSpec2021_python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/prior_SZ_CamSpec.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.259313 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/EE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      447 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/EE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      229 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      245 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      526 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      281 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      473 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      631 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      263 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      549 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_lite.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      460 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_lite.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      247 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_unbinned.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_unbinned.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1091 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_EE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_TE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      150 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_calib_pol.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      429 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_calib_temp.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       88 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/prior_SZ.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.263314 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      672 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/CMBMarged.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/PlanckLensing2018.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      890 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/clik.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      456 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/clik.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      618 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/native.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.263314 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2337 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      192 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE_clik.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE_clik.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      451 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE_sroll2.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      674 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE_sroll2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/TT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      219 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/TT_clik.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      408 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/TT_clik.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.271314 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      694 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/CamSpec_NPIPE_2022.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      299 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      339 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TT.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      367 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TT.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      301 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      324 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTEEE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      384 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/TTTEEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_EE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TE_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec_fixedcalpol.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_calib_CamSpec_2021.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_fixedcalEE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_fixedcalTE.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/planck_NPIPE_CamSpec_python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/prior_SZ_CamSpec.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.271314 cobaya-3.3.2/cobaya/likelihoods/sn/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      888 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla_lite.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla_lite.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/jla_lite.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/pantheon.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)      241 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/pantheon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/likelihoods/sn/pantheon.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10683 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/log.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70280 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12407 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/mpi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24143 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22327 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/parameterization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28170 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/post.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32094 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/prior.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11138 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25945 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/sampler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.271314 cobaya-3.3.2/cobaya/samplers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.275315 cobaya-3.3.2/cobaya/samplers/evaluate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/evaluate/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/evaluate/evaluate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      358 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/evaluate/evaluate.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.275315 cobaya-3.3.2/cobaya/samplers/mcmc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/mcmc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53121 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3330 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11618 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/mcmc/proposal.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.275315 cobaya-3.3.2/cobaya/samplers/minimize/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/minimize/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2889 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/minimize/minimize.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23148 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/minimize/minimize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1643 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/minimize/minimize.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.275315 cobaya-3.3.2/cobaya/samplers/polychord/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/polychord/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/polychord/polychord.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24364 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/polychord/polychord.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3734 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/samplers/polychord/polychord.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.275315 cobaya-3.3.2/cobaya/theories/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.279315 cobaya-3.3.2/cobaya/theories/camb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/camb/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/camb/camb.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48465 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/camb/camb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1159 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/camb/camb.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.279315 cobaya-3.3.2/cobaya/theories/classy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/classy/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      635 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/classy/classy.bibtex
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35171 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/classy/classy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1636 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/classy/classy.yaml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.279315 cobaya-3.3.2/cobaya/theories/cosmo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/cosmo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33132 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theories/cosmo/boltzmannbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18269 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/theory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51881 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3180 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/typing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9100 2023-07-29 05:05:04.000000 cobaya-3.3.2/cobaya/yaml.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.211310 cobaya-3.3.2/cobaya.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14767 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      632 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-07-29 05:16:40.000000 cobaya-3.3.2/cobaya.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-29 05:16:40.287315 cobaya-3.3.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4338 2023-07-29 05:05:04.000000 cobaya-3.3.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-29 05:16:40.287315 cobaya-3.3.2/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2690 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_H0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10234 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_bao.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1739 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_bicep_keck_2018.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4968 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_camb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2188 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_camb_sigma_8_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4168 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_des_y1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1383 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_docs_basic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_docs_likelihood.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3327 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_docs_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12383 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_multi_theory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_planck_2015.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15668 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_planck_2018.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_planck_NPIPE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9229 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_quantities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9231 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3250 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_cosmo_sn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7968 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_dependencies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2664 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_docs_example_quickstart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      630 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_docs_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3108 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_input.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1505 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_likelihood_external.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8420 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_mcmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3321 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_mcmc_initial_covmat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2401 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_minimize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5633 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_parameterization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5352 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_polychord.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2120 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_pools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8342 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_post.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_prior.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      920 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_prior_external.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3101 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_ref.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1373 2023-07-29 05:05:04.000000 cobaya-3.3.2/tests/test_scripts.py
```

### Comparing `cobaya-3.3.1/LICENCE.txt` & `cobaya-3.3.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/PKG-INFO` & `cobaya-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya
-Version: 3.3.1
+Version: 3.3.2
 Summary: Code for Bayesian Analysis
 Home-page: https://cobaya.readthedocs.io
 Author: Jesus Torrado and Antony Lewis
 License: LGPL
 Project-URL: Source, https://github.com/CobayaSampler/cobaya
 Project-URL: Tracker, https://github.com/CobayaSampler/cobaya/issues
 Project-URL: Licensing, https://github.com/CobayaSampler/cobaya/blob/master/LICENCE.txt
@@ -40,20 +40,22 @@
 
 :Support: For general support, CosmoCoffee_; for bugs and issues, use the `issue tracker <https://github.com/CobayaSampler/cobaya/issues>`_.
 
 :Installation: ``pip install cobaya --upgrade`` (see the `installation instructions <https://cobaya.readthedocs.io/en/latest/installation.html>`_; in general do *not* clone)
 
 .. image:: https://travis-ci.com/CobayaSampler/cobaya.svg?branch=master
    :target: https://app.travis-ci.com/CobayaSampler/cobaya
-.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
-   :target: https://pypi.python.org/pypi/cobaya/
 .. image:: https://readthedocs.org/projects/cobaya/badge/?version=latest
    :target: https://cobaya.readthedocs.org/en/latest
 .. image:: https://codecov.io/gh/CobayaSampler/cobaya/branch/master/graphs/badge.svg
    :target: https://codecov.io/github/CobayaSampler/cobaya/branch/master
+.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
+   :target: https://pypi.python.org/pypi/cobaya/
+.. image:: https://static.pepy.tech/personalized-badge/cobaya?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads
+   :target: https://pepy.tech/project/cobaya
 .. image:: https://img.shields.io/badge/arXiv-2005.05290-b31b1b.svg?color=0B6523
    :target: https://arxiv.org/abs/2005.05290
 
 **Cobaya** (**co**\ de for **bay**\ esian **a**\ nalysis, and Spanish for *Guinea Pig*) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC_, and the advanced nested sampler PolyChord_). The results of the sampling can be analysed with GetDist_. It supports MPI parallelization (and very soon HPC containerization with Docker/Shifter and Singularity).
 
 Its authors are `Jesus Torrado`_ and `Antony Lewis`_. Some ideas and pieces of code have been adapted from other codes (e.g CosmoMC_ by `Antony Lewis`_ and contributors, and `Monte Python`_, by `J. Lesgourgues`_ and `B. Audren`_).
```

### Comparing `cobaya-3.3.1/README.rst` & `cobaya-3.3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 
 :Support: For general support, CosmoCoffee_; for bugs and issues, use the `issue tracker <https://github.com/CobayaSampler/cobaya/issues>`_.
 
 :Installation: ``pip install cobaya --upgrade`` (see the `installation instructions <https://cobaya.readthedocs.io/en/latest/installation.html>`_; in general do *not* clone)
 
 .. image:: https://travis-ci.com/CobayaSampler/cobaya.svg?branch=master
    :target: https://app.travis-ci.com/CobayaSampler/cobaya
-.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
-   :target: https://pypi.python.org/pypi/cobaya/
 .. image:: https://readthedocs.org/projects/cobaya/badge/?version=latest
    :target: https://cobaya.readthedocs.org/en/latest
 .. image:: https://codecov.io/gh/CobayaSampler/cobaya/branch/master/graphs/badge.svg
    :target: https://codecov.io/github/CobayaSampler/cobaya/branch/master
+.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
+   :target: https://pypi.python.org/pypi/cobaya/
+.. image:: https://static.pepy.tech/personalized-badge/cobaya?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads
+   :target: https://pepy.tech/project/cobaya
 .. image:: https://img.shields.io/badge/arXiv-2005.05290-b31b1b.svg?color=0B6523
    :target: https://arxiv.org/abs/2005.05290
 
 **Cobaya** (**co**\ de for **bay**\ esian **a**\ nalysis, and Spanish for *Guinea Pig*) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC_, and the advanced nested sampler PolyChord_). The results of the sampling can be analysed with GetDist_. It supports MPI parallelization (and very soon HPC containerization with Docker/Shifter and Singularity).
 
 Its authors are `Jesus Torrado`_ and `Antony Lewis`_. Some ideas and pieces of code have been adapted from other codes (e.g CosmoMC_ by `Antony Lewis`_ and contributors, and `Monte Python`_, by `J. Lesgourgues`_ and `B. Audren`_).
```

### Comparing `cobaya-3.3.1/cobaya/__init__.py` & `cobaya-3.3.2/cobaya/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 
 if sys.version_info < (3, 8):
     print('Cobaya requires Python 3.8+, please upgrade.')
     sys.exit(1)
 
 __author__ = "Jesus Torrado and Antony Lewis"
-__version__ = "3.3.1"
+__version__ = "3.3.2"
 __obsolete__ = False
 __year__ = "2023"
 __url__ = "https://cobaya.readthedocs.io"
```

### Comparing `cobaya-3.3.1/cobaya/__main__.py` & `cobaya-3.3.2/cobaya/__main__.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/bib.py` & `cobaya-3.3.2/cobaya/bib.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/collection.py` & `cobaya-3.3.2/cobaya/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 # Global
 import os
 import functools
 import warnings
 from copy import deepcopy
-from typing import Union, Sequence, Optional, Tuple, Iterable
+from typing import Union, Sequence, Optional, Tuple
 from numbers import Number
 import numpy as np
 import pandas as pd
 from getdist import MCSamples, chains  # type: ignore
 from getdist.chains import WeightedSamples, WeightedSampleError  # type: ignore
 
 # Local
@@ -95,17 +95,18 @@
     """
     Returns the temperature of a sample.
 
     If ``check=True`` and the log-probabilites passed are arrays, checks consistency
     of the sample temperature, and raises ``AssertionError`` if inconsistent.
     """
     temp = (logprior + loglike) / logpost
-    if check and isinstance(temp, Iterable) and len(temp) > 1:
-        assert np.allclose(temp, temp[0]), "Inconsistent temperature in sample."
-        temp = temp[0]
+    if check and not isinstance(temp, Number) and len(temp) > 1:
+        assert np.allclose(temp, temp[0],
+                           rtol=1e-3), "Inconsistent temperature in sample."
+        temp = np.mean(temp)
     return temp
 
 
 def detempering_weights_factor(tempered_logpost, temperature):
     """
     Returns the detempering factors for the weights of a tempered sample, i.e. if ``w_t``
     is the weight of the tempered sample, then the weight of the unit-temperature one is
@@ -272,15 +273,15 @@
         # If loaded, check sample weights, consistent logp sums,
         # and temperature (ignores the given one)
         samples_loaded = len(self) > 0
         if samples_loaded:
             try:
                 self.temperature = self._check_logps()
                 if temperature is not None and \
-                   not np.isclose(temperature, self.temperature):
+                        not np.isclose(temperature, self.temperature):
                     raise LoggedError(
                         self.log,
                         "Sample temperature appears to be %r, but the collection was "
                         "explicitly initialized with temperature %r.",
                         self.temperature,
                         temperature,
                     )
@@ -550,19 +551,19 @@
         return np.allclose(np.round(weights), weights)
 
     def _detempered_weights(self):
         """Computes the detempered weights."""
         if self.temperature == 1:
             return self._data[OutPar.weight].to_numpy(dtype=np.float64)
         return (
-            self._data[OutPar.weight].to_numpy(dtype=np.float64) *
-            detempering_weights_factor(
-                -self._data[OutPar.minuslogpost].to_numpy(dtype=np.float64),
-                self.temperature
-            )
+                self._data[OutPar.weight].to_numpy(dtype=np.float64) *
+                detempering_weights_factor(
+                    -self._data[OutPar.minuslogpost].to_numpy(dtype=np.float64),
+                    self.temperature
+                )
         )
 
     def _detempered_minuslogpost(self):
         """Computes the detempered -log-posterior."""
         if self.temperature == 1:
             return self._data[OutPar.minuslogpost].to_numpy(dtype=np.float64)
         return -remove_temperature(
@@ -927,16 +928,16 @@
 
     def bestfit(self):
         """Best fit (maximum likelihood) sample. Returns a copy."""
         return self.data.loc[self.data[OutPar.chi2].astype(np.float64).idxmin()].copy()
 
     def MAP(self):
         """Maximum-a-posteriori (MAP) sample. Returns a copy."""
-        return self.data.loc[self.data[OutPar.minuslogpost].astype(np.float64).idxmin()]\
-                        .copy()
+        return self.data.loc[self.data[OutPar.minuslogpost].astype(np.float64).idxmin()] \
+            .copy()
 
     def _sampled_to_getdist(
             self,
             first: Optional[int] = None,
             last: Optional[int] = None,
             tempered: bool = False
     ) -> MCSamples:
@@ -1155,15 +1156,15 @@
     """
 
     def __getitem__(self, columns, *args):
         if isinstance(columns, str):
             return self.data.values[0, self.data.columns.get_loc(columns)]
         try:
             return self.data.values[0,
-                                    [self.data.columns.get_loc(c) for c in columns]]
+            [self.data.columns.get_loc(c) for c in columns]]
         except KeyError as excpt:
             raise ValueError("Some of the indices are not valid columns.") from excpt
 
     def add(self, *args, **kwargs):
         """Add/override the sampled point."""
         self.reset()  # resets the DataFrame, so never goes beyond 1 point
         super().add(*args, **kwargs)
```

### Comparing `cobaya-3.3.1/cobaya/component.py` & `cobaya-3.3.2/cobaya/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import time
 import inspect
-import pkg_resources
 from inspect import cleandoc
 from packaging import version
-from importlib import import_module
+from importlib import import_module, resources
 from typing import Optional, Union, List, Set
 
 from cobaya.log import HasLogger, LoggedError, get_logger
 from cobaya.typing import Any, InfoDict, InfoDictIn, empty_dict
 from cobaya.tools import resolve_packages_path, load_module, get_base_classes, \
     get_internal_class_component_name, deepcopy_where_possible, VersionCheckError
 from cobaya.conventions import kinds, cobaya_package, reserved_attributes
@@ -165,35 +164,49 @@
         """
         Get the content of .bibtex file for this component. If no specific bibtex
         from this class, it will return the result from an inherited class if that
         provides bibtex.
         """
         filename = cls.__dict__.get('bibtex_file')
         if filename:
-            bib = pkg_resources.resource_string(cls.__module__, filename).decode("utf-8")
+            bib = cls.get_text_file_content(filename)
         else:
             bib = cls.get_associated_file_content('.bibtex')
         if bib:
             return bib
         for base in cls.__bases__:
             if issubclass(base, HasDefaults) and base is not HasDefaults:
                 return base.get_bibtex()
         return None
 
     @classmethod
-    def get_associated_file_content(cls, ext, file_root=None) -> Optional[str]:
-        # handle extracting package files when may be inside a zipped package so files
-        # not accessible directly
+    def get_associated_file_content(cls, ext: str,
+                                    file_root: Optional[str] = None) -> Optional[str]:
+        """
+        Return the content of the associated file, if it exists.
+
+        This function handles extracting package files when they may be
+        inside a zipped package and thus not directly accessible.
+
+        Returns:
+            The content of the file as a string, if it exists and can be read. None otherwise.
+        """
+
+        return cls.get_text_file_content((file_root or cls.get_file_base_name()) + ext)
+
+    @classmethod
+    def get_text_file_content(cls, file_name: str) -> Optional[str]:
+        """
+        Return the content of a file in the directory of the module, if it exists.
+        """
+        package = inspect.getmodule(cls).__package__
         try:
-            string = pkg_resources.resource_string(
-                cls.__module__, (file_root or cls.get_file_base_name()) + ext)
+            return resources.read_text(package, file_name)
         except Exception:
             return None
-        else:
-            return string.decode("utf-8")
 
     @classmethod
     def get_class_options(cls, input_options=empty_dict) -> InfoDict:
         """
         Returns dictionary of names and values for class variables that can also be
         input and output in yaml files, by default it takes all the
         (non-inherited and non-private) attributes of the class excluding known
```

### Comparing `cobaya-3.3.1/cobaya/containers.py` & `cobaya-3.3.2/cobaya/containers.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/conventions.py` & `cobaya-3.3.2/cobaya/conventions.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/cosmo_input/autoselect_covmat.py` & `cobaya-3.3.2/cobaya/cosmo_input/autoselect_covmat.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/cosmo_input/convert_cosmomc.py` & `cobaya-3.3.2/cobaya/cosmo_input/convert_cosmomc.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/cosmo_input/create_input.py` & `cobaya-3.3.2/cobaya/cosmo_input/create_input.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/cosmo_input/gui.py` & `cobaya-3.3.2/cobaya/cosmo_input/gui.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/cosmo_input/input_database.py` & `cobaya-3.3.2/cobaya/cosmo_input/input_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,22 +723,20 @@
              field not in pre})
     if pre.get("sampler") != 'MCMC':
         pre.update(default_sampler)
 
 # BASIC INSTALLATION #####################################################################
 install_basic: InfoDict = {
     "theory": theory,
-    "likelihood": {
-        # Native first: avoids reinstalling clik code+data if supp data obsolete
+    "likelihood": dict(like_cmb["planck_NPIPE"]["likelihood"], **{
+        # 2018 lensing ensured covmat database also installed
         "planck_2018_lensing.native": None,
-        "planck_2018_lowl.TT": None,
-        "planck_2018_lowl.EE": None,
         "sn.pantheon": None,
         "bao.sdss_dr12_consensus_final": None,
-        "des_y1.joint": None}}
+        "des_y1.joint": None})}
 
 install_tests = deepcopy(install_basic)
 install_tests["likelihood"].update({"planck_2015_lowl": None,
                                     "planck_2018_highl_plik.TT_unbinned": None,
                                     "planck_2018_highl_plik.TT_lite_native": None,
                                     "planck_2018_highl_CamSpec.TT": None,
                                     "planck_2018_highl_CamSpec2021.TT": None,
```

### Comparing `cobaya-3.3.1/cobaya/doc.py` & `cobaya-3.3.2/cobaya/doc.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/batchjob.py` & `cobaya-3.3.2/cobaya/grid_tools/batchjob.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/batchjob_args.py` & `cobaya-3.3.2/cobaya/grid_tools/batchjob_args.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/delete_jobs.py` & `cobaya-3.3.2/cobaya/grid_tools/delete_jobs.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/gridconfig.py` & `cobaya-3.3.2/cobaya/grid_tools/gridconfig.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/jobqueue.py` & `cobaya-3.3.2/cobaya/grid_tools/jobqueue.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/runMPI.py` & `cobaya-3.3.2/cobaya/grid_tools/runMPI.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/runbatch.py` & `cobaya-3.3.2/cobaya/grid_tools/runbatch.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/grid_tools/running_jobs.py` & `cobaya-3.3.2/cobaya/grid_tools/running_jobs.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/input.py` & `cobaya-3.3.2/cobaya/input.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/install.py` & `cobaya-3.3.2/cobaya/install.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihood.py` & `cobaya-3.3.2/cobaya/likelihood.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,24 +139,33 @@
 class AbsorbUnusedParamsLikelihood(Likelihood):
     pass
 
 
 class LikelihoodExternalFunction(Likelihood):
     def __init__(self, info, name, timing=None):
         Theory.__init__(self, info, name=name, timing=timing, standalone=False)
+        self.input_params = str_to_list(self.input_params)
         # Store the external function and assign its arguments
         self.external_function = get_external_function(info["external"], name=name)
         self._self_arg = "_self"
         argspec = getfullargspec(self.external_function)
-        self.input_params = str_to_list(self.input_params)
+        # NB: unnamed args are not supported
+        has_unnamed_args = bool(argspec.varargs)
+        if has_unnamed_args:
+            raise LoggedError(
+                self.log, "External likelihoods with unnamed args are not supported.")
         ignore_args = [self._self_arg]
         if argspec.defaults:
-            required_args = argspec.args[:-len(argspec.defaults)]
+            required_args = set(argspec.args[:-len(argspec.defaults)])
         else:
-            required_args = argspec.args
+            required_args = set(argspec.args)
+        # Allows for passing a class method
+        # (Do not mistake for the use of _self to get quantities from provider, see below)
+        if hasattr(self.external_function, "__self__"):
+            required_args.remove("self")
         self.params = {p: None for p in required_args if p not in ignore_args}
         if self.output_params:
             self.output_params = str_to_list(self.output_params) or []
         # Required quantities from other components
         self._uses_self_arg = self._self_arg in argspec.args
         if info.get("requires") and not self._uses_self_arg:
             raise LoggedError(
@@ -167,15 +176,17 @@
         self._optional_args = \
             [p for p, val in chain(zip(argspec.args[-len(argspec.defaults):],
                                        argspec.defaults) if argspec.defaults else [],
                                    (argspec.kwonlydefaults or {}).items())
              if p not in ignore_args and
              (isinstance(val, numbers.Number) or val is None)]
         self._args = set(chain(self._optional_args, self.params))
-        if argspec.varkw:
+        # If has unnamed kwargs, assume these are the ones declared in input_params
+        has_unnamed_kwargs = bool(argspec.varkw)
+        if has_unnamed_kwargs:
             self._args.update(self.input_params)
         self.log.info("Initialized external likelihood.")
 
     def get_requirements(self):
         return self._requirements
 
     def get_can_support_params(self):
```

### Comparing `cobaya-3.3.1/cobaya/likelihoods/H0/freedman2020.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/H0/freedman2020.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/H0/riess2018a.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/H0/riess2018a.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/H0/riess2018b.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/H0/riess2018b.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/H0/riess201903.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/H0/riess201903.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_bao.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_final.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_final.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_consensus_full_shape.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr12_lrg_bao_dmdh.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_elg.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lrg.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyauto.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_lyxqso.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_baoplus_qso.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr16_lrg_bao_dmdh.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr7_mgs.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr7_mgs.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sdss_dr7_mgs.yaml` & `cobaya-3.3.2/cobaya/likelihoods/bao/sdss_dr7_mgs.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bao/sixdf_2011_bao.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bao/sixdf_2011_bao.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/DataSetLikelihood.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/DataSetLikelihood.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/H0.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/H0.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/InstallableLikelihood.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/InstallableLikelihood.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/Mb.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/Mb.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/bao.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/bao.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/cmblikes.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/cmblikes.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/des.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/des.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/planck2015.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/planck2015.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_2018_CamSpec_python.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_2018_CamSpec_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 Use dataset_params : { 'use_cl': '100x100 143x143 217x217 143x217'} to use e.g. just TT ,
 or other combination with TE and EE.
 
 Set use_range to string representation of L range to use, e.g. 50-100, 200-500, 1470-2500,
 or pass a dictionary of ranges for each spectrum.
 
+It is used by the 2018 and more recent CamSpec Planck likelihoods.
+
 """
 
 # Global
 import numpy as np
 import os
 import scipy
```

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_clik.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_clik.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 The likelihoods from the Planck 2015 data release have been superseded
 by the 2018 ones, and will eventually be deprecated.
 """)
 
 clik_url = 'https://github.com/benabed/clik/archive/refs/heads/main.zip'
 pla_url_prefix = r"https://pla.esac.esa.int/pla-sl/data-action?COSMOLOGY.COSMOLOGY_OID="
 
-last_version_supp_data_and_covmats = "v2.01"
+last_version_supp_data_and_covmats = "v2.1"
 last_version_clik = "16.0"
 min_version_clik = "3.1"
 
 
 class PlanckClik(Likelihood):
     # Data type for aggregated chi2 (case sensitive)
     type = "CMB"
@@ -51,20 +51,20 @@
             # displayed in the folder name and cannot be retrieved from the module.
             clik = load_clik(
                 "clik", path=self.path, install_path=install_path,
                 get_import_path=get_clik_import_path, logger=self.log,
                 not_installed_level="debug")
         except VersionCheckError as excpt:
             raise VersionCheckError(
-                str(excpt) + " Upgrade with `cobaya-install planck_2018_lowl.TT "
-                             "--upgrade`.")
+                str(excpt) + " Upgrade with `cobaya-install "
+                             "planck_2018_highl_plik.TTTEEE --upgrade`.")
         except ComponentNotInstalledError as excpt:
             raise ComponentNotInstalledError(
-                self.log, (f"Could not find clik: {excpt}. "
-                           "To install it, run `cobaya-install planck_2018_lowl.TT`"))
+                self.log, (f"Could not find clik: {excpt}. To install it, "
+                           f"run `cobaya-install planck_2018_highl_plik.TTTEEE`"))
         # Loading the likelihood data
         data_path = get_data_path(self.__class__.get_qualified_class_name())
         if not os.path.isabs(self.clik_file):
             self.path_data = getattr(self, "path_data", os.path.join(
                 self.path or self.packages_path, "data", data_path))
             self.clik_file = os.path.join(self.path_data, self.clik_file)
         # Differences in the wrapper for lensing and non-lensing likes
@@ -280,15 +280,15 @@
     if os.path.exists(version_file):
         with open(version_file, 'r') as f:
             installed_version = version.parse(f.readline().split("_")[-1].split('-')[0])
     else:
         installed_version = version.parse(clik_src_path.rstrip(os.sep).split("-")[-1])
     if installed_version < version.parse(min_version):
         raise VersionCheckError(
-            f"Installed version of the Plack likelihood code 'clik' ({installed_version})"
+            f"Installed version of the Planck likelihood code 'clik' ({installed_version})"
             f" older than minimum required one ({last_version_clik}).")
     elif installed_version > version.parse(last_version_clik):
         raise ValueError("This should not happen: min version needs update.")
     return os.path.join(clik_src_path, 'lib/python/site-packages')
 
 
 def load_clik(*args, **kwargs):
```

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/planck_pliklite.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/planck_pliklite.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/base_classes/sn.py` & `cobaya-3.3.2/cobaya/likelihoods/base_classes/sn.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/__init__.py` & `cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/__init__.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.yaml` & `cobaya-3.3.2/cobaya/likelihoods/bicep_keck_2018/bicep_keck_2018.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/des_y1/clustering.yaml` & `cobaya-3.3.2/cobaya/likelihoods/des_y1/clustering.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/des_y1/des_y1.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/des_y1/des_y1.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/des_y1/galaxy_galaxy.yaml` & `cobaya-3.3.2/cobaya/likelihoods/des_y1/galaxy_galaxy.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/des_y1/joint.yaml` & `cobaya-3.3.2/cobaya/likelihoods/des_y1/joint.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/des_y1/shear.yaml` & `cobaya-3.3.2/cobaya/likelihoods/des_y1/shear.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.py` & `cobaya-3.3.2/cobaya/likelihoods/gaussian_mixture/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/one/one.py` & `cobaya-3.3.2/cobaya/likelihoods/one/one.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing/planck_2015_lensing.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_lensing_cmblikes/planck_2015_lensing_cmblikes.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TT/params_TT_2015.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TT/params_TT_2015.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/params_TEEE_2015.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/params_TEEE_2015.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/planck_2015_plikHM_TTTEEE.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE/planck_2015_plikHM_TTTEEE.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/planck_2015_plikHM_TTTEEE_unbinned.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2015_plikHM_TTTEEE_unbinned/planck_2015_plikHM_TTTEEE_unbinned.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TT.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/TTTEEE.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec/params_TT_CamSpec.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/CamSpec2021.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/CamSpec2021.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/params_TT_CamSpec.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_CamSpec2021/planck_2018_CamSpec2021_python.py` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_CamSpec2021/planck_2018_CamSpec2021_python.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_lite_native.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TTTEEE_unbinned.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/TT_lite_native.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_EE.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_EE.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_TE.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_TE.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_highl_plik/params_TT.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_highl_plik/params_TT.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/CMBMarged.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/CMBMarged.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/__init__.py` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/__init__.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_lensing/native.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_lensing/native.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/EE.py` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/EE.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,24 +19,25 @@
     type = "CMB"
     aliases = ["lowE"]
 
     _lmin = 2
     _lmax = 29
     _nstepsEE = 3000
     _stepEE = 0.0001
+    _table_file_name = 'prob_table.txt'
 
     @classmethod
     def get_bibtex(cls):
         from cobaya.likelihoods.base_classes import Planck2018Clik
         return Planck2018Clik.get_bibtex()
 
     def initialize(self):
         if self.get_install_options() and self.packages_path:
             path = self.get_path(self.packages_path)
-            self.probEE = np.loadtxt(os.path.join(path, 'prob_table.txt'))
+            self.probEE = np.loadtxt(os.path.join(path, self._table_file_name))
 
     def get_can_support_params(self):
         return ['A_planck']
 
     def get_requirements(self):
         return {'Cl': {'ee': self._lmax}}
```

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_2018_lowl/TT.py` & `cobaya-3.3.2/cobaya/likelihoods/planck_2018_lowl/TT.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/CamSpec_NPIPE_2022.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/CamSpec_NPIPE_2022.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec.yaml` & `cobaya-3.3.2/cobaya/likelihoods/planck_NPIPE_highl_CamSpec/params_TT_CamSpec.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/sn/jla.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/sn/jla.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/sn/jla.yaml` & `cobaya-3.3.2/cobaya/likelihoods/sn/jla.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/sn/jla_lite.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/sn/jla_lite.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/sn/jla_lite.yaml` & `cobaya-3.3.2/cobaya/likelihoods/sn/jla_lite.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/likelihoods/sn/pantheon.bibtex` & `cobaya-3.3.2/cobaya/likelihoods/sn/pantheon.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/log.py` & `cobaya-3.3.2/cobaya/log.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/model.py` & `cobaya-3.3.2/cobaya/model.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/mpi.py` & `cobaya-3.3.2/cobaya/mpi.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/output.py` & `cobaya-3.3.2/cobaya/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
                     pass
             except OSError:
                 pass
         if mpi.is_disabled():
             raise LoggedError(self.log,
                               "File %s is locked by another process, you are running "
                               "with MPI disabled but may have more than one process. "
+                              "Make sure that you have mpi4py installed and working."
                               "Note that --test should not be used with MPI.")
         if mpi.get_mpi():
             import mpi4py
         else:
             mpi4py = None
         if mpi.is_main_process() and use_portalocker() is None:
             self.log.warning('install "portalocker" for better file lock control.')
@@ -106,15 +107,17 @@
                           "configured (using the same mpi as mpirun/mpiexec); "
                           "e.g. try the test at\n"
                           "https://cobaya.readthedocs.io/en/latest/installation."
                           "html#mpi-parallelization-optional-but-encouraged\n"
                           + ("Your current mpi4py config is:"
                              "\n %s" % mpi4py.get_config()
                              if mpi4py is not None else
-                             "mpi4py is NOT currently installed."), self.lock_file)
+                             "mpi4py is NOT currently installed.")
+                          + "\nIf this is a lock issue you can disable this check by"
+                            "setting env COBAYA_USE_FILE_LOCKING=False.", self.lock_file)
 
     def check_error(self):
         if self.lock_error_file and os.path.exists(self.lock_error_file):
             self.lock_error()
 
     def clear_lock(self):
         if self.has_lock():
@@ -444,16 +447,16 @@
         ``[folder]/[prefix].[name].[extension]``.
 
         Notice that ``name=None`` generates a date, but ``name=""`` removes the ``name``
         field, making it simply ``[folder]/[prefix].[extension]``.
         """
         if name is None:
             name = (datetime.datetime.now().isoformat().replace("T", "")
-                        .replace(":", "").replace(".", "")
-                        .replace("-", "")[:(4 + 2 + 2) + (2 + 2 + 2 + 3)])  # up to ms
+                    .replace(":", "").replace(".", "")
+                    .replace("-", "")[:(4 + 2 + 2) + (2 + 2 + 2 + 3)])  # up to ms
         file_name = os.path.join(
             self.folder,
             self.prefix + ("." if self.prefix else "") + (name + "." if name else "") +
             self.sanitize_collection_extension(extension))
         return file_name, self.kind
 
     def collection_regexp(self, name=None, extension=None):
```

### Comparing `cobaya-3.3.1/cobaya/parameterization.py` & `cobaya-3.3.2/cobaya/parameterization.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/post.py` & `cobaya-3.3.2/cobaya/post.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/prior.py` & `cobaya-3.3.2/cobaya/prior.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
         """
         if np.nan in self.ref_pdf and warn_if_no_ref:
             self.log.info(
                 "Reference values or pdfs for some parameters were not provided. "
                 "Sampling from the prior instead for those parameters.")
         # As a curiosity, `r is np.nan` was returning False after `r = np.nan` if
         # it had been passed via MPI before the test, since this creates a "new" np.nan
-        # NB: isinstance(np.nan, numers.Real) --> True
+        # NB: isinstance(np.nan, numbers.Real) --> True
         where_ignore_ref = [
             isinstance(r, numbers.Real) and (np.isnan(r) or ignore_fixed)
             for r in self.ref_pdf
         ]
         tries = 0
         warn_if_tries = read_dnumber(warn_if_tries, self.d())
         ref_sample = np.empty(len(self.ref_pdf))
```

### Comparing `cobaya-3.3.1/cobaya/run.py` & `cobaya-3.3.2/cobaya/run.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/sampler.py` & `cobaya-3.3.2/cobaya/sampler.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/evaluate/evaluate.py` & `cobaya-3.3.2/cobaya/samplers/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.bibtex` & `cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.py` & `cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         # Get first point, to be discarded -- not possible to determine its weight
         # Still, we need to compute derived parameters, since, as the proposal "blocked",
         # we may be saving the initial state of some block.
         # NB: if resuming but nothing was written (burn-in not finished): re-start
         if self.output.is_resuming() and len(self.collection):
             last = len(self.collection) - 1
             initial_point = (self.collection[self.collection.sampled_params]
-                             .iloc[last]).to_numpy(dtype=np.float64, copy=True)
+            .iloc[last]).to_numpy(dtype=np.float64, copy=True)
             results = LogPosterior(
                 logpost=-remove_temperature(
                     self.collection[OutPar.minuslogpost].iloc[last], self.temperature),
                 logpriors=-(self.collection[self.collection.minuslogprior_names]
                             .iloc[last].to_numpy(dtype=np.float64, copy=True)),
                 loglikes=-0.5 * (self.collection[self.collection.chi2_names]
                                  .iloc[last].to_numpy(dtype=np.float64, copy=True)),
@@ -162,27 +162,43 @@
             self.log.info("Getting initial point... (this may take a few seconds)")
             initial_point, results = \
                 self.model.get_valid_point(max_tries=min(self.max_tries.value, int(1e7)),
                                            random_state=self._rng)
             # If resuming but no existing chain, assume failed run and ignore blocking
             # if speeds measurement requested
             if self.output.is_resuming() and not self.collection \
-               and self.measure_speeds:
+                    and self.measure_speeds:
                 self.blocking = None
             if self.measure_speeds and self.blocking:
                 self.mpi_warning(
                     "Parameter blocking manually fixed: speeds will not be measured.")
             elif self.measure_speeds:
                 n = None if self.measure_speeds is True else int(self.measure_speeds)
                 self.model.measure_and_set_speeds(n=n, discard=0, random_state=self._rng)
         self.current_point.add(initial_point, results)
         self.log.info("Initial point: %s", self.current_point)
         # Set up blocked proposer
         self.set_proposer_blocking()
         self.set_proposer_initial_covmat(load=True)
+
+        if not self.output.is_resuming() and more_than_one_process():
+            # sanity check whether initial dispersion of points is plausible given the
+            # covariance being used
+            initial_mean = np.mean(np.array(mpi.allgather(initial_point)), axis=0)
+            delta = initial_point - initial_mean
+            diag, rot = np.linalg.eigh(self.proposer.get_covariance())
+            max_dist = np.max(np.abs(rot.T.dot(delta)) / np.sqrt(diag))
+            self.log.debug("Max dist to start mean: %s", max_dist)
+            max_dist = mpi.gather(max_dist)
+            if mpi.is_main_process() and np.max(max_dist) > 12:
+                self.mpi_warning(
+                    "The initial points are widely dispersed compared to "
+                    "the proposal covariance, it may take a long time to "
+                    "burn in (max dist to start mean: %s)", max_dist)
+
         # Max #(learn+convergence checks) to wait,
         # in case one process dies/hangs without raising error
         self.been_waiting = 0
         self.max_waiting = max(50, self.max_tries.unit_value)
         # Burning-in countdown -- the +1 accounts for the initial point (always accepted)
         self.burn_in_left = self.burn_in.value * self.current_point.output_thin + 1
         self._msg_ready = ("Ready to check convergence" +
@@ -418,16 +434,16 @@
     def n(self, burn_in=False):
         """
         Returns the total number of accepted steps taken, including or not burn-in steps
         depending on the value of the `burn_in` keyword.
         """
         return len(self.collection) + (
             0 if not burn_in else (
-                self.burn_in.value -
-                self.burn_in_left // self.current_point.output_thin + 1))
+                    self.burn_in.value -
+                    self.burn_in_left // self.current_point.output_thin + 1))
 
     def get_new_sample_metropolis(self):
         """
         Draws a new trial point from the proposal pdf and checks whether it is accepted:
         if it is accepted, it saves the old one into the collection and sets the new one
         as the current state; if it is rejected increases the weight of the current state
         by 1.
@@ -597,15 +613,15 @@
                     "Alternatively (though not advisable) make 'max_tries: np.inf' "
                     "(or 'max_tries: .inf' in yaml).\n"
                     "Current point: %s\nCurrent result: %s\n"
                     "Last proposal: %s\nWith rejected result: %s",
                     max_tries_now, self.current_point, self.current_point.results,
                     trial, trial_results)
             elif self.current_point.weight > max_tries_now and \
-                    not getattr(self, '_prior_tries_warning'):
+                    not getattr(self, '_prior_tries_warning', False):
                 self.log.warning("Proposal has been rejected %s times", max_tries_now)
                 self._prior_tries_warning = True
 
     # Functions to check convergence and learn the covariance of the proposal distribution
 
     def check_ready(self):
         """
@@ -651,19 +667,19 @@
             try:
                 acceptance_rate = self.get_acceptance_rate(cut)
                 Ns = np.ones(m - 1) * cut
                 ranges = [(i * cut, (i + 1) * cut - 1) for i in range(1, m)]
                 means = np.array(
                     [self.collection.mean(
                         first=f, last=l, tempered=True)
-                     for f, l in ranges])
+                        for f, l in ranges])
                 covs = np.array(
                     [self.collection.cov(
                         first=f, last=l, tempered=True)
-                     for f, l in ranges])
+                        for f, l in ranges])
             except always_stop_exceptions:
                 raise
             except Exception:  # pylint: disable=broad-except
                 self.log.info("Not enough points in chain to check convergence. "
                               "Waiting for next checkpoint.")
                 return
             acceptance_rates = None
```

### Comparing `cobaya-3.3.1/cobaya/samplers/mcmc/mcmc.yaml` & `cobaya-3.3.2/cobaya/samplers/mcmc/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/mcmc/proposal.py` & `cobaya-3.3.2/cobaya/samplers/mcmc/proposal.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/minimize/minimize.bibtex` & `cobaya-3.3.2/cobaya/samplers/minimize/minimize.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/minimize/minimize.py` & `cobaya-3.3.2/cobaya/samplers/minimize/minimize.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/minimize/minimize.yaml` & `cobaya-3.3.2/cobaya/samplers/minimize/minimize.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/polychord/polychord.bibtex` & `cobaya-3.3.2/cobaya/samplers/polychord/polychord.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/samplers/polychord/polychord.py` & `cobaya-3.3.2/cobaya/samplers/polychord/polychord.py`

 * *Files 3% similar despite different names*

```diff
@@ -389,27 +389,47 @@
                           "with prefix '%s'",
                           self.pc_settings.base_dir, self.pc_settings.file_root)
             self.log.info(
                 "log(Z) = %g +/- %g ; Z in [%.8g, %.8g] (68%% C.L. log-gaussian)",
                 self.logZ, self.logZstd,
                 *[np.exp(self.logZ + n * self.logZstd) for n in [-1, 1]])
 
-    def products(self):
+    def products(
+            self,
+            to_getdist: bool = False,
+            **kwargs,
+    ) -> dict:
         """
-        Auxiliary function to define what should be returned in a scripted call.
+        Returns the products of the sampling process.
+
+        Parameters
+        ----------
+        to_getdist: bool, default: True
+            If ``True``, returns sample collections as :class:'getdist.MCSamples`.
 
         Returns:
            The sample ``SampleCollection`` containing the sequentially
            discarded live points.
         """
+        if kwargs.get("skip_samples"):
+            self.mpi_warning(
+                "Initial samples should not be skipped in nested sampling. Ignoring."
+            )
         if is_main_process():
+            collection = self.collection
+            if to_getdist:
+                collection = self.collection.to_getdist(model=self.model)
             products = {
-                "sample": self.collection, "logZ": self.logZ, "logZstd": self.logZstd}
+                "sample": collection, "logZ": self.logZ, "logZstd": self.logZstd}
             if self.pc_settings.do_clustering:
-                products.update({"clusters": self.clusters})
+                clusters = self.clusters
+                if to_getdist:
+                    for c in clusters.values():
+                        c["sample"] = c["sample"].to_getdist(model=self.model)
+                products.update({"clusters": clusters})
             return products
         else:
             return {}
 
     @classmethod
     def get_base_dir(cls, output):
         if output:
```

### Comparing `cobaya-3.3.1/cobaya/samplers/polychord/polychord.yaml` & `cobaya-3.3.2/cobaya/samplers/polychord/polychord.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 # (Use with care if there are likelihood modes close to the edge of the prior)
 confidence_for_unbounded: 0.9999995  # 5 sigmas of the prior
 # Seeding runs
 # ------------
 seed:  # positive integer
 # Raw output of PolyChord (no need to change them, normally)
 # ----------------------------------------------------------
-file_root:
 posteriors: True
 equals: True
 cluster_posteriors: True
 write_resume: True
 read_resume: True
 write_stats: True
 write_live: True
```

### Comparing `cobaya-3.3.1/cobaya/theories/camb/camb.bibtex` & `cobaya-3.3.2/cobaya/theories/camb/camb.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/theories/camb/camb.py` & `cobaya-3.3.2/cobaya/theories/camb/camb.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 :Author: Jesus Torrado and Antony Lewis
 
 .. |br| raw:: html
 
    <br />
 
 This module imports and manages the CAMB cosmological code.
-It requires CAMB 1.1.3 or higher.
+It requires CAMB 1.5 or higher.
 
 .. note::
 
    **If you use this cosmological code, please cite it as:**
    |br|
    A. Lewis, A. Challinor, A. Lasenby,
    *Efficient computation of CMB anisotropies in closed FRW*
@@ -249,15 +249,15 @@
     CAMB cosmological Boltzmann code \cite{Lewis:1999bs,Howlett:2012mh}.
     """
 
     # Name of the Class repo/folder and version to download
     _camb_repo_name = "cmbant/CAMB"
     _camb_repo_version = os.environ.get("CAMB_REPO_VERSION", "master")
     _camb_min_gcc_version = "6.4"
-    _min_camb_version = '1.3.5'
+    _min_camb_version = '1.5.0'
 
     file_base_name = 'camb'
     external_primordial_pk: bool
     camb: Any
     ignore_obsolete: bool
 
     def initialize(self):
@@ -335,16 +335,40 @@
     def initialize_with_params(self):
         # must set WantTensors manually if using external_primordial_pk
         if not self.external_primordial_pk \
                 and set(self.input_params).intersection({'r', 'At'}):
             self.extra_attrs["WantTensors"] = True
             self.extra_attrs["Accuracy.AccurateBB"] = True
 
+        if "sigma8" in self.input_params:
+            if "As" in self.input_params:
+                raise LoggedError(self.log,
+                                  "Both As and sigma8 have been provided as input. "
+                                  "This will likely cause ill-defined outputs.")
+            self.extra_attrs["WantTransfer"] = True
+            self.add_to_redshifts([0.])
+
+    def initialize_with_provider(self, provider):
+        if "sigma8" in self.input_params or "As" in self.output_params:
+            if not self.needs_perts:
+                raise LoggedError(self.log, "Using sigma8 as input or As as output "
+                                            "but not using any power spectrum results")
+            if (power_model := self.extra_args.get('initial_power_model')) and not \
+                    isinstance(self.camb.CAMBparams.make_class_named(power_model),
+                               self.camb.initialpower.InitialPowerLaw):
+                raise LoggedError(self.log, "Using sigma8 as an input and As as an "
+                                            "output is only supported for power law "
+                                            "initial power spectra.")
+        super().initialize_with_provider(provider)
+
     def get_can_support_params(self):
-        return self.power_params + self.nonlin_params
+        params = self.power_params + self.nonlin_params
+        if not self.external_primordial_pk:
+            params += ["sigma8"]
+        return params
 
     def get_allow_agnostic(self):
         return False
 
     def set_cl_reqs(self, reqs):
         """
         Sets some common settings for both lensed and unlensed Cl's.
@@ -593,22 +617,27 @@
                     results.Params.InitPower.set_params(**args)
                 if self.non_linear_sources or self.non_linear_pk:
                     args = {self.translate_param(p): v for p, v in
                             params_values_dict.items() if p in self.nonlin_params}
                     args.update(self.nonlin_args)
                     results.Params.NonLinearModel.set_params(**args)
                 results.power_spectra_from_transfer()
+                if "sigma8" in params_values_dict:
+                    sigma8 = results.get_sigma8_0()
+                    results.Params.InitPower.As *= params_values_dict[
+                                                       "sigma8"] ** 2 / sigma8 ** 2
+                    results.power_spectra_from_transfer()
             for product, collector in self.collectors.items():
                 if collector:
                     state[product] = \
                         collector.method(results, *collector.args, **collector.kwargs)
                     if collector.post:
                         state[product] = collector.post(*state[product])
                 else:
-                    state[product] = results
+                    state[product] = results.copy()
         except self.camb.baseconfig.CAMBError as e:
             if self.stop_at_error:
                 self.log.error(
                     "Computation error (see traceback below)! "
                     "Parameters sent to CAMB: %r and %r.\n"
                     "To ignore this kind of error, make 'stop_at_error: False'.",
                     dict(state["params"]), dict(self.extra_args))
@@ -638,14 +667,16 @@
         if intermediates.derived:
             derived = intermediates.derived.get(p, None)
             if derived is not None:
                 return derived
         # Specific calls, if general ones fail:
         if p == "sigma8":
             return intermediates.results.get_sigma8_0()
+        if p == "As":
+            return intermediates.results.Params.InitPower.As
         try:
             return getattr(intermediates.camb_params, p)
         except AttributeError:
             try:
                 return getattr(intermediates.results, p)
             except AttributeError:
                 return getattr(intermediates.camb_params, "get_" + p, lambda: None)()
@@ -751,14 +782,16 @@
         fields = []
         # noinspection PyProtectedMember
         for f, tp in self.camb.CAMBparams._fields_:
             if tp is ctypes.c_double and 'max_eta_k' not in f \
                     and f not in ['Alens', 'num_nu_massless']:
                 fields.append(f)
         fields += ['omega_de', 'sigma8']  # only parameters from CAMBdata
+        if not self.external_primordial_pk:
+            fields += ['As']
         properties = get_properties(self.camb.CAMBparams)
         names = self.camb.model.derived_names + properties + fields + params_derived
         for name, mapped in self.renames.items():
             if mapped in names:
                 names.append(name)
         # remove any parameters explicitly tagged as input requirements
         return set(names).difference(chain(self._transfer_requires, self.requires))
@@ -766,16 +799,15 @@
     def get_version(self):
         return self.camb.__version__
 
     def set(self, params_values_dict, state):
         # Prepare parameters to be passed: this is called from the CambTransfers instance
         args = {self.translate_param(p): v for p, v in params_values_dict.items()}
         # Generate and save
-        self.log.debug("Setting parameters: %r and %r",
-                       dict(args), dict(self.extra_args))
+        self.log.debug("Setting parameters: %r and %r", args, self.extra_args)
         try:
             if not self._base_params:
                 base_args = args.copy()
                 base_args.update(self.extra_args)
                 # Remove extra args that might
                 # cause an error if the associated product is not requested
                 if not self.extra_attrs["WantCls"]:
```

### Comparing `cobaya-3.3.1/cobaya/theories/camb/camb.yaml` & `cobaya-3.3.2/cobaya/theories/camb/camb.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/theories/classy/classy.bibtex` & `cobaya-3.3.2/cobaya/theories/classy/classy.bibtex`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/theories/classy/classy.py` & `cobaya-3.3.2/cobaya/theories/classy/classy.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/theories/classy/classy.yaml` & `cobaya-3.3.2/cobaya/theories/classy/classy.yaml`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/theories/cosmo/boltzmannbase.py` & `cobaya-3.3.2/cobaya/theories/cosmo/boltzmannbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
                 #                 ": %r vs %r.", source, window, self.sources[source])
                 self._must_provide[k].update(v)
             elif k in {"Hubble", "Omega_b", "Omega_cdm", "Omega_nu_massive",
                        "angular_diameter_distance", "comoving_radial_distance",
                        "sigma8_z", "fsigma8"}:
                 if k not in self._must_provide:
                     self._must_provide[k] = {}
-                if not isinstance(v, Iterable) or "z" not in v:
+                if not isinstance(v, Mapping) or "z" not in v:
                     raise LoggedError(
                         self.log,
                         f"The value in the dictionary of requisites {k} must be a "
                         "dictionary containing the key 'z' with a list of redshifts "
                         f"(got instead {{{k}: {v}}})"
                     )
                 self._must_provide[k]["z"] = combine_1d(
```

### Comparing `cobaya-3.3.1/cobaya/theory.py` & `cobaya-3.3.2/cobaya/theory.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/tools.py` & `cobaya-3.3.2/cobaya/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import pandas as pd
 import numpy as np
 from itertools import chain
 from importlib import import_module
 from copy import deepcopy
 from packaging import version
 from itertools import permutations
-from typing import Mapping, Sequence, Any, List, TypeVar, Optional, Union, Iterable, Dict
+from typing import Mapping, Sequence, Any, List, TypeVar, Optional, Union, Iterable, \
+    Dict, Callable
 from types import ModuleType
 from inspect import cleandoc, getfullargspec
 from ast import parse
 from abc import ABC, abstractmethod
 
 # Local
 from cobaya.conventions import subfolders, kinds, packages_path_config_file, \
@@ -761,14 +762,17 @@
         _copy = {}
         for key, value in base.items():
             _copy[key] = deepcopy_where_possible(value)
         return _copy  # type: ignore
     if isinstance(base, (HasLogger, type)):
         return base  # type: ignore
     else:
+        # Special case: instance methods can be copied, but should not be.
+        if isinstance(base, Callable) and hasattr(base, "__self__"):
+            return base
         try:
             return deepcopy(base)
         except:
             return base
 
 
 def get_class_methods(cls, not_base=None, start='get_', excludes=(), first='self'):
```

### Comparing `cobaya-3.3.1/cobaya/typing.py` & `cobaya-3.3.2/cobaya/typing.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya/yaml.py` & `cobaya-3.3.2/cobaya/yaml.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/cobaya.egg-info/PKG-INFO` & `cobaya-3.3.2/cobaya.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya
-Version: 3.3.1
+Version: 3.3.2
 Summary: Code for Bayesian Analysis
 Home-page: https://cobaya.readthedocs.io
 Author: Jesus Torrado and Antony Lewis
 License: LGPL
 Project-URL: Source, https://github.com/CobayaSampler/cobaya
 Project-URL: Tracker, https://github.com/CobayaSampler/cobaya/issues
 Project-URL: Licensing, https://github.com/CobayaSampler/cobaya/blob/master/LICENCE.txt
@@ -40,20 +40,22 @@
 
 :Support: For general support, CosmoCoffee_; for bugs and issues, use the `issue tracker <https://github.com/CobayaSampler/cobaya/issues>`_.
 
 :Installation: ``pip install cobaya --upgrade`` (see the `installation instructions <https://cobaya.readthedocs.io/en/latest/installation.html>`_; in general do *not* clone)
 
 .. image:: https://travis-ci.com/CobayaSampler/cobaya.svg?branch=master
    :target: https://app.travis-ci.com/CobayaSampler/cobaya
-.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
-   :target: https://pypi.python.org/pypi/cobaya/
 .. image:: https://readthedocs.org/projects/cobaya/badge/?version=latest
    :target: https://cobaya.readthedocs.org/en/latest
 .. image:: https://codecov.io/gh/CobayaSampler/cobaya/branch/master/graphs/badge.svg
    :target: https://codecov.io/github/CobayaSampler/cobaya/branch/master
+.. image:: https://img.shields.io/pypi/v/cobaya.svg?style=flat
+   :target: https://pypi.python.org/pypi/cobaya/
+.. image:: https://static.pepy.tech/personalized-badge/cobaya?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads
+   :target: https://pepy.tech/project/cobaya
 .. image:: https://img.shields.io/badge/arXiv-2005.05290-b31b1b.svg?color=0B6523
    :target: https://arxiv.org/abs/2005.05290
 
 **Cobaya** (**co**\ de for **bay**\ esian **a**\ nalysis, and Spanish for *Guinea Pig*) is a framework for sampling and statistical modelling: it allows you to explore an arbitrary prior or posterior using a range of Monte Carlo samplers (including the advanced MCMC sampler from CosmoMC_, and the advanced nested sampler PolyChord_). The results of the sampling can be analysed with GetDist_. It supports MPI parallelization (and very soon HPC containerization with Docker/Shifter and Singularity).
 
 Its authors are `Jesus Torrado`_ and `Antony Lewis`_. Some ideas and pieces of code have been adapted from other codes (e.g CosmoMC_ by `Antony Lewis`_ and contributors, and `Monte Python`_, by `J. Lesgourgues`_ and `B. Audren`_).
```

### Comparing `cobaya-3.3.1/cobaya.egg-info/SOURCES.txt` & `cobaya-3.3.2/cobaya.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,16 @@
 cobaya/likelihoods/planck_2018_lensing/__init__.py
 cobaya/likelihoods/planck_2018_lensing/clik.py
 cobaya/likelihoods/planck_2018_lensing/clik.yaml
 cobaya/likelihoods/planck_2018_lensing/native.yaml
 cobaya/likelihoods/planck_2018_lowl/EE.py
 cobaya/likelihoods/planck_2018_lowl/EE_clik.py
 cobaya/likelihoods/planck_2018_lowl/EE_clik.yaml
+cobaya/likelihoods/planck_2018_lowl/EE_sroll2.bibtex
+cobaya/likelihoods/planck_2018_lowl/EE_sroll2.py
 cobaya/likelihoods/planck_2018_lowl/TT.py
 cobaya/likelihoods/planck_2018_lowl/TT_clik.py
 cobaya/likelihoods/planck_2018_lowl/TT_clik.yaml
 cobaya/likelihoods/planck_2018_lowl/__init__.py
 cobaya/likelihoods/planck_NPIPE_highl_CamSpec/CamSpec_NPIPE_2022.bibtex
 cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.py
 cobaya/likelihoods/planck_NPIPE_highl_CamSpec/EE.yaml
@@ -297,14 +299,15 @@
 cobaya/theories/classy/classy.yaml
 cobaya/theories/cosmo/__init__.py
 cobaya/theories/cosmo/boltzmannbase.py
 tests/test_cosmo_H0.py
 tests/test_cosmo_bao.py
 tests/test_cosmo_bicep_keck_2018.py
 tests/test_cosmo_camb.py
+tests/test_cosmo_camb_sigma_8_input.py
 tests/test_cosmo_des_y1.py
 tests/test_cosmo_docs_basic.py
 tests/test_cosmo_docs_likelihood.py
 tests/test_cosmo_docs_model.py
 tests/test_cosmo_multi_theory.py
 tests/test_cosmo_planck_2015.py
 tests/test_cosmo_planck_2018.py
```

### Comparing `cobaya-3.3.1/cobaya.egg-info/entry_points.txt` & `cobaya-3.3.2/cobaya.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/setup.py` & `cobaya-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     i_first = next(i for i, line in enumerate(lines)
                    if line.strip().startswith("-e")) + 1
     reqs = [line.strip() for line in lines[i_first:]]
     return ["sphinx"] + reqs
 
 
 install_requires = ['numpy>=1.17.0', 'scipy>=1.5', 'pandas>=1.0.1',
-                    'PyYAML>=5.1', 'requests>=2.18', 'py-bobyqa>=1.2',
+                    'PyYAML>=5.1', 'requests>=2.18', 'py-bobyqa>=1.4',
                     'GetDist>=1.3.1', 'fuzzywuzzy>=0.17', 'packaging', 'tqdm',
                     'portalocker>=2.3.0', 'dill>=0.3.3']
 
 setup(
     name='cobaya',
     version=find_version(),
     description='Code for Bayesian Analysis',
```

### Comparing `cobaya-3.3.1/tests/test_cosmo_H0.py` & `cobaya-3.3.2/tests/test_cosmo_H0.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_bao.py` & `cobaya-3.3.2/tests/test_cosmo_bao.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_bicep_keck_2018.py` & `cobaya-3.3.2/tests/test_cosmo_bicep_keck_2018.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_camb.py` & `cobaya-3.3.2/tests/test_cosmo_camb.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_des_y1.py` & `cobaya-3.3.2/tests/test_cosmo_des_y1.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_docs_basic.py` & `cobaya-3.3.2/tests/test_cosmo_docs_basic.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_docs_likelihood.py` & `cobaya-3.3.2/tests/test_cosmo_docs_likelihood.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_docs_model.py` & `cobaya-3.3.2/tests/test_cosmo_docs_model.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_multi_theory.py` & `cobaya-3.3.2/tests/test_cosmo_multi_theory.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_planck_2015.py` & `cobaya-3.3.2/tests/test_cosmo_planck_2015.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_planck_2018.py` & `cobaya-3.3.2/tests/test_cosmo_planck_2018.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_planck_NPIPE.py` & `cobaya-3.3.2/tests/test_cosmo_planck_NPIPE.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_quantities.py` & `cobaya-3.3.2/tests/test_cosmo_quantities.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_run.py` & `cobaya-3.3.2/tests/test_cosmo_run.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_cosmo_sn.py` & `cobaya-3.3.2/tests/test_cosmo_sn.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_dependencies.py` & `cobaya-3.3.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_docs_example_quickstart.py` & `cobaya-3.3.2/tests/test_docs_example_quickstart.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_docs_model.py` & `cobaya-3.3.2/tests/test_docs_model.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_input.py` & `cobaya-3.3.2/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_likelihood_external.py` & `cobaya-3.3.2/tests/test_likelihood_external.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 The test likelihood is a gaussian half-ring, combined with a gaussian in one of the tests.
 
 For manual testing, and observing/plotting the density, pass ``manual=True`` to
 ``body of test``.
 """
 
 # Local
-from .common_external import info_string, info_callable, info_mixed, info_import
-from .common_external import info_derived, body_of_test
+from .common_external import info_string, info_callable, info_mixed, info_import, \
+    info_method_args, info_method_kwargs, info_method_unnamed_kwargs, info_derived, \
+    body_of_test
 
 
 def test_likelihood_external_string(tmpdir):
     body_of_test(info_string, "likelihood", tmpdir)
 
 
 def test_likelihood_external_callable(tmpdir):
@@ -31,7 +32,19 @@
 
 def test_likelihood_external_import(tmpdir):
     body_of_test(info_import, "likelihood", tmpdir)
 
 
 def test_likelihood_external_derived(tmpdir):
     body_of_test(info_derived, "likelihood", tmpdir, derived=True)
+
+
+def test_likelihood_external_method_args(tmpdir):
+    body_of_test(info_method_args, "likelihood", tmpdir)
+
+
+def test_likelihood_external_method_kwargs(tmpdir):
+    body_of_test(info_method_kwargs, "likelihood", tmpdir)
+
+
+def test_likelihood_external_method_unnamed_kwargs(tmpdir):
+    body_of_test(info_method_unnamed_kwargs, "likelihood", tmpdir)
```

### Comparing `cobaya-3.3.1/tests/test_mcmc.py` & `cobaya-3.3.2/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_mcmc_initial_covmat.py` & `cobaya-3.3.2/tests/test_mcmc_initial_covmat.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_minimize.py` & `cobaya-3.3.2/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_parameterization.py` & `cobaya-3.3.2/tests/test_parameterization.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_polychord.py` & `cobaya-3.3.2/tests/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_pools.py` & `cobaya-3.3.2/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_post.py` & `cobaya-3.3.2/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_prior.py` & `cobaya-3.3.2/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_prior_external.py` & `cobaya-3.3.2/tests/test_prior_external.py`

 * *Files identical despite different names*

### Comparing `cobaya-3.3.1/tests/test_ref.py` & `cobaya-3.3.2/tests/test_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     assert model.prior.ref_pdf[2] == val
     assert model.prior.ref_pdf[3] == upd1_ref_info["d"]
     assert model.prior.ref_pdf[4] == upd1_ref_info["e"]
     # Should be non-point-like again
     assert not model.prior.reference_is_pointlike
 
 
-# Tests MPI-awareness of the referece, when using it to get the initial point of mcmc
+# Tests MPI-awareness of the reference, when using it to get the initial point of mcmc
 @pytest.mark.mpi
 @mpi.sync_errors
 def test_ref_mcmc_initial_point():
     val = 0.5
     info = {
         "params": {"a": {"prior": [0, 1 + mpi.size()], "ref": val + mpi.rank()}},
         "likelihood": {"one": None}}
```

### Comparing `cobaya-3.3.1/tests/test_scripts.py` & `cobaya-3.3.2/tests/test_scripts.py`

 * *Files identical despite different names*

