# Comparing `tmp/pyro-ppl-1.8.5.tar.gz` & `tmp/pyro-ppl-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyro-ppl-1.8.5.tar", last modified: Mon May 29 03:00:47 2023, max compression
+gzip compressed data, was "pyro-ppl-1.8.6.tar", last modified: Sat Jul 29 21:08:19 2023, max compression
```

## Comparing `pyro-ppl-1.8.5.tar` & `pyro-ppl-1.8.6.tar`

### file list

```diff
@@ -1,367 +1,374 @@
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899750 pyro-ppl-1.8.5/
--rw-r--r--   0 fritzo     (501) staff       (20)    11358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/LICENSE.md
--rw-r--r--   0 fritzo     (501) staff       (20)       60 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/MANIFEST.in
--rw-r--r--   0 fritzo     (501) staff       (20)     4768 2023-05-29 03:00:47.899828 pyro-ppl-1.8.5/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)     4538 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/README.md
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.842709 pyro-ppl-1.8.5/pyro/
--rw-r--r--   0 fritzo     (501) staff       (20)     1324 2023-05-29 01:08:09.000000 pyro-ppl-1.8.5/pyro/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      113 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro/_version.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.843481 pyro-ppl-1.8.5/pyro/contrib/
--rw-r--r--   0 fritzo     (501) staff       (20)      693 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844148 pyro-ppl-1.8.5/pyro/contrib/autoname/
--rw-r--r--   0 fritzo     (501) staff       (20)      486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5143 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/autoname.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/named.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6482 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/scoping.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844514 pyro-ppl-1.8.5/pyro/contrib/bnn/
--rw-r--r--   0 fritzo     (501) staff       (20)      177 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/hidden_layer.py
--rw-r--r--   0 fritzo     (501) staff       (20)      490 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/utils.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844638 pyro-ppl-1.8.5/pyro/contrib/cevae/
--rw-r--r--   0 fritzo     (501) staff       (20)    22960 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/cevae/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844880 pyro-ppl-1.8.5/pyro/contrib/conjugate/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/conjugate/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9073 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/conjugate/infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.845124 pyro-ppl-1.8.5/pyro/contrib/easyguide/
--rw-r--r--   0 fritzo     (501) staff       (20)      206 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/easyguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12912 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/contrib/easyguide/easyguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.846198 pyro-ppl-1.8.5/pyro/contrib/epidemiology/
--rw-r--r--   0 fritzo     (501) staff       (20)      406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49835 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/compartmental.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    51169 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10990 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.847433 pyro-ppl-1.8.5/pyro/contrib/examples/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6760 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/bart.py
--rw-r--r--   0 fritzo     (501) staff       (20)      694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/finance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2920 2023-05-28 13:37:12.000000 pyro-ppl-1.8.5/pyro/contrib/examples/multi_mnist.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/nextstrain.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/polyphonic_data_loader.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7442 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/scanvi_data.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1556 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.847960 pyro-ppl-1.8.5/pyro/contrib/forecast/
--rw-r--r--   0 fritzo     (501) staff       (20)      360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8823 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/evaluate.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/forecaster.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16054 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.848087 pyro-ppl-1.8.5/pyro/contrib/funsor/
--rw-r--r--   0 fritzo     (501) staff       (20)     1263 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.849471 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/
--rw-r--r--   0 fritzo     (501) staff       (20)      912 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9727 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7623 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/named_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15224 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1804 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8558 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3632 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/trace_messenger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.850324 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)      514 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2921 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1652 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1698 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12663 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1882 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/tracetmc_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.850792 pyro-ppl-1.8.5/pyro/contrib/gp/
--rw-r--r--   0 fritzo     (501) staff       (20)      340 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.851792 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/
--rw-r--r--   0 fritzo     (501) staff       (20)     1533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/brownian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3699 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/coregionalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2646 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/dot_product.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/isotropic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8446 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/periodic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/static.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.852497 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/
--rw-r--r--   0 fritzo     (501) staff       (20)      897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1988 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/binary.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1677 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/likelihood.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2859 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/multi_class.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1884 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/poisson.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.853731 pyro-ppl-1.8.5/pyro/contrib/gp/models/
--rw-r--r--   0 fritzo     (501) staff       (20)      546 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/gplvm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8932 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/gpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9145 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/model.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11001 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/sgpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6859 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/vgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8417 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/vsgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8058 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/parameterized.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7152 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15591 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/minipyro.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.854669 pyro-ppl-1.8.5/pyro/contrib/mue/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6063 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/mue/dataloaders.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/missingdatahmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    34329 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/mue/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9017 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/statearrangers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.855469 pyro-ppl-1.8.5/pyro/contrib/oed/
--rw-r--r--   0 fritzo     (501) staff       (20)     3789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    44795 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/eig.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.856010 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/
--rw-r--r--   0 fritzo     (501) staff       (20)     1551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16376 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/glmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11368 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)      867 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/search.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1230 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.858474 pyro-ppl-1.8.5/pyro/contrib/randomvariable/
--rw-r--r--   0 fritzo     (501) staff       (20)      193 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/randomvariable/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/randomvariable/random_variable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.859404 pyro-ppl-1.8.5/pyro/contrib/timeseries/
--rw-r--r--   0 fritzo     (501) staff       (20)      711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2211 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/base.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23486 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6439 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11250 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssmgp.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.860368 pyro-ppl-1.8.5/pyro/contrib/tracking/
--rw-r--r--   0 fritzo     (501) staff       (20)      167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19243 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/assignment.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3576 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16560 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/dynamic_models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7796 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/extended_kalman_filter.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/hashing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4544 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/measurements.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2800 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/contrib/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.868761 pyro-ppl-1.8.5/pyro/distributions/
--rw-r--r--   0 fritzo     (501) staff       (20)     5548 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/distributions/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3985 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/affine_beta.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/asymmetriclaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4062 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/avf_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20914 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/coalescent.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4815 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/conditional.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/constraints.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/delta.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10356 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9012 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture_shared_cov.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8443 2022-04-10 23:10:00.000000 pyro-ppl-1.8.5/pyro/distributions/distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6765 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/empirical.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1885 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/extended.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1290 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/folded.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7983 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/gaussian_scale_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6571 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/distributions/grouped_normal_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)    54250 2023-01-13 02:07:01.000000 pyro-ppl-1.8.5/pyro/distributions/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2448 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/improper_uniform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1429 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/inverse_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1661 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/kl.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/lkj.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5719 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/log_normal_negative_binomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5474 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5193 2022-06-12 12:50:39.000000 pyro-ppl-1.8.5/pyro/distributions/multivariate_studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3381 2022-07-16 22:52:12.000000 pyro-ppl-1.8.5/pyro/distributions/nanmasked.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3176 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/omt_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/one_one_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/one_two_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2874 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/ordered_logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3090 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/polya_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7441 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/distributions/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2933 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/rejector.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3637 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/relaxed_straight_through.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1125 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/score_parts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11563 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/sine_bivariate_von_mises.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/sine_skewed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2471 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/softlaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7746 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/spanning_tree.cpp
--rw-r--r--   0 fritzo     (501) staff       (20)    22257 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/spanning_tree.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8208 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/stable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.869999 pyro-ppl-1.8.5/pyro/distributions/testing/
--rw-r--r--   0 fritzo     (501) staff       (20)      215 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      421 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/fakes.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10761 2022-07-10 14:38:43.000000 pyro-ppl-1.8.5/pyro/distributions/testing/gof.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1598 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/naive_dirichlet.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/rejection_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8842 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/rejection_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3610 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13608 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/distributions/torch.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20332 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/distributions/torch_distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3044 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/torch_patch.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1452 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/torch_transform.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.874166 pyro-ppl-1.8.5/pyro/distributions/transforms/
--rw-r--r--   0 fritzo     (501) staff       (20)     6835 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16342 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/affine_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15805 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/affine_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2075 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/basic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6147 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/batchnorm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11702 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/block_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2115 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11680 2022-11-22 19:06:49.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/generalized_channel_permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2883 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/householder.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2479 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/lower_cholesky_affine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13725 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/matrix_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/neural_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1072 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/normalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)      921 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/ordered.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/planar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/polynomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2138 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/power.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/radial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/softplus.py
--rw-r--r--   0 fritzo     (501) staff       (20)    24458 2022-10-30 02:11:10.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11370 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6917 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/sylvester.py
--rw-r--r--   0 fritzo     (501) staff       (20)      809 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/unit_cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)      282 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/unit.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11913 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/distributions/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/von_mises_3d.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6861 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/zero_inflated.py
--rw-r--r--   0 fritzo     (501) staff       (20)      266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/generic.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.880293 pyro-ppl-1.8.5/pyro/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)     2041 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15986 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/abstract_infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.881965 pyro-ppl-1.8.5/pyro/infer/autoguide/
--rw-r--r--   0 fritzo     (501) staff       (20)     1618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19662 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/effect.py
--rw-r--r--   0 fritzo     (501) staff       (20)    26014 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49080 2022-11-25 23:04:16.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/initialization.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16327 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3089 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7251 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/csis.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9535 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10044 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/energy_distance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8063 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/enum.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9701 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/importance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21777 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/infer/inspect.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.883482 pyro-ppl-1.8.5/pyro/infer/mcmc/
--rw-r--r--   0 fritzo     (501) staff       (20)      412 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23000 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/adaptation.py
--rw-r--r--   0 fritzo     (501) staff       (20)    29191 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/api.py
--rw-r--r--   0 fritzo     (501) staff       (20)    18829 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/hmc.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/logger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2347 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/mcmc_kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21893 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/nuts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    33005 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11083 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/predictive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9418 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/renyi_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.885931 pyro-ppl-1.8.5/pyro/infer/reparam/
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4315 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3812 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/loc_scale.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/neutra.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2627 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/reparam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1869 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/softmax.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2642 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/split.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10231 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/stable.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7481 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/strategies.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4312 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1477 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/transform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3913 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/unit_jacobian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5720 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/infer/resampler.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11084 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/rws.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8713 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/smcfilter.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12959 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/svgd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5947 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/svi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10334 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_mean_field_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10876 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_mmd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3367 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_tail_adaptive_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23531 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16979 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/infer/tracegraph_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8714 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/tracetmc_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12502 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/infer/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)      463 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/logger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.886610 pyro-ppl-1.8.5/pyro/nn/
--rw-r--r--   0 fritzo     (501) staff       (20)      602 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/auto_reg_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5124 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/dense_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    31542 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/nn/module.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.890415 pyro-ppl-1.8.5/pyro/ops/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4306 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/arrowhead.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22550 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/ops/contract.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3402 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/dual_averaging.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.891519 pyro-ppl-1.8.5/pyro/ops/einsum/
--rw-r--r--   0 fritzo     (501) staff       (20)     1486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4971 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/adjoint.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2010 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_log.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1952 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_map.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2234 2022-07-05 20:35:43.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_marginal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2736 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_sample.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1901 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17941 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/gamma_gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    28046 2022-10-30 17:11:32.000000 pyro-ppl-1.8.5/pyro/ops/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/hessian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7458 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/indexing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5119 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/ops/integrator.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5970 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/jit.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/linalg.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9520 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/newton.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6350 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/packed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5651 2023-05-28 15:09:30.000000 pyro-ppl-1.8.5/pyro/ops/provenance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11388 2022-07-05 20:10:55.000000 pyro-ppl-1.8.5/pyro/ops/rings.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7050 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/ops/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6648 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/ssm_gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17109 2022-07-10 14:38:43.000000 pyro-ppl-1.8.5/pyro/ops/stats.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8903 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/streaming.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15783 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/ops/tensor_utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3405 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/welford.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.892830 pyro-ppl-1.8.5/pyro/optim/
--rw-r--r--   0 fritzo     (501) staff       (20)      594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3060 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/adagrad_rmsprop.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3462 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/clipped_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7634 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/dct_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1906 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/horovod.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2351 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/lr_scheduler.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/multi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10610 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/optim/optim.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2064 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/optim/pytorch_optimizers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.893127 pyro-ppl-1.8.5/pyro/params/
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/params/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13144 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/params/param_store.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899104 pyro-ppl-1.8.5/pyro/poutine/
--rw-r--r--   0 fritzo     (501) staff       (20)      922 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4794 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/block_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3528 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/broadcast_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6129 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/collapse_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2128 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/condition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3152 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/do_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9671 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1228 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/escape_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5427 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/poutine/guide.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8605 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/handlers.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3849 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/indep_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1744 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/infer_config_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4830 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/lift_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3139 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/markov_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/mask_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8691 2022-06-12 12:50:39.000000 pyro-ppl-1.8.5/pyro/poutine/messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)      664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/reentrant_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/reparam_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2982 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10402 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/scale_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1047 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/seed_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7725 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/poutine/subsample_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2935 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/substitute_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/trace_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/trace_struct.py
--rw-r--r--   0 fritzo     (501) staff       (20)      821 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/uncondition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4073 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/poutine/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5019 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/settings.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22051 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899654 pyro-ppl-1.8.5/pyro_ppl.egg-info/
--rw-r--r--   0 fritzo     (501) staff       (20)     4768 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)    10593 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/SOURCES.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        1 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/dependency_links.txt
--rw-r--r--   0 fritzo     (501) staff       (20)      901 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/requires.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        5 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/top_level.txt
--rw-r--r--   0 fritzo     (501) staff       (20)     1986 2023-05-29 03:00:47.900225 pyro-ppl-1.8.5/setup.cfg
--rw-r--r--   0 fritzo     (501) staff       (20)     5097 2023-05-28 13:37:12.000000 pyro-ppl-1.8.5/setup.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.253261 pyro-ppl-1.8.6/
+-rw-r--r--   0 fritzo     (501) staff       (20)    11358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/LICENSE.md
+-rw-r--r--   0 fritzo     (501) staff       (20)       60 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/MANIFEST.in
+-rw-r--r--   0 fritzo     (501) staff       (20)     4788 2023-07-29 21:08:19.253360 pyro-ppl-1.8.6/PKG-INFO
+-rw-r--r--   0 fritzo     (501) staff       (20)     4538 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/README.md
+-rw-r--r--   0 fritzo     (501) staff       (20)       81 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyproject.toml
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.191542 pyro-ppl-1.8.6/pyro/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1324 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      113 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro/_version.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.192378 pyro-ppl-1.8.6/pyro/contrib/
+-rw-r--r--   0 fritzo     (501) staff       (20)      693 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoguide.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193067 pyro-ppl-1.8.6/pyro/contrib/autoname/
+-rw-r--r--   0 fritzo     (501) staff       (20)      486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5143 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/autoname.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/named.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6482 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/autoname/scoping.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193425 pyro-ppl-1.8.6/pyro/contrib/bnn/
+-rw-r--r--   0 fritzo     (501) staff       (20)      177 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/hidden_layer.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      490 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/bnn/utils.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193539 pyro-ppl-1.8.6/pyro/contrib/cevae/
+-rw-r--r--   0 fritzo     (501) staff       (20)    22960 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/cevae/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.193782 pyro-ppl-1.8.6/pyro/contrib/conjugate/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/conjugate/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9073 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/conjugate/infer.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.194029 pyro-ppl-1.8.6/pyro/contrib/easyguide/
+-rw-r--r--   0 fritzo     (501) staff       (20)      206 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/easyguide/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12912 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/easyguide/easyguide.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.195178 pyro-ppl-1.8.6/pyro/contrib/epidemiology/
+-rw-r--r--   0 fritzo     (501) staff       (20)      406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    49835 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/compartmental.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/distributions.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    51169 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10990 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/epidemiology/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.196474 pyro-ppl-1.8.6/pyro/contrib/examples/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6760 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/bart.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/finance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2920 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/examples/multi_mnist.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/nextstrain.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/polyphonic_data_loader.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7442 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/scanvi_data.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1556 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/examples/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.197159 pyro-ppl-1.8.6/pyro/contrib/forecast/
+-rw-r--r--   0 fritzo     (501) staff       (20)      360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8823 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/evaluate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23353 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/forecaster.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16054 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/forecast/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.197285 pyro-ppl-1.8.6/pyro/contrib/funsor/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1223 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.198662 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/
+-rw-r--r--   0 fritzo     (501) staff       (20)      912 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9727 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/enum_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7623 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/named_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15224 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/plate_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/primitives.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1804 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/replay_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8558 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/runtime.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3632 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/trace_messenger.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.199389 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/
+-rw-r--r--   0 fritzo     (501) staff       (20)      514 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2921 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/discrete.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1652 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1698 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/trace_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12663 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/traceenum_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1882 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/funsor/infer/tracetmc_elbo.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.199851 pyro-ppl-1.8.6/pyro/contrib/gp/
+-rw-r--r--   0 fritzo     (501) staff       (20)      340 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.201189 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/brownian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3699 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/coregionalize.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2646 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/dot_product.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/isotropic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8446 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/kernel.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/periodic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/kernels/static.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.202035 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/
+-rw-r--r--   0 fritzo     (501) staff       (20)      897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1988 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/binary.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1677 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/likelihood.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2859 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/multi_class.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1884 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/poisson.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.204359 pyro-ppl-1.8.6/pyro/contrib/gp/models/
+-rw-r--r--   0 fritzo     (501) staff       (20)      546 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/gplvm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8932 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/gpr.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9145 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/model.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11001 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/sgpr.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6859 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/vgp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8417 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/models/vsgp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8058 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/parameterized.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7152 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/gp/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15591 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/minipyro.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.205290 pyro-ppl-1.8.6/pyro/contrib/mue/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6063 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/mue/dataloaders.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/missingdatahmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    34329 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/mue/models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9017 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/mue/statearrangers.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.207638 pyro-ppl-1.8.6/pyro/contrib/oed/
+-rw-r--r--   0 fritzo     (501) staff       (20)     3789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    44795 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/eig.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.208062 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16376 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/glmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11368 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/oed/glmm/guides.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      867 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/search.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1230 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/oed/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.208419 pyro-ppl-1.8.6/pyro/contrib/randomvariable/
+-rw-r--r--   0 fritzo     (501) staff       (20)      193 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/randomvariable/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/randomvariable/random_variable.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.209095 pyro-ppl-1.8.6/pyro/contrib/timeseries/
+-rw-r--r--   0 fritzo     (501) staff       (20)      711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2211 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/base.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23486 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/gp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6439 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11250 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssmgp.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.210262 pyro-ppl-1.8.6/pyro/contrib/tracking/
+-rw-r--r--   0 fritzo     (501) staff       (20)      167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    19243 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/assignment.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3576 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/distributions.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16560 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/dynamic_models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7796 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/extended_kalman_filter.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/hashing.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4544 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/contrib/tracking/measurements.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2800 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/contrib/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.218750 pyro-ppl-1.8.6/pyro/distributions/
+-rw-r--r--   0 fritzo     (501) staff       (20)     5548 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/distributions/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3985 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/affine_beta.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/asymmetriclaplace.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4062 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/avf_mvn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20914 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/coalescent.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4815 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/conditional.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/conjugate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4352 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/distributions/constraints.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/delta.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10356 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9012 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture_shared_cov.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8443 2022-04-10 23:10:00.000000 pyro-ppl-1.8.6/pyro/distributions/distribution.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6765 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/empirical.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1885 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/extended.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1290 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/folded.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7983 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/gaussian_scale_mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6571 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/distributions/grouped_normal_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    54250 2023-01-13 02:07:01.000000 pyro-ppl-1.8.6/pyro/distributions/hmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2448 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/improper_uniform.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1429 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/inverse_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1661 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/kl.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/lkj.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5719 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/log_normal_negative_binomial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5474 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/logistic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5193 2022-06-12 12:50:39.000000 pyro-ppl-1.8.6/pyro/distributions/multivariate_studentt.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3381 2022-07-16 22:52:12.000000 pyro-ppl-1.8.6/pyro/distributions/nanmasked.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3176 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/omt_mvn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/one_one_matching.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/one_two_matching.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2874 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/ordered_logistic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3090 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/polya_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7441 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/distributions/projected_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2933 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/rejector.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3637 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/relaxed_straight_through.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1125 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/score_parts.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11563 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/sine_bivariate_von_mises.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/sine_skewed.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2471 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/softlaplace.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7746 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/spanning_tree.cpp
+-rw-r--r--   0 fritzo     (501) staff       (20)    22257 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/spanning_tree.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8208 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/stable.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.220022 pyro-ppl-1.8.6/pyro/distributions/testing/
+-rw-r--r--   0 fritzo     (501) staff       (20)      215 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      421 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/fakes.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10761 2022-07-10 14:38:43.000000 pyro-ppl-1.8.6/pyro/distributions/testing/gof.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1598 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/naive_dirichlet.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/rejection_exponential.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8842 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/rejection_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3610 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/testing/special.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    14028 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/distributions/torch.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20332 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/distributions/torch_distribution.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3044 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/torch_patch.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1452 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/torch_transform.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.224482 pyro-ppl-1.8.6/pyro/distributions/transforms/
+-rw-r--r--   0 fritzo     (501) staff       (20)     6835 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16342 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/affine_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15805 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/affine_coupling.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2075 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/basic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6147 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/batchnorm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11702 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/block_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2115 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/cholesky.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/discrete_cosine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11680 2022-11-22 19:06:49.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/generalized_channel_permute.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2883 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/haar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/householder.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2479 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/lower_cholesky_affine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13725 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/matrix_exponential.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/neural_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1072 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/normalize.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      921 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/ordered.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/permute.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/planar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/polynomial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2138 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/power.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/radial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/softplus.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    24458 2022-10-30 02:11:10.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11370 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6917 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/spline_coupling.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/sylvester.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      809 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/unit_cholesky.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      282 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/transforms/utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/unit.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11913 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/distributions/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/von_mises_3d.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6861 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/distributions/zero_inflated.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/generic.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.228735 pyro-ppl-1.8.6/pyro/infer/
+-rw-r--r--   0 fritzo     (501) staff       (20)     2041 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15986 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/abstract_infer.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.230463 pyro-ppl-1.8.6/pyro/infer/autoguide/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    19662 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/effect.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    26014 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    49205 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/guides.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/initialization.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16327 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/structured.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3089 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/autoguide/utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7251 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/csis.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/discrete.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9535 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10044 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/energy_distance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8063 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/enum.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9701 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/importance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    21777 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/inspect.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.231907 pyro-ppl-1.8.6/pyro/infer/mcmc/
+-rw-r--r--   0 fritzo     (501) staff       (20)      412 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23000 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/adaptation.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    29191 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/api.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    18829 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/hmc.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/logger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2347 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/mcmc_kernel.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    21893 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/nuts.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    33005 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/infer/mcmc/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11083 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/predictive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9418 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/renyi_elbo.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.234291 pyro-ppl-1.8.6/pyro/infer/reparam/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4315 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/conjugate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/discrete_cosine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/haar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/hmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3812 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/loc_scale.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/neutra.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/projected_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2627 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/reparam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1869 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/softmax.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2642 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/split.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10231 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/stable.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7481 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/strategies.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4312 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/structured.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1477 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/studentt.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/transform.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3913 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/reparam/unit_jacobian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5720 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/infer/resampler.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11084 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/rws.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8713 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/smcfilter.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12959 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/svgd.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5947 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/svi.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10334 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8302 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/trace_mean_field_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10876 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_mmd.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3367 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/trace_tail_adaptive_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23531 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/traceenum_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16980 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/infer/tracegraph_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8714 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/infer/tracetmc_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12502 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/infer/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      463 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/logger.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.235081 pyro-ppl-1.8.6/pyro/nn/
+-rw-r--r--   0 fritzo     (501) staff       (20)      602 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/auto_reg_nn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5124 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/nn/dense_nn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    31542 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/nn/module.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.243248 pyro-ppl-1.8.6/pyro/ops/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4306 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/arrowhead.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    22550 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/ops/contract.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3402 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/dual_averaging.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.245648 pyro-ppl-1.8.6/pyro/ops/einsum/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4971 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/adjoint.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2010 2022-10-02 18:17:50.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_log.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1952 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_map.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2234 2022-07-05 20:35:43.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_marginal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2736 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/torch_sample.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1901 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/einsum/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    17941 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/gamma_gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    28046 2022-10-30 17:11:32.000000 pyro-ppl-1.8.6/pyro/ops/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/hessian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7458 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/indexing.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5119 2023-01-03 22:31:38.000000 pyro-ppl-1.8.6/pyro/ops/integrator.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5970 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/jit.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/linalg.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9520 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/newton.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6350 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/packed.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5967 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/ops/provenance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11388 2022-07-05 20:10:55.000000 pyro-ppl-1.8.6/pyro/ops/rings.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7050 2022-05-12 17:23:25.000000 pyro-ppl-1.8.6/pyro/ops/special.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6648 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/ssm_gp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    17109 2022-07-10 14:38:43.000000 pyro-ppl-1.8.6/pyro/ops/stats.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8903 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/streaming.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15783 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/ops/tensor_utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3405 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/ops/welford.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.246942 pyro-ppl-1.8.6/pyro/optim/
+-rw-r--r--   0 fritzo     (501) staff       (20)      594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3060 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/adagrad_rmsprop.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3462 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/clipped_adam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7634 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/dct_adam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1906 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/horovod.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2351 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/lr_scheduler.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/optim/multi.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10610 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/optim/optim.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2064 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/optim/pytorch_optimizers.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.247218 pyro-ppl-1.8.6/pyro/params/
+-rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/params/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13144 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/params/param_store.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.251620 pyro-ppl-1.8.6/pyro/poutine/
+-rw-r--r--   0 fritzo     (501) staff       (20)      922 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4794 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/block_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3528 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/broadcast_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6129 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/collapse_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2128 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/condition_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3152 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/do_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9671 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/enum_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1228 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/escape_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5427 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/guide.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8605 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/handlers.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3849 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/indep_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1744 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/infer_config_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4830 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/lift_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3139 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/markov_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/mask_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8689 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/poutine/messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/plate_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/reentrant_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/reparam_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2982 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/replay_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10402 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/runtime.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/scale_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1047 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/seed_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7725 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/subsample_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2935 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/pyro/poutine/substitute_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6891 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/pyro/poutine/trace_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20794 2023-07-24 22:31:37.000000 pyro-ppl-1.8.6/pyro/poutine/trace_struct.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      821 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/poutine/uncondition_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4073 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/poutine/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/primitives.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5019 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/pyro/settings.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    22051 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/pyro/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.252156 pyro-ppl-1.8.6/pyro_ppl.egg-info/
+-rw-r--r--   0 fritzo     (501) staff       (20)     4788 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/PKG-INFO
+-rw-r--r--   0 fritzo     (501) staff       (20)    10720 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/SOURCES.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)        1 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/dependency_links.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)      900 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/requires.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)        5 2023-07-29 21:08:19.000000 pyro-ppl-1.8.6/pyro_ppl.egg-info/top_level.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)     1986 2023-07-29 21:08:19.253974 pyro-ppl-1.8.6/setup.cfg
+-rw-r--r--   0 fritzo     (501) staff       (20)     5096 2023-07-29 21:05:45.000000 pyro-ppl-1.8.6/setup.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-07-29 21:08:19.253150 pyro-ppl-1.8.6/tests/
+-rw-r--r--   0 fritzo     (501) staff       (20)    21987 2023-05-29 03:02:16.000000 pyro-ppl-1.8.6/tests/test_examples.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3354 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_generic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_primitives.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1420 2022-11-06 16:58:27.000000 pyro-ppl-1.8.6/tests/test_settings.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.6/tests/test_util.py
```

### Comparing `pyro-ppl-1.8.5/LICENSE.md` & `pyro-ppl-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/PKG-INFO` & `pyro-ppl-1.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pyro-ppl
-Version: 1.8.5
+Version: 1.8.6
 Summary: A Python library for probabilistic modeling and inference
 Home-page: http://pyro.ai
 Author: Uber AI Labs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.pyro.ai
 Project-URL: Source, https://github.com/pyro-ppl/pyro
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
@@ -116,7 +117,9 @@
   journal   = {J. Mach. Learn. Res.},
   volume    = {20},
   pages     = {28:1--28:6},
   year      = {2019},
   url       = {http://jmlr.org/papers/v20/18-403.html}
 }
 ```
+
+
```

### Comparing `pyro-ppl-1.8.5/README.md` & `pyro-ppl-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/__init__.py` & `pyro-ppl-1.8.6/pyro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     validation_enabled,
 )
 from pyro.util import set_rng_seed
 
 from . import settings
 
 # After changing this, run scripts/update_version.py
-version_prefix = "1.8.5"
+version_prefix = "1.8.6"
 
 # Get the __version__ string from the auto-generated _version.py file, if exists.
 try:
     from pyro._version import __version__  # type: ignore
 except ImportError:
     __version__ = version_prefix
```

### Comparing `pyro-ppl-1.8.5/pyro/contrib/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/autoname/autoname.py` & `pyro-ppl-1.8.6/pyro/contrib/autoname/autoname.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/autoname/named.py` & `pyro-ppl-1.8.6/pyro/contrib/autoname/named.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/autoname/scoping.py` & `pyro-ppl-1.8.6/pyro/contrib/autoname/scoping.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/bnn/hidden_layer.py` & `pyro-ppl-1.8.6/pyro/contrib/bnn/hidden_layer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/cevae/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/cevae/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/conjugate/infer.py` & `pyro-ppl-1.8.6/pyro/contrib/conjugate/infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/easyguide/easyguide.py` & `pyro-ppl-1.8.6/pyro/contrib/easyguide/easyguide.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/epidemiology/compartmental.py` & `pyro-ppl-1.8.6/pyro/contrib/epidemiology/compartmental.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/epidemiology/distributions.py` & `pyro-ppl-1.8.6/pyro/contrib/epidemiology/distributions.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/epidemiology/models.py` & `pyro-ppl-1.8.6/pyro/contrib/epidemiology/models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/epidemiology/util.py` & `pyro-ppl-1.8.6/pyro/contrib/epidemiology/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/bart.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/bart.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/finance.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/finance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/multi_mnist.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/multi_mnist.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/nextstrain.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/nextstrain.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/polyphonic_data_loader.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/polyphonic_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/scanvi_data.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/scanvi_data.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/examples/util.py` & `pyro-ppl-1.8.6/pyro/contrib/examples/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/forecast/evaluate.py` & `pyro-ppl-1.8.6/pyro/contrib/forecast/evaluate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/forecast/forecaster.py` & `pyro-ppl-1.8.6/pyro/contrib/forecast/forecaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
         :returns: Return value is ignored.
         """
         raise NotImplementedError
 
     @property
     def time_plate(self):
         """
+        Helper to create a ``pyro.plate`` over time.
+
         :returns: A plate named "time" with size ``covariates.size(-2)`` and
             ``dim=-1``. This is available only during model execution.
         :rtype: :class:`~pyro.plate`
         """
         assert self._time_plate is not None, ".time_plate accessed outside of .model()"
         return self._time_plate
```

### Comparing `pyro-ppl-1.8.5/pyro/contrib/forecast/util.py` & `pyro-ppl-1.8.6/pyro/contrib/forecast/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 import pyroapi
 
-from pyro.contrib.funsor.handlers import condition, do, markov
+from pyro.contrib.funsor.handlers import condition, do, markov, vectorized_markov
 from pyro.contrib.funsor.handlers import plate as _plate
-from pyro.contrib.funsor.handlers import vectorized_markov
 from pyro.contrib.funsor.handlers.primitives import to_data, to_funsor
 from pyro.primitives import (
     clear_param_store,
     deterministic,
     enable_validation,
     factor,
     get_param_store,
```

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/enum_messenger.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/enum_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/named_messenger.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/named_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/plate_messenger.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/plate_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/primitives.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/primitives.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/replay_messenger.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/replay_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/runtime.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/runtime.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/trace_messenger.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/handlers/trace_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/discrete.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/discrete.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/elbo.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/trace_elbo.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/trace_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/traceenum_elbo.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/traceenum_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/tracetmc_elbo.py` & `pyro-ppl-1.8.6/pyro/contrib/funsor/infer/tracetmc_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/brownian.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/brownian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/coregionalize.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/coregionalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/dot_product.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/dot_product.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/isotropic.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/isotropic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/kernel.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/periodic.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/periodic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/static.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/kernels/static.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/binary.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/binary.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/gaussian.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/likelihood.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/likelihood.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/multi_class.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/multi_class.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/poisson.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/likelihoods/poisson.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/gplvm.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/gplvm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/gpr.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/gpr.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/model.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/model.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/sgpr.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/sgpr.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/vgp.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/vgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/models/vsgp.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/models/vsgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/parameterized.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/parameterized.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/gp/util.py` & `pyro-ppl-1.8.6/pyro/contrib/gp/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/minipyro.py` & `pyro-ppl-1.8.6/pyro/contrib/minipyro.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/mue/dataloaders.py` & `pyro-ppl-1.8.6/pyro/contrib/mue/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/mue/missingdatahmm.py` & `pyro-ppl-1.8.6/pyro/contrib/mue/missingdatahmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/mue/models.py` & `pyro-ppl-1.8.6/pyro/contrib/mue/models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/mue/statearrangers.py` & `pyro-ppl-1.8.6/pyro/contrib/mue/statearrangers.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/eig.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/eig.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/glmm.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/glmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/guides.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/glmm/guides.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/search.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/search.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/oed/util.py` & `pyro-ppl-1.8.6/pyro/contrib/oed/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/randomvariable/random_variable.py` & `pyro-ppl-1.8.6/pyro/contrib/randomvariable/random_variable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/timeseries/__init__.py` & `pyro-ppl-1.8.6/pyro/contrib/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/timeseries/base.py` & `pyro-ppl-1.8.6/pyro/contrib/timeseries/base.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/timeseries/gp.py` & `pyro-ppl-1.8.6/pyro/contrib/timeseries/gp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssm.py` & `pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssmgp.py` & `pyro-ppl-1.8.6/pyro/contrib/timeseries/lgssmgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/assignment.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/assignment.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/distributions.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/distributions.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/dynamic_models.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/extended_kalman_filter.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/hashing.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/hashing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/tracking/measurements.py` & `pyro-ppl-1.8.6/pyro/contrib/tracking/measurements.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/contrib/util.py` & `pyro-ppl-1.8.6/pyro/contrib/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/__init__.py` & `pyro-ppl-1.8.6/pyro/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/affine_beta.py` & `pyro-ppl-1.8.6/pyro/distributions/affine_beta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/asymmetriclaplace.py` & `pyro-ppl-1.8.6/pyro/distributions/asymmetriclaplace.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/avf_mvn.py` & `pyro-ppl-1.8.6/pyro/distributions/avf_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/coalescent.py` & `pyro-ppl-1.8.6/pyro/distributions/coalescent.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/conditional.py` & `pyro-ppl-1.8.6/pyro/distributions/conditional.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/conjugate.py` & `pyro-ppl-1.8.6/pyro/distributions/conjugate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/constraints.py` & `pyro-ppl-1.8.6/pyro/distributions/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from torch.distributions.constraints import *  # noqa F403
 
 # isort: split
 
 import torch
-from torch.distributions.constraints import Constraint
-from torch.distributions.constraints import __all__ as torch_constraints
 from torch.distributions.constraints import (
+    Constraint,
     independent,
     lower_cholesky,
     positive,
     positive_definite,
 )
+from torch.distributions.constraints import __all__ as torch_constraints
 
 
 # TODO move this upstream to torch.distributions
 class _Integer(Constraint):
     """
     Constrain to integers.
     """
```

### Comparing `pyro-ppl-1.8.5/pyro/distributions/delta.py` & `pyro-ppl-1.8.6/pyro/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture.py` & `pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture_shared_cov.py` & `pyro-ppl-1.8.6/pyro/distributions/diag_normal_mixture_shared_cov.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/distribution.py` & `pyro-ppl-1.8.6/pyro/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/empirical.py` & `pyro-ppl-1.8.6/pyro/distributions/empirical.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/extended.py` & `pyro-ppl-1.8.6/pyro/distributions/extended.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/folded.py` & `pyro-ppl-1.8.6/pyro/distributions/folded.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/gaussian_scale_mixture.py` & `pyro-ppl-1.8.6/pyro/distributions/gaussian_scale_mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/grouped_normal_normal.py` & `pyro-ppl-1.8.6/pyro/distributions/grouped_normal_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/hmm.py` & `pyro-ppl-1.8.6/pyro/distributions/hmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/improper_uniform.py` & `pyro-ppl-1.8.6/pyro/distributions/improper_uniform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/inverse_gamma.py` & `pyro-ppl-1.8.6/pyro/distributions/inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/kl.py` & `pyro-ppl-1.8.6/pyro/distributions/kl.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/lkj.py` & `pyro-ppl-1.8.6/pyro/distributions/lkj.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/log_normal_negative_binomial.py` & `pyro-ppl-1.8.6/pyro/distributions/log_normal_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/logistic.py` & `pyro-ppl-1.8.6/pyro/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/mixture.py` & `pyro-ppl-1.8.6/pyro/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/multivariate_studentt.py` & `pyro-ppl-1.8.6/pyro/distributions/multivariate_studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/nanmasked.py` & `pyro-ppl-1.8.6/pyro/distributions/nanmasked.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/omt_mvn.py` & `pyro-ppl-1.8.6/pyro/distributions/omt_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/one_one_matching.py` & `pyro-ppl-1.8.6/pyro/distributions/one_one_matching.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/one_two_matching.py` & `pyro-ppl-1.8.6/pyro/distributions/one_two_matching.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/ordered_logistic.py` & `pyro-ppl-1.8.6/pyro/distributions/ordered_logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/polya_gamma.py` & `pyro-ppl-1.8.6/pyro/distributions/polya_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/projected_normal.py` & `pyro-ppl-1.8.6/pyro/distributions/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/rejector.py` & `pyro-ppl-1.8.6/pyro/distributions/rejector.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/relaxed_straight_through.py` & `pyro-ppl-1.8.6/pyro/distributions/relaxed_straight_through.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/score_parts.py` & `pyro-ppl-1.8.6/pyro/distributions/score_parts.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/sine_bivariate_von_mises.py` & `pyro-ppl-1.8.6/pyro/distributions/sine_bivariate_von_mises.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/sine_skewed.py` & `pyro-ppl-1.8.6/pyro/distributions/sine_skewed.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/softlaplace.py` & `pyro-ppl-1.8.6/pyro/distributions/softlaplace.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/spanning_tree.cpp` & `pyro-ppl-1.8.6/pyro/distributions/spanning_tree.cpp`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/spanning_tree.py` & `pyro-ppl-1.8.6/pyro/distributions/spanning_tree.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/stable.py` & `pyro-ppl-1.8.6/pyro/distributions/stable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/testing/gof.py` & `pyro-ppl-1.8.6/pyro/distributions/testing/gof.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/testing/naive_dirichlet.py` & `pyro-ppl-1.8.6/pyro/distributions/testing/naive_dirichlet.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/testing/rejection_exponential.py` & `pyro-ppl-1.8.6/pyro/distributions/testing/rejection_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/testing/rejection_gamma.py` & `pyro-ppl-1.8.6/pyro/distributions/testing/rejection_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/testing/special.py` & `pyro-ppl-1.8.6/pyro/distributions/testing/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/torch.py` & `pyro-ppl-1.8.6/pyro/distributions/torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import math
+import re
+import textwrap
 
 import torch
 
 from pyro.distributions.torch_distribution import TorchDistributionMixin
 from pyro.distributions.util import broadcast_shape, sum_rightmost
 from pyro.ops.special import log_binomial
 
@@ -330,14 +332,24 @@
         return new
 
     @constraints.dependent_property(is_discrete=False, event_dim=0)
     def support(self):
         return constraints.interval(self._unbroadcasted_low, self._unbroadcasted_high)
 
 
+def _cat_docstrings(*docstrings):
+    result = "\n".join(textwrap.dedent(s.lstrip("\n")) for s in docstrings)
+    result = re.sub("\n\n+", "\n\n", result)
+    # Drop torch-specific lines.
+    result = "".join(
+        line for line in result.splitlines(keepends=True) if "xdoctest" not in line
+    )
+    return result
+
+
 # Programmatically load all distributions from PyTorch.
 __all__ = []
 for _name, _Dist in torch.distributions.__dict__.items():
     if not isinstance(_Dist, type):
         continue
     if not issubclass(_Dist, torch.distributions.Distribution):
         continue
@@ -350,18 +362,19 @@
         _PyroDist = type(_name, (_Dist, TorchDistributionMixin), {})
         _PyroDist.__module__ = __name__
         locals()[_name] = _PyroDist
 
     _PyroDist.__doc__ = """
     Wraps :class:`{}.{}` with
     :class:`~pyro.distributions.torch_distribution.TorchDistributionMixin`.
+
     """.format(
         _Dist.__module__, _Dist.__name__
     )
-
+    _PyroDist.__doc__ = _cat_docstrings(_PyroDist.__doc__, _Dist.__doc__)
     __all__.append(_name)
 
 
 # Create sphinx documentation.
 __doc__ = "\n\n".join(
     [
         """
```

### Comparing `pyro-ppl-1.8.5/pyro/distributions/torch_distribution.py` & `pyro-ppl-1.8.6/pyro/distributions/torch_distribution.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/torch_patch.py` & `pyro-ppl-1.8.6/pyro/distributions/torch_patch.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/torch_transform.py` & `pyro-ppl-1.8.6/pyro/distributions/torch_transform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/__init__.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/affine_autoregressive.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/affine_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/affine_coupling.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/affine_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/basic.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/basic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/batchnorm.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/block_autoregressive.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/block_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/cholesky.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/cholesky.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/discrete_cosine.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/generalized_channel_permute.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/generalized_channel_permute.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/haar.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/householder.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/householder.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/lower_cholesky_affine.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/lower_cholesky_affine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/matrix_exponential.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/matrix_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/neural_autoregressive.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/neural_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/normalize.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/ordered.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/ordered.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/permute.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/permute.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/planar.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/planar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/polynomial.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/polynomial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/power.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/power.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/radial.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/radial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/softplus.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/softplus.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/spline.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/spline.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/spline_autoregressive.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/spline_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/spline_coupling.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/spline_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/sylvester.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/sylvester.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/transforms/unit_cholesky.py` & `pyro-ppl-1.8.6/pyro/distributions/transforms/unit_cholesky.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/unit.py` & `pyro-ppl-1.8.6/pyro/distributions/unit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/util.py` & `pyro-ppl-1.8.6/pyro/distributions/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/von_mises_3d.py` & `pyro-ppl-1.8.6/pyro/distributions/von_mises_3d.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/distributions/zero_inflated.py` & `pyro-ppl-1.8.6/pyro/distributions/zero_inflated.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/__init__.py` & `pyro-ppl-1.8.6/pyro/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/abstract_infer.py` & `pyro-ppl-1.8.6/pyro/infer/abstract_infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/__init__.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/effect.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/effect.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/gaussian.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/guides.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/guides.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,15 +895,18 @@
         """
         Returns a MultivariateNormal posterior distribution.
         """
         scale_tril = self.scale[..., None] * self.scale_tril
         return dist.MultivariateNormal(self.loc, scale_tril=scale_tril)
 
     def _loc_scale(self, *args, **kwargs):
-        return self.loc, self.scale * self.scale_tril.diag()
+        scale_tril = self.scale[..., None] * self.scale_tril
+        scale = scale_tril.pow(2).sum(-1).sqrt()
+        assert scale.shape == self.loc.shape
+        return self.loc, scale
 
 
 class AutoDiagonalNormal(AutoContinuous):
     """
     This implementation of :class:`AutoContinuous` uses a Normal distribution
     with a diagonal covariance matrix to construct a guide over the entire
     latent space. The guide does not depend on the model's ``*args, **kwargs``.
```

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/initialization.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/initialization.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/structured.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/autoguide/utils.py` & `pyro-ppl-1.8.6/pyro/infer/autoguide/utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/csis.py` & `pyro-ppl-1.8.6/pyro/infer/csis.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/discrete.py` & `pyro-ppl-1.8.6/pyro/infer/discrete.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/elbo.py` & `pyro-ppl-1.8.6/pyro/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/energy_distance.py` & `pyro-ppl-1.8.6/pyro/infer/energy_distance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/enum.py` & `pyro-ppl-1.8.6/pyro/infer/enum.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/importance.py` & `pyro-ppl-1.8.6/pyro/infer/importance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/inspect.py` & `pyro-ppl-1.8.6/pyro/infer/inspect.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/adaptation.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/api.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/api.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/hmc.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/logger.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/logger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/mcmc_kernel.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/mcmc_kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/nuts.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/mcmc/util.py` & `pyro-ppl-1.8.6/pyro/infer/mcmc/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/predictive.py` & `pyro-ppl-1.8.6/pyro/infer/predictive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/renyi_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/renyi_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/__init__.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/conjugate.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/conjugate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/discrete_cosine.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/haar.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/hmm.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/hmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/loc_scale.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/loc_scale.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/neutra.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/neutra.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/projected_normal.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/reparam.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/reparam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/softmax.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/softmax.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/split.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/split.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/stable.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/stable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/strategies.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/strategies.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/structured.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/studentt.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/transform.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/transform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/reparam/unit_jacobian.py` & `pyro-ppl-1.8.6/pyro/infer/reparam/unit_jacobian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/resampler.py` & `pyro-ppl-1.8.6/pyro/infer/resampler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/rws.py` & `pyro-ppl-1.8.6/pyro/infer/rws.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/smcfilter.py` & `pyro-ppl-1.8.6/pyro/infer/smcfilter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/svgd.py` & `pyro-ppl-1.8.6/pyro/infer/svgd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/svi.py` & `pyro-ppl-1.8.6/pyro/infer/svi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/trace_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/trace_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/trace_mean_field_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/trace_mean_field_elbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,18 @@
                     # use kl divergence if available, else fall back on sampling
                     try:
                         kl_qp = kl_divergence(guide_site["fn"], model_site["fn"])
                         kl_qp = scale_and_mask(
                             kl_qp, scale=guide_site["scale"], mask=guide_site["mask"]
                         )
                         if torch.is_tensor(kl_qp):
-                            assert kl_qp.shape == guide_site["fn"].batch_shape
+                            assert (
+                                torch._C._get_tracing_state()
+                                or kl_qp.shape == guide_site["fn"].batch_shape
+                            )
                             kl_qp_sum = kl_qp.sum()
                         else:
                             kl_qp_sum = (
                                 kl_qp * torch.Size(guide_site["fn"].batch_shape).numel()
                             )
                         elbo_particle = elbo_particle - kl_qp_sum
                     except NotImplementedError:
```

### Comparing `pyro-ppl-1.8.5/pyro/infer/trace_mmd.py` & `pyro-ppl-1.8.6/pyro/infer/trace_mmd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/trace_tail_adaptive_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/trace_tail_adaptive_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/traceenum_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/traceenum_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/tracegraph_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/tracegraph_elbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,16 +408,16 @@
                 kwargs.pop("_pyro_model_id")
                 kwargs.pop("_pyro_guide_id")
                 self = weakself()
                 return self._loss_and_surrogate_loss(model, guide, args, kwargs)
 
             self._jit_loss_and_surrogate_loss = jit_loss_and_surrogate_loss
 
-        loss, surrogate_loss = self._jit_loss_and_surrogate_loss(*args, **kwargs)
+        elbo, surrogate_loss = self._jit_loss_and_surrogate_loss(*args, **kwargs)
 
         surrogate_loss.backward(
             retain_graph=self.retain_graph
         )  # triggers jit compilation
 
-        loss = loss.item()
+        loss = -elbo.item()
         warn_if_nan(loss, "loss")
         return loss
```

### Comparing `pyro-ppl-1.8.5/pyro/infer/tracetmc_elbo.py` & `pyro-ppl-1.8.6/pyro/infer/tracetmc_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/infer/util.py` & `pyro-ppl-1.8.6/pyro/infer/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/nn/__init__.py` & `pyro-ppl-1.8.6/pyro/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/nn/auto_reg_nn.py` & `pyro-ppl-1.8.6/pyro/nn/auto_reg_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/nn/dense_nn.py` & `pyro-ppl-1.8.6/pyro/nn/dense_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/nn/module.py` & `pyro-ppl-1.8.6/pyro/nn/module.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/arrowhead.py` & `pyro-ppl-1.8.6/pyro/ops/arrowhead.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/contract.py` & `pyro-ppl-1.8.6/pyro/ops/contract.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/dual_averaging.py` & `pyro-ppl-1.8.6/pyro/ops/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/__init__.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/adjoint.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/adjoint.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/torch_log.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/torch_log.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/torch_map.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/torch_map.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/torch_marginal.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/torch_marginal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/torch_sample.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/torch_sample.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/einsum/util.py` & `pyro-ppl-1.8.6/pyro/ops/einsum/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/gamma_gaussian.py` & `pyro-ppl-1.8.6/pyro/ops/gamma_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/gaussian.py` & `pyro-ppl-1.8.6/pyro/ops/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/hessian.py` & `pyro-ppl-1.8.6/pyro/ops/hessian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/indexing.py` & `pyro-ppl-1.8.6/pyro/ops/indexing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/integrator.py` & `pyro-ppl-1.8.6/pyro/ops/integrator.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/jit.py` & `pyro-ppl-1.8.6/pyro/ops/jit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/linalg.py` & `pyro-ppl-1.8.6/pyro/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/newton.py` & `pyro-ppl-1.8.6/pyro/ops/newton.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/packed.py` & `pyro-ppl-1.8.6/pyro/ops/packed.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/provenance.py` & `pyro-ppl-1.8.6/pyro/ops/provenance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
-from functools import singledispatch
+from functools import partial, singledispatch
 from typing import Tuple
 
 import torch
+from torch.utils._pytree import tree_flatten, tree_map, tree_unflatten
 
 
 class ProvenanceTensor(torch.Tensor):
     """
     Provenance tracking implementation in Pytorch.
 
     This class wraps a :class:`torch.Tensor` to track provenance through
@@ -38,52 +39,37 @@
         Nonstandard Interpretations of Probabilistic Programs for Efficient Inference
         http://papers.neurips.cc/paper/4309-nonstandard-interpretations-of-probabilistic-programs-for-efficient-inference.pdf
 
     :param torch.Tensor data: An initial tensor to start tracking.
     :param frozenset provenance: An initial provenance set.
     """
 
+    _t: torch.Tensor
+    _provenance: frozenset
+
     def __new__(cls, data: torch.Tensor, provenance=frozenset(), **kwargs):
         assert not isinstance(data, ProvenanceTensor)
         if not provenance:
             return data
         ret = data.as_subclass(cls)
         ret._t = data  # this makes sure that detach_provenance always
         # returns the same object. This is important when
         # using the tensor as key in a dict, e.g. the global
         # param store
+        ret._provenance = provenance
         return ret
 
-    def __init__(self, data, provenance=frozenset()):
-        assert isinstance(provenance, frozenset)
-        self._provenance = provenance
-
     def __repr__(self):
         return "Provenance:\n{}\nTensor:\n{}".format(self._provenance, self._t)
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
-        if kwargs is None:
-            kwargs = {}
-        # collect provenance information from args
-        provenance = frozenset()
-        # extract ProvenanceTensor._t data from args and kwargs
-        _args = []
-        for arg in args:
-            _arg, _provenance = extract_provenance(arg)
-            _args.append(_arg)
-            provenance |= _provenance
-        _kwargs = {}
-        for k, v in kwargs.items():
-            _v, _provenance = extract_provenance(v)
-            _kwargs[k] = _v
-            provenance |= provenance
+        _args, _kwargs = detach_provenance([args, kwargs or {}])
         ret = func(*_args, **_kwargs)
-        _ret = track_provenance(ret, provenance)
-        return _ret
+        return track_provenance(ret, get_provenance([args, kwargs]))
 
 
 @singledispatch
 def track_provenance(x, provenance: frozenset):
     """
     Adds provenance info to the :class:`torch.Tensor` leaves of a data structure.
 
@@ -94,21 +80,31 @@
     return x
 
 
 track_provenance.register(torch.Tensor)(ProvenanceTensor)
 
 
 @track_provenance.register(frozenset)
-@track_provenance.register(list)
 @track_provenance.register(set)
-@track_provenance.register(tuple)
-def _track_provenance_list(x, provenance: frozenset):
+def _track_provenance_set(x, provenance: frozenset):
     return type(x)(track_provenance(part, provenance) for part in x)
 
 
+@track_provenance.register(list)
+@track_provenance.register(tuple)
+@track_provenance.register(dict)
+def _track_provenance_pytree(x, provenance: frozenset):
+    # avoid max-recursion depth error for torch<=2.0
+    flat_args, _ = tree_flatten(x)
+    if not flat_args or flat_args[0] is x:
+        return x
+
+    return tree_map(partial(track_provenance, provenance=provenance), x)
+
+
 @track_provenance.register
 def _track_provenance_provenancetensor(x: ProvenanceTensor, provenance: frozenset):
     x_value, old_provenance = extract_provenance(x)
     return track_provenance(x_value, old_provenance | provenance)
 
 
 @singledispatch
@@ -127,28 +123,44 @@
 
 @extract_provenance.register(ProvenanceTensor)
 def _extract_provenance_tensor(x):
     return x._t, x._provenance
 
 
 @extract_provenance.register(frozenset)
-@extract_provenance.register(list)
 @extract_provenance.register(set)
-@extract_provenance.register(tuple)
-def _extract_provenance_list(x):
+def _extract_provenance_set(x):
     provenance = frozenset()
     values = []
     for part in x:
         v, p = extract_provenance(part)
         values.append(v)
         provenance |= p
     value = type(x)(values)
     return value, provenance
 
 
+@extract_provenance.register(list)
+@extract_provenance.register(tuple)
+@extract_provenance.register(dict)
+def _extract_provenance_pytree(x):
+    # avoid max-recursion depth error for torch<=2.0
+    flat_args, _ = tree_flatten(x)
+    if not flat_args or flat_args[0] is x:
+        return x, frozenset()
+
+    flat_args, spec = tree_flatten(x)
+    xs = []
+    provenance = frozenset()
+    for x, p in map(extract_provenance, flat_args):
+        xs.append(x)
+        provenance |= p
+    return tree_unflatten(xs, spec), provenance
+
+
 def get_provenance(x) -> frozenset:
     """
     Reads the provenance of a recursive datastructure possibly containing
     :class:`torch.Tensor` s.
 
     :param torch.Tensor tensor: An input tensor.
     :returns: A provenance frozenset.
```

### Comparing `pyro-ppl-1.8.5/pyro/ops/rings.py` & `pyro-ppl-1.8.6/pyro/ops/rings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/special.py` & `pyro-ppl-1.8.6/pyro/ops/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/ssm_gp.py` & `pyro-ppl-1.8.6/pyro/ops/ssm_gp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/stats.py` & `pyro-ppl-1.8.6/pyro/ops/stats.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/streaming.py` & `pyro-ppl-1.8.6/pyro/ops/streaming.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/tensor_utils.py` & `pyro-ppl-1.8.6/pyro/ops/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/ops/welford.py` & `pyro-ppl-1.8.6/pyro/ops/welford.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/__init__.py` & `pyro-ppl-1.8.6/pyro/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/adagrad_rmsprop.py` & `pyro-ppl-1.8.6/pyro/optim/adagrad_rmsprop.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/clipped_adam.py` & `pyro-ppl-1.8.6/pyro/optim/clipped_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/dct_adam.py` & `pyro-ppl-1.8.6/pyro/optim/dct_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/horovod.py` & `pyro-ppl-1.8.6/pyro/optim/horovod.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/lr_scheduler.py` & `pyro-ppl-1.8.6/pyro/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/multi.py` & `pyro-ppl-1.8.6/pyro/optim/multi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/optim.py` & `pyro-ppl-1.8.6/pyro/optim/optim.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/optim/pytorch_optimizers.py` & `pyro-ppl-1.8.6/pyro/optim/pytorch_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/params/param_store.py` & `pyro-ppl-1.8.6/pyro/params/param_store.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/__init__.py` & `pyro-ppl-1.8.6/pyro/poutine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/block_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/block_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/broadcast_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/broadcast_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/collapse_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/collapse_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/condition_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/condition_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/do_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/do_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/enum_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/enum_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/escape_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/escape_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/guide.py` & `pyro-ppl-1.8.6/pyro/poutine/guide.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/handlers.py` & `pyro-ppl-1.8.6/pyro/poutine/handlers.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/indep_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/indep_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/infer_config_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/infer_config_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/lift_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/lift_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/markov_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/markov_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/mask_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/mask_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         Can be overloaded to add any additional per-call setup functionality,
         but the derived class must always push itself onto the stack, usually
         by calling super().__enter__().
 
         Derived versions cannot be overridden to take arguments
         and must always return self.
         """
-        if not (self in _PYRO_STACK):
+        if self not in _PYRO_STACK:
             # if this poutine is not already installed,
             # put it on the bottom of the stack.
             _PYRO_STACK.append(self)
 
             # necessary to return self because the return value of __enter__
             # is bound to VAR in with EXPR as VAR.
             return self
```

### Comparing `pyro-ppl-1.8.5/pyro/poutine/plate_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/plate_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/reentrant_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/reentrant_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/reparam_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/reparam_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/replay_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/replay_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/runtime.py` & `pyro-ppl-1.8.6/pyro/poutine/runtime.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/scale_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/scale_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/seed_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/seed_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/subsample_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/subsample_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/substitute_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/substitute_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/trace_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/trace_messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     `cond_indep_stack` information stored at each site.
     """
     for name, node in trace.nodes.items():
         if site_is_subsample(node):
             continue
         if node["type"] == "sample":
             for past_name, past_node in trace.nodes.items():
-                if site_is_subsample(node):
+                if site_is_subsample(past_node):
                     continue
                 if past_node["type"] == "sample":
                     if past_name == name:
                         break
                     past_node_independent = False
                     for query, target in zip(
                         node["cond_indep_stack"], past_node["cond_indep_stack"]
```

### Comparing `pyro-ppl-1.8.5/pyro/poutine/trace_struct.py` & `pyro-ppl-1.8.6/pyro/poutine/trace_struct.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/uncondition_messenger.py` & `pyro-ppl-1.8.6/pyro/poutine/uncondition_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/poutine/util.py` & `pyro-ppl-1.8.6/pyro/poutine/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/primitives.py` & `pyro-ppl-1.8.6/pyro/primitives.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/settings.py` & `pyro-ppl-1.8.6/pyro/settings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro/util.py` & `pyro-ppl-1.8.6/pyro/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/pyro_ppl.egg-info/PKG-INFO` & `pyro-ppl-1.8.6/pyro_ppl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pyro-ppl
-Version: 1.8.5
+Version: 1.8.6
 Summary: A Python library for probabilistic modeling and inference
 Home-page: http://pyro.ai
 Author: Uber AI Labs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.pyro.ai
 Project-URL: Source, https://github.com/pyro-ppl/pyro
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
@@ -116,7 +117,9 @@
   journal   = {J. Mach. Learn. Res.},
   volume    = {20},
   pages     = {28:1--28:6},
   year      = {2019},
   url       = {http://jmlr.org/papers/v20/18-403.html}
 }
 ```
+
+
```

### Comparing `pyro-ppl-1.8.5/pyro_ppl.egg-info/SOURCES.txt` & `pyro-ppl-1.8.6/pyro_ppl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 pyro/__init__.py
 pyro/_version.py
 pyro/generic.py
 pyro/logger.py
 pyro/primitives.py
@@ -321,8 +322,13 @@
 pyro/poutine/trace_struct.py
 pyro/poutine/uncondition_messenger.py
 pyro/poutine/util.py
 pyro_ppl.egg-info/PKG-INFO
 pyro_ppl.egg-info/SOURCES.txt
 pyro_ppl.egg-info/dependency_links.txt
 pyro_ppl.egg-info/requires.txt
-pyro_ppl.egg-info/top_level.txt
+pyro_ppl.egg-info/top_level.txt
+tests/test_examples.py
+tests/test_generic.py
+tests/test_primitives.py
+tests/test_settings.py
+tests/test_util.py
```

### Comparing `pyro-ppl-1.8.5/pyro_ppl.egg-info/requires.txt` & `pyro-ppl-1.8.6/pyro_ppl.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 numpy>=1.7
 opt_einsum>=2.3.2
 pyro-api>=0.1.1
-torch>=2.0.1
+torch>=1.11.0
 tqdm>=4.36
 
 [dev]
 jupyter>=1.0.0
 graphviz>=0.8
 matplotlib>=1.3
 torchvision>=0.12.0
@@ -13,25 +13,24 @@
 pandas
 pillow==8.2.0
 scikit-learn
 seaborn>=0.11.0
 wget
 lap
 black>=21.4b0
-flake8
-isort>=5.0
 mypy>=0.812
 nbformat
 nbsphinx>=0.3.2
 nbstripout
 nbval
 ninja
 pypandoc
-pytest>=5.0
 pytest-xdist
+pytest>=5.0
+ruff
 scipy>=1.1
 sphinx
 sphinx_rtd_theme
 yapf
 
 [extras]
 jupyter>=1.0.0
@@ -69,12 +68,13 @@
 pandas
 pillow==8.2.0
 scikit-learn
 seaborn>=0.11.0
 wget
 lap
 black>=21.4b0
-flake8
 nbval
-pytest>=5.0
 pytest-cov
+pytest-xdist
+pytest>=5.0
+ruff
 scipy>=1.1
```

### Comparing `pyro-ppl-1.8.5/setup.cfg` & `pyro-ppl-1.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.5/setup.py` & `pyro-ppl-1.8.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,43 +98,43 @@
     install_requires=[
         # if you add any additional libraries, please also
         # add them to `docs/requirements.txt`
         # numpy is necessary for some functionality of PyTorch
         "numpy>=1.7",
         "opt_einsum>=2.3.2",
         "pyro-api>=0.1.1",
-        "torch>=2.0.1",
+        "torch>=1.11.0",
         "tqdm>=4.36",
     ],
     extras_require={
         "extras": EXTRAS_REQUIRE,
         "test": EXTRAS_REQUIRE
         + [
             "black>=21.4b0",
-            "flake8",
             "nbval",
-            "pytest>=5.0",
             "pytest-cov",
+            "pytest-xdist",
+            "pytest>=5.0",
+            "ruff",
             "scipy>=1.1",
         ],
         "profile": ["prettytable", "pytest-benchmark", "snakeviz"],
         "dev": EXTRAS_REQUIRE
         + [
             "black>=21.4b0",
-            "flake8",
-            "isort>=5.0",
             "mypy>=0.812",
             "nbformat",
             "nbsphinx>=0.3.2",
             "nbstripout",
             "nbval",
             "ninja",
             "pypandoc",
-            "pytest>=5.0",
             "pytest-xdist",
+            "pytest>=5.0",
+            "ruff",
             "scipy>=1.1",
             "sphinx",
             "sphinx_rtd_theme",
             "yapf",
         ],
         "horovod": ["horovod[pytorch]>=0.19"],
         "lightning": ["pytorch_lightning"],
```

