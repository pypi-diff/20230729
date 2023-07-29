# Comparing `tmp/voltaire-0.8.9.linux-x86_64.tar.gz` & `tmp/voltaire-0.9.0.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltaire-0.8.9.linux-x86_64.tar", last modified: Fri Jan 15 01:45:20 2021, max compression
+gzip compressed data, was "voltaire-0.9.0.linux-x86_64.tar", last modified: Fri Feb  5 06:54:56 2021, max compression
```

## Comparing `voltaire-0.8.9.linux-x86_64.tar` & `voltaire-0.9.0.linux-x86_64.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/Python/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/Python/3.8.7/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/Python/3.8.7/x64/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.876580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/
--rw-r--r--   0 runner    (1001) docker     (116)      552 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (116)      956 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      232 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)     2633 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/mermaid.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      983 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/pelican.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)    37856 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/search.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)     2435 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/tasks.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)     1224 2021-01-15 01:45:20.884580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/wikilinks.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-01-15 01:45:20.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)       74 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/mermaid.json
--rw-r--r--   0 runner    (1001) docker     (116)     3372 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (116)      872 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/pelican.py
--rw-r--r--   0 runner    (1001) docker     (116)    38455 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/search.py
--rw-r--r--   0 runner    (1001) docker     (116)     2237 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (116)    13038 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/awsm.css
--rw-r--r--   0 runner    (1001) docker     (116)      726 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/common.scss
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.880580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/
--rw-r--r--   0 runner    (1001) docker     (116)      270 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/archives.html
--rw-r--r--   0 runner    (1001) docker     (116)     3423 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/article.html
--rw-r--r--   0 runner    (1001) docker     (116)      179 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/author.html
--rw-r--r--   0 runner    (1001) docker     (116)      343 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/authors.html
--rw-r--r--   0 runner    (1001) docker     (116)     4120 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/categories.html
--rw-r--r--   0 runner    (1001) docker     (116)      823 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/category.html
--rw-r--r--   0 runner    (1001) docker     (116)      606 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/gosquared.html
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (116)      495 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (116)      404 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/pagination.html
--rw-r--r--   0 runner    (1001) docker     (116)      290 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/period_archives.html
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (116)        2 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/tag.html
--rw-r--r--   0 runner    (1001) docker     (116)      306 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/tags.html
--rw-r--r--   0 runner    (1001) docker     (116)      245 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/translations.html
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2021-01-15 01:44:39.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/wikilinks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:45:20.888580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1361 2021-01-15 01:45:20.852579 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1206 2021-01-15 01:45:20.872580 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 01:45:20.852579 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      103 2021-01-15 01:45:20.852579 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-01-15 01:45:20.852579 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.058762 ./
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.058762 ./opt/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.058762 ./opt/hostedtoolcache/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.058762 ./opt/hostedtoolcache/Python/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.058762 ./opt/hostedtoolcache/Python/3.8.7/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.062762 ./opt/hostedtoolcache/Python/3.8.7/x64/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.062762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.062762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.074762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.070762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/
+-rw-r--r--   0 runner    (1001) docker     (116)      635 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.074762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (116)     1003 2021-02-05 06:54:56.070762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)      232 2021-02-05 06:54:56.070762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)     2680 2021-02-05 06:54:56.070762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/mermaid.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)     1154 2021-02-05 06:54:56.074762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/pelican.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)    37856 2021-02-05 06:54:56.074762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/search.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)     3487 2021-02-05 06:54:56.070762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/tasks.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)     1230 2021-02-05 06:54:56.074762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/wikilinks.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2021-02-05 06:54:55.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      273 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/docker-compose.verify.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/mermaid.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3413 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1037 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/pelican.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38455 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/search.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3668 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.066762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.066762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.066762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (116)    13038 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/awsm.css
+-rw-r--r--   0 runner    (1001) docker     (116)      728 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/common.scss
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.066762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)      270 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/archives.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3423 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/article.html
+-rw-r--r--   0 runner    (1001) docker     (116)      179 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/author.html
+-rw-r--r--   0 runner    (1001) docker     (116)      343 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/authors.html
+-rw-r--r--   0 runner    (1001) docker     (116)     4212 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (116)      274 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/categories.html
+-rw-r--r--   0 runner    (1001) docker     (116)      823 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/category.html
+-rw-r--r--   0 runner    (1001) docker     (116)      606 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/gosquared.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1134 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (116)      495 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (116)      404 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (116)      290 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/period_archives.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (116)        2 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/tag.html
+-rw-r--r--   0 runner    (1001) docker     (116)      306 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/tags.html
+-rw-r--r--   0 runner    (1001) docker     (116)      245 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/translations.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1165 2021-02-05 06:54:08.000000 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/wikilinks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-05 06:54:56.078762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1425 2021-02-05 06:54:56.018762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1229 2021-02-05 06:54:56.046762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-05 06:54:56.018762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2021-02-05 06:54:56.018762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-02-05 06:54:56.022762 ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/top_level.txt
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__init__.py

```diff
@@ -15,8 +15,10 @@
     TASKS.add_task(wrapped_task, name=t.__name__)
 
 
 def site(host="localhost", port=8000, domain=None):
     add_task(tasks.build)
     add_task(tasks.livereload, host=host, port=port)
     add_task(tasks.publish, domain=domain)
+    add_task(tasks.stage, domain=domain)
+    add_task(tasks.verify, domain=domain)
     return TASKS
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/__init__.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 552 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 2802 0000  U..........`(...
+00000000: 550d 0d0a 0000 0000 90eb 1c60 7b02 0000  U..........`{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6404 6701 5a05  m.Z.m.Z...d.g.Z.
 00000050: 6503 6405 8301 5a06 6406 6407 8400 5a07  e.d...Z.d.d...Z.
 00000060: 640c 640b 6404 8401 5a08 640a 5300 290d  d.d.d...Z.d.S.).
 00000070: e901 0000 0029 01da 0574 6173 6b73 e900  .....)...tasks..
@@ -35,26 +35,29 @@
 00000220: 534b 53da 0861 6464 5f74 6173 6bda 085f  SKS..add_task.._
 00000230: 5f6e 616d 655f 5f29 0372 0d00 0000 720c  _name__).r....r.
 00000240: 0000 0072 0f00 0000 7209 0000 0072 0b00  ...r....r....r..
 00000250: 0000 720e 0000 0072 1200 0000 0900 0000  ..r....r........
 00000260: 7308 0000 0000 010e 0110 0308 0172 1200  s............r..
 00000270: 0000 da09 6c6f 6361 6c68 6f73 74e9 401f  ....localhost.@.
 00000280: 0000 4e63 0300 0000 0000 0000 0000 0000  ..Nc............
-00000290: 0300 0000 0500 0000 4300 0000 732c 0000  ........C...s,..
+00000290: 0300 0000 0500 0000 4300 0000 7348 0000  ........C...sH..
 000002a0: 0074 0074 016a 0283 0101 0074 0074 016a  .t.t.j.....t.t.j
 000002b0: 037c 007c 0164 018d 0301 0074 0074 016a  .|.|.d.....t.t.j
-000002c0: 047c 0264 028d 0201 0074 0553 0029 034e  .|.d.....t.S.).N
-000002d0: 2902 da04 686f 7374 da04 706f 7274 2901  )...host..port).
-000002e0: da06 646f 6d61 696e 2906 7212 0000 0072  ..domain).r....r
-000002f0: 0200 0000 da05 6275 696c 64da 0a6c 6976  ......build..liv
-00000300: 6572 656c 6f61 645a 0770 7562 6c69 7368  ereloadZ.publish
-00000310: 7211 0000 0029 0372 1600 0000 7217 0000  r....).r....r...
-00000320: 0072 1800 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000330: 720e 0000 0072 0600 0000 1200 0000 7308  r....r........s.
-00000340: 0000 0000 010a 0110 010e 0129 0372 1400  ...........).r..
-00000350: 0000 7215 0000 004e 2909 da00 7202 0000  ..r....N)...r...
-00000360: 00da 0669 6e76 6f6b 6572 0400 0000 7205  ...invoker....r.
-00000370: 0000 005a 075f 5f41 4c4c 5f5f 7211 0000  ...Z.__ALL__r...
-00000380: 0072 1200 0000 7206 0000 0072 0900 0000  .r....r....r....
-00000390: 7209 0000 0072 0900 0000 720e 0000 00da  r....r....r.....
-000003a0: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-000003b0: 0000 0c01 1003 0601 0803 0809            ............
+000002c0: 047c 0264 028d 0201 0074 0074 016a 057c  .|.d.....t.t.j.|
+000002d0: 0264 028d 0201 0074 0074 016a 067c 0264  .d.....t.t.j.|.d
+000002e0: 028d 0201 0074 0753 0029 034e 2902 da04  .....t.S.).N)...
+000002f0: 686f 7374 da04 706f 7274 2901 da06 646f  host..port)...do
+00000300: 6d61 696e 2908 7212 0000 0072 0200 0000  main).r....r....
+00000310: da05 6275 696c 64da 0a6c 6976 6572 656c  ..build..liverel
+00000320: 6f61 645a 0770 7562 6c69 7368 5a05 7374  oadZ.publishZ.st
+00000330: 6167 655a 0676 6572 6966 7972 1100 0000  ageZ.verifyr....
+00000340: 2903 7216 0000 0072 1700 0000 7218 0000  ).r....r....r...
+00000350: 0072 0900 0000 7209 0000 0072 0e00 0000  .r....r....r....
+00000360: 7206 0000 0012 0000 0073 0c00 0000 0001  r........s......
+00000370: 0a01 1001 0e01 0e01 0e01 2903 7214 0000  ..........).r...
+00000380: 0072 1500 0000 4e29 09da 0072 0200 0000  .r....N)...r....
+00000390: da06 696e 766f 6b65 7204 0000 0072 0500  ..invoker....r..
+000003a0: 0000 5a07 5f5f 414c 4c5f 5f72 1100 0000  ..Z.__ALL__r....
+000003b0: 7212 0000 0072 0600 0000 7209 0000 0072  r....r....r....r
+000003c0: 0900 0000 7209 0000 0072 0e00 0000 da08  ....r....r......
+000003d0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+000003e0: 000c 0110 0306 0108 0308 09              ...........
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/_version.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:45:20 2021 UTC, .py size: 142 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,15 +1,15 @@
-00000000: 550d 0d0a 0000 0000 b0f3 0060 8e00 0000  U..........`....
+00000000: 550d 0d0a 0000 0000 bfeb 1c60 8e00 0000  U..........`....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 7a05 302e  Z.d.Z.d.S.).z.0.
-00000040: 382e 3929 03e9 0000 0000 e908 0000 00e9  8.9)............
-00000050: 0900 0000 4e29 02da 0776 6572 7369 6f6e  ....N)...version
+00000040: 392e 3029 03e9 0000 0000 e909 0000 0072  9.0)...........r
+00000050: 0100 0000 4e29 02da 0776 6572 7369 6f6e  ....N)...version
 00000060: da0d 7665 7273 696f 6e5f 7475 706c 65a9  ..version_tuple.
-00000070: 0072 0600 0000 7206 0000 00fa 562f 6f70  .r....r.....V/op
+00000070: 0072 0500 0000 7205 0000 00fa 562f 6f70  .r....r.....V/op
 00000080: 742f 686f 7374 6564 746f 6f6c 6361 6368  t/hostedtoolcach
 00000090: 652f 5079 7468 6f6e 2f33 2e38 2e37 2f78  e/Python/3.8.7/x
 000000a0: 3634 2f6c 6962 2f70 7974 686f 6e33 2e38  64/lib/python3.8
 000000b0: 2f73 6974 652d 7061 636b 6167 6573 2f76  /site-packages/v
 000000c0: 6f6c 7461 6972 652f 5f76 6572 7369 6f6e  oltaire/_version
 000000d0: 2e70 79da 083c 6d6f 6475 6c65 3e04 0000  .py..<module>...
 000000e0: 0073 0200 0000 0401                      .s......
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/mermaid.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 3372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,165 +1,168 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 2c0d 0000  U..........`,...
+00000000: 550d 0d0a 0000 0000 90eb 1c60 550d 0000  U..........`U...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6501  ..d.d.l.m.Z...e.
-00000080: a00d 6406 a101 5a0e 6501 a00d 6407 a101  ..d...Z.e...d...
-00000090: 5a0f 6500 6a10 a011 6500 6a10 a012 6500  Z.e.j...e.j...e.
-000000a0: 6a10 a013 6514 a101 a101 6408 a102 5a15  j...e.....d...Z.
-000000b0: 6508 6508 6409 9c02 640a 640b 8404 5a16  e.e.d...d.d...Z.
-000000c0: 4700 640c 640d 8400 640d 650c 8303 5a17  G.d.d...d.e...Z.
-000000d0: 4700 640e 640f 8400 640f 650a 8303 5a18  G.d.d...d.e...Z.
-000000e0: 6410 6411 8400 5a19 6401 5300 2912 e900  d.d...Z.d.S.)...
-000000f0: 0000 004e 2902 da04 5049 5045 da05 506f  ...N)...PIPE..Po
-00000100: 7065 6e29 02da 0849 7465 7261 626c 65da  pen)...Iterable.
-00000110: 0454 6578 7429 01da 0945 7874 656e 7369  .Text)...Extensi
-00000120: 6f6e 2901 da0c 5072 6570 726f 6365 7373  on)...Preprocess
-00000130: 6f72 7a1d 5e60 6060 5b5c 205c 745d 2a5b  orz.^```[\ \t]*[
-00000140: 4d6d 5d65 726d 6169 645b 5c20 5c74 5d2a  Mm]ermaid[\ \t]*
-00000150: 247a 0c5e 6060 605b 5c20 5c74 5d2a 247a  $z.^```[\ \t]*$z
-00000160: 0c6d 6572 6d61 6964 2e6a 736f 6e29 02da  .mermaid.json)..
-00000170: 0c6d 6572 6d61 6964 5f63 6f64 65da 0672  .mermaid_code..r
-00000180: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-00000190: 0000 0a00 0000 0a00 0000 4300 0000 73f0  ..........C...s.
-000001a0: 0000 0074 006a 0164 0164 028d 017d 017c  ...t.j.d.d...}.|
-000001b0: 01a0 027c 00a0 0364 03a1 01a1 0101 007c  ...|...d.......|
-000001c0: 01a0 04a1 0001 007c 016a 0564 0417 007d  .......|.j.d...}
-000001d0: 0264 0564 067c 016a 0564 077c 0264 0874  .d.d.|.j.d.|.d.t
-000001e0: 0667 077d 037a 1e74 077c 0374 0874 0864  .g.}.z.t.|.t.t.d
-000001f0: 098d 037d 047c 04a0 09a1 005c 027d 057d  ...}.|.....\.}.}
-00000200: 0657 006e 2e04 0074 0a6b 0a72 8e01 007d  .W.n...t.k.r...}
-00000210: 0701 007a 1074 0a64 0a7c 0716 0083 0182  ...z.t.d.|......
-00000220: 0157 0035 0064 0b7d 077e 0758 0059 006e  .W.5.d.}.~.X.Y.n
-00000230: 5e58 007c 046a 0b64 0c6b 0272 d074 0ca0  ^X.|.j.d.k.r.t..
-00000240: 0d7c 016a 05a1 0101 0074 0e7c 0283 018f  .|.j.....t.|....
-00000250: 0e7d 087c 08a0 0fa1 007d 0957 0035 0051  .}.|.....}.W.5.Q
-00000260: 0052 0058 0074 0ca0 0d7c 02a1 0101 007c  .R.X.t...|.....|
-00000270: 0953 0074 1064 0d7c 069b 0064 0e7c 016a  .S.t.d.|...d.|.j
-00000280: 059b 0064 0f7c 029b 009d 0683 0182 0164  ...d.|.........d
-00000290: 0b53 0029 107a 8a0a 2020 2020 436f 6e76  .S.).z..    Conv
-000002a0: 6572 7473 204d 6572 6d61 6964 2073 6f75  erts Mermaid sou
-000002b0: 7263 6520 636f 6465 2074 6f20 5356 472e  rce code to SVG.
-000002c0: 0a20 2020 203a 7061 7261 6d20 6d65 726d  .    :param merm
-000002d0: 6169 645f 636f 6465 3a20 4d65 726d 6169  aid_code: Mermai
-000002e0: 6420 696e 7075 7420 636f 6465 2061 7320  d input code as 
-000002f0: 6120 7374 7269 6e67 2e0a 2020 2020 3a72  a string..    :r
-00000300: 6574 7572 6e3a 2053 5647 2063 6f64 6520  eturn: SVG code 
-00000310: 6173 2061 2073 7472 696e 672e 0a20 2020  as a string..   
-00000320: 2046 2901 da06 6465 6c65 7465 da04 7574   F)...delete..ut
-00000330: 6638 7a04 2e73 7667 5a04 6d6d 6463 7a02  f8z..svgZ.mmdcz.
-00000340: 2d69 7a02 2d6f 7a02 2d63 2902 da06 7374  -iz.-oz.-c)...st
-00000350: 646f 7574 da06 7374 6465 7272 7a19 4661  dout..stderrz.Fa
-00000360: 696c 6564 2074 6f20 7275 6e20 6d65 726d  iled to run merm
-00000370: 6169 643a 2025 734e 7201 0000 007a 1745  aid: %sNr....z.E
-00000380: 7272 6f72 2063 616c 6c69 6e67 206d 6572  rror calling mer
-00000390: 6d61 6964 3a20 7a0d 0a54 656d 7020 6669  maid: z..Temp fi
-000003a0: 6c65 733a 207a 0520 616e 6420 2911 da08  les: z. and )...
-000003b0: 7465 6d70 6669 6c65 da12 4e61 6d65 6454  tempfile..NamedT
-000003c0: 656d 706f 7261 7279 4669 6c65 da05 7772  emporaryFile..wr
-000003d0: 6974 65da 0665 6e63 6f64 65da 0566 6c75  ite..encode..flu
-000003e0: 7368 da04 6e61 6d65 da09 434f 4e46 5f46  sh..name..CONF_F
-000003f0: 494c 4572 0300 0000 7202 0000 00da 0b63  ILEr....r......c
-00000400: 6f6d 6d75 6e69 6361 7465 da09 4578 6365  ommunicate..Exce
-00000410: 7074 696f 6eda 0a72 6574 7572 6e63 6f64  ption..returncod
-00000420: 65da 026f 73da 0672 656d 6f76 65da 046f  e..os..remove..o
-00000430: 7065 6eda 0472 6561 64da 0c52 756e 7469  pen..read..Runti
-00000440: 6d65 4572 726f 7229 0a72 0800 0000 da02  meError).r......
-00000450: 7466 7213 0000 00da 0763 6d64 6c69 6e65  tfr......cmdline
-00000460: da01 70da 036f 7574 da03 6572 72da 0365  ..p..out..err..e
-00000470: 7863 da01 665a 0a73 7667 5f73 7472 696e  xc..fZ.svg_strin
-00000480: 67a9 0072 2400 0000 fa55 2f6f 7074 2f68  g..r$....U/opt/h
-00000490: 6f73 7465 6474 6f6f 6c63 6163 6865 2f50  ostedtoolcache/P
-000004a0: 7974 686f 6e2f 332e 382e 372f 7836 342f  ython/3.8.7/x64/
-000004b0: 6c69 622f 7079 7468 6f6e 332e 382f 7369  lib/python3.8/si
-000004c0: 7465 2d70 6163 6b61 6765 732f 766f 6c74  te-packages/volt
-000004d0: 6169 7265 2f6d 6572 6d61 6964 2e70 79da  aire/mermaid.py.
-000004e0: 0e67 656e 6572 6174 655f 696d 6167 6511  .generate_image.
-000004f0: 0000 0073 3400 0000 0006 0c01 1001 0802  ...s4...........
-00000500: 0a02 0201 0201 0401 0201 0201 0201 02f9  ................
-00000510: 040a 0201 0e01 1001 1001 1e02 0a01 0c01  ................
-00000520: 0a01 1201 0a01 0402 0201 16ff 7226 0000  ............r&..
-00000530: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000540: 0000 0300 0000 4000 0000 7322 0000 0065  ......@...s"...e
-00000550: 005a 0164 005a 0265 0367 0165 0465 0319  .Z.d.Z.e.g.e.e..
-00000560: 0064 019c 0264 0264 0384 045a 0564 0453  .d...d.d...Z.d.S
-00000570: 0029 05da 104d 6572 6d61 6964 5072 6f63  .)...MermaidProc
-00000580: 6573 736f 7229 02da 056c 696e 6573 7209  essor)...linesr.
-00000590: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000005a0: 0500 0000 0400 0000 6300 0000 7362 0000  ........c...sb..
-000005b0: 0064 017d 0264 027d 037c 0144 005d 507d  .d.}.d.}.|.D.]P}
-000005c0: 047c 0272 2e74 00a0 017c 04a1 0172 2664  .|.r.t...|...r&d
-000005d0: 037d 0271 0c71 5c7c 0456 0001 0071 0c74  .}.q.q\|.V...q.t
-000005e0: 02a0 017c 04a1 0172 4e74 037c 0383 0156  ...|...rNt.|...V
-000005f0: 0001 0064 027d 0364 017d 0271 0c71 0c7c  ...d.}.d.}.q.q.|
-00000600: 037c 0464 0417 0037 007d 0371 0c71 0c64  .|.d...7.}.q.q.d
-00000610: 0053 0029 054e 54da 0046 da01 0a29 04da  .S.).NT..F...)..
-00000620: 0d4d 4552 4d41 4944 5f53 5441 5254 da05  .MERMAID_START..
-00000630: 6d61 7463 68da 0b4d 4552 4d41 4944 5f45  match..MERMAID_E
-00000640: 4e44 7226 0000 0029 05da 0473 656c 6672  NDr&...)...selfr
-00000650: 2800 0000 5a14 6c6f 6f6b 696e 675f 666f  (...Z.looking_fo
-00000660: 725f 6d65 726d 6169 6473 7208 0000 00da  r_mermaidsr.....
-00000670: 046c 696e 6572 2400 0000 7224 0000 0072  .liner$...r$...r
-00000680: 2500 0000 da03 7275 6e39 0000 0073 1e00  %.....run9...s..
-00000690: 0000 0001 0401 0402 0804 0401 0a03 0401  ................
-000006a0: 0404 0802 0a03 0a03 0401 0401 0405 0c01  ................
-000006b0: 7a14 4d65 726d 6169 6450 726f 6365 7373  z.MermaidProcess
-000006c0: 6f72 2e72 756e 4e29 06da 085f 5f6e 616d  or.runN)...__nam
-000006d0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000006e0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0500  .__qualname__r..
-000006f0: 0000 7204 0000 0072 3000 0000 7224 0000  ..r....r0...r$..
-00000700: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00000710: 7227 0000 0038 0000 0073 0200 0000 0801  r'...8...s......
-00000720: 7227 0000 0063 0000 0000 0000 0000 0000  r'...c..........
-00000730: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
-00000740: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00000750: 005a 0364 0353 0029 04da 104d 6572 6d61  .Z.d.S.)...Merma
-00000760: 6964 4578 7465 6e73 696f 6e63 0200 0000  idExtensionc....
-00000770: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000780: 4300 0000 7320 0000 007c 016a 00a0 0174  C...s ...|.j...t
-00000790: 0283 0064 0164 02a1 0301 007c 01a0 037c  ...d.d.....|...|
-000007a0: 00a1 0101 0064 0053 0029 034e 5a07 6d65  .....d.S.).NZ.me
-000007b0: 726d 6169 64e9 2300 0000 2904 5a0d 7072  rmaid.#...).Z.pr
-000007c0: 6570 726f 6365 7373 6f72 73da 0872 6567  eprocessors..reg
-000007d0: 6973 7465 7272 2700 0000 5a11 7265 6769  isterr'...Z.regi
-000007e0: 7374 6572 4578 7465 6e73 696f 6e29 0272  sterExtension).r
-000007f0: 2e00 0000 5a02 6d64 7224 0000 0072 2400  ....Z.mdr$...r$.
-00000800: 0000 7225 0000 00da 0e65 7874 656e 644d  ..r%.....extendM
-00000810: 6172 6b64 6f77 6e5e 0000 0073 0400 0000  arkdown^...s....
-00000820: 0001 1201 7a1f 4d65 726d 6169 6445 7874  ....z.MermaidExt
-00000830: 656e 7369 6f6e 2e65 7874 656e 644d 6172  ension.extendMar
-00000840: 6b64 6f77 6e4e 2904 7231 0000 0072 3200  kdownN).r1...r2.
-00000850: 0000 7233 0000 0072 3700 0000 7224 0000  ..r3...r7...r$..
-00000860: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00000870: 7234 0000 005d 0000 0073 0200 0000 0801  r4...]...s......
-00000880: 7234 0000 0063 0000 0000 0000 0000 0000  r4...c..........
-00000890: 0000 0100 0000 0300 0000 4b00 0000 7314  ..........K...s.
-000008a0: 0000 0074 00a0 0164 01a1 0101 0074 0266  ...t...d.....t.f
-000008b0: 007c 008e 0153 0029 024e 7a34 7768 6963  .|...S.).Nz4whic
-000008c0: 6820 6d6d 6463 207c 7c20 6e70 6d20 696e  h mmdc || npm in
-000008d0: 7374 616c 6c20 2d67 2040 6d65 726d 6169  stall -g @mermai
-000008e0: 642d 6a73 2f6d 6572 6d61 6964 2d63 6c69  d-js/mermaid-cli
-000008f0: 2903 7218 0000 00da 0673 7973 7465 6d72  ).r......systemr
-00000900: 3400 0000 2901 da06 6b77 6172 6773 7224  4...)...kwargsr$
-00000910: 0000 0072 2400 0000 7225 0000 00da 0d6d  ...r$...r%.....m
-00000920: 616b 6545 7874 656e 7369 6f6e 6300 0000  akeExtensionc...
-00000930: 7304 0000 0000 010a 0172 3a00 0000 291a  s........r:...).
-00000940: 7218 0000 00da 0272 6572 0e00 0000 da0a  r......rer......
-00000950: 7375 6270 726f 6365 7373 7202 0000 0072  subprocessr....r
-00000960: 0300 0000 da06 7479 7069 6e67 7204 0000  ......typingr...
-00000970: 0072 0500 0000 5a13 6d61 726b 646f 776e  .r....Z.markdown
-00000980: 2e65 7874 656e 7369 6f6e 7372 0600 0000  .extensionsr....
-00000990: 5a16 6d61 726b 646f 776e 2e70 7265 7072  Z.markdown.prepr
-000009a0: 6f63 6573 736f 7273 7207 0000 00da 0763  ocessorsr......c
-000009b0: 6f6d 7069 6c65 722b 0000 0072 2d00 0000  ompiler+...r-...
-000009c0: da04 7061 7468 da04 6a6f 696e da07 6469  ..path..join..di
-000009d0: 726e 616d 65da 0872 6561 6c70 6174 68da  rname..realpath.
-000009e0: 085f 5f66 696c 655f 5f72 1400 0000 7226  .__file__r....r&
-000009f0: 0000 0072 2700 0000 7234 0000 0072 3a00  ...r'...r4...r:.
-00000a00: 0000 7224 0000 0072 2400 0000 7224 0000  ..r$...r$...r$..
-00000a10: 0072 2500 0000 da08 3c6d 6f64 756c 653e  .r%.....<module>
-00000a20: 0100 0000 7320 0000 0008 0108 0108 0110  ....s ..........
-00000a30: 0110 020c 010c 020a 010a 0106 0112 0002  ................
-00000a40: ff04 0510 2710 2510 06                   ....'.%..
+00000060: 6d08 5a08 6d09 5a09 0100 6400 6404 6c0a  m.Z.m.Z...d.d.l.
+00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6501 a00e 6406 a101 5a0f 6501 a00e  ..e...d...Z.e...
+00000090: 6407 a101 5a10 6500 6a11 a012 6500 6a11  d...Z.e.j...e.j.
+000000a0: a013 6500 6a11 a014 6515 a101 a101 6408  ..e.j...e.....d.
+000000b0: a102 5a16 6509 6509 6409 9c02 640a 640b  ..Z.e.e.d...d.d.
+000000c0: 8404 5a17 4700 640c 640d 8400 640d 650d  ..Z.G.d.d...d.e.
+000000d0: 8303 5a18 4700 640e 640f 8400 640f 650b  ..Z.G.d.d...d.e.
+000000e0: 8303 5a19 6410 6411 8400 5a1a 6401 5300  ..Z.d.d...Z.d.S.
+000000f0: 2912 e900 0000 004e 2902 da04 5049 5045  )......N)...PIPE
+00000100: da05 506f 7065 6e29 03da 0849 7465 7261  ..Popen)...Itera
+00000110: 626c 65da 044c 6973 74da 0454 6578 7429  ble..List..Text)
+00000120: 01da 0945 7874 656e 7369 6f6e 2901 da0c  ...Extension)...
+00000130: 5072 6570 726f 6365 7373 6f72 7a1d 5e60  Preprocessorz.^`
+00000140: 6060 5b5c 205c 745d 2a5b 4d6d 5d65 726d  ``[\ \t]*[Mm]erm
+00000150: 6169 645b 5c20 5c74 5d2a 247a 0c5e 6060  aid[\ \t]*$z.^``
+00000160: 605b 5c20 5c74 5d2a 247a 0c6d 6572 6d61  `[\ \t]*$z.merma
+00000170: 6964 2e6a 736f 6e29 02da 0c6d 6572 6d61  id.json)...merma
+00000180: 6964 5f63 6f64 65da 0672 6574 7572 6e63  id_code..returnc
+00000190: 0100 0000 0000 0000 0000 0000 0a00 0000  ................
+000001a0: 0a00 0000 4300 0000 73f4 0000 0074 006a  ....C...s....t.j
+000001b0: 0164 0164 028d 017d 017c 01a0 027c 00a0  .d.d...}.|...|..
+000001c0: 0364 03a1 01a1 0101 007c 01a0 04a1 0001  .d.......|......
+000001d0: 007c 016a 0564 0417 007d 0264 0564 067c  .|.j.d...}.d.d.|
+000001e0: 016a 0564 077c 0264 0874 0667 077d 037a  .j.d.|.d.t.g.}.z
+000001f0: 1e74 077c 0374 0874 0864 098d 037d 047c  .t.|.t.t.d...}.|
+00000200: 04a0 09a1 005c 027d 057d 0657 006e 2e04  .....\.}.}.W.n..
+00000210: 0074 0a6b 0a72 8e01 007d 0701 007a 1074  .t.k.r...}...z.t
+00000220: 0a64 0a7c 0716 0083 0182 0157 0035 0064  .d.|.......W.5.d
+00000230: 0b7d 077e 0758 0059 006e 6258 007c 046a  .}.~.X.Y.nbX.|.j
+00000240: 0b64 0c6b 0272 d074 0ca0 0d7c 016a 05a1  .d.k.r.t...|.j..
+00000250: 0101 0074 0e7c 0283 018f 0e7d 087c 08a0  ...t.|.....}.|..
+00000260: 0fa1 007d 0957 0035 0051 0052 0058 0074  ...}.W.5.Q.R.X.t
+00000270: 0ca0 0d7c 02a1 0101 007c 0953 0074 1064  ...|.....|.S.t.d
+00000280: 0d74 117c 0683 019b 0064 0e7c 016a 059b  .t.|.....d.|.j..
+00000290: 0064 0f7c 029b 009d 0683 0182 0164 0b53  .d.|.........d.S
+000002a0: 0029 107a 8a0a 2020 2020 436f 6e76 6572  .).z..    Conver
+000002b0: 7473 204d 6572 6d61 6964 2073 6f75 7263  ts Mermaid sourc
+000002c0: 6520 636f 6465 2074 6f20 5356 472e 0a20  e code to SVG.. 
+000002d0: 2020 203a 7061 7261 6d20 6d65 726d 6169     :param mermai
+000002e0: 645f 636f 6465 3a20 4d65 726d 6169 6420  d_code: Mermaid 
+000002f0: 696e 7075 7420 636f 6465 2061 7320 6120  input code as a 
+00000300: 7374 7269 6e67 2e0a 2020 2020 3a72 6574  string..    :ret
+00000310: 7572 6e3a 2053 5647 2063 6f64 6520 6173  urn: SVG code as
+00000320: 2061 2073 7472 696e 672e 0a20 2020 2046   a string..    F
+00000330: 2901 da06 6465 6c65 7465 da04 7574 6638  )...delete..utf8
+00000340: 7a04 2e73 7667 5a04 6d6d 6463 7a02 2d69  z..svgZ.mmdcz.-i
+00000350: 7a02 2d6f 7a02 2d63 2902 da06 7374 646f  z.-oz.-c)...stdo
+00000360: 7574 da06 7374 6465 7272 7a19 4661 696c  ut..stderrz.Fail
+00000370: 6564 2074 6f20 7275 6e20 6d65 726d 6169  ed to run mermai
+00000380: 643a 2025 734e 7201 0000 007a 1745 7272  d: %sNr....z.Err
+00000390: 6f72 2063 616c 6c69 6e67 206d 6572 6d61  or calling merma
+000003a0: 6964 3a20 7a0d 0a54 656d 7020 6669 6c65  id: z..Temp file
+000003b0: 733a 207a 0520 616e 6420 2912 da08 7465  s: z. and )...te
+000003c0: 6d70 6669 6c65 da12 4e61 6d65 6454 656d  mpfile..NamedTem
+000003d0: 706f 7261 7279 4669 6c65 da05 7772 6974  poraryFile..writ
+000003e0: 65da 0665 6e63 6f64 65da 0566 6c75 7368  e..encode..flush
+000003f0: da04 6e61 6d65 da09 434f 4e46 5f46 494c  ..name..CONF_FIL
+00000400: 4572 0300 0000 7202 0000 00da 0b63 6f6d  Er....r......com
+00000410: 6d75 6e69 6361 7465 da09 4578 6365 7074  municate..Except
+00000420: 696f 6eda 0a72 6574 7572 6e63 6f64 65da  ion..returncode.
+00000430: 026f 73da 0672 656d 6f76 65da 046f 7065  .os..remove..ope
+00000440: 6eda 0472 6561 64da 0c52 756e 7469 6d65  n..read..Runtime
+00000450: 4572 726f 72da 0373 7472 290a 7209 0000  Error..str).r...
+00000460: 00da 0274 6672 1400 0000 da07 636d 646c  ...tfr......cmdl
+00000470: 696e 65da 0170 da03 6f75 74da 0365 7272  ine..p..out..err
+00000480: da03 6578 63da 0166 5a0a 7376 675f 7374  ..exc..fZ.svg_st
+00000490: 7269 6e67 a900 7226 0000 00fa 552f 6f70  ring..r&....U/op
+000004a0: 742f 686f 7374 6564 746f 6f6c 6361 6368  t/hostedtoolcach
+000004b0: 652f 5079 7468 6f6e 2f33 2e38 2e37 2f78  e/Python/3.8.7/x
+000004c0: 3634 2f6c 6962 2f70 7974 686f 6e33 2e38  64/lib/python3.8
+000004d0: 2f73 6974 652d 7061 636b 6167 6573 2f76  /site-packages/v
+000004e0: 6f6c 7461 6972 652f 6d65 726d 6169 642e  oltaire/mermaid.
+000004f0: 7079 da0e 6765 6e65 7261 7465 5f69 6d61  py..generate_ima
+00000500: 6765 1100 0000 7334 0000 0000 060c 0110  ge....s4........
+00000510: 0108 020a 0202 0102 0104 0102 0102 0102  ................
+00000520: 0102 f904 0a02 010e 0110 0110 011e 020a  ................
+00000530: 010c 010a 0112 010a 0104 0202 011a ff72  ...............r
+00000540: 2800 0000 6300 0000 0000 0000 0000 0000  (...c...........
+00000550: 0000 0000 0003 0000 0040 0000 0073 2400  .........@...s$.
+00000560: 0000 6500 5a01 6400 5a02 6503 6504 1900  ..e.Z.d.Z.e.e...
+00000570: 6505 6504 1900 6401 9c02 6402 6403 8404  e.e...d...d.d...
+00000580: 5a06 6404 5300 2905 da10 4d65 726d 6169  Z.d.S.)...Mermai
+00000590: 6450 726f 6365 7373 6f72 2902 da05 6c69  dProcessor)...li
+000005a0: 6e65 7372 0a00 0000 6302 0000 0000 0000  nesr....c.......
+000005b0: 0000 0000 0005 0000 0004 0000 0063 0000  .............c..
+000005c0: 0073 6200 0000 6401 7d02 6402 7d03 7c01  .sb...d.}.d.}.|.
+000005d0: 4400 5d50 7d04 7c02 722e 7400 a001 7c04  D.]P}.|.r.t...|.
+000005e0: a101 7226 6403 7d02 710c 715c 7c04 5600  ..r&d.}.q.q\|.V.
+000005f0: 0100 710c 7402 a001 7c04 a101 724e 7403  ..q.t...|...rNt.
+00000600: 7c03 8301 5600 0100 6402 7d03 6401 7d02  |...V...d.}.d.}.
+00000610: 710c 710c 7c03 7c04 6404 1700 3700 7d03  q.q.|.|.d...7.}.
+00000620: 710c 710c 6400 5300 2905 4e54 da00 46da  q.q.d.S.).NT..F.
+00000630: 010a 2904 da0d 4d45 524d 4149 445f 5354  ..)...MERMAID_ST
+00000640: 4152 54da 056d 6174 6368 da0b 4d45 524d  ART..match..MERM
+00000650: 4149 445f 454e 4472 2800 0000 2905 da04  AID_ENDr(...)...
+00000660: 7365 6c66 722a 0000 005a 146c 6f6f 6b69  selfr*...Z.looki
+00000670: 6e67 5f66 6f72 5f6d 6572 6d61 6964 7372  ng_for_mermaidsr
+00000680: 0900 0000 da04 6c69 6e65 7226 0000 0072  ......liner&...r
+00000690: 2600 0000 7227 0000 00da 0372 756e 3900  &...r'.....run9.
+000006a0: 0000 731e 0000 0000 0104 0104 0208 0404  ..s.............
+000006b0: 010a 0304 0104 0408 020a 030a 0304 0104  ................
+000006c0: 0104 050c 017a 144d 6572 6d61 6964 5072  .....z.MermaidPr
+000006d0: 6f63 6573 736f 722e 7275 6e4e 2907 da08  ocessor.runN)...
+000006e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000006f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000700: 5f5f 7205 0000 0072 0600 0000 7204 0000  __r....r....r...
+00000710: 0072 3200 0000 7226 0000 0072 2600 0000  .r2...r&...r&...
+00000720: 7226 0000 0072 2700 0000 7229 0000 0038  r&...r'...r)...8
+00000730: 0000 0073 0200 0000 0801 7229 0000 0063  ...s......r)...c
+00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000750: 0200 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
+00000760: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
+00000770: 0029 04da 104d 6572 6d61 6964 4578 7465  .)...MermaidExte
+00000780: 6e73 696f 6e63 0200 0000 0000 0000 0000  nsionc..........
+00000790: 0000 0200 0000 0500 0000 4300 0000 7320  ..........C...s 
+000007a0: 0000 007c 016a 00a0 0174 0283 0064 0164  ...|.j...t...d.d
+000007b0: 02a1 0301 007c 01a0 037c 00a1 0101 0064  .....|...|.....d
+000007c0: 0053 0029 034e 5a07 6d65 726d 6169 64e9  .S.).NZ.mermaid.
+000007d0: 2300 0000 2904 5a0d 7072 6570 726f 6365  #...).Z.preproce
+000007e0: 7373 6f72 73da 0872 6567 6973 7465 7272  ssors..registerr
+000007f0: 2900 0000 5a11 7265 6769 7374 6572 4578  )...Z.registerEx
+00000800: 7465 6e73 696f 6e29 0272 3000 0000 5a02  tension).r0...Z.
+00000810: 6d64 7226 0000 0072 2600 0000 7227 0000  mdr&...r&...r'..
+00000820: 00da 0e65 7874 656e 644d 6172 6b64 6f77  ...extendMarkdow
+00000830: 6e5e 0000 0073 0400 0000 0001 1201 7a1f  n^...s........z.
+00000840: 4d65 726d 6169 6445 7874 656e 7369 6f6e  MermaidExtension
+00000850: 2e65 7874 656e 644d 6172 6b64 6f77 6e4e  .extendMarkdownN
+00000860: 2904 7233 0000 0072 3400 0000 7235 0000  ).r3...r4...r5..
+00000870: 0072 3900 0000 7226 0000 0072 2600 0000  .r9...r&...r&...
+00000880: 7226 0000 0072 2700 0000 7236 0000 005d  r&...r'...r6...]
+00000890: 0000 0073 0200 0000 0801 7236 0000 0063  ...s......r6...c
+000008a0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+000008b0: 0300 0000 4b00 0000 7314 0000 0074 00a0  ....K...s....t..
+000008c0: 0164 01a1 0101 0074 0266 007c 008e 0153  .d.....t.f.|...S
+000008d0: 0029 024e 7a40 7768 6963 6820 6d6d 6463  .).Nz@which mmdc
+000008e0: 2032 3e2f 6465 762f 6e75 6c6c 207c 7c20   2>/dev/null || 
+000008f0: 6e70 6d20 696e 7374 616c 6c20 2d67 2040  npm install -g @
+00000900: 6d65 726d 6169 642d 6a73 2f6d 6572 6d61  mermaid-js/merma
+00000910: 6964 2d63 6c69 2903 7219 0000 00da 0673  id-cli).r......s
+00000920: 7973 7465 6d72 3600 0000 2901 da06 6b77  ystemr6...)...kw
+00000930: 6172 6773 7226 0000 0072 2600 0000 7227  argsr&...r&...r'
+00000940: 0000 00da 0d6d 616b 6545 7874 656e 7369  .....makeExtensi
+00000950: 6f6e 6300 0000 7308 0000 0000 0104 0102  onc...s.........
+00000960: ff04 0372 3c00 0000 291b 7219 0000 00da  ...r<...).r.....
+00000970: 0272 6572 0f00 0000 da0a 7375 6270 726f  .rer......subpro
+00000980: 6365 7373 7202 0000 0072 0300 0000 da06  cessr....r......
+00000990: 7479 7069 6e67 7204 0000 0072 0500 0000  typingr....r....
+000009a0: 7206 0000 005a 136d 6172 6b64 6f77 6e2e  r....Z.markdown.
+000009b0: 6578 7465 6e73 696f 6e73 7207 0000 005a  extensionsr....Z
+000009c0: 166d 6172 6b64 6f77 6e2e 7072 6570 726f  .markdown.prepro
+000009d0: 6365 7373 6f72 7372 0800 0000 da07 636f  cessorsr......co
+000009e0: 6d70 696c 6572 2d00 0000 722f 0000 00da  mpiler-...r/....
+000009f0: 0470 6174 68da 046a 6f69 6eda 0764 6972  .path..join..dir
+00000a00: 6e61 6d65 da08 7265 616c 7061 7468 da08  name..realpath..
+00000a10: 5f5f 6669 6c65 5f5f 7215 0000 0072 2800  __file__r....r(.
+00000a20: 0000 7229 0000 0072 3600 0000 723c 0000  ..r)...r6...r<..
+00000a30: 0072 2600 0000 7226 0000 0072 2600 0000  .r&...r&...r&...
+00000a40: 7227 0000 00da 083c 6d6f 6475 6c65 3e01  r'.....<module>.
+00000a50: 0000 0073 2000 0000 0801 0801 0801 1001  ...s ...........
+00000a60: 1402 0c01 0c02 0a01 0a01 0601 1200 02ff  ................
+00000a70: 0405 1027 1025 1006                      ...'.%..
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/pelican.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 872 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,62 +1,73 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 6803 0000  U..........`h...
+00000000: 550d 0d0a 0000 0000 90eb 1c60 0d04 0000  U..........`....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6402 5a01 6403 6701 5a02  d.l.Z.d.Z.d.g.Z.
-00000040: 6404 6701 5a03 6700 5a04 6405 5a05 6406  d.g.Z.g.Z.d.Z.d.
-00000050: 5a06 6407 5a07 6408 5a08 6401 5a09 6401  Z.d.Z.d.Z.d.Z.d.
-00000060: 5a0a 6401 5a0b 6401 5a0c 6401 5a0d 6409  Z.d.Z.d.Z.d.Z.d.
-00000070: 640a 6702 5a0e 6500 6a0f a010 6500 6a0f  d.g.Z.e.j...e.j.
-00000080: a011 6500 6a0f a012 6513 a101 a101 640b  ..e.j...e.....d.
-00000090: a102 5a14 6500 6a0f a010 6514 640c a102  ..Z.e.j...e.d...
-000000a0: 6500 6a0f a010 6500 a015 a100 640c a102  e.j...e.....d...
-000000b0: 6702 5a16 6500 6a0f a010 6500 a015 a100  g.Z.e.j...e.....
-000000c0: 640c 640d 640e a104 5a17 6500 6a0f a018  d.d.d...Z.e.j...
-000000d0: 6517 a101 73ac 640f 5a17 6900 6900 6410  e...s.d.Z.i.i.d.
-000000e0: 9c02 6411 6412 9c02 5a19 6413 5a1a 6401  ..d.d...Z.d.Z.d.
-000000f0: 5300 2914 e900 0000 004e da07 636f 6e74  S.)......N..cont
-00000100: 656e 74da 012e 5a05 706f 7374 73da 0862  ent...Z.posts..b
-00000110: 6173 656e 616d 657a 077b 736c 7567 7d2f  asenamez.{slug}/
-00000120: 7a11 7b73 6c75 677d 2f69 6e64 6578 2e68  z.{slug}/index.h
-00000130: 746d 6c7a 0d45 7572 6f70 652f 4c6f 6e64  tmlz.Europe/Lond
-00000140: 6f6e 5a11 7065 6c69 6361 6e5f 7765 6261  onZ.pelican_weba
-00000150: 7373 6574 737a 1276 6f6c 7461 6972 652e  ssetsz.voltaire.
-00000160: 7769 6b69 6c69 6e6b 735a 0574 6865 6d65  wikilinksZ.theme
-00000170: da06 7374 6174 6963 da03 6373 737a 0a73  ..static..cssz.s
-00000180: 7479 6c65 2e73 6373 7346 2902 7a10 766f  tyle.scssF).z.vo
-00000190: 6c74 6169 7265 2e6d 6572 6d61 6964 7a19  ltaire.mermaidz.
-000001a0: 6d61 726b 646f 776e 2e65 7874 656e 7369  markdown.extensi
-000001b0: 6f6e 732e 6578 7472 61da 0568 746d 6c35  ons.extra..html5
-000001c0: 2902 5a11 6578 7465 6e73 696f 6e5f 636f  ).Z.extension_co
-000001d0: 6e66 6967 735a 0d6f 7574 7075 745f 666f  nfigsZ.output_fo
-000001e0: 726d 6174 5429 1bda 026f 73da 0450 4154  rmatT)...os..PAT
-000001f0: 485a 0a50 4147 455f 5041 5448 535a 0d41  HZ.PAGE_PATHSZ.A
-00000200: 5254 4943 4c45 5f50 4154 4853 5a0c 5354  RTICLE_PATHSZ.ST
-00000210: 4154 4943 5f50 4154 4853 5a0e 534c 5547  ATIC_PATHSZ.SLUG
-00000220: 4946 595f 534f 5552 4345 5a08 5041 4745  IFY_SOURCEZ.PAGE
-00000230: 5f55 524c 5a0c 5041 4745 5f53 4156 455f  _URLZ.PAGE_SAVE_
-00000240: 4153 5a08 5449 4d45 5a4f 4e45 5a0d 4645  ASZ.TIMEZONEZ.FE
-00000250: 4544 5f41 4c4c 5f41 544f 4d5a 1243 4154  ED_ALL_ATOMZ.CAT
-00000260: 4547 4f52 595f 4645 4544 5f41 544f 4d5a  EGORY_FEED_ATOMZ
-00000270: 1041 5554 484f 525f 4645 4544 5f41 544f  .AUTHOR_FEED_ATO
-00000280: 4d5a 0f41 5554 484f 525f 4645 4544 5f52  MZ.AUTHOR_FEED_R
-00000290: 5353 5a15 5452 414e 534c 4154 494f 4e5f  SSZ.TRANSLATION_
-000002a0: 4645 4544 5f41 544f 4d5a 0750 4c55 4749  FEED_ATOMZ.PLUGI
-000002b0: 4e53 da04 7061 7468 da04 6a6f 696e da07  NS..path..join..
-000002c0: 6469 726e 616d 65da 0872 6561 6c70 6174  dirname..realpat
-000002d0: 68da 085f 5f66 696c 655f 5f5a 0554 4845  h..__file__Z.THE
-000002e0: 4d45 da06 6765 7463 7764 5a12 5448 454d  ME..getcwdZ.THEM
-000002f0: 455f 5354 4154 4943 5f50 4154 4853 5a0a  E_STATIC_PATHSZ.
-00000300: 4c4f 4341 4c5f 5343 5353 da06 6578 6973  LOCAL_SCSS..exis
-00000310: 7473 5a08 4d41 524b 444f 574e 5a09 5459  tsZ.MARKDOWNZ.TY
-00000320: 504f 4752 4946 59a9 0072 1100 0000 7211  POGRIFY..r....r.
-00000330: 0000 00fa 552f 6f70 742f 686f 7374 6564  ....U/opt/hosted
-00000340: 746f 6f6c 6361 6368 652f 5079 7468 6f6e  toolcache/Python
-00000350: 2f33 2e38 2e37 2f78 3634 2f6c 6962 2f70  /3.8.7/x64/lib/p
-00000360: 7974 686f 6e33 2e38 2f73 6974 652d 7061  ython3.8/site-pa
-00000370: 636b 6167 6573 2f76 6f6c 7461 6972 652f  ckages/voltaire/
-00000380: 7065 6c69 6361 6e2e 7079 da08 3c6d 6f64  pelican.py..<mod
-00000390: 756c 653e 0100 0000 733a 0000 0008 0204  ule>....s:......
-000003a0: 0106 0106 0104 0204 0204 0104 0204 0204  ................
-000003b0: 0104 0104 0104 0104 0302 0102 fe04 051e  ................
-000003c0: 020c 0110 fe04 0516 010c 0104 0402 0102  ................
-000003d0: fe04 0402 fb06 08                        .......
+00000020: 0007 0000 0040 0000 0073 0401 0000 5500  .....@...s....U.
+00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
+00000040: 5a02 0100 6400 6403 6c03 6d04 5a04 6d05  Z...d.d.l.m.Z.m.
+00000050: 5a05 0100 6404 5a06 6405 6701 5a07 6406  Z...d.Z.d.g.Z.d.
+00000060: 6701 5a08 6700 5a09 6504 650a 1900 650b  g.Z.g.Z.e.e...e.
+00000070: 6407 3c00 6408 5a0c 6409 5a0d 640a 5a0e  d.<.d.Z.d.Z.d.Z.
+00000080: 640b 5a0f 6401 5a10 6401 5a11 6401 5a12  d.Z.d.Z.d.Z.d.Z.
+00000090: 6401 5a13 6401 5a14 640c 640d 6702 5a15  d.Z.d.Z.d.d.g.Z.
+000000a0: 6500 6a16 a017 6500 6a16 a018 6500 6a16  e.j...e.j...e.j.
+000000b0: a019 651a a101 a101 640e a102 5a1b 6500  ..e.....d...Z.e.
+000000c0: 6a16 a017 651b 640f a102 6500 6a16 a017  j...e.d...e.j...
+000000d0: 6500 a01c a100 640f a102 6702 5a1d 6401  e.....d...g.Z.d.
+000000e0: 5a1e 6505 650a 1900 650b 6410 3c00 6502  Z.e.e...e.d.<.e.
+000000f0: a01f a100 640f 1b00 6411 1b00 6412 1b00  ....d...d...d...
+00000100: 5a16 6502 650b 6413 3c00 6516 a020 a100  Z.e.e.d.<.e.. ..
+00000110: 72ec 650a 6516 8301 5a1e 6900 6900 6414  r.e.e...Z.i.i.d.
+00000120: 9c02 6415 6416 9c02 5a21 6417 5a22 6401  ..d.d...Z!d.Z"d.
+00000130: 5300 2918 e900 0000 004e 2901 da04 5061  S.)......N)...Pa
+00000140: 7468 2902 da04 4c69 7374 da08 4f70 7469  th)...List..Opti
+00000150: 6f6e 616c da07 636f 6e74 656e 74da 012e  onal..content...
+00000160: 5a05 706f 7374 73da 0c53 5441 5449 435f  Z.posts..STATIC_
+00000170: 5041 5448 53da 0862 6173 656e 616d 657a  PATHS..basenamez
+00000180: 077b 736c 7567 7d2f 7a11 7b73 6c75 677d  .{slug}/z.{slug}
+00000190: 2f69 6e64 6578 2e68 746d 6c7a 0d45 7572  /index.htmlz.Eur
+000001a0: 6f70 652f 4c6f 6e64 6f6e 5a11 7065 6c69  ope/LondonZ.peli
+000001b0: 6361 6e5f 7765 6261 7373 6574 737a 1276  can_webassetsz.v
+000001c0: 6f6c 7461 6972 652e 7769 6b69 6c69 6e6b  oltaire.wikilink
+000001d0: 735a 0574 6865 6d65 da06 7374 6174 6963  sZ.theme..static
+000001e0: da0a 4c4f 4341 4c5f 5343 5353 da03 6373  ..LOCAL_SCSS..cs
+000001f0: 737a 0a73 7479 6c65 2e73 6373 73da 0470  sz.style.scss..p
+00000200: 6174 6829 027a 1076 6f6c 7461 6972 652e  ath).z.voltaire.
+00000210: 6d65 726d 6169 647a 196d 6172 6b64 6f77  mermaidz.markdow
+00000220: 6e2e 6578 7465 6e73 696f 6e73 2e65 7874  n.extensions.ext
+00000230: 7261 da05 6874 6d6c 3529 025a 1165 7874  ra..html5).Z.ext
+00000240: 656e 7369 6f6e 5f63 6f6e 6669 6773 5a0d  ension_configsZ.
+00000250: 6f75 7470 7574 5f66 6f72 6d61 7454 2923  output_formatT)#
+00000260: da02 6f73 da07 7061 7468 6c69 6272 0200  ..os..pathlibr..
+00000270: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+00000280: 0400 0000 da04 5041 5448 5a0a 5041 4745  ......PATHZ.PAGE
+00000290: 5f50 4154 4853 5a0d 4152 5449 434c 455f  _PATHSZ.ARTICLE_
+000002a0: 5041 5448 5372 0700 0000 da03 7374 72da  PATHSr......str.
+000002b0: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+000002c0: 5a0e 534c 5547 4946 595f 534f 5552 4345  Z.SLUGIFY_SOURCE
+000002d0: 5a08 5041 4745 5f55 524c 5a0c 5041 4745  Z.PAGE_URLZ.PAGE
+000002e0: 5f53 4156 455f 4153 5a08 5449 4d45 5a4f  _SAVE_ASZ.TIMEZO
+000002f0: 4e45 5a0d 4645 4544 5f41 4c4c 5f41 544f  NEZ.FEED_ALL_ATO
+00000300: 4d5a 1243 4154 4547 4f52 595f 4645 4544  MZ.CATEGORY_FEED
+00000310: 5f41 544f 4d5a 1041 5554 484f 525f 4645  _ATOMZ.AUTHOR_FE
+00000320: 4544 5f41 544f 4d5a 0f41 5554 484f 525f  ED_ATOMZ.AUTHOR_
+00000330: 4645 4544 5f52 5353 5a15 5452 414e 534c  FEED_RSSZ.TRANSL
+00000340: 4154 494f 4e5f 4645 4544 5f41 544f 4d5a  ATION_FEED_ATOMZ
+00000350: 0750 4c55 4749 4e53 720c 0000 00da 046a  .PLUGINSr......j
+00000360: 6f69 6eda 0764 6972 6e61 6d65 da08 7265  oin..dirname..re
+00000370: 616c 7061 7468 da08 5f5f 6669 6c65 5f5f  alpath..__file__
+00000380: 5a05 5448 454d 45da 0667 6574 6377 645a  Z.THEME..getcwdZ
+00000390: 1254 4845 4d45 5f53 5441 5449 435f 5041  .THEME_STATIC_PA
+000003a0: 5448 5372 0a00 0000 da03 6377 64da 0665  THSr......cwd..e
+000003b0: 7869 7374 735a 084d 4152 4b44 4f57 4e5a  xistsZ.MARKDOWNZ
+000003c0: 0954 5950 4f47 5249 4659 a900 721b 0000  .TYPOGRIFY..r...
+000003d0: 0072 1b00 0000 fa55 2f6f 7074 2f68 6f73  .r.....U/opt/hos
+000003e0: 7465 6474 6f6f 6c63 6163 6865 2f50 7974  tedtoolcache/Pyt
+000003f0: 686f 6e2f 332e 382e 372f 7836 342f 6c69  hon/3.8.7/x64/li
+00000400: 622f 7079 7468 6f6e 332e 382f 7369 7465  b/python3.8/site
+00000410: 2d70 6163 6b61 6765 732f 766f 6c74 6169  -packages/voltai
+00000420: 7265 2f70 656c 6963 616e 2e70 79da 083c  re/pelican.py..<
+00000430: 6d6f 6475 6c65 3e01 0000 0073 4200 0000  module>....sB...
+00000440: 0200 0801 0c01 1002 0401 0601 0601 1002  ................
+00000450: 0402 0401 0402 0402 0401 0401 0401 0401  ................
+00000460: 0403 0201 02fe 0405 1e02 0c01 10fe 0406  ................
+00000470: 1001 1c01 0801 0804 0201 02fe 0404 02fb  ................
+00000480: 0608                                     ..
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/search.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 38455 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 3796 0000  U..........`7...
+00000000: 550d 0d0a 0000 0000 90eb 1c60 3796 0000  U..........`7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 7a10 6401 6407 6c0c 6d0d 5a0d 0100  ..z.d.d.l.m.Z...
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/tasks.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 2237 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,153 +1,218 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 bd08 0000  U..........`....
+00000000: 550d 0d0a 0000 0000 90eb 1c60 540e 0000  U..........`T...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 0100 6406 5a0b 6900  m.Z.m.Z...d.Z.i.
-00000070: 5a0c 650c a00d 6509 a101 0100 650a 650b  Z.e...e.....e.e.
-00000080: 8301 5a0e 650c a00d 650e a101 0100 6407  ..Z.e...e.....d.
-00000090: 5a0f 6504 6408 6409 8400 8301 5a10 6504  Z.e.d.d.....Z.e.
-000000a0: 6410 640a 640b 8401 8301 5a11 6504 6411  d.d.d.....Z.e.d.
-000000b0: 640e 640f 8401 8301 5a12 6401 5300 2912  d.d.....Z.d.S.).
-000000c0: e900 0000 004e 2901 da06 6465 6465 6e74  .....N)...dedent
-000000d0: 2901 da04 7461 736b 2901 da04 6d61 696e  )...task)...main
-000000e0: 2902 da0e 4445 4641 554c 545f 434f 4e46  )...DEFAULT_CONF
-000000f0: 4947 da16 6765 745f 7365 7474 696e 6773  IG..get_settings
-00000100: 5f66 726f 6d5f 6669 6c65 7a0e 7065 6c69  _from_filez.peli
-00000110: 6361 6e63 6f6e 662e 7079 7a0e 7075 626c  canconf.pyz.publ
-00000120: 6973 6863 6f6e 662e 7079 6301 0000 0000  ishconf.pyc.....
-00000130: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000140: 0000 0073 1000 0000 7400 6401 7401 6702  ...s....t.d.t.g.
-00000150: 8301 0100 6402 5300 2903 fa1b 4275 696c  ....d.S.)...Buil
-00000160: 6420 6c6f 6361 6c20 7665 7273 696f 6e20  d local version 
-00000170: 6f66 2073 6974 65fa 022d 734e 2902 da0c  of site..-sN)...
-00000180: 7065 6c69 6361 6e5f 6d61 696e da12 5345  pelican_main..SE
-00000190: 5454 494e 4753 5f46 494c 455f 4241 5345  TTINGS_FILE_BASE
-000001a0: a901 da01 63a9 0072 0d00 0000 fa53 2f6f  ....c..r.....S/o
-000001b0: 7074 2f68 6f73 7465 6474 6f6f 6c63 6163  pt/hostedtoolcac
-000001c0: 6865 2f50 7974 686f 6e2f 332e 382e 372f  he/Python/3.8.7/
-000001d0: 7836 342f 6c69 622f 7079 7468 6f6e 332e  x64/lib/python3.
-000001e0: 382f 7369 7465 2d70 6163 6b61 6765 732f  8/site-packages/
-000001f0: 766f 6c74 6169 7265 2f74 6173 6b73 2e70  voltaire/tasks.p
-00000200: 79da 0562 7569 6c64 1300 0000 7302 0000  y..build....s...
-00000210: 0000 0372 0f00 0000 6302 0000 0000 0000  ...r....c.......
-00000220: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
-00000230: 0073 8a00 0000 7400 6401 7401 6402 6403  .s....t.d.t.d.d.
-00000240: 6704 8301 0100 6404 a002 7403 6a04 a005  g.....d...t.j...
-00000250: a100 a006 a100 a101 7d02 7c01 7274 7407  ........}.|.rtt.
-00000260: 6405 6406 8302 8f10 7d03 7c03 a008 7c01  d.d.....}.|...|.
-00000270: a101 0100 5700 3500 5100 5200 5800 7407  ....W.5.Q.R.X.t.
-00000280: 6407 6406 8302 8f1c 7d03 7c03 a008 7409  d.d.....}.|...t.
-00000290: 6408 7c01 9b00 6409 9d03 8301 a101 0100  d.|...d.........
-000002a0: 5700 3500 5100 5200 5800 7c00 a00a 640a  W.5.Q.R.X.|...d.
-000002b0: 7c02 9b00 640b 9d03 a101 0100 640c 5300  |...d.......d.S.
-000002c0: 290d 7207 0000 0072 0800 0000 7a08 2d2d  ).r....r....z.--
-000002d0: 6f75 7470 7574 da04 6469 7374 7a14 2750  output..distz.'P
-000002e0: 7562 6c69 7368 2073 6974 6520 6f6e 207b  ublish site on {
-000002f0: 7d27 7a0a 6469 7374 2f43 4e41 4d45 da01  }'z.dist/CNAME..
-00000300: 777a 0f64 6973 742f 726f 626f 7473 2e74  wz.dist/robots.t
-00000310: 7874 7a62 0a20 2020 2020 2020 2020 2020  xtzb.           
-00000320: 2020 2020 2055 7365 722d 6167 656e 743a       User-agent:
-00000330: 202a 0a20 2020 2020 2020 2020 2020 2020   *.             
-00000340: 2020 2044 6973 616c 6c6f 773a 202f 6472     Disallow: /dr
-00000350: 6166 7473 2f0a 2020 2020 2020 2020 2020  afts/.          
-00000360: 2020 2020 2020 5369 7465 6d61 703a 2068        Sitemap: h
-00000370: 7474 703a 2f2f 7a19 2f73 6974 656d 6170  ttp://z./sitemap
-00000380: 2e78 6d6c 0a20 2020 2020 2020 2020 2020  .xml.           
-00000390: 207a 1a67 6870 2d69 6d70 6f72 7420 2d62   z.ghp-import -b
-000003a0: 2067 682d 7061 6765 7320 2d6d 207a 0820   gh-pages -m z. 
-000003b0: 6469 7374 202d 704e 290b 7209 0000 00da  dist -pN).r.....
-000003c0: 1150 5542 4c49 5348 5f46 494c 455f 4241  .PUBLISH_FILE_BA
-000003d0: 5345 da06 666f 726d 6174 da08 6461 7465  SE..format..date
-000003e0: 7469 6d65 da04 6461 7465 da05 746f 6461  time..date..toda
-000003f0: 79da 0969 736f 666f 726d 6174 da04 6f70  y..isoformat..op
-00000400: 656e da05 7772 6974 6572 0200 0000 da03  en..writer......
-00000410: 7275 6e29 0472 0c00 0000 da06 646f 6d61  run).r......doma
-00000420: 696e 5a0e 636f 6d6d 6974 5f6d 6573 7361  inZ.commit_messa
-00000430: 6765 da01 6672 0d00 0000 720d 0000 0072  ge..fr....r....r
-00000440: 0e00 0000 da07 7075 626c 6973 6819 0000  ......publish...
-00000450: 0073 2000 0000 0003 1001 0401 0cff 0403  .s .............
-00000460: 0401 0c01 1401 0c01 0401 0201 0203 02fd  ................
-00000470: 06ff 02ff 0e09 721d 0000 00da 096c 6f63  ......r......loc
-00000480: 616c 686f 7374 e940 1f00 0063 0300 0000  alhost.@...c....
-00000490: 0000 0000 0000 0000 0b00 0000 0700 0000  ................
-000004a0: 0300 0000 73d0 0000 0064 0164 026c 006d  ....s....d.d.l.m
-000004b0: 017d 0301 0074 0288 0083 0101 007c 0383  .}...t.......|..
-000004c0: 007d 047c 04a0 0374 0487 0066 0164 0364  .}.|...t...f.d.d
-000004d0: 0484 08a1 0201 0064 0564 0667 027d 057c  .......d.d.g.}.|
-000004e0: 0544 005d 287d 0664 07a0 0574 0664 0819  .D.](}.d...t.d..
-000004f0: 007c 06a1 027d 077c 04a0 037c 0787 0066  .|...}.|...|...f
-00000500: 0164 0964 0484 08a1 0201 0071 3a74 0664  .d.d.......q:t.d
-00000510: 0a19 007d 087c 04a0 0364 0ba0 057c 08a1  ...}.|...d...|..
-00000520: 0187 0066 0164 0c64 0484 08a1 0201 0064  ...f.d.d.......d
-00000530: 0d64 0e67 027d 097c 0944 005d 247d 0664  .d.g.}.|.D.]$}.d
-00000540: 0fa0 057c 087c 06a1 027d 0a7c 04a0 037c  ...|.|...}.|...|
-00000550: 0a87 0066 0164 1064 0484 08a1 0201 0071  ...f.d.d.......q
-00000560: 927c 046a 077c 017c 0274 0664 1119 0064  .|.j.|.|.t.d...d
-00000570: 128d 0301 0064 1353 0029 147a 3841 7574  .....d.S.).z8Aut
-00000580: 6f6d 6174 6963 616c 6c79 2072 656c 6f61  omatically reloa
-00000590: 6420 6272 6f77 7365 7220 7461 6220 7570  d browser tab up
-000005a0: 6f6e 2066 696c 6520 6d6f 6469 6669 6361  on file modifica
-000005b0: 7469 6f6e 2e72 0100 0000 2901 da06 5365  tion.r....)...Se
-000005c0: 7276 6572 6300 0000 0000 0000 0000 0000  rverc...........
-000005d0: 0000 0000 0002 0000 0013 0000 0073 0800  .............s..
-000005e0: 0000 7400 8800 8301 5300 a901 4ea9 0172  ..t.....S...N..r
-000005f0: 0f00 0000 720d 0000 0072 0b00 0000 720d  ....r....r....r.
-00000600: 0000 0072 0e00 0000 da08 3c6c 616d 6264  ...r......<lambd
-00000610: 613e 3800 0000 f300 0000 007a 1c6c 6976  a>8........z.liv
-00000620: 6572 656c 6f61 642e 3c6c 6f63 616c 733e  ereload.<locals>
-00000630: 2e3c 6c61 6d62 6461 3e7a 032e 6d64 7a04  .<lambda>z..mdz.
-00000640: 2e72 7374 7a0b 7b30 7d2f 2a2a 2f2a 7b31  .rstz.{0}/**/*{1
-00000650: 7dda 0450 4154 4863 0000 0000 0000 0000  }..PATHc........
-00000660: 0000 0000 0000 0000 0200 0000 1300 0000  ................
-00000670: 7308 0000 0074 0088 0083 0153 0072 2100  s....t.....S.r!.
-00000680: 0000 7222 0000 0072 0d00 0000 720b 0000  ..r"...r....r...
-00000690: 0072 0d00 0000 720e 0000 0072 2300 0000  .r....r....r#...
-000006a0: 3d00 0000 7224 0000 005a 0554 4845 4d45  =...r$...Z.THEME
-000006b0: 7a13 7b7d 2f74 656d 706c 6174 6573 2f2a  z.{}/templates/*
-000006c0: 2e68 746d 6c63 0000 0000 0000 0000 0000  .htmlc..........
-000006d0: 0000 0000 0000 0200 0000 1300 0000 7308  ..............s.
-000006e0: 0000 0074 0088 0083 0153 0072 2100 0000  ...t.....S.r!...
-000006f0: 7222 0000 0072 0d00 0000 720b 0000 0072  r"...r....r....r
-00000700: 0d00 0000 720e 0000 0072 2300 0000 4000  ....r....r#...@.
-00000710: 0000 7224 0000 007a 042e 6373 737a 032e  ..r$...z..cssz..
-00000720: 6a73 7a12 7b30 7d2f 7374 6174 6963 2f2a  jsz.{0}/static/*
-00000730: 2a2f 2a7b 317d 6300 0000 0000 0000 0000  */*{1}c.........
-00000740: 0000 0000 0000 0002 0000 0013 0000 0073  ...............s
-00000750: 0800 0000 7400 8800 8301 5300 7221 0000  ....t.....S.r!..
-00000760: 0072 2200 0000 720d 0000 0072 0b00 0000  .r"...r....r....
-00000770: 720d 0000 0072 0e00 0000 7223 0000 0044  r....r....r#...D
-00000780: 0000 0072 2400 0000 5a0b 4f55 5450 5554  ...r$...Z.OUTPUT
-00000790: 5f50 4154 4829 03da 0468 6f73 74da 0470  _PATH)...host..p
-000007a0: 6f72 74da 0472 6f6f 744e 2908 da0a 6c69  ort..rootN)...li
-000007b0: 7665 7265 6c6f 6164 7220 0000 0072 0f00  vereloadr ...r..
-000007c0: 0000 5a05 7761 7463 6872 0a00 0000 7213  ..Z.watchr....r.
-000007d0: 0000 00da 0853 4554 5449 4e47 535a 0573  .....SETTINGSZ.s
-000007e0: 6572 7665 290b 720c 0000 0072 2600 0000  erve).r....r&...
-000007f0: 7227 0000 0072 2000 0000 da06 7365 7276  r'...r .....serv
-00000800: 6572 5a17 636f 6e74 656e 745f 6669 6c65  erZ.content_file
-00000810: 5f65 7874 656e 7369 6f6e 73da 0965 7874  _extensions..ext
-00000820: 656e 7369 6f6e 5a0c 636f 6e74 656e 745f  ensionZ.content_
-00000830: 626c 6f62 5a0a 7468 656d 655f 7061 7468  blobZ.theme_path
-00000840: 5a16 7374 6174 6963 5f66 696c 655f 6578  Z.static_file_ex
-00000850: 7465 6e73 696f 6e73 5a0b 7374 6174 6963  tensionsZ.static
-00000860: 5f66 696c 6572 0d00 0000 720b 0000 0072  _filer....r....r
-00000870: 0e00 0000 7229 0000 0030 0000 0073 1e00  ....r)...0...s..
-00000880: 0000 0003 0c02 0801 0602 1402 0801 0801  ................
-00000890: 1001 1602 0801 1a01 0801 0801 0c01 1602  ................
-000008a0: 7229 0000 0029 014e 2902 721e 0000 0072  r)...).N).r....r
-000008b0: 1f00 0000 2913 7214 0000 00da 0874 6578  ....).r......tex
-000008c0: 7477 7261 7072 0200 0000 da06 696e 766f  twrapr......invo
-000008d0: 6b65 7203 0000 00da 0770 656c 6963 616e  ker......pelican
-000008e0: 7204 0000 0072 0900 0000 5a10 7065 6c69  r....r....Z.peli
-000008f0: 6361 6e2e 7365 7474 696e 6773 7205 0000  can.settingsr...
-00000900: 0072 0600 0000 720a 0000 0072 2a00 0000  .r....r....r*...
-00000910: da06 7570 6461 7465 5a0e 4c4f 4341 4c5f  ..updateZ.LOCAL_
-00000920: 5345 5454 494e 4753 7212 0000 0072 0f00  SETTINGSr....r..
-00000930: 0000 721d 0000 0072 2900 0000 720d 0000  ..r....r)...r...
-00000940: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000950: da08 3c6d 6f64 756c 653e 0200 0000 7320  ..<module>....s 
-00000960: 0000 0008 010c 020c 010c 0110 0204 0104  ................
-00000970: 010a 0108 010a 0304 0302 010a 0502 010c  ................
-00000980: 1602 01                                  ...
+00000020: 0007 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
+00000070: 0100 6406 5a0c 6900 5a0d 650d a00e 650a  ..d.Z.i.Z.e...e.
+00000080: a101 0100 650b 650c 8301 5a0f 650d a00e  ....e.e...Z.e...
+00000090: 650f a101 0100 6407 5a10 6501 6a11 a012  e.....d.Z.e.j...
+000000a0: 6501 6a11 a013 6501 6a11 a014 6515 a101  e.j...e.j...e...
+000000b0: a101 6408 a102 5a16 6505 6409 640a 8400  ..d...Z.e.d.d...
+000000c0: 8301 5a17 6505 6415 640b 640c 8401 8301  ..Z.e.d.d.d.....
+000000d0: 5a18 6505 6416 640d 640e 8401 8301 5a19  Z.e.d.d.d.....Z.
+000000e0: 6505 6417 640f 6410 8401 8301 5a1a 6505  e.d.d.d.....Z.e.
+000000f0: 6418 6413 6414 8401 8301 5a1b 6401 5300  d.d.d.....Z.d.S.
+00000100: 2919 e900 0000 004e 2901 da06 6465 6465  )......N)...dede
+00000110: 6e74 2901 da04 7461 736b 2901 da04 6d61  nt)...task)...ma
+00000120: 696e 2902 da0e 4445 4641 554c 545f 434f  in)...DEFAULT_CO
+00000130: 4e46 4947 da16 6765 745f 7365 7474 696e  NFIG..get_settin
+00000140: 6773 5f66 726f 6d5f 6669 6c65 7a0e 7065  gs_from_filez.pe
+00000150: 6c69 6361 6e63 6f6e 662e 7079 7a0e 7075  licanconf.pyz.pu
+00000160: 626c 6973 6863 6f6e 662e 7079 7a19 646f  blishconf.pyz.do
+00000170: 636b 6572 2d63 6f6d 706f 7365 2e76 6572  cker-compose.ver
+00000180: 6966 792e 796d 6c63 0100 0000 0000 0000  ify.ymlc........
+00000190: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000001a0: 7310 0000 0074 0064 0174 0167 0283 0101  s....t.d.t.g....
+000001b0: 0064 0253 0029 03fa 1b42 7569 6c64 206c  .d.S.)...Build l
+000001c0: 6f63 616c 2076 6572 7369 6f6e 206f 6620  ocal version of 
+000001d0: 7369 7465 fa02 2d73 4e29 02da 0c70 656c  site..-sN)...pel
+000001e0: 6963 616e 5f6d 6169 6eda 1253 4554 5449  ican_main..SETTI
+000001f0: 4e47 535f 4649 4c45 5f42 4153 45a9 01da  NGS_FILE_BASE...
+00000200: 0163 a900 720d 0000 00fa 532f 6f70 742f  .c..r.....S/opt/
+00000210: 686f 7374 6564 746f 6f6c 6361 6368 652f  hostedtoolcache/
+00000220: 5079 7468 6f6e 2f33 2e38 2e37 2f78 3634  Python/3.8.7/x64
+00000230: 2f6c 6962 2f70 7974 686f 6e33 2e38 2f73  /lib/python3.8/s
+00000240: 6974 652d 7061 636b 6167 6573 2f76 6f6c  ite-packages/vol
+00000250: 7461 6972 652f 7461 736b 732e 7079 da05  taire/tasks.py..
+00000260: 6275 696c 6417 0000 0073 0200 0000 0003  build....s......
+00000270: 720f 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00000280: 0000 0400 0000 0900 0000 4300 0000 738a  ..........C...s.
+00000290: 0000 0074 0064 0174 0164 0264 0367 0483  ...t.d.t.d.d.g..
+000002a0: 0101 0064 04a0 0274 036a 04a0 05a1 00a0  ...d...t.j......
+000002b0: 06a1 00a1 017d 027c 0172 7474 0764 0564  .....}.|.rtt.d.d
+000002c0: 0683 028f 107d 037c 03a0 087c 01a1 0101  .....}.|...|....
+000002d0: 0057 0035 0051 0052 0058 0074 0764 0764  .W.5.Q.R.X.t.d.d
+000002e0: 0683 028f 1c7d 037c 03a0 0874 0964 087c  .....}.|...t.d.|
+000002f0: 019b 0064 099d 0383 01a1 0101 0057 0035  ...d.........W.5
+00000300: 0051 0052 0058 007c 00a0 0a64 0a7c 029b  .Q.R.X.|...d.|..
+00000310: 0064 0b9d 03a1 0101 0064 0c53 0029 0d72  .d.......d.S.).r
+00000320: 0700 0000 7208 0000 00fa 082d 2d6f 7574  ....r......--out
+00000330: 7075 74da 0464 6973 747a 1427 5075 626c  put..distz.'Publ
+00000340: 6973 6820 7369 7465 206f 6e20 7b7d 27fa  ish site on {}'.
+00000350: 0a64 6973 742f 434e 414d 45da 0177 fa0f  .dist/CNAME..w..
+00000360: 6469 7374 2f72 6f62 6f74 732e 7478 74fa  dist/robots.txt.
+00000370: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
+00000380: 2020 5573 6572 2d61 6765 6e74 3a20 2a0a    User-agent: *.
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 4469 7361 6c6c 6f77 3a20 2f64 7261 6674  Disallow: /draft
+000003b0: 732f 0a20 2020 2020 2020 2020 2020 2020  s/.             
+000003c0: 2020 2053 6974 656d 6170 3a20 6874 7470     Sitemap: http
+000003d0: 3a2f 2ffa 192f 7369 7465 6d61 702e 786d  ://../sitemap.xm
+000003e0: 6c0a 2020 2020 2020 2020 2020 2020 7a1a  l.            z.
+000003f0: 6768 702d 696d 706f 7274 202d 6220 6768  ghp-import -b gh
+00000400: 2d70 6167 6573 202d 6d20 7a08 2064 6973  -pages -m z. dis
+00000410: 7420 2d70 4e29 0b72 0900 0000 da11 5055  t -pN).r......PU
+00000420: 424c 4953 485f 4649 4c45 5f42 4153 45da  BLISH_FILE_BASE.
+00000430: 0666 6f72 6d61 74da 0864 6174 6574 696d  .format..datetim
+00000440: 65da 0464 6174 65da 0574 6f64 6179 da09  e..date..today..
+00000450: 6973 6f66 6f72 6d61 74da 046f 7065 6eda  isoformat..open.
+00000460: 0577 7269 7465 7202 0000 00da 0372 756e  .writer......run
+00000470: 2904 720c 0000 00da 0664 6f6d 6169 6e5a  ).r......domainZ
+00000480: 0e63 6f6d 6d69 745f 6d65 7373 6167 65da  .commit_message.
+00000490: 0166 720d 0000 0072 0d00 0000 720e 0000  .fr....r....r...
+000004a0: 00da 0770 7562 6c69 7368 1d00 0000 7320  ...publish....s 
+000004b0: 0000 0000 0310 0104 010c ff04 0304 010c  ................
+000004c0: 0114 010c 0104 0102 0102 0302 fd06 ff02  ................
+000004d0: ff0e 0972 2200 0000 6302 0000 0000 0000  ...r"...c.......
+000004e0: 0000 0000 0003 0000 0009 0000 0043 0000  .............C..
+000004f0: 0073 6e00 0000 7400 6401 7401 6402 6403  .sn...t.d.t.d.d.
+00000500: 6704 8301 0100 7c01 7260 7402 6404 6405  g.....|.r`t.d.d.
+00000510: 8302 8f10 7d02 7c02 a003 7c01 a101 0100  ....}.|...|.....
+00000520: 5700 3500 5100 5200 5800 7402 6406 6405  W.5.Q.R.X.t.d.d.
+00000530: 8302 8f1c 7d02 7c02 a003 7404 6407 7c01  ....}.|...t.d.|.
+00000540: 9b00 6408 9d03 8301 a101 0100 5700 3500  ..d.........W.5.
+00000550: 5100 5200 5800 7c00 a005 6409 a101 0100  Q.R.X.|...d.....
+00000560: 6400 5300 290a 4e72 0800 0000 7210 0000  d.S.).Nr....r...
+00000570: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000580: 7214 0000 0072 1500 0000 7216 0000 007a  r....r....r....z
+00000590: 3c64 6f63 6b65 7220 7275 6e20 2d76 2024  <docker run -v $
+000005a0: 5057 442f 6469 7374 3a2f 7573 722f 7368  PWD/dist:/usr/sh
+000005b0: 6172 652f 6e67 696e 782f 6874 6d6c 202d  are/nginx/html -
+000005c0: 7020 3830 3a38 3020 6e67 696e 7829 0672  p 80:80 nginx).r
+000005d0: 0900 0000 7217 0000 0072 1d00 0000 721e  ....r....r....r.
+000005e0: 0000 0072 0200 0000 721f 0000 00a9 0372  ...r....r......r
+000005f0: 0c00 0000 7220 0000 0072 2100 0000 720d  ....r ...r!...r.
+00000600: 0000 0072 0d00 0000 720e 0000 00da 0573  ...r....r......s
+00000610: 7461 6765 3400 0000 731a 0000 0000 0210  tage4...s.......
+00000620: 0104 010c 0114 010c 0104 0102 0102 0302  ................
+00000630: fd06 ff02 ff0e 0972 2400 0000 6302 0000  .......r$...c...
+00000640: 0000 0000 0000 0000 0003 0000 000b 0000  ................
+00000650: 0043 0000 0073 9600 0000 7400 6401 7401  .C...s....t.d.t.
+00000660: 6402 6403 6704 8301 0100 7c01 7260 7402  d.d.g.....|.r`t.
+00000670: 6404 6405 8302 8f10 7d02 7c02 a003 7c01  d.d.....}.|...|.
+00000680: a101 0100 5700 3500 5100 5200 5800 7402  ....W.5.Q.R.X.t.
+00000690: 6406 6405 8302 8f1c 7d02 7c02 a003 7404  d.d.....}.|...t.
+000006a0: 6407 7c01 9b00 6408 9d03 8301 a101 0100  d.|...d.........
+000006b0: 5700 3500 5100 5200 5800 7a1c 7c00 a005  W.5.Q.R.X.z.|...
+000006c0: 640b 7c01 9b00 640c 7406 9b00 640d 9d05  d.|...d.t...d...
+000006d0: a101 0100 5700 3500 7c00 a005 6409 7406  ....W.5.|...d.t.
+000006e0: 9b00 640a 9d03 a101 0100 5800 6400 5300  ..d.......X.d.S.
+000006f0: 290e 4e72 0800 0000 7210 0000 0072 1100  ).Nr....r....r..
+00000700: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000710: 0072 1500 0000 7216 0000 007a 1264 6f63  .r....r....z.doc
+00000720: 6b65 722d 636f 6d70 6f73 6520 2d66 207a  ker-compose -f z
+00000730: 2220 646f 776e 202d 2d72 6d69 206c 6f63  " down --rmi loc
+00000740: 616c 202d 2d72 656d 6f76 652d 6f72 7068  al --remove-orph
+00000750: 616e 737a 0744 4f4d 4149 4e3d 7a13 2064  ansz.DOMAIN=z. d
+00000760: 6f63 6b65 722d 636f 6d70 6f73 6520 2d66  ocker-compose -f
+00000770: 207a 5220 7570 202d 2d62 7569 6c64 202d   zR up --build -
+00000780: 2d61 626f 7274 2d6f 6e2d 636f 6e74 6169  -abort-on-contai
+00000790: 6e65 722d 6578 6974 202d 2d65 7869 742d  ner-exit --exit-
+000007a0: 636f 6465 2d66 726f 6d20 7665 7269 6679  code-from verify
+000007b0: 202d 2d72 656e 6577 2d61 6e6f 6e2d 766f   --renew-anon-vo
+000007c0: 6c75 6d65 7329 0772 0900 0000 7217 0000  lumes).r....r...
+000007d0: 0072 1d00 0000 721e 0000 0072 0200 0000  .r....r....r....
+000007e0: 721f 0000 00da 0c43 4f4d 504f 5345 5f59  r......COMPOSE_Y
+000007f0: 414d 4c72 2300 0000 720d 0000 0072 0d00  AMLr#...r....r..
+00000800: 0000 720e 0000 00da 0676 6572 6966 7947  ..r......verifyG
+00000810: 0000 0073 2600 0000 0002 1001 0401 0c01  ...s&...........
+00000820: 1401 0c01 0401 0201 0203 02fd 06ff 02ff  ................
+00000830: 0e09 0201 0401 10ff 0804 0401 0aff 7226  ..............r&
+00000840: 0000 00da 096c 6f63 616c 686f 7374 e940  .....localhost.@
+00000850: 1f00 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000860: 0b00 0000 0700 0000 0300 0000 73d0 0000  ............s...
+00000870: 0064 0164 026c 006d 017d 0301 0074 0288  .d.d.l.m.}...t..
+00000880: 0083 0101 007c 0383 007d 047c 04a0 0374  .....|...}.|...t
+00000890: 0487 0066 0164 0364 0484 08a1 0201 0064  ...f.d.d.......d
+000008a0: 0564 0667 027d 057c 0544 005d 287d 0664  .d.g.}.|.D.](}.d
+000008b0: 07a0 0574 0664 0819 007c 06a1 027d 077c  ...t.d...|...}.|
+000008c0: 04a0 037c 0787 0066 0164 0964 0484 08a1  ...|...f.d.d....
+000008d0: 0201 0071 3a74 0664 0a19 007d 087c 04a0  ...q:t.d...}.|..
+000008e0: 0364 0ba0 057c 08a1 0187 0066 0164 0c64  .d...|.....f.d.d
+000008f0: 0484 08a1 0201 0064 0d64 0e67 027d 097c  .......d.d.g.}.|
+00000900: 0944 005d 247d 0664 0fa0 057c 087c 06a1  .D.]$}.d...|.|..
+00000910: 027d 0a7c 04a0 037c 0a87 0066 0164 1064  .}.|...|...f.d.d
+00000920: 0484 08a1 0201 0071 927c 046a 077c 017c  .......q.|.j.|.|
+00000930: 0274 0664 1119 0064 128d 0301 0064 1353  .t.d...d.....d.S
+00000940: 0029 147a 3841 7574 6f6d 6174 6963 616c  .).z8Automatical
+00000950: 6c79 2072 656c 6f61 6420 6272 6f77 7365  ly reload browse
+00000960: 7220 7461 6220 7570 6f6e 2066 696c 6520  r tab upon file 
+00000970: 6d6f 6469 6669 6361 7469 6f6e 2e72 0100  modification.r..
+00000980: 0000 2901 da06 5365 7276 6572 6300 0000  ..)...Serverc...
+00000990: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+000009a0: 0013 0000 0073 0800 0000 7400 8800 8301  .....s....t.....
+000009b0: 5300 a901 4ea9 0172 0f00 0000 720d 0000  S...N..r....r...
+000009c0: 0072 0b00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+000009d0: da08 3c6c 616d 6264 613e 6900 0000 f300  ..<lambda>i.....
+000009e0: 0000 007a 1c6c 6976 6572 656c 6f61 642e  ...z.livereload.
+000009f0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00000a00: 3e7a 032e 6d64 7a04 2e72 7374 7a0b 7b30  >z..mdz..rstz.{0
+00000a10: 7d2f 2a2a 2f2a 7b31 7dda 0450 4154 4863  }/**/*{1}..PATHc
+00000a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000a30: 0200 0000 1300 0000 7308 0000 0074 0088  ........s....t..
+00000a40: 0083 0153 0072 2a00 0000 722b 0000 0072  ...S.r*...r+...r
+00000a50: 0d00 0000 720b 0000 0072 0d00 0000 720e  ....r....r....r.
+00000a60: 0000 0072 2c00 0000 6e00 0000 722d 0000  ...r,...n...r-..
+00000a70: 005a 0554 4845 4d45 7a13 7b7d 2f74 656d  .Z.THEMEz.{}/tem
+00000a80: 706c 6174 6573 2f2a 2e68 746d 6c63 0000  plates/*.htmlc..
+00000a90: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000aa0: 0000 1300 0000 7308 0000 0074 0088 0083  ......s....t....
+00000ab0: 0153 0072 2a00 0000 722b 0000 0072 0d00  .S.r*...r+...r..
+00000ac0: 0000 720b 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000ad0: 0072 2c00 0000 7100 0000 722d 0000 007a  .r,...q...r-...z
+00000ae0: 042e 6373 737a 032e 6a73 7a12 7b30 7d2f  ..cssz..jsz.{0}/
+00000af0: 7374 6174 6963 2f2a 2a2f 2a7b 317d 6300  static/**/*{1}c.
+00000b00: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000b10: 0000 0013 0000 0073 0800 0000 7400 8800  .......s....t...
+00000b20: 8301 5300 722a 0000 0072 2b00 0000 720d  ..S.r*...r+...r.
+00000b30: 0000 0072 0b00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000b40: 0000 722c 0000 0075 0000 0072 2d00 0000  ..r,...u...r-...
+00000b50: 5a0b 4f55 5450 5554 5f50 4154 4829 03da  Z.OUTPUT_PATH)..
+00000b60: 0468 6f73 74da 0470 6f72 74da 0472 6f6f  .host..port..roo
+00000b70: 744e 2908 da0a 6c69 7665 7265 6c6f 6164  tN)...livereload
+00000b80: 7229 0000 0072 0f00 0000 5a05 7761 7463  r)...r....Z.watc
+00000b90: 6872 0a00 0000 7218 0000 00da 0853 4554  hr....r......SET
+00000ba0: 5449 4e47 535a 0573 6572 7665 290b 720c  TINGSZ.serve).r.
+00000bb0: 0000 0072 2f00 0000 7230 0000 0072 2900  ...r/...r0...r).
+00000bc0: 0000 da06 7365 7276 6572 5a17 636f 6e74  ....serverZ.cont
+00000bd0: 656e 745f 6669 6c65 5f65 7874 656e 7369  ent_file_extensi
+00000be0: 6f6e 73da 0965 7874 656e 7369 6f6e 5a0c  ons..extensionZ.
+00000bf0: 636f 6e74 656e 745f 626c 6f62 5a0a 7468  content_blobZ.th
+00000c00: 656d 655f 7061 7468 5a16 7374 6174 6963  eme_pathZ.static
+00000c10: 5f66 696c 655f 6578 7465 6e73 696f 6e73  _file_extensions
+00000c20: 5a0b 7374 6174 6963 5f66 696c 6572 0d00  Z.static_filer..
+00000c30: 0000 720b 0000 0072 0e00 0000 7232 0000  ..r....r....r2..
+00000c40: 0061 0000 0073 1e00 0000 0003 0c02 0801  .a...s..........
+00000c50: 0602 1402 0801 0801 1001 1602 0801 1a01  ................
+00000c60: 0801 0801 0c01 1602 7232 0000 0029 014e  ........r2...).N
+00000c70: 2901 4e29 014e 2902 7227 0000 0072 2800  ).N).N).r'...r(.
+00000c80: 0000 291c 7219 0000 00da 026f 73da 0874  ..).r......os..t
+00000c90: 6578 7477 7261 7072 0200 0000 da06 696e  extwrapr......in
+00000ca0: 766f 6b65 7203 0000 00da 0770 656c 6963  voker......pelic
+00000cb0: 616e 7204 0000 0072 0900 0000 5a10 7065  anr....r....Z.pe
+00000cc0: 6c69 6361 6e2e 7365 7474 696e 6773 7205  lican.settingsr.
+00000cd0: 0000 0072 0600 0000 720a 0000 0072 3300  ...r....r....r3.
+00000ce0: 0000 da06 7570 6461 7465 5a0e 4c4f 4341  ....updateZ.LOCA
+00000cf0: 4c5f 5345 5454 494e 4753 7217 0000 00da  L_SETTINGSr.....
+00000d00: 0470 6174 68da 046a 6f69 6eda 0764 6972  .path..join..dir
+00000d10: 6e61 6d65 da08 7265 616c 7061 7468 da08  name..realpath..
+00000d20: 5f5f 6669 6c65 5f5f 7225 0000 0072 0f00  __file__r%...r..
+00000d30: 0000 7222 0000 0072 2400 0000 7226 0000  ..r"...r$...r&..
+00000d40: 0072 3200 0000 720d 0000 0072 0d00 0000  .r2...r....r....
+00000d50: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+00000d60: 756c 653e 0200 0000 7332 0000 0008 0108  ule>....s2......
+00000d70: 010c 020c 010c 0110 0204 0104 010a 0108  ................
+00000d80: 010a 0304 0106 0112 0002 ff04 0502 010a  ................
+00000d90: 0502 010c 1602 010c 1202 010c 1902 01    ...............
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/__pycache__/wikilinks.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Jan 15 01:44:39 2021 UTC, .py size: 1135 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,77 +1,77 @@
-00000000: 550d 0d0a 0000 0000 87f3 0060 6f04 0000  U..........`o...
+00000000: 550d 0d0a 0000 0000 90eb 1c60 8d04 0000  U..........`....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6406 5a09 650a 650a 6407  m.Z...d.Z.e.e.d.
 00000070: 9c02 6408 6409 8404 5a0b 6506 640a 9c01  ..d.d...Z.e.d...
 00000080: 640b 640c 8404 5a0c 640d 640e 8400 5a0d  d.d...Z.d.d...Z.
 00000090: 6401 5300 290f e900 0000 004e 2901 da05  d.S.)......N)...
 000000a0: 4d61 7463 6829 01da 0773 6967 6e61 6c73  Match)...signals
 000000b0: 2901 da07 436f 6e74 656e 7429 01da 0773  )...Content)...s
 000000c0: 6c75 6769 6679 5a09 5749 4b49 4c49 4e4b  lugifyZ.WIKILINK
 000000d0: 5329 02da 0474 6578 74da 0672 6574 7572  S)...text..retur
 000000e0: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
-000000f0: 0000 0500 0000 4300 0000 7324 0000 0074  ......C...s$...t
+000000f0: 0000 0500 0000 4300 0000 7328 0000 0074  ......C...s(...t
 00000100: 0064 019c 0164 0264 0384 047d 017c 0072  .d...d.d...}.|.r
-00000110: 2074 01a0 0264 047c 017c 00a1 0353 0064   t...d.|.|...S.d
-00000120: 0053 0029 054e 2901 da05 6772 6f75 7063  .S.).N)...groupc
-00000130: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000140: 0600 0000 5300 0000 733a 0000 007c 00a0  ....S...s:...|..
-00000150: 00a1 005c 027d 017d 027c 0273 147c 017d  ...\.}.}.|.s.|.}
-00000160: 0274 017c 0164 0164 0264 0364 0467 0464  .t.|.d.d.d.d.g.d
-00000170: 058d 027d 0164 067c 019b 0064 077c 029b  ...}.d.|...d.|..
-00000180: 0064 089d 0553 0029 094e 2902 7a08 5b5e  .d...S.).N).z.[^
-00000190: 5c77 5c73 2d5d da00 2902 7a09 283f 7529  \w\s-]..).z.(?u)
-000001a0: 5c41 5c73 2a72 0900 0000 2902 7a09 283f  \A\s*r....).z.(?
-000001b0: 7529 5c73 2a5c 5a72 0900 0000 2902 7a06  u)\s*\Zr....).z.
-000001c0: 5b2d 5c73 5d2b fa01 2d29 015a 0a72 6567  [-\s]+..-).Z.reg
-000001d0: 6578 5f73 7562 737a 0a3c 6120 6872 6566  ex_subsz.<a href
-000001e0: 3d22 2f7a 032f 223e 7a04 3c2f 613e 2902  ="/z./">z.</a>).
-000001f0: da06 6772 6f75 7073 7205 0000 0029 0372  ..groupsr....).r
-00000200: 0800 0000 5a04 6872 6566 7206 0000 00a9  ....Z.hrefr.....
-00000210: 0072 0c00 0000 fa57 2f6f 7074 2f68 6f73  .r.....W/opt/hos
-00000220: 7465 6474 6f6f 6c63 6163 6865 2f50 7974  tedtoolcache/Pyt
-00000230: 686f 6e2f 332e 382e 372f 7836 342f 6c69  hon/3.8.7/x64/li
-00000240: 622f 7079 7468 6f6e 332e 382f 7369 7465  b/python3.8/site
-00000250: 2d70 6163 6b61 6765 732f 766f 6c74 6169  -packages/voltai
-00000260: 7265 2f77 696b 696c 696e 6b73 2e70 79da  re/wikilinks.py.
-00000270: 0472 6570 6c0c 0000 0073 1800 0000 0001  .repl....s......
-00000280: 0c01 0401 0401 0201 0202 0204 0201 0201  ................
-00000290: 02f9 02fe 060f 7a1f 7265 706c 6163 655f  ......z.replace_
-000002a0: 7769 6b69 6c69 6e6b 732e 3c6c 6f63 616c  wikilinks.<local
-000002b0: 733e 2e72 6570 6c7a 195c 5b5c 5b28 5b5e  s>.replz.\[\[([^
-000002c0: 7c5c 5d5d 2b29 5c7c 3f28 2e2a 3f29 5c5d  |\]]+)\|?(.*?)\]
-000002d0: 5c5d 2903 7202 0000 00da 0272 65da 0373  \]).r......re..s
-000002e0: 7562 2902 7206 0000 0072 0e00 0000 720c  ub).r....r....r.
-000002f0: 0000 0072 0c00 0000 720d 0000 00da 1172  ...r....r......r
-00000300: 6570 6c61 6365 5f77 696b 696c 696e 6b73  eplace_wikilinks
-00000310: 0b00 0000 7306 0000 0000 010e 1504 0172  ....s..........r
-00000320: 1100 0000 a901 da08 696e 7374 616e 6365  ........instance
-00000330: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000340: 0002 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
-00000350: 7c00 6a01 8301 7c00 5f01 6400 5300 a901  |.j...|._.d.S...
-00000360: 4e29 0272 1100 0000 5a08 5f63 6f6e 7465  N).r....Z._conte
-00000370: 6e74 7212 0000 0072 0c00 0000 720c 0000  ntr....r....r...
-00000380: 0072 0d00 0000 da13 636f 6e74 656e 745f  .r......content_
-00000390: 6f62 6a65 6374 5f69 6e69 7425 0000 0073  object_init%...s
-000003a0: 0200 0000 0001 7215 0000 0063 0000 0000  ......r....c....
-000003b0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000003c0: 4300 0000 7310 0000 0074 006a 01a0 0274  C...s....t.j...t
-000003d0: 01a1 0101 0064 0053 0072 1400 0000 2903  .....d.S.r....).
-000003e0: 7203 0000 0072 1500 0000 da07 636f 6e6e  r....r......conn
-000003f0: 6563 7472 0c00 0000 720c 0000 0072 0c00  ectr....r....r..
-00000400: 0000 720d 0000 00da 0872 6567 6973 7465  ..r......registe
-00000410: 7229 0000 0073 0200 0000 0001 7217 0000  r)...s......r...
-00000420: 0029 0e72 0f00 0000 da06 7479 7069 6e67  .).r......typing
-00000430: 7202 0000 00da 0770 656c 6963 616e 7203  r......pelicanr.
-00000440: 0000 005a 1070 656c 6963 616e 2e63 6f6e  ...Z.pelican.con
-00000450: 7465 6e74 7372 0400 0000 5a0d 7065 6c69  tentsr....Z.peli
-00000460: 6361 6e2e 7574 696c 7372 0500 0000 5a0d  can.utilsr....Z.
-00000470: 5345 5454 494e 4753 5f4e 414d 45da 0373  SETTINGS_NAME..s
-00000480: 7472 7211 0000 0072 1500 0000 7217 0000  trr....r....r...
-00000490: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000004a0: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000004b0: 0000 0073 1000 0000 0801 0c02 0c01 0c01  ...s............
-000004c0: 0c02 0403 101a 0e04                      ........
+00000110: 2074 01a0 0264 047c 017c 00a1 0353 007c   t...d.|.|...S.|
+00000120: 0053 0064 0053 0029 054e 2901 da05 6772  .S.d.S.).N)...gr
+00000130: 6f75 7063 0100 0000 0000 0000 0000 0000  oupc............
+00000140: 0300 0000 0600 0000 5300 0000 733a 0000  ........S...s:..
+00000150: 007c 00a0 00a1 005c 027d 017d 027c 0273  .|.....\.}.}.|.s
+00000160: 147c 017d 0274 017c 0164 0164 0264 0364  .|.}.t.|.d.d.d.d
+00000170: 0467 0464 058d 027d 0164 067c 019b 0064  .g.d...}.d.|...d
+00000180: 077c 029b 0064 089d 0553 0029 094e 2902  .|...d...S.).N).
+00000190: 7a08 5b5e 5c77 5c73 2d5d da00 2902 7a09  z.[^\w\s-]..).z.
+000001a0: 283f 7529 5c41 5c73 2a72 0900 0000 2902  (?u)\A\s*r....).
+000001b0: 7a09 283f 7529 5c73 2a5c 5a72 0900 0000  z.(?u)\s*\Zr....
+000001c0: 2902 7a06 5b2d 5c73 5d2b fa01 2d29 015a  ).z.[-\s]+..-).Z
+000001d0: 0a72 6567 6578 5f73 7562 737a 0a3c 6120  .regex_subsz.<a 
+000001e0: 6872 6566 3d22 2f7a 032f 223e 7a04 3c2f  href="/z./">z.</
+000001f0: 613e 2902 da06 6772 6f75 7073 7205 0000  a>)...groupsr...
+00000200: 0029 0372 0800 0000 5a04 6872 6566 7206  .).r....Z.hrefr.
+00000210: 0000 00a9 0072 0c00 0000 fa57 2f6f 7074  .....r.....W/opt
+00000220: 2f68 6f73 7465 6474 6f6f 6c63 6163 6865  /hostedtoolcache
+00000230: 2f50 7974 686f 6e2f 332e 382e 372f 7836  /Python/3.8.7/x6
+00000240: 342f 6c69 622f 7079 7468 6f6e 332e 382f  4/lib/python3.8/
+00000250: 7369 7465 2d70 6163 6b61 6765 732f 766f  site-packages/vo
+00000260: 6c74 6169 7265 2f77 696b 696c 696e 6b73  ltaire/wikilinks
+00000270: 2e70 79da 0472 6570 6c0c 0000 0073 1800  .py..repl....s..
+00000280: 0000 0001 0c01 0401 0401 0201 0202 0204  ................
+00000290: 0201 0201 02f9 02fe 060f 7a1f 7265 706c  ..........z.repl
+000002a0: 6163 655f 7769 6b69 6c69 6e6b 732e 3c6c  ace_wikilinks.<l
+000002b0: 6f63 616c 733e 2e72 6570 6c7a 195c 5b5c  ocals>.replz.\[\
+000002c0: 5b28 5b5e 7c5c 5d5d 2b29 5c7c 3f28 2e2a  [([^|\]]+)\|?(.*
+000002d0: 3f29 5c5d 5c5d 2903 7202 0000 00da 0272  ?)\]\]).r......r
+000002e0: 65da 0373 7562 2902 7206 0000 0072 0e00  e..sub).r....r..
+000002f0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000300: 00da 1172 6570 6c61 6365 5f77 696b 696c  ...replace_wikil
+00000310: 696e 6b73 0b00 0000 7308 0000 0000 010e  inks....s.......
+00000320: 1504 010e 0272 1100 0000 a901 da08 696e  .....r........in
+00000330: 7374 616e 6365 6301 0000 0000 0000 0000  stancec.........
+00000340: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000350: 1000 0000 7400 7c00 6a01 8301 7c00 5f01  ....t.|.j...|._.
+00000360: 6400 5300 a901 4e29 0272 1100 0000 5a08  d.S...N).r....Z.
+00000370: 5f63 6f6e 7465 6e74 7212 0000 0072 0c00  _contentr....r..
+00000380: 0000 720c 0000 0072 0d00 0000 da13 636f  ..r....r......co
+00000390: 6e74 656e 745f 6f62 6a65 6374 5f69 6e69  ntent_object_ini
+000003a0: 7427 0000 0073 0200 0000 0001 7215 0000  t'...s......r...
+000003b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000003c0: 0000 0300 0000 4300 0000 7310 0000 0074  ......C...s....t
+000003d0: 006a 01a0 0274 01a1 0101 0064 0053 0072  .j...t.....d.S.r
+000003e0: 1400 0000 2903 7203 0000 0072 1500 0000  ....).r....r....
+000003f0: da07 636f 6e6e 6563 7472 0c00 0000 720c  ..connectr....r.
+00000400: 0000 0072 0c00 0000 720d 0000 00da 0872  ...r....r......r
+00000410: 6567 6973 7465 722b 0000 0073 0200 0000  egister+...s....
+00000420: 0001 7217 0000 0029 0e72 0f00 0000 da06  ..r....).r......
+00000430: 7479 7069 6e67 7202 0000 00da 0770 656c  typingr......pel
+00000440: 6963 616e 7203 0000 005a 1070 656c 6963  icanr....Z.pelic
+00000450: 616e 2e63 6f6e 7465 6e74 7372 0400 0000  an.contentsr....
+00000460: 5a0d 7065 6c69 6361 6e2e 7574 696c 7372  Z.pelican.utilsr
+00000470: 0500 0000 5a0d 5345 5454 494e 4753 5f4e  ....Z.SETTINGS_N
+00000480: 414d 45da 0373 7472 7211 0000 0072 1500  AME..strr....r..
+00000490: 0000 7217 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+000004a0: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
+000004b0: 6475 6c65 3e01 0000 0073 1000 0000 0801  dule>....s......
+000004c0: 0c02 0c01 0c01 0c02 0403 101c 0e04       ..............
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/_version.py

```diff
@@ -1,5 +1,5 @@
 # coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = '0.8.9'
-version_tuple = (0, 8, 9)
+version = '0.9.0'
+version_tuple = (0, 9, 0)
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/mermaid.py

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 import tempfile
 from subprocess import PIPE, Popen
-from typing import Iterable, Text
+from typing import Iterable, List, Text
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 MERMAID_START = re.compile(r"^```[\ \t]*[Mm]ermaid[\ \t]*$")
 MERMAID_END = re.compile(r"^```[\ \t]*$")
 CONF_FILE = os.path.join(
@@ -45,20 +45,20 @@
             os.remove(tf.name)
             with open(name) as f:
                 svg_string = f.read()
             os.remove(name)
             return svg_string
         else:
             raise RuntimeError(
-                f"Error calling mermaid: {err}\nTemp files: {tf.name} and {name}"
+                f"Error calling mermaid: {str(err)}\nTemp files: {tf.name} and {name}"
             )
 
 
 class MermaidProcessor(Preprocessor):
-    def run(self, lines: [Text]) -> Iterable[Text]:
+    def run(self, lines: List[Text]) -> Iterable[Text]:
         looking_for_mermaids = True
         mermaid_code = ""
 
         for line in lines:
             # Ad hoc state machine to the rescue! (We only have two states:
             # either we're waiting for a potential Mermaid block or we're in
             # the middle of processing one).
@@ -93,9 +93,11 @@
 class MermaidExtension(Extension):
     def extendMarkdown(self, md):
         md.preprocessors.register(MermaidProcessor(), "mermaid", 35)
         md.registerExtension(self)
 
 
 def makeExtension(**kwargs):  # pragma: no cover
-    os.system("which mmdc || npm install -g @mermaid-js/mermaid-cli")
+    os.system(
+        "which mmdc 2>/dev/null || npm install -g @mermaid-js/mermaid-cli"
+    )
     return MermaidExtension(**kwargs)
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/pelican.py

```diff
@@ -1,13 +1,15 @@
 import os
+from pathlib import Path
+from typing import List, Optional
 
 PATH = "content"
 PAGE_PATHS = ["."]
 ARTICLE_PATHS = ["posts"]
-STATIC_PATHS = []
+STATIC_PATHS: List[str] = []
 
 SLUGIFY_SOURCE = "basename"
 
 PAGE_URL = "{slug}/"
 PAGE_SAVE_AS = "{slug}/index.html"
 
 TIMEZONE = "Europe/London"
@@ -25,17 +27,19 @@
 
 THEME = os.path.join(os.path.dirname(os.path.realpath(__file__)), "theme")
 THEME_STATIC_PATHS = [
     os.path.join(THEME, "static"),
     os.path.join(os.getcwd(), "static"),
 ]
 
-LOCAL_SCSS = os.path.join(os.getcwd(), "static", "css", "style.scss")
-if not os.path.exists(LOCAL_SCSS):
-    LOCAL_SCSS = False
+# LOCAL_SCSS: Optional[str] = os.path.join(os.getcwd(), "static", "css", "style.scss")
+LOCAL_SCSS: Optional[str] = None
+path: Path = Path.cwd() / "static" / "css" / "style.scss"
+if path.exists():
+    LOCAL_SCSS = str(path)
 
 MARKDOWN = {
     "extension_configs": {
         "voltaire.mermaid": {},
         "markdown.extensions.extra": {},
     },
     "output_format": "html5",
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/tasks.py

```diff
@@ -1,23 +1,27 @@
 # -*- coding: utf-8 -*-
 import datetime
+import os
 from textwrap import dedent
 
 from invoke import task
 from pelican import main as pelican_main
 from pelican.settings import DEFAULT_CONFIG, get_settings_from_file
 
 SETTINGS_FILE_BASE = "pelicanconf.py"
 SETTINGS = {}
 SETTINGS.update(DEFAULT_CONFIG)
 LOCAL_SETTINGS = get_settings_from_file(SETTINGS_FILE_BASE)
 SETTINGS.update(LOCAL_SETTINGS)
 
 
 PUBLISH_FILE_BASE = "publishconf.py"
+COMPOSE_YAML = os.path.join(
+    os.path.dirname(os.path.realpath(__file__)), "docker-compose.verify.yml"
+)
 
 
 @task
 def build(c):
     """Build local version of site"""
     pelican_main(["-s", SETTINGS_FILE_BASE])
 
@@ -42,14 +46,59 @@
             """
                 )
             )
     c.run("ghp-import -b gh-pages " f"-m {commit_message} " "dist -p")
 
 
 @task
+def stage(c, domain=None):
+    pelican_main(["-s", PUBLISH_FILE_BASE, "--output", "dist"])
+    if domain:
+        with open("dist/CNAME", "w") as f:
+            f.write(domain)
+        with open("dist/robots.txt", "w") as f:
+            f.write(
+                dedent(
+                    f"""
+                User-agent: *
+                Disallow: /drafts/
+                Sitemap: http://{domain}/sitemap.xml
+            """
+                )
+            )
+    c.run("docker run -v $PWD/dist:/usr/share/nginx/html -p 80:80 nginx")
+
+
+@task
+def verify(c, domain=None):
+    pelican_main(["-s", PUBLISH_FILE_BASE, "--output", "dist"])
+    if domain:
+        with open("dist/CNAME", "w") as f:
+            f.write(domain)
+        with open("dist/robots.txt", "w") as f:
+            f.write(
+                dedent(
+                    f"""
+                User-agent: *
+                Disallow: /drafts/
+                Sitemap: http://{domain}/sitemap.xml
+            """
+                )
+            )
+    try:
+        c.run(
+            f"DOMAIN={domain} docker-compose -f {COMPOSE_YAML} up --build --abort-on-container-exit --exit-code-from verify --renew-anon-volumes"
+        )
+    finally:
+        c.run(
+            f"docker-compose -f {COMPOSE_YAML} down --rmi local --remove-orphans"
+        )
+
+
+@task
 def livereload(c, host="localhost", port=8000):
     """Automatically reload browser tab upon file modification."""
     from livereload import Server
 
     build(c)
     server = Server()
     # Watch the base settings file
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/static/css/common.scss

```diff
@@ -13,15 +13,15 @@
                 }
             }
         }
     }
 
     nav {
         max-width: 40rem;
-        margin: 0 auto;
+        //margin: 0 auto;
         text-align: center;
     }
 }
 
 ol#post-list {
   list-style: none;
   padding: 0;
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/base.html

```diff
@@ -48,38 +48,38 @@
     {% endblock extra_head %}
 
 </head>
 
 <body>
     <header>
         <h1><a href="{{ SITEURL }}/">{{ SITENAME }} <strong>{{ SITESUBTITLE }}</strong></a></h1>
-    </header>
-    <nav>
-        <ul>
-        {% for title, link in MENUITEMS_START %}
-            <li><a href="{{ link }}">{{ title }}</a></li>
-        {% endfor %}
-        {% if DISPLAY_PAGES_ON_MENU %}
-          {% for p in pages %}
-            {% if p.menu %}
-            <li{% if p == page %} class="active"{% endif %}><a href="{{ SITEURL }}/{{ p.url }}">{{ p.menu_title or p.title }}</a></li>
+        <nav>
+            <ul>
+            {% for title, link in MENUITEMS_START %}
+                <li><a href="{{ link }}">{{ title }}</a></li>
+            {% endfor %}
+            {% if DISPLAY_PAGES_ON_MENU %}
+              {% for p in pages %}
+                {% if p.menu %}
+                <li{% if p == page %} class="active"{% endif %}><a href="{{ SITEURL }}/{{ p.url }}">{{ p.menu_title or p.title }}</a></li>
+                {% endif %}
+              {% endfor %}
+            {% else %}
+              {% if DISPLAY_CATEGORIES_ON_MENU %}
+                {% for cat, null in categories %}
+                  <li{% if cat == category %} class="active"{% endif %}><a href="{{ SITEURL }}/{{ cat.url }}">{{ cat }}</a></li>
+                {% endfor %}
+              {% endif %}
             {% endif %}
-          {% endfor %}
-        {% else %}
-          {% if DISPLAY_CATEGORIES_ON_MENU %}
-            {% for cat, null in categories %}
-              <li{% if cat == category %} class="active"{% endif %}><a href="{{ SITEURL }}/{{ cat.url }}">{{ cat }}</a></li>
+            {% for title, link in MENUITEMS_END %}
+                <li><a href="{{ link }}" target="_blank">{{ title }}</a></li>
             {% endfor %}
-          {% endif %}
-        {% endif %}
-        {% for title, link in MENUITEMS_END %}
-            <li><a href="{{ link }}" target="_blank">{{ title }}</a></li>
-        {% endfor %}
-        </ul>
-    </nav>
+            </ul>
+        </nav>
+    </header>
     {% block precontent %}
     {% endblock %}
 	<main>
         {% block content_title %}
         {% endblock %}
         {% block content %}
         {% endblock %}
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/theme/templates/categories.html

```diff
@@ -1,10 +1,12 @@
-
 {% extends "base.html" %}
 {% block content %}
+{% if CATEGORIES_TITLE %}
+<h1>{{ CATEGORIES_TITLE }}</h1>
+{% endif %}
 <ul>
 {% for category, articles in categories %}
     <li><a href="{{ SITEURL }}/{{ category.url }}">{{ category }}</a></li>
 {% endfor %}
 </ul>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
- {% extends "base.html" %} {% block content %}
+{% extends "base.html" %} {% block content %} {% if CATEGORIES_TITLE %}
+****** {{ CATEGORIES_TITLE }} ******
+{% endif %}
     * {% for category, articles in categories %}
     * {{_category_}}
     * {% endfor %}
 {% endblock %}
```

### ./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire/wikilinks.py

```diff
@@ -28,14 +28,16 @@
                 ),  # reduce multiple whitespace or '-' to single '-'
             ],
         )
         return f'<a href="/{href}/">{text}</a>'
 
     if text:
         return re.sub(r"\[\[([^|\]]+)\|?(.*?)\]\]", repl, text)
+    else:
+        return text
 
 
 def content_object_init(instance: Content):
     instance._content = replace_wikilinks(instance._content)
 
 
 def register():
```

### Comparing `./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/PKG-INFO` & `./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: voltaire
-Version: 0.8.9
-Summary: UNKNOWN
+Version: 0.9.0
+Summary: Tools for prolific writers (or more accurately, those that want to be).
 Home-page: https://github.com/avengerpenguin/voltaire
 Author: Ross Fenning
 Author-email: github@rossfenning.co.uk
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/avengerpenguin/voltaire/issues
 Description: # ![Voltaire](https://raw.githubusercontent.com/avengerpenguin/voltaire/main/logo.png)
```

### Comparing `./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.8.9-py3.8.egg-info/SOURCES.txt` & `./opt/hostedtoolcache/Python/3.8.7/x64/lib/python3.8/site-packages/voltaire-0.9.0-py3.8.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
-.travis.yml
 LICENSE
 MANIFEST.in
 README.md
 logo.png
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/python.yml
 tests/test_build.py
 voltaire/__init__.py
 voltaire/_version.py
+voltaire/docker-compose.verify.yml
 voltaire/mermaid.json
 voltaire/mermaid.py
 voltaire/pelican.py
 voltaire/search.py
 voltaire/tasks.py
 voltaire/wikilinks.py
 voltaire.egg-info/PKG-INFO
```

