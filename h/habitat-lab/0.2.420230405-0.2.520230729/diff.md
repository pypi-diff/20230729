# Comparing `tmp/habitat-lab-0.2.420230405.tar.gz` & `tmp/habitat-lab-0.2.520230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habitat-lab-0.2.420230405.tar", last modified: Wed Apr  5 18:53:23 2023, max compression
+gzip compressed data, was "habitat-lab-0.2.520230729.tar", last modified: Sat Jul 29 05:48:26 2023, max compression
```

## Comparing `habitat-lab-0.2.420230405.tar` & `habitat-lab-0.2.520230729.tar`

### file list

```diff
@@ -1,319 +1,330 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      210 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/PKG-INFO
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.438212 habitat-lab-0.2.420230405/habitat/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      887 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.438212 habitat-lab-0.2.420230405/habitat/articulated_agent_controllers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agent_controllers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9687 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.438212 habitat-lab-0.2.420230405/habitat/articulated_agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      968 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10558 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/articulated_agent_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3007 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/articulated_agent_interface.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.438212 habitat-lab-0.2.420230405/habitat/articulated_agents/humanoids/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      341 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/humanoids/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5425 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/humanoids/kinematic_humanoid.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18684 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/manipulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6693 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/mobile_manipulator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      634 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4655 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/fetch_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/fetch_suction.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1372 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/franka_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7298 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/spot_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/robots/stretch_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3802 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/articulated_agents/static_manipulator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19900 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/CONFIG_KEYS.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16883 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      384 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.434212 habitat-lab-0.2.420230405/habitat/config/benchmark/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/eqa_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      435 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/eqa_rgbonly_mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/imagenav/imagenav_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      355 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/imagenav/imagenav_gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      353 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/imagenav/imagenav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/imagenav/imagenav_test.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/instance_imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      840 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      840 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.442213 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      537 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      354 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      360 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_habitat_test.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/nav/vln_r2r.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/close_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      954 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/close_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1350 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/idle.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1116 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/idle_single_camera.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1353 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/interact.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      939 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/nav_to_obj.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/open_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      951 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/open_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      950 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/pick.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1407 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/pick_spa.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/place.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      976 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1189 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_human.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2115 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_spot.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1605 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_stretch.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      802 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/reach_state.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1011 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1746 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4838 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/default.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71761 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/default_structured_configs.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.434212 habitat-lab-0.2.420230405/habitat/config/habitat/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.434212 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      223 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/eqa/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/imagenav/gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/imagenav/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/instance_imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/instance_imagenav/hm3d_v1.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/instance_imagenav/hm3d_v2.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/objectnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/objectnav/hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/objectnav/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/gibson_0_plus.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/gibson_v2.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/habitat_test.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/pointnav/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/rearrangement/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/rearrangement/replica_cad.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.446213 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      225 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/dataset/vln/mp3d_r2r.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.434212 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.450213 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      148 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/depth_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      163 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/depth_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      249 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/depth_head_agent_vis.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      142 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgb_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgb_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      217 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbd_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbd_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbd_head_rgbd_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbd_head_rgbdp_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbdp_head_rgbd_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      298 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/rgbds_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/simulator/agents/semantic_agent.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.450213 habitat-lab-0.2.420230405/habitat/config/habitat/task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      255 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/eqa.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      392 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/imagenav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      676 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/instance_imagenav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/objectnav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      415 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/pointnav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/pointnav_franka.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      960 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/close_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/close_fridge.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/demo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      246 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/demo/idle.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      314 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/demo/interact.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      900 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/nav_to_obj.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1205 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/open_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1243 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/open_fridge.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2185 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      442 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      583 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3503 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      992 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pick.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1186 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pick_spa.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1079 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/place.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/play.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/play_human.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      672 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/reach_state.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1245 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1223 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1727 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1160 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1076 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/habitat/task/vln_r2r.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1070 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/config/read_write.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/core/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1221 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/agent.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5737 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/benchmark.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      654 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/challenge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19851 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13010 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/embodied_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16056 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/env.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3826 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/environments.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7888 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/registry.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12984 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/simulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/spaces.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5604 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22589 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/core/vector_env.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      733 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/eqa/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3974 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/eqa/mp3d_eqa_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/image_nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1263 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/image_nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3100 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/image_nav/instance_image_nav_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/object_nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/object_nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5664 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/object_nav/object_nav_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1220 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/pointnav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5609 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/pointnav/pointnav_dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7361 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/pointnav/pointnav_generator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.518218 habitat-lab-0.2.420230405/habitat/datasets/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1232 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/combine_datasets.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4250 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/all_receptacles.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3171 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/bench_config.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2132 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/empty.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6455 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5721 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4326 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4605 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2831 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2504 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/in_drawer.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/in_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2369 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/test_config.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1077 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/generate_episode_inits.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/rearrange_dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40651 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/rearrange_generator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16218 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/run_episode_generator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      756 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9654 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/art_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18567 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/object_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3987 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/object_target_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32875 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/receptacle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1154 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/scene_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/datasets/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/vln/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2482 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/datasets/vln/r2r_vln_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/gym/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/gym/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4726 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/gym/gym_definitions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1887 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/gym/gym_env_episode_count_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1591 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/gym/gym_env_obs_dict_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12439 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/gym/gym_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/py.typed
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/sims/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      267 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      956 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7101 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20974 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/debug_visualizer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23617 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/habitat_simulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12467 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/sim_utilities.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/sims/pyrobot/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      785 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/pyrobot/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8884 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/pyrobot/pyrobot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      721 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/sims/registration.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.522218 habitat-lab-0.2.420230405/habitat/tasks/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/eqa/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6173 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/eqa/eqa.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      670 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/nav/instance_image_nav_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46442 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/nav/nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6714 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/nav/object_nav_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3276 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/nav/shortest_path_follower.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2777 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28871 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1723 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/articulated_agent_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11263 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/grip_actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9146 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/oracle_nav_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3678 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/pddl_actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6687 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/articulated_agent_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1541 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/marker_info.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9357 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/composite_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2465 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/composite_task.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.526219 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/domain_configs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9792 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9099 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25049 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3155 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3817 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_predicate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16969 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_sim_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7080 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/rearrange_pddl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2825 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/task_creator_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/policy_modules.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13287 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_grasp_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31880 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33516 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_sim.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12281 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_task.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12483 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9450 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8684 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5010 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6178 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/pick_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3542 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/pick_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5563 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/place_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1329 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/place_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3982 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/reach_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/reach_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15377 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/rearrange/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      875 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1723 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat/tasks/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/vln/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/tasks/vln/vln.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2477 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1121 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/env_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5446 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/geometry_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/pickle5_multiprocessing.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2096 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/profiling_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1082 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/test_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat/utils/visualizations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      288 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/visualizations/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.438212 habitat-lab-0.2.420230405/habitat/utils/visualizations/assets/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5616 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4240 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/visualizations/fog_of_war.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15090 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/visualizations/maps.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11969 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/utils/visualizations/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/habitat/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/habitat_lab.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-04-05 18:53:23.000000 habitat-lab-0.2.420230405/habitat_lab.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12079 2023-04-05 18:53:23.000000 habitat-lab-0.2.420230405/habitat_lab.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 18:53:23.000000 habitat-lab-0.2.420230405/habitat_lab.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      253 2023-04-05 18:53:23.000000 habitat-lab-0.2.420230405/habitat_lab.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2023-04-05 18:53:23.000000 habitat-lab-0.2.420230405/habitat_lab.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      338 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-04-05 18:53:23.558221 habitat-lab-0.2.420230405/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4530 2023-04-05 18:52:58.000000 habitat-lab-0.2.420230405/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      210 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/PKG-INFO
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      887 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9687 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      968 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10558 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3007 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_interface.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      341 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5425 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/kinematic_humanoid.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18684 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/manipulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6693 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/mobile_manipulator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      634 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4655 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_suction.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1372 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/franka_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7298 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/spot_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/stretch_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3802 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/static_manipulator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20023 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/CONFIG_KEYS.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16816 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      384 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/benchmark/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      435 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_rgbonly_mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      355 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      353 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_test.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      773 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      904 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      774 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      926 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      754 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      537 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      354 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      360 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_habitat_test.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/vln_r2r.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      954 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1350 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1116 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle_single_camera.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1353 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/interact.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      939 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/nav_to_obj.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      951 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      950 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/pick.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/place.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      976 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1189 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_human.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2115 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_spot.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1605 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_stretch.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      802 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/reach_state.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1011 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1746 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4838 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/default.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74397 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/default_structured_configs.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      223 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/eqa/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/hm3d_v1.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/hm3d_v2.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/hssd-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/procthor-hab.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson_0_plus.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson_v2.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/habitat_test.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/rearrangement/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/rearrangement/replica_cad.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      225 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/vln/mp3d_r2r.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.150841 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      148 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      163 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      249 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_head_agent_vis.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      142 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgb_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgb_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      217 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_rgbd_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_rgbdp_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbdp_head_rgbd_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      298 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbds_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/semantic_agent.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.150841 habitat-lab-0.2.520230729/habitat/config/habitat/task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      255 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/eqa.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      392 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/imagenav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      748 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/instance_imagenav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      648 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/objectnav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      415 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/pointnav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/pointnav_franka.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      147 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/fetch_arm.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/fetch_base_arm.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      960 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_fridge.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      246 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/idle.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      314 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/interact.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      900 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/nav_to_obj.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1243 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_fridge.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2185 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      442 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      583 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3503 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      916 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pick.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1003 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/place.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play_human.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      672 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/reach_state.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1245 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1223 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1727 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1160 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1076 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/vln_r2r.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1070 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/read_write.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/core/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1221 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/agent.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/core/batch_rendering/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18384 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/env_batch_renderer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      330 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/env_batch_renderer_constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5737 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/benchmark.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      654 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/challenge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19851 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13582 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/embodied_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16056 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/env.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3978 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/environments.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7153 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/registry.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13195 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/simulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/spaces.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5604 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23512 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/vector_env.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/datasets/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/datasets/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      733 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/eqa/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3974 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/eqa/mp3d_eqa_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/image_nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/image_nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3100 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/image_nav/instance_image_nav_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/object_nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/object_nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5664 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/object_nav/object_nav_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1220 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7361 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_generator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/combine_datasets.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4250 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/all_receptacles.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/bench_config.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2132 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/empty.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6455 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5721 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4326 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4605 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2831 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2504 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_drawer.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2369 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/test_config.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1077 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/generate_episode_inits.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3450 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43253 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_generator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16486 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/run_episode_generator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      756 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9654 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/art_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23653 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3987 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_target_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/receptacle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1154 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/scene_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/vln/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2482 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/vln/r2r_vln_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/gym/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4757 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_definitions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1887 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_env_episode_count_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1591 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_env_obs_dict_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12898 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/py.typed
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/sims/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      267 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      711 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2517 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20974 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/debug_visualizer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26504 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/habitat_simulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12514 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/sim_utilities.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/sims/pyrobot/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      785 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/pyrobot/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8884 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/pyrobot/pyrobot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      721 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/registration.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/eqa/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6173 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/eqa/eqa.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      670 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/instance_image_nav_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46959 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6714 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/object_nav_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3276 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/shortest_path_follower.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1400 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27870 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1722 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/articulated_agent_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/grip_actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8828 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/oracle_nav_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/pddl_actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7368 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/articulated_agent_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1541 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/marker_info.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9441 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2465 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_task.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9792 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9255 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26009 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4432 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4749 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_predicate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19506 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_sim_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7259 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/rearrange_pddl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2825 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/task_creator_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/policy_modules.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13238 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_grasp_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32786 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37631 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sim.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13425 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_task.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12483 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9450 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9023 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5200 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6174 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3794 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5547 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1329 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3982 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17755 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      875 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1723 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/vln/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/vln/vln.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2477 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1244 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/env_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5446 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/geometry_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/pickle5_multiprocessing.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2096 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/profiling_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1082 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/test_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat/utils/visualizations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      288 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5616 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/fog_of_war.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15090 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/maps.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11969 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat_lab.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12658 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      253 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      338 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/requirements.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4530 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/setup.py
```

### Comparing `habitat-lab-0.2.420230405/PKG-INFO` & `habitat-lab-0.2.520230729/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-lab
-Version: 0.2.420230405
+Version: 0.2.520230729
 Summary: Habitat-Lab: a modular high-level library for end-to-end development in Embodied AI.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-lab-0.2.420230405/habitat/__init__.py` & `habitat-lab-0.2.520230729/habitat/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py` & `habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/__init__.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/articulated_agent_base.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_base.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/articulated_agent_interface.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_interface.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/humanoids/kinematic_humanoid.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/kinematic_humanoid.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/manipulator.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/mobile_manipulator.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/mobile_manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/__init__.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/fetch_robot.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/fetch_suction.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_suction.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/franka_robot.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/franka_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/spot_robot.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/spot_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/robots/stretch_robot.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/stretch_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/articulated_agents/static_manipulator.py` & `habitat-lab-0.2.520230729/habitat/articulated_agents/static_manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/CONFIG_KEYS.md` & `habitat-lab-0.2.520230729/habitat/config/CONFIG_KEYS.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
  - Rearrangement reach : `RearrangeReachTask-v0` The agent must place its end effector into a specific location defined by geometric coordinates.
  - Rearrangement composite tasks : `RearrangeCompositeTask-v0` The agent must perform a sequence of sub-tasks in succession defined by a PDDL plan.
 
 
 | Key | Description |
 | --- | --- |
 |habitat.task.type | The registered task that will be used. For example : `InstanceImageNav-v1` or `ObjectNav-v1`.
+|habitat.task.physics_target_sps |  The size of each simulator physics update will be 1 / physics_target_sps. |
 |habitat.task.reward_measure | The name of the Measurement that will correspond to the reward of the robot. This value must be a key present in the dictionary of Measurements in the habitat configuration (under `habitat.task.measurements`, see below for a list of available measurements). For example, `distance_to_goal_reward` for navigation or `place_reward` for the rearrangement place task.|
 |habitat.task.success_measure | The name of the Measurement that will correspond to the success criteria of the robot. This value must be a key present in the dictionary of Measurements in the habitat configuration (under `habitat.task.measurements`, see below for a list of available measurements). If the measurement has a non-zero value, the episode is considered a success. |
 |habitat.task.end_on_success | If True, the episode will end when the success measure indicates success. Otherwise the episode will go on (this is useful when doing hierarchical learning and the robot has to explicitly decide when to change policies)|
 |habitat.task.task_spec |  When doing the `RearrangeCompositeTask-v0` only, will look for a pddl plan of that name to determine the sequence of sub-tasks that need to be completed. The format of the pddl plans files is undocumented.|
 |habitat.task.task_spec_base_path |  When doing the `RearrangeCompositeTask-v0` only, the relative path where the task_spec file will be searched.|
 |habitat.task.spawn_max_dists_to_obj| For `RearrangePickTask-v0` task only. Controls the maximum distance the robot can be spawned from the target object. |
 | habitat.task.base_angle_noise| For Rearrangement tasks only. Controls the standard deviation of the random normal noise applied to the base's rotation angle at the start of an episode.|
@@ -80,16 +81,16 @@
 | Key | Description |
 | --- | --- |
 | habitat.task.actions.stop |     In Navigation tasks only, the stop action is a discrete action. When called, the Agent will request to stop the navigation task. Note that this action is needed to succeed in a Navigation task since the Success is determined by the Agent calling the stop action within range of the target. Note that this is different from the RearrangeStopActionConfig that works for Rearrangement tasks only instead of the Navigation tasks.|
 | habitat.task.actions.empty | In Navigation tasks only, the pass action. The robot will do nothing.|
 | habitat.task.actions.move_forward |     In Navigation tasks only, this discrete action will move the robot forward by a fixed amount determined by the `habitat.simulator.forward_step_size` amount. |
 | habitat.task.actions.turn_left |     In Navigation tasks only, this discrete action will rotate the robot to the left  by a fixed amount determined by the `habitat.simulator.turn_angle` amount. |
 | habitat.task.actions.turn_right |     In Navigation tasks only, this discrete action will rotate the robot to the right by a fixed amount determined by the `habitat.simulator.turn_angle` amount. |
-| habitat.task.actions.look_up |      In Navigation tasks only, this discrete action will rotate the robot's camera up by a fixed amount determined by the `habitat.simulator.tilt_angle` amount. |
-| habitat.task.actions.look_down |      In Navigation tasks only, this discrete action will rotate the robot's camera down by a fixed amount determined by the `habitat.simulator.tilt_angle` amount. |
+| habitat.task.actions.look_up |      In Navigation tasks only, this discrete action will rotate the robot's camera up by a fixed amount determined by the `tilt_angle` amount of the look_up action. |
+| habitat.task.actions.look_down |      In Navigation tasks only, this discrete action will rotate the robot's camera down by a fixed amount determined by the `tilt_angle` amount  of the look_down action. |
 
 ## Navigation Measures
 A measure is a way to collect data about the environment at each step that is not sensor information. Measures can contain privileged information for the user (like a top down map) or for training (like rewards).
 The way one would add a measure to a configuration file would be by adding to the `defaults` list. For example:
 ```
 defaults:
   - /habitat/task/measurements:
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/README.md` & `habitat-lab-0.2.520230729/habitat/config/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,31 +115,28 @@
       group_by_scene: true
       num_episode_sample: -1
       max_scene_repeat_episodes: -1
       max_scene_repeat_steps: 10000
       step_repetition_range: 0.2
   simulator:
     type: Sim-v0
-    action_space_config: v0
-    action_space_config_arguments: {}
     forward_step_size: 0.25
+    turn_angle: 10
     create_renderer: false
     requires_textures: true
     lag_observations: 0
     auto_sleep: false
     step_physics: true
     concur_render: false
     needs_markers: true
     update_articulated_agent: true
     scene: data/scene_datasets/habitat-test-scenes/van-gogh-room.glb
     scene_dataset: default
     additional_object_paths: []
     seed: ${habitat.seed}
-    turn_angle: 10
-    tilt_angle: 15
     default_agent_id: 0
     debug_render: false
     debug_render_robot: false
     kinematic_mode: false
     debug_render_goal: true
     robot_joint_start_noise: 0.0
     ctrl_freq: 120.0
@@ -262,24 +259,25 @@
     should_enforce_target_within_reach: false
     task_spec_base_path: habitat/task/rearrange/pddl/
     task_spec: ''
     pddl_domain_def: replica_cad
     obj_succ_thresh: 0.3
     art_succ_thresh: 0.15
     robot_at_thresh: 2.0
-    filter_nav_to_tasks: []
     actions:
       stop:
         type: StopAction
       move_forward:
         type: MoveForwardAction
       turn_left:
         type: TurnLeftAction
+        turn_angle: 10
       turn_right:
         type: TurnRightAction
+        turn_angle: 10
   dataset:
     type: PointNav-v1
     split: train
     scenes_dir: data/scene_datasets
     content_scenes:
     - '*'
     data_path: data/datasets/pointnav/gibson/v1/{split}/{split}.json.gz
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/eqa_mp3d.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_mp3d.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,14 @@
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 1000
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: v1
     agents:
       main_agent:
         sim_sensors:
           rgb_sensor:
             width: 640
             height: 480
             hfov: 79
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,14 @@
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 1000
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: v1
     agents:
       main_agent:
         sim_sensors:
           rgb_sensor:
             width: 360
             height: 640
             hfov: 42
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # @package _global_
 
 defaults:
   - /habitat: habitat_config_base
   - /habitat/task: objectnav
   - /habitat/simulator/agents@habitat.simulator.agents.main_agent: rgbd_agent
-  - /habitat/dataset/objectnav: hm3d
+  - /habitat/dataset/objectnav: mp3d
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 500
 
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: "v1"
     agents:
       main_agent:
         sim_sensors:
           rgb_sensor:
             width: 640
             height: 480
             hfov: 79
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,16 @@
   - /habitat/simulator/agents@habitat.simulator.agents.main_agent: semantic_agent
   - /habitat/dataset/objectnav: hm3d
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 500
-
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: "v1"
     agents:
       main_agent:
         sim_sensors:
           semantic_sensor:
             width: 640
             height: 480
             hfov: 79
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # @package _global_
 
 defaults:
   - /habitat: habitat_config_base
   - /habitat/task: objectnav
   - /habitat/simulator/agents@habitat.simulator.agents.main_agent: rgbd_agent
-  - /habitat/dataset/objectnav: mp3d
+  - /habitat/dataset/objectnav: hm3d
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 500
-
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: "v1"
     agents:
       main_agent:
         sim_sensors:
           rgb_sensor:
             width: 640
             height: 480
             hfov: 79
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,16 @@
   - /habitat/simulator/agents@habitat.simulator.agents.main_agent: semantic_agent
   - /habitat/dataset/objectnav: mp3d
   - _self_
 
 habitat:
   environment:
     max_episode_steps: 500
-
   simulator:
     turn_angle: 30
-    tilt_angle: 30
-    action_space_config: "v1"
     agents:
       main_agent:
         sim_sensors:
           semantic_sensor:
             width: 640
             height: 480
             hfov: 79
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/nav/vln_r2r.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/vln_r2r.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/close_cab.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/close_fridge.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/idle.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/idle_single_camera.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle_single_camera.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/interact.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/interact.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/nav_to_obj.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/nav_to_obj.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/open_cab.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/open_fridge.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/pick.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/pick.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/pick_spa.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/tidy_house.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 # @package _global_
 
 defaults:
   - /habitat: habitat_config_base
-  - /habitat/simulator/agents@habitat.simulator.agents.main_agent: rgbd_head_rgbd_arm_agent
-  # add third_rgb_sensor to rgbd_head_rgbd_arm_agent:
-  - /habitat/simulator/sim_sensors@habitat.simulator.agents.main_agent.sim_sensors.third_rgb_sensor: third_rgb_sensor
-  - /habitat/task/rearrange: pick_spa
+  - /habitat/simulator/agents@habitat.simulator.agents.main_agent: depth_head_agent
+  - /habitat/task/rearrange: tidy_house
   - /habitat/dataset/rearrangement: replica_cad
   - _self_
 
-# The configuration to run the SensePlanAct baseline architecture from https://arxiv.org/abs/2106.14405
 habitat:
+  gym:
+    obs_keys:
+    - head_depth
+    - relative_resting_position
+    - obj_start_sensor
+    - obj_goal_sensor
+    - obj_start_gps_compass
+    - obj_goal_gps_compass
+    - joint
+    - is_holding
   environment:
-    max_episode_steps: 30
+    max_episode_steps: 5000
   simulator:
     type: RearrangeSim-v0
     seed: 100
     additional_object_paths:
       - "data/objects/ycb/configs/"
     concur_render: True
     auto_sleep: True
     agents:
       main_agent:
         radius: 0.3
         sim_sensors:
-          head_rgb_sensor:
-            height: 128
-            width: 128
           head_depth_sensor:
-            width: 128
-            height: 128
-          arm_depth_sensor:
             height: 128
             width: 128
-          arm_rgb_sensor:
-            height: 128
-            width: 128
-          third_rgb_sensor:
-            height: 512
-            width: 512
-    # Agent setup
-    ac_freq_ratio: 8
-
     habitat_sim_v0:
       allow_sliding: False
       enable_physics: True
-
   dataset:
-    data_path: data/datasets/replica_cad/rearrange/v1/{split}/all_receptacles_10k_1k.json.gz
+    data_path: data/datasets/replica_cad/rearrange/v1/{split}/tidy_house_10k_1k.json.gz
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/place.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/place.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_human.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_human.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_spot.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_spot.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/play_stretch.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_stretch.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/prepare_groceries.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/reach_state.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/reach_state.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange_easy.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/set_table.yaml` & `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/benchmark/rearrange/tidy_house.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/set_table.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-# @package _global_
+# @package habitat.task
 
 defaults:
-  - /habitat: habitat_config_base
-  - /habitat/simulator/agents@habitat.simulator.agents.main_agent: depth_head_agent
-  - /habitat/task/rearrange: tidy_house
-  - /habitat/dataset/rearrangement: replica_cad
+  - /habitat/task: task_config_base
+  - /habitat/task/actions:
+    - arm_action
+    - base_velocity
+    - rearrange_stop
+  - /habitat/task/measurements:
+    - object_to_goal_distance
+    - articulated_agent_force
+    - force_terminate
+    - articulated_agent_colls
+    - end_effector_to_object_distance
+    - does_want_terminate
+    - composite_success
+    - bad_called_terminate
+    - num_steps
+    - did_violate_hold_constraint
+    - move_objects_reward
+    - composite_stage_goals
+  - /habitat/task/lab_sensors:
+    - relative_resting_pos_sensor
+    - target_start_sensor
+    - goal_sensor
+    - joint_sensor
+    - is_holding_sensor
+    - end_effector_sensor
+    - target_start_gps_compass_sensor
+    - target_goal_gps_compass_sensor
+    - localization_sensor
   - _self_
 
-habitat:
-  gym:
-    obs_keys:
-    - head_depth
-    - relative_resting_position
-    - obj_start_sensor
-    - obj_goal_sensor
-    - obj_start_gps_compass
-    - obj_goal_gps_compass
-    - joint
-    - is_holding
-  environment:
-    max_episode_steps: 5000
-  simulator:
-    type: RearrangeSim-v0
-    seed: 100
-    additional_object_paths:
-      - "data/objects/ycb/configs/"
-    concur_render: True
-    auto_sleep: True
-    agents:
-      main_agent:
-        radius: 0.3
-        sim_sensors:
-          head_depth_sensor:
-            height: 128
-            width: 128
-    habitat_sim_v0:
-      allow_sliding: False
-      enable_physics: True
-  dataset:
-    data_path: data/datasets/replica_cad/rearrange/v1/{split}/tidy_house_10k_1k.json.gz
+type: RearrangeCompositeTask-v0
+reward_measure: move_obj_reward
+success_measure: composite_success
+success_reward: 100.0
+end_on_success: True
+constraint_violation_ends_episode: False
+task_spec: set_table
+pddl_domain_def: replica_cad
+actions:
+  arm_action:
+    grip_controller: MagicGraspAction
+measurements:
+  move_objects_reward:
+    force_pen: 0.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/default.py` & `habitat-lab-0.2.520230729/habitat/config/default.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/default_structured_configs.py` & `habitat-lab-0.2.520230729/habitat/config/default_structured_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
     "PlaceSuccessMeasurementConfig",
     "PlaceRewardMeasurementConfig",
     "ArtObjSuccessMeasurementConfig",
     "ArtObjRewardMeasurementConfig",
     "NavToObjSuccessMeasurementConfig",
     "NavToObjRewardMeasurementConfig",
     "CompositeSuccessMeasurementConfig",
+    # PROFILING MEASURES
+    "RuntimePerfStatsMeasurementConfig",
 ]
 
 
 @dataclass
 class HabitatBaseConfig:
     pass
 
@@ -142,52 +144,59 @@
     """
     type: str = "EmptyAction"
 
 
 # -----------------------------------------------------------------------------
 # # NAVIGATION actions
 # -----------------------------------------------------------------------------
+
+
 @dataclass
-class MoveForwardActionConfig(ActionConfig):
+class DiscreteNavigationActionConfig(ActionConfig):
+    tilt_angle: int = 15  # angle to tilt the camera up or down in degrees
+
+
+@dataclass
+class MoveForwardActionConfig(DiscreteNavigationActionConfig):
     r"""
     In Navigation tasks only, this discrete action will move the robot forward by
     a fixed amount determined by the SimulatorConfig.forward_step_size amount.
     """
     type: str = "MoveForwardAction"
 
 
 @dataclass
-class TurnLeftActionConfig(ActionConfig):
+class TurnLeftActionConfig(DiscreteNavigationActionConfig):
     r"""
     In Navigation tasks only, this discrete action will rotate the robot to the left
     by a fixed amount determined by the SimulatorConfig.turn_angle amount.
     """
     type: str = "TurnLeftAction"
 
 
 @dataclass
-class TurnRightActionConfig(ActionConfig):
+class TurnRightActionConfig(DiscreteNavigationActionConfig):
     r"""
     In Navigation tasks only, this discrete action will rotate the robot to the right
     by a fixed amount determined by the SimulatorConfig.turn_angle amount.
     """
     type: str = "TurnRightAction"
 
 
 @dataclass
-class LookUpActionConfig(ActionConfig):
+class LookUpActionConfig(DiscreteNavigationActionConfig):
     r"""
     In Navigation tasks only, this discrete action will rotate the robot's camera up
     by a fixed amount determined by the SimulatorConfig.tilt_angle amount.
     """
     type: str = "LookUpAction"
 
 
 @dataclass
-class LookDownActionConfig(ActionConfig):
+class LookDownActionConfig(DiscreteNavigationActionConfig):
     r"""
     In Navigation tasks only, this discrete action will rotate the robot's camera down
     by a fixed amount determined by the SimulatorConfig.tilt_angle amount.
     """
     type: str = "LookDownAction"
 
 
@@ -672,14 +681,27 @@
 
 @dataclass
 class CollisionsMeasurementConfig(MeasurementConfig):
     type: str = "Collisions"
 
 
 @dataclass
+class RuntimePerfStatsMeasurementConfig(MeasurementConfig):
+    """
+    If added to the measurements, this will time various sections of code in
+    the simulator and task logic. If using with a multi-environment trainer
+    (like DD-PPO) it is recommended to only log this stat for one environment
+    since this metric can include many numbers.
+    """
+
+    type: str = "RuntimePerfStats"
+    disable_logging: bool = False
+
+
+@dataclass
 class RobotForceMeasurementConfig(MeasurementConfig):
     r"""
     The amount of force in newton's applied by the robot. It computes both the instant and accumulated.
     """
     type: str = "RobotForce"
     min_force: float = 20.0
 
@@ -1066,14 +1088,15 @@
 
 @dataclass
 class TaskConfig(HabitatBaseConfig):
     r"""
     The definition of the task in Habitat.
 
     :property type: The registered task that will be used. For example : `InstanceImageNav-v1` or `ObjectNav-v1`
+    :property physics_target_sps: The size of each simulator physics update will be 1 / physics_target_sps.
     :property reward_measure: The name of the Measurement that will correspond to the reward of the robot. This value must be a key present in the dictionary of Measurements in the habitat configuration. For example, `distance_to_goal_reward` for navigation or `place_reward` for the rearrangement place task.
     :property success_measure: The name of the Measurement that will correspond to the success criteria of the robot. This value must be a key present in the dictionary of Measurements in the habitat configuration. If the measurement has a non-zero value, the episode is considered a success.
     :property end_on_success: If True, the episode will end when the success measure indicates success. Otherwise the episode will go on (this is useful when doing hierarchical learning and the robot has to explicitly decide when to change policies)
     :property task_spec: When doing the `RearrangeCompositeTask-v0` only, will look for a pddl plan of that name to determine the sequence of tasks that need to be completed. The format of the pddl plans files is undocumented.
     :property task_spec_base_path:  When doing the `RearrangeCompositeTask-v0` only, the relative path where the task_spec file will be searched.
     :property spawn_max_dists_to_obj: For `RearrangePickTask-v0` task only. Controls the maximum distance the robot can be spawned from the target object.
     :property base_angle_noise: For Rearrangement tasks only. Controls the standard deviation of the random normal noise applied to the base's rotation angle at the start of an episode.
@@ -1092,24 +1115,32 @@
     -   Rearrangement navigate to object : `NavToObjTask-v0`
     -   Rearrangement pick : `RearrangePickTask-v0`
     -   Rearrangement place : `RearrangePlaceTask-v0`
     -   Rearrangement do nothing : `RearrangeEmptyTask-v0`
     -   Rearrangement reach : `RearrangeReachTask-v0`
     -   Rearrangement composite tasks : `RearrangeCompositeTask-v0`
     """
+    physics_target_sps: float = 60.0
     reward_measure: Optional[str] = None
     success_measure: Optional[str] = None
     success_reward: float = 2.5
     slack_reward: float = -0.01
     end_on_success: bool = False
     # NAVIGATION task
     type: str = "Nav-v0"
     # Temporary structure for sensors
     lab_sensors: Dict[str, LabSensorConfig] = field(default_factory=dict)
     measurements: Dict[str, MeasurementConfig] = field(default_factory=dict)
+    # Measures to only construct in the first environment of the first rank for
+    # vectorized environments.
+    rank0_env0_measure_names: List[str] = field(
+        default_factory=lambda: ["habitat_perf"]
+    )
+    # Measures to only record in the first rank for vectorized environments.
+    rank0_measure_names: List[str] = field(default_factory=list)
     goal_sensor_uuid: str = "pointgoal"
     # REARRANGE task
     count_obj_collisions: bool = True
     settle_steps: int = 5
     constraint_violation_ends_episode: bool = True
     constraint_violation_drops_object: bool = False
     # Forced to regenerate the starts even if they are already cached
@@ -1121,14 +1152,17 @@
     gfx_replay_dir = "data/replays"
     render_target: bool = True
     # Spawn parameters
     physics_stability_steps: int = 1
     num_spawn_attempts: int = 200
     spawn_max_dist_to_obj: float = 2.0
     base_angle_noise: float = 0.523599
+    # Factor to shrink the receptacle sampling volume when predicates place
+    # objects on top of receptacles.
+    recep_place_shrink_factor: float = 0.8
     # EE sample parameters
     ee_sample_factor: float = 0.2
     ee_exclude_region: float = 0.0
     base_noise: float = 0.05
     spawn_region_scale: float = 0.2
     joint_max_impulse: float = -1.0
     desired_resting_position: List[float] = field(
@@ -1145,15 +1179,14 @@
     # PDDL domain params
     pddl_domain_def: str = "replica_cad"
     obj_succ_thresh: float = 0.3
     # Disable drop except for when the object is at its goal.
     enable_safe_drop: bool = False
     art_succ_thresh: float = 0.15
     robot_at_thresh: float = 2.0
-    filter_nav_to_tasks: List = field(default_factory=list)
     actions: Dict[str, ActionConfig] = MISSING
 
 
 @dataclass
 class SimulatorSensorConfig(HabitatBaseConfig):
     type: str = MISSING
     height: int = 480
@@ -1310,22 +1343,38 @@
     radius: float = 0.1
     grasp_managers: int = 1
     sim_sensors: Dict[str, SimulatorSensorConfig] = field(default_factory=dict)
     is_set_start_state: bool = False
     start_position: List[float] = field(default_factory=lambda: [0, 0, 0])
     start_rotation: List[float] = field(default_factory=lambda: [0, 0, 0, 1])
     joint_start_noise: float = 0.1
+    # Hard-code the robot joint start. `joint_start_noise` still applies.
+    joint_start_override: Optional[List[float]] = None
     articulated_agent_urdf: str = "data/robots/hab_fetch/robots/hab_fetch.urdf"
     articulated_agent_type: str = "FetchRobot"
     ik_arm_urdf: str = "data/robots/hab_fetch/robots/fetch_onlyarm.urdf"
     # File to motion data, used to play pre-recorded motions
     motion_data_path: str = ""
 
 
 @dataclass
+class RendererConfig(HabitatBaseConfig):
+    r"""Configuration for the renderer.
+
+    :property enable_batch_renderer: [Experimental] Enables batch rendering, which accelerates rendering for concurrent environments. See env_batch_renderer.py for details.
+    :property composite_files: List of composite GLTF files to be pre-loaded by the batch renderer.
+    :property classic_replay_renderer: For debugging. Create a ClassicReplayRenderer instead of BatchReplayRenderer when enable_batch_renderer is active.
+    """
+
+    enable_batch_renderer: bool = False
+    composite_files: Optional[List[str]] = None
+    classic_replay_renderer: bool = False
+
+
+@dataclass
 class HabitatSimV0Config(HabitatBaseConfig):
     gpu_device_id: int = 0
     # Use Habitat-Sim's GPU->GPU copy mode to return rendering results in
     # pytorch tensors. Requires Habitat-Sim to be built with --with-cuda.
     # This will generally imply sharing cuda tensors between processes.
     # Read here:
     # https://pytorch.org/docs/stable/multiprocessing.html#sharing-cuda-tensors
@@ -1341,17 +1390,16 @@
     leave_context_with_background_renderer: bool = False
     enable_gfx_replay_save: bool = False
 
 
 @dataclass
 class SimulatorConfig(HabitatBaseConfig):
     type: str = "Sim-v0"
-    action_space_config: str = "v0"
-    action_space_config_arguments: Dict[str, Any] = field(default_factory=dict)
     forward_step_size: float = 0.25  # in metres
+    turn_angle: int = 10  # angle to rotate left or right in degrees
     create_renderer: bool = False
     requires_textures: bool = True
     # Sleep options
     auto_sleep: bool = False
     step_physics: bool = True
     concur_render: bool = False
     # If markers should be updated at every step:
@@ -1365,20 +1413,22 @@
     # A list of directory or config paths to search in addition to the dataset
     # for object configs. should match the generated episodes for the task:
     additional_object_paths: List[str] = field(default_factory=list)
     # Use config.seed (can't reference Config.seed) or define via code
     # otherwise it leads to circular references:
     #
     seed: int = II("habitat.seed")
-    turn_angle: int = 10  # angle to rotate left or right in degrees
-    tilt_angle: int = 15  # angle to tilt the camera up or down in degrees
     default_agent_id: int = 0
     debug_render: bool = False
     debug_render_articulated_agent: bool = False
     kinematic_mode: bool = False
+    # If False, will skip setting the semantic IDs of objects in
+    # `rearrange_sim.py` (there is overhead to this operation so skip if not
+    # using semantic information).
+    should_setup_semantic_ids: bool = True
     # If in render mode a visualization of the rearrangement goal position
     # should also be displayed
     debug_render_goal: bool = True
     robot_joint_start_noise: float = 0.0
     # Rearrange agent setup
     ctrl_freq: float = 120.0
     ac_freq_ratio: int = 4
@@ -1391,20 +1441,28 @@
     # agents_order specifies the order in which the agents
     # are stored on the habitat-sim side.
     # In other words, the order to return the observations and accept
     # the actions when using the environment API.
     # If the number of agents is greater than one,
     # then agents_order has to be set explicitly.
     agents_order: List[str] = MISSING
+
+    # Simulator should use default navmesh settings from agent config
+    default_agent_navmesh: bool = True
+    # if default navmesh is used, should it include static objects
+    navmesh_include_static_objects: bool = False
+
     habitat_sim_v0: HabitatSimV0Config = HabitatSimV0Config()
     # ep_info is added to the config in some rearrange tasks inside
     # merge_sim_episode_with_object_config
     ep_info: Optional[Any] = None
     # The offset id values for the object
     object_ids_start: int = 100
+    # Configuration for rendering
+    renderer: RendererConfig = RendererConfig()
 
 
 @dataclass
 class PyrobotSensor(HabitatBaseConfig):
     pass
 
 
@@ -2149,14 +2207,20 @@
 )
 cs.store(
     package="habitat.task.measurements.rearrange_reach_success",
     group="habitat/task/measurements",
     name="rearrange_reach_success",
     node=RearrangeReachSuccessMeasurementConfig,
 )
+cs.store(
+    package="habitat.task.measurements.habitat_perf",
+    group="habitat/task/measurements",
+    name="habitat_perf",
+    node=RuntimePerfStatsMeasurementConfig,
+)
 
 
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.core.plugins import Plugins
 from hydra.plugins.search_path_plugin import SearchPathPlugin
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/instance_imagenav.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/objectnav.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+
 defaults:
   - task_config_base
   - actions:
-      - stop
-      - move_forward
-      - turn_left
-      - turn_right
-      - look_up
-      - look_down
+    - stop
+    - move_forward
+    - turn_left
+    - turn_right
+    - look_up
+    - look_down
   - measurements:
-      - num_steps
-      - distance_to_goal
-      - success
-      - spl
-      - soft_spl
-      - distance_to_goal_reward
+    - distance_to_goal
+    - success
+    - spl
+    - soft_spl
+    - distance_to_goal_reward
   - lab_sensors:
-      - instance_imagegoal_sensor
-      - instance_imagegoal_hfov_sensor
-      - compass_sensor
-      - gps_sensor
+    - objectgoal_sensor
+    - compass_sensor
+    - gps_sensor
   - _self_
 
-type: InstanceImageNav-v1
+actions:
+  look_up:
+    tilt_angle: 30
+  look_down:
+    tilt_angle: 30
+
+type: ObjectNav-v1
 end_on_success: True
-reward_measure: distance_to_goal_reward
-success_measure: spl
-goal_sensor_uuid: instance_imagegoal
+reward_measure: "distance_to_goal_reward"
+success_measure: "spl"
+
+
+goal_sensor_uuid: objectgoal
+
 measurements:
   distance_to_goal:
     distance_to: VIEW_POINTS
   success:
     success_distance: 0.1
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/close_cab.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/close_fridge.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/nav_to_obj.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/nav_to_obj.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/open_cab.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_cab.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
   art_obj_reward:
     wrong_grasp_end: True
     grasp_reward: 5.0
     art_at_desired_state_reward: 5.0
     marker_dist_reward: 1.0
     constraint_violate_pen: 1.0
   force_terminate:
-    max_accum_force: 20_000.0
+    max_accum_force: -1.0
     max_instant_force: 10_000.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/open_fridge.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/set_table.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pick.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/place.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # @package habitat.task
 
 defaults:
   - /habitat/task: task_config_base
-  - /habitat/task/actions:
-    - arm_action
-    - base_velocity
+  - /habitat/task/rearrange/agents: fetch_base_arm
   - /habitat/task/measurements:
     - articulated_agent_force
     - force_terminate
+    - articulated_agent_colls
     - end_effector_to_rest_distance
-    - end_effector_to_object_distance
-    - did_pick_object
-    - pick_success
-    - pick_reward
-    - did_violate_hold_constraint
+    - end_effector_to_goal_distance
+    - object_to_goal_distance
+    - obj_at_goal
+    - place_success
+    - place_reward
     - num_steps
   - /habitat/task/lab_sensors:
     - target_start_sensor
+    - goal_sensor
     - joint_sensor
+    - joint_velocity_sensor
     - is_holding_sensor
     - end_effector_sensor
     - relative_resting_pos_sensor
+    - object_sensor
   - _self_
 
-type: RearrangePickTask-v0
+type: RearrangePlaceTask-v0
 base_angle_noise: 0.523599
 constraint_violation_ends_episode: False
 constraint_violation_drops_object: True
-reward_measure: "pick_reward"
-success_measure: "pick_success"
+reward_measure: place_reward
+success_measure: place_success
 success_reward: 10.0
 slack_reward: -0.005
 end_on_success: True
-actions:
-  arm_action:
-    grip_controller: SuctionGraspAction
 measurements:
   force_terminate:
     max_accum_force: 10_000.0
     max_instant_force: 10_000.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/pick_spa.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # @package habitat.task
 
 defaults:
   - /habitat/task: task_config_base
   - /habitat/task/actions:
     - arm_action
-    - empty
+    - base_velocity
+    - rearrange_stop
   - /habitat/task/measurements:
     - articulated_agent_force
-    - articulated_agent_colls
     - force_terminate
-    - end_effector_to_rest_distance
-    - end_effector_to_object_distance
-    - pick_success
-    - pick_reward
+    - articulated_agent_colls
+    - object_to_goal_distance
     - num_steps
+    - end_effector_to_object_distance
+    - does_want_terminate
+    - composite_success
+    - bad_called_terminate
+    - did_violate_hold_constraint
+    - move_objects_reward
   - /habitat/task/lab_sensors:
     - target_start_sensor
+    - goal_sensor
     - joint_sensor
     - is_holding_sensor
     - end_effector_sensor
     - relative_resting_pos_sensor
-    - goal_sensor
-    - object_sensor
+    - target_start_gps_compass_sensor
+    - target_goal_gps_compass_sensor
+    - localization_sensor
   - _self_
 
-# The configuration to run the SensePlanAct baseline architecture from https://arxiv.org/abs/2106.14405
-type: RearrangePickTask-v0
-count_obj_collisions: True
-desired_resting_position: [0.5, 0.0, 1.0]
-constraint_violation_ends_episode: True
-should_enforce_target_within_reach: False
-
-# In radians
-base_angle_noise: 0.15
-base_noise: 0.05
-force_regenerate: False
-
+type: RearrangeCompositeTask-v0
+reward_measure: move_obj_reward
+success_measure: composite_success
+success_reward: 100.0
+slack_reward: -0.01
+end_on_success: True
+constraint_violation_ends_episode: False
+constraint_violation_drops_object: True
+task_spec: rearrange
 actions:
   arm_action:
-    arm_controller: "ArmAbsPosKinematicAction"
-    grip_controller: "MagicGraspAction"
+    grip_controller: SuctionGraspAction
 measurements:
-  pick_reward:
-    dist_reward: 10.0
-    pick_reward: 5.0
+  force_terminate:
+    max_accum_force: 100000.0
+    max_instant_force: 10000.0
+  move_objects_reward:
     force_pen: 0.0
-    max_force_pen: 0.0
-    force_end_pen: 0.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/place.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pick.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 # @package habitat.task
 
 defaults:
   - /habitat/task: task_config_base
-  - /habitat/task/actions:
-    - arm_action
-    - base_velocity
+  - /habitat/task/rearrange/agents: fetch_base_arm
   - /habitat/task/measurements:
     - articulated_agent_force
     - force_terminate
-    - articulated_agent_colls
     - end_effector_to_rest_distance
-    - end_effector_to_goal_distance
-    - object_to_goal_distance
-    - obj_at_goal
-    - place_success
-    - place_reward
+    - end_effector_to_object_distance
+    - did_pick_object
+    - pick_success
+    - pick_reward
+    - did_violate_hold_constraint
     - num_steps
   - /habitat/task/lab_sensors:
     - target_start_sensor
-    - goal_sensor
     - joint_sensor
-    - joint_velocity_sensor
     - is_holding_sensor
     - end_effector_sensor
     - relative_resting_pos_sensor
-    - object_sensor
   - _self_
 
-type: RearrangePlaceTask-v0
+type: RearrangePickTask-v0
 base_angle_noise: 0.523599
 constraint_violation_ends_episode: False
 constraint_violation_drops_object: True
-reward_measure: place_reward
-success_measure: place_success
+reward_measure: "pick_reward"
+success_measure: "pick_success"
 success_reward: 10.0
 slack_reward: -0.005
 end_on_success: True
-actions:
-  arm_action:
-    grip_controller: SuctionGraspAction
 measurements:
   force_terminate:
     max_accum_force: 10_000.0
     max_instant_force: 10_000.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/play.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/play_human.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play_human.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/prepare_groceries.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/reach_state.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/reach_state.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # @package habitat.task
 
 defaults:
   - /habitat/task: task_config_base
   - /habitat/task/actions:
-    - arm_action
     - base_velocity
     - rearrange_stop
   - /habitat/task/measurements:
+    - object_to_goal_distance
     - articulated_agent_force
     - force_terminate
     - articulated_agent_colls
-    - object_to_goal_distance
-    - num_steps
     - end_effector_to_object_distance
     - does_want_terminate
     - composite_success
     - bad_called_terminate
+    - num_steps
     - did_violate_hold_constraint
     - move_objects_reward
+    - gfx_replay_measure
+    - composite_stage_goals
   - /habitat/task/lab_sensors:
+    - relative_resting_pos_sensor
     - target_start_sensor
     - goal_sensor
     - joint_sensor
     - is_holding_sensor
     - end_effector_sensor
-    - relative_resting_pos_sensor
     - target_start_gps_compass_sensor
     - target_goal_gps_compass_sensor
     - localization_sensor
   - _self_
 
 type: RearrangeCompositeTask-v0
 reward_measure: move_obj_reward
 success_measure: composite_success
 success_reward: 100.0
 slack_reward: -0.01
 end_on_success: True
 constraint_violation_ends_episode: False
 constraint_violation_drops_object: True
-task_spec: rearrange
-actions:
-  arm_action:
-    grip_controller: SuctionGraspAction
+task_spec: rearrange_easy
 measurements:
+  move_objects_reward:
+    force_pen: 0.0
   force_terminate:
     max_accum_force: 100000.0
     max_instant_force: 10000.0
-  move_objects_reward:
-    force_pen: 0.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/config/habitat/task/rearrange/set_table.yaml` & `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/tidy_house.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,11 @@
 
 type: RearrangeCompositeTask-v0
 reward_measure: move_obj_reward
 success_measure: composite_success
 success_reward: 100.0
 end_on_success: True
 constraint_violation_ends_episode: False
-task_spec: set_table
-pddl_domain_def: replica_cad
+task_spec: tidy_house
 actions:
   arm_action:
     grip_controller: MagicGraspAction
-measurements:
-  move_objects_reward:
-    force_pen: 0.0
```

### Comparing `habitat-lab-0.2.420230405/habitat/config/read_write.py` & `habitat-lab-0.2.520230729/habitat/config/read_write.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/agent.py` & `habitat-lab-0.2.520230729/habitat/core/agent.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/benchmark.py` & `habitat-lab-0.2.520230729/habitat/core/benchmark.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/challenge.py` & `habitat-lab-0.2.520230729/habitat/core/challenge.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/dataset.py` & `habitat-lab-0.2.520230729/habitat/core/dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/embodied_task.py` & `habitat-lab-0.2.520230729/habitat/core/embodied_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 r"""Implements task and measurements needed for training and benchmarking of
 ``habitat.Agent`` inside ``habitat.Env``.
 """
 
+import time
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 from omegaconf import OmegaConf
 
 from habitat.core.dataset import Dataset, Episode
@@ -160,17 +161,20 @@
             ), "'{}' is duplicated measure uuid".format(measure.uuid)
             self.measures[measure.uuid] = measure
 
     def reset_measures(self, *args: Any, **kwargs: Any) -> None:
         for measure in self.measures.values():
             measure.reset_metric(*args, **kwargs)
 
-    def update_measures(self, *args: Any, **kwargs: Any) -> None:
+    def update_measures(self, *args: Any, task, **kwargs: Any) -> None:
         for measure in self.measures.values():
-            measure.update_metric(*args, **kwargs)
+            t_start = time.time()
+            measure.update_metric(*args, task=task, **kwargs)
+            measure_name = measure._get_uuid(*args, task=task, **kwargs)
+            task.add_perf_timing(f"measures.{measure_name}", t_start)
 
     def get_metrics(self) -> Metrics:
         r"""Collects measurement from all :ref:`Measure`\ s and returns it
         packaged inside :ref:`Metrics`.
         """
         return Metrics(self.measures)
 
@@ -233,14 +237,18 @@
         dataset: Optional[Dataset] = None,
     ) -> None:
         from habitat.core.registry import registry
 
         self._config = config
         self._sim = sim
         self._dataset = dataset
+        self._physics_target_sps = config.physics_target_sps
+        assert (
+            self._physics_target_sps > 0
+        ), "physics_target_sps must be positive"
 
         self.measurements = Measurements(
             self._init_entities(
                 entities_configs=config.measurements,
                 register_func=registry.get_measure,
             ).values()
         )
@@ -256,14 +264,18 @@
             entities_configs=config.actions,
             register_func=registry.get_task_action,
         )
         self._action_keys = list(self.actions.keys())
 
         self._is_episode_active = False
 
+    def add_perf_timing(self, *args, **kwargs):
+        if hasattr(self._sim, "add_perf_timing"):
+            self._sim.add_perf_timing(*args, **kwargs)
+
     def _init_entities(self, entities_configs, register_func) -> OrderedDict:
         entities = OrderedDict()
         for entity_name, entity_cfg in entities_configs.items():
             entity_cfg = OmegaConf.create(entity_cfg)
             if "type" not in entity_cfg:
                 raise ValueError(f"Could not find type in {entity_cfg}")
             entity_type = register_func(entity_cfg.type)
@@ -278,72 +290,74 @@
             )
         return entities
 
     def reset(self, episode: Episode):
         observations = self._sim.reset()
         observations.update(
             self.sensor_suite.get_observations(
-                observations=observations, episode=episode, task=self
+                observations=observations,
+                episode=episode,
+                task=self,
+                should_time=True,
             )
         )
 
         for action_instance in self.actions.values():
             action_instance.reset(episode=episode, task=self)
 
         self._is_episode_active = True
 
         return observations
 
     def _step_single_action(
         self,
-        observations: Any,
         action_name: Any,
         action: Dict[str, Any],
         episode: Episode,
-        is_last_action=True,
     ):
         if isinstance(action_name, (int, np.integer)):
             action_name = self.get_action_name(action_name)
         assert (
             action_name in self.actions
         ), f"Can't find '{action_name}' action in {self.actions.keys()}."
         task_action = self.actions[action_name]
-        observations.update(
-            task_action.step(
-                **action["action_args"],
-                task=self,
-                is_last_action=is_last_action,
-            )
+        return task_action.step(
+            **action["action_args"],
+            task=self,
         )
 
     def step(self, action: Dict[str, Any], episode: Episode):
         action_name = action["action"]
         if "action_args" not in action or action["action_args"] is None:
             action["action_args"] = {}
-        observations: Any = {}
+        observations: Optional[Any] = None
         if isinstance(action_name, tuple):  # there are multiple actions
-            for i, a_name in enumerate(action_name):
-                self._step_single_action(
-                    observations,
+            for a_name in action_name:
+                observations = self._step_single_action(
                     a_name,
                     action,
                     episode,
-                    i == len(action_name) - 1,
                 )
         else:
-            self._step_single_action(
-                observations, action_name, action, episode
+            observations = self._step_single_action(
+                action_name, action, episode
             )
 
+        self._sim.step_physics(1.0 / self._physics_target_sps)  # type:ignore
+
+        if observations is None:
+            observations = self._sim.step(None)
+
         observations.update(
             self.sensor_suite.get_observations(
                 observations=observations,
                 episode=episode,
                 action=action,
                 task=self,
+                should_time=True,
             )
         )
         self._is_episode_active = self._check_episode_is_active(
             observations=observations, action=action, episode=episode
         )
         return observations
```

### Comparing `habitat-lab-0.2.420230405/habitat/core/env.py` & `habitat-lab-0.2.520230729/habitat/core/env.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/environments.py` & `habitat-lab-0.2.520230729/habitat/core/environments.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 class RLTaskEnv(habitat.RLEnv):
     def __init__(
         self, config: "DictConfig", dataset: Optional[Dataset] = None
     ):
         super().__init__(config, dataset)
         self._reward_measure_name = self.config.task.reward_measure
         self._success_measure_name = self.config.task.success_measure
+        self._slack_reward = self.config.task.slack_reward
+        self._success_reward = self.config.task.success_reward
+        self._end_on_success = self.config.task.end_on_success
         assert (
             self._reward_measure_name is not None
         ), "The key task.reward_measure cannot be None"
         assert (
             self._success_measure_name is not None
         ), "The key task.success_measure cannot be None"
 
@@ -65,31 +68,31 @@
 
     def get_reward_range(self):
         # We don't know what the reward measure is bounded by
         return (-np.inf, np.inf)
 
     def get_reward(self, observations):
         current_measure = self._env.get_metrics()[self._reward_measure_name]
-        reward = self.config.task.slack_reward
+        reward = self._slack_reward
 
         reward += current_measure
 
         if self._episode_success():
-            reward += self.config.task.success_reward
+            reward += self._success_reward
 
         return reward
 
     def _episode_success(self):
         return self._env.get_metrics()[self._success_measure_name]
 
     def get_done(self, observations):
         done = False
         if self._env.episode_over:
             done = True
-        if self.config.task.end_on_success and self._episode_success():
+        if self._end_on_success and self._episode_success():
             done = True
         return done
 
     def get_info(self, observations):
         return self._env.get_metrics()
```

### Comparing `habitat-lab-0.2.420230405/habitat/core/logging.py` & `habitat-lab-0.2.520230729/habitat/core/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
+import os
 
 
 class HabitatLogger(logging.Logger):
     def __init__(
         self,
         name,
         level,
@@ -31,9 +32,11 @@
     def add_filehandler(self, log_filename):
         filehandler = logging.FileHandler(log_filename)
         filehandler.setFormatter(self._formatter)
         self.addHandler(filehandler)
 
 
 logger = HabitatLogger(
-    name="habitat", level=logging.INFO, format_str="%(asctime)-15s %(message)s"
+    name="habitat",
+    level=int(os.environ.get("HABITAT_LAB_LOG", logging.INFO)),
+    format_str="%(asctime)-15s %(message)s",
 )
```

### Comparing `habitat-lab-0.2.420230405/habitat/core/registry.py` & `habitat-lab-0.2.520230729/habitat/core/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 """
 
 import collections
 from typing import TYPE_CHECKING, Any, Callable, DefaultDict, Optional, Type
 
 from habitat.core.dataset import Dataset
 from habitat.core.embodied_task import Action, EmbodiedTask, Measure
-from habitat.core.simulator import ActionSpaceConfiguration, Sensor, Simulator
+from habitat.core.simulator import Sensor, Simulator
 from habitat.core.utils import Singleton
 
 if TYPE_CHECKING:
     from habitat.core.env import RLEnv
 
 
 class Registry(metaclass=Singleton):
@@ -178,31 +178,14 @@
         """
 
         return cls._register_impl(
             "dataset", to_register, name, assert_type=Dataset
         )
 
     @classmethod
-    def register_action_space_configuration(
-        cls, to_register=None, *, name: Optional[str] = None
-    ):
-        r"""Register a action space configuration to registry with key :p:`name`
-
-        :param name: Key with which the action space will be registered.
-            If :py:`None` will use the name of the class
-        """
-
-        return cls._register_impl(
-            "action_space_config",
-            to_register,
-            name,
-            assert_type=ActionSpaceConfiguration,
-        )
-
-    @classmethod
     def register_env(cls, to_register=None, *, name: Optional[str] = None):
         r"""Register a environment to registry with key 'name'
             currently only support subclass of RLEnv.
 
         Args:
             name: Key with which the env will be registered.
                 If None will use the name of the class.
@@ -237,18 +220,12 @@
         return cls._get_impl("measure", name)
 
     @classmethod
     def get_dataset(cls, name: str) -> Type[Dataset]:
         return cls._get_impl("dataset", name)
 
     @classmethod
-    def get_action_space_configuration(
-        cls, name: str
-    ) -> Type[ActionSpaceConfiguration]:
-        return cls._get_impl("action_space_config", name)
-
-    @classmethod
     def get_env(cls, name: str) -> Type["RLEnv"]:
         return cls._get_impl("env", name)
 
 
 registry = Registry()
```

### Comparing `habitat-lab-0.2.420230405/habitat/core/simulator.py` & `habitat-lab-0.2.520230729/habitat/core/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 import abc
+import time
 from collections import OrderedDict
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
@@ -108,26 +109,33 @@
         raise NotImplementedError
 
 
 class Observations(Dict[str, Any]):
     r"""Dictionary containing sensor observations"""
 
     def __init__(
-        self, sensors: Dict[str, Sensor], *args: Any, **kwargs: Any
+        self,
+        sensors: Dict[str, Sensor],
+        *args: Any,
+        should_time: bool = False,
+        **kwargs: Any,
     ) -> None:
         """Constructor
 
         :param sensors: list of sensors whose observations are fetched and
             packaged.
         """
+        data = []
+        for uuid, sensor in sensors.items():
+            t_start = time.time()
+            data.append((uuid, sensor.get_observation(*args, **kwargs)))
+
+            if should_time:
+                kwargs["task"].add_perf_timing(f"sensors.{uuid}", t_start)
 
-        data = [
-            (uuid, sensor.get_observation(*args, **kwargs))
-            for uuid, sensor in sensors.items()
-        ]
         super().__init__(data)
 
 
 class RGBSensor(Sensor, metaclass=abc.ABCMeta):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
```

### Comparing `habitat-lab-0.2.420230405/habitat/core/spaces.py` & `habitat-lab-0.2.520230729/habitat/core/spaces.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/utils.py` & `habitat-lab-0.2.520230729/habitat/core/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/core/vector_env.py` & `habitat-lab-0.2.520230729/habitat/core/vector_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
+    OrderedDict,
     Sequence,
     Set,
     Tuple,
     Union,
     cast,
 )
 
 import attr
 import gym
 import numpy as np
 from gym import spaces
 
 import habitat
+from habitat.core.batch_rendering.env_batch_renderer import EnvBatchRenderer
 from habitat.core.env import Env, RLEnv
 from habitat.core.logging import logger
 from habitat.core.utils import tile_images
 from habitat.gym.gym_env_episode_count_wrapper import EnvCountEpisodeWrapper
 from habitat.gym.gym_env_obs_dict_wrapper import EnvObsDictWrapper
 from habitat.utils import profiling_wrapper
 from habitat.utils.pickle5_multiprocessing import (
@@ -144,14 +146,15 @@
     action_spaces: List[spaces.Dict]
     _workers: List[Union[mp.Process, Thread]]
     _num_envs: int
     _auto_reset_done: bool
     _mp_ctx: BaseContext
     _connection_read_fns: List[_ReadWrapper]
     _connection_write_fns: List[_WriteWrapper]
+    _batch_renderer: Optional[EnvBatchRenderer] = None
 
     def __init__(
         self,
         make_env_fn: Callable[..., gym.Env],
         env_fn_args: Sequence[Tuple],
         auto_reset_done: bool = True,
         multiprocessing_start_method: str = "forkserver",
@@ -225,15 +228,14 @@
 
     @property
     def num_envs(self):
         r"""number of individual environments."""
         return self._num_envs - len(self._paused)
 
     @staticmethod
-    @profiling_wrapper.RangeContext("_worker_env")
     def _worker_env(
         connection_read_fn: Callable,
         connection_write_fn: Callable,
         env_fn: Callable,
         env_fn_args: Tuple[Any],
         auto_reset_done: bool,
         mask_signals: bool = False,
@@ -252,20 +254,19 @@
         if parent_pipe is not None:
             parent_pipe.close()
         try:
             command, data = connection_read_fn()
             while command != CLOSE_COMMAND:
                 if command == STEP_COMMAND:
                     observations, reward, done, info = env.step(data)
+
                     if auto_reset_done and done:
                         observations = env.reset()
-                    with profiling_wrapper.RangeContext(
-                        "worker write after step"
-                    ):
-                        connection_write_fn((observations, reward, done, info))
+
+                    connection_write_fn((observations, reward, done, info))
 
                 elif command == RESET_COMMAND:
                     observations = env.reset()
                     connection_write_fn(observations)
 
                 elif command == RENDER_COMMAND:
                     connection_write_fn(env.render(*data[0], **data[1]))
@@ -286,16 +287,15 @@
 
                 elif command == COUNT_EPISODES_COMMAND:
                     connection_write_fn(len(env.episodes))
 
                 else:
                     raise NotImplementedError(f"Unknown command {command}")
 
-                with profiling_wrapper.RangeContext("worker wait for command"):
-                    command, data = connection_read_fn()
+                command, data = connection_read_fn()
 
         except KeyboardInterrupt:
             logger.info("Worker KeyboardInterrupt")
         finally:
             if child_pipe is not None:
                 child_pipe.close()
             env.close()
@@ -428,15 +428,15 @@
         """
 
         for index_env, act in enumerate(data):
             self.async_step_at(index_env, act)
 
     @profiling_wrapper.RangeContext("wait_step")
     def wait_step(self) -> List[Any]:
-        r"""Wait until all the asynchronized environments have synchronized."""
+        r"""Wait until all the asynchronous environments have synchronized."""
         return [
             self.wait_step_at(index_env) for index_env in range(self.num_envs)
         ]
 
     def step(self, data: Sequence[Union[int, np.ndarray]]) -> List[Any]:
         r"""Perform actions in the vectorized environments.
 
@@ -444,14 +444,24 @@
             pass to :ref:`step` method for each Environment. For example,
             :py:`[1, 3 ,5 , ...]`.
         :return: list of outputs from the step method of envs.
         """
         self.async_step(data)
         return self.wait_step()
 
+    def post_step(self, observations) -> List[OrderedDict]:
+        r"""Performs batch transformations on step outputs.
+
+        :param observations: Observation dicts for each environment.
+        :return: Processed observation dicts for each environment.
+        """
+        if self._batch_renderer is not None:
+            observations = self._batch_renderer.post_step(observations)
+        return observations
+
     def close(self) -> None:
         if self._is_closed:
             return
 
         for read_fn in self._connection_read_fns:
             if read_fn.is_waiting:
                 read_fn()
@@ -466,14 +476,17 @@
             process.join()
 
         for _, _, _, process in self._paused:
             process.join()
 
         self._is_closed = True
 
+        if self._batch_renderer != None:
+            self._batch_renderer.close()
+
     def pause_at(self, index: int) -> None:
         r"""Pauses computation on this env without destroying the env.
 
         :param index: which env to pause. All indexes after this one will be
             shifted down by one.
 
         This is useful for not needing to call steps on all environments when
@@ -542,31 +555,44 @@
             results.append(read_fn())
         return results
 
     def render(
         self, mode: str = "human", *args, **kwargs
     ) -> Optional[np.ndarray]:
         r"""Render observations from all environments in a tiled image."""
-        for write_fn in self._connection_write_fns:
-            write_fn((RENDER_COMMAND, (args, {"mode": "rgb_array", **kwargs})))
-        images = [read_fn() for read_fn in self._connection_read_fns]
+        if self._batch_renderer is not None:
+            images = self._batch_renderer.copy_output_to_image()
+        else:
+            for write_fn in self._connection_write_fns:
+                write_fn(
+                    (RENDER_COMMAND, (args, {"mode": "rgb_array", **kwargs}))
+                )
+            images = [read_fn() for read_fn in self._connection_read_fns]
         tile = tile_images(images)
         if mode == "human":
             from habitat.core.utils import try_cv2_import
 
             cv2 = try_cv2_import()
 
             cv2.imshow("vecenv", tile[:, :, ::-1])
             cv2.waitKey(1)
             return None
         elif mode == "rgb_array":
             return tile
         else:
             raise NotImplementedError
 
+    def initialize_batch_renderer(self, config: "DictConfig") -> None:
+        r"""Provides VectorEnv with batch rendering capability.
+        Refer to the EnvBatchRenderer class.
+
+        :param config: Base configuration."""
+        assert config.habitat.simulator.renderer.enable_batch_renderer
+        self._batch_renderer = EnvBatchRenderer(config, self.num_envs)
+
     @property
     def _valid_start_methods(self) -> Set[str]:
         return {"forkserver", "spawn", "fork"}
 
     def _warn_cuda_tensors(
         self,
         action: Union[int, np.ndarray, Dict[str, Any], "torch.Tensor"],
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/eqa/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/eqa/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/eqa/mp3d_eqa_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/eqa/mp3d_eqa_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/image_nav/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/image_nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/image_nav/instance_image_nav_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/image_nav/instance_image_nav_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/object_nav/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/object_nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/object_nav/object_nav_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/object_nav/object_nav_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/pointnav/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/pointnav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/pointnav/pointnav_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,23 +86,31 @@
         for filename in os.listdir(content_dir):
             if filename.endswith(scene_dataset_ext):
                 scene = filename[: -len(scene_dataset_ext)]
                 scenes.append(scene)
         scenes.sort()
         return scenes
 
+    def _load_from_file(self, fname: str, scenes_dir: str) -> None:
+        """
+        Load the data from a file into `self.episodes`.
+        """
+
+        with gzip.open(fname, "rt") as f:
+            self.from_json(f.read(), scenes_dir=scenes_dir)
+
     def __init__(self, config: Optional["DictConfig"] = None) -> None:
         self.episodes = []
 
         if config is None:
             return
 
         datasetfile_path = config.data_path.format(split=config.split)
-        with gzip.open(datasetfile_path, "rt") as f:
-            self.from_json(f.read(), scenes_dir=config.scenes_dir)
+
+        self._load_from_file(datasetfile_path, config.scenes_dir)
 
         # Read separate file for each scene
         dataset_dir = os.path.dirname(datasetfile_path)
         has_individual_scene_files = os.path.exists(
             self.content_scenes_path.split("{scene}")[0].format(
                 data_path=dataset_dir
             )
@@ -115,16 +123,16 @@
                     dataset_dir=dataset_dir,
                 )
 
             for scene in scenes:
                 scene_filename = self.content_scenes_path.format(
                     data_path=dataset_dir, scene=scene
                 )
-                with gzip.open(scene_filename, "rt") as f:
-                    self.from_json(f.read(), scenes_dir=config.scenes_dir)
+
+                self._load_from_file(scene_filename, config.scenes_dir)
 
         else:
             self.episodes = list(
                 filter(self.build_content_scenes_filter(config), self.episodes)
             )
 
     def from_json(
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/pointnav/pointnav_generator.py` & `habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_generator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/combine_datasets.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/combine_datasets.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/all_receptacles.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/all_receptacles.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/bench_config.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/bench_config.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/empty.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/empty.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/rearrange.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 object_samplers:
   -
     name: "clutter"
     type: "uniform"
     params:
       object_sets: ["hab2"]
       receptacle_sets: ["clutter"]
-      num_samples: [30, 30]
+      num_samples: [30, 40]
       orientation_sampling: "up"
   -
     name: "any_targets"
     type: "uniform"
     params:
       object_sets: ["hab2"]
       receptacle_sets: ["hab2_recep", "hab2"]
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/set_table.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/hab/tidy_house.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/in_drawer.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_drawer.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/in_fridge.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/configs/test_config.yaml` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/test_config.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/generate_episode_inits.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/generate_episode_inits.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/rearrange_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,20 @@
         self.config = config
 
         if config and not self.check_config_paths_exist(config):
             logger.info(
                 "Rearrange task assets are not downloaded locally, downloading and extracting now..."
             )
             data_downloader.main(
-                ["--uids", "rearrange_task_assets", "--no-replace"]
+                [
+                    "--uids",
+                    "rearrange_task_assets",
+                    "--no-replace",
+                    "--no-prune",
+                ]
             )
             logger.info("Downloaded and extracted the data.")
 
         check_and_gen_physics_config()
 
         super().__init__(config)
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/rearrange_generator.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os.path as osp
+import random
 import time
 from collections import defaultdict
 
 try:
     from collections import Sequence
 except ImportError:
     from collections.abc import Sequence
@@ -206,15 +207,14 @@
                     for x in self._obj_sets[y]
                 ]
                 object_handles = sorted(set(object_handles))
                 if len(object_handles) == 0:
                     raise ValueError(
                         f"Found no object handles for {obj_sampler_info}"
                     )
-
                 self._obj_samplers[
                     obj_sampler_info["name"]
                 ] = samplers.ObjectSampler(
                     object_handles,
                     obj_sampler_info["params"]["receptacle_sets"],
                     (
                         obj_sampler_info["params"]["num_samples"][0],
@@ -222,14 +222,17 @@
                     ),
                     obj_sampler_info["params"]["orientation_sampling"],
                     get_sample_region_ratios(obj_sampler_info),
                     obj_sampler_info["params"].get(
                         "nav_to_min_distance", -1.0
                     ),
                     obj_sampler_info["params"].get("sample_probs", None),
+                    obj_sampler_info["params"].get(
+                        "constrain_to_largest_nav_island", False
+                    ),
                 )
             else:
                 logger.info(
                     f"Requested object sampler '{obj_sampler_info['type']}' is not implemented."
                 )
                 raise (NotImplementedError)
 
@@ -450,74 +453,96 @@
             "sampled_objects": {},  # object sampler name -> sampled object instances
             "sampled_targets": {},  # target sampler name -> (object, target state)
         }
 
         ep_scene_handle = self.generate_scene()
         scene_base_dir = osp.dirname(osp.dirname(ep_scene_handle))
 
+        recep_tracker.init_scene_filters(
+            mm=self.sim.metadata_mediator, scene_handle=ep_scene_handle
+        )
+
         scene_name = ep_scene_handle.split(".")[0]
         navmesh_path = osp.join(
             scene_base_dir, "navmeshes", scene_name + ".navmesh"
         )
         self.sim.pathfinder.load_nav_mesh(navmesh_path)
 
+        # prepare target samplers
         self._get_object_target_samplers()
-        target_numbers = {
+        target_numbers: Dict[str, int] = {
             k: sampler.target_objects_number
             for k, sampler in self._target_samplers.items()
         }
-        targ_sampler_name_to_obj_sampler_names = {}
+        # prepare mapping of target samplers to their source object samplers
+        targ_sampler_name_to_obj_sampler_names: Dict[str, List[str]] = {}
         for targ_sampler_cfg in self.cfg.object_target_samplers:
             sampler_name = targ_sampler_cfg["name"]
             targ_sampler_name_to_obj_sampler_names[
                 sampler_name
             ] = targ_sampler_cfg["params"]["object_samplers"]
 
+        # sample and allocate receptacles to contain the target objects
         target_receptacles = defaultdict(list)
         all_target_receptacles = []
         for sampler_name, num_targets in target_numbers.items():
-            obj_sampler_name = targ_sampler_name_to_obj_sampler_names[
-                sampler_name
-            ][0]
-            sampler = self._obj_samplers[obj_sampler_name]
-            new_target_receptacles = []
-            for _ in range(num_targets):
-                new_receptacle = sampler.sample_receptacle(
-                    self.sim, recep_tracker
-                )
-                if recep_tracker.update_receptacle_tracking(new_receptacle):
+            new_target_receptacles: List[Receptacle] = []
+            failed_samplers: Dict[str, bool] = defaultdict(bool)
+            while len(new_target_receptacles) < num_targets:
+                assert len(failed_samplers.keys()) < len(
+                    targ_sampler_name_to_obj_sampler_names[sampler_name]
+                ), f"All target samplers failed to find a match for '{sampler_name}'."
+                obj_sampler_name = random.choice(
+                    targ_sampler_name_to_obj_sampler_names[sampler_name]
+                )
+                sampler = self._obj_samplers[obj_sampler_name]
+                new_receptacle = None
+                try:
+                    new_receptacle = sampler.sample_receptacle(
+                        self.sim, recep_tracker
+                    )
+                except AssertionError:
+                    # No receptacle instances found matching this sampler's requirements, likely ran out of allocations and a different sampler should be tried
+                    failed_samplers[obj_sampler_name]
+                    continue
+
+                if recep_tracker.allocate_one_placement(new_receptacle):
+                    # used up new_receptacle, need to recompute the sampler's receptacle_candidates
                     sampler.receptacle_candidates = None
                 new_target_receptacles.append(new_receptacle)
 
             target_receptacles[obj_sampler_name].extend(new_target_receptacles)
             all_target_receptacles.extend(new_target_receptacles)
 
+        # sample and allocate receptacles to contain the goal states for target objects
         goal_receptacles = {}
         all_goal_receptacles = []
         for sampler, (sampler_name, num_targets) in zip(
             self._target_samplers.values(), target_numbers.items()
         ):
             new_goal_receptacles = []
             for _ in range(num_targets):
                 new_receptacle = sampler.sample_receptacle(
                     self.sim,
                     recep_tracker,
                 )
                 if isinstance(new_receptacle, OnTopOfReceptacle):
                     new_receptacle.set_episode_data(self.episode_data)
-                if recep_tracker.update_receptacle_tracking(new_receptacle):
+                if recep_tracker.allocate_one_placement(new_receptacle):
+                    # used up new_receptacle, need to recompute the sampler's receptacle_candidates
                     sampler.receptacle_candidates = None
 
                 new_goal_receptacles.append(new_receptacle)
 
             goal_receptacles[sampler_name] = new_goal_receptacles
             all_goal_receptacles.extend(new_goal_receptacles)
 
+        # Goal and target containing receptacles are allowed 1 extra maximum object for each goal/target if a limit was defined
         for recep in [*all_goal_receptacles, *all_target_receptacles]:
-            recep_tracker.inc_count(recep.name)
+            recep_tracker.inc_count(recep.unique_name)
 
         # sample AO states for objects in the scene
         # ao_instance_handle -> [ (link_ix, state), ... ]
         ao_states: Dict[str, Dict[int, float]] = {}
         for _sampler_name, ao_state_sampler in self._ao_state_samplers.items():
             sampler_states = ao_state_sampler.sample(
                 self.sim,
@@ -532,27 +557,38 @@
                     ao_states[sampled_instance.handle][link_ix] = joint_state
 
         # visualize after setting AO states to correctly see scene state
         if self._render_debug_obs:
             self.visualize_scene_receptacles()
             self.vdb.make_debug_video(prefix="receptacles_")
 
+        # track a list of target objects to be used for settle culling later
+        target_object_names: List[str] = []
         # sample object placements
         self.object_to_containing_receptacle: Dict[str, Receptacle] = {}
         for sampler_name, obj_sampler in self._obj_samplers.items():
             object_sample_data = obj_sampler.sample(
                 self.sim,
                 recep_tracker,
                 target_receptacles[sampler_name],
                 snap_down=True,
                 vdb=(self.vdb if self._render_debug_obs else None),
             )
             if len(object_sample_data) == 0:
                 return None
             new_objects, receptacles = zip(*object_sample_data)
+            # collect names of all newly placed target objects
+            target_object_names.extend(
+                [
+                    obj.handle
+                    for obj in new_objects[
+                        : len(target_receptacles[sampler_name])
+                    ]
+                ]
+            )
             for obj, rec in zip(new_objects, receptacles):
                 self.object_to_containing_receptacle[obj.handle] = rec
             if sampler_name not in self.episode_data["sampled_objects"]:
                 self.episode_data["sampled_objects"][
                     sampler_name
                 ] = new_objects
             else:
@@ -573,15 +609,15 @@
                     self.vdb.look_at(new_object.translation)
                     self.vdb.get_observation()
                 logger.debug(
                     f"... done generating the debug images for {len(new_objects)} objects."
                 )
 
         # simulate the world for a few seconds to validate the placements
-        if not self.settle_sim():
+        if not self.settle_sim(target_object_names):
             logger.warning(
                 "Aborting episode generation due to unstable state."
             )
             return None
 
         for sampler, target_sampler_info in zip(
             self._target_samplers.values(), self.cfg.object_target_samplers
@@ -594,15 +630,15 @@
             sampler.object_set = [
                 x.creation_attributes.handle
                 for x in sampler.object_instance_set
             ]
 
         target_refs: Dict[str, str] = {}
 
-        # sample targets
+        # sample goal positions for target objects after all other clutter is placed and validated
         handle_to_obj = {obj.handle: obj for obj in self.ep_sampled_objects}
         for sampler_name, target_sampler in self._target_samplers.items():
             obj_sampler_name = targ_sampler_name_to_obj_sampler_names[
                 sampler_name
             ][0]
             new_target_objects = target_sampler.sample(
                 self.sim,
@@ -688,15 +724,16 @@
             extract_recep_info(x) for x in all_target_receptacles
         ]
         save_goal_receps = [
             extract_recep_info(x) for x in all_goal_receptacles
         ]
 
         name_to_receptacle = {
-            k: v.name for k, v in self.object_to_containing_receptacle.items()
+            k: v.unique_name
+            for k, v in self.object_to_containing_receptacle.items()
         }
 
         return RearrangeEpisode(
             scene_dataset_config=self.cfg.dataset_path,
             additional_obj_config_paths=self.cfg.additional_object_paths,
             episode_id=str(self.num_ep_generated - 1),
             start_position=[0, 0, 0],
@@ -733,14 +770,15 @@
             }
         }
 
         backend_cfg = habitat_sim.SimulatorConfiguration()
         backend_cfg.scene_dataset_config_file = dataset_path
         backend_cfg.scene_id = scene_name
         backend_cfg.enable_physics = True
+        backend_cfg.gpu_device_id = self.cfg.gpu_device_id
         if not self._render_debug_obs:
             # don't bother loading textures if not intending to visualize the generation process
             backend_cfg.create_renderer = False
 
         sensor_specs = []
         for sensor_uuid, sensor_params in sensors.items():
             # sensor_spec = habitat_sim.EquirectangularSensorSpec()
@@ -789,15 +827,18 @@
             "rearrange_ep_gen_output/"
             if self.vdb is None
             else self.vdb.output_path
         )
         self.vdb = DebugVisualizer(self.sim, output_path=output_path)
 
     def settle_sim(
-        self, duration: float = 5.0, make_video: bool = True
+        self,
+        target_object_names: List[str],
+        duration: float = 5.0,
+        make_video: bool = True,
     ) -> bool:
         """
         Run dynamics for a few seconds to check for stability of newly placed objects and optionally produce a video.
         Returns whether or not the simulation was stable.
         """
         if len(self.ep_sampled_objects) == 0:
             return True
@@ -888,33 +929,45 @@
                     "num_objects": 0,
                     "num_unstable_objects": 0,
                 }
             rec_num_obj_vs_unstable[rec]["num_objects"] += 1
             if obj_name in unstable_placements:
                 rec_num_obj_vs_unstable[rec]["num_unstable_objects"] += 1
         for rec, obj_in_rec in rec_num_obj_vs_unstable.items():
-            detailed_receptacle_stability_report += f"\n      receptacle '{rec.name}': ({obj_in_rec['num_unstable_objects']}/{obj_in_rec['num_objects']}) (unstable/total) objects."
+            detailed_receptacle_stability_report += f"\n      receptacle '{rec.unique_name}': ({obj_in_rec['num_unstable_objects']}/{obj_in_rec['num_objects']}) (unstable/total) objects."
 
         success = len(unstable_placements) == 0
 
+        # count unstable target objects, these can't be salvaged
+        unstable_target_objects = [
+            obj_name
+            for obj_name in unstable_placements
+            if obj_name in target_object_names
+        ]
+
         # optionally salvage the episode by removing unstable objects
-        if self.cfg.correct_unstable_results and not success:
+        if (
+            self.cfg.correct_unstable_results
+            and not success
+            and len(unstable_target_objects) == 0
+        ):
             detailed_receptacle_stability_report += (
                 "\n  attempting to correct unstable placements..."
             )
             for sampler_name, objects in self.episode_data[
                 "sampled_objects"
             ].items():
                 obj_names = [obj.handle for obj in objects]
                 sampler = self._obj_samplers[sampler_name]
                 unstable_subset = [
                     obj_name
                     for obj_name in unstable_placements
                     if obj_name in obj_names
                 ]
+
                 # check that we have freedom to reject some objects
                 num_required_objects = sampler.num_objects[0]
                 num_stable_objects = len(objects) - len(unstable_subset)
                 if num_stable_objects >= num_required_objects:
                     # remove the unstable objects from datastructures
                     self.episode_data["sampled_objects"][sampler_name] = [
                         obj
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/run_episode_generator.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/run_episode_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,24 +39,24 @@
     comment: str = ""
 
 
 @dataclass
 class RearrangeEpisodeGeneratorConfig:
     # The minimum distance from the target object starting position to its goal
     min_dist_from_start_to_goal: float = 0.5
+    gpu_device_id: int = 0
     # ----- import/initialization parameters ------
     # the scene dataset from which scenes and objects are sampled
     dataset_path: str = "data/replica_cad/replicaCAD.scene_dataset_config.json"
     # any additional object assets to load before defining object sets
     additional_object_paths: List[str] = field(
         default_factory=lambda: ["data/objects/ycb/"]
     )
     # optionally correct unstable states by removing extra unstable objects (within minimum samples limitations)
-    # TODO: This option is off by default for backwards compatibility and because it does not yet work with target sampling.
-    correct_unstable_results: bool = False
+    correct_unstable_results: bool = True
     # ----- resource set definitions ------
     # Define the sets of scenes, objects, and receptacles which can be sampled from.
     # The SceneDataset will be searched for resources of each type with handles containing ANY "included" substrings and NO "excluded" substrings.
 
     # Define sets of scene instance handles which can be sampled from for initialization:
     scene_sets: List[Any] = field(
         default_factory=lambda: [
@@ -117,16 +117,18 @@
     # receptacle. To allow only two objects in the chair, specify:
     # - ["receptacle_aabb_Chr1_Top1_frl_apartment_chair_01", 2]
     max_objects_per_receptacle: List[Any] = field(default_factory=list)
 
     # Define the object sampling configuration
     object_samplers: List[Any] = field(default_factory=list)
     # {"name":str, "type:str", "params":{})
-    # - uniform sampler params: {"object_sets":[str], "receptacle_sets":[str], "num_samples":[min, max], "orientation_sampling":str)
+    # - uniform sampler params: {"object_sets":[str], "receptacle_sets":[str], "num_samples":[min, max], "orientation_sampling":str, "nav_to_min_distance":float, "constrain_to_largest_nav_island":bool)
     # NOTE: "orientation_sampling" options: "none", "up", "all"
+    # NOTE: (optional) "constrain_to_largest_nav_island" (default False): if True, valid placements must snap to the largest navmesh island
+    # NOTE: (optional) "nav_to_min_distance" (default -1): if not -1, valid placements must snap to the navmesh with horizontal distance less than this value
     # TODO: convert some special examples to yaml:
     # (
     #     "fridge_middle",
     #     "uniform",
     #     (["any"], ["fridge_middle"], 1, 30, "up"),
     # ),
     # Composite object sampling (e.g. apple in bowl)
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/art_sampler.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/art_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/object_sampler.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_sampler.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,33 +23,45 @@
     find_receptacles,
 )
 from habitat.sims.habitat_simulator.debug_visualizer import DebugVisualizer
 
 
 class ObjectSampler:
     """
-    Sample an object from a set and try to place it in the scene from some receptacle set.
+    Sample an object from a set and try to place it in the scene on a Receptacles from some Receptacle set.
     """
 
     def __init__(
         self,
         object_set: List[str],
         allowed_recep_set_names: List[str],
         num_objects: Tuple[int, int] = (1, 1),
         orientation_sample: Optional[str] = None,
         sample_region_ratio: Optional[Dict[str, float]] = None,
         nav_to_min_distance: float = -1.0,
         recep_set_sample_probs: Optional[Dict[str, float]] = None,
+        translation_up_offset: float = 0.08,
+        constrain_to_largest_nav_island: bool = False,
     ) -> None:
         """
+        :param object_set: The set objects from which placements will be sampled.
+        :param allowed_recep_set_names:
+        :param num_objects: The [minimum, maximum] number of objects for this sampler. Actual target value for the sampler will be uniform random number in this range.
+        :param orientation_sample: Optionally choose to sample object orientation as well as position. Options are: None, "up" (1D), "all" (rand quat).
+        :param sample_region_ratio: Defines a XZ scaling of the sample region around its center. Default no scaling. Enables shrinking aabb receptacles away from edges.
         :param nav_to_min_distance: -1.0 means there will be no accessibility constraint. Positive values indicate minimum distance from sampled object to a navigable point.
+        :param recep_set_sample_probs: Optionally provide a non-uniform weighting for receptacle sampling.
+        :param translation_up_offset: Optionally offset sample points to improve likelyhood of successful placement on inflated collision shapes.
+        :param check_if_in_largest_island_id: Optionally check if the snapped point is in the largest island id
         """
         self.object_set = object_set
         self._allowed_recep_set_names = allowed_recep_set_names
         self._recep_set_sample_probs = recep_set_sample_probs
+        self._translation_up_offset = translation_up_offset
+        self._constrain_to_largest_nav_island = constrain_to_largest_nav_island
 
         self.receptacle_instances: Optional[
             List[Receptacle]
         ] = None  # all receptacles in the scene
         self.receptacle_candidates: Optional[
             List[Receptacle]
         ] = None  # the specific receptacle instances relevant to this sampler
@@ -61,38 +73,46 @@
             orientation_sample  # None, "up" (1D), "all" (rand quat)
         )
         if sample_region_ratio is None:
             sample_region_ratio = defaultdict(lambda: 1.0)
         self.sample_region_ratio = sample_region_ratio
         self.nav_to_min_distance = nav_to_min_distance
         self.set_num_samples()
+        self.largest_island_id = -1
         # More possible parameters of note:
         # - surface vs volume
         # - apply physics stabilization: none, dynamic, projection
 
     def reset(self) -> None:
         """
         Reset any per-scene variables.
         """
         # receptacle instances should be scraped for every new scene
         self.receptacle_instances = None
         self.receptacle_candidates = None
         # number of objects in the range should be reset each time
         self.set_num_samples()
+        self.largest_island_id = -1
 
     def sample_receptacle(
         self,
         sim: habitat_sim.Simulator,
         recep_tracker: ReceptacleTracker,
         cull_tilted_receptacles: bool = True,
         tilt_tolerance: float = 0.9,
     ) -> Receptacle:
         """
         Sample a receptacle from the receptacle_set and return relevant information.
-        If cull_tilted_receptacles is True, receptacles are culled for objects with local "down" (-Y), not aligned with gravity (unit dot product compared to tilt_tolerance).
+
+        :param sim: The active Simulator instance.
+        :param recep_tracker: The pre-initialized ReceptacleTracker object defining available ReceptacleSets.
+        :param cull_tilted_receptacles: Whether or not to remove tilted Receptacles from the candidate set.
+        :param tilt_tolerance: If cull_tilted_receptacles is True, receptacles are culled for objects with local "down" (-Y), not aligned with gravity (unit dot product compared to tilt_tolerance).
+
+        :return: The sampled Receptacle. AssertionError if no valid Receptacle candidates are found.
         """
         if self.receptacle_instances is None:
             self.receptacle_instances = find_receptacles(sim)
 
         match_recep_sets = [
             recep_tracker.recep_sets[k] for k in self._allowed_recep_set_names
         ]
@@ -126,41 +146,41 @@
                     ):
                         if ex_object_substr in receptacle.parent_object_handle:
                             culled = True
                             break
                     for (
                         ex_receptacle_substr
                     ) in receptacle_set.excluded_receptacle_substrings:
-                        if ex_receptacle_substr in receptacle.name:
+                        if ex_receptacle_substr in receptacle.unique_name:
                             culled = True
                             break
                     if culled:
                         break
 
                     # if the receptacle is stage/global (no object handle) then always a match
                     if receptacle.parent_object_handle is None:
                         # check the inclusion name constraints
                         for (
                             name_constraint
                         ) in receptacle_set.included_receptacle_substrings:
-                            if name_constraint in receptacle.name:
+                            if name_constraint in receptacle.unique_name:
                                 found_match = True
                                 break
                         break
 
                     # then search for inclusion
                     for (
                         object_substr
                     ) in receptacle_set.included_object_substrings:
                         if object_substr in receptacle.parent_object_handle:
                             # object substring is valid, try receptacle name constraint
                             for (
                                 name_constraint
                             ) in receptacle_set.included_receptacle_substrings:
-                                if name_constraint in receptacle.name:
+                                if name_constraint in receptacle.unique_name:
                                     # found a valid substring match for this receptacle, stop the search
                                     found_match = True
                                     break
                         if found_match:
                             # break object substr search
                             break
                     if found_match:
@@ -177,15 +197,15 @@
                         )
                         gravity_alignment = mn.math.dot(
                             obj_down, sim.get_gravity().normalized()
                         )
                         if gravity_alignment < tilt_tolerance:
                             culled = True
                             logger.info(
-                                f"Culled by tilt: '{receptacle.name}', {gravity_alignment}"
+                                f"Culled by tilt: '{receptacle.unique_name}', {gravity_alignment}"
                             )
                     if not culled:
                         # found a valid receptacle
                         self.receptacle_candidates.append(receptacle)
 
         assert (
             len(self.receptacle_candidates) > 0
@@ -207,31 +227,49 @@
         object_handle: str,
         receptacle: Receptacle,
         snap_down: bool = False,
         vdb: Optional[DebugVisualizer] = None,
     ) -> Optional[habitat_sim.physics.ManagedRigidObject]:
         """
         Attempt to sample a valid placement of the object in/on a receptacle given an object handle and receptacle information.
+
+        :param sim: The active Simulator instance.
+        :param object_handle: The handle of the object template for instantiation and attempted placement.
+        :param receptacle: The Receptacle instance on which to sample a placement position.
+        :param snap_down: Whether or not to use the snap_down utility to place the object.
+        :param vdb: Optionally provide a debug visualizer (vdb)
+
+        :return: The newly instanced rigid object or None if placement sampling failed.
         """
         num_placement_tries = 0
         new_object = None
-        navmesh_vertices = np.stack(
-            sim.pathfinder.build_navmesh_vertices(), axis=0
-        )
-        # Note: we cache the largest island to reject samples which are primarily accessible from disconnected navmesh regions. This assumption limits sampling to the largest navigable component of any scene.
-        self.largest_island_size = max(
-            [sim.pathfinder.island_radius(p) for p in navmesh_vertices]
-        )
+
+        # Note: we cache the largest island ID to reject samples which are primarily accessible from disconnected navmesh regions.
+        # This assumption limits sampling to the largest navigable component of any scene.
+        if (
+            self._constrain_to_largest_nav_island
+            and self.largest_island_id == -1
+        ):
+            island_areas = list(
+                map(
+                    sim.pathfinder.island_area,
+                    range(sim.pathfinder.num_islands),
+                )
+            )
+            self.largest_island_id = island_areas.index(max(island_areas))
 
         while num_placement_tries < self.max_placement_attempts:
             num_placement_tries += 1
 
             # sample the object location
-            target_object_position = receptacle.sample_uniform_global(
-                sim, self.sample_region_ratio[receptacle.name]
+            target_object_position = (
+                receptacle.sample_uniform_global(
+                    sim, self.sample_region_ratio[receptacle.name]
+                )
+                + self._translation_up_offset * receptacle.up
             )
 
             # instance the new potential object from the handle
             if new_object == None:
                 assert sim.get_object_template_manager().get_library_has_handle(
                     object_handle
                 ), f"Found no object in the SceneDataset with handle '{object_handle}'."
@@ -301,124 +339,171 @@
                     continue
                 return new_object
 
         # if num_placement_tries > self.max_placement_attempts:
         sim.get_rigid_object_manager().remove_object_by_handle(
             new_object.handle
         )
-        logger.warning(
-            f"Failed to sample {object_handle} placement on {receptacle.name} in {self.max_placement_attempts} tries."
+        logger.info(
+            f"Failed to sample {object_handle} placement on {receptacle.unique_name} in {self.max_placement_attempts} tries."
         )
 
         return None
 
-    def _is_accessible(self, sim, new_object) -> bool:
+    def _is_accessible(
+        self,
+        sim: habitat_sim.Simulator,
+        obj: habitat_sim.physics.ManagedRigidObject,
+    ) -> bool:
         """
-        Return if the object is within a threshold distance of the nearest
-        navigable point and that the nearest navigable point is on the same
-        navigation mesh.
-
-        Note that this might not catch all edge cases since the distance is
-        based on Euclidean distance. The nearest navigable point may be
-        separated from the object by an obstacle.
+        Return if the object is within a threshold horizontal distance of the nearest
+        navigable point, in which the nearest navigable point is on the same
+        navigation mesh of the object.
+
+        Note that this might not catch all edge cases since the heuristic is
+        horizontal Euclidean distance. The nearest navigable point may be
+        separated from the object by an obstacle on a stairway, etc...
         """
         if self.nav_to_min_distance == -1:
             return True
-        snapped = sim.pathfinder.snap_point(new_object.translation)
-        island_radius: float = sim.pathfinder.island_radius(snapped)
-        dist = float(
-            np.linalg.norm(
-                np.array((snapped - new_object.translation))[[0, 2]]
-            )
+
+        # If the sanp_point fails, the sanpped point is NaN and the distance
+        # check returns False. So it works out.
+        snapped = sim.pathfinder.snap_point(
+            obj.translation, self.largest_island_id
         )
-        return (
-            dist < self.nav_to_min_distance
-            and island_radius == self.largest_island_size
+        horizontal_dist = float(
+            np.linalg.norm(np.array((snapped - obj.translation))[[0, 2]])
         )
+        return horizontal_dist < self.nav_to_min_distance
 
     def single_sample(
         self,
         sim: habitat_sim.Simulator,
         recep_tracker: ReceptacleTracker,
         snap_down: bool = False,
         vdb: Optional[DebugVisualizer] = None,
         fixed_target_receptacle=None,
         fixed_obj_handle: Optional[str] = None,
     ) -> Optional[habitat_sim.physics.ManagedRigidObject]:
+        """
+        Sample a single object placement by first sampling a Receptacle candidate, then an object, then attempting to place that object on the Receptacle.
+
+        :param sim: The active Simulator instance.
+        :param recep_tracker: The pre-initialized ReceptacleTracker instace containg active ReceptacleSets.
+        :param snap_down: Whether or not to use the snap_down utility to place the objects.
+        :param vdb: Optionally provide a debug visualizer (vdb)
+        :param fixed_target_receptacle: Optionally provide a pre-selected Receptacle instead of sampling. For example, when a target object's receptacle is selected in advance.
+        :param fixed_obj_handle: Optionally provide a pre-selected object instead of sampling. For example, when sampling the goal position for a known target object.
+
+        :return: The newly instanced rigid object or None if sampling failed.
+        """
         # draw a new pairing
         if fixed_obj_handle is None:
             object_handle = self.sample_object()
         else:
             object_handle = fixed_obj_handle
+
         if fixed_target_receptacle is not None:
             target_receptacle = fixed_target_receptacle
         else:
             target_receptacle = self.sample_receptacle(sim, recep_tracker)
         logger.info(
-            f"Sampling '{object_handle}' from '{target_receptacle.name}'"
+            f"Sampling '{object_handle}' from '{target_receptacle.unique_name}'"
         )
 
         new_object = self.sample_placement(
             sim, object_handle, target_receptacle, snap_down, vdb
         )
 
         return new_object, target_receptacle
 
-    def set_num_samples(self):
+    def set_num_samples(self) -> None:
+        """
+        Choose a target number of objects to sample from the configured range.
+        """
         self.target_objects_number = (
             random.randrange(self.num_objects[0], self.num_objects[1])
             if self.num_objects[1] > self.num_objects[0]
             else self.num_objects[0]
         )
 
     def sample(
         self,
         sim: habitat_sim.Simulator,
         recep_tracker: ReceptacleTracker,
-        target_receptacles,
+        target_receptacles: List[Receptacle],
         snap_down: bool = False,
         vdb: Optional[DebugVisualizer] = None,
-    ) -> List[habitat_sim.physics.ManagedRigidObject]:
+        target_object_handles: Optional[List[str]] = None,
+        object_idx_to_recep: Optional[Dict[int, Receptacle]] = None,
+    ) -> List[Tuple[habitat_sim.physics.ManagedRigidObject, Receptacle]]:
         """
         Defaults to uniform sample: object -> receptacle -> volume w/ rejection -> repeat.
-        Optionally provide a debug visualizer (vdb)
+
+        :param sim: The active Simulator instance.
+        :param recep_tracker: The pre-initialized ReceptacleTracker instace containg active ReceptacleSets.
+        :param target_receptacles: A list of pre-selected Receptacles for target object placement. These will be sampled first.
+        :param snap_down: Whether or not to use the snap_down utility to place the objects.
+        :param vdb: Optionally provide a debug visualizer (vdb)
+
+        :return: The list of new (object,receptacle) pairs placed by the sampler.
         """
         num_pairing_tries = 0
-        new_objects: List[habitat_sim.physics.ManagedRigidObject] = []
+        new_objects: List[
+            Tuple[habitat_sim.physics.ManagedRigidObject, Receptacle]
+        ] = []
+        if object_idx_to_recep is None:
+            object_idx_to_recep = {}
 
         logger.info(
             f"    Trying to sample {self.target_objects_number} from range {self.num_objects}"
         )
 
         sampling_start_time = time.time()
         pairing_start_time = sampling_start_time
         while (
             len(new_objects) < self.target_objects_number
             and num_pairing_tries < self.max_sample_attempts
         ):
+            cur_obj_idx = len(new_objects)
+            if target_object_handles is None:
+                fixed_obj_handle = None
+            else:
+                fixed_obj_handle = target_object_handles[cur_obj_idx]
+
             num_pairing_tries += 1
             if len(new_objects) < len(target_receptacles):
-                # no objects sampled yet
+                # sample objects explicitly from pre-designated target receptacles first
                 new_object, receptacle = self.single_sample(
                     sim,
                     recep_tracker,
                     snap_down,
                     vdb,
-                    target_receptacles[len(new_objects)],
+                    target_receptacles[cur_obj_idx],
+                    fixed_obj_handle=fixed_obj_handle,
                 )
                 # This receptacle has already been counted in the receptacle
                 # tracking so don't double count.
             else:
                 new_object, receptacle = self.single_sample(
-                    sim, recep_tracker, snap_down, vdb
+                    sim,
+                    recep_tracker,
+                    snap_down,
+                    vdb,
+                    fixed_target_receptacle=object_idx_to_recep.get(
+                        cur_obj_idx, None
+                    ),
+                    fixed_obj_handle=fixed_obj_handle,
                 )
                 if (
                     new_object is not None
-                    and recep_tracker.update_receptacle_tracking(receptacle)
+                    and recep_tracker.allocate_one_placement(receptacle)
                 ):
+                    # used up receptacle, need to recompute the sampler's receptacle_candidates
                     self.receptacle_candidates = None
 
             if new_object is not None:
                 # when an object placement is successful, reset the try counter.
                 logger.info(
                     f"    found obj|receptacle pairing ({len(new_objects)}/{self.target_objects_number}) in {num_pairing_tries} attempts ({time.time()-pairing_start_time}sec)."
                 )
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/object_target_sampler.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_target_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/receptacle.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/receptacle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+import json
 import os
 import random
 from abc import ABC, abstractmethod
-from collections import namedtuple
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
+import corrade as cr
 import magnum as mn
 import numpy as np
 
 import habitat_sim
 from habitat.core.logging import logger
 from habitat.sims.habitat_simulator.sim_utilities import add_wire_box
 from habitat.utils.geometry_utils import random_triangle_point
 
+# global module singleton for mesh importing instantiated upon first import
+_manager = mn.trade.ImporterManager()
+
 
 class Receptacle(ABC):
     """
     Defines a volume or surface for sampling object placements within a scene.
     Receptacles can be attached to rigid and articulated objects or defined in the global space of a stage or scene.
     Receptacle metadata should be defined in the SceneDataset in object_config.json, ao_config.json, and stage_config.json, and scene_config.json files or added programmatically to associated Attributes objects.
     To define a Receptacle within a JSON metadata file, add a new subgroup with a key beginning with "receptacle_" to the "user_defined" JSON subgroup. See ReplicaCAD v1.2+ for examples.
@@ -50,14 +54,23 @@
         assert (
             len(nonzero_indices) == 1
         ), "The 'up' vector must be aligned with a primary axis for an AABB."
         self.up_axis = nonzero_indices[0]
         self.parent_object_handle = parent_object_handle
         self.parent_link = parent_link
 
+        # The unique name of this Receptacle instance in the current scene.
+        # This name is a combination of the object instance name and Receptacle name.
+        self.unique_name = ""
+        if self.parent_object_handle is None:
+            # this is a stage receptacle
+            self.unique_name = "stage|" + self.name
+        else:
+            self.unique_name = self.parent_object_handle + "|" + self.name
+
     @property
     def is_parent_object_articulated(self):
         """
         Convenience query for articulated vs. rigid object check.
         """
         return self.parent_link is not None
 
@@ -296,21 +309,14 @@
         dblr = sim.get_debug_line_render()
         dblr.push_transform(self.get_global_transform(sim))
         dblr.draw_box(self.bounds.min, self.bounds.max, color)
         dblr.pop_transform()
         # TODO: test this
 
 
-# TriangleMeshData "vertices":List[mn.Vector3] "indices":List[int]
-TriangleMeshData = namedtuple(
-    "TriangleMeshData",
-    "vertices indices",
-)
-
-
 def assert_triangles(indices: List[int]) -> None:
     """
     Assert that an index array is divisible by 3 as a heuristic for triangle-only faces.
     """
     assert (
         len(indices) % 3 == 0
     ), "TriangleMeshReceptacles must be exclusively composed of triangles. The provided mesh_data is not."
@@ -321,24 +327,24 @@
     Defines a Receptacle surface as a triangle mesh.
     TODO: configurable maximum height.
     """
 
     def __init__(
         self,
         name: str,
-        mesh_data: TriangleMeshData,  # vertices, indices
+        mesh_data: mn.trade.MeshData,
         parent_object_handle: str = None,
         parent_link: Optional[int] = None,
         up: Optional[mn.Vector3] = None,
     ) -> None:
         """
         Initialize the TriangleMeshReceptacle from mesh data and pre-compute the area weighted accumulator.
 
         :param name: The name of the Receptacle. Should be unique and descriptive for any one object.
-        :param mesh_data: The Receptacle's mesh data. A Tuple of two Lists, first vertex geometry (Vector3) and second topology (indicies of triangle corner verts(int) (len divisible by 3)).
+        :param mesh_data: The Receptacle's mesh data. A magnum.trade.MeshData object (indices len divisible by 3).
         :param parent_object_handle: The rigid or articulated object instance handle for the parent object to which the Receptacle is attached. None for globally defined stage Receptacles.
         :param parent_link: Index of the link to which the Receptacle is attached if the parent is an ArticulatedObject. -1 denotes the base link. None for rigid objects and stage Receptables.
         :param up: The "up" direction of the Receptacle in local AABB space. Used for optionally culling receptacles in un-supportive states such as inverted surfaces.
         """
         super().__init__(name, parent_object_handle, parent_link, up)
         self.mesh_data = mesh_data
         self.area_weighted_accumulator = (
@@ -349,40 +355,38 @@
         # pre-compute the normalized cumulative area of all triangle faces for later sampling
         self.total_area = 0.0
         for f_ix in range(int(len(mesh_data.indices) / 3)):
             v = self.get_face_verts(f_ix)
             w1 = v[1] - v[0]
             w2 = v[2] - v[1]
             self.area_weighted_accumulator.append(
-                0.5 * float(np.linalg.norm(np.cross(w1, w2)))
+                0.5 * mn.math.cross(w1, w2).length()
             )
             self.total_area += self.area_weighted_accumulator[-1]
         for f_ix in range(len(self.area_weighted_accumulator)):
             self.area_weighted_accumulator[f_ix] = (
                 self.area_weighted_accumulator[f_ix] / self.total_area
             )
             if f_ix > 0:
                 self.area_weighted_accumulator[
                     f_ix
                 ] += self.area_weighted_accumulator[f_ix - 1]
 
-    def get_face_verts(self, f_ix: int) -> List[np.ndarray]:
+    def get_face_verts(self, f_ix: int) -> List[mn.Vector3]:
         """
         Get all three vertices of a mesh triangle given it's face index as a list of numpy arrays.
 
         :param f_ix: The index of the mesh triangle.
         """
-        verts: List[np.ndarray] = []
+        verts: List[mn.Vector3] = []
         for ix in range(3):
+            index = int(f_ix * 3 + ix)
+            v_ix = self.mesh_data.indices[index]
             verts.append(
-                np.array(
-                    self.mesh_data.vertices[
-                        self.mesh_data.indices[int(f_ix * 3 + ix)]
-                    ]
-                )
+                self.mesh_data.attribute(mn.trade.MeshAttribute.POSITION)[v_ix]
             )
         return verts
 
     def sample_area_weighted_triangle(self) -> int:
         """
         Isolates the area weighted triangle sampling code.
 
@@ -501,42 +505,93 @@
                     receptacles["articulated"][urdf_handle] = []
                 receptacles["articulated"][urdf_handle].append(item)
         aom.remove_object_by_handle(ao.handle)
 
     return receptacles
 
 
-def import_tri_mesh_ply(ply_file: str) -> TriangleMeshData:
+def filter_interleave_mesh(mesh: mn.trade.MeshData) -> mn.trade.MeshData:
     """
-    Returns a Tuple of (verts,indices) from a ply mesh using magnum trade importer.
+    Filter all but position data and interleave a mesh to reduce overall memory footprint.
+    Convert triangle like primitives into triangles and assert only triangles remain.
 
-    :param ply_file: The input PLY mesh file. NOTE: must contain only triangles.
+    NOTE: Modifies the mesh data in-place
+    :return: The modified mesh for easy of use.
     """
-    manager = mn.trade.ImporterManager()
-    importer = manager.load_and_instantiate("AnySceneImporter")
-    importer.open_file(ply_file)
 
-    # TODO: We don't support mesh merging or multi-mesh parsing currently
-    if importer.mesh_count > 1:
-        raise NotImplementedError(
-            "Importing multi-mesh receptacles (mesh merging or multi-mesh parsing) is not supported."
-        )
-
-    mesh_ix = 0
-    mesh = importer.mesh(mesh_ix)
+    # convert to triangles and validate the result
+    if mesh.primitive in [
+        mn.MeshPrimitive.TRIANGLE_STRIP,
+        mn.MeshPrimitive.TRIANGLE_FAN,
+    ]:
+        mesh = mn.meshtools.generate_indices(mesh)
     assert (
         mesh.primitive == mn.MeshPrimitive.TRIANGLES
     ), "Must be a triangle mesh."
 
-    # zero-copy reference to importer datastructures
-    mesh_data = TriangleMeshData(
-        mesh.attribute(mn.trade.MeshAttribute.POSITION),
-        mesh.indices,
+    # filter out all but positions (and indices) from the mesh
+    mesh = mn.meshtools.filter_only_attributes(
+        mesh, [mn.trade.MeshAttribute.POSITION]
     )
 
+    # reformat the mesh data after filtering
+    mesh = mn.meshtools.interleave(mesh, mn.meshtools.InterleaveFlags.NONE)
+
+    return mesh
+
+
+def import_tri_mesh(mesh_file: str) -> List[mn.trade.MeshData]:
+    """
+    Returns a list of MeshData objects from a mesh asset using magnum trade importer.
+
+    :param mesh_file: The input meshes file. NOTE: must contain only triangles.
+    """
+    importer = _manager.load_and_instantiate("AnySceneImporter")
+    importer.open_file(mesh_file)
+
+    mesh_data: List[mn.trade.MeshData] = []
+
+    # import mesh data and pre-process
+    mesh_data = [
+        filter_interleave_mesh(importer.mesh(mesh_ix))
+        for mesh_ix in range(importer.mesh_count)
+    ]
+
+    # if there is a scene defined, apply any transformations
+    if importer.scene_count > 0:
+        scene_id = importer.default_scene
+        # If there's no default scene, load the first one
+        if scene_id == -1:
+            scene_id = 0
+
+        scene = importer.scene(scene_id)
+
+        # Mesh referenced by mesh_assignments[i] has a corresponding transform in
+        # mesh_transformations[i]. Association to a particular node ID is stored in
+        # scene.mapping(mn.trade.SceneField.MESH)[i], but it's not needed for anything
+        # here.
+        mesh_assignments: cr.containers.StridedArrayView1D = scene.field(
+            mn.trade.SceneField.MESH
+        )
+        mesh_transformations: List[
+            mn.Matrix4
+        ] = mn.scenetools.absolute_field_transformations3d(
+            scene, mn.trade.SceneField.MESH
+        )
+        assert len(mesh_assignments) == len(mesh_transformations)
+
+        # A mesh can be referenced by multiple nodes, so this can't operate in-place.
+        # i.e., len(mesh_data) likely changes after this step
+        mesh_data = [
+            mn.meshtools.transform3d(mesh_data[mesh_id], transformation)
+            for mesh_id, transformation in zip(
+                mesh_assignments, mesh_transformations
+            )
+        ]
+
     return mesh_data
 
 
 def parse_receptacles_from_user_config(
     user_subconfig: habitat_sim._ext.habitat_sim_bindings.Configuration,
     parent_object_handle: Optional[str] = None,
     parent_template_directory: str = "",
@@ -635,44 +690,50 @@
                 mesh_file = os.path.join(
                     parent_template_directory, sub_config.get("mesh_filepath")
                 )
                 assert os.path.exists(
                     mesh_file
                 ), f"Configured receptacle mesh asset '{mesh_file}' not found."
                 # TODO: build the mesh_data entry from scale and mesh
-                mesh_data = import_tri_mesh_ply(mesh_file)
+                mesh_data: List[mn.trade.MeshData] = import_tri_mesh(mesh_file)
 
-                receptacles.append(
-                    TriangleMeshReceptacle(
-                        name=receptacle_name,
-                        mesh_data=mesh_data,
-                        up=up,
-                        parent_object_handle=parent_object_handle,
-                        parent_link=parent_link_ix,
+                for mix, single_mesh_data in enumerate(mesh_data):
+                    single_receptacle_name = (
+                        receptacle_name + "." + str(mix).rjust(4, "0")
+                    )
+                    receptacles.append(
+                        TriangleMeshReceptacle(
+                            name=single_receptacle_name,
+                            mesh_data=single_mesh_data,
+                            up=up,
+                            parent_object_handle=parent_object_handle,
+                            parent_link=parent_link_ix,
+                        )
                     )
-                )
             else:
                 raise AssertionError(
                     f"Receptacle detected without a subtype specifier: '{mesh_receptacle_id_string}'"
                 )
 
     return receptacles
 
 
 def find_receptacles(
-    sim: habitat_sim.Simulator,
+    sim: habitat_sim.Simulator, ignore_handles: Optional[List[str]] = None
 ) -> List[Union[Receptacle, AABBReceptacle, TriangleMeshReceptacle]]:
     """
     Scrape and return a list of all Receptacles defined in the metadata belonging to the scene's currently instanced objects.
 
     :param sim: Simulator must be provided.
     """
 
     obj_mgr = sim.get_rigid_object_manager()
     ao_mgr = sim.get_articulated_object_manager()
+    if ignore_handles is None:
+        ignore_handles = []
 
     receptacles: List[
         Union[Receptacle, AABBReceptacle, TriangleMeshReceptacle]
     ] = []
 
     # search for global receptacles included with the stage
     stage_config = sim.get_stage_initialization_template()
@@ -683,27 +744,31 @@
                 stage_user_attr,
                 parent_template_directory=stage_config.file_directory,
             )
         )
 
     # rigid object receptacles
     for obj_handle in obj_mgr.get_object_handles():
+        if obj_handle in ignore_handles:
+            continue
         obj = obj_mgr.get_object_by_handle(obj_handle)
         source_template_file = obj.creation_attributes.file_directory
         user_attr = obj.user_attributes
         receptacles.extend(
             parse_receptacles_from_user_config(
                 user_attr,
                 parent_object_handle=obj_handle,
                 parent_template_directory=source_template_file,
             )
         )
 
     # articulated object receptacles
     for obj_handle in ao_mgr.get_object_handles():
+        if obj_handle in ignore_handles:
+            continue
         obj = ao_mgr.get_object_by_handle(obj_handle)
         # TODO: no way to get filepath from AO currently. Add this API.
         source_template_file = ""
         user_attr = obj.user_attributes
         receptacles.extend(
             parse_receptacles_from_user_config(
                 user_attr,
@@ -713,14 +778,22 @@
                     obj.get_link_name(link)
                     for link in range(-1, obj.num_links)
                 ],
                 ao_uniform_scaling=obj.global_scale,
             )
         )
 
+    # check for non-unique naming mistakes in user dataset
+    for rec_ix in range(len(receptacles)):
+        rec1_unique_name = receptacles[rec_ix].unique_name
+        for rec_ix2 in range(rec_ix + 1, len(receptacles)):
+            assert (
+                rec1_unique_name != receptacles[rec_ix2].unique_name
+            ), "Two Receptacles found with the same unique name '{rec1_unique_name}'. Likely indicates multiple receptacle entries with the same name in the same config."
+
     return receptacles
 
 
 @dataclass
 class ReceptacleSet:
     name: str
     included_object_substrings: List[str]
@@ -730,34 +803,92 @@
     is_on_top_of_sampler: bool = False
     comment: str = ""
 
 
 class ReceptacleTracker:
     def __init__(
         self,
-        max_objects_per_receptacle,
+        max_objects_per_receptacle: Dict[str, int],
         receptacle_sets: Dict[str, ReceptacleSet],
     ):
-        self._receptacle_counts = dict(max_objects_per_receptacle)
-        self._receptacle_sets = {
+        """
+        :param max_objects_per_receptacle: A Dict mapping receptacle unique names to the remaining number of objects allowed in the receptacle.
+        :param receptacle_sets: Dict mapping ReceptacleSet name to its dataclass.
+        """
+        self._receptacle_counts: Dict[str, int] = max_objects_per_receptacle
+        # deep copy ReceptacleSets because they may be modified by allocations
+        self._receptacle_sets: Dict[str, ReceptacleSet] = {
             k: deepcopy(v) for k, v in receptacle_sets.items()
         }
 
     @property
     def recep_sets(self) -> Dict[str, ReceptacleSet]:
         return self._receptacle_sets
 
-    def inc_count(self, recep_name):
+    def init_scene_filters(
+        self, mm: habitat_sim.metadata.MetadataMediator, scene_handle: str
+    ) -> None:
+        """
+        Initialize the scene specific filter strings from metadata.
+        Looks for a filter file defined for the scene, loads filtered strings and adds them to the exclude list of all ReceptacleSets.
+
+        :param mm: The active MetadataMediator instance from which to load the filter data.
+        :param scene_handle: The handle of the currently instantiated scene.
+        """
+        scene_user_defined = mm.get_scene_user_defined(scene_handle)
+        filtered_unique_names = []
+        if scene_user_defined is not None and scene_user_defined.has_value(
+            "scene_filter_file"
+        ):
+            scene_filter_file = scene_user_defined.get("scene_filter_file")
+            # construct the dataset level path for the filter data file
+            scene_filter_file = os.path.join(
+                os.path.dirname(mm.active_dataset), scene_filter_file
+            )
+            with open(scene_filter_file, "r") as f:
+                filter_json = json.load(f)
+                for filter_type in [
+                    "manually_filtered",
+                    "access_filtered",
+                    "stability_filtered",
+                    "height_filtered",
+                ]:
+                    for filtered_unique_name in filter_json[filter_type]:
+                        filtered_unique_names.append(filtered_unique_name)
+            # add exclusion filters to all receptacles sets
+            for r_set in self._receptacle_sets.values():
+                r_set.excluded_receptacle_substrings.extend(
+                    filtered_unique_names
+                )
+            logger.debug(
+                f"Loaded receptacle filter data for scene '{scene_handle}' from configured filter file '{scene_filter_file}'."
+            )
+
+    def inc_count(self, recep_name: str) -> None:
+        """
+        Increment allowed objects for a Receptacle.
+        :param recep_name: The unique name of the Receptacle.
+        """
         if recep_name in self._receptacle_counts:
             self._receptacle_counts[recep_name] += 1
 
-    def update_receptacle_tracking(self, new_receptacle: Receptacle):
-        recep_name = new_receptacle.name
+    def allocate_one_placement(self, allocated_receptacle: Receptacle) -> bool:
+        """
+        Record that a Receptacle has been allocated for one new object placement.
+        If the Receptacle has a configured maximum number of remaining object placements, decrement that counter.
+        If the Receptacle has no remaining allocations after this one, remove it from any existing ReceptacleSets to prevent it being sampled in the future.
+
+        :param new_receptacle: The Receptacle with a new allocated object placement.
+
+        :return: Whether or not the Receptacle has run out of remaining allocations.
+        """
+        recep_name = allocated_receptacle.unique_name
         if recep_name not in self._receptacle_counts:
             return False
+        # decrement remaining allocations
         self._receptacle_counts[recep_name] -= 1
         if self._receptacle_counts[recep_name] < 0:
             raise ValueError(f"Receptacle count for {recep_name} is invalid")
         if self._receptacle_counts[recep_name] == 0:
             for receptacle_set in self._receptacle_sets.values():
                 # Exclude this receptacle from appearing in the future.
                 if (
```

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/rearrange/samplers/scene_sampler.py` & `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/scene_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/registration.py` & `habitat-lab-0.2.520230729/habitat/datasets/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/utils.py` & `habitat-lab-0.2.520230729/habitat/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/vln/__init__.py` & `habitat-lab-0.2.520230729/habitat/datasets/vln/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/datasets/vln/r2r_vln_dataset.py` & `habitat-lab-0.2.520230729/habitat/datasets/vln/r2r_vln_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/gym/gym_definitions.py` & `habitat-lab-0.2.520230729/habitat/gym/gym_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 
 def _get_env_name(cfg: "DictConfig") -> Optional[str]:
     if "habitat" in cfg:
         cfg = cfg.habitat
     return cfg["env_task"]
 
 
-def make_gym_from_config(config: "DictConfig") -> gym.Env:
+def make_gym_from_config(config: "DictConfig", dataset=None) -> gym.Env:
     """
     From a habitat-lab or habitat-baseline config, create the associated gym environment.
     """
     if "habitat" in config:
         config = config.habitat
     env_class_name = _get_env_name(config)
     env_class = get_env_class(env_class_name)
     assert (
         env_class is not None
     ), f"No environment class with name `{env_class_name}` was found, you need to specify a valid one with env_task"
-    return make_env_fn(env_class=env_class, config=config)
+    return make_env_fn(env_class=env_class, config=config, dataset=dataset)
 
 
 def _add_sim_sensor_to_config(
     config: "DictConfig", sensor: SimulatorSensorConfig
 ):
     with read_write(config):
         sim_config = config.habitat.simulator
```

### Comparing `habitat-lab-0.2.420230405/habitat/gym/gym_env_episode_count_wrapper.py` & `habitat-lab-0.2.520230729/habitat/gym/gym_env_episode_count_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/gym/gym_env_obs_dict_wrapper.py` & `habitat-lab-0.2.520230729/habitat/gym/gym_env_obs_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/gym/gym_wrapper.py` & `habitat-lab-0.2.520230729/habitat/gym/gym_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 import gym
 import numpy as np
 from gym import spaces
 
+from habitat.core.batch_rendering.env_batch_renderer_constants import (
+    KEYFRAME_OBSERVATION_KEY,
+)
 from habitat.core.simulator import Observations
 from habitat.core.spaces import EmptySpace
+from habitat.tasks.rearrange.rearrange_sim import add_perf_timing_func
 from habitat.utils.visualizations.utils import observations_to_image
 
 if TYPE_CHECKING:
     from habitat.core.dataset import BaseEpisode
     from habitat.core.env import RLEnv
 
 try:
     import pygame
 
 except ImportError:
     pygame = None
 
-
 HabGymWrapperObsType = Union[np.ndarray, Dict[str, np.ndarray]]
 
 
 def filter_observation_space(obs_space, limit_keys):
     return spaces.Dict(
         {k: v for k, v in obs_space.spaces.items() if k in limit_keys}
     )
@@ -64,15 +67,15 @@
         # Any Box means it is continuous
         return True
     if isinstance(original_space, EmptySpace):
         return False
     if isinstance(original_space, Mapping):
         return any((_is_continuous(v) for v in original_space.values()))
     raise NotImplementedError(
-        f"Unknow action space found : {original_space}. Can only be Box or Empty"
+        f"Unknown action space found : {original_space}. Can only be Box or Empty"
     )
 
 
 def _recursive_continuous_size_getter(
     original_space: gym.Space, low: List[float], high: List[float]
 ):
     """
@@ -86,15 +89,15 @@
         low.append(-1.0)
         high.append(1.0)
     elif isinstance(original_space, Mapping):
         for v in original_space.values():
             _recursive_continuous_size_getter(v, low, high)
     else:
         raise NotImplementedError(
-            f"Unknow continuous action space found : {original_space}. Can only be Box, Empty or Dict."
+            f"Unknown continuous action space found : {original_space}. Can only be Box, Empty or Dict."
         )
 
 
 def create_action_space(original_space: gym.Space) -> gym.Space:
     """
     Converts a habitat task action space into a either continuous (Box) or discrete (Discrete) gym.space.
     """
@@ -233,15 +236,18 @@
                 env.observation_space, self._gym_achieved_goal_keys
             )
 
         if len(dict_space) > 1:
             self.observation_space = spaces.Dict(dict_space)
 
         self._screen: Optional[pygame.surface.Surface] = None
+        # Store so we can profile functions on this class.
+        self._sim = self.env._env._sim
 
+    @add_perf_timing_func()
     def step(
         self, action: Union[np.ndarray, int]
     ) -> Tuple[HabGymWrapperObsType, float, bool, dict]:
         assert self.action_space.contains(
             action
         ), f"Invalid action {action} for action space {self.action_space}"
 
@@ -283,14 +289,19 @@
             )
 
         if len(self._gym_achieved_goal_keys) > 0:
             observation["achieved_goal"] = OrderedDict(
                 [(k, obs[k]) for k in self._gym_achieved_goal_keys]
             )
 
+        if KEYFRAME_OBSERVATION_KEY in obs:
+            observation[KEYFRAME_OBSERVATION_KEY] = obs[
+                KEYFRAME_OBSERVATION_KEY
+            ]
+
         for k, v in observation.items():
             if isinstance(self.observation_space, spaces.Box):
                 observation[k] = np.concatenate(list(v.values()))
         if len(observation) == 1:
             observation = observation["observation"]
 
         return observation
```

### Comparing `habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/__init__.py` & `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from habitat.core.registry import registry
 from habitat.core.simulator import Simulator
 
-# from habitat.sims.habitat_simulator.actions import (
-#     HabitatSimV1ActionSpaceConfiguration,
-# )
-
 
 def _try_register_habitat_sim():
     try:
         import habitat_sim  # noqa: F401
 
         has_habitat_sim = True
     except ImportError as e:
         has_habitat_sim = False
         habitat_sim_import_error = e
 
-    if has_habitat_sim:
-        from habitat.sims.habitat_simulator.actions import (  # noqa: F401
-            HabitatSimV1ActionSpaceConfiguration,
-        )
-    else:
+    if not has_habitat_sim:
 
         @registry.register_simulator(name="Sim-v0")
         class HabitatSimImportError(Simulator):
             def __init__(self, *args, **kwargs):
                 raise habitat_sim_import_error
```

### Comparing `habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/debug_visualizer.py` & `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/debug_visualizer.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/habitat_simulator.py` & `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/habitat_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,26 @@
     Optional,
     Sequence,
     Set,
     Union,
     cast,
 )
 
+import magnum as mn
 import numpy as np
 from gym import spaces
 from gym.spaces.box import Box
 from omegaconf import DictConfig
 
 import habitat_sim
 from habitat.config.default import get_agent_config
+from habitat.core.batch_rendering.env_batch_renderer_constants import (
+    KEYFRAME_OBSERVATION_KEY,
+    KEYFRAME_SENSOR_PREFIX,
+)
 from habitat.core.dataset import Episode
 from habitat.core.registry import registry
 from habitat.core.simulator import (
     AgentState,
     DepthSensor,
     Observations,
     RGBSensor,
@@ -334,17 +339,28 @@
                 "start_rotation",
                 "articulated_agent_urdf",
                 "articulated_agent_type",
                 "joint_start_noise",
                 "motion_data_path",
                 "ik_arm_urdf",
                 "grasp_managers",
+                "joint_start_override",
             },
         )
 
+        # configure default navmesh parameters to match the configured agent
+        if self.habitat_config.default_agent_navmesh:
+            sim_config.navmesh_settings = habitat_sim.nav.NavMeshSettings()
+            sim_config.navmesh_settings.set_defaults()
+            sim_config.navmesh_settings.agent_radius = agent_config.radius
+            sim_config.navmesh_settings.agent_height = agent_config.height
+            sim_config.navmesh_settings.include_static_objects = (
+                self.habitat_config.navmesh_include_static_objects
+            )
+
         sensor_specifications = []
         for sensor in _sensor_suite.sensors.values():
             assert isinstance(sensor, HabitatSimSensor)
             sim_sensor_cfg = sensor._get_default_spec()  # type: ignore[operator]
             overwrite_config(
                 config_from=sensor.config,
                 config_to=sim_sensor_cfg,
@@ -372,19 +388,42 @@
             sim_sensor_cfg.sensor_type = sensor.sim_sensor_type
             sim_sensor_cfg.gpu2gpu_transfer = (
                 self.habitat_config.habitat_sim_v0.gpu_gpu
             )
             sensor_specifications.append(sim_sensor_cfg)
 
         agent_config.sensor_specifications = sensor_specifications
-        agent_config.action_space = registry.get_action_space_configuration(
-            self.habitat_config.action_space_config
-        )(self.habitat_config).get()
 
-        return habitat_sim.Configuration(sim_config, [agent_config])
+        agent_config.action_space = {
+            0: habitat_sim.ActionSpec("stop"),
+            1: habitat_sim.ActionSpec(
+                "move_forward",
+                habitat_sim.ActuationSpec(
+                    amount=self.habitat_config.forward_step_size
+                ),
+            ),
+            2: habitat_sim.ActionSpec(
+                "turn_left",
+                habitat_sim.ActuationSpec(
+                    amount=self.habitat_config.turn_angle
+                ),
+            ),
+            3: habitat_sim.ActionSpec(
+                "turn_right",
+                habitat_sim.ActuationSpec(
+                    amount=self.habitat_config.turn_angle
+                ),
+            ),
+        }
+
+        output = habitat_sim.Configuration(sim_config, [agent_config])
+        output.enable_batch_renderer = (
+            self.habitat_config.renderer.enable_batch_renderer
+        )
+        return output
 
     @property
     def sensor_suite(self) -> SensorSuite:
         return self._sensor_suite
 
     @property
     def action_space(self) -> Space:
@@ -408,31 +447,45 @@
 
     def reset(self) -> Observations:
         sim_obs = super().reset()
         if self._update_agents_state():
             sim_obs = self.get_sensor_observations()
 
         self._prev_sim_obs = sim_obs
-        return self._sensor_suite.get_observations(sim_obs)
+        if self.config.enable_batch_renderer:
+            self.add_keyframe_to_observations(sim_obs)
+            return sim_obs
+        else:
+            return self._sensor_suite.get_observations(sim_obs)
 
-    def step(self, action: Union[str, np.ndarray, int]) -> Observations:
-        sim_obs = super().step(action)
+    def step(
+        self, action: Optional[Union[str, np.ndarray, int]]
+    ) -> Observations:
+        if action is None:
+            sim_obs = self.get_sensor_observations()
+        else:
+            sim_obs = super().step(action)
         self._prev_sim_obs = sim_obs
-        observations = self._sensor_suite.get_observations(sim_obs)
-        return observations
+        if self.config.enable_batch_renderer:
+            self.add_keyframe_to_observations(sim_obs)
+            return sim_obs
+        else:
+            return self._sensor_suite.get_observations(sim_obs)
 
     def render(self, mode: str = "rgb") -> Any:
         r"""
         Args:
             mode: sensor whose observation is used for returning the frame,
                 eg: "rgb", "depth", "semantic"
 
         Returns:
             rendered frame according to the mode
         """
+        assert not self.config.enable_batch_renderer
+
         sim_obs = self.get_sensor_observations()
         observations = self._sensor_suite.get_observations(sim_obs)
 
         output = observations.get(mode)
         assert output is not None, "mode {} sensor is not active".format(mode)
         if not isinstance(output, np.ndarray):
             # If it is not a numpy array, it is a torch tensor
@@ -646,13 +699,35 @@
     def previous_step_collided(self):
         r"""Whether or not the previous step resulted in a collision
 
         Returns:
             bool: True if the previous step resulted in a collision, false otherwise
 
         Warning:
-            This feild is only updated when :meth:`step`, :meth:`reset`, or :meth:`get_observations_at` are
-            called.  It does not update when the agent is moved to a new loction.  Furthermore, it
+            This field is only updated when :meth:`step`, :meth:`reset`, or :meth:`get_observations_at` are
+            called.  It does not update when the agent is moved to a new location.  Furthermore, it
             will _always_ be false after :meth:`reset` or :meth:`get_observations_at` as neither of those
             result in an action (step) being taken.
         """
         return self._prev_sim_obs.get("collided", False)
+
+    def add_keyframe_to_observations(self, observations):
+        r"""Adds an item to observations that contains the latest gfx-replay keyframe.
+        This is used to communicate the state of concurrent simulators to the batch renderer between processes.
+
+        :param observations: Original observations upon which the keyframe is added.
+        """
+        assert self.config.enable_batch_renderer
+
+        assert KEYFRAME_OBSERVATION_KEY not in observations
+        for _sensor_uuid, sensor in self._sensors.items():
+            node = sensor._sensor_object.node
+            transform = node.absolute_transformation()
+            rotation = mn.Quaternion.from_matrix(transform.rotation())
+            self.gfx_replay_manager.add_user_transform_to_keyframe(
+                KEYFRAME_SENSOR_PREFIX + _sensor_uuid,
+                transform.translation,
+                rotation,
+            )
+        observations[
+            KEYFRAME_OBSERVATION_KEY
+        ] = self.gfx_replay_manager.extract_keyframe()
```

### Comparing `habitat-lab-0.2.420230405/habitat/sims/habitat_simulator/sim_utilities.py` & `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/sim_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,21 +147,21 @@
     :param check_all_corners: Optionally cast rays from all bounding box corners instead of only casting a ray from the center of mass.
     """
     if support_obj_ids is None:
         # set default support surface to stage/ground mesh
         support_obj_ids = [-1]
     lowest_key_point: mn.Vector3 = None
     lowest_key_point_height = None
-    highest_support_impact: mn.Vector3 = None
+    highest_support_impact: Optional[mn.Vector3] = None
     highest_support_impact_height = None
-    highest_support_impact_with_stage = False
+    highest_support_impact_id = None
     raycast_results = []
     gravity_dir = sim.get_gravity().normalized()
     object_local_to_global = obj.transformation
-    bb_corners = get_bb_corners(obj.collision_shape_aabb)
+    bb_corners = get_bb_corners(obj.root_scene_node.cumulative_bb)
     key_points = [mn.Vector3(0)] + bb_corners  # [COM, c0, c1 ...]
     support_impacts: Dict[int, mn.Vector3] = {}  # indexed by keypoints
     for ix, key_point in enumerate(key_points):
         world_point = object_local_to_global.transform_point(key_point)
         # NOTE: instead of explicit Y coordinate, we project onto any gravity vector
         world_point_height = world_point.projected_onto_normalized(
             -gravity_dir
@@ -177,49 +177,50 @@
             ray = habitat_sim.geo.Ray(world_point, gravity_dir)
             raycast_results.append(sim.cast_ray(ray))
             # classify any obstructions before hitting the support surface
             for hit in raycast_results[-1].hits:
                 if hit.object_id == obj.object_id:
                     continue
                 elif hit.object_id in support_obj_ids:
-                    hit_point = ray.origin + ray.direction * hit.ray_distance
+                    hit_point = hit.point
                     support_impacts[ix] = hit_point
                     support_impact_height = mn.math.dot(
                         hit_point, -gravity_dir
                     )
 
                     if (
                         highest_support_impact is None
                         or highest_support_impact_height
                         < support_impact_height
                     ):
                         highest_support_impact = hit_point
                         highest_support_impact_height = support_impact_height
-                        highest_support_impact_with_stage = hit.object_id == -1
+                        highest_support_impact_id = hit.object_id
 
                 # terminates at the first non-self ray hit
                 break
+
     # compute the relative base height of the object from its lowest bb corner and COM
     base_rel_height = (
         lowest_key_point_height
         - obj.translation.projected_onto_normalized(-gravity_dir).length()
     )
 
     # account for the affects of stage mesh margin
     # Warning: Bullet raycast on stage triangle mesh does NOT consider the margin, so explicitly consider this here.
-    margin_offset = (
-        0
-        if not highest_support_impact_with_stage
-        else sim.get_stage_initialization_template().margin
-    )
+    margin_offset = 0
+    if highest_support_impact_id is None:
+        pass
+    elif highest_support_impact_id == -1:
+        margin_offset = sim.get_stage_initialization_template().margin
 
     surface_snap_point = (
         None
         if 0 not in support_impacts
-        else support_impacts[0]
+        else highest_support_impact
         + gravity_dir * (base_rel_height - margin_offset)
     )
 
     # return list of relative base height, object position for surface snapped point, and ray results details
     return {
         "base_rel_height": base_rel_height,
         "surface_snap_point": surface_snap_point,
@@ -250,15 +251,17 @@
     """
     cached_position = obj.translation
 
     if support_obj_ids is None:
         # set default support surface to stage/ground mesh
         support_obj_ids = [-1]
 
-    bb_ray_prescreen_results = bb_ray_prescreen(sim, obj, support_obj_ids)
+    bb_ray_prescreen_results = bb_ray_prescreen(
+        sim, obj, support_obj_ids, check_all_corners=False
+    )
 
     if bb_ray_prescreen_results["surface_snap_point"] is None:
         # no support under this object, return failure
         return False
 
     # finish up
     if bb_ray_prescreen_results["surface_snap_point"] is not None:
@@ -269,15 +272,15 @@
         sim.perform_discrete_collision_detection()
         cps = sim.get_physics_contact_points()
         for cp in cps:
             if (
                 cp.object_id_a == obj.object_id
                 or cp.object_id_b == obj.object_id
             ) and (
-                (cp.contact_distance < -0.01)
+                (cp.contact_distance < -0.05)
                 or not (
                     cp.object_id_a in support_obj_ids
                     or cp.object_id_b in support_obj_ids
                 )
             ):
                 obj.translation = cached_position
                 # print(f" Failure: contact in final position w/ distance = {cp.contact_distance}.")
```

### Comparing `habitat-lab-0.2.420230405/habitat/sims/pyrobot/__init__.py` & `habitat-lab-0.2.520230729/habitat/sims/pyrobot/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/sims/pyrobot/pyrobot.py` & `habitat-lab-0.2.520230729/habitat/sims/pyrobot/pyrobot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/sims/registration.py` & `habitat-lab-0.2.520230729/habitat/sims/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/eqa/__init__.py` & `habitat-lab-0.2.520230729/habitat/tasks/eqa/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/eqa/eqa.py` & `habitat-lab-0.2.520230729/habitat/tasks/eqa/eqa.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/nav/__init__.py` & `habitat-lab-0.2.520230729/habitat/tasks/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/nav/instance_image_nav_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/nav/instance_image_nav_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/nav/nav.py` & `habitat-lab-0.2.520230729/habitat/tasks/nav/nav.py`

 * *Files 1% similar despite different names*

```diff
@@ -1036,14 +1036,32 @@
         distance_to_target = task.measurements.measures[
             DistanceToGoal.cls_uuid
         ].get_metric()
         self._metric = -(distance_to_target - self._previous_distance)
         self._previous_distance = distance_to_target
 
 
+class NavigationMovementAgentAction(SimulatorTaskAction):
+    def __init__(self, *args, config, sim, **kwargs):
+        super().__init__(*args, config=config, sim=sim, **kwargs)
+        self._sim = sim
+        self._tilt_angle = config.tilt_angle
+
+    def _move_camera_vertical(self, amount: float):
+        assert (
+            len(self._sim.agents) == 1  # type: ignore
+        ), "For navigation tasks, there can be only one agent in the scene"
+        sensor_names = list(self._sim.agents[0]._sensors.keys())  # type: ignore
+        for sensor_name in sensor_names:
+            sensor = self._sim.agents[0]._sensors[sensor_name].node  # type: ignore
+            sensor.rotation = sensor.rotation * mn.Quaternion.rotation(
+                mn.Deg(amount), mn.Vector3.x_axis()
+            )
+
+
 @registry.register_task_action
 class MoveForwardAction(SimulatorTaskAction):
     name: str = "move_forward"
 
     def step(self, *args: Any, **kwargs: Any):
         r"""Update ``_metric``, this method is called from ``Env`` on each
         ``step``.
@@ -1062,14 +1080,15 @@
 
 @registry.register_task_action
 class TurnRightAction(SimulatorTaskAction):
     def step(self, *args: Any, **kwargs: Any):
         r"""Update ``_metric``, this method is called from ``Env`` on each
         ``step``.
         """
+
         return self._sim.step(HabitatSimActions.turn_right)
 
 
 @registry.register_task_action
 class StopAction(SimulatorTaskAction):
     name: str = "stop"
 
@@ -1077,33 +1096,32 @@
         task.is_stop_called = False  # type: ignore
 
     def step(self, task: EmbodiedTask, *args: Any, **kwargs: Any):
         r"""Update ``_metric``, this method is called from ``Env`` on each
         ``step``.
         """
         task.is_stop_called = True  # type: ignore
-        return self._sim.get_observations_at()  # type: ignore
 
 
 @registry.register_task_action
-class LookUpAction(SimulatorTaskAction):
+class LookUpAction(NavigationMovementAgentAction):
     def step(self, *args: Any, **kwargs: Any):
         r"""Update ``_metric``, this method is called from ``Env`` on each
         ``step``.
         """
-        return self._sim.step(HabitatSimActions.look_up)
+        self._move_camera_vertical(self._tilt_angle)
 
 
 @registry.register_task_action
-class LookDownAction(SimulatorTaskAction):
+class LookDownAction(NavigationMovementAgentAction):
     def step(self, *args: Any, **kwargs: Any):
         r"""Update ``_metric``, this method is called from ``Env`` on each
         ``step``.
         """
-        return self._sim.step(HabitatSimActions.look_down)
+        self._move_camera_vertical(-self._tilt_angle)
 
 
 @registry.register_task_action
 class TeleportAction(SimulatorTaskAction):
     # TODO @maksymets: Propagate through Simulator class
     COORDINATE_EPSILON = 1e-6
     COORDINATE_MIN = -62.3241 - COORDINATE_EPSILON
@@ -1123,18 +1141,18 @@
         ``step``.
         """
 
         if not isinstance(rotation, list):
             rotation = list(rotation)
 
         if not self._sim.is_navigable(position):
-            return self._sim.get_observations_at()  # type: ignore
+            return
 
-        return self._sim.get_observations_at(
-            position=position, rotation=rotation, keep_agent_at_new_pose=True
+        self._sim.set_agent_state(  # type:ignore
+            position, rotation, reset_sensors=False
         )
 
     @property
     def action_space(self) -> spaces.Dict:
         return spaces.Dict(
             {
                 "position": spaces.Box(
@@ -1231,15 +1249,15 @@
 
         # Stop is called if both linear/angular speed are below their threshold
         if (
             abs(linear_velocity) < self.min_abs_lin_speed
             and abs(angular_velocity) < self.min_abs_ang_speed
         ):
             task.is_stop_called = True  # type: ignore
-            return self._sim.get_observations_at(position=None, rotation=None)
+            return
 
         angular_velocity = np.deg2rad(angular_velocity)
         self.vel_control.linear_velocity = np.array(
             [0.0, 0.0, -linear_velocity]
         )
         self.vel_control.angular_velocity = np.array(
             [0.0, angular_velocity, 0.0]
@@ -1271,39 +1289,34 @@
             agent_state.position, goal_rigid_state.translation
         )
         final_rotation = [
             *goal_rigid_state.rotation.vector,
             goal_rigid_state.rotation.scalar,
         ]
 
-        # Check if a collision occured
+        # Check if a collision occurred
         dist_moved_before_filter = (
             goal_rigid_state.translation - agent_state.position
         ).dot()
         dist_moved_after_filter = (final_position - agent_state.position).dot()
 
         # NB: There are some cases where ||filter_end - end_pos|| > 0 when a
         # collision _didn't_ happen. One such case is going up stairs.  Instead,
         # we check to see if the the amount moved after the application of the
         # filter is _less_ than the amount moved before the application of the
         # filter.
         EPS = 1e-5
         collided = (dist_moved_after_filter + EPS) < dist_moved_before_filter
 
-        agent_observations = self._sim.get_observations_at(
-            position=final_position,
-            rotation=final_rotation,
-            keep_agent_at_new_pose=True,
+        self._sim.set_agent_state(  # type:ignore
+            final_position, final_rotation, reset_sensors=False
         )
-
         # TODO: Make a better way to flag collisions
         self._sim._prev_sim_obs["collided"] = collided  # type: ignore
 
-        return agent_observations
-
 
 @registry.register_task(name="Nav-v0")
 class NavigationTask(EmbodiedTask):
     def __init__(
         self,
         config: "DictConfig",
         sim: Simulator,
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/nav/object_nav_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/nav/object_nav_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/nav/shortest_path_follower.py` & `habitat-lab-0.2.520230729/habitat/tasks/nav/shortest_path_follower.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/actions.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,36 +47,28 @@
                     high=1,
                     dtype=np.float32,
                 )
             }
         )
 
     def step(self, *args, **kwargs):
-        return self._sim.step(HabitatSimActions.empty)
+        pass
 
 
 @registry.register_task_action
 class RearrangeStopAction(SimulatorTaskAction):
     def reset(self, *args, **kwargs):
         super().reset(*args, **kwargs)
         self.does_want_terminate = False
 
-    def step(self, task, *args, is_last_action, **kwargs):
+    def step(self, task, *args, **kwargs):
         should_stop = kwargs.get("rearrange_stop", [1.0])
         if should_stop[0] > 0.0:
-            rearrange_logger.debug(
-                "Rearrange stop action requesting episode stop."
-            )
             self.does_want_terminate = True
 
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.rearrange_stop)
-        else:
-            return {}
-
 
 @registry.register_task_action
 class ArmAction(ArticulatedAgentAction):
     """An arm control and grip control into one action space."""
 
     def __init__(self, *args, config, sim: RearrangeSim, **kwargs):
         super().__init__(*args, config=config, sim=sim, **kwargs)
@@ -111,24 +103,20 @@
         }
         if self.grip_ctrlr is not None and self.grip_ctrlr.requires_action:
             action_spaces[
                 self._action_arg_prefix + "grip_action"
             ] = self.grip_ctrlr.action_space
         return spaces.Dict(action_spaces)
 
-    def step(self, is_last_action, *args, **kwargs):
+    def step(self, *args, **kwargs):
         arm_action = kwargs[self._action_arg_prefix + "arm_action"]
         self.arm_ctrlr.step(arm_action)
         if self.grip_ctrlr is not None and not self.disable_grip:
             grip_action = kwargs[self._action_arg_prefix + "grip_action"]
             self.grip_ctrlr.step(grip_action)
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.arm_action)
-        else:
-            return {}
 
 
 @registry.register_task_action
 class ArmRelPosAction(ArticulatedAgentAction):
     """
     The arm motor targets are offset by the delta joint values specified by the
     action
@@ -447,32 +435,27 @@
 
         if self.cur_articulated_agent._base_type == "leg":
             # Fix the leg joints
             self.cur_articulated_agent.leg_joint_pos = (
                 self.cur_articulated_agent.params.leg_init_params
             )
 
-    def step(self, *args, is_last_action, **kwargs):
+    def step(self, *args, **kwargs):
         lin_vel, ang_vel = kwargs[self._action_arg_prefix + "base_vel"]
         lin_vel = np.clip(lin_vel, -1, 1) * self._lin_speed
         ang_vel = np.clip(ang_vel, -1, 1) * self._ang_speed
         if not self._allow_back:
             lin_vel = np.maximum(lin_vel, 0)
 
         self.base_vel_ctrl.linear_velocity = mn.Vector3(lin_vel, 0, 0)
         self.base_vel_ctrl.angular_velocity = mn.Vector3(0, ang_vel, 0)
 
         if lin_vel != 0.0 or ang_vel != 0.0:
             self.update_base()
 
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.base_velocity)
-        else:
-            return {}
-
 
 @registry.register_task_action
 class BaseVelNonCylinderAction(ArticulatedAgentAction):
     """
     The articulated agent base motion is constrained to the NavMesh and controlled with velocity commands integrated with the VelocityControl interface.
 
     Optionally cull states with active collisions if config parameter `allow_dyn_slide` is True
@@ -606,15 +589,15 @@
 
         if self.cur_articulated_agent._base_type == "leg":
             # Fix the leg joints
             self.cur_articulated_agent.leg_joint_pos = (
                 self.cur_articulated_agent.params.leg_init_params
             )
 
-    def step(self, *args, is_last_action, **kwargs):
+    def step(self, *args, **kwargs):
         lateral_lin_vel = 0.0
         if self._enable_lateral_move:
             longitudinal_lin_vel, lateral_lin_vel, ang_vel = kwargs[
                 self._action_arg_prefix + "base_vel"
             ]
         else:
             longitudinal_lin_vel, ang_vel = kwargs[
@@ -639,19 +622,14 @@
         if (
             longitudinal_lin_vel != 0.0
             or lateral_lin_vel != 0.0
             or ang_vel != 0.0
         ):
             self.update_base(ang_vel != 0.0)
 
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.base_velocity)
-        else:
-            return {}
-
 
 @registry.register_task_action
 class ArmEEAction(ArticulatedAgentAction):
     """Uses inverse kinematics (requires pybullet) to apply end-effector position control for the articulated_agent's arm."""
 
     def __init__(self, *args, sim: RearrangeSim, **kwargs):
         self.ee_target: Optional[np.ndarray] = None
@@ -734,26 +712,24 @@
                     low=-1,
                     high=1,
                     dtype=np.float32,
                 )
             }
         )
 
-    def step(self, *args, is_last_action, **kwargs):
+    def step(self, *args, **kwargs):
         r"""
         Updates the joint rotations and root transformation of the humanoid.
         :param self._action_arg_prefix+human_joints_trans: Array of size
             (num_joints*4)+32. The last 32 dimensions define two 4x4 root
             transformation matrices, a base transform that controls the base
             of the character, and an offset transform, that controls
             a transformation offset that comes from the MOCAP pose.
             The first elements correspond to a flattened list of quaternions for each joint.
             When the array is all 0 it keeps the previous joint rotation and transform.
-        :param is_last_action: whether this is the last action before calling environment
-          step
         """
         human_joints_trans = kwargs[
             self._action_arg_prefix + "human_joints_trans"
         ]
         new_joints = human_joints_trans[:-16]
         new_pos_transform_base = human_joints_trans[-16:]
         new_pos_transform_offset = human_joints_trans[-32:-16]
@@ -776,12 +752,7 @@
                 and new_transform_base.is_rigid_transformation()
             ):
                 # TODO: this will cause many sampled actions to be invalid
                 # Maybe we should update the sampling mechanism
                 self.cur_articulated_agent.set_joint_transform(
                     new_joints, new_transform_offset, new_transform_base
                 )
-
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.humanoidjoint_action)
-        else:
-            return {}
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/articulated_agent_action.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/articulated_agent_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         else:
             self._agent_index = self._config.agent
             self._multi_agent = True
 
     @property
     def _articulated_agent_mgr(self):
         """
-        Underlying articulated_agent mananger for the articulated_agent instance the action is attached to.
+        Underlying articulated_agent manager for the articulated_agent instance the action is attached to.
         """
         return self._sim.agents_mgr[self._agent_index]
 
     @property
     def _ik_helper(self):
         """
         The IK helper for this articulated_agent instance.
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/grip_actions.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/grip_actions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/oracle_nav_action.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/oracle_nav_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import magnum as mn
 import numpy as np
 from gym import spaces
 
 import habitat_sim
 from habitat.articulated_agent_controllers import HumanoidRearrangeController
 from habitat.core.registry import registry
-from habitat.sims.habitat_simulator.actions import HabitatSimActions
 from habitat.tasks.rearrange.actions.actions import (
     BaseVelAction,
     HumanoidJointAction,
 )
 from habitat.tasks.rearrange.utils import get_robot_spawns
 from habitat.tasks.utils import get_angle
 
@@ -134,25 +133,22 @@
         path.requested_start = agent_pos
         path.requested_end = point
         found_path = self._sim.pathfinder.find_path(path)
         if not found_path:
             return [agent_pos, point]
         return path.points
 
-    def step(self, *args, is_last_action, **kwargs):
+    def step(self, *args, **kwargs):
         nav_to_target_idx = kwargs[
             self._action_arg_prefix + "oracle_nav_action"
         ]
         if nav_to_target_idx <= 0 or nav_to_target_idx > len(
             self._poss_entities
         ):
-            if is_last_action:
-                return self._sim.step(HabitatSimActions.base_velocity)
-            else:
-                return {}
+            return
         nav_to_target_idx = int(nav_to_target_idx[0]) - 1
 
         final_nav_targ, obj_targ_pos = self._get_target_for_idx(
             nav_to_target_idx
         )
         base_T = self.cur_articulated_agent.base_transformation
         curr_path_points = self._path_to_point(final_nav_targ)
@@ -199,17 +195,16 @@
                         # Look at the target waypoint.
                         vel = OracleNavAction._compute_turn(
                             rel_targ, self._config.turn_velocity, robot_forward
                         )
                 else:
                     vel = [0, 0]
                 kwargs[f"{self._action_arg_prefix}base_vel"] = np.array(vel)
-                return BaseVelAction.step(
-                    self, *args, is_last_action=is_last_action, **kwargs
-                )
+                BaseVelAction.step(self, *args, **kwargs)
+                return
 
             elif self.motion_type == "human_joints":
                 # Update the humanoid base
                 self.humanoid_controller.obj_transform_base = base_T
                 if not at_goal:
                     if dist_to_final_nav_targ < self._config.dist_thresh:
                         # Look at the object
@@ -225,14 +220,13 @@
                     self.humanoid_controller.calculate_stop_pose()
 
                 base_action = self.humanoid_controller.get_pose()
                 kwargs[
                     f"{self._action_arg_prefix}human_joints_trans"
                 ] = base_action
 
-                return HumanoidJointAction.step(
-                    self, *args, is_last_action=is_last_action, **kwargs
-                )
+                HumanoidJointAction.step(self, *args, **kwargs)
+                return
             else:
                 raise ValueError(
                     "Unrecognized motion type for oracle nav action"
                 )
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/actions/pddl_actions.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/pddl_actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,32 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import numpy as np
 from gym import spaces
 
 from habitat.core.registry import registry
-from habitat.sims.habitat_simulator.actions import HabitatSimActions
 from habitat.tasks.rearrange.actions.grip_actions import ArticulatedAgentAction
 
 
 @registry.register_task_action
 class PddlApplyAction(ArticulatedAgentAction):
     def __init__(self, *args, task, **kwargs):
+        self._action_ordering = task.pddl_problem.get_ordered_actions()
+        self._entities_list = task.pddl_problem.get_ordered_entities_list()
         super().__init__(*args, **kwargs)
         self._task = task
-        self._action_ordering = None
         self._was_prev_action_invalid = False
 
     @property
-    def action_space(self):
-        if self._action_ordering is None:
-            self._action_ordering = (
-                self._task.pddl_problem.get_ordered_actions()
-            )
-            self._entities_list = (
-                self._task.pddl_problem.get_ordered_entities_list()
-            )
+    def entities(self):
+        return self._entities_list
 
+    @property
+    def action_space(self):
         action_n_args = sum(
             [action.n_args for action in self._action_ordering]
         )
 
         return spaces.Dict(
             {
                 self._action_arg_prefix
@@ -68,17 +64,15 @@
                 real_action_idxs = [int(a) - 1 for a in action_part]
                 for a in real_action_idxs:
                     if a < 0.0:
                         raise ValueError(
                             f"Got invalid action value < 0 in {action_part} with action {action}"
                         )
 
-                param_values = [
-                    self._entities_list[i] for i in real_action_idxs
-                ]
+                param_values = [self.entities[i] for i in real_action_idxs]
 
                 # Look up the most recent version of this action.
                 apply_action = self._task.pddl_problem.actions[
                     action.name
                 ].clone()
                 apply_action.set_param_values(param_values)
                 self._prev_action = apply_action
@@ -86,21 +80,16 @@
                 if not apply_action.apply_if_true(
                     self._task.pddl_problem.sim_info
                 ):
                     self._was_prev_action_invalid = True
 
             cur_i += action.n_args
 
-    def step(self, *args, is_last_action, **kwargs):
+    def step(self, *args, **kwargs):
         self._prev_action = None
         apply_pddl_action = kwargs[self._action_arg_prefix + "pddl_action"]
         self._was_prev_action_invalid = False
         inputs_outside = any(
-            a < 0 or a > len(self._entities_list) for a in apply_pddl_action
+            a < 0 or a > len(self.entities) for a in apply_pddl_action
         )
         if not inputs_outside:
             self._apply_action(apply_pddl_action)
-
-        if is_last_action:
-            return self._sim.step(HabitatSimActions.arm_action)
-        else:
-            return {}
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/articulated_agent_manager.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/articulated_agent_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     SpotRobot,
     StretchRobot,
 )
 from habitat.articulated_agents.robots.fetch_suction import FetchSuctionRobot
 from habitat.tasks.rearrange.rearrange_grasp_manager import (
     RearrangeGraspManager,
 )
-from habitat.tasks.rearrange.utils import IkHelper, is_pb_installed
+from habitat.tasks.rearrange.utils import (
+    IkHelper,
+    add_perf_timing_func,
+    is_pb_installed,
+)
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
 
 @dataclass
 class ArticulatedAgentData:
@@ -87,42 +91,60 @@
                     for k, v in agent.params.cameras.items()
                 }
                 for camera_prefix in agent.params.cameras:
                     for sensor_name in self._sim._sensors:
                         if sensor_name.startswith(camera_prefix):
                             agent._cameras[camera_prefix].append(sensor_name)
 
+            if agent_cfg.joint_start_override is None:
+                use_arm_init = np.array(agent.params.arm_init_params)
+            else:
+                use_arm_init = np.array(agent_cfg.joint_start_override)
             self._all_agent_data.append(
                 ArticulatedAgentData(
                     articulated_agent=agent,
                     grasp_mgrs=grasp_managers,
                     cfg=agent_cfg,
-                    start_js=np.array(agent.params.arm_init_params),
+                    start_js=use_arm_init,
                     is_pb_installed=self._is_pb_installed,
                 )
             )
 
-    def reconfigure(self, is_new_scene: bool):
+    @add_perf_timing_func()
+    def on_new_scene(self) -> None:
+        """
+        Call on a new scene. This will destroy and re-create the robot
+        simulator instances.
+        """
         ao_mgr = self._sim.get_articulated_object_manager()
         for agent_data in self._all_agent_data:
-            if is_new_scene:
-                agent_data.grasp_mgr.reconfigure()
-                if (
-                    agent_data.articulated_agent.sim_obj is not None
-                    and agent_data.articulated_agent.sim_obj.is_alive
-                ):
-                    ao_mgr.remove_object_by_id(
-                        agent_data.articulated_agent.sim_obj.object_id
-                    )
+            agent_data.grasp_mgr.reconfigure()
+            if (
+                agent_data.articulated_agent.sim_obj is not None
+                and agent_data.articulated_agent.sim_obj.is_alive
+            ):
+                ao_mgr.remove_object_by_id(
+                    agent_data.articulated_agent.sim_obj.object_id
+                )
 
-                agent_data.articulated_agent.reconfigure()
+            agent_data.articulated_agent.reconfigure()
 
+    def pre_obj_clear(self) -> None:
+        """
+        Must call before all objects in the scene are removed before the next
+        episode. This will reset the grasp constraints and any references to
+        previously existing objects.
+        """
+
+        for agent_data in self._all_agent_data:
             for grasp_manager in agent_data.grasp_mgrs:
                 grasp_manager.reset()
+            agent_data.grasp_mgr.reconfigure()
 
+    @add_perf_timing_func()
     def post_obj_load_reconfigure(self):
         """
         Called at the end of the simulator reconfigure method. Used to set the starting configurations of the robots if specified in the task config.
         """
         for agent_data in self._all_agent_data:
             agent_data.articulated_agent.params.arm_init_params = (
                 agent_data.start_js
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/marker_info.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/marker_info.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/composite_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_sensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,19 +107,18 @@
         """
         # Get the next target object
         idxs, _ = self._sim.get_targets()
         targ_obj_idx = idxs[self._cur_rearrange_stage]
 
         # Get the target object's absolute index
         self.abs_targ_obj_idx = self._sim.scene_obj_ids[targ_obj_idx]
-        self.targ_obj_idx = str(targ_obj_idx)
 
     def get_distance(self, task, distance):
         return task.measurements.measures[distance.cls_uuid].get_metric()[
-            self.targ_obj_idx
+            str(self._cur_rearrange_stage)
         ]
 
     def update_metric(self, *args, episode, task, observations, **kwargs):
         super().update_metric(
             *args,
             episode=episode,
             task=task,
@@ -160,14 +159,17 @@
         # PLACE REWARD: Reward for placing the object correcly (within success dist)
         # We also udate the target object for the next stage.
 
         place_success = obj_to_goal_dist < self._config.success_dist
         if place_success and not is_holding_obj:
             self._metric += self._config.single_rearrange_reward
             self._cur_rearrange_stage += 1
+            self._cur_rearrange_stage = (
+                self._cur_rearrange_stage % self.num_targets
+            )
             if self._cur_rearrange_stage < self.num_targets:
                 self.update_target_object()
 
         # Need to call the get_distance functions again because the target
         # object may have changed in the previous if statement.
         self._prev_obj_to_goal_dist = self.get_distance(
             task, ObjectToGoalDistance
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/composite_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_action.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,44 +66,27 @@
         self._pre_cond = pre_cond
         self._post_cond = post_cond
         self._task_info = task_info
         self._post_cond_search = post_cond_search
 
     def set_post_cond_search(
         self, post_cond_search: List[Dict[PddlEntity, PddlEntity]]
-    ):
+    ) -> None:
         self._post_cond_search = post_cond_search
 
     def apply_if_true(self, sim_info: PddlSimInfo) -> bool:
         """
         Apply the action post-condition to the simulator if the action
         pre-condition is true. This will also dynamically select the right
         entities for the post-condition based on the pre-condition quantifiers.
         """
         is_sat = self._pre_cond.is_true(sim_info)
         if not is_sat:
             return False
-
-        post_conds = self._post_cond
-        if self._post_cond_search is not None:
-            found_assign = None
-            assert len(self._pre_cond.prev_truth_vals) == len(
-                self._post_cond_search
-            )
-            for sat, assign in zip(
-                self._pre_cond.prev_truth_vals, self._post_cond_search
-            ):
-                if sat:
-                    found_assign = assign
-                    break
-            # Clone and sub in so we don't overwrite the original predicates
-            post_conds = [p.clone().sub_in(found_assign) for p in post_conds]
-
-        for p in post_conds:
-            p.set_state(sim_info)
+        self.apply(sim_info)
 
         return True
 
     def get_arg_value(self, param_name: str) -> Optional[PddlEntity]:
         """
         Get the assigned value of a parameter with name `param_name`. Returns
         `None` if the parameter is not yet assigned.
@@ -135,19 +118,26 @@
         predicates ALONE.
         :param predicates: The set of predicates currently true in the
             environment.
         """
 
         return self._pre_cond.is_true_from_predicates(predicates)
 
-    def set_precond(self, new_precond):
+    def set_precond(self, new_precond) -> "PddlAction":
         """
         Sets the preconditions for the action.
         """
-        self._pre_cond = new_precond
+        return PddlAction(
+            self._name,
+            self._params,
+            new_precond,
+            self._post_cond,
+            self._task_info,
+            self._post_cond_search,
+        )
 
     @property
     def precond(self):
         return self._pre_cond
 
     @property
     def name(self):
@@ -195,16 +185,31 @@
             self._pre_cond.clone(),
             [p.clone() for p in self._post_cond],
             self._task_info,
             self._post_cond_search,
         )
 
     def apply(self, sim_info: PddlSimInfo) -> None:
-        for p in self._post_cond:
-            rearrange_logger.debug(f"Setting predicate {p}")
+        post_conds = self._post_cond
+        if self._post_cond_search is not None:
+            found_assign = None
+            assert len(self._pre_cond.prev_truth_vals) == len(
+                self._post_cond_search
+            )
+            for sat, assign in zip(
+                self._pre_cond.prev_truth_vals, self._post_cond_search
+            ):
+                if sat is not None and sat:
+                    found_assign = assign
+                    break
+            assert found_assign is not None
+            # Clone and sub in so we don't overwrite the original predicates
+            post_conds = [p.clone().sub_in(found_assign) for p in post_conds]
+
+        for p in post_conds:
             p.set_state(sim_info)
 
     @property
     def params(self) -> List[PddlEntity]:
         return self._params
 
     @property
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_domain.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import itertools
 import os.path as osp
+import time
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
@@ -57,25 +58,39 @@
     Manages the information from the PDDL domain and task definition.
     """
 
     def __init__(
         self,
         domain_file_path: str,
         cur_task_config: Optional["DictConfig"] = None,
+        read_config: bool = True,
     ):
         """
         :param domain_file_path: Either an absolute path or a path relative to `habitat/task/rearrange/multi_task/domain_configs/`.
         :param cur_task_config: The task config (`habitat.task`). This is
             used when the action initializes a task via `PddlAction::init_task`. If
             this is not used, `cur_task_config` can be None.
         """
         self._sim_info: Optional[PddlSimInfo] = None
         self._config = cur_task_config
         self._orig_actions: Dict[str, PddlAction] = {}
 
+        if read_config:
+            # Setup config properties
+            self._obj_succ_thresh = self._config.obj_succ_thresh
+            self._art_succ_thresh = self._config.art_succ_thresh
+            self._robot_at_thresh = self._config.robot_at_thresh
+            self._num_spawn_attempts = self._config.num_spawn_attempts
+            self._physics_stability_steps = (
+                self._config.physics_stability_steps
+            )
+            self._recep_place_shrink_factor = (
+                self._config.recep_place_shrink_factor
+            )
+
         if not osp.isabs(domain_file_path):
             parent_dir = osp.dirname(__file__)
             domain_file_path = osp.join(
                 parent_dir, "domain_configs", domain_file_path
             )
 
         if "." not in domain_file_path:
@@ -181,14 +196,15 @@
                     return all_entities.get(s, s)
                 else:
                     return s
 
             for k, v in robot_states.items():
                 use_k = all_entities[k]
 
+                # Sub in any referred entities.
                 v = {sub_k: fetch_entity(sub_v) for sub_k, sub_v in v.items()}
 
                 use_robot_states[use_k] = PddlRobotState(**v)
 
             set_state = PddlSimState(art_states, obj_states, use_robot_states)
 
             pred = Predicate(pred_d["name"], set_state, arg_entities)
@@ -354,56 +370,55 @@
             id_to_name[i] = k
 
         self._sim_info = PddlSimInfo(
             sim=sim,
             dataset=dataset,
             env=env,
             episode=episode,
-            obj_thresh=self._config.obj_succ_thresh,
-            art_thresh=self._config.art_succ_thresh,
-            robot_at_thresh=self._config.robot_at_thresh,
+            obj_thresh=self._obj_succ_thresh,
+            art_thresh=self._art_succ_thresh,
+            robot_at_thresh=self._robot_at_thresh,
             expr_types=self.expr_types,
             obj_ids=sim.handle_to_object_id,
             target_ids={
                 f"TARGET_{id_to_name[idx]}": idx
                 for idx in sim.get_targets()[0]
             },
             art_handles={k.handle: i for i, k in enumerate(sim.art_objs)},
             marker_handles=sim.get_all_markers(),
             robot_ids={
                 f"robot_{agent_id}": agent_id
                 for agent_id in range(sim.num_articulated_agents)
             },
             all_entities=self.all_entities,
             predicates=self.predicates,
-            num_spawn_attempts=self._config.num_spawn_attempts,
-            physics_stability_steps=self._config.physics_stability_steps,
+            num_spawn_attempts=self._num_spawn_attempts,
+            physics_stability_steps=self._physics_stability_steps,
             receptacles=sim.receptacles,
+            recep_place_shrink_factor=self._recep_place_shrink_factor,
         )
         # Ensure that all objects are accounted for.
         for entity in self.all_entities.values():
             self._sim_info.search_for_entity(entity)
 
     def bind_actions(self) -> None:
         """
         Expand all quantifiers in the actions. This should be done per instance
         bind in case the typing changes.
         """
-        for k, orig_action in self._orig_actions.items():
-            new_ac = orig_action.clone()
+        for k, ac in self._orig_actions.items():
+            precond_quant = ac.precond.quantifier
+            new_preconds, assigns = self.expand_quantifiers(ac.precond.clone())
 
-            precond_quant = new_ac.precond.quantifier
-            new_preconds, assigns = self.expand_quantifiers(
-                new_ac.precond, new_ac.name
-            )
-            new_ac.set_precond(new_preconds)
+            new_ac = ac.set_precond(new_preconds)
             if precond_quant == LogicalQuantifierType.EXISTS:
-                # So action post conditions can use the entities which satisfy
-                # the pre-conditions.
+                # So the action post conditions can use the entities which
+                # satisfy the pre-conditions.
                 new_ac.set_post_cond_search(assigns)
+
             self._actions[k] = new_ac
 
     @property
     def sim_info(self) -> PddlSimInfo:
         """
         Info from the simulator instance needed to interface the planning
         domain with the simulator. This property is used for all calls in the
@@ -431,18 +446,18 @@
         """
         Get all the predicates that are true in the current simulator state.
         """
 
         all_entities = self.all_entities.values()
         true_preds: List[Predicate] = []
         for pred in self.predicates.values():
-            for entity_input in itertools.combinations(
+            for entity_input in itertools.permutations(
                 all_entities, pred.n_args
             ):
-                if not pred.are_args_compatible(entity_input):
+                if not pred.are_args_compatible(list(entity_input)):
                     continue
 
                 use_pred = pred.clone()
                 use_pred.set_param_values(entity_input)
 
                 if use_pred.is_true(self.sim_info):
                     true_preds.append(use_pred)
@@ -566,15 +581,15 @@
         )
 
     @property
     def all_entities(self) -> Dict[str, PddlEntity]:
         return {**self._constants, **self._added_entities}
 
     def expand_quantifiers(
-        self, expr: LogicalExpr, tmp=None
+        self, expr: LogicalExpr
     ) -> Tuple[LogicalExpr, List[Dict[PddlEntity, PddlEntity]]]:
         """
         Expand out a logical expression that could involve a quantifier into
         only logical expressions that don't involve any quantifier. Doesn't
         require the simulation to be grounded and expands using the current
         defined types.
 
@@ -592,53 +607,61 @@
         if expr.quantifier == LogicalQuantifierType.FORALL:
             combine_type = LogicalExprType.AND
         elif expr.quantifier == LogicalQuantifierType.EXISTS:
             combine_type = LogicalExprType.OR
         elif expr.quantifier is None:
             return expr, []
         else:
-            raise ValueError(f"Unrecongized {expr.quantifier}")
+            raise ValueError(f"Unrecognized {expr.quantifier}")
 
-        all_matching_entities = []
+        t_start = time.time()
+        assigns: List[List[PddlEntity]] = [[]]
         for expand_entity in expr.inputs:
-            all_matching_entities.append(
-                [
-                    e
-                    for e in self.all_entities.values()
-                    if e.expr_type.is_subtype_of(expand_entity.expr_type)
-                ]
-            )
-
-        expanded_exprs: List[Union[LogicalExpr, Predicate]] = []
-        assigns = []
-        for poss_input in itertools.product(*all_matching_entities):
-            assert len(poss_input) == len(expr.inputs)
-            sub_dict = dict(zip(expr.inputs, poss_input))
-            assigns.append(sub_dict)
-
-            expanded_exprs.append(expr.clone().sub_in(sub_dict))
+            entity_assigns = []
+            for e in self.all_entities.values():
+                if not e.expr_type.is_subtype_of(expand_entity.expr_type):
+                    continue
+                for cur_assign in assigns:
+                    if e in cur_assign:
+                        continue
+                    entity_assigns.append([*cur_assign, e])
+            assigns = entity_assigns
+        if self._sim_info is not None:
+            self.sim_info.sim.add_perf_timing("assigns_search", t_start)
+
+        t_start = time.time()
+        assigns = [dict(zip(expr.inputs, assign)) for assign in assigns]
+        expanded_exprs = []
+        for assign in assigns:
+            expanded_exprs.append(expr.sub_in_clone(assign))
+        if self._sim_info is not None:
+            self.sim_info.sim.add_perf_timing("expand_exprs_set", t_start)
 
         inputs: List[PddlEntity] = []
-        return LogicalExpr(combine_type, expanded_exprs, inputs, None), assigns
+        return (
+            LogicalExpr(combine_type, expanded_exprs, inputs, None),
+            assigns,
+        )
 
 
 class PddlProblem(PddlDomain):
     stage_goals: Dict[str, LogicalExpr]
     init: List[Predicate]
     goal: LogicalExpr
 
     def __init__(
         self,
         domain_file_path: str,
         problem_file_path: str,
         cur_task_config: Optional["DictConfig"] = None,
+        read_config: bool = True,
     ):
         self._objects = {}
 
-        super().__init__(domain_file_path, cur_task_config)
+        super().__init__(domain_file_path, cur_task_config, read_config)
         with open(get_full_habitat_config_path(problem_file_path), "r") as f:
             problem_def = yaml.safe_load(f)
         self._objects = {
             o["name"]: PddlEntity(o["name"], self.expr_types[o["expr_type"]])
             for o in problem_def["objects"]
         }
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from enum import Enum
-from functools import reduce
 from typing import Dict, List, Optional, Union
 
 from habitat.tasks.rearrange.multi_task.pddl_predicate import Predicate
 from habitat.tasks.rearrange.multi_task.rearrange_pddl import (
     PddlEntity,
     PddlSimInfo,
 )
@@ -33,14 +32,24 @@
         inputs: List[PddlEntity],
         quantifier: Optional[LogicalQuantifierType],
     ):
         self._expr_type = expr_type
         self._sub_exprs = sub_exprs
         self._inputs = inputs
         self._quantifier = quantifier
+        self._truth_vals: List[Optional[bool]] = []
+
+    @property
+    def prev_truth_vals(self) -> List[Optional[bool]]:
+        """
+        Sub-expression truth values for the last `self.is_true` computation. A
+        value of None is if the truth value was not computed (due to early
+        break).
+        """
+        return self._truth_vals
 
     @property
     def expr_type(self):
         return self._expr_type
 
     @property
     def inputs(self):
@@ -67,51 +76,73 @@
 
         return self._is_true(check_statement)
 
     def is_true(self, sim_info: PddlSimInfo) -> bool:
         return self._is_true(lambda p: p.is_true(sim_info))
 
     def _is_true(self, is_true_fn) -> bool:
+        self._truth_vals = [None] * len(self._sub_exprs)
+
         if (
             self._expr_type == LogicalExprType.AND
             or self._expr_type == LogicalExprType.NAND
         ):
-            reduce_op = lambda x, y: x and y
-            init_value = True
+            result = True
+            for i, sub_expr in enumerate(self._sub_exprs):
+                truth_val = is_true_fn(sub_expr)
+                assert isinstance(truth_val, bool)
+                self._truth_vals[i] = truth_val
+                result = result and truth_val
+                if not result:
+                    break
         elif (
             self._expr_type == LogicalExprType.OR
             or self._expr_type == LogicalExprType.NOR
         ):
-            reduce_op = lambda x, y: x or y
-            init_value = False
+            result = False
+            for i, sub_expr in enumerate(self._sub_exprs):
+                truth_val = is_true_fn(sub_expr)
+                assert isinstance(truth_val, bool)
+                self._truth_vals[i] = truth_val
+                result = result or truth_val
+                if result:
+                    break
         else:
-            raise ValueError()
-        self.prev_truth_vals = [
-            is_true_fn(sub_expr) for sub_expr in self._sub_exprs
-        ]
-
-        ret = reduce(
-            reduce_op,
-            self.prev_truth_vals,
-            init_value,
-        )
+            raise ValueError(
+                f"Got unexpected expr_type: {self._expr_type} of type {type(self._expr_type)}"
+            )
+
         if (
             self._expr_type == LogicalExprType.NAND
             or self._expr_type == LogicalExprType.NOR
         ):
-            ret = not ret
-        return ret
+            # Invert the entire result for NAND and NOR expressions.
+            result = not result
+        return result
 
     def sub_in(self, sub_dict: Dict[PddlEntity, PddlEntity]) -> "LogicalExpr":
         self._sub_exprs = [e.sub_in(sub_dict) for e in self._sub_exprs]
         return self
 
+    def sub_in_clone(self, sub_dict: Dict[PddlEntity, PddlEntity]):
+        return LogicalExpr(
+            self._expr_type,
+            [e.sub_in_clone(sub_dict) for e in self._sub_exprs],
+            self._inputs,
+            self._quantifier,
+        )
+
     def __repr__(self):
         return f"({self._expr_type}: {self._sub_exprs}"
 
+    @property
+    def compact_str(self):
+        sub_s = ",".join((s.compact_str for s in self._sub_exprs))
+        return f"{self._expr_type.value}({sub_s})"
+
     def clone(self) -> "LogicalExpr":
         return LogicalExpr(
             self._expr_type,
             [p.clone() for p in self._sub_exprs],
             self._inputs,
             self._quantifier,
         )
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_predicate.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_predicate.py`

 * *Files 15% similar despite different names*

```diff
@@ -76,19 +76,45 @@
         self._arg_values = [
             sub_dict.get(entity, entity) for entity in self._arg_values
         ]
         ensure_entity_lists_match(self._args, self._arg_values)
         self._pddl_sim_state.sub_in(sub_dict)
         return self
 
+    def sub_in_clone(self, sub_dict: Dict[PddlEntity, PddlEntity]):
+        p = Predicate(
+            self._name,
+            self._pddl_sim_state.sub_in_clone(sub_dict),
+            self._args,
+        )
+        if self._arg_values is not None:
+            p.set_param_values(
+                [sub_dict.get(entity, entity) for entity in self._arg_values]
+            )
+        return p
+
     def is_true(self, sim_info: PddlSimInfo) -> bool:
         """
         Returns if the predicate is satisfied in the current simulator state.
+        Potentially returns the cached truth value of the predicate depending
+        on `sim_info`.
         """
-        return self._pddl_sim_state.is_true(sim_info)
+        self_repr = repr(self)
+        if (
+            sim_info.pred_truth_cache is not None
+            and self_repr in sim_info.pred_truth_cache
+        ):
+            # Return the cached value.
+            return sim_info.pred_truth_cache[self_repr]
+
+        # Recompute and potentially cache the result.
+        result = self._pddl_sim_state.is_true(sim_info)
+        if sim_info.pred_truth_cache is not None:
+            sim_info.pred_truth_cache[self_repr] = result
+        return result
 
     def set_state(self, sim_info: PddlSimInfo) -> None:
         """
         Sets the simulator state to satisfy the predicate.
         """
         return self._pddl_sim_state.set_state(sim_info)
 
@@ -102,15 +128,15 @@
         return f"<Predicate: {self._name} [{self._args}] [{self._arg_values}]>"
 
     def __repr__(self):
         return str(self)
 
     @property
     def compact_str(self):
-        args = ",".join([str(x) for x in self._arg_values])
+        args = ",".join((x.name for x in self._arg_values))
         return f"{self._name}({args})"
 
     def __eq__(self, other_pred):
         return (
             self._name == other_pred._name
             and self._args == other_pred._args
             and self._arg_values == other_pred._arg_values
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/pddl_sim_state.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_sim_state.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 from habitat.sims.habitat_simulator.sim_utilities import get_ao_global_bb
 from habitat.tasks.rearrange.marker_info import MarkerInfo
 from habitat.tasks.rearrange.multi_task.rearrange_pddl import (
     PddlEntity,
     PddlSimInfo,
     SimulatorObjectType,
 )
-from habitat.tasks.rearrange.utils import (
-    get_angle_to_pos,
-    get_robot_spawns,
-    rearrange_logger,
-)
+from habitat.tasks.rearrange.utils import get_robot_spawns, rearrange_logger
 
 CAB_TYPE = "cab_type"
 FRIDGE_TYPE = "fridge_type"
 
 
 class ArtSampler:
     def __init__(
@@ -56,32 +52,64 @@
 @dataclass
 class PddlRobotState:
     """
     Specifies the configuration of the robot.
 
     :property place_at_pos_dist: If -1.0, this will place the robot as close
         as possible to the entity. Otherwise, it will place the robot within X
-        meters of the entity.
+        meters of the entity. If unset, sets to task default.
     :property base_angle_noise: How much noise to add to the robot base angle
-        when setting the robot base position.
+        when setting the robot base position. If not set, sets to task default.
+    :property place_at_angle_thresh: The required maximum angle to the target
+        entity in the robot's local frame. Specified in radains. If not specified,
+        no angle is considered.
+    :property physics_stability_steps: Number of physics checks for placing the
+        robot. If not set, sets to task default.
     """
 
     holding: Optional[PddlEntity] = None
     should_drop: bool = False
     pos: Optional[Any] = None
-    place_at_pos_dist: float = -1.0
-    base_angle_noise: float = 0.0
+    place_at_pos_dist: Optional[float] = None
+    place_at_angle_thresh: Optional[float] = None
+    base_angle_noise: Optional[float] = None
+    physics_stability_steps: Optional[int] = None
+
+    def get_place_at_pos_dist(self, sim_info) -> float:
+        if self.place_at_pos_dist is None:
+            return sim_info.robot_at_thresh
+        else:
+            return self.place_at_pos_dist
+
+    def get_base_angle_noise(self, sim_info) -> float:
+        if self.base_angle_noise is None:
+            return 0.0
+        return self.base_angle_noise
+
+    def get_physics_stability_steps(self, sim_info) -> Optional[int]:
+        if self.physics_stability_steps is None:
+            return sim_info.physics_stability_steps
+        else:
+            return self.physics_stability_steps
 
     def sub_in(
         self, sub_dict: Dict[PddlEntity, PddlEntity]
     ) -> "PddlRobotState":
         self.holding = sub_dict.get(self.holding, self.holding)
         self.pos = sub_dict.get(self.pos, self.pos)
         return self
 
+    def sub_in_clone(
+        self, sub_dict: Dict[PddlEntity, PddlEntity]
+    ) -> "PddlRobotState":
+        other = replace(self)
+        other.holding = sub_dict.get(self.holding, self.holding)
+        other.pos = sub_dict.get(self.pos, self.pos)
+        return other
+
     def clone(self) -> "PddlRobotState":
         """
         Returns a shallow copy
         """
         return replace(self)
 
     def is_true(self, sim_info: PddlSimInfo, robot_entity: PddlEntity) -> bool:
@@ -104,20 +132,39 @@
                 return False
         elif self.should_drop and grasp_mgr.snap_idx != None:
             return False
 
         if isinstance(self.pos, PddlEntity):
             targ_pos = sim_info.get_entity_pos(self.pos)
             robot = sim_info.sim.get_agent_data(robot_id).articulated_agent
-            dist = np.linalg.norm(robot.base_pos - targ_pos)
-            if self.place_at_pos_dist == -1.0:
-                use_thresh = sim_info.robot_at_thresh
-            else:
-                use_thresh = self.place_at_pos_dist
-            if dist > use_thresh:
+
+            # Get the base transformation
+            T = robot.base_transformation
+            # Do transformation
+            pos = T.inverted().transform_point(targ_pos)
+            # Compute distance
+            dist = np.linalg.norm(pos)
+            # Project to 2D plane (x,y,z=0)
+            pos[2] = 0.0
+            # Unit vector of the pos
+            pos = pos.normalized()
+            # Define the coordinate of the robot
+            pos_robot = np.array([1.0, 0.0, 0.0])
+            # Get the angle
+            angle = np.arccos(np.dot(pos, pos_robot))
+
+            # Check the distance threshold.
+            if dist > self.get_place_at_pos_dist(sim_info):
+                return False
+
+            # Check for the angle threshold
+            if (
+                self.place_at_angle_thresh is not None
+                and np.abs(angle) > self.place_at_angle_thresh
+            ):
                 return False
 
         return True
 
     def set_state(
         self, sim_info: PddlSimInfo, robot_entity: PddlEntity
     ) -> None:
@@ -125,61 +172,51 @@
         Sets the robot state in the simulator.
         """
         robot_id = cast(
             int,
             sim_info.search_for_entity(robot_entity),
         )
         sim = sim_info.sim
-        grasp_mgr = sim.get_agent_data(robot_id).grasp_mgr
+        agent_data = sim.get_agent_data(robot_id)
         # Set the snapped object information
-        if self.should_drop and grasp_mgr.is_grasped:
-            grasp_mgr.desnap(True)
+        if self.should_drop and agent_data.grasp_mgr.is_grasped:
+            agent_data.grasp_mgr.desnap(True)
         elif self.holding is not None:
             # Swap objects to the desired object.
             obj_idx = cast(int, sim_info.search_for_entity(self.holding))
-            grasp_mgr.desnap(True)
+            agent_data.grasp_mgr.desnap(True)
             sim.internal_step(-1)
-            grasp_mgr.snap_to_obj(sim.scene_obj_ids[obj_idx])
+            agent_data.grasp_mgr.snap_to_obj(sim.scene_obj_ids[obj_idx])
             sim.internal_step(-1)
 
         # Set the robot starting position
         if isinstance(self.pos, PddlEntity):
             targ_pos = sim_info.get_entity_pos(self.pos)
-            agent = sim.get_agent_data(robot_id).articulated_agent
 
-            if self.place_at_pos_dist == -1.0:
-                # Place as close to the object as possible.
-                if not sim_info.sim.is_point_within_bounds(targ_pos):
-                    rearrange_logger.error(
-                        f"Object {self.pos} is out of bounds but trying to set robot position"
-                    )
-
-                agent_pos = sim_info.sim.safe_snap_point(targ_pos)
-                agent.base_pos = agent_pos
-                agent.base_rot = get_angle_to_pos(
-                    np.array(targ_pos - agent_pos)
-                )
-            else:
-                # Place some distance away from the object.
-                start_pos, start_rot, was_fail = get_robot_spawns(
-                    targ_pos,
-                    self.base_angle_noise,
-                    self.place_at_pos_dist,
-                    sim,
-                    sim_info.num_spawn_attempts,
-                    sim_info.physics_stability_steps,
-                )
-                sim.articulated_agent.base_pos = start_pos
-                sim.articulated_agent.base_rot = start_rot
-                if was_fail:
-                    rearrange_logger.error("Failed to place the robot.")
+            # Place some distance away from the object.
+            start_pos, start_rot, was_fail = get_robot_spawns(
+                target_position=targ_pos,
+                rotation_perturbation_noise=self.get_base_angle_noise(
+                    sim_info
+                ),
+                distance_threshold=self.get_place_at_pos_dist(sim_info),
+                sim=sim,
+                num_spawn_attempts=sim_info.num_spawn_attempts,
+                physics_stability_steps=self.get_physics_stability_steps(
+                    sim_info
+                ),
+                agent=agent_data.articulated_agent,
+            )
+            agent_data.articulated_agent.base_pos = start_pos
+            agent_data.articulated_agent.base_rot = start_rot
+            if was_fail:
+                rearrange_logger.error("Failed to place the robot.")
 
             # We teleported the agent. We also need to teleport the object the agent was holding.
-            grasp_mgr = sim.get_agent_data(robot_id).grasp_mgr
-            grasp_mgr.update_object_to_grasp()
+            agent_data.grasp_mgr.update_object_to_grasp()
 
         elif self.pos is not None:
             raise ValueError(f"Unrecongized set position {self.pos}")
 
 
 class PddlSimState:
     def __init__(
@@ -212,14 +249,29 @@
     def clone(self) -> "PddlSimState":
         return PddlSimState(
             self._art_states,
             self._obj_states,
             {k: v.clone() for k, v in self._robot_states.items()},
         )
 
+    def sub_in_clone(
+        self, sub_dict: Dict[PddlEntity, PddlEntity]
+    ) -> "PddlSimState":
+        return PddlSimState(
+            {sub_dict.get(k, k): v for k, v in self._art_states.items()},
+            {
+                sub_dict.get(k, k): sub_dict.get(v, v)
+                for k, v in self._obj_states.items()
+            },
+            {
+                sub_dict.get(k, k): robot_state.sub_in_clone(sub_dict)
+                for k, robot_state in self._robot_states.items()
+            },
+        )
+
     def sub_in(self, sub_dict: Dict[PddlEntity, PddlEntity]) -> "PddlSimState":
         self._robot_states = {
             sub_dict.get(k, k): robot_state.sub_in(sub_dict)
             for k, robot_state in self._robot_states.items()
         }
         self._art_states = {
             sub_dict.get(k, k): v for k, v in self._art_states.items()
@@ -385,15 +437,24 @@
                 )
                 all_targ_idxs, pos_targs = sim.get_targets()
                 targ_pos = pos_targs[list(all_targ_idxs).index(targ_idx)]
                 set_T = mn.Matrix4.translation(targ_pos)
             elif sim_info.check_type_matches(
                 target, SimulatorObjectType.STATIC_RECEPTACLE_ENTITY.value
             ):
-                raise NotImplementedError()
+                # Place object on top of receptacle.
+                recep = cast(mn.Range3D, sim_info.search_for_entity(target))
+
+                # Divide by 2 because the `from_center` creates from the half size.
+                shrunk_recep = mn.Range3D.from_center(
+                    recep.center(),
+                    (recep.size() / 2.0) * sim_info.recep_place_shrink_factor,
+                )
+                pos = np.random.uniform(shrunk_recep.min, shrunk_recep.max)
+                set_T = mn.Matrix4.translation(pos)
             else:
                 raise ValueError(f"Got unexpected target {target}")
 
             obj_idx = cast(int, sim_info.search_for_entity(entity))
             abs_obj_id = sim.scene_obj_ids[obj_idx]
 
             # Get the object id corresponding to this name
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/rearrange_pddl.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/rearrange_pddl.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,28 +140,34 @@
     expr_types: Dict[str, ExprType]
     predicates: Dict[str, Any]
     all_entities: Dict[str, Any]
     receptacles: Dict[str, mn.Range3D]
 
     num_spawn_attempts: int
     physics_stability_steps: int
+    recep_place_shrink_factor: float
+
+    pred_truth_cache: Optional[Dict[str, bool]] = None
+
+    def reset_pred_truth_cache(self):
+        self.pred_truth_cache = {}
 
     def get_predicate(self, pred_name: str):
         return self.predicates[pred_name]
 
     def check_type_matches(self, entity: PddlEntity, match_name: str) -> bool:
         return entity.expr_type.is_subtype_of(self.expr_types[match_name])
 
     def get_entity_pos(self, entity: PddlEntity) -> np.ndarray:
         ename = entity.name
         if self.check_type_matches(
             entity, SimulatorObjectType.ROBOT_ENTITY.value
         ):
             robot_id = self.robot_ids[ename]
-            return self.sim.get_agent_data(robot_id).robot.base_pos
+            return self.sim.get_agent_data(robot_id).articulated_agent.base_pos
         if self.check_type_matches(
             entity, SimulatorObjectType.ARTICULATED_RECEPTACLE_ENTITY.value
         ):
             marker_info = self.marker_handles[ename]
             return marker_info.get_current_position()
         if self.check_type_matches(
             entity, SimulatorObjectType.GOAL_ENTITY.value
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/multi_task/task_creator_utils.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/task_creator_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_grasp_manager.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_grasp_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         self._config = config
         self._managed_articulated_agent = articulated_agent
         self.ee_index = ee_index
 
         self._kinematic_mode = self._sim.habitat_config.kinematic_mode
 
     def reconfigure(self) -> None:
-        """Removes any existing constraints managed by this structure.
-        Called from _sim.reconfigure().
-        """
+        """Removes any existing constraints managed by this structure."""
         self._snap_constraints.clear()
 
     def reset(self) -> None:
         """Reset the grasp manager by re-defining the collision group and dropping any grasped object."""
         # Setup the collision groups. UserGroup7 is the held object group, it
         # can interact with anything except for the robot.
         CollisionGroupHelper.set_mask_for_group(
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 
+from collections import defaultdict, deque
+
 import numpy as np
 from gym import spaces
 
 from habitat.core.embodied_task import Measure
 from habitat.core.registry import registry
 from habitat.core.simulator import Sensor, SensorTypes
 from habitat.tasks.nav.nav import PointGoalSensor
@@ -470,15 +472,15 @@
         self.update_metric(*args, episode=episode, **kwargs)
 
     def update_metric(self, *args, episode, **kwargs):
         idxs, goal_pos = self._sim.get_targets()
         scene_pos = self._sim.get_scene_pos()
         target_pos = scene_pos[idxs]
         distances = np.linalg.norm(target_pos - goal_pos, ord=2, axis=-1)
-        self._metric = {str(idx): dist for idx, dist in zip(idxs, distances)}
+        self._metric = {str(idx): dist for idx, dist in enumerate(distances)}
 
 
 @registry.register_measure
 class GfxReplayMeasure(Measure):
     cls_uuid: str = "gfx_replay_keyframes_string"
 
     def __init__(self, sim, config, *args, **kwargs):
@@ -574,19 +576,19 @@
     def update_metric(self, *args, observations, **kwargs):
         ee_pos = (
             self._sim.get_agent_data(self.agent_id)
             .articulated_agent.ee_transform()
             .translation
         )
 
-        idxs, goals = self._sim.get_targets()
+        goals = self._sim.get_targets()[1]
 
         distances = np.linalg.norm(goals - ee_pos, ord=2, axis=-1)
 
-        self._metric = {str(idx): dist for idx, dist in zip(idxs, distances)}
+        self._metric = {str(idx): dist for idx, dist in enumerate(distances)}
 
 
 @registry.register_measure
 class EndEffectorToObjectDistance(UsesArticulatedAgentInterface, Measure):
     """
     Gets the distance between the end-effector and all current target object COMs.
     """
@@ -614,15 +616,15 @@
 
         idxs, _ = self._sim.get_targets()
         scene_pos = self._sim.get_scene_pos()
         target_pos = scene_pos[idxs]
 
         distances = np.linalg.norm(target_pos - ee_pos, ord=2, axis=-1)
 
-        self._metric = {str(idx): dist for idx, dist in zip(idxs, distances)}
+        self._metric = {str(idx): dist for idx, dist in enumerate(distances)}
 
 
 @registry.register_measure
 class EndEffectorToRestDistance(Measure):
     """
     Distance between current end effector position and position where end effector rests within the robot body.
     """
@@ -1019,7 +1021,36 @@
             DoesWantTerminate.cls_uuid
         ].get_metric()
         is_succ = task.measurements.measures[
             self._success_measure_name
         ].get_metric()
 
         self._metric = (not is_succ) and does_action_want_stop
+
+
+@registry.register_measure
+class RuntimePerfStats(Measure):
+    cls_uuid: str = "habitat_perf"
+
+    @staticmethod
+    def _get_uuid(*args, **kwargs):
+        return RuntimePerfStats.cls_uuid
+
+    def __init__(self, sim, config, *args, **kwargs):
+        self._sim = sim
+        self._sim.enable_perf_logging()
+        self._disable_logging = config.disable_logging
+        super().__init__()
+
+    def reset_metric(self, *args, **kwargs):
+        self._metric_queue = defaultdict(deque)
+        self._metric = {}
+
+    def update_metric(self, *args, task, **kwargs):
+        for k, v in self._sim.get_runtime_perf_stats().items():
+            self._metric_queue[k].append(v)
+        if self._disable_logging:
+            self._metric = {}
+        else:
+            self._metric = {
+                k: np.mean(v) for k, v in self._metric_queue.items()
+            }
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_sim.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os.path as osp
+import time
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
@@ -32,21 +33,23 @@
 from habitat.datasets.rearrange.rearrange_dataset import RearrangeEpisode
 from habitat.datasets.rearrange.samplers.receptacle import (
     AABBReceptacle,
     find_receptacles,
 )
 from habitat.sims.habitat_simulator.habitat_simulator import HabitatSim
 from habitat.tasks.rearrange.articulated_agent_manager import (
+    ArticulatedAgentData,
     ArticulatedAgentManager,
 )
 from habitat.tasks.rearrange.marker_info import MarkerInfo
 from habitat.tasks.rearrange.rearrange_grasp_manager import (
     RearrangeGraspManager,
 )
 from habitat.tasks.rearrange.utils import (
+    add_perf_timing_func,
     get_aabb,
     make_render_only,
     rearrange_collision,
     rearrange_logger,
 )
 from habitat_sim.nav import NavMeshSettings
 from habitat_sim.physics import CollisionGroups, JointMotorSettings, MotionType
@@ -90,44 +93,67 @@
 
         self.art_objs: List[habitat_sim.physics.ManagedArticulatedObject] = []
         self._start_art_states: Dict[
             habitat_sim.physics.ManagedArticulatedObject, List[float]
         ] = {}
         self._prev_obj_names: Optional[List[str]] = None
         self._scene_obj_ids: List[int] = []
+        # The receptacle information cached between all scenes.
+        self._receptacles_cache: Dict[str, Dict[str, mn.Range3D]] = {}
+        # The per episode receptacle information.
         self._receptacles: Dict[str, mn.Range3D] = {}
         # Used to get data from the RL environment class to sensors.
         self._goal_pos = None
         self.viz_ids: Dict[Any, Any] = defaultdict(lambda: None)
         self._handle_to_object_id: Dict[str, int] = {}
         self._markers: Dict[str, MarkerInfo] = {}
 
         self._viz_templates: Dict[str, Any] = {}
         self._viz_handle_to_template: Dict[str, float] = {}
         self._viz_objs: Dict[str, Any] = {}
         self._draw_bb_objs: List[int] = []
 
         self.agents_mgr = ArticulatedAgentManager(self.habitat_config, self)
 
+        # Setup config options.
         self._debug_render_articulated_agent = (
             self.habitat_config.debug_render_articulated_agent
         )
         self._debug_render_goal = self.habitat_config.debug_render_goal
         self._debug_render = self.habitat_config.debug_render
         self._concur_render = self.habitat_config.concur_render
+        self._batch_render = config.renderer.enable_batch_renderer
         self._enable_gfx_replay_save = (
             self.habitat_config.habitat_sim_v0.enable_gfx_replay_save
         )
         self._needs_markers = self.habitat_config.needs_markers
         self._update_articulated_agent = (
             self.habitat_config.update_articulated_agent
         )
         self._step_physics = self.habitat_config.step_physics
+        self._auto_sleep = self.habitat_config.auto_sleep
+        self._load_objs = self.habitat_config.load_objs
+        self._additional_object_paths = (
+            self.habitat_config.additional_object_paths
+        )
         self._kinematic_mode = self.habitat_config.kinematic_mode
 
+        self._extra_runtime_perf_stats: Dict[str, float] = defaultdict(float)
+        self._perf_logging_enabled = False
+        self.cur_runtime_perf_scope: List[str] = []
+        self._should_setup_semantic_ids = (
+            self.habitat_config.should_setup_semantic_ids
+        )
+
+    def enable_perf_logging(self):
+        """
+        Will turn on the performance logging (by default this is off).
+        """
+        self._perf_logging_enabled = True
+
     @property
     def receptacles(self) -> Dict[str, AABBReceptacle]:
         return self._receptacles
 
     @property
     def handle_to_object_id(self) -> Dict[str, int]:
         """
@@ -186,18 +212,20 @@
         for target_handle, trans in self._targets.items():
             targ_idx = self._scene_obj_ids.index(
                 rom.get_object_by_handle(target_handle).object_id
             )
             target_trans.append((targ_idx, trans))
         return target_trans
 
+    @add_perf_timing_func()
     def _try_acquire_context(self):
-        if self._concur_render:
+        if self.renderer and self._concur_render:
             self.renderer.acquire_gl_context()
 
+    @add_perf_timing_func()
     def _sleep_all_objects(self):
         """
         De-activate (sleep) all rigid objects in the scene, assuming they are already in a dynamically stable state.
         """
         rom = self.get_rigid_object_manager()
         for _, ro in rom.get_objects_by_handle_substring().items():
             ro.awake = False
@@ -233,44 +261,49 @@
     def get_all_markers(self):
         return self._markers
 
     def _update_markers(self) -> None:
         for m in self._markers.values():
             m.update()
 
+    @add_perf_timing_func()
     def reset(self):
         SimulatorBackend.reset(self)
         for i in range(len(self.agents)):
             self.reset_agent(i)
         return None
 
+    @add_perf_timing_func()
     def reconfigure(self, config: "DictConfig", ep_info: RearrangeEpisode):
         self._handle_to_goal_name = ep_info.info["object_labels"]
 
-        with read_write(config):
-            config["scene"] = ep_info.scene_id
-
-        super().reconfigure(config, should_close_on_new_scene=False)
-
         self.ep_info = ep_info
-        self._try_acquire_context()
-
         new_scene = self.prev_scene_id != ep_info.scene_id
-
         if new_scene:
             self._prev_obj_names = None
 
-        self.agents_mgr.reconfigure(new_scene)
-
-        # Only remove and re-add objects if we have a new set of objects.
         obj_names = [x[0] for x in ep_info.rigid_objs]
+        # Only remove and re-add objects if we have a new set of objects.
         should_add_objects = self._prev_obj_names != obj_names
         self._prev_obj_names = obj_names
 
-        self._clear_objects(should_add_objects)
+        self.agents_mgr.pre_obj_clear()
+        self._clear_objects(should_add_objects, new_scene)
+
+        is_hard_reset = new_scene or should_add_objects
+
+        if is_hard_reset:
+            with read_write(config):
+                config["scene"] = ep_info.scene_id
+            t_start = time.time()
+            super().reconfigure(config, should_close_on_new_scene=False)
+            self.add_perf_timing("super_reconfigure", t_start)
+
+        if new_scene:
+            self.agents_mgr.on_new_scene()
 
         self.prev_scene_id = ep_info.scene_id
         self._viz_templates = {}
         self._viz_handle_to_template = {}
 
         # Set the default articulated object joint state.
         for ao, set_joint_state in self._start_art_states.items():
@@ -279,22 +312,22 @@
 
         # Load specified articulated object states from episode config
         self._set_ao_states_from_ep(ep_info)
 
         self.agents_mgr.post_obj_load_reconfigure()
 
         # add episode clutter objects additional to base scene objects
-        if self.habitat_config.load_objs:
-            self._add_objs(ep_info, should_add_objects)
+        if self._load_objs:
+            self._add_objs(ep_info, should_add_objects, new_scene)
         self._setup_targets(ep_info)
 
         self._add_markers(ep_info)
 
         # auto-sleep rigid objects as optimization
-        if self.habitat_config.auto_sleep:
+        if self._auto_sleep:
             self._sleep_all_objects()
 
         rom = self.get_rigid_object_manager()
         self._obj_orig_motion_types = {
             handle: ro.motion_type
             for handle, ro in rom.get_objects_by_handle_substring().items()
         }
@@ -324,24 +357,29 @@
             self.first_setup = False
             self.agents_mgr.first_setup()
             # Capture the starting art states
             self._start_art_states = {
                 ao: ao.joint_positions for ao in self.art_objs
             }
 
+        if self._should_setup_semantic_ids:
+            self._setup_semantic_ids()
+
+    @add_perf_timing_func()
+    def _setup_semantic_ids(self):
         # Add the rigid object id for the semantic map
         rom = self.get_rigid_object_manager()
         for i, handle in enumerate(rom.get_object_handles()):
             obj = rom.get_object_by_handle(handle)
             for node in obj.visual_scene_nodes:
                 node.semantic_id = (
                     obj.object_id + self.habitat_config.object_ids_start
                 )
 
-    def get_agent_data(self, agent_idx: Optional[int]):
+    def get_agent_data(self, agent_idx: Optional[int]) -> ArticulatedAgentData:
         if agent_idx is None:
             return self.agents_mgr[0]
         else:
             return self.agents_mgr[agent_idx]
 
     @property
     def num_articulated_agents(self):
@@ -386,30 +424,44 @@
     def _setup_targets(self, ep_info):
         self._targets = {}
         for target_handle, transform in ep_info.targets.items():
             self._targets[target_handle] = mn.Matrix4(
                 [[transform[j][i] for j in range(4)] for i in range(4)]
             )
 
+    @add_perf_timing_func()
     def _load_navmesh(self, ep_info):
         scene_name = ep_info.scene_id.split("/")[-1].split(".")[0]
         base_dir = osp.join(*ep_info.scene_id.split("/")[:2])
 
         navmesh_path = osp.join(base_dir, "navmeshes", scene_name + ".navmesh")
         self.pathfinder.load_nav_mesh(navmesh_path)
 
         self._navmesh_vertices = np.stack(
             self.pathfinder.build_navmesh_vertices(), axis=0
         )
         self._island_sizes = [
             self.pathfinder.island_radius(p) for p in self._navmesh_vertices
         ]
         self._max_island_size = max(self._island_sizes)
+        self._largest_island_idx = self.pathfinder.get_island(
+            self._navmesh_vertices[np.argmax(self._island_sizes)]
+        )
+
+    @property
+    def largest_island_idx(self) -> int:
+        """
+        The path finder index of the island that has the largest area.
+        """
+        return self._largest_island_idx
 
-    def _clear_objects(self, should_add_objects: bool) -> None:
+    @add_perf_timing_func()
+    def _clear_objects(
+        self, should_add_objects: bool, new_scene: bool
+    ) -> None:
         rom = self.get_rigid_object_manager()
 
         # Clear all the rigid objects.
         if should_add_objects:
             for scene_obj_id in self._scene_obj_ids:
                 if not rom.get_library_has_id(scene_obj_id):
                     continue
@@ -424,18 +476,20 @@
 
         # Remove all object mesh visualizations.
         for viz_obj in self._viz_objs.values():
             if rom.get_library_has_id(viz_obj.object_id):
                 rom.remove_object_by_id(viz_obj.object_id)
         self._viz_objs = {}
 
-        # Do not remove the articulated objects from the scene, these are
-        # managed by the underlying sim.
-        self.art_objs = []
+        if new_scene:
+            # Do not remove the articulated objects from the scene, these are
+            # managed by the underlying sim.
+            self.art_objs = []
 
+    @add_perf_timing_func()
     def _set_ao_states_from_ep(self, ep_info: RearrangeEpisode) -> None:
         """
         Sets the ArticulatedObject states for the episode which are differ from base scene state.
         """
         aom = self.get_articulated_object_manager()
         for aoi_handle, joint_states in ep_info.ao_states.items():
             ao = aom.get_object_by_handle(aoi_handle)
@@ -478,40 +532,45 @@
                 np.array(pos).reshape(1, 3) - use_verts, axis=-1
             )
             closest_idx = np.argmin(distances)
             new_pos = self._navmesh_vertices[closest_idx]
 
         return new_pos
 
+    @add_perf_timing_func()
     def _add_objs(
-        self, ep_info: RearrangeEpisode, should_add_objects: bool
+        self,
+        ep_info: RearrangeEpisode,
+        should_add_objects: bool,
+        new_scene: bool,
     ) -> None:
         # Load clutter objects:
         rom = self.get_rigid_object_manager()
         obj_counts: Dict[str, int] = defaultdict(int)
 
         self._handle_to_object_id = {}
-        self._receptacles = {}
         if should_add_objects:
             self._scene_obj_ids = []
 
         for i, (obj_handle, transform) in enumerate(ep_info.rigid_objs):
+            t_start = time.time()
             if should_add_objects:
-                obj_attr_mgr = self.get_object_template_manager()
-                matching_templates = (
-                    obj_attr_mgr.get_templates_by_handle_substring(obj_handle)
-                )
+                template = None
+                for obj_path in self._additional_object_paths:
+                    template = osp.join(obj_path, obj_handle)
+                    if osp.isfile(template):
+                        break
                 assert (
-                    len(matching_templates.values()) == 1
-                ), f"Object attributes not uniquely matched to shortened handle. '{obj_handle}' matched to {matching_templates}. TODO: relative paths as handles should fix some duplicates. For now, try renaming objects to avoid collision."
-                ro = rom.add_object_by_template_handle(
-                    list(matching_templates.keys())[0]
-                )
+                    template is not None
+                ), f"Could not find config file for object {obj_handle}"
+
+                ro = rom.add_object_by_template_handle(template)
             else:
                 ro = rom.get_object_by_id(self._scene_obj_ids[i])
+            self.add_perf_timing("create_asset", t_start)
 
             # The saved matrices need to be flipped when reloading.
             ro.transformation = mn.Matrix4(
                 [[transform[j][i] for j in range(4)] for i in range(4)]
             )
             ro.angular_velocity = mn.Vector3.zero_init()
             ro.linear_velocity = mn.Vector3.zero_init()
@@ -530,37 +589,54 @@
 
             if other_obj_handle in self._handle_to_goal_name:
                 ref_handle = self._handle_to_goal_name[other_obj_handle]
                 self._handle_to_object_id[ref_handle] = rel_idx
 
             obj_counts[obj_handle] += 1
 
-        all_receps = find_receptacles(self)
-        for recep in all_receps:
-            recep = cast(AABBReceptacle, recep)
-            local_bounds = recep.bounds
-            global_T = recep.get_global_transform(self)
-            self._receptacles[recep.name] = mn.Range3D(
-                global_T.transform_point(local_bounds.min),
-                global_T.transform_point(local_bounds.max),
+        if new_scene:
+            self._receptacles = self._create_recep_info(
+                ep_info.scene_id, list(self._handle_to_object_id.keys())
             )
 
-        ao_mgr = self.get_articulated_object_manager()
-        articulated_agent_art_handles = [
-            articulated_agent.sim_obj.handle
-            for articulated_agent in self.agents_mgr.articulated_agents_iter
-        ]
-        for aoi_handle in ao_mgr.get_object_handles():
-            ao = ao_mgr.get_object_by_handle(aoi_handle)
-            if (
-                self._kinematic_mode
-                and ao.handle not in articulated_agent_art_handles
-            ):
-                ao.motion_type = habitat_sim.physics.MotionType.KINEMATIC
-            self.art_objs.append(ao)
+            ao_mgr = self.get_articulated_object_manager()
+            # Make all articulated objects (including the robots) kinematic
+            for aoi_handle in ao_mgr.get_object_handles():
+                ao = ao_mgr.get_object_by_handle(aoi_handle)
+                if self._kinematic_mode:
+                    ao.motion_type = habitat_sim.physics.MotionType.KINEMATIC
+                self.art_objs.append(ao)
+
+    def _create_recep_info(
+        self, scene_id: str, ignore_handles: List[str]
+    ) -> Dict[str, mn.Range3D]:
+        if scene_id not in self._receptacles_cache:
+            receps = {}
+            all_receps = find_receptacles(
+                self,
+                ignore_handles=ignore_handles,
+            )
+            for recep in all_receps:
+                recep = cast(AABBReceptacle, recep)
+                local_bounds = recep.bounds
+                global_T = recep.get_global_transform(self)
+                # Some coordinates may be flipped by the global transformation,
+                # mixing the minimum and maximum bound coordinates.
+                bounds = np.stack(
+                    [
+                        global_T.transform_point(local_bounds.min),
+                        global_T.transform_point(local_bounds.max),
+                    ],
+                    axis=0,
+                )
+                receps[recep.name] = mn.Range3D(
+                    np.min(bounds, axis=0), np.max(bounds, axis=0)
+                )
+            self._receptacles_cache[scene_id] = receps
+        return self._receptacles_cache[scene_id]
 
     def _create_obj_viz(self):
         """
         Adds a visualization of the goal for each of the target objects in the
         scene. This is the same as the target object, but is a render only
         object. This also places dots around the bounding box of the object to
         further distinguish the goal from the target object.
@@ -715,14 +791,15 @@
             mn.Rad(-np.pi / 2), mn.Vector3(0, 1, 0)
         )
         return AgentState(
             articulated_agent.base_pos,
             quat_from_magnum(articulated_agent.sim_obj.rotation * rot_offset),
         )
 
+    @add_perf_timing_func()
     def step(self, action: Union[str, int]) -> Observations:
         rom = self.get_rigid_object_manager()
 
         if self._debug_render:
             if self._debug_render_articulated_agent:
                 self.agents_mgr.update_debug()
             rom = self.get_rigid_object_manager()
@@ -748,29 +825,43 @@
                 rom.remove_object_by_id(viz_id)
                 r = self._viz_handle_to_template[viz_id]
                 add_back_viz_objs[name] = (before_pos, r)
             self.viz_ids = defaultdict(lambda: None)
 
         self.maybe_update_articulated_agent()
 
-        if self._concur_render:
-            self._prev_sim_obs = self.start_async_render()
+        if self._batch_render:
+            for _ in range(self.ac_freq_ratio):
+                self.internal_step(-1, update_articulated_agent=False)
+
+            obs = self.get_sensor_observations()
+            self.add_keyframe_to_observations(obs)
+        elif self._concur_render:
+            self.start_async_render()
 
             for _ in range(self.ac_freq_ratio):
                 self.internal_step(-1, update_articulated_agent=False)
 
-            self._prev_sim_obs = self.get_sensor_observations_async_finish()
-            obs = self._sensor_suite.get_observations(self._prev_sim_obs)
+            t_start = time.time()
+            obs = self._sensor_suite.get_observations(
+                self.get_sensor_observations_async_finish()
+            )
+            self.add_perf_timing("get_sensor_observations", t_start)
         else:
             for _ in range(self.ac_freq_ratio):
                 self.internal_step(-1, update_articulated_agent=False)
-            self._prev_sim_obs = self.get_sensor_observations()
-            obs = self._sensor_suite.get_observations(self._prev_sim_obs)
 
-        if self._enable_gfx_replay_save:
+            t_start = time.time()
+            obs = self._sensor_suite.get_observations(
+                self.get_sensor_observations()
+            )
+            self.add_perf_timing("get_sensor_observations", t_start)
+
+        # TODO: Support recording while batch rendering
+        if self._enable_gfx_replay_save and not self._batch_render:
             self.gfx_replay_manager.save_keyframe()
 
         if self._needs_markers:
             self._update_markers()
 
         # TODO: Make debug cameras more flexible
         if "third_rgb" in obs and self._debug_render:
@@ -827,20 +918,21 @@
             self._viz_handle_to_template[viz_obj.object_id] = r
         else:
             viz_obj = rom.get_object_by_id(viz_id)
 
         viz_obj.translation = mn.Vector3(*position)
         return viz_obj.object_id
 
+    @add_perf_timing_func()
     def internal_step(
         self, dt: Union[int, float], update_articulated_agent: bool = True
     ) -> None:
         """Step the world and update the articulated_agent.
 
-        :param dt: Timestep by which to advance the world. Multiple physics substeps can be excecuted within a single timestep. -1 indicates a single physics substep.
+        :param dt: Timestep by which to advance the world. Multiple physics substeps can be executed within a single timestep. -1 indicates a single physics substep.
 
         Never call sim.step_world directly or miss updating the articulated_agent.
         """
         # Optionally step physics and update the articulated_agent for benchmarking purposes
         if self._step_physics:
             self.step_world(dt)
 
@@ -875,7 +967,30 @@
         rom = self.get_rigid_object_manager()
         return np.array(
             [
                 rom.get_object_by_id(idx).translation
                 for idx in self._scene_obj_ids
             ]
         )
+
+    def add_perf_timing(self, desc: str, t_start: float) -> None:
+        """
+        Records a duration since `t_start` into the perf stats. Note that this
+        is additive, so times between successive calls accumulate, not reset.
+        Also note that this will only log if `self._perf_logging_enabled=True`.
+        """
+        if not self._perf_logging_enabled:
+            return
+
+        name = ".".join(self.cur_runtime_perf_scope)
+        if desc != "":
+            name += "." + desc
+        self._extra_runtime_perf_stats[name] += time.time() - t_start
+
+    def get_runtime_perf_stats(self) -> Dict[str, float]:
+        stats_dict = {}
+        for name, value in self._extra_runtime_perf_stats.items():
+            stats_dict[name] = value
+        # clear this dict so we don't accidentally collect these twice
+        self._extra_runtime_perf_stats = defaultdict(float)
+
+        return stats_dict
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/rearrange_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import numpy as np
 from gym import spaces
 
 from habitat.core.dataset import Episode
 from habitat.core.registry import registry
 from habitat.core.simulator import Sensor, SensorSuite
 from habitat.tasks.nav.nav import NavigationTask
-from habitat.tasks.rearrange.rearrange_sim import RearrangeSim
+from habitat.tasks.rearrange.rearrange_sim import (
+    RearrangeSim,
+    add_perf_timing_func,
+)
 from habitat.tasks.rearrange.utils import (
     CacheHelper,
     CollisionDetails,
     UsesArticulatedAgentInterface,
     rearrange_collision,
     rearrange_logger,
 )
@@ -76,14 +79,27 @@
         self._desired_resting = np.array(self._config.desired_resting_position)
         self._sim_reset = True
         self._targ_idx: int = 0
         self._episode_id: str = ""
         self._cur_episode_step = 0
         self._should_place_articulated_agent = should_place_articulated_agent
 
+        # Get config options
+        self._force_regenerate = self._config.force_regenerate
+        self._should_save_to_cache = self._config.should_save_to_cache
+        self._obj_succ_thresh = self._config.obj_succ_thresh
+        self._enable_safe_drop = self._config.enable_safe_drop
+        self._constraint_violation_ends_episode = (
+            self._config.constraint_violation_ends_episode
+        )
+        self._constraint_violation_drops_object = (
+            self._config.constraint_violation_drops_object
+        )
+        self._count_obj_collisions = self._config.count_obj_collisions
+
         data_path = dataset.config.data_path.format(split=dataset.config.split)
         fname = data_path.split("/")[-1].split(".")[0]
         cache_path = osp.join(
             osp.dirname(data_path),
             f"{fname}_{self._config.type}_robot_start.pickle",
         )
 
@@ -127,27 +143,27 @@
         self._sim_reset = sim_reset
 
     def _get_cached_articulated_agent_start(self, agent_idx: int = 0):
         start_ident = self._get_ep_init_ident(agent_idx)
         if (
             self._articulated_agent_pos_start is None
             or start_ident not in self._articulated_agent_pos_start
-            or self._config.force_regenerate
+            or self._force_regenerate
         ):
             return None
         else:
             return self._articulated_agent_pos_start[start_ident]
 
     def _get_ep_init_ident(self, agent_idx):
         return f"{self._episode_id}_{agent_idx}"
 
     def _cache_articulated_agent_start(self, cache_data, agent_idx: int = 0):
         if (
             self._articulated_agent_pos_start is not None
-            and self._config.should_save_to_cache
+            and self._should_save_to_cache
         ):
             start_ident = self._get_ep_init_ident(agent_idx)
             self._articulated_agent_pos_start[start_ident] = cache_data
             self._articulated_agent_init_cache.save(
                 self._articulated_agent_pos_start
             )
 
@@ -172,14 +188,15 @@
             ) = articulated_agent_start
         articulated_agent = self._sim.get_agent_data(
             agent_idx
         ).articulated_agent
         articulated_agent.base_pos = articulated_agent_pos
         articulated_agent.base_rot = articulated_agent_rot
 
+    @add_perf_timing_func()
     def reset(self, episode: Episode, fetch_observations: bool = True):
         self._episode_id = episode.episode_id
         self._ignore_collisions = []
 
         if self._sim_reset:
             self._sim.reset()
             for action_instance in self.actions.values():
@@ -199,52 +216,63 @@
         self._cur_episode_step = 0
         if fetch_observations:
             self._sim.maybe_update_articulated_agent()
             return self._get_observations(episode)
         else:
             return None
 
+    @add_perf_timing_func()
     def _get_observations(self, episode):
+        # Fetch the simulator observations, all visual sensors.
         obs = self._sim.get_sensor_observations()
-        obs = self._sim._sensor_suite.get_observations(obs)
 
-        task_obs = self.sensor_suite.get_observations(
-            observations=obs, episode=episode, task=self
+        if not self._sim.sim_config.enable_batch_renderer:
+            # Post-process visual sensor observations
+            obs = self._sim._sensor_suite.get_observations(obs)
+        else:
+            # Keyframes are added so that the simulator state can be reconstituted when batch rendering.
+            # The post-processing step above is done after batch rendering.
+            self._sim.add_keyframe_to_observations(obs)
+
+        # Task sensors (all non-visual sensors)
+        obs.update(
+            self.sensor_suite.get_observations(
+                observations=obs, episode=episode, task=self, should_time=True
+            )
         )
-        obs.update(task_obs)
         return obs
 
     def _is_violating_safe_drop(self, action_args):
         idxs, goal_pos = self._sim.get_targets()
         scene_pos = self._sim.get_scene_pos()
         target_pos = scene_pos[idxs]
         min_dist = np.min(
             np.linalg.norm(target_pos - goal_pos, ord=2, axis=-1)
         )
         return (
             self._sim.grasp_mgr.is_grasped
             and action_args.get("grip_action", None) is not None
             and action_args["grip_action"] < 0
-            and min_dist < self._config.obj_succ_thresh
+            and min_dist < self._obj_succ_thresh
         )
 
     def step(self, action: Dict[str, Any], episode: Episode):
         action_args = action["action_args"]
-        if self._config.enable_safe_drop and self._is_violating_safe_drop(
+        if self._enable_safe_drop and self._is_violating_safe_drop(
             action_args
         ):
             action_args["grip_action"] = None
         obs = super().step(action=action, episode=episode)
 
         self.prev_coll_accum = copy.copy(self.coll_accum)
         self._cur_episode_step += 1
         for grasp_mgr in self._sim.agents_mgr.grasp_iter:
             if (
                 grasp_mgr.is_violating_hold_constraint()
-                and self._config.constraint_violation_drops_object
+                and self._constraint_violation_drops_object
             ):
                 grasp_mgr.desnap(True)
 
         return obs
 
     def _check_episode_is_active(
         self,
@@ -257,15 +285,15 @@
         if self.should_end:
             done = True
 
         # Check that none of the articulated agents are violating the hold constraint
         for grasp_mgr in self._sim.agents_mgr.grasp_iter:
             if (
                 grasp_mgr.is_violating_hold_constraint()
-                and self._config.constraint_violation_ends_episode
+                and self._constraint_violation_ends_episode
             ):
                 done = True
                 break
 
         if done:
             rearrange_logger.debug("-" * 10)
             rearrange_logger.debug("------ Episode Over --------")
@@ -310,15 +338,15 @@
         max_articulated_agent_force = get_max_force(
             contact_points, articulated_agent_id
         )
         return max_articulated_agent_force, max_obj_force, max_force
 
     def get_cur_collision_info(self, agent_idx) -> CollisionDetails:
         _, coll_details = rearrange_collision(
-            self._sim, self._config.count_obj_collisions, agent_idx=agent_idx
+            self._sim, self._count_obj_collisions, agent_idx=agent_idx
         )
         return coll_details
 
     def get_n_targets(self) -> int:
         return self.n_objs
 
     @property
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 from habitat.core.embodied_task import Measure
 from habitat.core.registry import registry
 from habitat.core.simulator import Sensor, SensorTypes
 from habitat.tasks.rearrange.rearrange_sensors import (
     DoesWantTerminate,
     RearrangeReward,
 )
-from habitat.tasks.rearrange.utils import (
-    UsesArticulatedAgentInterface,
-    get_angle_to_pos,
-)
+from habitat.tasks.rearrange.utils import UsesArticulatedAgentInterface
 from habitat.tasks.utils import cartesian_to_polar
 
 BASE_ACTION_NAME = "base_velocity"
 
 
 @registry.register_sensor
 class NavGoalPointGoalSensor(UsesArticulatedAgentInterface, Sensor):
@@ -210,17 +207,28 @@
         self.update_metric(
             *args,
             **kwargs,
         )
 
     def update_metric(self, *args, episode, task, observations, **kwargs):
         targ = task.nav_goal_pos
+        # Get the agent
         robot = self._sim.articulated_agent
+        # Get the base transformation
         T = robot.base_transformation
-        angle = get_angle_to_pos(T.transform_vector(targ))
+        # Do transformation
+        pos = T.inverted().transform_point(targ)
+        # Project to 2D plane (x,y,z=0)
+        pos[2] = 0.0
+        # Unit vector of the pos
+        pos = pos.normalized()
+        # Define the coordinate of the robot
+        pos_robot = np.array([1.0, 0.0, 0.0])
+        # Get the angle
+        angle = np.arccos(np.dot(pos, pos_robot))
         self._metric = np.abs(float(angle))
 
 
 @registry.register_measure
 class NavToPosSucc(Measure):
     cls_uuid: str = "nav_to_pos_success"
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,20 @@
             dataset=dataset,
             should_place_articulated_agent=False,
             **kwargs,
         )
         self.force_obj_to_idx = None
         self.force_recep_to_name = None
 
+        # Set config options
+        self._object_in_hand_sample_prob = (
+            self._config.object_in_hand_sample_prob
+        )
+        self._min_start_distance = self._config.min_start_distance
+
         self._nav_to_info = None
 
     @property
     def nav_goal_pos(self):
         return self._nav_to_info.nav_goal_pos
 
     def set_args(self, obj, **kwargs):
@@ -71,15 +77,15 @@
         """
 
         start_hold_obj_idx: Optional[int] = None
 
         # Only change the scene if this skill is not running as a sub-task
         if (
             force_idx is None
-            and random.random() < self._config.object_in_hand_sample_prob
+            and random.random() < self._object_in_hand_sample_prob
         ):
             start_hold_obj_idx = self._generate_snap_to_obj()
 
         if start_hold_obj_idx is None:
             # Select an object at random and navigate to that object.
             all_pos = self._sim.get_target_objs_start()
             if force_idx is None:
@@ -90,15 +96,15 @@
             # Select a goal at random and navigate to that goal.
             _, all_pos = self._sim.get_targets()
             nav_to_pos = all_pos[np.random.randint(0, len(all_pos))]
 
         def filter_func(start_pos, _):
             return (
                 np.linalg.norm(start_pos - nav_to_pos)
-                > self._config.min_start_distance
+                > self._min_start_distance
             )
 
         (
             articulated_agent_pos,
             articulated_agent_angle,
         ) = self._sim.set_articulated_agent_base_to_random_point(
             filter_func=filter_func
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/pick_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         snapped_id = self._sim.grasp_mgr.snap_idx
         cur_picked = snapped_id is not None
 
         if cur_picked:
             dist_to_goal = ee_to_rest_distance
         else:
-            dist_to_goal = ee_to_object_distance[str(task.abs_targ_idx)]
+            dist_to_goal = ee_to_object_distance[str(task.targ_idx)]
 
         abs_targ_obj_idx = self._sim.scene_obj_ids[task.abs_targ_idx]
 
         did_pick = cur_picked and (not self._prev_picked)
         if did_pick:
             if snapped_id == abs_targ_obj_idx:
                 self._metric += self._config.pick_reward
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/pick_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,18 @@
             dataset=dataset,
             should_place_articulated_agent=False,
             **kwargs,
         )
 
         self.prev_colls = None
         self.force_set_idx = None
+        self._base_angle_noise = self._config.base_angle_noise
+        self._spawn_max_dist_to_obj = self._config.spawn_max_dist_to_obj
+        self._num_spawn_attempts = self._config.num_spawn_attempts
+        self._physics_stability_steps = self._config.physics_stability_steps
 
     def set_args(self, obj, **kwargs):
         self.force_set_idx = obj
 
     def _get_targ_pos(self, sim):
         scene_pos = sim.get_scene_pos()
         targ_idxs = sim.get_targets()[0]
@@ -52,19 +56,19 @@
 
     def _gen_start_pos(self, sim, episode, sel_idx):
         target_positions = self._get_targ_pos(sim)
         targ_pos = target_positions[sel_idx]
 
         start_pos, angle_to_obj, was_fail = get_robot_spawns(
             targ_pos,
-            self._config.base_angle_noise,
-            self._config.spawn_max_dist_to_obj,
+            self._base_angle_noise,
+            self._spawn_max_dist_to_obj,
             sim,
-            self._config.num_spawn_attempts,
-            self._config.physics_stability_steps,
+            self._num_spawn_attempts,
+            self._physics_stability_steps,
         )
 
         if was_fail:
             rearrange_logger.error(
                 f"Episode {episode.episode_id} failed to place robot"
             )
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/place_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,24 +72,24 @@
             ObjectToGoalDistance.cls_uuid
         ].get_metric()
         ee_to_rest_distance = task.measurements.measures[
             EndEffectorToRestDistance.cls_uuid
         ].get_metric()
         obj_at_goal = task.measurements.measures[
             ObjAtGoal.cls_uuid
-        ].get_metric()[str(task.abs_targ_idx)]
+        ].get_metric()[str(task.targ_idx)]
 
         snapped_id = self._sim.grasp_mgr.snap_idx
         cur_picked = snapped_id is not None
 
         if (not obj_at_goal) or cur_picked:
             if self._config.use_ee_dist:
-                dist_to_goal = ee_to_goal_dist[str(task.abs_targ_idx)]
+                dist_to_goal = ee_to_goal_dist[str(task.targ_idx)]
             else:
-                dist_to_goal = obj_to_goal_dist[str(task.abs_targ_idx)]
+                dist_to_goal = obj_to_goal_dist[str(task.targ_idx)]
             min_dist = self._config.min_dist_to_goal
         else:
             dist_to_goal = ee_to_rest_distance
             min_dist = 0.0
 
         if (not self._prev_dropped) and (not cur_picked):
             self._prev_dropped = True
@@ -154,15 +154,15 @@
             observations=observations,
             **kwargs
         )
 
     def update_metric(self, *args, episode, task, observations, **kwargs):
         is_obj_at_goal = task.measurements.measures[
             ObjAtGoal.cls_uuid
-        ].get_metric()[str(task.abs_targ_idx)]
+        ].get_metric()[str(task.targ_idx)]
         is_holding = self._sim.grasp_mgr.is_grasped
 
         ee_to_rest_distance = task.measurements.measures[
             EndEffectorToRestDistance.cls_uuid
         ].get_metric()
 
         self._metric = (
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/place_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/reach_sensors.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/sub_tasks/reach_task.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/rearrange/utils.py` & `habitat-lab-0.2.520230729/habitat/tasks/rearrange/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 import os
 import os.path as osp
 import pickle
 import time
+from functools import wraps
 from typing import List, Optional, Tuple
 
 import attr
 import magnum as mn
 import numpy as np
 import quaternion
 
@@ -404,45 +405,62 @@
 
     :param target_position: The position of the target. This point is not
         necessarily on the navmesh.
     :param rotation_perturbation_noise: The amount of noise to add to the robot's rotation.
     :param distance_threshold: The maximum distance from the target.
     :param sim: The simulator instance.
     :param num_spawn_attempts: The number of sample attempts for the distance threshold.
-    :param physics_stability_steps: The number of steps to perform for physics stability check.
+    :param physics_stability_steps: The number of steps to perform for physics stability check. If specified as 0, then it will return the result without doing any checks.
     :param agent: The agent to set the position for. If not specified, defaults to the simulator default agent.
 
     :return: The robot's start position, rotation, and whether the placement was a failure (True for failure, False for success).
     """
-
-    state = sim.capture_state()
     if agent is None:
         agent = sim.articulated_agent
+    start_rotation = agent.base_rot
+    start_position = agent.base_pos
+
+    state = sim.capture_state()
 
     # Try to place the robot.
     for _ in range(num_spawn_attempts):
         sim.set_state(state)
-        start_position = sim.pathfinder.get_random_navigable_point_near(
-            target_position, distance_threshold
-        )
 
-        relative_target = target_position - start_position
+        if distance_threshold == -1.0:
+            # Place as close to the object as possible.
+            if not sim.is_point_within_bounds(target_position):
+                rearrange_logger.error(
+                    f"Object {target_position} is out of bounds but trying to set robot position"
+                )
 
+            start_position = sim.safe_snap_point(target_position)
+        else:
+            # Place within `distance_threshold` of the object.
+            start_position = sim.pathfinder.get_random_navigable_point_near(
+                target_position, distance_threshold
+            )
+        # Face the robot towards the object.
+        relative_target = target_position - start_position
         angle_to_object = get_angle_to_pos(relative_target)
+        rotation_noise = np.random.normal(0.0, rotation_perturbation_noise)
+        start_rotation = angle_to_object + rotation_noise
+
+        if physics_stability_steps == 0:
+            return start_position, start_rotation, False
+
+        island_idx = sim.pathfinder.get_island(start_position)
+        if island_idx != sim.largest_island_idx:
+            continue
 
         target_distance = np.linalg.norm(
             (start_position - target_position)[[0, 2]]
         )
 
         is_navigable = sim.pathfinder.is_navigable(start_position)
 
-        # Face the robot towards the object.
-        rotation_noise = np.random.normal(0.0, rotation_perturbation_noise)
-        start_rotation = angle_to_object + rotation_noise
-
         if target_distance > distance_threshold or not is_navigable:
             continue
 
         agent.base_pos = start_position
         agent.base_rot = start_rotation
 
         # Make sure the robot is not colliding with anything in this
@@ -481,7 +499,52 @@
     rel_pos = rel_pos[[0, 2]]
 
     heading_angle = get_angle(forward, rel_pos)
     c = np.cross(forward, rel_pos) < 0
     if not c:
         heading_angle = -1.0 * heading_angle
     return heading_angle
+
+
+def add_perf_timing_func(name: Optional[str] = None):
+    """
+    Function decorator for logging the speed of a method to the RearrangeSim.
+    This must either be applied to methods from RearrangeSim or to methods from
+    objects that contain `self._sim` so this decorator can access the
+    underlying `RearrangeSim` instance to log the speed. This scopes the
+    logging name so nested function calls will include the outer perf timing
+    name separate by a ".".
+
+    :param name: The name of the performance logging key. If unspecified, this
+        defaults to "ModuleName[FuncName]"
+    """
+
+    def perf_time(f):
+        if name is None:
+            module_name = f.__module__.split(".")[-1]
+            use_name = f"{module_name}[{f.__name__}]"
+        else:
+            use_name = name
+
+        @wraps(f)
+        def wrapper(self, *args, **kwargs):
+            if hasattr(self, "add_perf_timing") and hasattr(
+                self, "cur_runtime_perf_scope"
+            ):
+                sim = self
+            else:
+                sim = self._sim
+
+            if not hasattr(sim, "add_perf_timing"):
+                # Does not support logging.
+                return f(self, *args, **kwargs)
+
+            sim.cur_runtime_perf_scope.append(use_name)
+            t_start = time.time()
+            ret = f(self, *args, **kwargs)
+            sim.add_perf_timing("", t_start)
+            sim.cur_runtime_perf_scope.pop()
+            return ret
+
+        return wrapper
+
+    return perf_time
```

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/registration.py` & `habitat-lab-0.2.520230729/habitat/tasks/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/utils.py` & `habitat-lab-0.2.520230729/habitat/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/vln/__init__.py` & `habitat-lab-0.2.520230729/habitat/tasks/vln/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/tasks/vln/vln.py` & `habitat-lab-0.2.520230729/habitat/tasks/vln/vln.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/common.py` & `habitat-lab-0.2.520230729/habitat/utils/common.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/env_utils.py` & `habitat-lab-0.2.520230729/habitat/utils/env_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 from habitat.datasets import make_dataset
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
 
 def make_env_fn(
-    config: "DictConfig", env_class: Union[Type[Env], Type[RLEnv]]
+    config: "DictConfig",
+    env_class: Union[Type[Env], Type[RLEnv]],
+    dataset=None,
 ) -> Union[Env, RLEnv]:
     r"""Creates an env of type env_class with specified config and rank.
     This is to be passed in as an argument when creating VectorEnv.
 
     Args:
         config: root exp config that has core env config node as well as
             env-specific config node.
         env_class: class type of the env to be created.
+        dataset: If specified, load the environment using this dataset.
 
     Returns:
         env object created according to specification.
     """
     if "habitat" in config:
         config = config.habitat
-    dataset = make_dataset(config.dataset.type, config=config.dataset)
+    if dataset is None:
+        dataset = make_dataset(config.dataset.type, config=config.dataset)
     env = env_class(config=config, dataset=dataset)
     env.seed(config.seed)
     return env
```

### Comparing `habitat-lab-0.2.420230405/habitat/utils/geometry_utils.py` & `habitat-lab-0.2.520230729/habitat/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/pickle5_multiprocessing.py` & `habitat-lab-0.2.520230729/habitat/utils/pickle5_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/profiling_wrapper.py` & `habitat-lab-0.2.520230729/habitat/utils/profiling_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/test_utils.py` & `habitat-lab-0.2.520230729/habitat/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png` & `habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/visualizations/fog_of_war.py` & `habitat-lab-0.2.520230729/habitat/utils/visualizations/fog_of_war.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/visualizations/maps.py` & `habitat-lab-0.2.520230729/habitat/utils/visualizations/maps.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat/utils/visualizations/utils.py` & `habitat-lab-0.2.520230729/habitat/utils/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.420230405/habitat_lab.egg-info/PKG-INFO` & `habitat-lab-0.2.520230729/habitat_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-lab
-Version: 0.2.420230405
+Version: 0.2.520230729
 Summary: Habitat-Lab: a modular high-level library for end-to-end development in Embodied AI.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-lab-0.2.420230405/habitat_lab.egg-info/SOURCES.txt` & `habitat-lab-0.2.520230729/habitat_lab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,20 @@
 habitat/config/benchmark/nav/imagenav/imagenav_gibson.yaml
 habitat/config/benchmark/nav/imagenav/imagenav_mp3d.yaml
 habitat/config/benchmark/nav/imagenav/imagenav_test.yaml
 habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml
 habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml
 habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml
 habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml
+habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml
+habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml
 habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml
 habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml
+habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml
+habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_base.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_gibson.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_habitat_test.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_hm3d.yaml
 habitat/config/benchmark/nav/pointnav/pointnav_mp3d.yaml
 habitat/config/benchmark/rearrange/close_cab.yaml
@@ -50,15 +54,14 @@
 habitat/config/benchmark/rearrange/idle.yaml
 habitat/config/benchmark/rearrange/idle_single_camera.yaml
 habitat/config/benchmark/rearrange/interact.yaml
 habitat/config/benchmark/rearrange/nav_to_obj.yaml
 habitat/config/benchmark/rearrange/open_cab.yaml
 habitat/config/benchmark/rearrange/open_fridge.yaml
 habitat/config/benchmark/rearrange/pick.yaml
-habitat/config/benchmark/rearrange/pick_spa.yaml
 habitat/config/benchmark/rearrange/place.yaml
 habitat/config/benchmark/rearrange/play.yaml
 habitat/config/benchmark/rearrange/play_human.yaml
 habitat/config/benchmark/rearrange/play_spot.yaml
 habitat/config/benchmark/rearrange/play_stretch.yaml
 habitat/config/benchmark/rearrange/prepare_groceries.yaml
 habitat/config/benchmark/rearrange/reach_state.yaml
@@ -69,15 +72,17 @@
 habitat/config/benchmark/rearrange/tidy_house.yaml
 habitat/config/habitat/dataset/eqa/mp3d.yaml
 habitat/config/habitat/dataset/imagenav/gibson.yaml
 habitat/config/habitat/dataset/imagenav/mp3d.yaml
 habitat/config/habitat/dataset/instance_imagenav/hm3d_v1.yaml
 habitat/config/habitat/dataset/instance_imagenav/hm3d_v2.yaml
 habitat/config/habitat/dataset/objectnav/hm3d.yaml
+habitat/config/habitat/dataset/objectnav/hssd-hab.yaml
 habitat/config/habitat/dataset/objectnav/mp3d.yaml
+habitat/config/habitat/dataset/objectnav/procthor-hab.yaml
 habitat/config/habitat/dataset/pointnav/gibson.yaml
 habitat/config/habitat/dataset/pointnav/gibson_0_plus.yaml
 habitat/config/habitat/dataset/pointnav/gibson_v2.yaml
 habitat/config/habitat/dataset/pointnav/habitat_test.yaml
 habitat/config/habitat/dataset/pointnav/hm3d.yaml
 habitat/config/habitat/dataset/pointnav/mp3d.yaml
 habitat/config/habitat/dataset/rearrangement/replica_cad.yaml
@@ -103,26 +108,27 @@
 habitat/config/habitat/task/vln_r2r.yaml
 habitat/config/habitat/task/rearrange/close_cab.yaml
 habitat/config/habitat/task/rearrange/close_fridge.yaml
 habitat/config/habitat/task/rearrange/nav_to_obj.yaml
 habitat/config/habitat/task/rearrange/open_cab.yaml
 habitat/config/habitat/task/rearrange/open_fridge.yaml
 habitat/config/habitat/task/rearrange/pick.yaml
-habitat/config/habitat/task/rearrange/pick_spa.yaml
 habitat/config/habitat/task/rearrange/place.yaml
 habitat/config/habitat/task/rearrange/play.yaml
 habitat/config/habitat/task/rearrange/play_human.yaml
 habitat/config/habitat/task/rearrange/prepare_groceries.yaml
 habitat/config/habitat/task/rearrange/reach_state.yaml
 habitat/config/habitat/task/rearrange/rearrange.yaml
 habitat/config/habitat/task/rearrange/rearrange_easy.yaml
 habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml
 habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml
 habitat/config/habitat/task/rearrange/set_table.yaml
 habitat/config/habitat/task/rearrange/tidy_house.yaml
+habitat/config/habitat/task/rearrange/agents/fetch_arm.yaml
+habitat/config/habitat/task/rearrange/agents/fetch_base_arm.yaml
 habitat/config/habitat/task/rearrange/demo/idle.yaml
 habitat/config/habitat/task/rearrange/demo/interact.yaml
 habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml
 habitat/config/habitat/task/rearrange/pddl/rearrange.yaml
 habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml
 habitat/config/habitat/task/rearrange/pddl/set_table.yaml
 habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml
@@ -136,14 +142,17 @@
 habitat/core/environments.py
 habitat/core/logging.py
 habitat/core/registry.py
 habitat/core/simulator.py
 habitat/core/spaces.py
 habitat/core/utils.py
 habitat/core/vector_env.py
+habitat/core/batch_rendering/__init__.py
+habitat/core/batch_rendering/env_batch_renderer.py
+habitat/core/batch_rendering/env_batch_renderer_constants.py
 habitat/datasets/__init__.py
 habitat/datasets/registration.py
 habitat/datasets/utils.py
 habitat/datasets/eqa/__init__.py
 habitat/datasets/eqa/mp3d_eqa_dataset.py
 habitat/datasets/image_nav/__init__.py
 habitat/datasets/image_nav/instance_image_nav_dataset.py
```

### Comparing `habitat-lab-0.2.420230405/setup.py` & `habitat-lab-0.2.520230729/setup.py`

 * *Files identical despite different names*

