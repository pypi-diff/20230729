# Comparing `tmp/oneat-6.1.6.tar.gz` & `tmp/oneat-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.1.6.tar", last modified: Sat Jul 29 12:52:03 2023, max compression
+gzip compressed data, was "oneat-6.1.7.tar", last modified: Sat Jul 29 13:23:18 2023, max compression
```

## Comparing `oneat-6.1.6.tar` & `oneat-6.1.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.987565 oneat-6.1.6/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.6/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.6/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.963820 oneat-6.1.6/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.966838 oneat-6.1.6/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.6/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.967726 oneat-6.1.6/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.967995 oneat-6.1.6/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.6/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.6/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.6/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.6/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.6/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 12:52:03.987664 oneat-6.1.6/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.6/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.972593 oneat-6.1.6/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.6/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.6/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.6/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.973969 oneat-6.1.6/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.6/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.6/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-29 12:52:03.988051 oneat-6.1.6/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.964276 oneat-6.1.6/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.974733 oneat-6.1.6/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.978829 oneat-6.1.6/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.1.6/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38288 2023-07-29 12:38:35.000000 oneat-6.1.6/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.981224 oneat-6.1.6/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24144 2023-07-29 12:49:23.000000 oneat-6.1.6/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.6/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      603 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.982101 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.982977 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.983377 oneat-6.1.6/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.987326 oneat-6.1.6/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.6/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 12:52:03.975525 oneat-6.1.6/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-29 12:52:03.000000 oneat-6.1.6/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.6/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.036756 oneat-6.1.7/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.7/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.7/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.010333 oneat-6.1.7/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.013137 oneat-6.1.7/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.7/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.014304 oneat-6.1.7/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.014453 oneat-6.1.7/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.7/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.7/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.7/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.7/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:23:18.036847 oneat-6.1.7/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.7/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.019160 oneat-6.1.7/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.7/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.7/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.7/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.020570 oneat-6.1.7/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.7/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.7/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-29 13:23:18.037238 oneat-6.1.7/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.010775 oneat-6.1.7/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.021337 oneat-6.1.7/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.025335 oneat-6.1.7/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.1.7/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38288 2023-07-29 12:38:35.000000 oneat-6.1.7/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.027238 oneat-6.1.7/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.1.7/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.7/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.1.7/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.1.7/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.028263 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.029152 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.029518 oneat-6.1.7/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.035839 oneat-6.1.7/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.7/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:23:18.022154 oneat-6.1.7/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-29 13:23:18.000000 oneat-6.1.7/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-29 13:23:17.000000 oneat-6.1.7/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.7/tox.ini
```

### Comparing `oneat-6.1.6/.DS_Store` & `oneat-6.1.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/.github/workflows/test_and_deploy.yml` & `oneat-6.1.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/.gitignore` & `oneat-6.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/.pre-commit-config.yaml` & `oneat-6.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/LICENSE` & `oneat-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/PKG-INFO` & `oneat-6.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.6
+Version: 6.1.7
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.6/README.md` & `oneat-6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/Xenopus_example.jpg` & `oneat-6.1.7/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/Xenopus_example.png` & `oneat-6.1.7/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_0_crop.png` & `oneat-6.1.7/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_1_crop.png` & `oneat-6.1.7/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_2_crop.png` & `oneat-6.1.7/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_3_crop.png` & `oneat-6.1.7/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_4_crop.png` & `oneat-6.1.7/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/images/ch_5_crop.png` & `oneat-6.1.7/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/Apache-2` & `oneat-6.1.7/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/BSD-3` & `oneat-6.1.7/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/GPL-3` & `oneat-6.1.7/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/LGPL-3` & `oneat-6.1.7/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/MIT` & `oneat-6.1.7/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/licenses/MPL-2` & `oneat-6.1.7/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/setup.cfg` & `oneat-6.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.1.7/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.1.7/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.1.7/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.1.7/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/__init__.py` & `oneat-6.1.7/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/config.py` & `oneat-6.1.7/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.1.7/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/loss.py` & `oneat-6.1.7/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_focus.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.1.7/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATModels/nets.py` & `oneat-6.1.7/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.1.7/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 import glob
 import json
 import os
 from pathlib import Path
 import numpy as np
 import pandas as pd
 import napari
-
-
 from scipy import spatial
 
 
-
 class NEATViz:
     def __init__(
         self,
         imagedir: str,
         csvdir: str,
         savedir: str,
         categories_json: dict,
```

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.1.7/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/NMS.py` & `oneat-6.1.7/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.1.7/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.1.7/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from pathlib import Path
-import json
-from oneat.NEATUtils.oneat_animation._qt import OneatVisualizeWidget
-import napari
-from qtpy.QtCore import Qt
+
 
 class VizDet:
     
         
         
     def __init__(self):
         
+        from oneat.NEATUtils.oneat_animation._qt import OneatVisualizeWidget
+        import napari
+        from qtpy.QtCore import Qt
         self.viewer = napari.Viewer()
         self.viz_widget = OneatVisualizeWidget(self.viewer)
         
         dock_widget = self.viewer.window.add_dock_widget(
             self.viz_widget, area="right"
         )
         self.viewer.window._qt_window.resizeDocks(
```

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.1.7/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.1.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/plotters.py` & `oneat-6.1.7/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/NEATUtils/utils.py` & `oneat-6.1.7/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/__init__.py` & `oneat-6.1.7/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/_tests/test_nets.py` & `oneat-6.1.7/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/_tests/utils.py` & `oneat-6.1.7/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.1.7/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/_tests/variables/variables.index` & `oneat-6.1.7/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat/pretrained.py` & `oneat-6.1.7/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/src/oneat.egg-info/PKG-INFO` & `oneat-6.1.7/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.6
+Version: 6.1.7
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.6/src/oneat.egg-info/SOURCES.txt` & `oneat-6.1.7/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.1.6/tox.ini` & `oneat-6.1.7/tox.ini`

 * *Files identical despite different names*

