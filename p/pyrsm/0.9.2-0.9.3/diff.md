# Comparing `tmp/pyrsm-0.9.2.tar.gz` & `tmp/pyrsm-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.9.2.tar", last modified: Sat Jul 29 07:43:51 2023, max compression
+gzip compressed data, was "pyrsm-0.9.3.tar", last modified: Sat Jul 29 08:04:03 2023, max compression
```

## Comparing `pyrsm-0.9.2.tar` & `pyrsm-0.9.3.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.272814 pyrsm-0.9.2/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 07:43:51.272941 pyrsm-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.2/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.2/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.255629 pyrsm-0.9.2/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-29 07:43:18.000000 pyrsm-0.9.2/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.257794 pyrsm-0.9.2/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.2/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.2/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8847 2023-07-22 13:22:08.000000 pyrsm-0.9.2/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.2/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.2/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9645 2023-07-22 13:13:41.000000 pyrsm-0.9.2/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6717 2023-07-22 14:39:10.000000 pyrsm-0.9.2/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.2/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.2/pyrsm/basics/probability_calculator_functions.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.2/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.2/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.2/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2847 2023-07-23 22:04:07.000000 pyrsm-0.9.2/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.258007 pyrsm-0.9.2/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      820 2023-07-28 07:03:06.000000 pyrsm-0.9.2/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.259056 pyrsm-0.9.2/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.260833 pyrsm-0.9.2/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.261322 pyrsm-0.9.2/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.264497 pyrsm-0.9.2/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.2/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.2/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ratings_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.2/pyrsm/data/model/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.2/pyrsm/data/model/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.267186 pyrsm-0.9.2/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3910 2023-07-24 08:59:20.000000 pyrsm-0.9.2/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9490 2023-07-23 22:05:12.000000 pyrsm-0.9.2/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.2/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.2/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.2/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.268485 pyrsm-0.9.2/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      216 2023-07-22 06:25:56.000000 pyrsm-0.9.2/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10069 2023-07-27 07:43:27.000000 pyrsm-0.9.2/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5625 2023-07-27 07:41:53.000000 pyrsm-0.9.2/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     4453 2023-07-27 07:43:46.000000 pyrsm-0.9.2/pyrsm/radiant/data_view.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-07-27 07:41:42.000000 pyrsm-0.9.2/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5991 2023-07-27 07:41:30.000000 pyrsm-0.9.2/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    11263 2023-07-26 16:45:47.000000 pyrsm-0.9.2/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)    11466 2023-07-27 07:42:33.000000 pyrsm-0.9.2/pyrsm/radiant/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     5502 2023-07-27 07:41:06.000000 pyrsm-0.9.2/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     6241 2023-07-27 07:52:22.000000 pyrsm-0.9.2/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    19793 2023-07-27 08:32:29.000000 pyrsm-0.9.2/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.269030 pyrsm-0.9.2/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.2/pyrsm/radiant/www/.DS_Store
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.270320 pyrsm-0.9.2/pyrsm/radiant/www/imgs/
--rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-nc-sa.png
--rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-sa.png
--rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/icon.png
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.271525 pyrsm-0.9.2/pyrsm/radiant/www/js/
--rw-r--r--   0 root         (0) staff       (20)      513 2023-07-23 21:45:57.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/radiantUI.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/screenshot.js
--rw-r--r--   0 root         (0) staff       (20)      829 2023-07-20 17:40:43.000000 pyrsm-0.9.2/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9495 2023-07-24 19:44:21.000000 pyrsm-0.9.2/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.2/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.2/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.2/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.256256 pyrsm-0.9.2/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4049 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      273 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1088 2023-07-29 07:43:51.273297 pyrsm-0.9.2/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.272688 pyrsm-0.9.2/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.2/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.2/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.2/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.2/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.2/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.2/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.984174 pyrsm-0.9.3/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 08:04:03.984293 pyrsm-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.3/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.3/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.947057 pyrsm-0.9.3/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-29 08:03:22.000000 pyrsm-0.9.3/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.955214 pyrsm-0.9.3/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.3/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.3/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8847 2023-07-22 13:22:08.000000 pyrsm-0.9.3/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.3/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.3/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9645 2023-07-22 13:13:41.000000 pyrsm-0.9.3/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6717 2023-07-22 14:39:10.000000 pyrsm-0.9.3/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.3/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.3/pyrsm/basics/probability_calculator_functions.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.3/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.3/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.3/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2847 2023-07-23 22:04:07.000000 pyrsm-0.9.3/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.955576 pyrsm-0.9.3/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      820 2023-07-28 07:03:06.000000 pyrsm-0.9.3/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.957672 pyrsm-0.9.3/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.961389 pyrsm-0.9.3/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.962392 pyrsm-0.9.3/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.968535 pyrsm-0.9.3/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.3/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.3/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-28 07:02:54.000000 pyrsm-0.9.3/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/model/ratings_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.3/pyrsm/data/model/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.3/pyrsm/data/model/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.974094 pyrsm-0.9.3/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-28 07:02:53.000000 pyrsm-0.9.3/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3910 2023-07-24 08:59:20.000000 pyrsm-0.9.3/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9490 2023-07-23 22:05:12.000000 pyrsm-0.9.3/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.3/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.3/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.3/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.3/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.978581 pyrsm-0.9.3/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      216 2023-07-22 06:25:56.000000 pyrsm-0.9.3/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10483 2023-07-29 08:01:51.000000 pyrsm-0.9.3/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     6039 2023-07-29 08:00:55.000000 pyrsm-0.9.3/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     4460 2023-07-29 07:59:38.000000 pyrsm-0.9.3/pyrsm/radiant/data_view.py
+-rw-r--r--   0 root         (0) staff       (20)     5825 2023-07-29 07:58:15.000000 pyrsm-0.9.3/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5972 2023-07-29 07:57:12.000000 pyrsm-0.9.3/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11263 2023-07-26 16:45:47.000000 pyrsm-0.9.3/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)    11880 2023-07-29 07:55:50.000000 pyrsm-0.9.3/pyrsm/radiant/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     5483 2023-07-29 07:55:10.000000 pyrsm-0.9.3/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     6222 2023-07-29 07:56:27.000000 pyrsm-0.9.3/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    19793 2023-07-27 08:32:29.000000 pyrsm-0.9.3/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.979487 pyrsm-0.9.3/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.3/pyrsm/radiant/www/.DS_Store
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.980412 pyrsm-0.9.3/pyrsm/radiant/www/imgs/
+-rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.3/pyrsm/radiant/www/imgs/by-nc-sa.png
+-rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.3/pyrsm/radiant/www/imgs/by-sa.png
+-rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.3/pyrsm/radiant/www/imgs/icon.png
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.981308 pyrsm-0.9.3/pyrsm/radiant/www/js/
+-rw-r--r--   0 root         (0) staff       (20)      513 2023-07-23 21:45:57.000000 pyrsm-0.9.3/pyrsm/radiant/www/js/radiantUI.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.3/pyrsm/radiant/www/js/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.3/pyrsm/radiant/www/js/screenshot.js
+-rw-r--r--   0 root         (0) staff       (20)      829 2023-07-20 17:40:43.000000 pyrsm-0.9.3/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9495 2023-07-24 19:44:21.000000 pyrsm-0.9.3/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.3/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.3/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.3/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.948212 pyrsm-0.9.3/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 08:04:03.000000 pyrsm-0.9.3/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4049 2023-07-29 08:04:03.000000 pyrsm-0.9.3/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-29 08:04:03.000000 pyrsm-0.9.3/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      273 2023-07-29 08:04:03.000000 pyrsm-0.9.3/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-29 08:04:03.000000 pyrsm-0.9.3/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1088 2023-07-29 08:04:03.984702 pyrsm-0.9.3/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 08:04:03.983685 pyrsm-0.9.3/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.3/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.3/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.3/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.3/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.3/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.3/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.3/tests/test_utils.py
```

### Comparing `pyrsm-0.9.2/LICENSE` & `pyrsm-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/MANIFEST.in` & `pyrsm-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/PKG-INFO` & `pyrsm-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.2/README.md` & `pyrsm-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.9.3/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/compare_means.py` & `pyrsm-0.9.3/pyrsm/basics/compare_means.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/compare_props.py` & `pyrsm-0.9.3/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/correlation.py` & `pyrsm-0.9.3/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/cross_tabs.py` & `pyrsm-0.9.3/pyrsm/basics/cross_tabs.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/goodness.py` & `pyrsm-0.9.3/pyrsm/basics/goodness.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/probability_calculator.py` & `pyrsm-0.9.3/pyrsm/basics/probability_calculator.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/probability_calculator_functions.py` & `pyrsm-0.9.3/pyrsm/basics/probability_calculator_functions.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/single_mean.py` & `pyrsm-0.9.3/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/basics/single_prop.py` & `pyrsm-0.9.3/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/bins.py` & `pyrsm-0.9.3/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.9.3/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/consider.parquet` & `pyrsm-0.9.3/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/consider_description.md` & `pyrsm-0.9.3/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.9.3/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.9.3/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.9.3/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/salary.parquet` & `pyrsm-0.9.3/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/basics/salary_description.md` & `pyrsm-0.9.3/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/avengers.parquet` & `pyrsm-0.9.3/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.9.3/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.9.3/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/publishers.parquet` & `pyrsm-0.9.3/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.9.3/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/titanic.parquet` & `pyrsm-0.9.3/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/data/titanic_description.md` & `pyrsm-0.9.3/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.9.3/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/catalog.parquet` & `pyrsm-0.9.3/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/catalog_description.md` & `pyrsm-0.9.3/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.9.3/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.9.3/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.9.3/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.9.3/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/dvd.parquet` & `pyrsm-0.9.3/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/dvd_description.md` & `pyrsm-0.9.3/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.9.3/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.9.3/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.9.3/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/ideal.parquet` & `pyrsm-0.9.3/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.9.3/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.9.3/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/ratings.parquet` & `pyrsm-0.9.3/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/titanic.parquet` & `pyrsm-0.9.3/pyrsm/data/model/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/model/titanic_description.md` & `pyrsm-0.9.3/pyrsm/data/model/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.9.3/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.9.3/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/example_data.py` & `pyrsm-0.9.3/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/logistic.py` & `pyrsm-0.9.3/pyrsm/logistic.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/model.py` & `pyrsm-0.9.3/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/notebook.py` & `pyrsm-0.9.3/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/perf.py` & `pyrsm-0.9.3/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/props.py` & `pyrsm-0.9.3/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/compare_means.py` & `pyrsm-0.9.3/pyrsm/radiant/compare_means.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
+from pathlib import Path
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
 import webbrowser
 import nest_asyncio
 import uvicorn
 import signal
 import os
 import sys
@@ -318,16 +322,25 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
+    app = App(rc.shiny_ui(), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
+
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.9.3/pyrsm/radiant/cross_tabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
+from pathlib import Path
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser
 import nest_asyncio
 import uvicorn
 import signal
 import os
 import sys
@@ -186,16 +190,25 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
+    app = App(rc.shiny_ui(), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
+
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/data_view.py` & `pyrsm-0.9.3/pyrsm/radiant/data_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 # individual user on a server
 # https://discord.com/channels/1109483223987277844/1129448698611511326/1129732244353851432
 
 
 class data_view:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
-        self.state = {"data_filter": "price > 1000", "datasets": "diamonds"}
+        # self.state = {"data_filter": "price > 1000", "datasets": "diamonds"}
+        self.state = {}
 
     def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
                 "<< Data > View >>",
                 ui.row(
@@ -103,15 +104,15 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
-    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    app = App(rc.shiny_ui(), rc.shiny_server)
     www_dir = Path(__file__).parent.parent / "radiant" / "www"
     app_static = StaticFiles(directory=www_dir, html=False)
 
     routes = [
         Mount("/www", app=app_static),
         Mount("/", app=app),
     ]
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/goodness.py` & `pyrsm-0.9.3/pyrsm/radiant/regress.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,197 +1,199 @@
-from shiny import App, render, ui, reactive, Inputs, Outputs, Session
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
+from shiny import App, ui, reactive, Inputs, Outputs, Session
+from pathlib import Path
 import webbrowser
 import nest_asyncio
 import uvicorn
-import signal
 import os
+import signal
 import sys
 import tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
-    "observed": "Observed",
-    "expected": "Expected",
-    "chisq": "Chi-squared",
-    "dev_std": "Deviation std.",
+    "None": "None",
+    "dist": "Distribution",
+    "corr": "Correlation",
+    "scatter": "Scatter",
+    "dashboard": "Dashboard",
+    "residual": "Residual vs Explanatory",
+    "pred": "Prediction plots",
+    "vimp": "Permutation importance",
+    "coef": "Coefficient plot",
 }
 
+controls = {
+    "ci": "Confidence intervals",
+    "ssq": "Sum of Squares",
+    "vif": "VIF",
+}
 
-def ui_summary():
-    return ui.panel_conditional(
-        "input.tabs == 'Summary'",
-        ui.panel_well(
-            ui.output_ui("ui_var"),
-            ru.input_return_text_area(
-                "probs",
-                label="Probabilities:",
-                placeholder="Insert list [1/2, 1/2]",
-                value=None,
-            ),
-            ui.input_checkbox_group(
-                id="output",
-                label="Select output tables:",
-                choices=choices,
-            ),
+summary_extra = (
+    ui.input_radio_buttons(
+        "show_interactions",
+        "Interactions:",
+        choices={0: "None", 2: "2-way", 3: "3-way"},
+        inline=True,
+    ),
+    ui.panel_conditional(
+        "input.show_interactions > 0",
+        ui.output_ui("ui_interactions"),
+    ),
+    ui.input_checkbox_group(
+        "controls",
+        "Additional output:",
+        choices=controls,
+    ),
+    ui.output_ui("ui_evar_test"),
+)
+
+plots_extra = (
+    ui.panel_conditional(
+        "input.plots == 'corr'",
+        ui.input_select(
+            "nobs",
+            "Number of data points plotted:",
+            {1000: "1,000", -1: "All"},
         ),
-    )
+    ),
+    ui.panel_conditional(
+        "input.plots == 'pred'",
+        ui.output_ui("ui_incl_evar"),
+        ui.output_ui("ui_incl_interactions"),
+    ),
+)
 
 
-plots = {"None": "None"}
-plots.update(choices)
-
-
-class basics_goodness:
+class model_regress:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "<< Basics > Goodness-of-fit >>",
+                "<< Model > Linear regression (OLS) >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
-                        ui_summary(),
-                        ru.ui_plot(plots),
+                        ru.ui_summary(summary_extra),
+                        mu.ui_predict(self),
+                        ru.ui_plot(choices, plots_extra),
                     ),
-                    ui.column(8, ru.ui_main_basics()),
+                    ui.column(8, ru.ui_main_model()),
                 ),
             ),
             *args,
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-goodness.ipynb",
-                "Goodness-of-fit example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/model-linear-regression.ipynb",
+                "Linear regression (OLS) example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
         get_data = ru.make_data_elements(self, input, output, session)
 
-        # --- section unique to each app ---
-        @output(id="ui_var")
-        @render.ui
-        def ui_var1():
-            isCat = get_data()["var_types"]["isCat"]
-            return ui.input_select(
-                id="var",
-                label="Select a categorical variable:",
-                selected=None,
-                choices=isCat,
-            )
-
-        def estimation_code():
-            data_name, code = (get_data()[k] for k in ["data_name", "code"])
-
-            if ru.is_empty(input.probs()):
-                probs = None
-            else:
-                probs = input.probs()
-
-            args = {
-                "data": f"""{{"{data_name}": {data_name}}}""",
-                "var": input.var(),
-                "probs": probs,
-            }
-
-            args_string = ru.drop_default_args(
-                args, rsm.basics.goodness, ignore=["data", "probs"]
-            )
-            return f"""rsm.basics.goodness({args_string})""", code
+        # --- section standard for all model apps ---
+        ru.reestimate(input)
 
+        # --- section unique to each app ---
+        mu.make_model_inputs(input, output, get_data, "isNum")
+        mu.make_int_inputs(input, output, get_data)
         show_code, estimate = mu.make_estimate(
+            self, input, output, get_data, fun="regress", ret="reg", debug=False
+        )
+        mu.make_summary(
             self,
             input,
             output,
-            get_data,
-            fun="basics.goodness",
-            ret="gf",
-            ec=estimation_code,
-            run=False,
-            debug=True,
+            session,
+            show_code,
+            estimate,
+            ret="reg",
+            sum_fun=rsm.regress.summary,
         )
-
-        def summary_code():
-            args = [c for c in input.output()]
-            return f"""gf.summary(output={args})"""
-
-        mu.make_summary(
+        mu.make_predict(
             self,
             input,
             output,
             session,
             show_code,
             estimate,
-            ret="gf",
-            sum_fun=rsm.basics.goodness.summary,
-            sc=summary_code,
+            ret="reg",
+            pred_fun=rsm.regress.predict,
         )
-
-        def plot_code():
-            return f"""gf.plot(plots="{input.plots()}")"""
-
         mu.make_plot(
             self,
             input,
             output,
             session,
             show_code,
             estimate,
-            ret="gf",
-            pc=plot_code,
+            ret="reg",
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
             rsm.md(f"```python\n{self.stop_code}\n```")
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
-def goodness(
+def regress(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
     debug: bool = False,
 ):
     """
-    Launch a Radiant-for-Python app for goodness of fit analysis
+    Launch a Radiant-for-Python app for linear regression analysis
     """
     if data_dct is None:
-        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
-    rc = basics_goodness(data_dct, descriptions_dct, code=code)
+        data_dct, descriptions_dct = ru.get_dfs(pkg="model")
+    rc = model_regress(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
+    app = App(rc.shiny_ui(), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
+
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    goodness(debug=False)
+    regress(debug=False)
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/logistic.py` & `pyrsm-0.9.3/pyrsm/radiant/logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
-    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    app = App(rc.shiny_ui(), rc.shiny_server)
     www_dir = Path(__file__).parent.parent / "radiant" / "www"
     app_static = StaticFiles(directory=www_dir, html=False)
 
     routes = [
         Mount("/www", app=app_static),
         Mount("/", app=app),
     ]
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/model_utils.py` & `pyrsm-0.9.3/pyrsm/radiant/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/probability_calculator.py` & `pyrsm-0.9.3/pyrsm/radiant/probability_calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from starlette.applications import Starlette
+from starlette.routing import Mount
+from starlette.staticfiles import StaticFiles
+from pathlib import Path
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
 import webbrowser
 import nest_asyncio
 import uvicorn
 import signal
 import os
 import io
@@ -330,16 +334,25 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
+    app = App(rc.shiny_ui(), rc.shiny_server)
+    www_dir = Path(__file__).parent.parent / "radiant" / "www"
+    app_static = StaticFiles(directory=www_dir, html=False)
+
+    routes = [
+        Mount("/www", app=app_static),
+        Mount("/", app=app),
+    ]
+
     uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
+        Starlette(debug=debug, routes=routes),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/regress.py` & `pyrsm-0.9.3/pyrsm/radiant/goodness.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,188 +1,199 @@
 from starlette.applications import Starlette
 from starlette.routing import Mount
 from starlette.staticfiles import StaticFiles
-from shiny import App, ui, reactive, Inputs, Outputs, Session
+from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 from pathlib import Path
 import webbrowser
 import nest_asyncio
 import uvicorn
-import os
 import signal
+import os
 import sys
 import tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
-    "None": "None",
-    "dist": "Distribution",
-    "corr": "Correlation",
-    "scatter": "Scatter",
-    "dashboard": "Dashboard",
-    "residual": "Residual vs Explanatory",
-    "pred": "Prediction plots",
-    "vimp": "Permutation importance",
-    "coef": "Coefficient plot",
+    "observed": "Observed",
+    "expected": "Expected",
+    "chisq": "Chi-squared",
+    "dev_std": "Deviation std.",
 }
 
-controls = {
-    "ci": "Confidence intervals",
-    "ssq": "Sum of Squares",
-    "vif": "VIF",
-}
 
-summary_extra = (
-    ui.input_radio_buttons(
-        "show_interactions",
-        "Interactions:",
-        choices={0: "None", 2: "2-way", 3: "3-way"},
-        inline=True,
-    ),
-    ui.panel_conditional(
-        "input.show_interactions > 0",
-        ui.output_ui("ui_interactions"),
-    ),
-    ui.input_checkbox_group(
-        "controls",
-        "Additional output:",
-        choices=controls,
-    ),
-    ui.output_ui("ui_evar_test"),
-)
-
-plots_extra = (
-    ui.panel_conditional(
-        "input.plots == 'corr'",
-        ui.input_select(
-            "nobs",
-            "Number of data points plotted:",
-            {1000: "1,000", -1: "All"},
+def ui_summary():
+    return ui.panel_conditional(
+        "input.tabs == 'Summary'",
+        ui.panel_well(
+            ui.output_ui("ui_var"),
+            ru.input_return_text_area(
+                "probs",
+                label="Probabilities:",
+                placeholder="Insert list [1/2, 1/2]",
+                value=None,
+            ),
+            ui.input_checkbox_group(
+                id="output",
+                label="Select output tables:",
+                choices=choices,
+            ),
         ),
-    ),
-    ui.panel_conditional(
-        "input.plots == 'pred'",
-        ui.output_ui("ui_incl_evar"),
-        ui.output_ui("ui_incl_interactions"),
-    ),
-)
+    )
+
+
+plots = {"None": "None"}
+plots.update(choices)
 
 
-class model_regress:
+class basics_goodness:
     def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self, *args):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "<< Model > Linear regression (OLS) >>",
+                "<< Basics > Goodness-of-fit >>",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
-                        ru.ui_summary(summary_extra),
-                        mu.ui_predict(self),
-                        ru.ui_plot(choices, plots_extra),
+                        ui_summary(),
+                        ru.ui_plot(plots),
                     ),
-                    ui.column(8, ru.ui_main_model()),
+                    ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             *args,
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/model-linear-regression.ipynb",
-                "Linear regression (OLS) example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-goodness.ipynb",
+                "Goodness-of-fit example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
         get_data = ru.make_data_elements(self, input, output, session)
 
-        # --- section standard for all model apps ---
-        ru.reestimate(input)
-
         # --- section unique to each app ---
-        mu.make_model_inputs(input, output, get_data, "isNum")
-        mu.make_int_inputs(input, output, get_data)
+        @output(id="ui_var")
+        @render.ui
+        def ui_var1():
+            isCat = get_data()["var_types"]["isCat"]
+            return ui.input_select(
+                id="var",
+                label="Select a categorical variable:",
+                selected=None,
+                choices=isCat,
+            )
+
+        def estimation_code():
+            data_name, code = (get_data()[k] for k in ["data_name", "code"])
+
+            if ru.is_empty(input.probs()):
+                probs = None
+            else:
+                probs = input.probs()
+
+            args = {
+                "data": f"""{{"{data_name}": {data_name}}}""",
+                "var": input.var(),
+                "probs": probs,
+            }
+
+            args_string = ru.drop_default_args(
+                args, rsm.basics.goodness, ignore=["data", "probs"]
+            )
+            return f"""rsm.basics.goodness({args_string})""", code
+
         show_code, estimate = mu.make_estimate(
-            self, input, output, get_data, fun="regress", ret="reg", debug=False
-        )
-        mu.make_summary(
             self,
             input,
             output,
-            session,
-            show_code,
-            estimate,
-            ret="reg",
-            sum_fun=rsm.regress.summary,
+            get_data,
+            fun="basics.goodness",
+            ret="gf",
+            ec=estimation_code,
+            run=False,
+            debug=True,
         )
-        mu.make_predict(
+
+        def summary_code():
+            args = [c for c in input.output()]
+            return f"""gf.summary(output={args})"""
+
+        mu.make_summary(
             self,
             input,
             output,
             session,
             show_code,
             estimate,
-            ret="reg",
-            pred_fun=rsm.regress.predict,
+            ret="gf",
+            sum_fun=rsm.basics.goodness.summary,
+            sc=summary_code,
         )
+
+        def plot_code():
+            return f"""gf.plot(plots="{input.plots()}")"""
+
         mu.make_plot(
             self,
             input,
             output,
             session,
             show_code,
             estimate,
-            ret="reg",
+            ret="gf",
+            pc=plot_code,
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
             rsm.md(f"```python\n{self.stop_code}\n```")
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
-def regress(
+def goodness(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
     debug: bool = False,
 ):
     """
-    Launch a Radiant-for-Python app for linear regression analysis
+    Launch a Radiant-for-Python app for goodness of fit analysis
     """
     if data_dct is None:
-        data_dct, descriptions_dct = ru.get_dfs(pkg="model")
-    rc = model_regress(data_dct, descriptions_dct, code=code)
+        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
+    rc = basics_goodness(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
-    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    app = App(rc.shiny_ui(), rc.shiny_server)
     www_dir = Path(__file__).parent.parent / "radiant" / "www"
     app_static = StaticFiles(directory=www_dir, html=False)
 
     routes = [
         Mount("/www", app=app_static),
         Mount("/", app=app),
     ]
@@ -192,8 +203,8 @@
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    regress(debug=False)
+    goodness(debug=False)
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/single_mean.py` & `pyrsm-0.9.3/pyrsm/radiant/single_mean.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     # redirect stdout and stderr to the temporary file
     if not debug:
         temp = tempfile.NamedTemporaryFile()
         sys.stdout = open(temp.name, "w")
         sys.stderr = open(temp.name, "w")
 
-    app = App(rc.shiny_ui(ru.radiant_navbar()), rc.shiny_server)
+    app = App(rc.shiny_ui(), rc.shiny_server)
     www_dir = Path(__file__).parent.parent / "radiant" / "www"
     app_static = StaticFiles(directory=www_dir, html=False)
 
     routes = [
         Mount("/www", app=app_static),
         Mount("/", app=app),
     ]
```

### Comparing `pyrsm-0.9.2/pyrsm/radiant/utils.py` & `pyrsm-0.9.3/pyrsm/radiant/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.9.3/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-nc-sa.png` & `pyrsm-0.9.3/pyrsm/radiant/www/imgs/by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-sa.png` & `pyrsm-0.9.3/pyrsm/radiant/www/imgs/by-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/imgs/icon.png` & `pyrsm-0.9.3/pyrsm/radiant/www/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/js/radiantUI.js` & `pyrsm-0.9.3/pyrsm/radiant/www/js/radiantUI.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/js/returnTextAreaBinding.js` & `pyrsm-0.9.3/pyrsm/radiant/www/js/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/js/screenshot.js` & `pyrsm-0.9.3/pyrsm/radiant/www/js/screenshot.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/radiant/www/style.css` & `pyrsm-0.9.3/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/regress.py` & `pyrsm-0.9.3/pyrsm/regress.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/stats.py` & `pyrsm-0.9.3/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/utils.py` & `pyrsm-0.9.3/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm/visualize.py` & `pyrsm-0.9.3/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.9.3/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.2/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.9.3/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/setup.cfg` & `pyrsm-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_basics.py` & `pyrsm-0.9.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_bins.py` & `pyrsm-0.9.3/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_example_data.py` & `pyrsm-0.9.3/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_perf.py` & `pyrsm-0.9.3/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_regression.py` & `pyrsm-0.9.3/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_stats.py` & `pyrsm-0.9.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.2/tests/test_utils.py` & `pyrsm-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

