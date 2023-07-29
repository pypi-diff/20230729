# Comparing `tmp/rlgym-1.2.1.tar.gz` & `tmp/rlgym-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rlgym-1.2.1.tar", last modified: Mon Jun 12 22:11:29 2023, max compression
+gzip compressed data, was "dist/rlgym-1.2.2.tar", last modified: Sat Jul 29 21:33:23 2023, max compression
```

## Comparing `rlgym-1.2.1.tar` & `rlgym-1.2.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-12 22:11:22.000000 rlgym-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 22:11:22.000000 rlgym-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 22:11:29.000000 rlgym-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 22:11:22.000000 rlgym-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/communication_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/communication_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/communication/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/envs/match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/gamelaunch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/epic_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gamelaunch/paging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)   252928 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/plugin/RLGym.dll
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/plugin/RLMultiInjector.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/action_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/continuous_act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/default_act.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/action_parsers/discrete_act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/common_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/gamestates/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/game_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/physics_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/gamestates/player_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/obs_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/advanced_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/default_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/obs_builders/obs_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/reward_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/combined_reward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/misc_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/default_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/reward_functions/reward_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/state_setters/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/default_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/state_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/state_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/car_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/physics_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/state_setters/wrappers/state_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/common_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/utils/terminal_conditions/terminal_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-12 22:11:22.000000 rlgym-1.2.1/rlgym/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 22:11:29.000000 rlgym-1.2.1/rlgym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:11:29.000000 rlgym-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-12 22:11:22.000000 rlgym-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/cases/boost_pad_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:29.000000 rlgym-1.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/setter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 22:11:22.000000 rlgym-1.2.1/tests/utils/state_obs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-29 21:33:17.000000 rlgym-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 21:33:17.000000 rlgym-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-29 21:33:23.000000 rlgym-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-29 21:33:17.000000 rlgym-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/communication/communication_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/communication/communication_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/communication/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/envs/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/envs/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/gamelaunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gamelaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gamelaunch/epic_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gamelaunch/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gamelaunch/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gamelaunch/paging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)   252928 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/plugin/RLGym.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/plugin/RLMultiInjector.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/action_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/action_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/action_parsers/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/action_parsers/continuous_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/action_parsers/default_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/action_parsers/discrete_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/common_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/gamestates/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/gamestates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/gamestates/game_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/gamestates/physics_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/gamestates/player_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/obs_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/obs_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/obs_builders/advanced_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/obs_builders/default_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/obs_builders/obs_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/reward_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/combined_reward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/misc_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/default_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/reward_functions/reward_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/state_setters/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/default_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/state_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/state_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/state_setters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/wrappers/car_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/wrappers/physics_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/state_setters/wrappers/state_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym/utils/terminal_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/terminal_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/terminal_conditions/common_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/utils/terminal_conditions/terminal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-29 21:33:17.000000 rlgym-1.2.2/rlgym/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 21:33:23.000000 rlgym-1.2.2/rlgym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:33:23.000000 rlgym-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-29 21:33:17.000000 rlgym-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/cases/boost_pad_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:23.000000 rlgym-1.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/utils/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/utils/setter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-29 21:33:17.000000 rlgym-1.2.2/tests/utils/state_obs.py
```

### Comparing `rlgym-1.2.1/LICENSE` & `rlgym-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/PKG-INFO` & `rlgym-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://github.com/lucas-emery/rocket-league-gym
 Author: Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # The Rocket League Gym
         This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
         
@@ -29,9 +29,9 @@
         
 Keywords: rocket-league,gym,reinforcement-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7,<=3.9
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
```

### Comparing `rlgym-1.2.1/README.md` & `rlgym-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/communication/communication_exception_handler.py` & `rlgym-1.2.2/rlgym/communication/communication_exception_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/communication/communication_handler.py` & `rlgym-1.2.2/rlgym/communication/communication_handler.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/communication/message.py` & `rlgym-1.2.2/rlgym/communication/message.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/envs/environment.py` & `rlgym-1.2.2/rlgym/envs/environment.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/envs/match.py` & `rlgym-1.2.2/rlgym/envs/match.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/gamelaunch/epic_launch.py` & `rlgym-1.2.2/rlgym/gamelaunch/epic_launch.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/gamelaunch/launch.py` & `rlgym-1.2.2/rlgym/gamelaunch/launch.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/gamelaunch/minimize.py` & `rlgym-1.2.2/rlgym/gamelaunch/minimize.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/gamelaunch/paging.py` & `rlgym-1.2.2/rlgym/gamelaunch/paging.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/gym.py` & `rlgym-1.2.2/rlgym/gym.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/make.py` & `rlgym-1.2.2/rlgym/make.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/plugin/RLGym.dll` & `rlgym-1.2.2/rlgym/plugin/RLGym.dll`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/plugin/RLMultiInjector.exe` & `rlgym-1.2.2/rlgym/plugin/RLMultiInjector.exe`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/action_parsers/action_parser.py` & `rlgym-1.2.2/rlgym/utils/action_parsers/action_parser.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/action_parsers/continuous_act.py` & `rlgym-1.2.2/rlgym/utils/action_parsers/continuous_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/action_parsers/default_act.py` & `rlgym-1.2.2/rlgym/utils/action_parsers/default_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/action_parsers/discrete_act.py` & `rlgym-1.2.2/rlgym/utils/action_parsers/discrete_act.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/common_values.py` & `rlgym-1.2.2/rlgym/utils/common_values.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,46 @@
 SIDE_WALL_X = 4096  # +/-
 BACK_WALL_Y = 5120  # +/-
 CEILING_Z = 2044
 BACK_NET_Y = 6000  # +/-
 
 GOAL_HEIGHT = 642.775
+GOAL_CENTER_TO_POST = 892.755
 
 ORANGE_GOAL_CENTER = (0, BACK_WALL_Y, GOAL_HEIGHT / 2)
 BLUE_GOAL_CENTER = (0, -BACK_WALL_Y, GOAL_HEIGHT / 2)
 
 # Often more useful than center
 ORANGE_GOAL_BACK = (0, BACK_NET_Y, GOAL_HEIGHT / 2)
 BLUE_GOAL_BACK = (0, -BACK_NET_Y, GOAL_HEIGHT / 2)
 
+ORANGE_GOAL_TOP_LEFT = (GOAL_CENTER_TO_POST, BACK_WALL_Y, GOAL_HEIGHT)
+BLUE_GOAL_TOP_LEFT = (-GOAL_CENTER_TO_POST, -BACK_WALL_Y, GOAL_HEIGHT)
+
+ORANGE_GOAL_TOP_RIGHT = (-GOAL_CENTER_TO_POST, BACK_WALL_Y, GOAL_HEIGHT)
+BLUE_GOAL_TOP_RIGHT = (GOAL_CENTER_TO_POST, -BACK_WALL_Y, GOAL_HEIGHT)
+
+ORANGE_GOAL_BOTTOM_LEFT = (GOAL_CENTER_TO_POST, BACK_WALL_Y, 0)
+BLUE_GOAL_BOTTOM_LEFT = (-GOAL_CENTER_TO_POST, -BACK_WALL_Y, 0)
+
+ORANGE_GOAL_BOTTOM_RIGHT = (-GOAL_CENTER_TO_POST, BACK_WALL_Y, 0)
+BLUE_GOAL_BOTTOM_RIGHT = (GOAL_CENTER_TO_POST, -BACK_WALL_Y, 0)
+
+ORANGE_FIELD_TOP_LEFT = (SIDE_WALL_X, BACK_WALL_Y, CEILING_Z)
+BLUE_FIELD_TOP_LEFT = (-SIDE_WALL_X, -BACK_WALL_Y, CEILING_Z)
+
+ORANGE_FIELD_TOP_RIGHT = (-SIDE_WALL_X, BACK_WALL_Y, CEILING_Z)
+BLUE_FIELD_TOP_RIGHT = (SIDE_WALL_X, -BACK_WALL_Y, CEILING_Z)
+
+ORANGE_FIELD_BOTTOM_LEFT = (SIDE_WALL_X, BACK_WALL_Y, 0)
+BLUE_FIELD_BOTTOM_LEFT = (-SIDE_WALL_X, -BACK_WALL_Y, 0)
+
+ORANGE_FIELD_BOTTOM_RIGHT = (-SIDE_WALL_X, BACK_WALL_Y, 0)
+BLUE_FIELD_BOTTOM_RIGHT = (SIDE_WALL_X, -BACK_WALL_Y, 0)
+
 BALL_RADIUS = 92.75
 
 BALL_MAX_SPEED = 6000
 CAR_MAX_SPEED = 2300
 SUPERSONIC_THRESHOLD = 2200
 CAR_MAX_ANG_VEL = 5.5
```

### Comparing `rlgym-1.2.1/rlgym/utils/gamestates/game_state.py` & `rlgym-1.2.2/rlgym/utils/gamestates/game_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/gamestates/physics_object.py` & `rlgym-1.2.2/rlgym/utils/gamestates/physics_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,19 @@
 import numpy as np
 from typing import Optional
 
 
 class PhysicsObject(object):
     def __init__(self, position=None, quaternion=None, linear_velocity=None, angular_velocity=None):
         self.position: np.ndarray = position if position is not None else np.zeros(3)
-
-        # ones by default to prevent mathematical errors when converting quat to rot matrix on empty physics state
-        self.quaternion: np.ndarray = quaternion if quaternion is not None else np.ones(4)
-
+        self.quaternion: np.ndarray = quaternion if quaternion is not None else np.array([1, 0, 0, 0], dtype=np.float32)
         self.linear_velocity: np.ndarray = linear_velocity if linear_velocity is not None else np.zeros(3)
         self.angular_velocity: np.ndarray = angular_velocity if angular_velocity is not None else np.zeros(3)
-        self._euler_angles: Optional[np.ndarray] = np.zeros(3)
-        self._rotation_mtx: Optional[np.ndarray] = np.zeros((3,3))
+        self._euler_angles: Optional[np.ndarray] = None
+        self._rotation_mtx: Optional[np.ndarray] = None
         self._has_computed_rot_mtx = False
         self._has_computed_euler_angles = False
 
     def decode_car_data(self, car_data: np.ndarray):
         """
         Function to decode the physics state of a car from the game state array.
         :param car_data: Slice of game state array containing the car data to decode.
```

### Comparing `rlgym-1.2.1/rlgym/utils/gamestates/player_data.py` & `rlgym-1.2.2/rlgym/utils/gamestates/player_data.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/math.py` & `rlgym-1.2.2/rlgym/utils/math.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/obs_builders/advanced_obs.py` & `rlgym-1.2.2/rlgym/utils/obs_builders/advanced_obs.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/obs_builders/default_obs.py` & `rlgym-1.2.2/rlgym/utils/obs_builders/default_obs.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/obs_builders/obs_builder.py` & `rlgym-1.2.2/rlgym/utils/obs_builders/obs_builder.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/combined_reward.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/combined_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/ball_goal_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/conditional_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/misc_rewards.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/misc_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/common_rewards/player_ball_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/default_reward.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/default_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/reward_functions/reward_function.py` & `rlgym-1.2.2/rlgym/utils/reward_functions/reward_function.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/default_state.py` & `rlgym-1.2.2/rlgym/utils/state_setters/default_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/random_state.py` & `rlgym-1.2.2/rlgym/utils/state_setters/random_state.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/state_setter.py` & `rlgym-1.2.2/rlgym/utils/state_setters/state_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/state_wrapper.py` & `rlgym-1.2.2/rlgym/utils/state_setters/state_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/car_wrapper.py` & `rlgym-1.2.2/rlgym/utils/state_setters/wrappers/car_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/physics_wrapper.py` & `rlgym-1.2.2/rlgym/utils/state_setters/wrappers/physics_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/state_setters/wrappers/state_wrapper.py` & `rlgym-1.2.2/rlgym/utils/state_setters/wrappers/state_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/terminal_conditions/common_conditions.py` & `rlgym-1.2.2/rlgym/utils/terminal_conditions/common_conditions.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/utils/terminal_conditions/terminal_condition.py` & `rlgym-1.2.2/rlgym/utils/terminal_conditions/terminal_condition.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/rlgym/version.py` & `rlgym-1.2.2/rlgym/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # From https://github.com/RLBot/RLBot/blob/master/src/main/python/rlbot/version.py
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
 # https://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 release_notes = {
     'beta':
     """
     - This version contains numerous untested and potentially breaking changes. Run at your own risk.
     """,
+    '1.2.2':
+    """
+    - Fixed max python version
+    """,
     '1.2.1':
     """
     - Fixed epic version crashing instantly - Bakkes
     - Added max python version
     - Added ActionParser to utils submodule
     - Updated default reward, it now minimizes linear velocity instead of angular
     - RIP RhobotObs
```

### Comparing `rlgym-1.2.1/rlgym.egg-info/PKG-INFO` & `rlgym-1.2.2/rlgym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python API that can be used to treat the game Rocket League as an Openai Gym-like environment for Reinforcement Learning projects.
 Home-page: https://github.com/lucas-emery/rocket-league-gym
 Author: Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # The Rocket League Gym
         This is a python API that can be used to treat the game [Rocket League](https://www.rocketleague.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects. This API must be used with the accompanying Bakkesmod plugin.
         
@@ -29,9 +29,9 @@
         
 Keywords: rocket-league,gym,reinforcement-learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7,<=3.9
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
```

### Comparing `rlgym-1.2.1/rlgym.egg-info/SOURCES.txt` & `rlgym-1.2.2/rlgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/setup.py` & `rlgym-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     install_requires=[
         'gym>=0.17',
         'numpy>=1.19',
         'pywin32==228',
         'pywinauto==0.6.8',
         'psutil>=5.8',
     ],
-    python_requires='>=3.7,<=3.9',
+    python_requires='>=3.7,<3.10',
     cmdclass={'install': CustomInstall},
     license='Apache 2.0',
     license_file='LICENSE',
     keywords=['rocket-league', 'gym', 'reinforcement-learning'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `rlgym-1.2.1/tests/cases/boost_pad_test.py` & `rlgym-1.2.2/tests/cases/boost_pad_test.py`

 * *Files identical despite different names*

### Comparing `rlgym-1.2.1/tests/run_tests.py` & `rlgym-1.2.2/tests/run_tests.py`

 * *Files identical despite different names*

