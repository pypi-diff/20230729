# Comparing `tmp/oneat-6.1.9.tar.gz` & `tmp/oneat-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.1.9.tar", last modified: Sat Jul 29 13:37:31 2023, max compression
+gzip compressed data, was "oneat-6.2.0.tar", last modified: Sat Jul 29 13:41:43 2023, max compression
```

## Comparing `oneat-6.1.9.tar` & `oneat-6.2.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.324818 oneat-6.1.9/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.1.9/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.1.9/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.301457 oneat-6.1.9/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.304171 oneat-6.1.9/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.1.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.1.9/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.305406 oneat-6.1.9/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.305555 oneat-6.1.9/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.1.9/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.1.9/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.1.9/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.9/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.1.9/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:37:31.324912 oneat-6.1.9/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.1.9/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.310449 oneat-6.1.9/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.1.9/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.1.9/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.1.9/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.311973 oneat-6.1.9/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.1.9/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.1.9/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-29 13:37:31.325296 oneat-6.1.9/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.301897 oneat-6.1.9/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.312657 oneat-6.1.9/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.316191 oneat-6.1.9/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.1.9/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38493 2023-07-29 13:36:58.000000 oneat-6.1.9/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.318340 oneat-6.1.9/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.1.9/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.1.9/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.1.9/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.1.9/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.319174 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.320005 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70763 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.320399 oneat-6.1.9/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.324582 oneat-6.1.9/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.1.9/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:37:31.313487 oneat-6.1.9/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-29 13:37:31.000000 oneat-6.1.9/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.1.9/tox.ini
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.456904 oneat-6.2.0/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.2.0/.DS_Store
+-rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.2.0/.gitattributes
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.430965 oneat-6.2.0/.github/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.434016 oneat-6.2.0/.github/workflows/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.2.0/.gitignore
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.435099 oneat-6.2.0/.idea/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/.gitignore
+-rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/Yoloneat.iml
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.435253 oneat-6.2.0/.idea/inspectionProfiles/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/misc.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/modules.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/other.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.2.0/.idea/vcs.xml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.2.0/1
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.0/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.2.0/MANIFEST.in
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:41:43.456997 oneat-6.2.0/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.2.0/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.440044 oneat-6.2.0/images/
+-rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.2.0/images/Xenopus_example.jpg
+-rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.2.0/images/Xenopus_example.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_0_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_1_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_2_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_3_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_4_crop.png
+-rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.2.0/images/ch_5_crop.png
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.441445 oneat-6.2.0/licenses/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/Apache-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/BSD-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/GPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/LGPL-3
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/MIT
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.2.0/licenses/MPL-2
+-rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-21 10:27:28.000000 oneat-6.2.0/pyproject.toml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-29 13:41:43.457377 oneat-6.2.0/setup.cfg
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.431412 oneat-6.2.0/src/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.442229 oneat-6.2.0/src/oneat/
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.446313 oneat-6.2.0/src/oneat/NEATModels/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/.neat_focus.py.swp
+-rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/MidogConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/Staticconfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/TrainConfig.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/config.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/gen_anchors.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.2.0/src/oneat/NEATModels/loss.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38493 2023-07-29 13:36:58.000000 oneat-6.2.0/src/oneat/NEATModels/neat_densevollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_focus.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_focus_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_lstm.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_microscope.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_static_resnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/neat_vollnet.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATModels/nets.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.448541 oneat-6.2.0/src/oneat/NEATUtils/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    24141 2023-07-29 13:19:14.000000 oneat-6.2.0/src/oneat/NEATUtils/HolovizNapari.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.2.0/src/oneat/NEATUtils/MovieCreator.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/NMS.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/TrainDataMaker.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.2.0/src/oneat/NEATUtils/VisualizeDetections.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/Zmapgen.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.2.0/src/oneat/NEATUtils/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.449742 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    21222 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.450572 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2867 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6471 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/NEATUtils/plotters.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    70764 2023-07-29 13:41:03.000000 oneat-6.2.0/src/oneat/NEATUtils/utils.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/__init__.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.450986 oneat-6.2.0/src/oneat/_tests/
+-rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/_tests/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/_tests/test_nets.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/_tests/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.456677 oneat-6.2.0/src/oneat/_tests/variables/
+-rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/_tests/variables/variables.index
+-rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/caped.yaml
+-rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.2.0/src/oneat/pretrained.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 13:41:43.442972 oneat-6.2.0/src/oneat.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-29 13:41:43.000000 oneat-6.2.0/src/oneat.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.2.0/tox.ini
```

### Comparing `oneat-6.1.9/.DS_Store` & `oneat-6.2.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/.github/workflows/test_and_deploy.yml` & `oneat-6.2.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/.gitignore` & `oneat-6.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/.pre-commit-config.yaml` & `oneat-6.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/LICENSE` & `oneat-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/PKG-INFO` & `oneat-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.9
+Version: 6.2.0
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.9/README.md` & `oneat-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/Xenopus_example.jpg` & `oneat-6.2.0/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/Xenopus_example.png` & `oneat-6.2.0/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_0_crop.png` & `oneat-6.2.0/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_1_crop.png` & `oneat-6.2.0/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_2_crop.png` & `oneat-6.2.0/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_3_crop.png` & `oneat-6.2.0/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_4_crop.png` & `oneat-6.2.0/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/images/ch_5_crop.png` & `oneat-6.2.0/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/Apache-2` & `oneat-6.2.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/BSD-3` & `oneat-6.2.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/GPL-3` & `oneat-6.2.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/LGPL-3` & `oneat-6.2.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/MIT` & `oneat-6.2.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/licenses/MPL-2` & `oneat-6.2.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/setup.cfg` & `oneat-6.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.2.0/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.2.0/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.2.0/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.2.0/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/__init__.py` & `oneat-6.2.0/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/config.py` & `oneat-6.2.0/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.2.0/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/loss.py` & `oneat-6.2.0/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_focus.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.2.0/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATModels/nets.py` & `oneat-6.2.0/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.2.0/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.2.0/src/oneat/NEATUtils/MovieCreator.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/NMS.py` & `oneat-6.2.0/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.2.0/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.2.0/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.2.0/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.2.0/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/plotters.py` & `oneat-6.2.0/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/NEATUtils/utils.py` & `oneat-6.2.0/src/oneat/NEATUtils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1611,15 +1611,15 @@
                     confidences,
                 ]
             )
             event_count = sorted(
                 event_count, key=lambda x: x[0], reverse=False
             )
             event_data = []
-            csvname = savedir + "/" + f"pred_{event_name}_locations"
+            csvname = Path(savedir) /  f"pred_{event_name}_locations"
 
             writer = csv.writer(open(csvname + ".csv", "a", newline=""))
             filesize = os.stat(csvname + ".csv").st_size
 
             if filesize < 1:
                 writer.writerow(
                     ["T", "Z", "Y", "X", "Score", "Size", "Confidence"]
```

### Comparing `oneat-6.1.9/src/oneat/__init__.py` & `oneat-6.2.0/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/_tests/test_nets.py` & `oneat-6.2.0/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/_tests/utils.py` & `oneat-6.2.0/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.2.0/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/_tests/variables/variables.index` & `oneat-6.2.0/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat/pretrained.py` & `oneat-6.2.0/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/src/oneat.egg-info/PKG-INFO` & `oneat-6.2.0/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.1.9
+Version: 6.2.0
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.1.9/src/oneat.egg-info/SOURCES.txt` & `oneat-6.2.0/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.1.9/tox.ini` & `oneat-6.2.0/tox.ini`

 * *Files identical despite different names*

