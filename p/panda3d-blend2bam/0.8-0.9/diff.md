# Comparing `tmp/panda3d-blend2bam-0.8.tar.gz` & `tmp/panda3d-blend2bam-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panda3d-blend2bam-0.8.tar", last modified: Fri Sep 13 04:27:34 2019, max compression
+gzip compressed data, was "dist/panda3d-blend2bam-0.9.tar", last modified: Tue Sep 17 04:31:21 2019, max compression
```

## Comparing `panda3d-blend2bam-0.8.tar` & `panda3d-blend2bam-0.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4620 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1147 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2232 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/blender_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-09-13 04:26:12.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/.git
--rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptyNormal.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptyRoughness.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptySpecular.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)  1823737 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/YABEE_HowTo.odt
--rw-rw-r--   0 travis    (2000) travis    (2000)  1789001 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/YABEE_HowTo.pdf
--rw-rw-r--   0 travis    (2000) travis    (2000)    18793 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/empty.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/release.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)  6967092 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/Plant N120314.blend
--rw-rw-r--   0 travis    (2000) travis    (2000)  2789538 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/Plant N120314.egg.pz
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/
--rwxrwxr-x   0 travis    (2000) travis    (2000)   497736 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/leaves.blend
--rwxrwxr-x   0 travis    (2000) travis    (2000)    23969 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/leaves.egg
--rwxrwxr-x   0 travis    (2000) travis    (2000)    92508 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/mpm_vol.09_p25_leaf_2_front.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   472164 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/perFaceMaterials.blend
--rw-rw-r--   0 travis    (2000) travis    (2000)     5467 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/perFaceMaterials.egg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/
--rw-rw-r--   0 travis    (2000) travis    (2000)    92191 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_0.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    91434 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_1.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    91528 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_2.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   128914 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_3.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    49810 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_4.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    91700 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_5.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   566788 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.blend
--rw-rw-r--   0 travis    (2000) travis    (2000)     6467 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.egg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80261 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/egg_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37780 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/texture_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2172 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2947 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blender28_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2494 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blender_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.git
--rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.gitattributes
--rw-rw-r--   0 travis    (2000) travis    (2000)      827 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)    12997 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.pylintrc
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     6375 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20384 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18829 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/blendergltf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16223 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/animation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1044 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/camera.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9476 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4138 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12286 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/mesh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5792 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2014 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/scene.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2904 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/skin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4012 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/texture.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/
--rw-rw-r--   0 travis    (2000) travis    (2000)      581 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/_lights_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2143 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/blender_physics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_lights.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3541 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_unlit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14656 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_technique_webgl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10110 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/pbr_utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3178 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/utils/mesh.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6468 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3040 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.shape.schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/scene.BLENDER_physics.schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blend2gltf/gltfexts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      567 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/blenderutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6058 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/egg2bam/
--rw-rw-r--   0 travis    (2000) travis    (2000)      857 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/egg2bam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-09-13 04:26:14.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.git
--rw-rw-r--   0 travis    (2000) travis    (2000)     1203 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)    14435 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.pylintrc
--rw-rw-r--   0 travis    (2000) travis    (2000)      994 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3027 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51597 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/converter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      535 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/post.vert
--rw-rw-r--   0 travis    (2000) travis    (2000)     4390 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.frag
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.vert
--rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/tonemap.frag
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/viewer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      662 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      694 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9297 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/tests/test.gltf
--rw-rw-r--   0 travis    (2000) travis    (2000)      878 2019-09-13 04:26:15.000000 panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/tests/test_load.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      846 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/blend2bam/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4620 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5679 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      106 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2019-09-13 04:27:34.000000 panda3d-blend2bam-0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2019-09-13 04:26:10.000000 panda3d-blend2bam-0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      147 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4707 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3489 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1147 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2232 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/blender_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-09-17 04:29:55.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/.git
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptyNormal.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptyRoughness.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2800 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptySpecular.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      337 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1823737 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/YABEE_HowTo.odt
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1789001 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/YABEE_HowTo.pdf
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18793 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/empty.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/release.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  6967092 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/Plant N120314.blend
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2789538 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/Plant N120314.egg.pz
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)   497736 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/leaves.blend
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    23969 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/leaves.egg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    92508 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/mpm_vol.09_p25_leaf_2_front.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   472164 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/perFaceMaterials.blend
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5467 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/perFaceMaterials.egg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92191 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_0.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91434 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_1.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91528 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_2.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128914 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_3.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49810 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_4.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91700 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_5.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   566788 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.blend
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6467 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.egg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80261 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/egg_writer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37780 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/texture_processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2786 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2172 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3288 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blender28_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2767 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blender_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-09-17 04:29:57.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.git
+-rw-rw-r--   0 travis    (2000) travis    (2000)      419 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.gitattributes
+-rw-rw-r--   0 travis    (2000) travis    (2000)      827 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12997 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.pylintrc
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      805 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6375 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20384 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18829 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/blendergltf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16223 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/animation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1044 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/camera.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9476 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4138 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12286 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/mesh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5792 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/node.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2014 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/scene.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2904 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/skin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4012 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/texture.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      581 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/_lights_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2143 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/blender_physics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_lights.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3541 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      773 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_unlit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14656 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_technique_webgl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10110 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/pbr_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3178 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/utils/mesh.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6468 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3040 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.shape.schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/scene.BLENDER_physics.schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blend2gltf/gltfexts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/blenderutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6058 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      818 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/egg2bam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      867 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/egg2bam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1035 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.git
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1203 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14435 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.pylintrc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      994 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3027 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1155 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51597 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/converter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      535 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      263 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/post.vert
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4390 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.frag
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.vert
+-rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/tonemap.frag
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/viewer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      662 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      694 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9297 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/tests/test.gltf
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2019-09-17 04:29:58.000000 panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/tests/test_load.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      846 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/blend2bam/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4707 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5679 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      106 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2019-09-17 04:31:21.000000 panda3d-blend2bam-0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2019-09-17 04:29:53.000000 panda3d-blend2bam-0.9/setup.py
```

### Comparing `panda3d-blend2bam-0.8/LICENSE.txt` & `panda3d-blend2bam-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/PKG-INFO` & `panda3d-blend2bam-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-blend2bam
-Version: 0.8
+Version: 0.9
 Summary: A tool to convert Blender blend files to Panda3D BAM files
 Home-page: https://github.com/Moguri/panda3d-blend2bam
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/blend2bam.svg?branch=master)](https://travis-ci.org/Moguri/blend2bam)
         [![Python Versions](https://img.shields.io/pypi/pyversions/panda3d-blend2bam.svg)](https://pypi.org/project/panda3d-blend2bam/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.9%2C%201.10%2C%201.11-blue.svg)](https://www.panda3d.org/)
@@ -72,14 +72,15 @@
         |Skeletal Animations|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
         |Shape Keys|:x:|:heavy_check_mark:|:x:|
         |Shape Key Animations|:x:|:heavy_check_mark:|:x:|
         |CollisionSolids|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
         |Bullet Shapes|:heavy_check_mark:|:x:|:heavy_check_mark:|
         |Tags from Game Properties|:heavy_check_mark:|:heavy_check_mark:|:x:|
         |Tags from Custom Properties|:heavy_check_mark:|:x:|:heavy_check_mark:|
+        |Convert Particle Systems to Meshes|:heavy_check_mark:|:x:|:heavy_check_mark:|
         
         
         ## License
         
         [MIT](https://choosealicense.com/licenses/mit/)
         
 Keywords: panda3d gamedev
```

### Comparing `panda3d-blend2bam-0.8/README.md` & `panda3d-blend2bam-0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -65,12 +65,13 @@
 |Skeletal Animations|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
 |Shape Keys|:x:|:heavy_check_mark:|:x:|
 |Shape Key Animations|:x:|:heavy_check_mark:|:x:|
 |CollisionSolids|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
 |Bullet Shapes|:heavy_check_mark:|:x:|:heavy_check_mark:|
 |Tags from Game Properties|:heavy_check_mark:|:heavy_check_mark:|:x:|
 |Tags from Custom Properties|:heavy_check_mark:|:x:|:heavy_check_mark:|
+|Convert Particle Systems to Meshes|:heavy_check_mark:|:x:|:heavy_check_mark:|
 
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/blender_script.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/blender_script.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptyNormal.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptyNormal.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptyRoughness.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptyRoughness.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/EmptySpecular.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/EmptySpecular.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/LICENSE` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/LICENSE`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/YABEE_HowTo.odt` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/YABEE_HowTo.odt`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/YABEE_HowTo.pdf` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/YABEE_HowTo.pdf`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/empty.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/empty.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/release.txt` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/release.txt`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/Plant N120314.blend` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/Plant N120314.blend`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/Plant N120314.egg.pz` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/Plant N120314.egg.pz`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/leaves.blend` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/leaves.blend`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/leaves.egg` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/leaves.egg`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/leaves/mpm_vol.09_p25_leaf_2_front.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/leaves/mpm_vol.09_p25_leaf_2_front.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/perFaceMaterials.blend` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/perFaceMaterials.blend`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/perFaceMaterials.egg` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/perFaceMaterials.egg`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_0.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_0.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_1.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_1.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_2.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_2.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_3.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_3.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_4.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_4.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_5.png` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/SkyBox256_5.png`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.blend` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.blend`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.egg` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/test/skybox/skybox-cube.egg`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/egg_writer.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/egg_writer.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/texture_processor.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/texture_processor.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2egg/yabee/yabee_libs/utils.py` & `panda3d-blend2bam-0.9/blend2bam/blend2egg/yabee/yabee_libs/utils.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blender28_script.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blender28_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import json
 import os
 import sys
 
 import bpy #pylint: disable=import-error
 
+def make_particles_real():
+    for obj in bpy.data.objects[:]:
+        if hasattr(obj, 'particle_systems'):
+            print(f'Making particles on {obj.name} real')
+            obj.select_set(True)
+            bpy.ops.object.duplicates_make_real()
+
 def export_physics(gltf_data):
-    gltf_data['extensionsUsed'].append('BLENDER_physics')
+    gltf_data.setdefault('extensionsUsed', []).append('BLENDER_physics')
 
 
     objs = [
         (bpy.data.objects[gltf_node['name']], gltf_node)
         for gltf_node in gltf_data['nodes']
+        if gltf_node['name'] in bpy.data.objects
     ]
 
     objs = [
         i for i in objs
         if getattr(i[0], 'rigid_body')
     ]
 
@@ -49,14 +57,16 @@
 
 def export_gltf(_settings, src, dst):
     print('Converting .blend file ({}) to .gltf ({})'.format(src, dst))
 
     dstdir = os.path.dirname(dst)
     os.makedirs(dstdir, exist_ok=True)
 
+    make_particles_real()
+
     bpy.ops.export_scene.gltf(
         filepath=dst,
         export_format='GLTF_EMBEDDED',
         export_cameras=True,
         export_extras=True,
         export_yup=False,
         export_lights=True,
```

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blender_script.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blender_script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import json
 import os
 import sys
 
 import bpy #pylint: disable=import-error
 
+def make_particles_real():
+    for obj in bpy.data.objects[:]:
+        if hasattr(obj, 'particle_systems'):
+            print(f'Making particles on {obj.name} real')
+            obj.select = True
+            bpy.ops.object.duplicates_make_real()
 
 def export_gltf(settings, src, dst):
     print('Converting .blend file ({}) to .gltf ({})'.format(src, dst))
 
+    make_particles_real()
+
     # Lazy-load blendergltf
     scriptdir = os.path.dirname(__file__)
     sys.path.insert(0, os.path.join(scriptdir, 'blendergltf'))
     sys.path.insert(0, os.path.join(scriptdir))
     if 'blendergltf' in sys.modules:
         del sys.modules['blendergltf']
     from gltfexts import ExtMaterialsLegacy #pylint: disable=import-error
```

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.gitignore` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.gitignore`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/.pylintrc` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/.pylintrc`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/LICENSE` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/LICENSE`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/Makefile` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/Makefile`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/README.md` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/README.md`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/blendergltf.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/blendergltf.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/animation.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/animation.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/base.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/base.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/camera.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/camera.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/common.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/common.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/image.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/image.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/material.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/material.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/mesh.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/mesh.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/node.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/node.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/scene.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/scene.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/skin.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/skin.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/texture.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/exporters/texture.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/_lights_common.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/_lights_common.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/blender_physics.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/blender_physics.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_lights.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_lights.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_common.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_common.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_unlit.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_materials_unlit.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_technique_webgl.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/extension_exporters/khr_technique_webgl.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/filters.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/filters.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/pbr_utils.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/pbr_utils.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/blendergltf/utils/mesh.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/blendergltf/utils/mesh.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/README.md` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/README.md`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.schema.json` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.schema.json`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.shape.schema.json` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/blendergltf/extensions/BLENDER_physics/schema/node.BLENDER_physics.shape.schema.json`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/blend2gltf/gltfexts.py` & `panda3d-blend2bam-0.9/blend2bam/blend2gltf/gltfexts.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/cli.py` & `panda3d-blend2bam-0.9/blend2bam/cli.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/common.py` & `panda3d-blend2bam-0.9/blend2bam/common.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/egg2bam/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/egg2bam/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         stdout = subprocess.DEVNULL
         subprocess.check_call(args, stdout=stdout)
 
     def convert_batch(self, srcroot, dstdir, files):
         for outfile in files:
             src = outfile
-            dst = src.replace(srcroot, dstdir)
+            dst = src.replace(str(srcroot), str(dstdir))
 
             if self.settings.append_ext:
                 dst = dst.replace('.egg', '.blend.bam')
             else:
                 dst = dst.replace('.egg', '.bam')
 
             self.convert_single(src, dst)
```

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             skip_axis_conversion=True,
         )
         gltf.converter.convert(src, dst, settings)
 
     def convert_batch(self, srcroot, dstdir, files):
         for gltffile in files:
             src = gltffile
-            dst = src.replace(srcroot, dstdir)
+            dst = src.replace(str(srcroot), str(dstdir))
 
             if self.settings.append_ext:
                 dst = dst.replace('.gltf', '.blend.bam')
             else:
                 dst = dst.replace('.gltf', '.bam')
 
             self.convert_single(src, dst)
```

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.gitignore` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.gitignore`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.pylintrc` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.pylintrc`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/.travis.yml` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/.travis.yml`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/LICENSE.txt` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/README.md` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/README.md`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/__init__.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/__init__.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/cli.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/cli.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/converter.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/converter.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/loader.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/loader.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.frag` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.frag`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.vert` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/simplepbr.vert`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/gltf/viewer.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/gltf/viewer.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/setup.cfg` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/setup.cfg`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/setup.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/setup.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/tests/test.gltf` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/tests/test.gltf`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/gltf2bam/panda3d-gltf/tests/test_load.py` & `panda3d-blend2bam-0.9/blend2bam/gltf2bam/panda3d-gltf/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/blend2bam/loader.py` & `panda3d-blend2bam-0.9/blend2bam/loader.py`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/PKG-INFO` & `panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-blend2bam
-Version: 0.8
+Version: 0.9
 Summary: A tool to convert Blender blend files to Panda3D BAM files
 Home-page: https://github.com/Moguri/panda3d-blend2bam
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/blend2bam.svg?branch=master)](https://travis-ci.org/Moguri/blend2bam)
         [![Python Versions](https://img.shields.io/pypi/pyversions/panda3d-blend2bam.svg)](https://pypi.org/project/panda3d-blend2bam/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.9%2C%201.10%2C%201.11-blue.svg)](https://www.panda3d.org/)
@@ -72,14 +72,15 @@
         |Skeletal Animations|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
         |Shape Keys|:x:|:heavy_check_mark:|:x:|
         |Shape Key Animations|:x:|:heavy_check_mark:|:x:|
         |CollisionSolids|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
         |Bullet Shapes|:heavy_check_mark:|:x:|:heavy_check_mark:|
         |Tags from Game Properties|:heavy_check_mark:|:heavy_check_mark:|:x:|
         |Tags from Custom Properties|:heavy_check_mark:|:x:|:heavy_check_mark:|
+        |Convert Particle Systems to Meshes|:heavy_check_mark:|:x:|:heavy_check_mark:|
         
         
         ## License
         
         [MIT](https://choosealicense.com/licenses/mit/)
         
 Keywords: panda3d gamedev
```

### Comparing `panda3d-blend2bam-0.8/panda3d_blend2bam.egg-info/SOURCES.txt` & `panda3d-blend2bam-0.9/panda3d_blend2bam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda3d-blend2bam-0.8/setup.py` & `panda3d-blend2bam-0.9/setup.py`

 * *Files identical despite different names*

