# Comparing `tmp/pyrsm-0.9.1.tar.gz` & `tmp/pyrsm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.9.1.tar", last modified: Mon Jul 24 01:43:55 2023, max compression
+gzip compressed data, was "pyrsm-0.9.2.tar", last modified: Sat Jul 29 07:43:51 2023, max compression
```

## Comparing `pyrsm-0.9.1.tar` & `pyrsm-0.9.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.753359 pyrsm-0.9.1/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-24 01:43:55.753454 pyrsm-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.1/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.712963 pyrsm-0.9.1/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-24 01:42:19.000000 pyrsm-0.9.1/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.714995 pyrsm-0.9.1/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.1/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.1/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8847 2023-07-22 13:22:08.000000 pyrsm-0.9.1/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.1/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.1/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9645 2023-07-22 13:13:41.000000 pyrsm-0.9.1/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6717 2023-07-22 14:39:10.000000 pyrsm-0.9.1/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.1/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.1/pyrsm/basics/probability_calculator_functions.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.1/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.1/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.1/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2847 2023-07-23 22:04:07.000000 pyrsm-0.9.1/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.717374 pyrsm-0.9.1/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.9.1/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.718780 pyrsm-0.9.1/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.723110 pyrsm-0.9.1/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.723446 pyrsm-0.9.1/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.728828 pyrsm-0.9.1/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.1/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.1/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/model/ratings_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.1/pyrsm/data/model/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.1/pyrsm/data/model/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.733369 pyrsm-0.9.1/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3793 2023-07-20 19:08:24.000000 pyrsm-0.9.1/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9490 2023-07-23 22:05:12.000000 pyrsm-0.9.1/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.1/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.1/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.1/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.1/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.741488 pyrsm-0.9.1/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      216 2023-07-22 06:25:56.000000 pyrsm-0.9.1/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10003 2023-07-23 21:54:37.000000 pyrsm-0.9.1/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5585 2023-07-22 14:07:40.000000 pyrsm-0.9.1/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     4452 2023-07-22 20:03:41.000000 pyrsm-0.9.1/pyrsm/radiant/data_view.py
--rw-r--r--   0 root         (0) staff       (20)     5358 2023-07-22 14:09:25.000000 pyrsm-0.9.1/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5960 2023-07-22 14:08:11.000000 pyrsm-0.9.1/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    11256 2023-07-20 19:19:46.000000 pyrsm-0.9.1/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)    11364 2023-07-22 23:15:06.000000 pyrsm-0.9.1/pyrsm/radiant/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     5483 2023-07-22 14:08:47.000000 pyrsm-0.9.1/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     6155 2023-07-23 22:33:41.000000 pyrsm-0.9.1/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    22324 2023-07-23 01:56:31.000000 pyrsm-0.9.1/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.742138 pyrsm-0.9.1/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.1/pyrsm/radiant/www/.DS_Store
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.746723 pyrsm-0.9.1/pyrsm/radiant/www/imgs/
--rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-nc-sa.png
--rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-sa.png
--rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.1/pyrsm/radiant/www/imgs/icon.png
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.747165 pyrsm-0.9.1/pyrsm/radiant/www/js/
--rw-r--r--   0 root         (0) staff       (20)      513 2023-07-23 21:45:57.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/radiantUI.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.1/pyrsm/radiant/www/js/screenshot.js
--rw-r--r--   0 root         (0) staff       (20)      829 2023-07-20 17:40:43.000000 pyrsm-0.9.1/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9554 2023-07-22 17:06:30.000000 pyrsm-0.9.1/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.1/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.1/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.1/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.713525 pyrsm-0.9.1/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4049 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      273 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-24 01:43:55.000000 pyrsm-0.9.1/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1088 2023-07-24 01:43:55.753807 pyrsm-0.9.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-24 01:43:55.753233 pyrsm-0.9.1/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.1/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.1/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.1/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.1/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.1/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.1/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.272814 pyrsm-0.9.2/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 07:43:51.272941 pyrsm-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.2/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.255629 pyrsm-0.9.2/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-29 07:43:18.000000 pyrsm-0.9.2/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.257794 pyrsm-0.9.2/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.2/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.2/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8847 2023-07-22 13:22:08.000000 pyrsm-0.9.2/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.2/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.2/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9645 2023-07-22 13:13:41.000000 pyrsm-0.9.2/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6717 2023-07-22 14:39:10.000000 pyrsm-0.9.2/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.2/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.2/pyrsm/basics/probability_calculator_functions.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.2/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.2/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.2/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2847 2023-07-23 22:04:07.000000 pyrsm-0.9.2/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.258007 pyrsm-0.9.2/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      820 2023-07-28 07:03:06.000000 pyrsm-0.9.2/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.259056 pyrsm-0.9.2/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.260833 pyrsm-0.9.2/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.261322 pyrsm-0.9.2/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.264497 pyrsm-0.9.2/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.2/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.2/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-28 07:02:54.000000 pyrsm-0.9.2/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/model/ratings_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.2/pyrsm/data/model/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.2/pyrsm/data/model/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.267186 pyrsm-0.9.2/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-28 07:02:53.000000 pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3910 2023-07-24 08:59:20.000000 pyrsm-0.9.2/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9490 2023-07-23 22:05:12.000000 pyrsm-0.9.2/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.2/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.2/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.2/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.2/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.268485 pyrsm-0.9.2/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      216 2023-07-22 06:25:56.000000 pyrsm-0.9.2/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10069 2023-07-27 07:43:27.000000 pyrsm-0.9.2/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5625 2023-07-27 07:41:53.000000 pyrsm-0.9.2/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     4453 2023-07-27 07:43:46.000000 pyrsm-0.9.2/pyrsm/radiant/data_view.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-07-27 07:41:42.000000 pyrsm-0.9.2/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5991 2023-07-27 07:41:30.000000 pyrsm-0.9.2/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11263 2023-07-26 16:45:47.000000 pyrsm-0.9.2/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)    11466 2023-07-27 07:42:33.000000 pyrsm-0.9.2/pyrsm/radiant/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     5502 2023-07-27 07:41:06.000000 pyrsm-0.9.2/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     6241 2023-07-27 07:52:22.000000 pyrsm-0.9.2/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    19793 2023-07-27 08:32:29.000000 pyrsm-0.9.2/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.269030 pyrsm-0.9.2/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.2/pyrsm/radiant/www/.DS_Store
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.270320 pyrsm-0.9.2/pyrsm/radiant/www/imgs/
+-rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-nc-sa.png
+-rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-sa.png
+-rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.2/pyrsm/radiant/www/imgs/icon.png
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.271525 pyrsm-0.9.2/pyrsm/radiant/www/js/
+-rw-r--r--   0 root         (0) staff       (20)      513 2023-07-23 21:45:57.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/radiantUI.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.2/pyrsm/radiant/www/js/screenshot.js
+-rw-r--r--   0 root         (0) staff       (20)      829 2023-07-20 17:40:43.000000 pyrsm-0.9.2/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9495 2023-07-24 19:44:21.000000 pyrsm-0.9.2/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.2/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.2/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.2/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.256256 pyrsm-0.9.2/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4049 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      273 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-29 07:43:51.000000 pyrsm-0.9.2/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1088 2023-07-29 07:43:51.273297 pyrsm-0.9.2/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-29 07:43:51.272688 pyrsm-0.9.2/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.2/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.2/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.2/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.2/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.2/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.2/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.2/tests/test_utils.py
```

### Comparing `pyrsm-0.9.1/LICENSE` & `pyrsm-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/MANIFEST.in` & `pyrsm-0.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/PKG-INFO` & `pyrsm-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.1/README.md` & `pyrsm-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.9.2/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/compare_means.py` & `pyrsm-0.9.2/pyrsm/basics/compare_means.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/compare_props.py` & `pyrsm-0.9.2/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/correlation.py` & `pyrsm-0.9.2/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/cross_tabs.py` & `pyrsm-0.9.2/pyrsm/basics/cross_tabs.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/goodness.py` & `pyrsm-0.9.2/pyrsm/basics/goodness.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/probability_calculator.py` & `pyrsm-0.9.2/pyrsm/basics/probability_calculator.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/probability_calculator_functions.py` & `pyrsm-0.9.2/pyrsm/basics/probability_calculator_functions.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/single_mean.py` & `pyrsm-0.9.2/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/basics/single_prop.py` & `pyrsm-0.9.2/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/bins.py` & `pyrsm-0.9.2/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/consider.parquet` & `pyrsm-0.9.2/pyrsm/data/basics/consider.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -399,17 +399,17 @@
 000018e0: 7079 5f74 7970 6522 3a20 2269 6e74 3822  py_type": "int8"
 000018f0: 2c20 226d 6574 6164 6174 6122 3a20 7b22  , "metadata": {"
 00001900: 6e75 6d5f 6361 7465 676f 7269 6573 223a  num_categories":
 00001910: 2032 2c20 226f 7264 6572 6564 223a 2066   2, "ordered": f
 00001920: 616c 7365 7d7d 5d2c 2022 6372 6561 746f  alse}}], "creato
 00001930: 7222 3a20 7b22 6c69 6272 6172 7922 3a20  r": {"library": 
 00001940: 2270 7961 7272 6f77 222c 2022 7665 7273  "pyarrow", "vers
-00001950: 696f 6e22 3a20 2231 302e 302e 3122 7d2c  ion": "10.0.1"},
+00001950: 696f 6e22 3a20 2231 322e 302e 3122 7d2c  ion": "12.0.1"},
 00001960: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-00001970: 223a 2022 312e 352e 3322 7d00 180c 4152  ": "1.5.3"}...AR
+00001970: 223a 2022 322e 302e 3322 7d00 180c 4152  ": "2.0.3"}...AR
 00001980: 524f 573a 7363 6865 6d61 1880 092f 2f2f  ROW:schema...///
 00001990: 2f2f 3167 4441 4141 5141 4141 4141 4141  //1gDAAAQAAAAAAA
 000019a0: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
 000019b0: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
 000019c0: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
 000019d0: 4141 4877 4341 4141 4541 4141 4141 5141  AAHwCAAAEAAAAAQA
 000019e0: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
@@ -455,18 +455,18 @@
 00001c60: 3059 5349 3649 4873 6962 6e56 7458 324e  0YSI6IHsibnVtX2N
 00001c70: 6864 4756 6e62 334a 705a 584d 694f 6941  hdGVnb3JpZXMiOiA
 00001c80: 794c 4341 6962 334a 6b5a 584a 6c5a 4349  yLCAib3JkZXJlZCI
 00001c90: 3649 475a 6862 484e 6c66 5831 644c 4341  6IGZhbHNlfX1dLCA
 00001ca0: 6959 334a 6c59 5852 7663 6949 3649 4873  iY3JlYXRvciI6IHs
 00001cb0: 6962 476c 6963 6d46 7965 5349 3649 434a  ibGlicmFyeSI6ICJ
 00001cc0: 7765 5746 7963 6d39 3349 6977 6749 6e5a  weWFycm93IiwgInZ
-00001cd0: 6c63 6e4e 7062 3234 694f 6941 694d 5441  lcnNpb24iOiAiMTA
+00001cd0: 6c63 6e4e 7062 3234 694f 6941 694d 5449  lcnNpb24iOiAiMTI
 00001ce0: 754d 4334 7849 6e30 7349 434a 7759 5735  uMC4xIn0sICJwYW5
 00001cf0: 6b59 584e 6664 6d56 7963 326c 7662 6949  kYXNfdmVyc2lvbiI
-00001d00: 3649 4349 784c 6a55 754d 794a 3941 4141  6ICIxLjUuMyJ9AAA
+00001d00: 3649 4349 794c 6a41 754d 794a 3941 4141  6ICIyLjAuMyJ9AAA
 00001d10: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
 00001d20: 4141 4149 4141 4142 3441 4141 4146 4141  AAAIAAAB4AAAAFAA
 00001d30: 4141 4241 4147 4141 4941 4159 4142 7741  AABAAGAAIAAYABwA
 00001d40: 4d41 4241 4146 4141 5141 4141 4141 4141  MABAAFAAQAAAAAAA
 00001d50: 4242 5251 4141 4142 4141 4141 414a 4141  BBRQAAABAAAAAJAA
 00001d60: 4141 4151 4141 4141 4141 4141 4143 4141  AAAQAAAAAAAAACAA
 00001d70: 4141 474e 7662 6e4e 705a 4756 7941 4141  AAGNvbnNpZGVyAAA
@@ -476,10 +476,10 @@
 00001db0: 4141 4241 4146 4141 4941 4159 4142 7741  AABAAFAAIAAYABwA
 00001dc0: 4d41 4141 4145 4141 5141 4141 4141 4141  MAAAAEAAQAAAAAAA
 00001dd0: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
 00001de0: 4141 4141 4141 4141 4341 4141 4161 5751  AAAAAAAACAAAAaWQ
 00001df0: 4141 4167 4144 4141 4941 4163 4143 4141  AAAgADAAIAAcACAA
 00001e00: 4141 4141 4141 4145 6741 4141 4100 1820  AAAAAAAEgAAAA.. 
 00001e10: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00001e20: 7720 7665 7273 696f 6e20 3130 2e30 2e31  w version 10.0.1
+00001e20: 7720 7665 7273 696f 6e20 3132 2e30 2e30  w version 12.0.0
 00001e30: 192c 1c00 001c 0000 00e7 0700 0050 4152  .,...........PAR
 00001e40: 31                                       1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/consider_description.md` & `pyrsm-0.9.2/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.9.2/pyrsm/data/basics/demand_uk.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -725,17 +725,17 @@
 00002d40: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
 00002d50: 2275 6e69 636f 6465 222c 2022 6e75 6d70  "unicode", "nump
 00002d60: 795f 7479 7065 223a 2022 6f62 6a65 6374  y_type": "object
 00002d70: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
 00002d80: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
 00002d90: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
 00002da0: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00002db0: 6e22 3a20 2231 302e 302e 3122 7d2c 2022  n": "10.0.1"}, "
+00002db0: 6e22 3a20 2231 322e 302e 3122 7d2c 2022  n": "12.0.1"}, "
 00002dc0: 7061 6e64 6173 5f76 6572 7369 6f6e 223a  pandas_version":
-00002dd0: 2022 312e 352e 3322 7d00 180c 4152 524f   "1.5.3"}...ARRO
+00002dd0: 2022 322e 302e 3322 7d00 180c 4152 524f   "2.0.3"}...ARRO
 00002de0: 573a 7363 6865 6d61 18b8 092f 2f2f 2f2f  W:schema.../////
 00002df0: 3441 4441 4141 5141 4141 4141 4141 4b41  4ADAAAQAAAAAAAKA
 00002e00: 4134 4142 6741 4641 4167 4143 6741 4141  A4ABgAFAAgACgAAA
 00002e10: 4141 4242 4141 5141 4141 4141 4141 4b41  AABBAAQAAAAAAAKA
 00002e20: 4177 4141 4141 4541 4167 4143 6741 4141  AwAAAAEAAgACgAAA
 00002e30: 4a51 4341 4141 4541 4141 4141 5141 4141  JQCAAAEAAAAAQAAA
 00002e40: 4177 4141 4141 4941 4177 4142 4141 4941  AwAAAAIAAwABAAIA
@@ -784,17 +784,17 @@
 000030f0: 486c 775a 5349 3649 434a 7659 6d70 6c59  HlwZSI6ICJvYmplY
 00003100: 3351 694c 4341 6962 5756 3059 5752 6864  3QiLCAibWV0YWRhd
 00003110: 4745 694f 6942 7564 5778 7366 5630 7349  GEiOiBudWxsfV0sI
 00003120: 434a 6a63 6d56 6864 4739 7949 6a6f 6765  CJjcmVhdG9yIjoge
 00003130: 794a 7361 574a 7959 584a 3549 6a6f 6749  yJsaWJyYXJ5IjogI
 00003140: 6e42 3559 584a 7962 3363 694c 4341 6964  nB5YXJyb3ciLCAid
 00003150: 6d56 7963 326c 7662 6949 3649 4349 784d  mVyc2lvbiI6ICIxM
-00003160: 4334 774c 6a45 6966 5377 6749 6e42 6862  C4wLjEifSwgInBhb
+00003160: 6934 774c 6a45 6966 5377 6749 6e42 6862  i4wLjEifSwgInBhb
 00003170: 6d52 6863 3139 325a 584a 7a61 5739 7549  mRhc192ZXJzaW9uI
-00003180: 6a6f 6749 6a45 754e 5334 7a49 6e30 4141  jogIjEuNS4zIn0AA
+00003180: 6a6f 6749 6a49 754d 4334 7a49 6e30 4141  jogIjIuMC4zIn0AA
 00003190: 4159 4141 4142 7759 5735 6b59 584d 4141  AYAAABwYW5kYXMAA
 000031a0: 414d 4141 4143 4541 4141 4151 4141 4141  AMAAACEAAAAQAAAA
 000031b0: 4151 4141 4143 592f 2f2f 2f41 4141 4242  AQAAACY////AAABB
 000031c0: 5241 4141 4141 6f41 4141 4142 4141 4141  RAAAAAoAAAABAAAA
 000031d0: 4141 4141 4141 5241 4141 4158 3139 7062  AAAAAARAAAAX19pb
 000031e0: 6d52 6c65 4639 735a 585a 6c62 4638 7758  mRleF9sZXZlbF8wX
 000031f0: 3138 4141 4141 4541 4151 4142 4141 4141  18AAAAEAAQABAAAA
@@ -806,9 +806,9 @@
 00003250: 4141 4145 4141 5141 4141 4141 4141 4241  AAAEAAQAAAAAAABA
 00003260: 6841 4141 4141 6341 4141 4142 4141 4141  hAAAAAcAAAABAAAA
 00003270: 4141 4141 4141 4341 4141 4161 5751 4141  AAAAAACAAAAaWQAA
 00003280: 4167 4144 4141 4941 4163 4143 4141 4141  AgADAAIAAcACAAAA
 00003290: 4141 4141 4145 6741 4141 4141 4141 4141  AAAAAEgAAAAAAAAA
 000032a0: 413d 3d00 1820 7061 7271 7565 742d 6370  A==.. parquet-cp
 000032b0: 702d 6172 726f 7720 7665 7273 696f 6e20  p-arrow version 
-000032c0: 3130 2e30 2e31 193c 1c00 001c 0000 1c00  10.0.1.<........
+000032c0: 3132 2e30 2e30 193c 1c00 001c 0000 1c00  12.0.0.<........
 000032d0: 0000 c308 0000 5041 5231                 ......PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.9.2/pyrsm/data/basics/newspaper.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -293,17 +293,17 @@
 00001240: 7970 6522 3a20 2269 6e74 3822 2c20 226d  ype": "int8", "m
 00001250: 6574 6164 6174 6122 3a20 7b22 6e75 6d5f  etadata": {"num_
 00001260: 6361 7465 676f 7269 6573 223a 2032 2c20  categories": 2, 
 00001270: 226f 7264 6572 6564 223a 2066 616c 7365  "ordered": false
 00001280: 7d7d 5d2c 2022 6372 6561 746f 7222 3a20  }}], "creator": 
 00001290: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
 000012a0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-000012b0: 3a20 2231 302e 302e 3122 7d2c 2022 7061  : "10.0.1"}, "pa
+000012b0: 3a20 2231 322e 302e 3122 7d2c 2022 7061  : "12.0.1"}, "pa
 000012c0: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-000012d0: 312e 352e 3322 7d00 180c 4152 524f 573a  1.5.3"}...ARROW:
+000012d0: 322e 302e 3322 7d00 180c 4152 524f 573a  2.0.3"}...ARROW:
 000012e0: 7363 6865 6d61 18b8 0b2f 2f2f 2f2f 3041  schema.../////0A
 000012f0: 4541 4141 5141 4141 4141 4141 4b41 4134  EAAAQAAAAAAAKAA4
 00001300: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
 00001310: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
 00001320: 4141 4141 4541 4167 4143 6741 4141 4241  AAAAEAAgACgAAABA
 00001330: 4441 4141 4541 4141 4141 5141 4141 4177  DAAAEAAAAAQAAAAw
 00001340: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
@@ -362,17 +362,17 @@
 00001690: 7458 324e 6864 4756 6e62 334a 705a 584d  tX2NhdGVnb3JpZXM
 000016a0: 694f 6941 794c 4341 6962 334a 6b5a 584a  iOiAyLCAib3JkZXJ
 000016b0: 6c5a 4349 3649 475a 6862 484e 6c66 5831  lZCI6IGZhbHNlfX1
 000016c0: 644c 4341 6959 334a 6c59 5852 7663 6949  dLCAiY3JlYXRvciI
 000016d0: 3649 4873 6962 476c 6963 6d46 7965 5349  6IHsibGlicmFyeSI
 000016e0: 3649 434a 7765 5746 7963 6d39 3349 6977  6ICJweWFycm93Iiw
 000016f0: 6749 6e5a 6c63 6e4e 7062 3234 694f 6941  gInZlcnNpb24iOiA
-00001700: 694d 5441 754d 4334 7849 6e30 7349 434a  iMTAuMC4xIn0sICJ
+00001700: 694d 5449 754d 4334 7849 6e30 7349 434a  iMTIuMC4xIn0sICJ
 00001710: 7759 5735 6b59 584e 6664 6d56 7963 326c  wYW5kYXNfdmVyc2l
-00001720: 7662 6949 3649 4349 784c 6a55 754d 794a  vbiI6ICIxLjUuMyJ
+00001720: 7662 6949 3649 4349 794c 6a41 754d 794a  vbiI6ICIyLjAuMyJ
 00001730: 3941 4141 4741 4141 4163 4746 755a 4746  9AAAGAAAAcGFuZGF
 00001740: 7a41 4141 4441 4141 417a 4141 4141 4777  zAAADAAAAzAAAAGw
 00001750: 4141 4141 4541 4141 4172 502f 2f2f 7741  AAAAEAAAArP///wA
 00001760: 4141 5155 5541 4141 4152 4141 4141 4351  AAQUUAAAARAAAACQ
 00001770: 4141 4141 4541 4141 4141 4141 4141 416b  AAAAEAAAAAAAAAAk
 00001780: 4141 4142 4f5a 5864 7a63 4746 775a 5849  AAABOZXdzcGFwZXI
 00001790: 4141 4141 4941 4241 4143 4141 4541 4167  AAAAIABAACAAEAAg
@@ -389,10 +389,10 @@
 00001840: 4141 4141 5141 4251 4143 4141 4741 4163  AAAAQABQACAAGAAc
 00001850: 4144 4141 4141 4241 4145 4141 4141 4141  ADAAAABAAEAAAAAA
 00001860: 4141 5149 5141 4141 4148 4141 4141 4151  AAQIQAAAAHAAAAAQ
 00001870: 4141 4141 4141 4141 4141 6741 4141 476c  AAAAAAAAAAgAAAGl
 00001880: 6b41 4141 4941 4177 4143 4141 4841 4167  kAAAIAAwACAAHAAg
 00001890: 4141 4141 4141 4141 4249 4141 4141 413d  AAAAAAAABIAAAAA=
 000018a0: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-000018b0: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-000018c0: 2e30 2e31 193c 1c00 001c 0000 1c00 0000  .0.1.<..........
+000018b0: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+000018c0: 2e30 2e30 193c 1c00 001c 0000 1c00 0000  .0.0.<..........
 000018d0: 2f0a 0000 5041 5231                      /...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.9.2/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/salary.parquet` & `pyrsm-0.9.2/pyrsm/data/basics/salary.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -357,17 +357,17 @@
 00001640: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
 00001650: 696e 7438 222c 2022 6d65 7461 6461 7461  int8", "metadata
 00001660: 223a 207b 226e 756d 5f63 6174 6567 6f72  ": {"num_categor
 00001670: 6965 7322 3a20 322c 2022 6f72 6465 7265  ies": 2, "ordere
 00001680: 6422 3a20 6661 6c73 657d 7d5d 2c20 2263  d": false}}], "c
 00001690: 7265 6174 6f72 223a 207b 226c 6962 7261  reator": {"libra
 000016a0: 7279 223a 2022 7079 6172 726f 7722 2c20  ry": "pyarrow", 
-000016b0: 2276 6572 7369 6f6e 223a 2022 3130 2e30  "version": "10.0
+000016b0: 2276 6572 7369 6f6e 223a 2022 3132 2e30  "version": "12.0
 000016c0: 2e31 227d 2c20 2270 616e 6461 735f 7665  .1"}, "pandas_ve
-000016d0: 7273 696f 6e22 3a20 2231 2e35 2e33 227d  rsion": "1.5.3"}
+000016d0: 7273 696f 6e22 3a20 2232 2e30 2e33 227d  rsion": "2.0.3"}
 000016e0: 0018 0c41 5252 4f57 3a73 6368 656d 6118  ...ARROW:schema.
 000016f0: d811 2f2f 2f2f 2f35 6747 4141 4155 4141  ../////5gGAAAUAA
 00001700: 4141 4141 4141 4141 4141 4367 414f 4141  AAAAAAAAAACgAOAA
 00001710: 5941 4251 4149 4141 6f41 4141 4141 4151  YABQAIAAoAAAAAAQ
 00001720: 5141 4541 4141 4141 4141 4367 414d 4141  QAEAAAAAAACgAMAA
 00001730: 4141 4241 4149 4141 6f41 4141 4359 4241  AABAAIAAoAAACYBA
 00001740: 4141 4241 4141 4141 4541 4141 414d 4141  AABAAAAAEAAAAMAA
@@ -459,18 +459,18 @@
 00001ca0: 6f67 6579 4a75 6457 3166 5932 4630 5a57  ogeyJudW1fY2F0ZW
 00001cb0: 6476 636d 6c6c 6379 4936 4944 4973 4943  dvcmllcyI6IDIsIC
 00001cc0: 4a76 636d 526c 636d 566b 496a 6f67 5a6d  JvcmRlcmVkIjogZm
 00001cd0: 4673 6332 5639 6656 3073 4943 4a6a 636d  Fsc2V9fV0sICJjcm
 00001ce0: 5668 6447 3979 496a 6f67 6579 4a73 6157  VhdG9yIjogeyJsaW
 00001cf0: 4a79 5958 4a35 496a 6f67 496e 4235 5958  JyYXJ5IjogInB5YX
 00001d00: 4a79 6233 6369 4c43 4169 646d 5679 6332  Jyb3ciLCAidmVyc2
-00001d10: 6c76 6269 4936 4943 4978 4d43 3477 4c6a  lvbiI6ICIxMC4wLj
+00001d10: 6c76 6269 4936 4943 4978 4d69 3477 4c6a  lvbiI6ICIxMi4wLj
 00001d20: 4569 6653 7767 496e 4268 626d 5268 6331  EifSwgInBhbmRhc1
 00001d30: 3932 5a58 4a7a 6157 3975 496a 6f67 496a  92ZXJzaW9uIjogIj
-00001d40: 4575 4e53 347a 496e 3041 4141 4147 4141  EuNS4zIn0AAAAGAA
+00001d40: 4975 4d43 347a 496e 3041 4141 4147 4141  IuMC4zIn0AAAAGAA
 00001d50: 4141 6347 4675 5a47 467a 4141 4147 4141  AAcGFuZGFzAAAGAA
 00001d60: 4141 6c41 4541 4144 5142 4141 4449 4141  AAlAEAADQBAADIAA
 00001d70: 4141 6a41 4141 4146 5141 4141 4145 4141  AAjAAAAFQAAAAEAA
 00001d80: 4141 3850 372f 2f77 4141 4151 5555 4141  AA8P7//wAAAQUUAA
 00001d90: 4141 5041 4141 4142 7741 4141 4145 4141  AAPAAAABwAAAAEAA
 00001da0: 4141 4141 4141 4141 4d41 4141 427a 5a58  AAAAAAAAMAAABzZX
 00001db0: 6741 4341 4151 4141 6741 4241 4149 4141  gACAAQAAgABAAIAA
@@ -504,10 +504,10 @@
 00001f70: 5941 4277 414d 4141 4141 4541 4151 4141  YABwAMAAAAEAAQAA
 00001f80: 4141 4141 4142 4168 4141 4141 4167 4141  AAAAABAhAAAAAgAA
 00001f90: 4141 4241 4141 4141 4141 4141 4147 4141  AABAAAAAAAAAAGAA
 00001fa0: 4141 6332 4673 5958 4a35 4141 4149 4141  AAc2FsYXJ5AAAIAA
 00001fb0: 7741 4341 4148 4141 6741 4141 4141 4141  wACAAHAAgAAAAAAA
 00001fc0: 4142 4941 4141 4141 3d3d 0018 2070 6172  ABIAAAAA==.. par
 00001fd0: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-00001fe0: 6572 7369 6f6e 2031 302e 302e 3119 6c1c  ersion 10.0.1.l.
+00001fe0: 6572 7369 6f6e 2031 322e 302e 3019 6c1c  ersion 12.0.0.l.
 00001ff0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00002000: 0000 fa0f 0000 5041 5231                 ......PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/basics/salary_description.md` & `pyrsm-0.9.2/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/data/avengers.parquet` & `pyrsm-0.9.2/pyrsm/data/data/avengers.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,17 @@
 000006c0: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
 000006d0: 223a 2022 756e 6963 6f64 6522 2c20 226e  ": "unicode", "n
 000006e0: 756d 7079 5f74 7970 6522 3a20 226f 626a  umpy_type": "obj
 000006f0: 6563 7422 2c20 226d 6574 6164 6174 6122  ect", "metadata"
 00000700: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
 00000710: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
 00000720: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00000730: 7369 6f6e 223a 2022 3130 2e30 2e31 227d  sion": "10.0.1"}
+00000730: 7369 6f6e 223a 2022 3132 2e30 2e31 227d  sion": "12.0.1"}
 00000740: 2c20 2270 616e 6461 735f 7665 7273 696f  , "pandas_versio
-00000750: 6e22 3a20 2231 2e35 2e33 227d 0018 0c41  n": "1.5.3"}...A
+00000750: 6e22 3a20 2232 2e30 2e33 227d 0018 0c41  n": "2.0.3"}...A
 00000760: 5252 4f57 3a73 6368 656d 6118 b80b 2f2f  RROW:schema...//
 00000770: 2f2f 2f30 4145 4141 4151 4141 4141 4141  ///0AEAAAQAAAAAA
 00000780: 414b 4141 3441 4267 4146 4141 6741 4367  AKAA4ABgAFAAgACg
 00000790: 4141 4141 4142 4241 4151 4141 4141 4141  AAAAABBAAQAAAAAA
 000007a0: 414b 4141 7741 4141 4145 4141 6741 4367  AKAAwAAAAEAAgACg
 000007b0: 4141 4145 4144 4141 4145 4141 4141 4151  AAAEADAAAEAAAAAQ
 000007c0: 4141 4141 7741 4141 4149 4141 7741 4241  AAAAwAAAAIAAwABA
@@ -182,18 +182,18 @@
 00000b50: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
 00000b60: 6f67 496d 3969 616d 566a 6443 4973 4943  ogIm9iamVjdCIsIC
 00000b70: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
 00000b80: 3531 6247 7839 5853 7767 496d 4e79 5a57  51bGx9XSwgImNyZW
 00000b90: 4630 6233 4969 4f69 4237 496d 7870 596e  F0b3IiOiB7ImxpYn
 00000ba0: 4a68 636e 6b69 4f69 4169 6348 6c68 636e  JhcnkiOiAicHlhcn
 00000bb0: 4a76 6479 4973 4943 4a32 5a58 4a7a 6157  JvdyIsICJ2ZXJzaW
-00000bc0: 3975 496a 6f67 496a 4577 4c6a 4175 4d53  9uIjogIjEwLjAuMS
+00000bc0: 3975 496a 6f67 496a 4579 4c6a 4175 4d53  9uIjogIjEyLjAuMS
 00000bd0: 4a39 4c43 4169 6347 4675 5a47 467a 5833  J9LCAicGFuZGFzX3
-00000be0: 5a6c 636e 4e70 6232 3469 4f69 4169 4d53  ZlcnNpb24iOiAiMS
-00000bf0: 3431 4c6a 4d69 6651 4147 4141 4141 6347  41LjMifQAGAAAAcG
+00000be0: 5a6c 636e 4e70 6232 3469 4f69 4169 4d69  ZlcnNpb24iOiAiMi
+00000bf0: 3477 4c6a 4d69 6651 4147 4141 4141 6347  4wLjMifQAGAAAAcG
 00000c00: 4675 5a47 467a 4141 4145 4141 4141 6f41  FuZGFzAAAEAAAAoA
 00000c10: 4141 4147 4141 4141 4130 4141 4141 4241  AAAGAAAAA0AAAABA
 00000c20: 4141 4149 442f 2f2f 3841 4141 4546 4541  AAAID///8AAAEFEA
 00000c30: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
 00000c40: 4141 4141 6b41 4141 4277 6457 4a73 6158  AAAAkAAABwdWJsaX
 00000c50: 4e6f 5a58 4941 4141 4230 2f2f 2f2f 7250  NoZXIAAAB0////rP
 00000c60: 2f2f 2f77 4141 4151 5551 4141 4141 4741  ///wAAAQUQAAAAGA
@@ -206,9 +206,9 @@
 00000cd0: 4155 4141 6741 4267 4148 4141 7741 4141  AUAAgABgAHAAwAAA
 00000ce0: 4151 4142 4141 4141 4141 4141 4546 4541  AQABAAAAAAAAEFEA
 00000cf0: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
 00000d00: 4141 4141 5141 4141 4275 5957 316c 4141  AAAAQAAABuYW1lAA
 00000d10: 4141 4141 5141 4241 4145 4141 4141 4141  AAAAQABAAEAAAAAA
 00000d20: 4141 4141 3d3d 0018 2070 6172 7175 6574  AAAA==.. parquet
 00000d30: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-00000d40: 6f6e 2031 302e 302e 3119 4c1c 0000 1c00  on 10.0.1.L.....
+00000d40: 6f6e 2031 322e 302e 3019 4c1c 0000 1c00  on 12.0.0.L.....
 00000d50: 001c 0000 1c00 0000 af0a 0000 5041 5231  ............PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.9.2/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.9.2/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/data/publishers.parquet` & `pyrsm-0.9.2/pyrsm/data/data/publishers.parquet`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 000003d0: 666f 756e 6465 6422 2c20 2270 616e 6461  founded", "panda
 000003e0: 735f 7479 7065 223a 2022 696e 7433 3222  s_type": "int32"
 000003f0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
 00000400: 2269 6e74 3332 222c 2022 6d65 7461 6461  "int32", "metada
 00000410: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
 00000420: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 00000430: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-00000440: 7665 7273 696f 6e22 3a20 2231 302e 302e  version": "10.0.
+00000440: 7665 7273 696f 6e22 3a20 2231 322e 302e  version": "12.0.
 00000450: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-00000460: 7369 6f6e 223a 2022 312e 352e 3322 7d00  sion": "1.5.3"}.
+00000460: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
 00000470: 180c 4152 524f 573a 7363 6865 6d61 18ac  ..ARROW:schema..
 00000480: 082f 2f2f 2f2f 7867 4441 4141 5141 4141  ./////xgDAAAQAAA
 00000490: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
 000004a0: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
 000004b0: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
 000004c0: 4143 6741 4141 4751 4341 4141 4541 4141  ACgAAAGQCAAAEAAA
 000004d0: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
@@ -117,27 +117,27 @@
 00000740: 3162 5842 3558 3352 3563 4755 694f 6941  1bXB5X3R5cGUiOiA
 00000750: 6961 5735 304d 7a49 694c 4341 6962 5756  iaW50MzIiLCAibWV
 00000760: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
 00000770: 7366 5630 7349 434a 6a63 6d56 6864 4739  sfV0sICJjcmVhdG9
 00000780: 7949 6a6f 6765 794a 7361 574a 7959 584a  yIjogeyJsaWJyYXJ
 00000790: 3549 6a6f 6749 6e42 3559 584a 7962 3363  5IjogInB5YXJyb3c
 000007a0: 694c 4341 6964 6d56 7963 326c 7662 6949  iLCAidmVyc2lvbiI
-000007b0: 3649 4349 784d 4334 774c 6a45 6966 5377  6ICIxMC4wLjEifSw
+000007b0: 3649 4349 784d 6934 774c 6a45 6966 5377  6ICIxMi4wLjEifSw
 000007c0: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-000007d0: 7a61 5739 7549 6a6f 6749 6a45 754e 5334  zaW9uIjogIjEuNS4
+000007d0: 7a61 5739 7549 6a6f 6749 6a49 754d 4334  zaW9uIjogIjIuMC4
 000007e0: 7a49 6e30 4141 4159 4141 4142 7759 5735  zIn0AAAYAAABwYW5
 000007f0: 6b59 584d 4141 4149 4141 4142 5541 4141  kYXMAAAIAAABUAAA
 00000800: 4142 4141 4141 4d54 2f2f 2f38 4141 4145  ABAAAAMT///8AAAE
 00000810: 4345 4141 4141 4351 4141 4141 4541 4141  CEAAAACQAAAAEAAA
 00000820: 4141 4141 4141 416f 4141 4142 3563 6c39  AAAAAAAoAAAB5cl9
 00000830: 6d62 3356 755a 4756 6b41 4141 4941 4177  mb3VuZGVkAAAIAAw
 00000840: 4143 4141 4841 4167 4141 4141 4141 4141  ACAAHAAgAAAAAAAA
 00000850: 4249 4141 4141 4241 4146 4141 4941 4159  BIAAAABAAFAAIAAY
 00000860: 4142 7741 4d41 4141 4145 4141 5141 4141  ABwAMAAAAEAAQAAA
 00000870: 4141 4141 4242 5241 4141 4141 6741 4141  AAAABBRAAAAAgAAA
 00000880: 4142 4141 4141 4141 4141 4141 4a41 4141  ABAAAAAAAAAAJAAA
 00000890: 4163 4856 6962 476c 7a61 4756 7941 4141  AcHVibGlzaGVyAAA
 000008a0: 4142 4141 4541 4151 4141 4141 3d00 1820  ABAAEAAQAAAA=.. 
 000008b0: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-000008c0: 7720 7665 7273 696f 6e20 3130 2e30 2e31  w version 10.0.1
+000008c0: 7720 7665 7273 696f 6e20 3132 2e30 2e30  w version 12.0.0
 000008d0: 192c 1c00 001c 0000 008d 0700 0050 4152  .,...........PAR
 000008e0: 31                                       1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.9.2/pyrsm/data/data/superheroes.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 000006c0: 6173 5f74 7970 6522 3a20 2275 6e69 636f  as_type": "unico
 000006d0: 6465 222c 2022 6e75 6d70 795f 7479 7065  de", "numpy_type
 000006e0: 223a 2022 6f62 6a65 6374 222c 2022 6d65  ": "object", "me
 000006f0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 00000700: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 00000710: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 00000720: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00000730: 302e 302e 3122 7d2c 2022 7061 6e64 6173  0.0.1"}, "pandas
-00000740: 5f76 6572 7369 6f6e 223a 2022 312e 352e  _version": "1.5.
+00000730: 322e 302e 3122 7d2c 2022 7061 6e64 6173  2.0.1"}, "pandas
+00000740: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
 00000750: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
 00000760: 6d61 18b8 0b2f 2f2f 2f2f 3041 4541 4141  ma.../////0AEAAA
 00000770: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00000780: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 00000790: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 000007a0: 4541 4167 4143 6741 4141 4541 4441 4141  EAAgACgAAAEADAAA
 000007b0: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
@@ -182,17 +182,17 @@
 00000b50: 3065 5842 6c49 6a6f 6749 6d39 6961 6d56  0eXBlIjogIm9iamV
 00000b60: 6a64 4349 7349 434a 745a 5852 685a 4746  jdCIsICJtZXRhZGF
 00000b70: 3059 5349 3649 4735 3162 4778 3958 5377  0YSI6IG51bGx9XSw
 00000b80: 6749 6d4e 795a 5746 3062 3349 694f 6942  gImNyZWF0b3IiOiB
 00000b90: 3749 6d78 7059 6e4a 6863 6e6b 694f 6941  7ImxpYnJhcnkiOiA
 00000ba0: 6963 486c 6863 6e4a 7664 7949 7349 434a  icHlhcnJvdyIsICJ
 00000bb0: 325a 584a 7a61 5739 7549 6a6f 6749 6a45  2ZXJzaW9uIjogIjE
-00000bc0: 774c 6a41 754d 534a 394c 4341 6963 4746  wLjAuMSJ9LCAicGF
+00000bc0: 794c 6a41 754d 534a 394c 4341 6963 4746  yLjAuMSJ9LCAicGF
 00000bd0: 755a 4746 7a58 335a 6c63 6e4e 7062 3234  uZGFzX3ZlcnNpb24
-00000be0: 694f 6941 694d 5334 314c 6a4d 6966 5141  iOiAiMS41LjMifQA
+00000be0: 694f 6941 694d 6934 774c 6a4d 6966 5141  iOiAiMi4wLjMifQA
 00000bf0: 4741 4141 4163 4746 755a 4746 7a41 4141  GAAAAcGFuZGFzAAA
 00000c00: 4541 4141 416f 4141 4141 4741 4141 4141  EAAAAoAAAAGAAAAA
 00000c10: 3041 4141 4142 4141 4141 4944 2f2f 2f38  0AAAABAAAAID///8
 00000c20: 4141 4145 4645 4141 4141 4277 4141 4141  AAAEFEAAAABwAAAA
 00000c30: 4541 4141 4141 4141 4141 416b 4141 4142  EAAAAAAAAAAkAAAB
 00000c40: 7764 574a 7361 584e 6f5a 5849 4141 4142  wdWJsaXNoZXIAAAB
 00000c50: 302f 2f2f 2f72 502f 2f2f 7741 4141 5155  0////rP///wAAAQU
@@ -205,10 +205,10 @@
 00000cc0: 492f 2f2f 2f45 4141 5541 4167 4142 6741  I////EAAUAAgABgA
 00000cd0: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
 00000ce0: 4141 4145 4645 4141 4141 4277 4141 4141  AAAEFEAAAABwAAAA
 00000cf0: 4541 4141 4141 4141 4141 4151 4141 4142  EAAAAAAAAAAQAAAB
 00000d00: 7559 5731 6c41 4141 4141 4151 4142 4141  uYW1lAAAAAAQABAA
 00000d10: 4541 4141 4141 4141 4141 413d 3d00 1820  EAAAAAAAAAA==.. 
 00000d20: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00000d30: 7720 7665 7273 696f 6e20 3130 2e30 2e31  w version 10.0.1
+00000d30: 7720 7665 7273 696f 6e20 3132 2e30 2e30  w version 12.0.0
 00000d40: 194c 1c00 001c 0000 1c00 001c 0000 00a7  .L..............
 00000d50: 0a00 0050 4152 31                        ...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/data/titanic.parquet` & `pyrsm-0.9.2/pyrsm/data/model/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/data/titanic_description.md` & `pyrsm-0.9.2/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.9.2/pyrsm/data/design/rndnames.parquet`

 * *Files 3% similar despite different names*

```diff
@@ -167,17 +167,17 @@
 00000a60: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
 00000a70: 7438 222c 2022 6d65 7461 6461 7461 223a  t8", "metadata":
 00000a80: 207b 226e 756d 5f63 6174 6567 6f72 6965   {"num_categorie
 00000a90: 7322 3a20 322c 2022 6f72 6465 7265 6422  s": 2, "ordered"
 00000aa0: 3a20 6661 6c73 657d 7d5d 2c20 2263 7265  : false}}], "cre
 00000ab0: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00000ac0: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00000ad0: 6572 7369 6f6e 223a 2022 3130 2e30 2e31  ersion": "10.0.1
+00000ad0: 6572 7369 6f6e 223a 2022 3132 2e30 2e31  ersion": "12.0.1
 00000ae0: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00000af0: 696f 6e22 3a20 2231 2e35 2e33 227d 0018  ion": "1.5.3"}..
+00000af0: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
 00000b00: 0c41 5252 4f57 3a73 6368 656d 6118 8009  .ARROW:schema...
 00000b10: 2f2f 2f2f 2f31 6744 4141 4151 4141 4141  /////1gDAAAQAAAA
 00000b20: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00000b30: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 00000b40: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 00000b50: 4367 4141 4149 4143 4141 4145 4141 4141  CgAAAIACAAAEAAAA
 00000b60: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -224,17 +224,17 @@
 00000df0: 496d 3531 6256 396a 5958 526c 5a32 3979  Im51bV9jYXRlZ29y
 00000e00: 6157 567a 496a 6f67 4d69 7767 496d 3979  aWVzIjogMiwgIm9y
 00000e10: 5a47 5679 5a57 5169 4f69 426d 5957 787a  ZGVyZWQiOiBmYWxz
 00000e20: 5a58 3139 5853 7767 496d 4e79 5a57 4630  ZX19XSwgImNyZWF0
 00000e30: 6233 4969 4f69 4237 496d 7870 596e 4a68  b3IiOiB7ImxpYnJh
 00000e40: 636e 6b69 4f69 4169 6348 6c68 636e 4a76  cnkiOiAicHlhcnJv
 00000e50: 6479 4973 4943 4a32 5a58 4a7a 6157 3975  dyIsICJ2ZXJzaW9u
-00000e60: 496a 6f67 496a 4577 4c6a 4175 4d53 4a39  IjogIjEwLjAuMSJ9
+00000e60: 496a 6f67 496a 4579 4c6a 4175 4d53 4a39  IjogIjEyLjAuMSJ9
 00000e70: 4c43 4169 6347 4675 5a47 467a 5833 5a6c  LCAicGFuZGFzX3Zl
-00000e80: 636e 4e70 6232 3469 4f69 4169 4d53 3431  cnNpb24iOiAiMS41
+00000e80: 636e 4e70 6232 3469 4f69 4169 4d69 3477  cnNpb24iOiAiMi4w
 00000e90: 4c6a 4d69 6651 4141 4141 4147 4141 4141  LjMifQAAAAAGAAAA
 00000ea0: 6347 4675 5a47 467a 4141 4143 4141 4141  cGFuZGFzAAACAAAA
 00000eb0: 6541 4141 4142 5141 4141 4151 4142 6741  eAAAABQAAAAQABgA
 00000ec0: 4341 4147 4141 6341 4441 4151 4142 5141  CAAGAAcADAAQABQA
 00000ed0: 4541 4141 4141 4141 4151 5555 4141 4141  EAAAAAAAAQUUAAAA
 00000ee0: 5141 4141 4143 4141 4141 4145 4141 4141  QAAAACAAAAAEAAAA
 00000ef0: 4141 4141 4141 5941 4141 4248 5a57 356b  AAAAAAYAAABHZW5k
@@ -244,10 +244,10 @@
 00000f30: 4341 4141 414d 6a2f 2f2f 3851 4142 5141  CAAAAMj///8QABQA
 00000f40: 4341 4147 4141 6341 4441 4141 4142 4141  CAAGAAcADAAAABAA
 00000f50: 4541 4141 4141 4141 4151 5551 4141 4141  EAAAAAAAAQUQAAAA
 00000f60: 4841 4141 4141 5141 4141 4141 4141 4141  HAAAAAQAAAAAAAAA
 00000f70: 4251 4141 4145 3568 6257 567a 4141 4141  BQAAAE5hbWVzAAAA
 00000f80: 4241 4145 4141 5141 4141 4141 4141 4141  BAAEAAQAAAAAAAAA
 00000f90: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-00000fa0: 7272 6f77 2076 6572 7369 6f6e 2031 302e  rrow version 10.
-00000fb0: 302e 3119 2c1c 0000 1c00 0000 fc07 0000  0.1.,...........
+00000fa0: 7272 6f77 2076 6572 7369 6f6e 2031 322e  rrow version 12.
+00000fb0: 302e 3019 2c1c 0000 1c00 0000 fc07 0000  0.0.,...........
 00000fc0: 5041 5231                                PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/catalog.parquet` & `pyrsm-0.9.2/pyrsm/data/model/catalog.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -333,17 +333,17 @@
 000014c0: 6765 222c 2022 7061 6e64 6173 5f74 7970  ge", "pandas_typ
 000014d0: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
 000014e0: 6e75 6d70 795f 7479 7065 223a 2022 666c  numpy_type": "fl
 000014f0: 6f61 7436 3422 2c20 226d 6574 6164 6174  oat64", "metadat
 00001500: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00001510: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00001520: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00001530: 6572 7369 6f6e 223a 2022 3130 2e30 2e31  ersion": "10.0.1
+00001530: 6572 7369 6f6e 223a 2022 3132 2e30 2e31  ersion": "12.0.1
 00001540: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00001550: 696f 6e22 3a20 2231 2e35 2e33 227d 0018  ion": "1.5.3"}..
+00001550: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
 00001560: 0c41 5252 4f57 3a73 6368 656d 6118 800d  .ARROW:schema...
 00001570: 2f2f 2f2f 2f39 6745 4141 4151 4141 4141  /////9gEAAAQAAAA
 00001580: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00001590: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 000015a0: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 000015b0: 4367 4141 414a 7744 4141 4145 4141 4141  CgAAAJwDAAAEAAAA
 000015c0: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -414,17 +414,17 @@
 000019d0: 6448 6c77 5a53 4936 4943 4a6d 6247 3968  dHlwZSI6ICJmbG9h
 000019e0: 6444 5930 4969 7767 496d 316c 6447 466b  dDY0IiwgIm1ldGFk
 000019f0: 5958 5268 496a 6f67 626e 5673 6248 3164  YXRhIjogbnVsbH1d
 00001a00: 4c43 4169 5933 4a6c 5958 5276 6369 4936  LCAiY3JlYXRvciI6
 00001a10: 4948 7369 6247 6c69 636d 4679 6553 4936  IHsibGlicmFyeSI6
 00001a20: 4943 4a77 6557 4679 636d 3933 4969 7767  ICJweWFycm93Iiwg
 00001a30: 496e 5a6c 636e 4e70 6232 3469 4f69 4169  InZlcnNpb24iOiAi
-00001a40: 4d54 4175 4d43 3478 496e 3073 4943 4a77  MTAuMC4xIn0sICJw
+00001a40: 4d54 4975 4d43 3478 496e 3073 4943 4a77  MTIuMC4xIn0sICJw
 00001a50: 5957 356b 5958 4e66 646d 5679 6332 6c76  YW5kYXNfdmVyc2lv
-00001a60: 6269 4936 4943 4978 4c6a 5575 4d79 4a39  biI6ICIxLjUuMyJ9
+00001a60: 6269 4936 4943 4979 4c6a 4175 4d79 4a39  biI6ICIyLjAuMyJ9
 00001a70: 4141 4141 4141 5941 4141 4277 5957 356b  AAAAAAYAAABwYW5k
 00001a80: 5958 4d41 4141 5541 4141 4459 4141 4141  YXMAAAUAAADYAAAA
 00001a90: 6c41 4141 4147 5141 4141 4177 4141 4141  lAAAAGQAAAAwAAAA
 00001aa0: 4241 4141 4145 7a2f 2f2f 3841 4141 4544  BAAAAEz///8AAAED
 00001ab0: 4541 4141 4142 5141 4141 4145 4141 4141  EAAAABQAAAAEAAAA
 00001ac0: 4141 4141 4141 4d41 4141 4242 5a32 5541  AAAAAAMAAABBZ2UA
 00001ad0: 6576 2f2f 2f77 4141 4167 4230 2f2f 2f2f  ev///wAAAgB0////
@@ -442,10 +442,10 @@
 00001b90: 4141 4143 4142 4141 4641 4149 4141 5941  AAACABAAFAAIAAYA
 00001ba0: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
 00001bb0: 4141 4142 4168 4141 4141 4163 4141 4141  AAABAhAAAAAcAAAA
 00001bc0: 4241 4141 4141 4141 4141 4143 4141 4141  BAAAAAAAAAACAAAA
 00001bd0: 6157 5141 4141 6741 4441 4149 4141 6341  aWQAAAgADAAIAAcA
 00001be0: 4341 4141 4141 4141 4141 4567 4141 4141  CAAAAAAAAAEgAAAA
 00001bf0: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-00001c00: 7272 6f77 2076 6572 7369 6f6e 2031 302e  rrow version 10.
-00001c10: 302e 3119 5c1c 0000 1c00 001c 0000 1c00  0.1.\...........
+00001c00: 7272 6f77 2076 6572 7369 6f6e 2031 322e  rrow version 12.
+00001c10: 302e 3019 5c1c 0000 1c00 001c 0000 1c00  0.0.\...........
 00001c20: 001c 0000 005f 0c00 0050 4152 31         ....._...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/catalog_description.md` & `pyrsm-0.9.2/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.9.2/pyrsm/data/data/diamonds.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -2849,17 +2849,17 @@
 0000b200: 3a20 2264 6174 6522 2c20 2270 616e 6461  : "date", "panda
 0000b210: 735f 7479 7065 223a 2022 6461 7465 222c  s_type": "date",
 0000b220: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
 0000b230: 6f62 6a65 6374 222c 2022 6d65 7461 6461  object", "metada
 0000b240: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
 0000b250: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 0000b260: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-0000b270: 7665 7273 696f 6e22 3a20 2231 302e 302e  version": "10.0.
+0000b270: 7665 7273 696f 6e22 3a20 2231 322e 302e  version": "12.0.
 0000b280: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-0000b290: 7369 6f6e 223a 2022 312e 352e 3322 7d00  sion": "1.5.3"}.
+0000b290: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
 0000b2a0: 180c 4152 524f 573a 7363 6865 6d61 1880  ..ARROW:schema..
 0000b2b0: 192f 2f2f 2f2f 3167 4a41 4141 5541 4141  ./////1gJAAAUAAA
 0000b2c0: 4141 4141 4141 4141 4143 6741 4f41 4159  AAAAAAAAACgAOAAY
 0000b2d0: 4142 5141 4941 416f 4141 4141 4141 5151  ABQAIAAoAAAAAAQQ
 0000b2e0: 4145 4141 4141 4141 4143 6741 4d41 4141  AEAAAAAAACgAMAAA
 0000b2f0: 4142 4141 4941 416f 4141 4143 4d42 6741  ABAAIAAoAAACMBgA
 0000b300: 4142 4141 4141 4145 4141 4141 4d41 4141  ABAAAAAEAAAAMAAA
@@ -2993,17 +2993,17 @@
 0000bb00: 7765 5639 3065 5842 6c49 6a6f 6749 6d39  weV90eXBlIjogIm9
 0000bb10: 6961 6d56 6a64 4349 7349 434a 745a 5852  iamVjdCIsICJtZXR
 0000bb20: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
 0000bb30: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
 0000bb40: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
 0000bb50: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
 0000bb60: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
-0000bb70: 6749 6a45 774c 6a41 754d 534a 394c 4341  gIjEwLjAuMSJ9LCA
+0000bb70: 6749 6a45 794c 6a41 754d 534a 394c 4341  gIjEyLjAuMSJ9LCA
 0000bb80: 6963 4746 755a 4746 7a58 335a 6c63 6e4e  icGFuZGFzX3ZlcnN
-0000bb90: 7062 3234 694f 6941 694d 5334 314c 6a4d  pb24iOiAiMS41LjM
+0000bb90: 7062 3234 694f 6941 694d 6934 774c 6a4d  pb24iOiAiMi4wLjM
 0000bba0: 6966 5141 4141 4159 4141 4142 7759 5735  ifQAAAAYAAABwYW5
 0000bbb0: 6b59 584d 4141 4173 4141 4142 6741 6741  kYXMAAAsAAABgAgA
 0000bbc0: 4148 4149 4141 4d77 4241 4142 6f41 5141  AHAIAAMwBAABoAQA
 0000bbd0: 4147 4145 4141 4f67 4141 4143 3441 4141  AGAEAAOgAAAC4AAA
 0000bbe0: 416a 4141 4141 4741 4141 4141 3041 4141  AjAAAAGAAAAA0AAA
 0000bbf0: 4142 4141 4141 4e7a 392f 2f38 4141 4145  ABAAAANz9//8AAAE
 0000bc00: 4945 4141 4141 4267 4141 4141 4541 4141  IEAAAABgAAAAEAAA
@@ -3054,11 +3054,11 @@
 0000bed0: 4145 4141 5541 4167 4142 6741 4841 4177  AEAAUAAgABgAHAAw
 0000bee0: 4141 4141 5141 4241 4141 4141 4141 4145  AAAAQABAAAAAAAAE
 0000bef0: 4345 4141 4141 4341 4141 4141 4541 4141  CEAAAACAAAAAEAAA
 0000bf00: 4141 4141 4141 4155 4141 4142 7763 6d6c  AAAAAAAUAAABwcml
 0000bf10: 6a5a 5141 4141 4167 4144 4141 4941 4163  jZQAAAAgADAAIAAc
 0000bf20: 4143 4141 4141 4141 4141 4145 6741 4141  ACAAAAAAAAAEgAAA
 0000bf30: 4100 1820 7061 7271 7565 742d 6370 702d  A.. parquet-cpp-
-0000bf40: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-0000bf50: 2e30 2e31 19bc 1c00 001c 0000 1c00 001c  .0.1............
+0000bf40: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+0000bf50: 2e30 2e30 19bc 1c00 001c 0000 1c00 001c  .0.0............
 0000bf60: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 0000bf70: 001c 0000 1c00 0000 c517 0000 5041 5231  ............PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.9.2/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.9.2/pyrsm/data/model/direct_marketing.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -1193,17 +1193,17 @@
 00004a80: 2272 6e64 3222 2c20 2270 616e 6461 735f  "rnd2", "pandas_
 00004a90: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
 00004aa0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
 00004ab0: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
 00004ac0: 6461 7461 223a 206e 756c 6c7d 5d2c 2022  data": null}], "
 00004ad0: 6372 6561 746f 7222 3a20 7b22 6c69 6272  creator": {"libr
 00004ae0: 6172 7922 3a20 2270 7961 7272 6f77 222c  ary": "pyarrow",
-00004af0: 2022 7665 7273 696f 6e22 3a20 2231 302e   "version": "10.
+00004af0: 2022 7665 7273 696f 6e22 3a20 2231 322e   "version": "12.
 00004b00: 302e 3122 7d2c 2022 7061 6e64 6173 5f76  0.1"}, "pandas_v
-00004b10: 6572 7369 6f6e 223a 2022 312e 352e 3322  ersion": "1.5.3"
+00004b10: 6572 7369 6f6e 223a 2022 322e 302e 3322  ersion": "2.0.3"
 00004b20: 7d00 180c 4152 524f 573a 7363 6865 6d61  }...ARROW:schema
 00004b30: 18b8 1e2f 2f2f 2f2f 3241 4c41 4141 5141  .../////2ALAAAQA
 00004b40: 4141 4141 4141 4b41 4134 4142 6741 4641  AAAAAAKAA4ABgAFA
 00004b50: 4167 4143 6741 4141 4141 4242 4141 5141  AgACgAAAAABBAAQA
 00004b60: 4141 4141 4141 4b41 4177 4141 4141 4541  AAAAAAKAAwAAAAEA
 00004b70: 4167 4143 6741 4141 4d67 4841 4141 4541  AgACgAAAMgHAAAEA
 00004b80: 4141 4141 5141 4141 4177 4141 4141 4941  AAAAQAAAAwAAAAIA
@@ -1363,17 +1363,17 @@
 00005520: 486c 6664 486c 775a 5349 3649 434a 6d62  HlfdHlwZSI6ICJmb
 00005530: 4739 6864 4459 3049 6977 6749 6d31 6c64  G9hdDY0IiwgIm1ld
 00005540: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
 00005550: 4831 644c 4341 6959 334a 6c59 5852 7663  H1dLCAiY3JlYXRvc
 00005560: 6949 3649 4873 6962 476c 6963 6d46 7965  iI6IHsibGlicmFye
 00005570: 5349 3649 434a 7765 5746 7963 6d39 3349  SI6ICJweWFycm93I
 00005580: 6977 6749 6e5a 6c63 6e4e 7062 3234 694f  iwgInZlcnNpb24iO
-00005590: 6941 694d 5441 754d 4334 7849 6e30 7349  iAiMTAuMC4xIn0sI
+00005590: 6941 694d 5449 754d 4334 7849 6e30 7349  iAiMTIuMC4xIn0sI
 000055a0: 434a 7759 5735 6b59 584e 6664 6d56 7963  CJwYW5kYXNfdmVyc
-000055b0: 326c 7662 6949 3649 4349 784c 6a55 754d  2lvbiI6ICIxLjUuM
+000055b0: 326c 7662 6949 3649 4349 794c 6a41 754d  2lvbiI6ICIyLjAuM
 000055c0: 794a 3941 4141 4141 4159 4141 4142 7759  yJ9AAAAAAYAAABwY
 000055d0: 5735 6b59 584d 4141 4177 4141 4141 7341  W5kYXMAAAwAAAAsA
 000055e0: 7741 4130 4149 4141 4767 4341 4141 5541  wAA0AIAAGgCAAAUA
 000055f0: 6741 4179 4145 4141 4867 4241 4142 4541  gAAyAEAAHgBAABEA
 00005600: 5141 4138 4141 4141 4b41 4141 4142 6f41  QAA8AAAAKAAAABoA
 00005610: 4141 414e 4141 4141 4151 4141 4141 552f  AAANAAAAAQAAAAU/
 00005620: 662f 2f41 4141 4241 7841 4141 4141 5941  f//AAABAxAAAAAYA
@@ -1442,11 +1442,11 @@
 00005a10: 4177 4141 4141 5141 4241 4141 4141 4141  AwAAAAQABAAAAAAA
 00005a20: 4145 4345 4141 4141 4351 4141 4141 4541  AECEAAAACQAAAAEA
 00005a30: 4141 4141 4141 4141 4173 4141 4142 4262  AAAAAAAAAsAAABBb
 00005a40: 5739 3162 6e52 5463 4756 7564 4141 4941  W91bnRTcGVudAAIA
 00005a50: 4177 4143 4141 4841 4167 4141 4141 4141  AwACAAHAAgAAAAAA
 00005a60: 4141 4249 4141 4141 413d 3d00 1820 7061  AABIAAAAA==.. pa
 00005a70: 7271 7565 742d 6370 702d 6172 726f 7720  rquet-cpp-arrow 
-00005a80: 7665 7273 696f 6e20 3130 2e30 2e31 19cc  version 10.0.1..
+00005a80: 7665 7273 696f 6e20 3132 2e30 2e30 19cc  version 12.0.0..
 00005a90: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00005aa0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00005ab0: 001c 0000 00f0 1b00 0050 4152 31         .........PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.9.2/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/dvd.parquet` & `pyrsm-0.9.2/pyrsm/data/model/dvd.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -2370,17 +2370,17 @@
 00009410: 6169 6e69 6e67 222c 2022 7061 6e64 6173  aining", "pandas
 00009420: 5f74 7970 6522 3a20 2269 6e74 3332 222c  _type": "int32",
 00009430: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
 00009440: 696e 7433 3222 2c20 226d 6574 6164 6174  int32", "metadat
 00009450: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00009460: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00009470: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00009480: 6572 7369 6f6e 223a 2022 3130 2e30 2e31  ersion": "10.0.1
+00009480: 6572 7369 6f6e 223a 2022 3132 2e30 2e31  ersion": "12.0.1
 00009490: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-000094a0: 696f 6e22 3a20 2231 2e35 2e33 227d 0018  ion": "1.5.3"}..
+000094a0: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
 000094b0: 0c41 5252 4f57 3a73 6368 656d 6118 800e  .ARROW:schema...
 000094c0: 2f2f 2f2f 2f7a 6746 4141 4151 4141 4141  /////zgFAAAQAAAA
 000094d0: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 000094e0: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 000094f0: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 00009500: 4367 4141 414d 4144 4141 4145 4141 4141  CgAAAMADAAAEAAAA
 00009510: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -2454,17 +2454,17 @@
 00009950: 6556 3930 6558 426c 496a 6f67 496d 6c75  eV90eXBlIjogImlu
 00009960: 6444 4d79 4969 7767 496d 316c 6447 466b  dDMyIiwgIm1ldGFk
 00009970: 5958 5268 496a 6f67 626e 5673 6248 3164  YXRhIjogbnVsbH1d
 00009980: 4c43 4169 5933 4a6c 5958 5276 6369 4936  LCAiY3JlYXRvciI6
 00009990: 4948 7369 6247 6c69 636d 4679 6553 4936  IHsibGlicmFyeSI6
 000099a0: 4943 4a77 6557 4679 636d 3933 4969 7767  ICJweWFycm93Iiwg
 000099b0: 496e 5a6c 636e 4e70 6232 3469 4f69 4169  InZlcnNpb24iOiAi
-000099c0: 4d54 4175 4d43 3478 496e 3073 4943 4a77  MTAuMC4xIn0sICJw
+000099c0: 4d54 4975 4d43 3478 496e 3073 4943 4a77  MTIuMC4xIn0sICJw
 000099d0: 5957 356b 5958 4e66 646d 5679 6332 6c76  YW5kYXNfdmVyc2lv
-000099e0: 6269 4936 4943 4978 4c6a 5575 4d79 4a39  biI6ICIxLjUuMyJ9
+000099e0: 6269 4936 4943 4979 4c6a 4175 4d79 4a39  biI6ICIyLjAuMyJ9
 000099f0: 4141 4141 4141 5941 4141 4277 5957 356b  AAAAAAYAAABwYW5k
 00009a00: 5958 4d41 4141 5541 4141 4434 4141 4141  YXMAAAUAAAD4AAAA
 00009a10: 7441 4141 4148 4141 4141 4138 4141 4141  tAAAAHAAAAA8AAAA
 00009a20: 4241 4141 4147 7a2f 2f2f 3841 4141 4543  BAAAAGz///8AAAEC
 00009a30: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
 00009a40: 4141 4141 4141 6741 4141 4230 636d 4670  AAAAAAgAAAB0cmFp
 00009a50: 626d 6c75 5a77 4141 4141 4151 2f2f 2f2f  bmluZwAAAAAQ////
@@ -2487,10 +2487,10 @@
 00009b60: 4641 4141 4145 4141 4141 4163 4141 4141  FAAAAEAAAAAcAAAA
 00009b70: 4241 4141 4141 4141 4141 4144 4141 4141  BAAAAAAAAAADAAAA
 00009b80: 596e 5635 4141 6741 4341 4141 4141 5141  YnV5AAgACAAAAAQA
 00009b90: 4341 4141 4141 7741 4141 4149 4141 7741  CAAAAAwAAAAIAAwA
 00009ba0: 4341 4148 4141 6741 4141 4141 4141 4142  CAAHAAgAAAAAAAAB
 00009bb0: 4341 4141 4141 5141 4241 4145 4141 4141  CAAAAAQABAAEAAAA
 00009bc0: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-00009bd0: 7272 6f77 2076 6572 7369 6f6e 2031 302e  rrow version 10.
-00009be0: 302e 3119 5c1c 0000 1c00 001c 0000 1c00  0.1.\...........
+00009bd0: 7272 6f77 2076 6572 7369 6f6e 2031 322e  rrow version 12.
+00009be0: 302e 3019 5c1c 0000 1c00 001c 0000 1c00  0.0.\...........
 00009bf0: 001c 0000 00e6 0c00 0050 4152 31         .........PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/dvd_description.md` & `pyrsm-0.9.2/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.9.2/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.9.2/pyrsm/data/model/houseprices.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,17 @@
 00000e10: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
 00000e20: 7438 222c 2022 6d65 7461 6461 7461 223a  t8", "metadata":
 00000e30: 207b 226e 756d 5f63 6174 6567 6f72 6965   {"num_categorie
 00000e40: 7322 3a20 332c 2022 6f72 6465 7265 6422  s": 3, "ordered"
 00000e50: 3a20 6661 6c73 657d 7d5d 2c20 2263 7265  : false}}], "cre
 00000e60: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00000e70: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00000e80: 6572 7369 6f6e 223a 2022 3130 2e30 2e31  ersion": "10.0.1
+00000e80: 6572 7369 6f6e 223a 2022 3132 2e30 2e31  ersion": "12.0.1
 00000e90: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00000ea0: 696f 6e22 3a20 2231 2e35 2e33 227d 0018  ion": "1.5.3"}..
+00000ea0: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
 00000eb0: 0c41 5252 4f57 3a73 6368 656d 6118 8011  .ARROW:schema...
 00000ec0: 2f2f 2f2f 2f31 6747 4141 4155 4141 4141  /////1gGAAAUAAAA
 00000ed0: 4141 4141 4141 4141 4367 414f 4141 5941  AAAAAAAACgAOAAYA
 00000ee0: 4251 4149 4141 6f41 4141 4141 4151 5141  BQAIAAoAAAAAAQQA
 00000ef0: 4541 4141 4141 4141 4367 414d 4141 4141  EAAAAAAACgAMAAAA
 00000f00: 4241 4149 4141 6f41 4141 4230 4241 4141  BAAIAAoAAAB0BAAA
 00000f10: 4241 4141 4141 4541 4141 414d 4141 4141  BAAAAAEAAAAMAAAA
@@ -325,18 +325,18 @@
 00001440: 6579 4a75 6457 3166 5932 4630 5a57 6476  eyJudW1fY2F0ZWdv
 00001450: 636d 6c6c 6379 4936 4944 4d73 4943 4a76  cmllcyI6IDMsICJv
 00001460: 636d 526c 636d 566b 496a 6f67 5a6d 4673  cmRlcmVkIjogZmFs
 00001470: 6332 5639 6656 3073 4943 4a6a 636d 5668  c2V9fV0sICJjcmVh
 00001480: 6447 3979 496a 6f67 6579 4a73 6157 4a79  dG9yIjogeyJsaWJy
 00001490: 5958 4a35 496a 6f67 496e 4235 5958 4a79  YXJ5IjogInB5YXJy
 000014a0: 6233 6369 4c43 4169 646d 5679 6332 6c76  b3ciLCAidmVyc2lv
-000014b0: 6269 4936 4943 4978 4d43 3477 4c6a 4569  biI6ICIxMC4wLjEi
+000014b0: 6269 4936 4943 4978 4d69 3477 4c6a 4569  biI6ICIxMi4wLjEi
 000014c0: 6653 7767 496e 4268 626d 5268 6331 3932  fSwgInBhbmRhc192
-000014d0: 5a58 4a7a 6157 3975 496a 6f67 496a 4575  ZXJzaW9uIjogIjEu
-000014e0: 4e53 347a 496e 3041 4141 4147 4141 4141  NS4zIn0AAAAGAAAA
+000014d0: 5a58 4a7a 6157 3975 496a 6f67 496a 4975  ZXJzaW9uIjogIjIu
+000014e0: 4d43 347a 496e 3041 4141 4147 4141 4141  MC4zIn0AAAAGAAAA
 000014f0: 6347 4675 5a47 467a 4141 4147 4141 4141  cGFuZGFzAAAGAAAA
 00001500: 6541 4541 4144 4142 4141 4434 4141 4141  eAEAADABAAD4AAAA
 00001510: 7741 4141 4148 4141 4141 4145 4141 4141  wAAAAHAAAAAEAAAA
 00001520: 7150 2f2f 2f77 4141 4151 5555 4141 4141  qP///wAAAQUUAAAA
 00001530: 5341 4141 4143 6741 4141 4145 4141 4141  SAAAACgAAAAEAAAA
 00001540: 4141 4141 4141 7741 4141 4275 5a57 6c6e  AAAAAAwAAABuZWln
 00001550: 6147 4a76 636d 6876 6232 5141 4141 4141  aGJvcmhvb2QAAAAA
@@ -367,10 +367,10 @@
 000016e0: 4541 4155 4141 6741 4267 4148 4141 7741  EAAUAAgABgAHAAwA
 000016f0: 4141 4151 4142 4141 4141 4141 4141 4543  AAAQABAAAAAAAAEC
 00001700: 4541 4141 4143 4141 4141 4145 4141 4141  EAAAACAAAAAEAAAA
 00001710: 4141 4141 4141 5541 4141 4277 636d 6c6a  AAAAAAUAAABwcmlj
 00001720: 5a51 4141 4141 6741 4441 4149 4141 6341  ZQAAAAgADAAIAAcA
 00001730: 4341 4141 4141 4141 4141 4567 4141 4141  CAAAAAAAAAEgAAAA
 00001740: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-00001750: 7272 6f77 2076 6572 7369 6f6e 2031 302e  rrow version 10.
-00001760: 302e 3119 6c1c 0000 1c00 001c 0000 1c00  0.1.l...........
+00001750: 7272 6f77 2076 6572 7369 6f6e 2031 322e  rrow version 12.
+00001760: 302e 3019 6c1c 0000 1c00 001c 0000 1c00  0.0.l...........
 00001770: 001c 0000 1c00 0000 840f 0000 5041 5231  ............PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.9.2/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/ideal.parquet` & `pyrsm-0.9.2/pyrsm/data/model/ideal.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -2431,17 +2431,17 @@
 000097e0: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
 000097f0: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
 00009800: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
 00009810: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
 00009820: 6c6c 7d5d 2c20 2263 7265 6174 6f72 223a  ll}], "creator":
 00009830: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
 00009840: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-00009850: 223a 2022 3130 2e30 2e31 227d 2c20 2270  ": "10.0.1"}, "p
+00009850: 223a 2022 3132 2e30 2e31 227d 2c20 2270  ": "12.0.1"}, "p
 00009860: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00009870: 2231 2e35 2e33 227d 0018 0c41 5252 4f57  "1.5.3"}...ARROW
+00009870: 2232 2e30 2e33 227d 0018 0c41 5252 4f57  "2.0.3"}...ARROW
 00009880: 3a73 6368 656d 6118 800b 2f2f 2f2f 2f78  :schema.../////x
 00009890: 6745 4141 4151 4141 4141 4141 414b 4141  gEAAAQAAAAAAAKAA
 000098a0: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
 000098b0: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
 000098c0: 7741 4141 4145 4141 6741 4367 4141 4143  wAAAAEAAgACgAAAC
 000098d0: 4144 4141 4145 4141 4141 4151 4141 4141  ADAAAEAAAAAQAAAA
 000098e0: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
@@ -2501,17 +2501,17 @@
 00009c40: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
 00009c50: 5a73 6232 4630 4e6a 5169 4c43 4169 6257  Zsb2F0NjQiLCAibW
 00009c60: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
 00009c70: 7873 6656 3073 4943 4a6a 636d 5668 6447  xsfV0sICJjcmVhdG
 00009c80: 3979 496a 6f67 6579 4a73 6157 4a79 5958  9yIjogeyJsaWJyYX
 00009c90: 4a35 496a 6f67 496e 4235 5958 4a79 6233  J5IjogInB5YXJyb3
 00009ca0: 6369 4c43 4169 646d 5679 6332 6c76 6269  ciLCAidmVyc2lvbi
-00009cb0: 4936 4943 4978 4d43 3477 4c6a 4569 6653  I6ICIxMC4wLjEifS
+00009cb0: 4936 4943 4978 4d69 3477 4c6a 4569 6653  I6ICIxMi4wLjEifS
 00009cc0: 7767 496e 4268 626d 5268 6331 3932 5a58  wgInBhbmRhc192ZX
-00009cd0: 4a7a 6157 3975 496a 6f67 496a 4575 4e53  JzaW9uIjogIjEuNS
+00009cd0: 4a7a 6157 3975 496a 6f67 496a 4975 4d43  JzaW9uIjogIjIuMC
 00009ce0: 347a 496e 3041 4141 4141 4267 4141 4148  4zIn0AAAAABgAAAH
 00009cf0: 4268 626d 5268 6377 4141 4241 4141 414a  BhbmRhcwAABAAAAJ
 00009d00: 6741 4141 4263 4141 4141 4d41 4141 4141  gAAABcAAAAMAAAAA
 00009d10: 5141 4141 4349 2f2f 2f2f 4141 4142 4178  QAAACI////AAABAx
 00009d20: 4141 4141 4155 4141 4141 4241 4141 4141  AAAAAUAAAABAAAAA
 00009d30: 4141 4141 4143 4141 4141 6544 4d41 4148  AAAAACAAAAeDMAAH
 00009d40: 722f 2f2f 3841 4141 4941 7350 2f2f 2f77  r///8AAAIAsP///w
@@ -2524,10 +2524,10 @@
 00009db0: 4141 4167 4151 4142 5141 4341 4147 4141  AAAgAQABQACAAGAA
 00009dc0: 6341 4441 4141 4142 4141 4541 4141 4141  cADAAAABAAEAAAAA
 00009dd0: 4141 4151 4d51 4141 4141 4741 4141 4141  AAAQMQAAAAGAAAAA
 00009de0: 5141 4141 4141 4141 4141 4151 4141 4148  QAAAAAAAAAAQAAAH
 00009df0: 6b41 4267 4149 4141 5941 4267 4141 4141  kABgAIAAYABgAAAA
 00009e00: 4141 4167 4141 4141 4141 0018 2070 6172  AAAgAAAAAA.. par
 00009e10: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-00009e20: 6572 7369 6f6e 2031 302e 302e 3119 4c1c  ersion 10.0.1.L.
+00009e20: 6572 7369 6f6e 2031 322e 302e 3019 4c1c  ersion 12.0.0.L.
 00009e30: 0000 1c00 001c 0000 1c00 0000 900a 0000  ................
 00009e40: 5041 5231                                PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.9.2/pyrsm/data/model/ketchup.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -1312,17 +1312,17 @@
 000051f0: 7970 6522 3a20 2269 6e74 3822 2c20 226d  ype": "int8", "m
 00005200: 6574 6164 6174 6122 3a20 7b22 6e75 6d5f  etadata": {"num_
 00005210: 6361 7465 676f 7269 6573 223a 2032 2c20  categories": 2, 
 00005220: 226f 7264 6572 6564 223a 2066 616c 7365  "ordered": false
 00005230: 7d7d 5d2c 2022 6372 6561 746f 7222 3a20  }}], "creator": 
 00005240: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
 00005250: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00005260: 3a20 2231 302e 302e 3122 7d2c 2022 7061  : "10.0.1"}, "pa
+00005260: 3a20 2231 322e 302e 3122 7d2c 2022 7061  : "12.0.1"}, "pa
 00005270: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-00005280: 312e 352e 3322 7d00 180c 4152 524f 573a  1.5.3"}...ARROW:
+00005280: 322e 302e 3322 7d00 180c 4152 524f 573a  2.0.3"}...ARROW:
 00005290: 7363 6865 6d61 18f8 252f 2f2f 2f2f 7a41  schema..%/////zA
 000052a0: 4f41 4141 5541 4141 4141 4141 4141 4141  OAAAUAAAAAAAAAAA
 000052b0: 4143 6741 4f41 4159 4142 5141 4941 416f  ACgAOAAYABQAIAAo
 000052c0: 4141 4141 4141 5151 4145 4141 4141 4141  AAAAAAQQAEAAAAAA
 000052d0: 4143 6741 4d41 4141 4142 4141 4941 416f  ACgAMAAAABAAIAAo
 000052e0: 4141 4143 6b43 5141 4142 4141 4141 4145  AAACkCQAABAAAAAE
 000052f0: 4141 4141 4d41 4141 4143 4141 4d41 4151  AAAAMAAAACAAMAAQ
@@ -1521,18 +1521,18 @@
 00005f00: 3059 5349 3649 4873 6962 6e56 7458 324e  0YSI6IHsibnVtX2N
 00005f10: 6864 4756 6e62 334a 705a 584d 694f 6941  hdGVnb3JpZXMiOiA
 00005f20: 794c 4341 6962 334a 6b5a 584a 6c5a 4349  yLCAib3JkZXJlZCI
 00005f30: 3649 475a 6862 484e 6c66 5831 644c 4341  6IGZhbHNlfX1dLCA
 00005f40: 6959 334a 6c59 5852 7663 6949 3649 4873  iY3JlYXRvciI6IHs
 00005f50: 6962 476c 6963 6d46 7965 5349 3649 434a  ibGlicmFyeSI6ICJ
 00005f60: 7765 5746 7963 6d39 3349 6977 6749 6e5a  weWFycm93IiwgInZ
-00005f70: 6c63 6e4e 7062 3234 694f 6941 694d 5441  lcnNpb24iOiAiMTA
+00005f70: 6c63 6e4e 7062 3234 694f 6941 694d 5449  lcnNpb24iOiAiMTI
 00005f80: 754d 4334 7849 6e30 7349 434a 7759 5735  uMC4xIn0sICJwYW5
 00005f90: 6b59 584e 6664 6d56 7963 326c 7662 6949  kYXNfdmVyc2lvbiI
-00005fa0: 3649 4349 784c 6a55 754d 794a 3941 4159  6ICIxLjUuMyJ9AAY
+00005fa0: 3649 4349 794c 6a41 754d 794a 3941 4159  6ICIyLjAuMyJ9AAY
 00005fb0: 4141 4142 7759 5735 6b59 584d 4141 4134  AAABwYW5kYXMAAA4
 00005fc0: 4141 4141 4942 4141 4170 414d 4141 4767  AAAAIBAAApAMAAGg
 00005fd0: 4441 4141 6741 7741 4136 4149 4141 4c41  DAAAgAwAA6AIAALA
 00005fe0: 4341 4142 5141 6741 412f 4145 4141 4b67  CAABQAgAA/AEAAKg
 00005ff0: 4241 4142 5541 5141 4141 4145 4141 4b77  BAABUAQAAAAEAAKw
 00006000: 4141 4142 5941 4141 4142 4141 4141 4544  AAABYAAAABAAAAED
 00006010: 382f 2f38 4141 4145 4646 4141 4141 4541  8//8AAAEFFAAAAEA
@@ -1620,12 +1620,12 @@
 00006530: 4141 4142 4141 4141 4148 4141 4141 4151  AAABAAAAAHAAAAAQ
 00006540: 4141 4141 4141 4141 4141 6741 4141 476c  AAAAAAAAAAgAAAGl
 00006550: 6b41 4141 4941 4167 4141 4141 4541 4167  kAAAIAAgAAAAEAAg
 00006560: 4141 4141 4d41 4141 4143 4141 4d41 4167  AAAAMAAAACAAMAAg
 00006570: 4142 7741 4941 4141 4141 4141 4141 5241  ABwAIAAAAAAAAARA
 00006580: 4141 4141 4541 4151 4142 4141 4141 413d  AAAAEAAQABAAAAA=
 00006590: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-000065a0: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-000065b0: 2e30 2e31 19ec 1c00 001c 0000 1c00 001c  .0.1............
+000065a0: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+000065b0: 2e30 2e30 19ec 1c00 001c 0000 1c00 001c  .0.0............
 000065c0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 000065d0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 000065e0: 00dc 2200 0050 4152 31                   .."..PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.9.2/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/model/ratings.parquet` & `pyrsm-0.9.2/pyrsm/data/model/ratings.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,17 @@
 00000770: 7261 696e 696e 6722 2c20 2270 616e 6461  raining", "panda
 00000780: 735f 7479 7065 223a 2022 696e 7433 3222  s_type": "int32"
 00000790: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
 000007a0: 2269 6e74 3332 222c 2022 6d65 7461 6461  "int32", "metada
 000007b0: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
 000007c0: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 000007d0: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-000007e0: 7665 7273 696f 6e22 3a20 2231 302e 302e  version": "10.0.
+000007e0: 7665 7273 696f 6e22 3a20 2231 322e 302e  version": "12.0.
 000007f0: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-00000800: 7369 6f6e 223a 2022 312e 352e 3322 7d00  sion": "1.5.3"}.
+00000800: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
 00000810: 180c 4152 524f 573a 7363 6865 6d61 18a0  ..ARROW:schema..
 00000820: 0d2f 2f2f 2f2f 2f41 4541 4141 5141 4141  .//////AEAAAQAAA
 00000830: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
 00000840: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
 00000850: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
 00000860: 4143 6741 4141 4951 4441 4141 4541 4141  ACgAAAIQDAAAEAAA
 00000870: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
@@ -199,17 +199,17 @@
 00000c60: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
 00000c70: 6749 6d6c 7564 444d 7949 6977 6749 6d31  gImludDMyIiwgIm1
 00000c80: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
 00000c90: 7362 4831 644c 4341 6959 334a 6c59 5852  sbH1dLCAiY3JlYXR
 00000ca0: 7663 6949 3649 4873 6962 476c 6963 6d46  vciI6IHsibGlicmF
 00000cb0: 7965 5349 3649 434a 7765 5746 7963 6d39  yeSI6ICJweWFycm9
 00000cc0: 3349 6977 6749 6e5a 6c63 6e4e 7062 3234  3IiwgInZlcnNpb24
-00000cd0: 694f 6941 694d 5441 754d 4334 7849 6e30  iOiAiMTAuMC4xIn0
+00000cd0: 694f 6941 694d 5449 754d 4334 7849 6e30  iOiAiMTIuMC4xIn0
 00000ce0: 7349 434a 7759 5735 6b59 584e 6664 6d56  sICJwYW5kYXNfdmV
-00000cf0: 7963 326c 7662 6949 3649 4349 784c 6a55  yc2lvbiI6ICIxLjU
+00000cf0: 7963 326c 7662 6949 3649 4349 794c 6a41  yc2lvbiI6ICIyLjA
 00000d00: 754d 794a 3941 4159 4141 4142 7759 5735  uMyJ9AAYAAABwYW5
 00000d10: 6b59 584d 4141 4151 4141 4144 6f41 4141  kYXMAAAQAAADoAAA
 00000d20: 4167 4141 4141 4577 4141 4141 4541 4141  AgAAAAEwAAAAEAAA
 00000d30: 417a 502f 2f2f 7741 4141 5149 5141 4141  AzP///wAAAQIQAAA
 00000d40: 4148 4141 4141 4151 4141 4141 4141 4141  AHAAAAAQAAAAAAAA
 00000d50: 4143 4141 4141 4852 7959 576c 7561 5735  ACAAAAHRyYWluaW5
 00000d60: 6e41 4141 4141 426a 2f2f 2f38 4141 4141  nAAAAABj///8AAAA
@@ -231,10 +231,10 @@
 00000e60: 4152 4141 4141 4341 4141 4141 4541 4141  ARAAAACAAAAAEAAA
 00000e70: 4141 4141 4141 4155 4141 4142 5663 3256  AAAAAAAUAAABVc2V
 00000e80: 7963 7741 4141 4167 4143 4141 4141 4151  ycwAAAAgACAAAAAQ
 00000e90: 4143 4141 4141 4177 4141 4141 4941 4177  ACAAAAAwAAAAIAAw
 00000ea0: 4143 4141 4841 4167 4141 4141 4141 4141  ACAAHAAgAAAAAAAA
 00000eb0: 4243 4141 4141 4151 4142 4141 4541 4141  BCAAAAAQABAAEAAA
 00000ec0: 4100 1820 7061 7271 7565 742d 6370 702d  A.. parquet-cpp-
-00000ed0: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-00000ee0: 2e30 2e31 194c 1c00 001c 0000 1c00 001c  .0.1.L..........
+00000ed0: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+00000ee0: 2e30 2e30 194c 1c00 001c 0000 1c00 001c  .0.0.L..........
 00000ef0: 0000 00d5 0b00 0050 4152 31              .......PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/titanic.parquet` & `pyrsm-0.9.2/pyrsm/data/data/titanic.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -1845,16 +1845,16 @@
 00007340: 223a 2022 696e 7438 222c 2022 6d65 7461  ": "int8", "meta
 00007350: 6461 7461 223a 207b 226e 756d 5f63 6174  data": {"num_cat
 00007360: 6567 6f72 6965 7322 3a20 332c 2022 6f72  egories": 3, "or
 00007370: 6465 7265 6422 3a20 6661 6c73 657d 7d5d  dered": false}}]
 00007380: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
 00007390: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
 000073a0: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-000073b0: 3130 2e30 2e31 227d 2c20 2270 616e 6461  10.0.1"}, "panda
-000073c0: 735f 7665 7273 696f 6e22 3a20 2231 2e35  s_version": "1.5
+000073b0: 3132 2e30 2e31 227d 2c20 2270 616e 6461  12.0.1"}, "panda
+000073c0: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
 000073d0: 2e33 227d 0018 0c41 5252 4f57 3a73 6368  .3"}...ARROW:sch
 000073e0: 656d 6118 c018 2f2f 2f2f 2f79 674a 4141  ema.../////ygJAA
 000073f0: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
 00007400: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
 00007410: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
 00007420: 4145 4141 6741 4367 4141 4146 7747 4141  AEAAgACgAAAFwGAA
 00007430: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
@@ -1984,17 +1984,17 @@
 00007bf0: 3166 5932 4630 5a57 6476 636d 6c6c 6379  1fY2F0ZWdvcmllcy
 00007c00: 4936 4944 4d73 4943 4a76 636d 526c 636d  I6IDMsICJvcmRlcm
 00007c10: 566b 496a 6f67 5a6d 4673 6332 5639 6656  VkIjogZmFsc2V9fV
 00007c20: 3073 4943 4a6a 636d 5668 6447 3979 496a  0sICJjcmVhdG9yIj
 00007c30: 6f67 6579 4a73 6157 4a79 5958 4a35 496a  ogeyJsaWJyYXJ5Ij
 00007c40: 6f67 496e 4235 5958 4a79 6233 6369 4c43  ogInB5YXJyb3ciLC
 00007c50: 4169 646d 5679 6332 6c76 6269 4936 4943  AidmVyc2lvbiI6IC
-00007c60: 4978 4d43 3477 4c6a 4569 6653 7767 496e  IxMC4wLjEifSwgIn
+00007c60: 4978 4d69 3477 4c6a 4569 6653 7767 496e  IxMi4wLjEifSwgIn
 00007c70: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-00007c80: 3975 496a 6f67 496a 4575 4e53 347a 496e  9uIjogIjEuNS4zIn
+00007c80: 3975 496a 6f67 496a 4975 4d43 347a 496e  9uIjogIjIuMC4zIn
 00007c90: 3041 4141 4141 4267 4141 4148 4268 626d  0AAAAABgAAAHBhbm
 00007ca0: 5268 6377 4141 4367 4141 4145 6743 4141  RhcwAACgAAAEgCAA
 00007cb0: 4463 4151 4141 6b41 4541 4146 7742 4141  DcAQAAkAEAAFwBAA
 00007cc0: 4159 4151 4141 3541 4141 414c 5141 4141  AYAQAA5AAAALQAAA
 00007cd0: 4349 4141 4141 5841 4141 4141 5141 4141  CIAAAAXAAAAAQAAA
 00007ce0: 4477 2f66 2f2f 4141 4142 4252 5141 4141  Dw/f//AAABBRQAAA
 00007cf0: 4245 4141 4141 4a41 4141 4141 5141 4141  BEAAAAJAAAAAQAAA
@@ -2046,11 +2046,11 @@
 00007fd0: 4145 4141 4141 4141 4141 4141 5941 4141  AEAAAAAAAAAAYAAA
 00007fe0: 4277 5932 7868 6333 4d41 4141 6741 4341  BwY2xhc3MAAAgACA
 00007ff0: 4141 4141 5141 4341 4141 4141 7741 4141  AAAAQACAAAAAwAAA
 00008000: 4149 4141 7741 4341 4148 4141 6741 4141  AIAAwACAAHAAgAAA
 00008010: 4141 4141 4142 4341 4141 4141 5141 4241  AAAAABCAAAAAQABA
 00008020: 4145 4141 4141 0018 2070 6172 7175 6574  AEAAAA.. parquet
 00008030: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-00008040: 6f6e 2031 302e 302e 3119 ac1c 0000 1c00  on 10.0.1.......
+00008040: 6f6e 2031 322e 302e 3019 ac1c 0000 1c00  on 12.0.0.......
 00008050: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00008060: 1c00 001c 0000 1c00 0000 cd16 0000 5041  ..............PA
 00008070: 5231                                     R1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/model/titanic_description.md` & `pyrsm-0.9.2/pyrsm/data/model/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/carpet.parquet`

 * *Files 4% similar despite different names*

```diff
@@ -163,17 +163,17 @@
 00000a20: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
 00000a30: 2022 696e 7433 3222 2c20 226e 756d 7079   "int32", "numpy
 00000a40: 5f74 7970 6522 3a20 2269 6e74 3332 222c  _type": "int32",
 00000a50: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
 00000a60: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
 00000a70: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
 00000a80: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00000a90: 3a20 2231 302e 302e 3122 7d2c 2022 7061  : "10.0.1"}, "pa
+00000a90: 3a20 2231 322e 302e 3122 7d2c 2022 7061  : "12.0.1"}, "pa
 00000aa0: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-00000ab0: 312e 352e 3322 7d00 180c 4152 524f 573a  1.5.3"}...ARROW:
+00000ab0: 322e 302e 3322 7d00 180c 4152 524f 573a  2.0.3"}...ARROW:
 00000ac0: 7363 6865 6d61 18d8 122f 2f2f 2f2f 2f67  schema...//////g
 00000ad0: 4741 4141 5141 4141 4141 4141 4b41 4134  GAAAQAAAAAAAKAA4
 00000ae0: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
 00000af0: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
 00000b00: 4141 4141 4541 4167 4143 6741 4141 4e51  AAAAEAAgACgAAANQ
 00000b10: 4541 4141 4541 4141 4141 5141 4141 4177  EAAAEAAAAAQAAAAw
 00000b20: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
@@ -269,18 +269,18 @@
 000010c0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
 000010d0: 6c49 6a6f 6749 6d6c 7564 444d 7949 6977  lIjogImludDMyIiw
 000010e0: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
 000010f0: 6762 6e56 7362 4831 644c 4341 6959 334a  gbnVsbH1dLCAiY3J
 00001100: 6c59 5852 7663 6949 3649 4873 6962 476c  lYXRvciI6IHsibGl
 00001110: 6963 6d46 7965 5349 3649 434a 7765 5746  icmFyeSI6ICJweWF
 00001120: 7963 6d39 3349 6977 6749 6e5a 6c63 6e4e  ycm93IiwgInZlcnN
-00001130: 7062 3234 694f 6941 694d 5441 754d 4334  pb24iOiAiMTAuMC4
+00001130: 7062 3234 694f 6941 694d 5449 754d 4334  pb24iOiAiMTIuMC4
 00001140: 7849 6e30 7349 434a 7759 5735 6b59 584e  xIn0sICJwYW5kYXN
 00001150: 6664 6d56 7963 326c 7662 6949 3649 4349  fdmVyc2lvbiI6ICI
-00001160: 784c 6a55 754d 794a 3941 4141 4141 4159  xLjUuMyJ9AAAAAAY
+00001160: 794c 6a41 754d 794a 3941 4141 4141 4159  yLjAuMyJ9AAAAAAY
 00001170: 4141 4142 7759 5735 6b59 584d 4141 4159  AAABwYW5kYXMAAAY
 00001180: 4141 4143 6741 5141 414f 4145 4141 4f51  AAACgAQAAOAEAAOQ
 00001190: 4141 4143 5941 4141 4153 4141 4141 4251  AAACYAAAASAAAABQ
 000011a0: 4141 4141 5141 4251 4143 4141 4741 4163  AAAAQABQACAAGAAc
 000011b0: 4144 4141 4141 4241 4145 4141 4141 4141  ADAAAABAAEAAAAAA
 000011c0: 4141 5149 5141 4141 4147 4141 4141 4151  AAQIQAAAAGAAAAAQ
 000011d0: 4141 4141 4141 4141 4142 7741 4141 484a  AAAAAAAAABwAAAHJ
@@ -317,11 +317,11 @@
 000013c0: 4141 4141 6741 4141 4142 4141 4141 4141  AAAAgAAAABAAAAAA
 000013d0: 4141 4141 4741 4141 415a 4756 7a61 5764  AAAAGAAAAZGVzaWd
 000013e0: 7541 4141 4941 4167 4141 4141 4541 4167  uAAAIAAgAAAAEAAg
 000013f0: 4141 4141 4d41 4141 4143 4141 4d41 4167  AAAAMAAAACAAMAAg
 00001400: 4142 7741 4941 4141 4141 4141 4141 5167  ABwAIAAAAAAAAAQg
 00001410: 4141 4141 4541 4151 4142 4141 4141 413d  AAAAEAAQABAAAAA=
 00001420: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-00001430: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-00001440: 2e30 2e31 196c 1c00 001c 0000 1c00 001c  .0.1.l..........
+00001430: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+00001440: 2e30 2e30 196c 1c00 001c 0000 1c00 001c  .0.0.l..........
 00001450: 0000 1c00 001c 0000 0081 1000 0050 4152  .............PAR
 00001460: 31                                       1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/city.parquet`

 * *Files 5% similar despite different names*

```diff
@@ -103,16 +103,16 @@
 00000660: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
 00000670: 6e74 3332 222c 2022 6e75 6d70 795f 7479  nt32", "numpy_ty
 00000680: 7065 223a 2022 696e 7433 3222 2c20 226d  pe": "int32", "m
 00000690: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
 000006a0: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
 000006b0: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
 000006c0: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-000006d0: 3130 2e30 2e31 227d 2c20 2270 616e 6461  10.0.1"}, "panda
-000006e0: 735f 7665 7273 696f 6e22 3a20 2231 2e35  s_version": "1.5
+000006d0: 3132 2e30 2e31 227d 2c20 2270 616e 6461  12.0.1"}, "panda
+000006e0: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
 000006f0: 2e33 227d 0018 0c41 5252 4f57 3a73 6368  .3"}...ARROW:sch
 00000700: 656d 6118 d809 2f2f 2f2f 2f35 6744 4141  ema.../////5gDAA
 00000710: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
 00000720: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
 00000730: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
 00000740: 4145 4141 6741 4367 4141 414d 4143 4141  AEAAgACgAAAMACAA
 00000750: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
@@ -165,17 +165,17 @@
 00000a40: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
 00000a50: 6c75 6444 4d79 4969 7767 496d 316c 6447  ludDMyIiwgIm1ldG
 00000a60: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
 00000a70: 3164 4c43 4169 5933 4a6c 5958 5276 6369  1dLCAiY3JlYXRvci
 00000a80: 4936 4948 7369 6247 6c69 636d 4679 6553  I6IHsibGlicmFyeS
 00000a90: 4936 4943 4a77 6557 4679 636d 3933 4969  I6ICJweWFycm93Ii
 00000aa0: 7767 496e 5a6c 636e 4e70 6232 3469 4f69  wgInZlcnNpb24iOi
-00000ab0: 4169 4d54 4175 4d43 3478 496e 3073 4943  AiMTAuMC4xIn0sIC
+00000ab0: 4169 4d54 4975 4d43 3478 496e 3073 4943  AiMTIuMC4xIn0sIC
 00000ac0: 4a77 5957 356b 5958 4e66 646d 5679 6332  JwYW5kYXNfdmVyc2
-00000ad0: 6c76 6269 4936 4943 4978 4c6a 5575 4d79  lvbiI6ICIxLjUuMy
+00000ad0: 6c76 6269 4936 4943 4979 4c6a 4175 4d79  lvbiI6ICIyLjAuMy
 00000ae0: 4a39 4141 4141 4267 4141 4148 4268 626d  J9AAAABgAAAHBhbm
 00000af0: 5268 6377 4141 4177 4141 4148 7741 4141  RhcwAAAwAAAHwAAA
 00000b00: 4245 4141 4141 4241 4141 414b 442f 2f2f  BEAAAABAAAAKD///
 00000b10: 3841 4141 4543 4541 4141 4143 5141 4141  8AAAECEAAAACQAAA
 00000b20: 4145 4141 4141 4141 4141 4141 6741 4141  AEAAAAAAAAAAgAAA
 00000b30: 426b 6158 4e30 5957 356a 5a51 4141 4141  BkaXN0YW5jZQAAAA
 00000b40: 4149 4141 7741 4341 4148 4141 6741 4141  AIAAwACAAHAAgAAA
@@ -185,10 +185,10 @@
 00000b80: 4230 6277 4141 7950 2f2f 2f78 4141 4641  B0bwAAyP///xAAFA
 00000b90: 4149 4141 5941 4277 414d 4141 4141 4541  AIAAYABwAMAAAAEA
 00000ba0: 4151 4141 4141 4141 4142 4252 4141 4141  AQAAAAAAABBRAAAA
 00000bb0: 4163 4141 4141 4241 4141 4141 4141 4141  AcAAAABAAAAAAAAA
 00000bc0: 4145 4141 4141 5a6e 4a76 6251 4141 4141  AEAAAAZnJvbQAAAA
 00000bd0: 4145 4141 5141 4241 4141 4141 3d3d 0018  AEAAQABAAAAA==..
 00000be0: 2070 6172 7175 6574 2d63 7070 2d61 7272   parquet-cpp-arr
-00000bf0: 6f77 2076 6572 7369 6f6e 2031 302e 302e  ow version 10.0.
-00000c00: 3119 3c1c 0000 1c00 001c 0000 00e5 0800  1.<.............
+00000bf0: 6f77 2076 6572 7369 6f6e 2031 322e 302e  ow version 12.0.
+00000c00: 3019 3c1c 0000 1c00 001c 0000 00e5 0800  0.<.............
 00000c10: 0050 4152 31                             .PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/city2.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
 00000a80: 6173 5f74 7970 6522 3a20 2275 6e69 636f  as_type": "unico
 00000a90: 6465 222c 2022 6e75 6d70 795f 7479 7065  de", "numpy_type
 00000aa0: 223a 2022 6f62 6a65 6374 222c 2022 6d65  ": "object", "me
 00000ab0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 00000ac0: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 00000ad0: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 00000ae0: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00000af0: 302e 302e 3122 7d2c 2022 7061 6e64 6173  0.0.1"}, "pandas
-00000b00: 5f76 6572 7369 6f6e 223a 2022 312e 352e  _version": "1.5.
+00000af0: 322e 302e 3122 7d2c 2022 7061 6e64 6173  2.0.1"}, "pandas
+00000b00: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
 00000b10: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
 00000b20: 6d61 1880 0b2f 2f2f 2f2f 7867 4541 4141  ma.../////xgEAAA
 00000b30: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00000b40: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 00000b50: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 00000b60: 4541 4167 4143 6741 4141 4167 4441 4141  EAAgACgAAAAgDAAA
 00000b70: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
@@ -237,17 +237,17 @@
 00000ec0: 3558 3352 3563 4755 694f 6941 6962 324a  5X3R5cGUiOiAib2J
 00000ed0: 715a 574e 3049 6977 6749 6d31 6c64 4746  qZWN0IiwgIm1ldGF
 00000ee0: 6b59 5852 6849 6a6f 6762 6e56 7362 4831  kYXRhIjogbnVsbH1
 00000ef0: 644c 4341 6959 334a 6c59 5852 7663 6949  dLCAiY3JlYXRvciI
 00000f00: 3649 4873 6962 476c 6963 6d46 7965 5349  6IHsibGlicmFyeSI
 00000f10: 3649 434a 7765 5746 7963 6d39 3349 6977  6ICJweWFycm93Iiw
 00000f20: 6749 6e5a 6c63 6e4e 7062 3234 694f 6941  gInZlcnNpb24iOiA
-00000f30: 694d 5441 754d 4334 7849 6e30 7349 434a  iMTAuMC4xIn0sICJ
+00000f30: 694d 5449 754d 4334 7849 6e30 7349 434a  iMTIuMC4xIn0sICJ
 00000f40: 7759 5735 6b59 584e 6664 6d56 7963 326c  wYW5kYXNfdmVyc2l
-00000f50: 7662 6949 3649 4349 784c 6a55 754d 794a  vbiI6ICIxLjUuMyJ
+00000f50: 7662 6949 3649 4349 794c 6a41 754d 794a  vbiI6ICIyLjAuMyJ
 00000f60: 3941 4141 4142 6741 4141 4842 6862 6d52  9AAAABgAAAHBhbmR
 00000f70: 6863 7741 4142 4141 4141 4c51 4141 4142  hcwAABAAAALQAAAB
 00000f80: 3841 4141 4150 4141 4141 4151 4141 4142  8AAAAPAAAAAQAAAB
 00000f90: 732f 2f2f 2f41 4141 4242 5241 4141 4141  s////AAABBRAAAAA
 00000fa0: 6b41 4141 4142 4141 4141 4141 4141 4141  kAAAABAAAAAAAAAA
 00000fb0: 5241 4141 4158 3139 7062 6d52 6c65 4639  RAAAAX19pbmRleF9
 00000fc0: 735a 585a 6c62 4638 7758 3138 4141 4142  sZXZlbF8wX18AAAB
@@ -262,9 +262,9 @@
 00001050: 492f 2f2f 2f45 4141 5541 4167 4142 6741  I////EAAUAAgABgA
 00001060: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
 00001070: 4141 4145 4645 4141 4141 4277 4141 4141  AAAEFEAAAABwAAAA
 00001080: 4541 4141 4141 4141 4141 4151 4141 4142  EAAAAAAAAAAQAAAB
 00001090: 6d63 6d39 7441 4141 4141 4151 4142 4141  mcm9tAAAAAAQABAA
 000010a0: 4541 4141 4100 1820 7061 7271 7565 742d  EAAAA.. parquet-
 000010b0: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
-000010c0: 6e20 3130 2e30 2e31 194c 1c00 001c 0000  n 10.0.1.L......
+000010c0: 6e20 3132 2e30 2e30 194c 1c00 001c 0000  n 12.0.0.L......
 000010d0: 1c00 001c 0000 0045 0a00 0050 4152 31    .......E...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/computer.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -240,17 +240,17 @@
 00000ef0: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
 00000f00: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
 00000f10: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
 00000f20: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
 00000f30: 6c6c 7d5d 2c20 2263 7265 6174 6f72 223a  ll}], "creator":
 00000f40: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
 00000f50: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-00000f60: 223a 2022 3130 2e30 2e31 227d 2c20 2270  ": "10.0.1"}, "p
+00000f60: 223a 2022 3132 2e30 2e31 227d 2c20 2270  ": "12.0.1"}, "p
 00000f70: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000f80: 2231 2e35 2e33 227d 0018 0c41 5252 4f57  "1.5.3"}...ARROW
+00000f80: 2232 2e30 2e33 227d 0018 0c41 5252 4f57  "2.0.3"}...ARROW
 00000f90: 3a73 6368 656d 6118 b812 2f2f 2f2f 2f2b  :schema.../////+
 00000fa0: 4147 4141 4151 4141 4141 4141 414b 4141  AGAAAQAAAAAAAKAA
 00000fb0: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
 00000fc0: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
 00000fd0: 7741 4141 4145 4141 6741 4367 4141 4141  wAAAAEAAgACgAAAA
 00000fe0: 7746 4141 4145 4141 4141 4151 4141 4141  wFAAAEAAAAAQAAAA
 00000ff0: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
@@ -351,18 +351,18 @@
 000015e0: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
 000015f0: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
 00001600: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
 00001610: 3531 6247 7839 5853 7767 496d 4e79 5a57  51bGx9XSwgImNyZW
 00001620: 4630 6233 4969 4f69 4237 496d 7870 596e  F0b3IiOiB7ImxpYn
 00001630: 4a68 636e 6b69 4f69 4169 6348 6c68 636e  JhcnkiOiAicHlhcn
 00001640: 4a76 6479 4973 4943 4a32 5a58 4a7a 6157  JvdyIsICJ2ZXJzaW
-00001650: 3975 496a 6f67 496a 4577 4c6a 4175 4d53  9uIjogIjEwLjAuMS
+00001650: 3975 496a 6f67 496a 4579 4c6a 4175 4d53  9uIjogIjEyLjAuMS
 00001660: 4a39 4c43 4169 6347 4675 5a47 467a 5833  J9LCAicGFuZGFzX3
-00001670: 5a6c 636e 4e70 6232 3469 4f69 4169 4d53  ZlcnNpb24iOiAiMS
-00001680: 3431 4c6a 4d69 6651 4141 4267 4141 4148  41LjMifQAABgAAAH
+00001670: 5a6c 636e 4e70 6232 3469 4f69 4169 4d69  ZlcnNpb24iOiAiMi
+00001680: 3477 4c6a 4d69 6651 4141 4267 4141 4148  4wLjMifQAABgAAAH
 00001690: 4268 626d 5268 6377 4141 4341 4141 4148  BhbmRhcwAACAAAAH
 000016a0: 5142 4141 4173 4151 4141 2f41 4141 414d  QBAAAsAQAA/AAAAM
 000016b0: 7741 4141 4363 4141 4141 6241 4141 4144  wAAACcAAAAbAAAAD
 000016c0: 6741 4141 4145 4141 4141 7650 372f 2f77  gAAAAEAAAAvP7//w
 000016d0: 4141 4151 4d51 4141 4141 4841 4141 4141  AAAQMQAAAAHAAAAA
 000016e0: 5141 4141 4141 4141 4141 4341 4141 4147  QAAAAAAAAACAAAAG
 000016f0: 4a31 6332 6c75 5a58 4e7a 4141 4141 4150  J1c2luZXNzAAAAAP
@@ -393,10 +393,10 @@
 00001880: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
 00001890: 4141 4141 4141 4141 4546 4541 4141 4142  AAAAAAAAEFEAAAAB
 000018a0: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
 000018b0: 5541 4141 4269 636d 4675 5a41 4141 4141  UAAABicmFuZAAAAA
 000018c0: 5141 4241 4145 4141 4141 4141 4141 4141  QABAAEAAAAAAAAAA
 000018d0: 3d3d 0018 2070 6172 7175 6574 2d63 7070  ==.. parquet-cpp
 000018e0: 2d61 7272 6f77 2076 6572 7369 6f6e 2031  -arrow version 1
-000018f0: 302e 302e 3119 8c1c 0000 1c00 001c 0000  0.0.1...........
+000018f0: 322e 302e 3019 8c1c 0000 1c00 001c 0000  2.0.0...........
 00001900: 1c00 001c 0000 1c00 001c 0000 1c00 0000  ................
 00001910: 0412 0000 5041 5231                      ....PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/movie.parquet`

 * *Files 4% similar despite different names*

```diff
@@ -181,17 +181,17 @@
 00000b40: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
 00000b50: 696e 7438 222c 2022 6d65 7461 6461 7461  int8", "metadata
 00000b60: 223a 207b 226e 756d 5f63 6174 6567 6f72  ": {"num_categor
 00000b70: 6965 7322 3a20 332c 2022 6f72 6465 7265  ies": 3, "ordere
 00000b80: 6422 3a20 6661 6c73 657d 7d5d 2c20 2263  d": false}}], "c
 00000b90: 7265 6174 6f72 223a 207b 226c 6962 7261  reator": {"libra
 00000ba0: 7279 223a 2022 7079 6172 726f 7722 2c20  ry": "pyarrow", 
-00000bb0: 2276 6572 7369 6f6e 223a 2022 3130 2e30  "version": "10.0
+00000bb0: 2276 6572 7369 6f6e 223a 2022 3132 2e30  "version": "12.0
 00000bc0: 2e31 227d 2c20 2270 616e 6461 735f 7665  .1"}, "pandas_ve
-00000bd0: 7273 696f 6e22 3a20 2231 2e35 2e33 227d  rsion": "1.5.3"}
+00000bd0: 7273 696f 6e22 3a20 2232 2e30 2e33 227d  rsion": "2.0.3"}
 00000be0: 0018 0c41 5252 4f57 3a73 6368 656d 6118  ...ARROW:schema.
 00000bf0: e012 2f2f 2f2f 2f77 4148 4141 4151 4141  ../////wAHAAAQAA
 00000c00: 4141 4141 414b 4141 3441 4267 4146 4141  AAAAAKAA4ABgAFAA
 00000c10: 6741 4367 4141 4141 4142 4241 4151 4141  gACgAAAAABBAAQAA
 00000c20: 4141 4141 414b 4141 7741 4141 4145 4141  AAAAAKAAwAAAAEAA
 00000c30: 6741 4367 4141 414e 6745 4141 4145 4141  gACgAAANgEAAAEAA
 00000c40: 4141 4151 4141 4141 7741 4141 4149 4141  AAAQAAAAwAAAAIAA
@@ -288,18 +288,18 @@
 000011f0: 4936 4948 7369 626e 5674 5832 4e68 6447  I6IHsibnVtX2NhdG
 00001200: 566e 6233 4a70 5a58 4d69 4f69 417a 4c43  Vnb3JpZXMiOiAzLC
 00001210: 4169 6233 4a6b 5a58 4a6c 5a43 4936 4947  Aib3JkZXJlZCI6IG
 00001220: 5a68 6248 4e6c 6658 3164 4c43 4169 5933  ZhbHNlfX1dLCAiY3
 00001230: 4a6c 5958 5276 6369 4936 4948 7369 6247  JlYXRvciI6IHsibG
 00001240: 6c69 636d 4679 6553 4936 4943 4a77 6557  licmFyeSI6ICJweW
 00001250: 4679 636d 3933 4969 7767 496e 5a6c 636e  Fycm93IiwgInZlcn
-00001260: 4e70 6232 3469 4f69 4169 4d54 4175 4d43  Npb24iOiAiMTAuMC
+00001260: 4e70 6232 3469 4f69 4169 4d54 4975 4d43  Npb24iOiAiMTIuMC
 00001270: 3478 496e 3073 4943 4a77 5957 356b 5958  4xIn0sICJwYW5kYX
 00001280: 4e66 646d 5679 6332 6c76 6269 4936 4943  NfdmVyc2lvbiI6IC
-00001290: 4978 4c6a 5575 4d79 4a39 4141 4147 4141  IxLjUuMyJ9AAAGAA
+00001290: 4979 4c6a 4175 4d79 4a39 4141 4147 4141  IyLjAuMyJ9AAAGAA
 000012a0: 4141 6347 4675 5a47 467a 4141 4147 4141  AAcGFuZGFzAAAGAA
 000012b0: 4141 7741 4541 4147 4142 4141 4434 4141  AAwAEAAGABAAD4AA
 000012c0: 4141 7041 4141 4146 4141 4141 4145 4141  AApAAAAFAAAAAEAA
 000012d0: 4141 7850 372f 2f77 4141 4151 5555 4141  AAxP7//wAAAQUUAA
 000012e0: 4141 4f41 4141 4142 6741 4141 4145 4141  AAOAAAABgAAAAEAA
 000012f0: 4141 4141 4141 4141 5141 4141 426d 6232  AAAAAAAAQAAABmb2
 00001300: 396b 4141 4141 4147 6a2f 2f2f 384d 4141  9kAAAAAGj///8MAA
@@ -337,10 +337,10 @@
 00001500: 7741 4141 4151 4142 4141 4141 4141 4141  wAAAAQABAAAAAAAA
 00001510: 4543 4541 4141 4143 4141 4141 4145 4141  ECEAAAACAAAAAEAA
 00001520: 4141 4141 4141 4141 6341 4141 4253 5957  AAAAAAAAcAAABSYW
 00001530: 3572 6157 356e 4141 6741 4441 4149 4141  5raW5nAAgADAAIAA
 00001540: 6341 4341 4141 4141 4141 4141 4567 4141  cACAAAAAAAAAEgAA
 00001550: 4141 0018 2070 6172 7175 6574 2d63 7070  AA.. parquet-cpp
 00001560: 2d61 7272 6f77 2076 6572 7369 6f6e 2031  -arrow version 1
-00001570: 302e 302e 3119 6c1c 0000 1c00 001c 0000  0.0.1.l.........
+00001570: 322e 302e 3019 6c1c 0000 1c00 001c 0000  2.0.0.l.........
 00001580: 1c00 001c 0000 1c00 0000 d310 0000 5041  ..............PA
 00001590: 5231                                     R1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/mp3.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,17 @@
 00000a40: 7479 7065 223a 2022 696e 7438 222c 2022  type": "int8", "
 00000a50: 6d65 7461 6461 7461 223a 207b 226e 756d  metadata": {"num
 00000a60: 5f63 6174 6567 6f72 6965 7322 3a20 332c  _categories": 3,
 00000a70: 2022 6f72 6465 7265 6422 3a20 6661 6c73   "ordered": fals
 00000a80: 657d 7d5d 2c20 2263 7265 6174 6f72 223a  e}}], "creator":
 00000a90: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
 00000aa0: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-00000ab0: 223a 2022 3130 2e30 2e31 227d 2c20 2270  ": "10.0.1"}, "p
+00000ab0: 223a 2022 3132 2e30 2e31 227d 2c20 2270  ": "12.0.1"}, "p
 00000ac0: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000ad0: 2231 2e35 2e33 227d 0018 0c41 5252 4f57  "1.5.3"}...ARROW
+00000ad0: 2232 2e30 2e33 227d 0018 0c41 5252 4f57  "2.0.3"}...ARROW
 00000ae0: 3a73 6368 656d 6118 c012 2f2f 2f2f 2f2b  :schema.../////+
 00000af0: 6747 4141 4151 4141 4141 4141 414b 4141  gGAAAQAAAAAAAKAA
 00000b00: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
 00000b10: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
 00000b20: 7741 4141 4145 4141 6741 4367 4141 414d  wAAAAEAAgACgAAAM
 00000b30: 6745 4141 4145 4141 4141 4151 4141 4141  gEAAAEAAAAAQAAAA
 00000b40: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
@@ -270,18 +270,18 @@
 000010d0: 4936 4948 7369 626e 5674 5832 4e68 6447  I6IHsibnVtX2NhdG
 000010e0: 566e 6233 4a70 5a58 4d69 4f69 417a 4c43  Vnb3JpZXMiOiAzLC
 000010f0: 4169 6233 4a6b 5a58 4a6c 5a43 4936 4947  Aib3JkZXJlZCI6IG
 00001100: 5a68 6248 4e6c 6658 3164 4c43 4169 5933  ZhbHNlfX1dLCAiY3
 00001110: 4a6c 5958 5276 6369 4936 4948 7369 6247  JlYXRvciI6IHsibG
 00001120: 6c69 636d 4679 6553 4936 4943 4a77 6557  licmFyeSI6ICJweW
 00001130: 4679 636d 3933 4969 7767 496e 5a6c 636e  Fycm93IiwgInZlcn
-00001140: 4e70 6232 3469 4f69 4169 4d54 4175 4d43  Npb24iOiAiMTAuMC
+00001140: 4e70 6232 3469 4f69 4169 4d54 4975 4d43  Npb24iOiAiMTIuMC
 00001150: 3478 496e 3073 4943 4a77 5957 356b 5958  4xIn0sICJwYW5kYX
 00001160: 4e66 646d 5679 6332 6c76 6269 4936 4943  NfdmVyc2lvbiI6IC
-00001170: 4978 4c6a 5575 4d79 4a39 4141 4141 4141  IxLjUuMyJ9AAAAAA
+00001170: 4979 4c6a 4175 4d79 4a39 4141 4141 4141  IyLjAuMyJ9AAAAAA
 00001180: 5941 4141 4277 5957 356b 5958 4d41 4141  YAAABwYW5kYXMAAA
 00001190: 5941 4141 4334 4151 4141 5741 4541 4150  YAAAC4AQAAWAEAAP
 000011a0: 4141 4141 4363 4141 4141 5541 4141 4141  AAAACcAAAAUAAAAA
 000011b0: 5141 4141 444d 2f76 2f2f 4141 4142 4252  QAAADM/v//AAABBR
 000011c0: 5141 4141 4134 4141 4141 4741 4141 4141  QAAAA4AAAAGAAAAA
 000011d0: 5141 4141 4141 4141 4141 4251 4141 4146  QAAAAAAAAABQAAAF
 000011e0: 4e6f 5958 426c 4141 4141 6350 2f2f 2f77  NoYXBlAAAAcP///w
@@ -318,10 +318,10 @@
 000013d0: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
 000013e0: 4141 4141 4141 4141 4543 4541 4141 4143  AAAAAAAAECEAAAAC
 000013f0: 4141 4141 4145 4141 4141 4141 4141 4141  AAAAAEAAAAAAAAAA
 00001400: 5941 4141 4253 5958 5270 626d 6341 4141  YAAABSYXRpbmcAAA
 00001410: 6741 4441 4149 4141 6341 4341 4141 4141  gADAAIAAcACAAAAA
 00001420: 4141 4141 4567 4141 4141 0018 2070 6172  AAAAEgAAAA.. par
 00001430: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-00001440: 6572 7369 6f6e 2031 302e 302e 3119 6c1c  ersion 10.0.1.l.
+00001440: 6572 7369 6f6e 2031 322e 302e 3019 6c1c  ersion 12.0.0.l.
 00001450: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001460: 0000 5e10 0000 5041 5231                 ..^...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/retailers.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -311,17 +311,17 @@
 00001360: 6e74 3222 2c20 2270 616e 6461 735f 7479  nt2", "pandas_ty
 00001370: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
 00001380: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
 00001390: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
 000013a0: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
 000013b0: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 000013c0: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-000013d0: 7665 7273 696f 6e22 3a20 2231 302e 302e  version": "10.0.
+000013d0: 7665 7273 696f 6e22 3a20 2231 322e 302e  version": "12.0.
 000013e0: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-000013f0: 7369 6f6e 223a 2022 312e 352e 3322 7d00  sion": "1.5.3"}.
+000013f0: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
 00001400: 180c 4152 524f 573a 7363 6865 6d61 18e0  ..ARROW:schema..
 00001410: 162f 2f2f 2f2f 3441 4941 4141 5141 4141  ./////4AIAAAQAAA
 00001420: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
 00001430: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
 00001440: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
 00001450: 4143 6741 4141 4377 4741 4141 4541 4141  ACgAAACwGAAAEAAA
 00001460: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
@@ -446,18 +446,18 @@
 00001bd0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
 00001be0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
 00001bf0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
 00001c00: 694f 6942 7564 5778 7366 5630 7349 434a  iOiBudWxsfV0sICJ
 00001c10: 6a63 6d56 6864 4739 7949 6a6f 6765 794a  jcmVhdG9yIjogeyJ
 00001c20: 7361 574a 7959 584a 3549 6a6f 6749 6e42  saWJyYXJ5IjogInB
 00001c30: 3559 584a 7962 3363 694c 4341 6964 6d56  5YXJyb3ciLCAidmV
-00001c40: 7963 326c 7662 6949 3649 4349 784d 4334  yc2lvbiI6ICIxMC4
+00001c40: 7963 326c 7662 6949 3649 4349 784d 6934  yc2lvbiI6ICIxMi4
 00001c50: 774c 6a45 6966 5377 6749 6e42 6862 6d52  wLjEifSwgInBhbmR
 00001c60: 6863 3139 325a 584a 7a61 5739 7549 6a6f  hc192ZXJzaW9uIjo
-00001c70: 6749 6a45 754e 5334 7a49 6e30 4141 4141  gIjEuNS4zIn0AAAA
+00001c70: 6749 6a49 754d 4334 7a49 6e30 4141 4141  gIjIuMC4zIn0AAAA
 00001c80: 4142 6741 4141 4842 6862 6d52 6863 7741  ABgAAAHBhbmRhcwA
 00001c90: 4143 6741 4141 5051 4241 4143 6f41 5141  ACgAAAPQBAACoAQA
 00001ca0: 4163 4145 4141 4541 4241 4141 4d41 5141  AcAEAAEABAAAMAQA
 00001cb0: 4132 4141 4141 4b41 4141 4142 7341 4141  A2AAAAKAAAABsAAA
 00001cc0: 414f 4141 4141 4151 4141 4142 452f 762f  AOAAAAAQAAABE/v/
 00001cd0: 2f41 4141 4241 7841 4141 4141 6341 4141  /AAABAxAAAAAcAAA
 00001ce0: 4142 4141 4141 4141 4141 4141 4941 4141  ABAAAAAAAAAAIAAA
@@ -498,11 +498,11 @@
 00001f10: 4142 6741 4141 4141 4141 6741 5141 4251  ABgAAAAAAAgAQABQ
 00001f20: 4143 4141 4741 4163 4144 4141 4141 4241  ACAAGAAcADAAAABA
 00001f30: 4145 4141 4141 4141 4141 5155 5141 4141  AEAAAAAAAAQUQAAA
 00001f40: 4149 4141 4141 4151 4141 4141 4141 4141  AIAAAAAQAAAAAAAA
 00001f50: 4143 4141 4141 484a 6c64 4746 7062 4756  ACAAAAHJldGFpbGV
 00001f60: 7941 4141 4141 4151 4142 4141 4541 4141  yAAAAAAQABAAEAAA
 00001f70: 4100 1820 7061 7271 7565 742d 6370 702d  A.. parquet-cpp-
-00001f80: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-00001f90: 2e30 2e31 19ac 1c00 001c 0000 1c00 001c  .0.1............
+00001f80: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+00001f90: 2e30 2e30 19ac 1c00 001c 0000 1c00 001c  .0.0............
 00001fa0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001fb0: 001c 0000 006e 1600 0050 4152 31         .....n...PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/shopping.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,17 @@
 00000b40: 6e61 6d65 223a 2022 7636 222c 2022 7061  name": "v6", "pa
 00000b50: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
 00000b60: 3332 222c 2022 6e75 6d70 795f 7479 7065  32", "numpy_type
 00000b70: 223a 2022 696e 7433 3222 2c20 226d 6574  ": "int32", "met
 00000b80: 6164 6174 6122 3a20 6e75 6c6c 7d5d 2c20  adata": null}], 
 00000b90: 2263 7265 6174 6f72 223a 207b 226c 6962  "creator": {"lib
 00000ba0: 7261 7279 223a 2022 7079 6172 726f 7722  rary": "pyarrow"
-00000bb0: 2c20 2276 6572 7369 6f6e 223a 2022 3130  , "version": "10
+00000bb0: 2c20 2276 6572 7369 6f6e 223a 2022 3132  , "version": "12
 00000bc0: 2e30 2e31 227d 2c20 2270 616e 6461 735f  .0.1"}, "pandas_
-00000bd0: 7665 7273 696f 6e22 3a20 2231 2e35 2e33  version": "1.5.3
+00000bd0: 7665 7273 696f 6e22 3a20 2232 2e30 2e33  version": "2.0.3
 00000be0: 227d 0018 0c41 5252 4f57 3a73 6368 656d  "}...ARROW:schem
 00000bf0: 6118 d80f 2f2f 2f2f 2f39 6746 4141 4151  a.../////9gFAAAQ
 00000c00: 4141 4141 4141 414b 4141 3441 4267 4146  AAAAAAAKAA4ABgAF
 00000c10: 4141 6741 4367 4141 4141 4142 4241 4151  AAgACgAAAAABBAAQ
 00000c20: 4141 4141 4141 414b 4141 7741 4141 4145  AAAAAAAKAAwAAAAE
 00000c30: 4141 6741 4367 4141 4144 7745 4141 4145  AAgACgAAADwEAAAE
 00000c40: 4141 4141 4151 4141 4141 7741 4141 4149  AAAAAQAAAAwAAAAI
@@ -275,18 +275,18 @@
 00001120: 4d7a 4969 4c43 4169 626e 5674 6348 6c66  MzIiLCAibnVtcHlf
 00001130: 6448 6c77 5a53 4936 4943 4a70 626e 517a  dHlwZSI6ICJpbnQz
 00001140: 4d69 4973 4943 4a74 5a58 5268 5a47 4630  MiIsICJtZXRhZGF0
 00001150: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
 00001160: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
 00001170: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
 00001180: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
-00001190: 5a58 4a7a 6157 3975 496a 6f67 496a 4577  ZXJzaW9uIjogIjEw
+00001190: 5a58 4a7a 6157 3975 496a 6f67 496a 4579  ZXJzaW9uIjogIjEy
 000011a0: 4c6a 4175 4d53 4a39 4c43 4169 6347 4675  LjAuMSJ9LCAicGFu
 000011b0: 5a47 467a 5833 5a6c 636e 4e70 6232 3469  ZGFzX3ZlcnNpb24i
-000011c0: 4f69 4169 4d53 3431 4c6a 4d69 6651 4147  OiAiMS41LjMifQAG
+000011c0: 4f69 4169 4d69 3477 4c6a 4d69 6651 4147  OiAiMi4wLjMifQAG
 000011d0: 4141 4141 6347 4675 5a47 467a 4141 4148  AAAAcGFuZGFzAAAH
 000011e0: 4141 4141 4e41 4541 4150 5141 4141 4445  AAAANAEAAPQAAADE
 000011f0: 4141 4141 6c41 4141 4147 5141 4141 4130  AAAAlAAAAGQAAAA0
 00001200: 4141 4141 4241 4141 4150 6a2b 2f2f 3841  AAAABAAAAPj+//8A
 00001210: 4141 4543 4541 4141 4142 5141 4141 4145  AAECEAAAABQAAAAE
 00001220: 4141 4141 4141 4141 4141 4941 4141 4232  AAAAAAAAAAIAAAB2
 00001230: 4e67 4141 3650 372f 2f77 4141 4141 4567  NgAA6P7//wAAAAEg
@@ -312,10 +312,10 @@
 00001370: 4141 5941 4277 414d 4141 4141 4541 4151  AAYABwAMAAAAEAAQ
 00001380: 4141 4141 4141 4142 4168 4141 4141 4163  AAAAAAABAhAAAAAc
 00001390: 4141 4141 4241 4141 4141 4141 4141 4143  AAAABAAAAAAAAAAC
 000013a0: 4141 4141 6157 5141 4141 6741 4441 4149  AAAAaWQAAAgADAAI
 000013b0: 4141 6341 4341 4141 4141 4141 4141 4567  AAcACAAAAAAAAAEg
 000013c0: 4141 4141 4141 4141 4141 3d3d 0018 2070  AAAAAAAAAA==.. p
 000013d0: 6172 7175 6574 2d63 7070 2d61 7272 6f77  arquet-cpp-arrow
-000013e0: 2076 6572 7369 6f6e 2031 302e 302e 3119   version 10.0.1.
+000013e0: 2076 6572 7369 6f6e 2031 322e 302e 3019   version 12.0.0.
 000013f0: 7c1c 0000 1c00 001c 0000 1c00 001c 0000  |...............
 00001400: 1c00 001c 0000 00bd 0e00 0050 4152 31    ...........PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,17 @@
 00001170: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
 00001180: 6e74 3822 2c20 226d 6574 6164 6174 6122  nt8", "metadata"
 00001190: 3a20 7b22 6e75 6d5f 6361 7465 676f 7269  : {"num_categori
 000011a0: 6573 223a 2032 2c20 226f 7264 6572 6564  es": 2, "ordered
 000011b0: 223a 2066 616c 7365 7d7d 5d2c 2022 6372  ": false}}], "cr
 000011c0: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 000011d0: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-000011e0: 7665 7273 696f 6e22 3a20 2231 302e 302e  version": "10.0.
+000011e0: 7665 7273 696f 6e22 3a20 2231 322e 302e  version": "12.0.
 000011f0: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-00001200: 7369 6f6e 223a 2022 312e 352e 3322 7d00  sion": "1.5.3"}.
+00001200: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
 00001210: 180c 4152 524f 573a 7363 6865 6d61 18a0  ..ARROW:schema..
 00001220: 162f 2f2f 2f2f 3141 4941 4141 5141 4141  ./////1AIAAAQAAA
 00001230: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
 00001240: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
 00001250: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
 00001260: 4143 6741 4141 4e41 4641 4141 4541 4141  ACgAAANAFAAAEAAA
 00001270: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
@@ -408,17 +408,17 @@
 00001970: 7564 5731 6659 3246 305a 5764 7663 6d6c  udW1fY2F0ZWdvcml
 00001980: 6c63 7949 3649 4449 7349 434a 7663 6d52  lcyI6IDIsICJvcmR
 00001990: 6c63 6d56 6b49 6a6f 675a 6d46 7363 3256  lcmVkIjogZmFsc2V
 000019a0: 3966 5630 7349 434a 6a63 6d56 6864 4739  9fV0sICJjcmVhdG9
 000019b0: 7949 6a6f 6765 794a 7361 574a 7959 584a  yIjogeyJsaWJyYXJ
 000019c0: 3549 6a6f 6749 6e42 3559 584a 7962 3363  5IjogInB5YXJyb3c
 000019d0: 694c 4341 6964 6d56 7963 326c 7662 6949  iLCAidmVyc2lvbiI
-000019e0: 3649 4349 784d 4334 774c 6a45 6966 5377  6ICIxMC4wLjEifSw
+000019e0: 3649 4349 784d 6934 774c 6a45 6966 5377  6ICIxMi4wLjEifSw
 000019f0: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001a00: 7a61 5739 7549 6a6f 6749 6a45 754e 5334  zaW9uIjogIjEuNS4
+00001a00: 7a61 5739 7549 6a6f 6749 6a49 754d 4334  zaW9uIjogIjIuMC4
 00001a10: 7a49 6e30 4141 4159 4141 4142 7759 5735  zIn0AAAYAAABwYW5
 00001a20: 6b59 584d 4141 416f 4141 4141 6341 6741  kYXMAAAoAAAAcAgA
 00001a30: 4133 4145 4141 4b77 4241 4142 3841 5141  A3AEAAKwBAAB8AQA
 00001a40: 4154 4145 4141 4277 4241 4144 7341 4141  ATAEAABwBAADsAAA
 00001a50: 4176 4141 4141 4777 4141 4141 4541 4141  AvAAAAGwAAAAEAAA
 00001a60: 4172 502f 2f2f 7741 4141 5155 5541 4141  ArP///wAAAQUUAAA
 00001a70: 4152 4141 4141 4341 4141 4141 4541 4141  ARAAAACAAAAAEAAA
@@ -463,11 +463,11 @@
 00001ce0: 4249 4141 4141 4241 4146 4141 4941 4159  BIAAAABAAFAAIAAY
 00001cf0: 4142 7741 4d41 4141 4145 4141 5141 4141  ABwAMAAAAEAAQAAA
 00001d00: 4141 4141 4241 6841 4141 4141 6341 4141  AAAABAhAAAAAcAAA
 00001d10: 4142 4141 4141 4141 4141 4141 4341 4141  ABAAAAAAAAAACAAA
 00001d20: 4161 5751 4141 4167 4144 4141 4941 4163  AaWQAAAgADAAIAAc
 00001d30: 4143 4141 4141 4141 4141 4145 6741 4141  ACAAAAAAAAAEgAAA
 00001d40: 4100 1820 7061 7271 7565 742d 6370 702d  A.. parquet-cpp-
-00001d50: 6172 726f 7720 7665 7273 696f 6e20 3130  arrow version 10
-00001d60: 2e30 2e31 19ac 1c00 001c 0000 1c00 001c  .0.1............
+00001d50: 6172 726f 7720 7665 7273 696f 6e20 3132  arrow version 12
+00001d60: 2e30 2e30 19ac 1c00 001c 0000 1c00 001c  .0.0............
 00001d70: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001d80: 001c 0000 00b6 1400 0050 4152 31         .........PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
 00000b00: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
 00000b10: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
 00000b20: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
 00000b30: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
 00000b40: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
 00000b50: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
 00000b60: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-00000b70: 2022 3130 2e30 2e31 227d 2c20 2270 616e   "10.0.1"}, "pan
-00000b80: 6461 735f 7665 7273 696f 6e22 3a20 2231  das_version": "1
-00000b90: 2e35 2e33 227d 0018 0c41 5252 4f57 3a73  .5.3"}...ARROW:s
+00000b70: 2022 3132 2e30 2e31 227d 2c20 2270 616e   "12.0.1"}, "pan
+00000b80: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
+00000b90: 2e30 2e33 227d 0018 0c41 5252 4f57 3a73  .0.3"}...ARROW:s
 00000ba0: 6368 656d 6118 cc0b 2f2f 2f2f 2f31 4145  chema.../////1AE
 00000bb0: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
 00000bc0: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
 00000bd0: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
 00000be0: 4141 4145 4141 6741 4367 4141 4145 6744  AAAEAAgACgAAAEgD
 00000bf0: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
 00000c00: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
@@ -250,18 +250,18 @@
 00000f90: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
 00000fa0: 4943 4a6d 6247 3968 6444 5930 4969 7767  ICJmbG9hdDY0Iiwg
 00000fb0: 496d 316c 6447 466b 5958 5268 496a 6f67  Im1ldGFkYXRhIjog
 00000fc0: 626e 5673 6248 3164 4c43 4169 5933 4a6c  bnVsbH1dLCAiY3Jl
 00000fd0: 5958 5276 6369 4936 4948 7369 6247 6c69  YXRvciI6IHsibGli
 00000fe0: 636d 4679 6553 4936 4943 4a77 6557 4679  cmFyeSI6ICJweWFy
 00000ff0: 636d 3933 4969 7767 496e 5a6c 636e 4e70  cm93IiwgInZlcnNp
-00001000: 6232 3469 4f69 4169 4d54 4175 4d43 3478  b24iOiAiMTAuMC4x
+00001000: 6232 3469 4f69 4169 4d54 4975 4d43 3478  b24iOiAiMTIuMC4x
 00001010: 496e 3073 4943 4a77 5957 356b 5958 4e66  In0sICJwYW5kYXNf
-00001020: 646d 5679 6332 6c76 6269 4936 4943 4978  dmVyc2lvbiI6ICIx
-00001030: 4c6a 5575 4d79 4a39 4141 4141 4141 5941  LjUuMyJ9AAAAAAYA
+00001020: 646d 5679 6332 6c76 6269 4936 4943 4979  dmVyc2lvbiI6ICIy
+00001030: 4c6a 4175 4d79 4a39 4141 4141 4141 5941  LjAuMyJ9AAAAAAYA
 00001040: 4141 4277 5957 356b 5958 4d41 4141 5141  AABwYW5kYXMAAAQA
 00001050: 4141 4373 4141 4141 6441 4141 4144 6741  AACsAAAAdAAAADgA
 00001060: 4141 4145 4141 4141 6450 2f2f 2f77 4141  AAAEAAAAdP///wAA
 00001070: 4151 4d51 4141 4141 4841 4141 4141 5141  AQMQAAAAHAAAAAQA
 00001080: 4141 4141 4141 4141 4367 4141 4148 4e70  AAAAAAAACgAAAHNp
 00001090: 6257 6c73 5958 4a70 6448 6b41 414d 372f  bWlsYXJpdHkAAM7/
 000010a0: 2f2f 3841 4141 4941 7050 2f2f 2f77 4141  //8AAAIApP///wAA
@@ -275,9 +275,9 @@
 00001120: 2f2f 3851 4142 5141 4341 4147 4141 6341  //8QABQACAAGAAcA
 00001130: 4441 4141 4142 4141 4541 4141 4141 4141  DAAAABAAEAAAAAAA
 00001140: 4151 5551 4141 4141 4741 4141 4141 5141  AQUQAAAAGAAAAAQA
 00001150: 4141 4141 4141 4141 4177 4141 4147 6c6b  AAAAAAAAAwAAAGlk
 00001160: 4d51 4145 4141 5141 4241 4141 4141 4141  MQAEAAQABAAAAAAA
 00001170: 4141 413d 0018 2070 6172 7175 6574 2d63  AAA=.. parquet-c
 00001180: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-00001190: 2031 302e 302e 3119 4c1c 0000 1c00 001c   10.0.1.L.......
+00001190: 2031 322e 302e 3019 4c1c 0000 1c00 001c   12.0.0.L.......
 000011a0: 0000 1c00 0000 f60a 0000 5041 5231       ..........PAR1
```

### Comparing `pyrsm-0.9.1/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.9.2/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/example_data.py` & `pyrsm-0.9.2/pyrsm/example_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from importlib import import_module
 import pandas as pd
+import polars as pl
 
 
-def load_data(pkg=None, name=None, dct=None):
+def load_data(pkg=None, name=None, dct=None, polars=False):
     """
     Load example data included in the pyrsm package
 
     Parameters
     ----------
     pkg : str
         One of "data", "design", "basics", "model", or "multivariate"
@@ -29,15 +30,18 @@
     data, description = rsm.load_data(pkg="basics", name="demand_uk")
     """
 
     base = "pyrsm.data"
     base_path = import_module(base).__path__[0]
 
     def load_data(file_path):
-        return pd.read_parquet(file_path)
+        if polars:
+            return pl.read_parquet(file_path)
+        else:
+            return pd.read_parquet(file_path)
 
     def load_description(file_path):
         # read a text file into a string
         with open(f"{file_path}_description.md", "r") as file:
             descr = file.read()
         return descr
```

### Comparing `pyrsm-0.9.1/pyrsm/logistic.py` & `pyrsm-0.9.2/pyrsm/logistic.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/model.py` & `pyrsm-0.9.2/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/notebook.py` & `pyrsm-0.9.2/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/perf.py` & `pyrsm-0.9.2/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/props.py` & `pyrsm-0.9.2/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/compare_means.py` & `pyrsm-0.9.2/pyrsm/radiant/compare_means.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,34 +299,36 @@
 def compare_means(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for compare means hypothesis testing
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="salary")
     rc = basics_compare_means(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
 
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    compare_means()
+    compare_means(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.9.2/pyrsm/radiant/cross_tabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
-import webbrowser, nest_asyncio, uvicorn
-import signal, os, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import signal
+import os
+import sys
+import tempfile
 import pyrsm as rsm
-from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "observed": "Observed",
     "expected": "Expected",
     "chisq": "Chi-squared",
@@ -163,34 +167,36 @@
 def cross_tabs(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for cross-tabs hypothesis testing
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
     rc = basics_cross_tabs(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
 
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    cross_tabs()
+    cross_tabs(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/data_view.py` & `pyrsm-0.9.2/pyrsm/radiant/data_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,8 +124,8 @@
     )
 
 
 if __name__ == "__main__":
     # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
     # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
     # single_mean(data_dct, descriptions_dct, code=True)
-    view(debug=True)
+    view(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/goodness.py` & `pyrsm-0.9.2/pyrsm/radiant/goodness.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
-import webbrowser, nest_asyncio, uvicorn
-import signal, io, os, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import signal
+import os
+import sys
+import tempfile
 import pyrsm as rsm
-from contextlib import redirect_stdout
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "observed": "Observed",
     "expected": "Expected",
     "chisq": "Chi-squared",
@@ -158,34 +162,36 @@
 def goodness(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for goodness of fit analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
     rc = basics_goodness(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
 
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    goodness()
+    goodness(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/logistic.py` & `pyrsm-0.9.2/pyrsm/radiant/logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from starlette.applications import Starlette
 from starlette.routing import Mount
 from starlette.staticfiles import StaticFiles
 from shiny import App, ui, render, reactive, Inputs, Outputs, Session
 from pathlib import Path
-import webbrowser, nest_asyncio, uvicorn
-import signal, os, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import signal
+import os
+import sys
+import tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     # "dist": "Distribution",
@@ -202,8 +207,8 @@
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     # titanic, titanic_description = rsm.load_data(pkg="data", name="titanic")
     # logistic({"titanic": titanic}, {"titanic": titanic_description}, code=True)
-    logistic(debug=True)
+    logistic(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/model_utils.py` & `pyrsm-0.9.2/pyrsm/radiant/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,17 @@
             args["data"] = input.pred_datasets()
             args["data_cmd"] = cmd
 
         ci = input.pred_ci()
         if ci:
             args.update({"ci": ci, "conf": input.conf()})
 
-        args_string = ru.drop_default_args(args, pred_fun)
+        args_string = ru.drop_default_args(
+            args, pred_fun, ignore=["data", "cmd", "data_cmd"]
+        )
         return f"""{ret}.predict({args_string})"""
 
     @output(id="show_predict_code")
     @render.text
     def show_predict_code():
         return ru.code_formatter(
             f"""{show_code()}\npred = {predict_code()}""",
@@ -300,15 +302,14 @@
 
             return render.DataTable(pred.round(3), summary=summary)
         else:
             return None
 
 
 def make_plot(self, input, output, session, show_code, estimate, ret, pc=None):
-
     if pc is None:
 
         def plot_code():
             plots = input.plots()
             if plots == "pred":
                 incl = list(input.incl_evar())
                 incl_int = list(input.incl_interactions())
@@ -327,15 +328,14 @@
 
     @output(id="show_plot_code")
     @render.text
     def show_plot_code():
         plots = input.plots()
         if plots != "None":
             cmd = f"""{show_code()}\n{plot_code()}"""
-            # return ru.code_formatter(cmd, self)
             return ru.code_formatter(cmd, self, input, session, id="copy_plot")
 
     @reactive.Calc
     def gen_plot():
         locals()[ret] = estimate()
         eval(f"""{plot_code()}""")
         fig = plt.gcf()
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/probability_calculator.py` & `pyrsm-0.9.2/pyrsm/radiant/probability_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
-import webbrowser, nest_asyncio, uvicorn
-import signal, os, io, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import signal
+import os
+import io
+import sys
+import tempfile
 import matplotlib.pyplot as plt
 from contextlib import redirect_stdout, redirect_stderr
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.basics.probability_calculator as pc
 
 pc_type = {"values": "Values", "probs": "Probabilities"}
@@ -307,32 +313,34 @@
 
 
 def prob_calc(
     code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "critical",
+    debug: bool = False,
 ):
     """
     Launch a Radiant-for-Python app for compare means hypothesis testing
     """
     rc = basics_probability_calculator(code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
 
     # redirect stdout and stderr to the temporary file
-    temp = tempfile.NamedTemporaryFile()
-    sys.stdout = open(temp.name, "w")
-    sys.stderr = open(temp.name, "w")
+    if not debug:
+        temp = tempfile.NamedTemporaryFile()
+        sys.stdout = open(temp.name, "w")
+        sys.stderr = open(temp.name, "w")
 
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    prob_calc()
+    prob_calc(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/regress.py` & `pyrsm-0.9.2/pyrsm/radiant/regress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from starlette.applications import Starlette
 from starlette.routing import Mount
 from starlette.staticfiles import StaticFiles
 from shiny import App, ui, reactive, Inputs, Outputs, Session
 from pathlib import Path
-import webbrowser, nest_asyncio, uvicorn, os, signal
-import signal, os, sys, tempfile
+import webbrowser
+import nest_asyncio
+import uvicorn
+import os
+import signal
+import sys
+import tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     "dist": "Distribution",
@@ -187,8 +192,8 @@
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    regress(debug=True)
+    regress(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/single_mean.py` & `pyrsm-0.9.2/pyrsm/radiant/single_mean.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from starlette.applications import Starlette
 from starlette.routing import Mount
 from starlette.staticfiles import StaticFiles
-from shiny import App, render, ui, reactive, Inputs, Outputs, Session
+from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
 from pathlib import Path
 import webbrowser
 import nest_asyncio
 import uvicorn
 import signal
 import os
 import sys
@@ -99,14 +99,15 @@
                 label="Variable (select one)",
                 selected=None,
                 choices=isNum,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
+            req(input.comp_value() is not None, "comp_value must be specified")
 
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
                 "var": input.var(),
                 "alt_hyp": input.alt_hyp(),
                 "conf": input.conf(),
                 "comp_value": input.comp_value(),
@@ -205,8 +206,8 @@
     )
 
 
 if __name__ == "__main__":
     # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
     # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
     # single_mean(data_dct, descriptions_dct, code=True)
-    single_mean(debug=True)
+    single_mean(debug=False)
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/utils.py` & `pyrsm-0.9.2/pyrsm/radiant/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from faicons import icon_svg
 import pandas as pd
 import polars as pl
 from pyrsm.utils import ifelse
 from pyrsm.example_data import load_data
 
 
-def get_dfs(pkg=None, name=None, obj=pd.DataFrame):
+def get_dfs(pkg=None, name=None, polars=False):
+    obj = pd.DataFrame if not polars else pl.DataFrame
     data_dct = {k: v for k, v in globals().items() if isinstance(v, obj)}
     descriptions_dct = {
         k: globals()[f"{k}_description"]
         for k in data_dct
         if f"{k}_description" in globals()
     }
     if len(data_dct) == 0 and name is not None:
-        data, description = load_data(pkg=pkg, name=name)
+        data, description = load_data(pkg=pkg, name=name, polars=polars)
         data_dct = {name: data}
         descriptions_dct = {name: description}
     elif len(data_dct) == 0 and pkg is not None:
         data_dct, descriptions_dct = load_data(pkg=pkg)
 
     return ifelse(len(data_dct) == 0, None, data_dct), ifelse(
         len(descriptions_dct) == 0, None, descriptions_dct
@@ -42,15 +43,15 @@
     """
     return ui.head_content(
         # from https://github.com/rstudio/py-shiny/issues/491#issuecomment-1579138681
         ui.tags.link(
             href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/agate.min.css",
             rel="stylesheet",
         ),
-        ui.tags.link(rel="shortcut icon", href=f"/www/imgs/icon.png"),
+        ui.tags.link(rel="shortcut icon", href="/www/imgs/icon.png"),
         ui.tags.link(href="/www/style.css", rel="stylesheet"),
         ui.tags.script(src="/www/js/returnTextAreaBinding.js"),
         ui.tags.script(src="/www/js/radiantUI.js"),
         ui.tags.script(src="/www/js/screenshot.js"),
         ui.tags.script(
             src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js",
         ),
@@ -306,15 +307,15 @@
             #     inline=True,
             # ),
             input_return_text_area(
                 "data_filter",
                 "Data Filter:",
                 rows=2,
                 value=self.state.get("data_filter", ""),
-                placeholder="Provide a filter (e.g., price >  5000) and press return",
+                placeholder="Provide a filter (e.g., price > 5000) and press return",
             ),
             input_return_text_area(
                 "data_sort",
                 "Data sort:",
                 rows=2,
                 placeholder="Sort (e.g., ['color', 'price'], ascending=[True, False])) and press return",
             ),
@@ -480,22 +481,22 @@
             ),
         ),
     )
 
 
 def ui_stop():
     return (
-        ui.nav_control(
-            ui.input_action_link(
-                "screenshot",
-                "Screenshot",
-                icon=icon_svg("camera"),
-                onclick="generate_screenshot();",
-            ),
-        ),
+        # ui.nav_control(
+        #     ui.input_action_link(
+        #         "screenshot",
+        #         "Screenshot",
+        #         icon=icon_svg("camera"),
+        #         onclick="generate_screenshot();",
+        #     ),
+        # ),
         ui.nav_control(
             ui.input_action_link(
                 "stop", "Stop", icon=icon_svg("stop"), onclick="window.close();"
             ),
         ),
     )
 
@@ -556,32 +557,14 @@
         if not is_empty(input.evar()) and not is_empty(input.rvar()):
             update()
 
         # not clear why this needs to be separate from the above
         if not is_empty(input.interactions()):
             update()
 
-    ## first bit works but can't reset on a timer
-    # @reactive.Effect
-    # @reactive.event(input.copy, ignore_none=True)
-    # def copy_success():
-    #     ui.update_action_link(
-    #         "copy",
-    #         icon=icon_svg("check", width="1.5em", height="1.5em"),
-    #     )
-
-    # @reactive.Effect
-    # @reactive.event(input.copy, ignore_none=True)
-    # def copy_reset():
-    #     reactive.invalidate_later(0.5)
-    #     ui.update_action_link(
-    #         "copy",
-    #         icon=icon_svg("copy", width="1.5em", height="1.5em"),
-    #     )
-
     @reactive.Effect
     @reactive.event(input.run, ignore_none=True)
     def run_done():
         ui.update_action_button(
             "run",
             label="Estimate model",
             icon=icon_svg("play"),
@@ -651,57 +634,7 @@
 #   caption = "Save radiant screenshot",
 #   plot = render_screenshot,
 #   btn = "button",
 #   label = "Save",
 #   class = "btn-primary",
 #   onclick = "get_img_src();"
 # )
-
-# getting data to work as a separate nav item caused problems
-# def ui_data(self):
-#     return ui.nav(
-#         "Data",
-#         ui.row(
-#             ui.column(
-#                 3,
-#                 ui.panel_well(
-#                     ui.input_select("datasets", "Datasets:", self.dataset_list)
-#                 ),
-#                 ui.panel_well(
-#                     ui.input_checkbox("show_filter", "Show data filter", value=True),
-#                     ui.panel_conditional(
-#                         "input.show_filter == true",
-#                         ui.input_radio_buttons(
-#                             "data_language",
-#                             "Data language",
-#                             choices=["Pandas", "Polars", "SQL"],
-#                             inline=True,
-#                         ),
-#                         input_return_text_area(
-#                             "data_filter",
-#                             "Data Filter:",
-#                             rows=2,
-#                             placeholder="Provide a filter (e.g., price >  5000) and press return",
-#                         ),
-#                         input_return_text_area(
-#                             "data_sort",
-#                             "Data sort:",
-#                             rows=2,
-#                             placeholder="Sort (e.g., ['color', 'price'], ascending=[True, False])) and press return",
-#                         ),
-#                         input_return_text_area(
-#                             "data_slice",
-#                             "Data slice (rows):",
-#                             rows=1,
-#                             placeholder="e.g., 1:50 and press return",
-#                         ),
-#                     ),
-#                 ),
-#             ),
-#             ui.column(
-#                 8,
-#                 ui.output_ui("show_data_code"),
-#                 ui.output_data_frame("show_data"),
-#                 ui.output_ui("show_description"),
-#             ),
-#         ),
-#     )
```

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.9.2/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-nc-sa.png` & `pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/imgs/by-sa.png` & `pyrsm-0.9.2/pyrsm/radiant/www/imgs/by-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/imgs/icon.png` & `pyrsm-0.9.2/pyrsm/radiant/www/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/js/radiantUI.js` & `pyrsm-0.9.2/pyrsm/radiant/www/js/radiantUI.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/js/returnTextAreaBinding.js` & `pyrsm-0.9.2/pyrsm/radiant/www/js/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/js/screenshot.js` & `pyrsm-0.9.2/pyrsm/radiant/www/js/screenshot.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/radiant/www/style.css` & `pyrsm-0.9.2/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/regress.py` & `pyrsm-0.9.2/pyrsm/regress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pandas as pd
 import re
 import statsmodels.formula.api as smf
 from typing import Optional, Union
-from statsmodels.regression.linear_model import RegressionResults as rrs
-from .utils import ifelse, format_nr, setdiff
-from .visualize import pred_plot_sm, vimp_plot_sm
-from .model import (
+from pyrsm.utils import ifelse, format_nr, setdiff
+from pyrsm.visualize import pred_plot_sm, vimp_plot_sm
+from pyrsm.model import (
     sig_stars,
     model_fit,
     extract_evars,
     extract_rvar,
     scatter_plot,
     reg_dashboard,
     residual_plot,
@@ -28,15 +27,14 @@
         self,
         data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         rvar: Optional[str] = None,
         evar: Optional[list[str]] = None,
         ivar: Optional[list[str]] = None,
         form: Optional[str] = None,
     ) -> None:
-
         """
         Estimate linear regression model
 
         Parameters
         ----------
         data: pandas DataFrame; dataset
         evar: List of strings; contains the names of the columns of data to be used as explanatory variables
```

### Comparing `pyrsm-0.9.1/pyrsm/stats.py` & `pyrsm-0.9.2/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/utils.py` & `pyrsm-0.9.2/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm/visualize.py` & `pyrsm-0.9.2/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.9.2/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.9.1/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.9.2/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/setup.cfg` & `pyrsm-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_basics.py` & `pyrsm-0.9.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_bins.py` & `pyrsm-0.9.2/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_example_data.py` & `pyrsm-0.9.2/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_perf.py` & `pyrsm-0.9.2/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_regression.py` & `pyrsm-0.9.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_stats.py` & `pyrsm-0.9.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.9.1/tests/test_utils.py` & `pyrsm-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

