# Comparing `tmp/dghs-imgutils-0.2.1.tar.gz` & `tmp/dghs-imgutils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.2.1.tar", last modified: Thu Jul  6 07:03:11 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.2.2.tar", last modified: Sat Jul 29 10:13:05 2023, max compression
```

## Comparing `dghs-imgutils-0.2.1.tar` & `dghs-imgutils-0.2.2.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 07:02:12.000000 dghs-imgutils-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-06 07:02:12.000000 dghs-imgutils-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-06 07:02:12.000000 dghs-imgutils-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-07-06 07:03:11.000000 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 07:03:11.000000 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:03:11.000000 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-06 07:03:11.000000 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 07:03:11.000000 dghs-imgutils-0.2.1/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/censor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.623241 dghs-imgutils-0.2.1/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/metrics/ccip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/imgutils/operate/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/align.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/censor_.py
--rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/emoji_censor.png
--rw-r--r--   0 runner    (1001) docker     (123)    83886 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/heart_censor.png
--rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/imgcensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    74310 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/smile_censor.png
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/operate/squeeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/nsfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:03:11.627241 dghs-imgutils-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-06 07:02:13.000000 dghs-imgutils-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 10:11:49.000000 dghs-imgutils-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-29 10:11:49.000000 dghs-imgutils-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-29 10:11:49.000000 dghs-imgutils-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-07-29 10:13:05.000000 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-29 10:13:05.000000 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:13:05.000000 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-29 10:13:05.000000 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 10:13:05.000000 dghs-imgutils-0.2.2/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/ascii/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/ascii/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.082549 dghs-imgutils-0.2.2/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83886 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74310 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/nsfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:13:05.086550 dghs-imgutils-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-29 10:11:51.000000 dghs-imgutils-0.2.2/setup.py
```

### Comparing `dghs-imgutils-0.2.1/LICENSE` & `dghs-imgutils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/PKG-INFO` & `dghs-imgutils-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.2.1
+Version: 0.2.2
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs-imgutils-0.2.1/README.md` & `dghs-imgutils-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.2.2/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.2.1
+Version: 0.2.2
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs-imgutils-0.2.1/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.2.2/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 setup.py
 dghs_imgutils.egg-info/PKG-INFO
 dghs_imgutils.egg-info/SOURCES.txt
 dghs_imgutils.egg-info/dependency_links.txt
 dghs_imgutils.egg-info/requires.txt
 dghs_imgutils.egg-info/top_level.txt
 imgutils/__init__.py
+imgutils/ascii/__init__.py
+imgutils/ascii/drawing.py
 imgutils/config/__init__.py
 imgutils/config/meta.py
 imgutils/data/__init__.py
 imgutils/data/background.py
 imgutils/data/decode.py
 imgutils/data/encode.py
 imgutils/data/image.py
 imgutils/data/layer.py
 imgutils/detect/__init__.py
 imgutils/detect/_yolo.py
 imgutils/detect/censor.py
 imgutils/detect/face.py
+imgutils/detect/hand.py
 imgutils/detect/head.py
 imgutils/detect/person.py
 imgutils/detect/visual.py
 imgutils/edge/__init__.py
 imgutils/edge/_base.py
 imgutils/edge/canny.py
 imgutils/edge/lineart.py
```

### Comparing `dghs-imgutils-0.2.1/dghs_imgutils.egg-info/requires.txt` & `dghs-imgutils-0.2.2/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/config/meta.py` & `dghs-imgutils-0.2.2/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.2.1'
+__VERSION__ = '0.2.2'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d'
```

### Comparing `dghs-imgutils-0.2.1/imgutils/data/background.py` & `dghs-imgutils-0.2.2/imgutils/data/background.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 import numpy as np
 from PIL import ImageColor, Image
 
 from .image import ImageTyping
+from .image import load_image
 from .layer import istack
 
 __all__ = [
     'grid_background',
     'grid_transparent',
 ]
 
@@ -58,9 +59,10 @@
         In this document, :func:`grid_transparent` is the default option used to
         accurately present the state of the generated image, as shown in the following figure
 
         .. image:: grid_transparent.plot.py.svg
            :align: center
 
     """
+    image = load_image(image, force_background=None)
     retval = grid_background(image.height, image.width, step, forecolor, backcolor)
     return istack(retval, image).convert('RGB')
```

### Comparing `dghs-imgutils-0.2.1/imgutils/data/decode.py` & `dghs-imgutils-0.2.2/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/data/encode.py` & `dghs-imgutils-0.2.2/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/data/image.py` & `dghs-imgutils-0.2.2/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/data/layer.py` & `dghs-imgutils-0.2.2/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/_yolo.py` & `dghs-imgutils-0.2.2/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/censor.py` & `dghs-imgutils-0.2.2/imgutils/detect/censor.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/face.py` & `dghs-imgutils-0.2.2/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/head.py` & `dghs-imgutils-0.2.2/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/person.py` & `dghs-imgutils-0.2.2/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/detect/visual.py` & `dghs-imgutils-0.2.2/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/edge/__init__.py` & `dghs-imgutils-0.2.2/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/edge/_base.py` & `dghs-imgutils-0.2.2/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/edge/canny.py` & `dghs-imgutils-0.2.2/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/edge/lineart.py` & `dghs-imgutils-0.2.2/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.2.2/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/metrics/aesthetic.py` & `dghs-imgutils-0.2.2/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/metrics/ccip.py` & `dghs-imgutils-0.2.2/imgutils/metrics/ccip.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/metrics/lpips.py` & `dghs-imgutils-0.2.2/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.2.2/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/align.py` & `dghs-imgutils-0.2.2/imgutils/operate/align.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/censor_.py` & `dghs-imgutils-0.2.2/imgutils/operate/censor_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/emoji_censor.png` & `dghs-imgutils-0.2.2/imgutils/operate/emoji_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/heart_censor.png` & `dghs-imgutils-0.2.2/imgutils/operate/heart_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/imgcensor.py` & `dghs-imgutils-0.2.2/imgutils/operate/imgcensor.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/smile_censor.png` & `dghs-imgutils-0.2.2/imgutils/operate/smile_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/operate/squeeze.py` & `dghs-imgutils-0.2.2/imgutils/operate/squeeze.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/segment/isnetis.py` & `dghs-imgutils-0.2.2/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.2.2/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/tagging/format.py` & `dghs-imgutils-0.2.2/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/tagging/mldanbooru.py` & `dghs-imgutils-0.2.2/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/tagging/wd14.py` & `dghs-imgutils-0.2.2/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.2.2/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/aicheck.py` & `dghs-imgutils-0.2.2/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/classify.py` & `dghs-imgutils-0.2.2/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/color.py` & `dghs-imgutils-0.2.2/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/monochrome.py` & `dghs-imgutils-0.2.2/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/nsfw.py` & `dghs-imgutils-0.2.2/imgutils/validate/nsfw.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/rating.py` & `dghs-imgutils-0.2.2/imgutils/validate/rating.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/imgutils/validate/truncate.py` & `dghs-imgutils-0.2.2/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.2.1/setup.py` & `dghs-imgutils-0.2.2/setup.py`

 * *Files identical despite different names*

