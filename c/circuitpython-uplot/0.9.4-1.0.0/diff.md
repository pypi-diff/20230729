# Comparing `tmp/circuitpython-uplot-0.9.4.tar.gz` & `tmp/circuitpython-uplot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-uplot-0.9.4.tar", last modified: Fri Mar 10 14:44:13 2023, max compression
+gzip compressed data, was "circuitpython-uplot-1.0.0.tar", last modified: Fri Jul 28 19:29:44 2023, max compression
```

## Comparing `circuitpython-uplot-0.9.4.tar` & `circuitpython-uplot-1.0.0.tar`

### file list

```diff
@@ -1,106 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.873950 circuitpython-uplot-0.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.873950 circuitpython-uplot-0.9.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/circuitpython_uplot/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ucartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ufillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ulogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/upie.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/uplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/uscatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.881950 circuitpython-uplot-0.9.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.881950 circuitpython-uplot-0.9.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/quick_start.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/readme.png
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/readme.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif.license
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex7.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_display_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_integration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_readme_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_stackplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_tickparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ubar_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_uboxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ucartesian_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ucartesian_loggin_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ufillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ulogging.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_upie_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_uscatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.743825 circuitpython-uplot-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.687825 circuitpython-uplot-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.695824 circuitpython-uplot-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-28 19:29:44.743825 circuitpython-uplot-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.703825 circuitpython-uplot-1.0.0/circuitpython_uplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/fillbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/shade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/circuitpython_uplot/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.703825 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-28 19:29:44.000000 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-28 19:29:44.000000 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:29:44.000000 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 19:29:44.000000 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 19:29:44.000000 circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.723825 circuitpython-uplot-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.727825 circuitpython-uplot-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/bar_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/bar_palette.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/bar_scale.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/fillbetween_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  3215396 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/logging.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/logging_fill.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/logging_table.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/map.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/polar_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    59396 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/polar_plots.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/readme.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/readme2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/scatter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_3DBars.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_cartesian.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_cartesian_advance.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex12.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex16.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_ex6.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   107604 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_lissajous.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_pie.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    65562 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_shade.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23581 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/docs/uplot_svg.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.743825 circuitpython-uplot-1.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:29:44.743825 circuitpython-uplot-1.0.0/examples/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    68124 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/examples/fonts/LibreBodoniv2002-Bold-10.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)    85245 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/examples/fonts/LibreBodoniv2002-Regular-17.bdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   408924 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/examples/fonts/forkawesome-36.pcf
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/examples/fonts/forkawesome-36.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_3Dbars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_color_changing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_colorpalette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_scale_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_bar_updating_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_cartesian_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_cartesian_loggin_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_cartesian_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_display_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_fillbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_integration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_lissajous_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_logging_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_logging_changing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_logging_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_logging_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_pie_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_polar_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_polar_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_readme_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_shade_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_stackplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_svg_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_tickparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/examples/uplot_uboxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-28 19:29:34.000000 circuitpython-uplot-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 19:29:24.000000 circuitpython-uplot-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:29:44.743825 circuitpython-uplot-1.0.0/setup.cfg
```

### Comparing `circuitpython-uplot-0.9.4/.pre-commit-config.yaml` & `circuitpython-uplot-1.0.0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-# SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
+# SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
-    hooks:
-      - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `circuitpython-uplot-0.9.4/LICENSE` & `circuitpython-uplot-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/PKG-INFO` & `circuitpython-uplot-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 0.9.4
+Version: 1.0.0
 Summary: framework to display different plots in displayio. similar to widget
-Author-email: "Jose D. Montoya" <uplot@mailmeto.mozmail.com>
+Author-email: JDM <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
-Keywords: adafruit,blinka,circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,displayio,circuitpython,graphics,plot,library,plotting,ulab
+Keywords: circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,line,displayio,graphics,library,ulab,svg,widget,graph,graphing,chart,charts,plotting,plot,plotter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -20,34 +20,48 @@
     :target: https://circuitpython-uplot.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_uplot/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-uplot.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-uplot
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-uplot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-uplot
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Framework to display different plots in displayio. Similar to widget.
+Framework to display different graphical plots in displayio.
 Take a look in the `examples <https://circuitpython-uplot.readthedocs.io/en/latest/examples.html>`_ section in RTD to see the gallery
 
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
+
+
+Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
+
 
 Dependencies
 =============
 This library depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-This library is ressource consuming, may or may not with some CircuitPython supported devices.
+This library is resource consuming, may or may not with some CircuitPython supported devices.
 Tinker it as you wish in order to work.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
@@ -112,10 +126,8 @@
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-uplot.readthedocs.io/>`_.
 
 
 Contributing
 ============
 
-Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/jposada202020/CircuitPython_uplot/blob/HEAD/CODE_OF_CONDUCT.md>`_
-before contributing to help this project stay welcoming.
+Contributions are welcome!
```

### Comparing `circuitpython-uplot-0.9.4/README.rst` & `circuitpython-uplot-1.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,48 @@
     :target: https://circuitpython-uplot.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_uplot/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-uplot.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-uplot
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-uplot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-uplot
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Framework to display different plots in displayio. Similar to widget.
+Framework to display different graphical plots in displayio.
 Take a look in the `examples <https://circuitpython-uplot.readthedocs.io/en/latest/examples.html>`_ section in RTD to see the gallery
 
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
+
+
+Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
+
 
 Dependencies
 =============
 This library depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-This library is ressource consuming, may or may not with some CircuitPython supported devices.
+This library is resource consuming, may or may not with some CircuitPython supported devices.
 Tinker it as you wish in order to work.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
@@ -94,10 +108,8 @@
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-uplot.readthedocs.io/>`_.
 
 
 Contributing
 ============
 
-Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/jposada202020/CircuitPython_uplot/blob/HEAD/CODE_OF_CONDUCT.md>`_
-before contributing to help this project stay welcoming.
+Contributions are welcome!
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/ucartesian.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/cartesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`ucartesian`
+`cartesian`
 ================================================================================
 
 CircuitPython cartesian graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Optional, Union
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from bitmaptools import draw_line, fill_region
 from ulab import numpy as np
 from vectorio import Polygon
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
-# pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
-# pylint: disable=too-many-locals, too-many-branches
-class ucartesian:
+class Cartesian:
     """
     Class to draw cartesian plane
     """
 
     def __init__(
         self,
-        plot: Uplot,
+        plot: Plot,
         x: Union[list, np.linspace, np.ndarray],
         y: Union[list, np.linspace, np.ndarray],
         rangex: Optional[list] = None,
         rangey: Optional[list] = None,
         line_color: Optional[int] = None,
         fill: bool = False,
         nudge: bool = True,
         logging: bool = False,
     ) -> None:
         """
 
-        :param Uplot plot: Plot object for the scatter to be drawn
+        :param Plot plot: Plot object for the scatter to be drawn
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray x: x points coordinates
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray y: y points coordinates
         :param list|None rangex: x range limits. Defaults to None
         :param list|None rangey: y range limits. Defaults to None
         :param int|None line_color: line color. Defaults to None
         :param bool fill: Show the filling. Defaults to `False`
         :param bool nudge: moves the graph a little for better displaying. Defaults to `True`
@@ -119,14 +117,16 @@
                     plot._newymin - plot._tickheighty,
                     0,
                 )
 
             for index, _ in enumerate(xnorm):
                 if index + 1 >= len(xnorm):
                     break
+                if y[index] >= ymax:
+                    continue
                 draw_line(
                     plot._plotbitmap,
                     xnorm[index],
                     ynorm[index],
                     xnorm[index + 1],
                     ynorm[index + 1],
                     plot._index_colorused,
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/ufillbetween.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/fillbetween.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`ufillbetween`
+`fillbetween`
 ================================================================================
 
 CircuitPython fillbetween graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Optional, Union
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from ulab import numpy as np
 from vectorio import Polygon
 
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
-# pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
-# pylint: disable=too-many-locals
-class ufillbetween:
+
+class Fillbetween:
     """
     Class to draw a fillbetween graph
     """
 
     def __init__(
         self,
-        plot: Uplot,
+        plot: Plot,
         x: Union[list, np.linspace, np.ndarray],
         y1: Union[list, np.linspace, np.ndarray],
         y2: Union[list, np.linspace, np.ndarray],
         rangex: Optional[list] = None,
         rangey: Optional[list] = None,
         fill_color: int = 0xF6FF41,
         nudge: bool = True,
     ) -> None:
         """
-        :param Uplot plot: Plot object for the scatter to be drawn
+        :param Plot plot: Plot object for the scatter to be drawn
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray x: x points coordinates
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray y1: y1 points coordinates
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray y2: y2 points coordinates
         :param list|None rangex: x range limits
         :param list|None rangey: y range limits
         :param int fill_color: filling color. Defaults to 0xF6FF41
         :param bool nudge: moves the graph a little for better displaying
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/ulogging.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/logging.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,86 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`ulogging`
+`logging`
 ================================================================================
 
 CircuitPython logging data graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Union
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from bitmaptools import draw_line, fill_region
 from ulab import numpy as np
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
-# pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
-# pylint: disable=too-many-locals, too-many-branches, protected-access
-class ulogging:
+class Logging:
     """
     Class to log data
     """
 
     def __init__(
         self,
-        plot: Uplot,
+        plot: Plot,
         x: Union[list, np.linspace, np.ndarray],
         y: Union[list, np.linspace, np.ndarray],
         rangex: list,
         rangey: list,
         line_color: int = 0xFFFFFF,
         ticksx: Union[np.array, list] = np.array([0, 10, 30, 50, 70, 90]),
         ticksy: Union[np.array, list] = np.array([0, 10, 30, 50, 70, 90]),
+        tick_pos: bool = False,
+        fill: bool = False,
     ) -> None:
         """
 
-        :param Uplot plot: Plot object for the log to be drawn
+        :param Plot plot: Plot object for the log to be drawn
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray x: x points coordinates
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray y: y points coordinates
         :param list|None rangex: x range limits. Defaults to None
         :param list|None rangey: y range limits. Defaults to None
         :param int|None line_color: line color. Defaults to None
         :param np.array|list ticksx: X axis ticks values
         :param np.array|list ticksy: Y axis ticks values
+        :param bool tick_pos: indicates ticks position. True for below the axes.
+         Defaults to ``False``
+        :param bool fill: enable the filling of the plot. Defaults to ``False``
 
         """
         self.points = []
         self.ticksx = np.array(ticksx)
         self.ticksy = np.array(ticksy)
+        if tick_pos:
+            self._tickposx = plot._tickheightx
+            self._tickposy = plot._tickheighty
+        else:
+            self._tickposx = 0
+            self._tickposy = 0
 
         plot._plot_palette[plot._index_colorused] = line_color
 
         self.xmin = rangex[0]
         self.xmax = rangex[1]
         self.ymin = rangey[0]
         self.ymax = rangey[1]
 
-        x = np.array(x)
-        y = np.array(y)
-
-        xnorm = np.array(
-            plot.transform(self.xmin, self.xmax, plot._newxmin, plot._newxmax, x),
-            dtype=np.int16,
-        )
-        ynorm = np.array(
-            plot.transform(self.ymin, self.ymax, plot._newymin, plot._newymax, y),
-            dtype=np.int16,
-        )
-
-        fill_region(
-            plot._plotbitmap,
-            plot._newxmin + plot._tickheightx + 1,
-            plot._newymax + 1,
-            plot._newxmax - 1,
-            plot._newymin - plot._tickheighty,
-            0,
-        )
+        self.draw_points(plot, x, y, fill)
 
-        if len(x) == 1:
-            plot._plotbitmap[xnorm[0], ynorm[0]] = 1
-        else:
-            for index, _ in enumerate(xnorm):
-                if index + 1 >= len(xnorm):
-                    break
-                draw_line(
-                    plot._plotbitmap,
-                    xnorm[index],
-                    ynorm[index],
-                    xnorm[index + 1],
-                    ynorm[index + 1],
-                    plot._index_colorused,
-                )
         if plot._showticks:
             if plot._loggingfirst:
                 self._draw_ticks(plot)
                 plot._loggingfirst = False
                 plot._showticks = False
 
     def _draw_ticks(self, plot) -> None:
@@ -126,29 +102,99 @@
             dtype=np.int16,
         )
 
         for i, tick in enumerate(ticksxnorm):
             draw_line(
                 plot._plotbitmap,
                 tick,
-                plot._newymin,
+                plot._newymin + self._tickposx,
                 tick,
-                plot._newymin - plot._tickheightx,
+                plot._newymin - plot._tickheightx + self._tickposx,
                 2,
             )
             if plot._showtext:
-                plot.show_text(
-                    "{:.2f}".format(ticksxnorm[i]), tick, plot._newymin, (0.5, 0.0)
-                )
+                plot.show_text(f"{self.ticksx[i]:.0f}", tick, plot._newymin, (0.5, 0.0))
         for i, tick in enumerate(ticksynorm):
             draw_line(
                 plot._plotbitmap,
-                plot._newxmin,
+                plot._newxmin - self._tickposy,
                 tick,
-                plot._newxmin + plot._tickheighty,
+                plot._newxmin + plot._tickheighty - self._tickposy,
                 tick,
                 2,
             )
             if plot._showtext:
-                plot.show_text(
-                    "{:.2f}".format(ticksynorm[i]), plot._newxmin, tick, (1.0, 0.5)
+                plot.show_text(f"{self.ticksy[i]:.0f}", plot._newxmin, tick, (1.0, 0.5))
+
+    @staticmethod
+    def clear_plot(plot) -> None:
+        """
+        Clears the plot area
+        """
+
+        fill_region(
+            plot._plotbitmap,
+            plot._newxmin + plot._tickheightx + 1,
+            plot._newymax + 1,
+            plot._newxmax - 1,
+            plot._newymin - plot._tickheighty,
+            0,
+        )
+
+    def draw_points(self, plot: Plot, x: list, y: list, fill: bool = False) -> None:
+        """
+        Draws points in the plot
+        :param Plot plot: plot object provided
+        :param list x: list of x values
+        :param list y: list of y values
+        :param bool fill: parameter to fill the plot graphic. Defaults to False
+        :return: None
+        """
+        self.clear_plot(plot)
+
+        self.draw_new_lines(plot, x, y, fill)
+
+    def draw_new_lines(self, plot: Plot, x: list, y: list, fill: bool = False) -> None:
+        """
+        Draw the plot lines
+        :param Plot plot: plot object provided
+        :param list x: list of x values
+        :param list y: list of y values
+        :param bool fill: parameter to fill the plot graphic. Defaults to False
+        :return: None
+        """
+        x = np.array(x)
+        y = np.array(y)
+
+        xnorm = np.array(
+            plot.transform(self.xmin, self.xmax, plot._newxmin, plot._newxmax, x),
+            dtype=np.int16,
+        )
+        ynorm = np.array(
+            plot.transform(self.ymin, self.ymax, plot._newymin, plot._newymax, y),
+            dtype=np.int16,
+        )
+
+        if len(x) == 1:
+            plot._plotbitmap[xnorm[0], ynorm[0]] = 1
+        else:
+            for index, _ in enumerate(xnorm):
+                if index + 1 >= len(xnorm):
+                    break
+                draw_line(
+                    plot._plotbitmap,
+                    xnorm[index],
+                    ynorm[index],
+                    xnorm[index + 1],
+                    ynorm[index + 1],
+                    plot._index_colorused,
                 )
+            if fill:
+                for index, _ in enumerate(xnorm):
+                    draw_line(
+                        plot._plotbitmap,
+                        xnorm[index],
+                        ynorm[index],
+                        xnorm[index],
+                        plot._newymin,
+                        plot._index_colorused,
+                    )
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/umap.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 
 """
 
-`umap`
+`map`
 ================================================================================
 
 CircuitPython color map graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 
 from ulab import numpy as np
 import displayio
 from vectorio import Rectangle
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
-# pylint: disable=too-few-public-methods, invalid-name, duplicate-code, too-many-locals, too-many-arguments
-# pylint: disable=unused-variable
-class umap:
+class Map:
     """
     Main class to display different graphics
     """
 
     def __init__(
         self,
-        plot: Uplot,
+        plot: Plot,
         data_points: np.ndarray,
         initial_color: int,
         final_color: int,
     ) -> None:
-
         """
 
-        :param Uplot plot: Plot object for the scatter to be drawn
+        :param Plot plot: Plot object for the scatter to be drawn
         :param np.array data_points: data points to create the color map
         :param int initial_color: initial color to create the color map
         :param int final_color: final color to create the color map
 
         """
 
         xmin = np.min(data_points)
@@ -72,16 +69,16 @@
             for element in row:
                 palette[counter] = color_fade(start_color, end_color, element)
                 counter = counter + 1
 
         deltax = plot._newxmin
         deltay = plot._newymax
         color = 0
-        for j in range(box_iny):
-            for i in range(box_inx):
+        for _ in range(box_iny):
+            for _ in range(box_inx):
                 plot.append(
                     Rectangle(
                         pixel_shader=palette,
                         x=deltax,
                         y=deltay,
                         width=xdist,
                         height=ydist,
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/upie.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/pie.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`upie`
+`pie`
 ================================================================================
 
 CircuitPython pie graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 
 
 import math
 from vectorio import Polygon
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
-# pylint: disable=too-many-arguments, invalid-name, no-self-use
-class upie:
+
+class Pie:
     """
     Class to draw pie
     """
 
     def __init__(
-        self, plot: Uplot, data: list, x: int = 0, y: int = 0, radius: int = 40
+        self, plot: Plot, data: list, x: int = 0, y: int = 0, radius: int = 40
     ) -> None:
         """
 
-        :param Uplot plot: Plot object for the upie to be drawn
+        :param Plot plot: Plot object for the pie to be drawn
         :param list data: data to make the pie
-        :param x: pie center x coordinate
-        :param y: pie center y coordinate
+        :param int x: pie center x coordinate
+        :param int y: pie center y coordinate
         :param int radius: pie radius
 
         """
 
         step = 1
         total = sum(data)
         per = [int(i / total * 360) for i in data]
@@ -69,18 +69,18 @@
             start = start + pie
             index_color = index_color + 1
             self.pointlist = [(x, y)]
 
     def get_points(self, x: int, y: int, radius: int, angle: float) -> None:
         """
 
-        :param x: center x coordinate
-        :param y: center y coordinate
-        :param radius: pie radius in pixels
-        :param angle: line angle
+        :param int x: center x coordinate
+        :param int y: center y coordinate
+        :param int radius: pie radius in pixels
+        :param flaot angle: line angle
         :return: None
 
         """
         self.pointlist.append(
             (
                 x + int(radius * math.cos(angle * math.pi / 180)),
                 y + int(radius * math.sin(angle * math.pi / 180)),
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/uplot.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`uplot`
+`plot`
 ================================================================================
 
 CircuitPython Plot Class
 
 * Author(s): Jose D. Montoya
 
 Implementation Notes
@@ -17,36 +17,35 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
+# pylint: disable=too-many-statements, unused-import, no-member
+# pylint: disable=unused-import, import-outside-toplevel, undefined-variable
+# pylint: disable=attribute-defined-outside-init
+
 try:
     from typing import Union, Tuple
     from typing_extensions import Literal
 except ImportError:
     pass
 import displayio
 import terminalio
 from bitmaptools import draw_line
 from vectorio import Circle
 from ulab import numpy as np
 
 
-__version__ = "0.9.4"
-__repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
+__version__ = "1.0.0"
+__repo__ = "https://github.com/jposada202020/CircuitPython_uplot.git"
 
 
-# pylint: disable=too-many-arguments, too-many-instance-attributes, too-many-locals
-# pylint: disable=too-many-statements
-# pylint: disable=unused-import, import-outside-toplevel, undefined-variable
-
-
-class Uplot(displayio.Group):
+class Plot(displayio.Group):
     """
     Canvas Class to add different elements to the screen.
     The origin point set by ``x`` and ``y`` properties
 
     :param int x: origin x coordinate
     :param int y: origin y coordinate
     :param int width: plot box width in pixels
@@ -90,26 +89,26 @@
         if y + height > 321:
             print(
                 "Modify this settings. Some of the graphics will not shown int the screen"
             )
             print("Defaulting to y=0")
             y = 0
 
-        super().__init__(x=x, y=y, scale=1)
+        super().__init__(x=x, y=y, scale=scale)
 
         self._axesparams = "box"
 
         self._width = width
         self._height = height
 
         self.padding = padding
         self._newxmin = padding
-        self._newxmax = width - padding
+        self._newxmax = width - padding - 1
 
-        self._newymin = height - padding
+        self._newymin = height - padding - 1
         self._newymax = padding
 
         self._cartesianfirst = True
         self._loggingfirst = True
 
         self._showtext = False
 
@@ -124,34 +123,41 @@
 
         self._barcolor = 0x69FF8F
 
         self._piecolor = 0x8B77FF
 
         self._index_colorused = 4
 
-        self._plotbitmap = displayio.Bitmap(width, height, 14)
+        self._plotbitmap = displayio.Bitmap(width, height, 20)
 
         if show_box:
             self._drawbox()
 
-        self._plot_palette = displayio.Palette(14)
+        self._plot_palette = displayio.Palette(20)
         self._plot_palette[0] = background_color
         self._plot_palette[1] = box_color
         self._plot_palette[2] = self._tickcolor
         self._plot_palette[3] = self._barcolor
         self._plot_palette[4] = 0x149F14  # Pie Chart color 1
         self._plot_palette[5] = 0x647182  # Pie Chart color 2
         self._plot_palette[6] = 0x7428EF  # Pie Chart color 3
         self._plot_palette[7] = 0x005E99  # Pie Chart color 4
         self._plot_palette[8] = 0x00A76D  # Pie Chart color 5
         self._plot_palette[9] = 0x2C4971  # Pie Chart color 6
         self._plot_palette[10] = 0x64A813
         self._plot_palette[11] = 0x0F4E12
         self._plot_palette[12] = 0xF0075E
-        self._plot_palette[13] = 0x1AF0FF
+        self._plot_palette[13] = 0x123456
+        self._plot_palette[14] = 0xFF00FF
+        self._plot_palette[15] = 0xFF0000
+        self._plot_palette[16] = 0x440044
+        self._plot_palette[17] = 0x2222FF
+        self._plot_palette[18] = 0x1A50FF
+        self._plot_palette[19] = 0xF0FF32
+
         self.append(
             displayio.TileGrid(
                 self._plotbitmap, pixel_shader=self._plot_palette, x=0, y=0
             )
         )
 
     def axs_params(self, axstype: Literal["box", "cartesian", "line"] = "box") -> None:
@@ -176,48 +182,52 @@
         if self._axesparams == "cartesian":
             draw_box = [True, True, False, False]
         elif self._axesparams == "line":
             draw_box = [False, True, False, False]
         else:
             draw_box = [True, True, True, True]
 
+        # left y axes line
         if draw_box[0]:
             # y axes line
             draw_line(
                 self._plotbitmap,
                 self.padding,
                 self.padding,
                 self.padding,
-                self._height - self.padding,
+                self._height - self.padding - 1,
                 1,
             )
+        # bottom x axes line
         if draw_box[1]:
             draw_line(
                 self._plotbitmap,
                 self.padding,
-                self._height - self.padding,
-                self._width - self.padding,
-                self._height - self.padding,
+                self._height - self.padding - 1,
+                self._width - self.padding - 1,
+                self._height - self.padding - 1,
                 1,
             )
+        # right y axes line
         if draw_box[2]:
             draw_line(
                 self._plotbitmap,
-                self._width - self.padding,
+                self._width - self.padding - 1,
                 self.padding,
-                self._width - self.padding,
-                self._height - self.padding,
+                self._width - self.padding - 1,
+                self._height - self.padding - 1,
                 1,
             )
+        # top x axes line
         if draw_box[3]:
             draw_line(
                 self._plotbitmap,
                 self.padding,
                 self.padding,
-                self._width - self.padding,
+                self._width - self.padding - 1,
                 self.padding,
                 1,
             )
 
     def draw_circle(self, radius: int = 5, x: int = 100, y: int = 100) -> None:
         """
         Draw a circle in the plot area
@@ -378,14 +388,16 @@
         self._tickheighty = ticky_height
         self._plot_palette[2] = tickcolor
         self._tickgrid = tickgrid
         self._showtext = showtext
         if self._showtext:
             from adafruit_display_text import bitmap_label
 
+            self.bitmap_label = bitmap_label
+
     def _draw_gridx(self, ticks_data: list[int]) -> None:
         """
         Draws the plot grid
 
         :param list[int] ticks_data: ticks data information
 
         :return: None
@@ -437,23 +449,23 @@
         self._drawbox()
 
     def show_text(
         self, text: str, x: int, y: int, anchorpoint: Tuple = (0.5, 0.0)
     ) -> None:
         """
 
-        Show desired text in the scree
+        Show desired text in the screen
         :param str text: text to be displayed
         :param int x: x coordinate
         :param int y: y coordinate
         :param Tuple anchorpoint: Display_text anchor point. Defaults to (0.5, 0.0)
         :return: None
         """
         if self._showtext:
-            text_toplot = bitmap_label.Label(terminalio.FONT, text=text, x=x, y=y)
+            text_toplot = self.bitmap_label.Label(terminalio.FONT, text=text, x=x, y=y)
             text_toplot.anchor_point = anchorpoint
             text_toplot.anchored_position = (x, y)
             self.append(text_toplot)
 
 
 # pylint: disable=missing-class-docstring, too-few-public-methods, invalid-name
 class color:
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot/uscatter.py` & `circuitpython-uplot-1.0.0/circuitpython_uplot/scatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 
 """
 
-`uscatter`
+`scatter`
 ================================================================================
 
 CircuitPython scatter graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Optional, Union
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 
 
 from ulab import numpy as np
 import displayio
 from vectorio import Circle
 
-__version__ = "0.9.4"
+__version__ = "1.0.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
-# pylint: disable=too-few-public-methods, invalid-name, duplicate-code, too-many-locals, too-many-arguments
-class uscatter:
+class Scatter:
     """
     Main class to display different graphics
     """
 
     def __init__(
         self,
-        plot: Uplot,
+        plot: Plot,
         x: Union[list, np.linspace, np.ndarray],
         y: Union[list, np.linspace, np.ndarray],
         rangex: Optional[list] = None,
         rangey: Optional[list] = None,
         radius: Optional[Union[list, int]] = 3,
         circle_color: int = 0xFF905D,
         nudge: bool = True,
@@ -95,15 +94,14 @@
             for i, _ in enumerate(x):
                 plot.append(
                     Circle(
                         pixel_shader=palette, radius=radius[i], x=xnorm[i], y=ynorm[i]
                     )
                 )
         else:
-
             for i, _ in enumerate(x):
                 plot.append(
                     Circle(pixel_shader=palette, radius=radius, x=xnorm[i], y=ynorm[i])
                 )
 
         if plot._showticks:
             plot._draw_ticks(x, y)
```

### Comparing `circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/PKG-INFO` & `circuitpython-uplot-1.0.0/circuitpython_uplot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 0.9.4
+Version: 1.0.0
 Summary: framework to display different plots in displayio. similar to widget
-Author-email: "Jose D. Montoya" <uplot@mailmeto.mozmail.com>
+Author-email: JDM <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
-Keywords: adafruit,blinka,circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,displayio,circuitpython,graphics,plot,library,plotting,ulab
+Keywords: circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,line,displayio,graphics,library,ulab,svg,widget,graph,graphing,chart,charts,plotting,plot,plotter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -20,34 +20,48 @@
     :target: https://circuitpython-uplot.readthedocs.io/
     :alt: Documentation Status
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/workflows/Build%20CI/badge.svg
     :target: https://github.com/jposada202020/CircuitPython_uplot/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/pypi/v/circuitpython-uplot.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/circuitpython-uplot
+
+.. image:: https://static.pepy.tech/personalized-badge/circuitpython-uplot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/circuitpython-uplot
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Framework to display different plots in displayio. Similar to widget.
+Framework to display different graphical plots in displayio.
 Take a look in the `examples <https://circuitpython-uplot.readthedocs.io/en/latest/examples.html>`_ section in RTD to see the gallery
 
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
+
+
+Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+
+.. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
+
 
 Dependencies
 =============
 This library depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
-This library is ressource consuming, may or may not with some CircuitPython supported devices.
+This library is resource consuming, may or may not with some CircuitPython supported devices.
 Tinker it as you wish in order to work.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
@@ -112,10 +126,8 @@
 =============
 API documentation for this library can be found on `Read the Docs <https://circuitpython-uplot.readthedocs.io/>`_.
 
 
 Contributing
 ============
 
-Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/jposada202020/CircuitPython_uplot/blob/HEAD/CODE_OF_CONDUCT.md>`_
-before contributing to help this project stay welcoming.
+Contributions are welcome!
```

### Comparing `circuitpython-uplot-0.9.4/docs/api.rst` & `circuitpython-uplot-1.0.0/docs/api.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,35 @@
+Uplot Library
+==============
 
-.. If you created a package, create one automodule per module in the package.
+.. automodule:: circuitpython_uplot.plot
+    :members:
+
+.. automodule:: circuitpython_uplot.scatter
+    :members:
+
+.. automodule:: circuitpython_uplot.bar
+    :members:
 
-.. automodule:: circuitpython_uplot.uplot
+.. automodule:: circuitpython_uplot.pie
     :members:
 
-.. automodule:: circuitpython_uplot.uscatter
+.. automodule:: circuitpython_uplot.cartesian
     :members:
 
-.. automodule:: circuitpython_uplot.ubar
+.. automodule:: circuitpython_uplot.fillbetween
     :members:
 
-.. automodule:: circuitpython_uplot.upie
+.. automodule:: circuitpython_uplot.map
     :members:
 
-.. automodule:: circuitpython_uplot.ucartesian
+.. automodule:: circuitpython_uplot.logging
     :members:
 
-.. automodule:: circuitpython_uplot.ufillbetween
+.. automodule:: circuitpython_uplot.svg
     :members:
 
-.. automodule:: circuitpython_uplot.umap
+.. automodule:: circuitpython_uplot.shade
     :members:
 
-.. automodule:: circuitpython_uplot.ulogging
+.. automodule:: circuitpython_uplot.polar
     :members:
```

### Comparing `circuitpython-uplot-0.9.4/docs/index.rst` & `circuitpython-uplot-1.0.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 .. include:: ../docs/quick_start.rst
 
 
 Table of Contents
 =================
 
 .. toctree::
-    :maxdepth: 2
+    :maxdepth: 4
     :hidden:
 
     self
 
 .. toctree::
     :caption: Examples
```

### Comparing `circuitpython-uplot-0.9.4/docs/quick_start.rst` & `circuitpython-uplot-1.0.0/docs/quick_start.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 A small tour for uplot.
 
 
 Plot Usage
 =============
-We start importing some fundamental libraries for uplot to operate
+We start importing some fundamental libraries for plot to operate
 
 .. code-block:: python
 
     import board
     import displayio
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.plot import Plot
 
 For reference, screen in CircuitPython are defined from left to right and up to bottom. This means
 that our (x=0, y=0) will be in the left upper corner of the screen.
 For boards or feather with a integrated screen the following statement will initiate the scree
 
 .. code-block:: python
 
@@ -21,23 +21,28 @@
 
 For other displays please consult the right support library
 
 We add the plot area. in this case we are selecting the whole screen as our plot area
 
 .. code-block:: python
 
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
-The Uplot will be used to display our graphics. The position and the size of the plot area
+The Plot will be used to display our graphics. The position and the size of the plot area
 could vary. This allows us to have more than 1 plot at the same time in the screen.
 Every one of them with different characteristics or graphs.
 
 Options available are:
+    * width: width of the plot area
+    * height: height of the plot area
     * backround_color: Allows to change the background color. The default is black.
     * box_color: Allows to change the box color. Default is white.
+    * padding: allows the user to give the plot area a pad. This is helpful if you are planning to include text and legends in the axes.
+    * scale: scale of the plot. This will allow a plot to be scaled up at a user defined rate. This is currently only available for logging and bar plots.
+
 
 We tell the microcontroller to display our plot:
 
 .. code-block:: python
 
     display.show(plot)
 
@@ -51,15 +56,15 @@
 Graphics
 ===========
 
 At the moment the following objects can be added to the plot area:
 
 * Elements in the library
     * Cartesian Plane
-    * Ufillbetween graph
+    * Fillbetween graph
     * Stackplot
     * Bar graph
     * Pie Chart
     * Colormap
 * Display_shapes library objects
 * Histograms from the uhistogram library
 * Boxplots from the uboxplot library
@@ -71,49 +76,49 @@
 library
 
 .. code-block:: python
 
     import board
     from adafruit_display_shapes.polygon import Polygon
     from adafruit_display_shapes.roundrect import RoundRect
-    from circuitpython_uplot.uplot import Uplot
+    from circuitpython_uplot.uplot import Plot
 
     display = board.DISPLAY
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
     roundrect = RoundRect(30, 30, 61, 81, 10, fill=0x0, outline=0xFF00FF, stroke=6)
     plot.append(roundrect)
     display.show(plot)
 
 
 
 Ticks and Grid
 ===============
 Plot axes are shown by default. To change this behaviour you would need
-to use the correct keyword in the `Uplot.axs_params` function:
+to use the correct keyword in the `Plot.axs_params` function:
 
-.. py:function:: Uplot.axs_params(axstype: Literal["box", "cartesian", "line"] = "box")
+.. py:function:: Plot.axs_params(axstype: Literal["box", "cartesian", "line"] = "box")
 
    :param axstype: Option to display the axes
 
 Options available are:
     * box : draws a box
     * cartesian: draws the left and bottom axes
     * line: draws the bottom axis
 
 The following snippet shows how to create a cartesian plot
 
 .. code-block:: python
 
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
     plot.axs_params(axstype="cartesian")
 
 Tick spacing and numbers are selected by default. However it's possible to customize
 the following parameters:
 
-.. py:function:: Uplot.tick_params(tickx_height, ticky_height, tickcolor, tickgrid)
+.. py:function:: Plot.tick_params(tickx_height, ticky_height, tickcolor, tickgrid)
 
    :param int tickx_height: tickx_height in pixels
    :param int ticky_height: ticky_height in pixels
    :param int tickcolor: tickcolor in Hex format
    :param bool tickgrid: displays the tickgrid. Defaults to `False`
 
 .. code-block:: python
@@ -130,32 +135,31 @@
 
 Colors
 ===============
 You can choose some colors directly from the library. This can be done by importing the color class:
 
 .. code-block:: python
 
-    from circuitpython_uplot.uplot import color
+    from circuitpython_uplot.plot import color
 
 This will allow you to use the colors in the list as color variable definitions
-
     * WHITE
     * BLACK
     * RED
     * GREEN
     * BLUE
     * PURPLE
     * YELLOW
     * ORANGE
     * TEAL
     * GRAY
 
 .. code-block:: python
 
-    plot = Uplot(0, 0, display.width, display.height, background_color=color.WHITE, box_color=color.BLACK)
+    plot = Plot(0, 0, display.width, display.height, background_color=color.WHITE, box_color=color.BLACK)
 
 
 
 ===========
 Cartesian
 ===========
 With the cartesian class it's possible to add (x,y) plots. You can add different (x,y) plots to the
@@ -163,80 +167,79 @@
 for the plot. Secondly, you will need to give some ``x`` and ``y`` data.
 This data will be converted to a `ulab.numpy.ndarray`. For more information please refer
 to the `ulab` library
 
 .. code-block:: python
 
     from ulab import numpy as np
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.ucartesian import ucartesian
+    from circuitpython_uplot.plot import Plot
+    from circuitpython_uplot.cartesian import Cartesian
     display = board.DISPLAY
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
     x = np.linspace(-4, 4, num=25)
     constant = 1.0 / np.sqrt(2 * np.pi)
     y = constant * np.exp((-(x**2)) / 2.0)
 
 After the initial setup we add our xy plane and show our plot
 
 .. code-block:: python
 
-    ucartesian(plot, x, y)
+    Cartesian(plot, x, y)
     display.show(plot)
 
 
 There are some parameters that you can customize:
-
     * rangex and rangey: you could specify the ranges of your graph. Allowing you to move your graph according to your needs. This parameters only accept lists
     * line color: you could specify the color in HEX
     * fill: if you selected this as `True` the area under your graph will be filled
     * nudge: this parameter allows yuo to move a little bit the graph. This is useful when the data start/end in the limits of your range
 
 With the following code, we are setting up the x axis to [-5, 5]
 the y axis to [0, 1], line color to Green :const:`0x00FF00` and no filling
 
 
 .. code-block:: python
 
     x = np.linspace(-3, 3, num=50)
     constant = 2.0 / np.sqrt(2 * np.pi)
     y = constant * np.exp((-(x**2)) / 2.0)
-    ucartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0x00FF00)
+    Cartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0x00FF00)
 
 
 if you want to add more than un line to your plot, you could do something like this:
 
 .. code-block:: python
 
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
     x = np.linspace(-4, 4, num=25)
     y1 = x**2 / 2
     y2 = 2 + x**2 + 3 * x
-    ucartesian(plot, x, y1)
-    ucartesian(plot, x, y1)
+    Cartesian(plot, x, y1)
+    Cartesian(plot, x, y1)
     display.show(plot)
 
 
 ===============
 Pie Chart
 ===============
 
-You can easily create Pie charts with uplot. Pie Charts are limited to 6 elements as per the automatic coloring.
+You can easily create Pie charts with plot. Pie Charts are limited to 6 elements as per the automatic coloring.
 To make the Pie Chart the data needs to be in a python list form. The library will take care of the rest
 
 .. code-block:: python
 
     import board
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.upie import upie
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.pie import Pie
 
     display = board.DISPLAY
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
     a = [5, 2, 7, 3]
-    upie(plot, a)
+    Pie(plot, a)
     display.show(plot)
 
 There are no other special parameters to customize
 
 ===============
 Scatter
 ===============
@@ -244,139 +247,260 @@
 
 .. code-block:: python
 
 
     from random import choice
     import board
     from ulab import numpy as np
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.uscatter import uscatter
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.scatter import Scatter
 
     display = board.DISPLAY
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
     a = np.linspace(1, 100)
     b = [choice(a) for _ in a]
-    uscatter(plot, a, b)
+    Scatter(plot, a, b)
 
 
 There are some parameters that you can customize:
-
     * rangex and rangey: you can specify the ranges of your graph. This allows you to move your graph according to your needs. This parameters only accept lists
     * radius: circles radius/radii
     * circle_color: you can specify the color in HEX
     * nudge: this parameter allows you to move the graph slighty. This is useful when the data start/end in the limits of your range
 
 
 .. code-block:: python
 
     a = np.linspace(1, 200, 150)
     z = [4, 5, 6, 7, 8]
     radi = [choice(z) for _ in a]
     b = [choice(a) for _ in a]
-    uscatter(plot, a, b, rangex=[0,210], rangey=[0, 210], radius=radi, circle_color=0xF456F3)
+    Scatter(plot, a, b, rangex=[0,210], rangey=[0, 210], radius=radi, circle_color=0xF456F3)
 
 ===============
 Bar Plot
 ===============
 
 Allows you to graph bar plots. You just need to give the values of the bar in a python list.
-You can choose to create shell or filled bars
+You can choose to create shell or filled bars.
 
 .. code-block:: python
 
     import board
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.ubar import ubar
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.bar import Bar
 
     display = board.DISPLAY
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
 
     a = ["a", "b", "c", "d"]
     b = [3, 5, 1, 7]
-    ubar(plot, a, b)
+    Bar(plot, a, b)
 
 
 You can select the color or and if the bars are filled
 
 .. code-block:: python
 
-    ubar(plot, a, b, 0xFF1000, True)
+    Bar(plot, a, b, 0xFF1000, True)
+
+
+You can also select the bar spacing and the xstart position:
+
+.. code-block:: python
+
+    Bar(plot, a, b, 0xFF1000, fill=True, bar_space=30, xstart=70)
+
+For bar filled graphs you can pass a color_palette list. This will allow you to select the color of each bar
+This will not work for shell bars sadly.
+
+.. code-block:: python
+
+    import board
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.bar import Bar
+
+    display = board.DISPLAY
+    plot = Plot(0, 0, display.width, display.height)
+    Bar(plot, a, b, fill=True, bar_space=30, xstart=70, color_palette=[0xFF1000, 0x00FF00, 0x0000FF, 0x00FFFF])
+
+
+with the projection argument you can show the bars with projection. This will give them a 3D
+appearance
+
+.. code-block:: python
+
+    import board
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.bar import bar
+
+    display = board.DISPLAY
+    plot = Plot(0, 0, display.width, display.height)
+
+
+    a = ["a", "b", "c", "d"]
+    b = [3, 5, 1, 7]
+    Bar(plot, a, b, color=0xFF1000, fill=True, bar_space=30, xstart=70, projection=True)
+
+
+For filled unprojected bars you can update their values. This is useful for data logging.
+The max_value argument will allow you to set the maximum value of the graph. The plot will scale
+according to this max value, and bar plot will update their values accordingly
+
+.. code-block:: python
+
+    import board
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.bar import Bar
+
+    display = board.DISPLAY
+    plot = Plot(0, 0, display.width, display.height)
+
+
+    a = ["a", "b", "c", "d"]
+    b = [3, 5, 1, 7]
+    my_bar = Bar(plot, a, b, color=0xFF1000, fill=True, color_palette=[0xFF1000, 0x00FF00, 0xFFFF00, 0x123456], max_value=10)
+
+Then you can update the values of the bar plot:
+
+.. code-block:: python
+
+    my_bar.update_values([1, 2, 3, 4])
+
+
+Also for Filled unprojected bars you can change all bars color at once. The following
+code will change all the bar's color to red
+
+.. code-block:: python
+
+    my_bar.update_colors(0xFF0000, 0xFF0000, 0xFF0000, 0xFF0000)
+
+If you prefer, you can change the color of a single bar using the following code:
+
+.. code-block:: python
+
+    my_bar.update_bar_color(0, 0x0000FF)
+
+This will change the first bar to Blue.
+
 
 
 ===============
 Fillbetween
 ===============
 This is a special case of cartesian graph and has all the attributes of that class. However,
 it will fill the area between two curves:
 
 .. code-block:: python
 
 
     import board
     from ulab import numpy as np
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.ufillbetween import ufillbetween
+    from circuitpython_uplot.uplot import Plot
+    from circuitpython_uplot.fillbetween import Fillbetween
 
 
     display = board.DISPLAY
 
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
     x = np.linspace(0, 8, num=25)
 
     y1 = x**2 / 2
     y2 = 2 + x**2 + 3 * x
 
-    ufillbetween(plot, x, y1, y2)
+    Fillbetween(plot, x, y1, y2)
 
     display.show(plot)
 
 ===============
 Color Map
 ===============
 
 Allows you to graph color maps. You just need to give the values in a ulab.numpy.array.
 You can choose the initial and final colors for the color map.
 
 .. code-block:: python
 
     import board
     from ulab import numpy as np
-    from circuitpython_uplot.uplot import Uplot
-    from circuitpython_uplot.umap import umap
+    from circuitpython_uplot.plot import Plot
+    from circuitpython_uplot.map import Map
 
 
     display = board.DISPLAY
 
-    plot = Uplot(0, 0, display.width, display.height, show_box=False)
+    plot = Plot(0, 0, display.width, display.height, show_box=False)
 
     x = np.array(
         [
             [1, 3, 9, 25],
             [12, 8, 4, 2],
             [18, 3, 7, 5],
             [2, 10, 9, 22],
             [8, 8, 14, 12],
             [3, 13, 17, 15],
         ],
         dtype=np.int16,
     )
 
-    umap(plot, x, 0xFF0000, 0x0000FF)
+    Map(plot, x, 0xFF0000, 0x0000FF)
 
     display.show(plot)
 
 
 ===============
 Logging
 ===============
 
 This is a similar to Cartesian but designed to allow the user to use it as a data logger.
-The user needs to setup manually the range and tick values in order for this graph to work proeprly
+The user needs to manually set up the range and tick values in order for this graph to work properly
+
+There are some parameters that you can customize:
+    * rangex and rangey: you need specify the ranges of your graph. This allows you to move your graph according to your needs. This parameters only accept lists
+    * ticksx and ticksy: Specific ticks for the X and Y axes
+    * line_color: you can specify the color in HEX
+    * tick_pos: Allows to show the ticks below the axes.
+    * fill: generates lines under each point, to fill the area under the points
+
 
 .. code-block:: python
 
-    plot = Uplot(0, 0, display.width, display.height)
+    plot = Plot(0, 0, display.width, display.height)
 
-    ulogging(plot, x, y, rangex=[0, 200], rangey=[0, 100], ticksx=[10, 50, 80, 100], ticksy=[15, 30, 45, 60],)
+    x = [10, 20, 30, 40, 50]
+    temp_y = [10, 15, 35, 10, 25]
+
+    my_log = Logging(plot, x, y, rangex=[0, 200], rangey=[0, 100], ticksx=[10, 50, 80, 100], ticksy=[15, 30, 45, 60],)
+
+
+if you want to redraw new data in the same plot, you could do something like this:
+
+.. code-block:: python
+
+
+    x_new = [10, 20, 30, 40, 50]
+    y_new = [26, 50, 26, 50, 26]
+
+    my_log.draw_points(plot_1, x_new, y_new)
+
+
+===============
+SVG
+===============
+
+A small module to load, locate and scale svg path collection of points in the plot area. This will tend to be memory consuming as some SVG will have several path points.
+There are some pre-provided icons in the ``icons.py`` file, you could add more if needed.
+Specific icons are stored as a dictionary in the icons.py file. Every path is a entry in the dictionary.
+For example, if you want to load the Temperature icon with a scale of 2
+
+.. code-block:: python
+
+    from circuitpython_uplot.svg import SVG
+    from circuitpython_uplot.icons import Temperature
+
+    display = board.DISPLAY
+    plot = Plot(0, 0, display.width, display.height)
+    SVG(plot, Temperature, 250, 50, 2)
+    display.show(plot)
```

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif` & `circuitpython-uplot-1.0.0/docs/uplot_cartesian.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex1.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex10.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_cartesian_advance.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex12.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg` & `circuitpython-uplot-1.0.0/docs/fillbetween_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex16.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg` & `circuitpython-uplot-1.0.0/docs/map.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex3.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex4.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex5.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_ex6.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg` & `circuitpython-uplot-1.0.0/docs/bar_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg` & `circuitpython-uplot-1.0.0/docs/uplot_pie.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_display_shapes.py` & `circuitpython-uplot-1.0.0/examples/uplot_display_shapes.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
 from adafruit_display_shapes.polygon import Polygon
 from adafruit_display_shapes.roundrect import RoundRect
-from circuitpython_uplot.uplot import Uplot
+from circuitpython_uplot.plot import Plot
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Setting up tick parameters
 plot.tick_params(tickx_height=12, ticky_height=12, tickcolor=0xFF0008, tickgrid=True)
 plot.axs_params(axstype="box")
 
 # Creating some shapes to show
 polygon = Polygon(
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_integration_example.py` & `circuitpython-uplot-1.0.0/examples/uplot_integration_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import board
 from ulab import numpy as np
 from uhistogram import Histogram
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.cartesian import Cartesian
 
 # Setting Up the histogram
 data = [5, 4, 3, 2, 7, 5, 3, 3, 3, 3, 2, 9, 7, 6]
 my_box = Histogram(data, x=50, y=50, width=100, height=100)
 my_box.draw()
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Seeting some date to plot
 x = np.linspace(-4, 4, num=50)
 constant = 1.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 2.0)
 
 # Plotting and showing the plot
-ucartesian(plot, x, y)
+Cartesian(plot, x, y)
 
 # Adding a circle
 plot.draw_circle(radius=8, x=120, y=120)
 
 # Showing in the screen
 display.show(plot)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_plot_example.py` & `circuitpython-uplot-1.0.0/examples/uplot_plot_example.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.cartesian import Cartesian
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Creating some points to graph
 x = np.linspace(-4, 4, num=25)
 constant = 1.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 2.0)
 
 # Drawing the graph
-ucartesian(plot, x, y)
+Cartesian(plot, x, y)
 
 display.show(plot)
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_readme_example.py` & `circuitpython-uplot-1.0.0/examples/uplot_readme_example.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,93 +2,93 @@
 #
 # SPDX-License-Identifier: MIT
 
 from random import choice
 import board
 import displayio
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ubar import ubar
-from circuitpython_uplot.uscatter import uscatter
-from circuitpython_uplot.upie import upie
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.bar import Bar
+from circuitpython_uplot.scatter import Scatter
+from circuitpython_uplot.pie import Pie
+from circuitpython_uplot.cartesian import Cartesian
 
 
 display = board.DISPLAY
-plot = Uplot(0, 0, display.width, display.height, show_box=False)
+plot = Plot(0, 0, display.width, display.height, show_box=False)
 
 group = displayio.Group()
 
 palette = displayio.Palette(1)
 palette[0] = 0xFFFFFF
 
 
-plot2 = Uplot(0, 0, 130, 130)
+plot2 = Plot(0, 0, 130, 130)
 x = np.linspace(-4, 4, num=25)
 constant = 2.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 4.0)
-ucartesian(plot2, x, y, rangex=[-5, 5], rangey=[0, 1])
+Cartesian(plot2, x, y, rangex=[-5, 5], rangey=[0, 1])
 plot.append(plot2)
 
-plot3 = Uplot(130, 0, 160, 160)
+plot3 = Plot(130, 0, 160, 160)
 
 # Setting up tick parameters
 plot3.tick_params(tickx_height=12, ticky_height=12, tickcolor=0xFF00FF, tickgrid=True)
 
 # Seeting some data to plot
 x = np.linspace(-4, 4, num=50)
 constant = 1.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 2.0)
 
 # Plotting and showing the plot
-ucartesian(plot3, x, y, rangex=[-5, 5], rangey=[0, 0.5])
+Cartesian(plot3, x, y, rangex=[-5, 5], rangey=[0, 0.5])
 plot.append(plot3)
 
-plot4 = Uplot(290, 0, 150, 150)
+plot4 = Plot(290, 0, 150, 150)
 
 # Setting up tick parameters
 plot4.axs_params(axstype="box")
 a = ["a", "b", "c", "d"]
 b = [3, 5, 1, 7]
-ubar(plot4, a, b, 0xFF1000, fill=True)
+Bar(plot4, a, b, 0xFF1000, fill=True)
 
 plot.append(plot4)
 
-plot5 = Uplot(0, 180, 120, 120)
+plot5 = Plot(0, 180, 120, 120)
 
 # Setting up tick parameters
 plot5.axs_params(axstype="cartesian")
 a = np.linspace(3, 98)
 b = [choice(a) for _ in a]
-uscatter(plot5, a, b, rangex=[0, 102], rangey=[0, 102], radius=2)
+Scatter(plot5, a, b, rangex=[0, 102], rangey=[0, 102], radius=2)
 
 plot.append(plot5)
 
-plot6 = Uplot(130, 160, 150, 150)
+plot6 = Plot(130, 160, 150, 150)
 
 # Setting up tick parameters
 plot6.axs_params(axstype="box")
 a = [5, 2, 7, 3]
 
-upie(plot6, a, 0, 0)
+Pie(plot6, a, 0, 0)
 
 plot.append(plot6)
 
 
-plot7 = Uplot(290, 160, 150, 150)
+plot7 = Plot(290, 160, 150, 150)
 
 # Creating some points to graph
 x = np.linspace(1, 10, num=10)
 
 y = [6, 7, 9, 6, 9, 7, 6, 6, 8, 9]
-ucartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF0000, fill=True)
+Cartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF0000, fill=True)
 
 y = [4, 3, 7, 8, 3, 9, 3, 2, 1, 2]
-ucartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF00FF, fill=True)
+Cartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF00FF, fill=True)
 
 y = [1, 4, 6, 3, 6, 6, 5, 0, 9, 2]
-ucartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0x4444FF, fill=True)
+Cartesian(plot7, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0x4444FF, fill=True)
 
 plot.append(plot7)
 
 # Plotting and showing the plot
 display.show(plot)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_sparkline.py` & `circuitpython-uplot-1.0.0/examples/uplot_sparkline.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
 from ulab import numpy as np
 from adafruit_display_shapes.sparkline import Sparkline
-from circuitpython_uplot.uplot import Uplot, color
+from circuitpython_uplot.plot import Plot, color
 
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # 500 linearly spaced numbers
 x = np.linspace(-10 * np.pi, 10 * np.pi, 500)
 
 # the function, which is y = sin(x) here
 y = np.sin(x)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_stackplot.py` & `circuitpython-uplot-1.0.0/examples/uplot_stackplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 """
 Example to show how to draw stackplots
 """
 
 import time
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.cartesian import Cartesian
 
 # Setting up the display
 display = board.DISPLAY
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Creating some points to graph
 x = np.linspace(1, 10, num=10)
 
 y = [6, 7, 9, 6, 9, 7, 6, 6, 8, 9]
-ucartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF0000, fill=True)
+Cartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF0000, fill=True)
 
 y = [4, 3, 7, 8, 3, 9, 3, 2, 1, 2]
-ucartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF00FF, fill=True)
+Cartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0xFF00FF, fill=True)
 
 y = [1, 4, 6, 3, 6, 6, 5, 0, 9, 2]
-ucartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0x4444FF, fill=True)
+Cartesian(plot, x, y, rangex=[0, 11], rangey=[0, 12], line_color=0x4444FF, fill=True)
 
 
 display.show(plot)
 
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_tickparameters.py` & `circuitpython-uplot-1.0.0/examples/uplot_bar_color_changing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
-from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot, color
-from circuitpython_uplot.ucartesian import ucartesian
-
+from circuitpython_uplot.plot import Plot, color
+from circuitpython_uplot.bar import Bar
 
 # Setting up the display
 display = board.DISPLAY
 
-# Setting up the plot area
-plot = Uplot(
+# Configuring display dimensions
+DISPLAY_WIDTH = 480
+DISPLAY_HEIGHT = 320
+
+# Defining the plot
+plot = Plot(
     0,
     0,
-    display.width,
-    display.height,
-    background_color=color.WHITE,
-    box_color=color.BLACK,
+    DISPLAY_WIDTH,
+    DISPLAY_HEIGHT,
+    background_color=color.BLACK,
+    padding=10,
+    box_color=color.WHITE,
 )
 
-# Setting up tick parameters
-plot.tick_params(tickx_height=12, ticky_height=6, tickcolor=color.BLACK, tickgrid=False)
-# Seeting some date to plot
-x = np.linspace(-4, 4, num=50)
-constant = 1.0 / np.sqrt(2 * np.pi)
-y = constant * np.exp((-(x**2)) / 2.0)
+display.show(plot)
 
-# Drawing the graph
-ucartesian(plot, x, y, line_color=color.BLACK)
+# Dummy data to plot
+some_values = [55, 20, 25, 30, 35, 10]
+a = ["a", "b", "c", "d", "e", "f"]
 
-# Plotting and showing the plot
+# Showing the plot
 display.show(plot)
 
-# Adding some wait time
-while True:
-    time.sleep(1)
+# Creating the bar
+my_bar = Bar(
+    plot,
+    a,
+    some_values,
+    0xFF1000,
+    True,
+    projection=False,
+    max_value=50,
+)
+time.sleep(2)
+# Changing all the bars to Yellow
+my_bar.update_colors(
+    [color.YELLOW, color.YELLOW, color.YELLOW, color.YELLOW, color.YELLOW, color.YELLOW]
+)
+
+time.sleep(2)
+
+# Changing the 3 bar to Purple
+my_bar.update_bar_color(2, color.PURPLE)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_ubar_example.py` & `circuitpython-uplot-1.0.0/examples/uplot_bar_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ubar import ubar
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.bar import Bar
 
 
 # Setting up the display
 display = board.DISPLAY
 
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Setting up tick parameters
 plot.axs_params(axstype="box")
 a = ["a", "b", "c", "d"]
 b = [3, 5, 1, 7]
-ubar(plot, a, b, 0xFF1000, True)
+Bar(plot, a, b, 0xFF1000, True)
 
 # Plotting and showing the plot
 display.show(plot)
 
 # Adding some wait time
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_uboxplot.py` & `circuitpython-uplot-1.0.0/examples/uplot_uboxplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 """
-Simple test to display boxplot using uplot
+Simple test to display boxplot using plot
 """
 
 import board
 from uboxplot import Boxplot
-from circuitpython_uplot.uplot import Uplot
+from circuitpython_uplot.plot import Plot
 
 
 display = board.DISPLAY
 
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 plot.tick_params(tickx_height=10, ticky_height=10, tickcolor=0x440008, tickgrid=True)
 
 a = [1, 1, 4, 5, 6, 7, 7, 7, 8, 9, 10, 15, 16, 17, 24, 56, 76, 87, 87]
 my_box = Boxplot(a, x=50, y=50, height=100, line_color=0xFF00FF)
 my_box.draw()
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_ucartesian_advanced.py` & `circuitpython-uplot-1.0.0/examples/uplot_cartesian_advanced.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.cartesian import Cartesian
 
 # Setting up the display
 display = board.DISPLAY
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Creating some points to graph
 x = np.linspace(-4, 4, num=25)
 constant = 1.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 2.0)
 
 # Drawing the graph
-ucartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0xFF0000)
+Cartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0xFF0000)
 
 # Creating some points to graph
 x = np.linspace(-3, 3, num=50)
 constant = 2.0 / np.sqrt(2 * np.pi)
 y = constant * np.exp((-(x**2)) / 2.0)
-ucartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0x00FF00)
+Cartesian(plot, x, y, rangex=[-5, 5], rangey=[0, 1], line_color=0x00FF00)
 
 # Plotting and showing the plot
 display.show(plot)
 
 # Adding some wait time
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_ucartesian_loggin_data.py` & `circuitpython-uplot-1.0.0/examples/uplot_cartesian_loggin_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 import time
 from random import choice
 import displayio
 import terminalio
 import board
 from adafruit_display_text import label
-from circuitpython_uplot.uplot import Uplot, color
-from circuitpython_uplot.ucartesian import ucartesian
+from circuitpython_uplot.plot import Plot, color
+from circuitpython_uplot.cartesian import Cartesian
 
 # Setting up the display
 display = board.DISPLAY
 
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 g = displayio.Group()
 
 DISPLAY_WIDTH = 200
 DISPLAY_HEIGHT = 200
 FOREGROUND_COLOR = color.BLACK
 BACKGROUND_COLOR = color.WHITE
 
@@ -37,26 +37,26 @@
 
 text_humidity = label.Label(terminalio.FONT, color=FOREGROUND_COLOR, scale=3)
 text_humidity.anchor_point = 0.0, 0.0
 text_humidity.anchored_position = 130, 0
 g.append(text_humidity)
 
 
-plot_1 = Uplot(
+plot_1 = Plot(
     0,
     50,
     200,
     60,
     padding=1,
     show_box=True,
     box_color=color.BLACK,
     background_color=color.WHITE,
 )
 
-plot_2 = Uplot(
+plot_2 = Plot(
     0,
     180,
     200,
     60,
     padding=1,
     show_box=True,
     box_color=color.BLACK,
@@ -79,25 +79,25 @@
 g.append(plot_1)
 g.append(plot_2)
 
 display.show(g)
 display.refresh()
 
 for i, element in enumerate(x):
-    ucartesian(
+    Cartesian(
         plot_1,
         x[0:i],
         temp_y[0:i],
         rangex=[0, 143],
         rangey=[0, 40],
         fill=False,
         line_color=color.BLACK,
         logging=True,
     )
-    ucartesian(
+    Cartesian(
         plot_2,
         x[0:i],
         humidity_y[0:i],
         rangex=[0, 143],
         rangey=[0, 100],
         fill=False,
         line_color=color.BLACK,
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_ufillbetween.py` & `circuitpython-uplot-1.0.0/examples/uplot_fillbetween.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.ufillbetween import ufillbetween
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.fillbetween import Fillbetween
 
 
 # Setting up the display
 display = board.DISPLAY
 
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 x = np.linspace(0, 8, num=25)
 
 y1 = x**2 / 2
 y2 = 2 + x**2 + 3 * x
 
-ufillbetween(plot, x, y1, y2)
+Fillbetween(plot, x, y1, y2)
 
 display.show(plot)
 
 # Adding some wait time
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_ulogging.py` & `circuitpython-uplot-1.0.0/examples/uplot_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 #
 # SPDX-License-Identifier: MIT
 
 import displayio
 import terminalio
 import board
 from adafruit_display_text import label
-from circuitpython_uplot.uplot import Uplot, color
-from circuitpython_uplot.ulogging import ulogging
+from circuitpython_uplot.plot import Plot, color
+from circuitpython_uplot.logging import Logging
 
 # Setting up the display
 display = board.DISPLAY
 
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 g = displayio.Group()
 
 DISPLAY_WIDTH = 200
 DISPLAY_HEIGHT = 200
 FOREGROUND_COLOR = color.BLACK
 BACKGROUND_COLOR = color.WHITE
 
@@ -34,15 +34,15 @@
 g.append(text_temperature)
 
 text_humidity = label.Label(terminalio.FONT, color=FOREGROUND_COLOR, scale=3)
 text_humidity.anchor_point = 0.0, 0.0
 text_humidity.anchored_position = 130, 0
 g.append(text_humidity)
 
-plot_1 = Uplot(
+plot_1 = Plot(
     0,
     50,
     200,
     60,
     padding=1,
     show_box=True,
     box_color=color.BLACK,
@@ -59,17 +59,19 @@
 g.append(plot_1)
 
 display.show(g)
 display.refresh()
 
 dist = 3
 
-ulogging(
+Logging(
     plot_1,
     x[0:dist],
     temp_y[0:dist],
     rangex=[0, 200],
     rangey=[0, 100],
     line_color=color.BLACK,
     ticksx=[10, 50, 80, 100],
     ticksy=[15, 30, 45, 60],
 )
+
+text_temperature.text = "{}C".format(temp_y[dist])
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_umap.py` & `circuitpython-uplot-1.0.0/examples/uplot_map.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 #
 # SPDX-License-Identifier: MIT
 
 import time
 from random import choice
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.umap import umap
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.map import Map
 
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height, show_box=False)
+plot = Plot(0, 0, display.width, display.height, show_box=False)
 
 # Setting some date to plot
 x = np.linspace(-4, 4, num=100)
 y = 2.0 / np.sqrt(2 * np.pi) * np.exp((-(x**2)) / 4.0)
 b = [choice(y) for _ in y]
 y1 = np.array(b).reshape((10, 10))
 
 # Plotting and showing the plot
-umap(plot, y1, 0xFF0044, 0x4400FF)
+Map(plot, y1, 0xFF0044, 0x4400FF)
 # Plotting and showing the plot
 display.show(plot)
 
 # Adding some wait time
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/examples/uplot_uscatter.py` & `circuitpython-uplot-1.0.0/examples/uplot_scatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 #
 # SPDX-License-Identifier: MIT
 
 import time
 from random import choice
 import board
 from ulab import numpy as np
-from circuitpython_uplot.uplot import Uplot
-from circuitpython_uplot.uscatter import uscatter
+from circuitpython_uplot.plot import Plot
+from circuitpython_uplot.scatter import Scatter
 
 
 # Setting up the display
 display = board.DISPLAY
 
 # Adding the plot area
-plot = Uplot(0, 0, display.width, display.height)
+plot = Plot(0, 0, display.width, display.height)
 
 # Setting up tick parameters
 plot.tick_params(tickx_height=12, ticky_height=12, tickcolor=0xFF0008, tickgrid=True)
 plot.axs_params(axstype="cartesian")
 a = np.linspace(1, 100)
 b = [choice(a) for _ in a]
-uscatter(plot, a, b)
+Scatter(plot, a, b)
 
 # Plotting and showing the plot
 display.show(plot)
 
 # Adding some wait time
 while True:
     time.sleep(1)
```

### Comparing `circuitpython-uplot-0.9.4/pyproject.toml` & `circuitpython-uplot-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-# SPDX-FileCopyrightText: 2022 Alec Delaney, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 [build-system]
 requires = [
     "setuptools",
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-uplot"
 description = "framework to display different plots in displayio. similar to widget"
-version = "0.9.4"
+version = "1.0.0"
 readme = "README.rst"
 authors = [
-    {name = "Jose D. Montoya", email = "uplot@mailmeto.mozmail.com"}
+    {name = "JDM", email = "uplot@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_uplot"}
 keywords = [
-    "adafruit",
-    "blinka",
     "circuitpython",
     "uplot",
     "bar",
     "stackplot",
     "fillbetween",
     "piechart",
     "scatter",
+    "line",
     "displayio",
-    "circuitpython",
     "graphics",
-    "plot",
     "library",
-    "plotting",
     "ulab",
+    "svg",
+    "widget",
+    "graph",
+    "graphing",
+    "chart",
+    "charts",
+    "plotting",
+    "plot",
+    "plotter",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
```

