# Comparing `tmp/habitat-baselines-0.2.420230405.tar.gz` & `tmp/habitat-baselines-0.2.520230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habitat-baselines-0.2.420230405.tar", last modified: Wed Apr  5 18:53:36 2023, max compression
+gzip compressed data, was "habitat-baselines-0.2.520230729.tar", last modified: Sat Jul 29 05:48:39 2023, max compression
```

## Comparing `habitat-baselines-0.2.420230405.tar` & `habitat-baselines-0.2.520230729.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       88 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4857 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.795164 habitat-baselines-0.2.420230405/habitat_baselines/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1049 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.795164 habitat-baselines-0.2.420230405/habitat_baselines/agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      280 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/agents/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/agents/ppo_agents.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4929 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/agents/simple_agents.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/base_il_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13480 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/base_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/baseline_registry.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3680 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/construct_vector_env.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      534 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/env_spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      511 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47017 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/obs_transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9419 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/rollout_storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1027 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12086 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/tensor_dict.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/tensorboard_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2141 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/common/windowed_running_mean.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1604 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/config/default.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14422 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/config/default_structured_configs.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/il/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/il/data/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/data/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9286 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/data/data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/data/eqa_cnn_pretrain_data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19248 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/data/nav_data.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3620 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/metrics.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/il/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23402 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/models/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       30 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9920 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26493 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/pacman_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14516 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/vqa_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/py.typed
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/rl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/algo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/algo/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5007 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/algo/ddppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14526 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/ddp_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.799164 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      301 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8222 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/resnet.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21267 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/resnet_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2891 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        6 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.803164 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14668 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hierarchical_policy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.803164 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3901 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/fixed_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3582 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/high_level_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7421 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/neural_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3925 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hrl_ppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7785 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hrl_rollout_storage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.803164 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1080 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2212 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/art_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2386 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7634 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/nn_skill.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/noop.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4882 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/oracle_nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2114 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/pick.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1997 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/place.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2895 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/reset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12443 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/skill.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1423 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      924 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.803164 habitat-baselines-0.2.420230405/habitat_baselines/rl/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4610 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/models/action_embedding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14957 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/models/rnn_state_encoder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5488 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/models/simple_cnn.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.803164 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      528 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3820 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/agent_access_mgr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11534 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/cpc_aux_loss.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14445 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11997 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/ppo.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39728 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/ppo_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10165 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/single_agent_access_mgr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      326 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/updater.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       64 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/requirements.txt
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10807 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/environment_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20945 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/inference_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14349 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/preemption_decider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14483 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/report_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/task_enums.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1743 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/timing.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23391 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/ver_rollout_storage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20522 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/ver_trainer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6394 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/worker_common.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     2660 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/run.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/habitat_baselines/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      258 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24850 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1841 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/utils/info_dict.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/habitat_baselines/utils/visualizations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      284 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/utils/visualizations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4229 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/utils/visualizations/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/habitat_baselines/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 18:53:36.795164 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4240 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       65 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       18 2023-04-05 18:53:36.000000 habitat-baselines-0.2.420230405/habitat_baselines.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-04-05 18:53:36.807165 habitat-baselines-0.2.420230405/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2558 2023-04-05 18:52:58.000000 habitat-baselines-0.2.420230405/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       88 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4857 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1049 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      280 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/ppo_agents.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4929 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/agents/simple_agents.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/base_il_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13480 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/base_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/baseline_registry.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/env_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      534 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/env_spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4697 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/habitat_env_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      511 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47017 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/obs_transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9561 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/rollout_storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1027 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12061 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/tensor_dict.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/tensorboard_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2141 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/common/windowed_running_mean.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1604 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/default.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/config/default_structured_configs.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/data/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9286 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/eqa_cnn_pretrain_data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19248 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/data/nav_data.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3620 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/metrics.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23402 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/models/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       30 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9920 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26493 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/pacman_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14516 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/vqa_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/py.typed
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5451 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/ddppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14526 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/ddp_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.704371 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      301 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8222 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26845 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2891 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        6 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22462 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hierarchical_policy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4359 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/fixed_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3763 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/high_level_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7469 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/neural_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3925 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_ppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7858 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_rollout_storage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1080 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2212 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/art_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2712 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nn_skill.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/noop.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4882 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/oracle_nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2114 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/pick.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2005 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/place.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3009 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/reset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11880 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/skill.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1423 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      937 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4610 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/action_embedding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14957 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/rnn_state_encoder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5488 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/models/simple_cnn.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.708372 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      528 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3849 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/agent_access_mgr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11534 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/cpc_aux_loss.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15171 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12710 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44038 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10138 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/single_agent_access_mgr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/updater.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/requirements.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10806 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/environment_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20944 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/inference_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14349 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/preemption_decider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14483 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/report_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/requirements.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/task_enums.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23285 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_rollout_storage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20595 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_trainer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6394 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/worker_common.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     2660 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/run.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      258 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24850 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2201 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/info_dict.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/timing.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      284 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4229 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/habitat_baselines/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:39.700369 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5936 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4278 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       65 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       18 2023-07-29 05:48:39.000000 habitat-baselines-0.2.520230729/habitat_baselines.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-07-29 05:48:39.712374 habitat-baselines-0.2.520230729/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2558 2023-07-29 05:48:00.000000 habitat-baselines-0.2.520230729/setup.py
```

### Comparing `habitat-baselines-0.2.420230405/PKG-INFO` & `habitat-baselines-0.2.520230729/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-baselines
-Version: 0.2.420230405
+Version: 0.2.520230729
 Summary: Habitat-Baselines: Embodied AI baselines.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-baselines-0.2.420230405/README.md` & `habitat-baselines-0.2.520230729/README.md`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/__init__.py` & `habitat-baselines-0.2.520230729/habitat_baselines/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/agents/ppo_agents.py` & `habitat-baselines-0.2.520230729/habitat_baselines/agents/ppo_agents.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/agents/simple_agents.py` & `habitat-baselines-0.2.520230729/habitat_baselines/agents/simple_agents.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/base_il_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/base_il_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/base_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/base_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/baseline_registry.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/baseline_registry.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/construct_vector_env.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/habitat_env_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,95 +5,116 @@
 import os
 import random
 from typing import TYPE_CHECKING, Any, List, Type
 
 from habitat import ThreadedVectorEnv, VectorEnv, logger, make_dataset
 from habitat.config import read_write
 from habitat.gym import make_gym_from_config
+from habitat_baselines.common.env_factory import VectorEnvFactory
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
 
-def construct_envs(
-    config: "DictConfig",
-    workers_ignore_signals: bool = False,
-    enforce_scenes_greater_eq_environments: bool = False,
-) -> VectorEnv:
-    r"""Create VectorEnv object with specified config and env class type.
-    To allow better performance, dataset are split into small ones for
-    each individual env, grouped by scenes.
-
-    :param config: configs that contain num_environments as well as information
-    :param necessary to create individual environments.
-    :param workers_ignore_signals: Passed to :ref:`habitat.VectorEnv`'s constructor
-    :param enforce_scenes_greater_eq_environments: Make sure that there are more (or equal)
-        scenes than environments. This is needed for correct evaluation.
-
-    :return: VectorEnv object created according to specification.
-    """
-
-    num_environments = config.habitat_baselines.num_environments
-    configs = []
-    dataset = make_dataset(config.habitat.dataset.type)
-    scenes = config.habitat.dataset.content_scenes
-    if "*" in config.habitat.dataset.content_scenes:
-        scenes = dataset.get_scenes_to_load(config.habitat.dataset)
-
-    if num_environments < 1:
-        raise RuntimeError("num_environments must be strictly positive")
-
-    if len(scenes) == 0:
-        raise RuntimeError(
-            "No scenes to load, multiple process logic relies on being able to split scenes uniquely between processes"
-        )
+class HabitatVectorEnvFactory(VectorEnvFactory):
+    def construct_envs(
+        self,
+        config: "DictConfig",
+        workers_ignore_signals: bool = False,
+        enforce_scenes_greater_eq_environments: bool = False,
+        is_first_rank: bool = True,
+    ) -> VectorEnv:
+        r"""Create VectorEnv object with specified config and env class type.
+        To allow better performance, dataset are split into small ones for
+        each individual env, grouped by scenes.
+        """
+
+        num_environments = config.habitat_baselines.num_environments
+        configs = []
+        dataset = make_dataset(config.habitat.dataset.type)
+        scenes = config.habitat.dataset.content_scenes
+        if "*" in config.habitat.dataset.content_scenes:
+            scenes = dataset.get_scenes_to_load(config.habitat.dataset)
+
+        if num_environments < 1:
+            raise RuntimeError("num_environments must be strictly positive")
+
+        if len(scenes) == 0:
+            raise RuntimeError(
+                "No scenes to load, multiple process logic relies on being able to split scenes uniquely between processes"
+            )
 
-    random.shuffle(scenes)
+        random.shuffle(scenes)
 
-    scene_splits: List[List[str]] = [[] for _ in range(num_environments)]
-    if len(scenes) < num_environments:
-        msg = f"There are less scenes ({len(scenes)}) than environments ({num_environments}). "
-        if enforce_scenes_greater_eq_environments:
-            logger.warn(
-                msg
-                + "Reducing the number of environments to be the number of scenes."
-            )
-            num_environments = len(scenes)
-            scene_splits = [[s] for s in scenes]
+        scene_splits: List[List[str]] = [[] for _ in range(num_environments)]
+        if len(scenes) < num_environments:
+            msg = f"There are less scenes ({len(scenes)}) than environments ({num_environments}). "
+            if enforce_scenes_greater_eq_environments:
+                logger.warn(
+                    msg
+                    + "Reducing the number of environments to be the number of scenes."
+                )
+                num_environments = len(scenes)
+                scene_splits = [[s] for s in scenes]
+            else:
+                logger.warn(
+                    msg
+                    + "Each environment will use all the scenes instead of using a subset."
+                )
+            for scene in scenes:
+                for split in scene_splits:
+                    split.append(scene)
         else:
+            for idx, scene in enumerate(scenes):
+                scene_splits[idx % len(scene_splits)].append(scene)
+            assert sum(map(len, scene_splits)) == len(scenes)
+
+        for env_index in range(num_environments):
+            proc_config = config.copy()
+            with read_write(proc_config):
+                task_config = proc_config.habitat
+                task_config.seed = task_config.seed + env_index
+                remove_measure_names = []
+                if not is_first_rank:
+                    # Filter out non rank0_measure from the task config if we are not on rank0.
+                    remove_measure_names.extend(
+                        task_config.task.rank0_measure_names
+                    )
+                if (env_index != 0) or not is_first_rank:
+                    # Filter out non-rank0_env0 measures from the task config if we
+                    # are not on rank0 env0.
+                    remove_measure_names.extend(
+                        task_config.task.rank0_env0_measure_names
+                    )
+
+                task_config.task.measurements = {
+                    k: v
+                    for k, v in task_config.task.measurements.items()
+                    if k not in remove_measure_names
+                }
+
+                if len(scenes) > 0:
+                    task_config.dataset.content_scenes = scene_splits[
+                        env_index
+                    ]
+
+            configs.append(proc_config)
+
+        vector_env_cls: Type[Any]
+        if int(os.environ.get("HABITAT_ENV_DEBUG", 0)):
             logger.warn(
-                msg
-                + "Each environment will use all the scenes instead of using a subset."
+                "Using the debug Vector environment interface. Expect slower performance."
             )
-        for scene in scenes:
-            for split in scene_splits:
-                split.append(scene)
-    else:
-        for idx, scene in enumerate(scenes):
-            scene_splits[idx % len(scene_splits)].append(scene)
-        assert sum(map(len, scene_splits)) == len(scenes)
-
-    for i in range(num_environments):
-        proc_config = config.copy()
-        with read_write(proc_config):
-            task_config = proc_config.habitat
-            task_config.seed = task_config.seed + i
-            if len(scenes) > 0:
-                task_config.dataset.content_scenes = scene_splits[i]
-
-        configs.append(proc_config)
-
-    vector_env_cls: Type[Any]
-    if int(os.environ.get("HABITAT_ENV_DEBUG", 0)):
-        logger.warn(
-            "Using the debug Vector environment interface. Expect slower performance."
+            vector_env_cls = ThreadedVectorEnv
+        else:
+            vector_env_cls = VectorEnv
+
+        envs = vector_env_cls(
+            make_env_fn=make_gym_from_config,
+            env_fn_args=tuple((c,) for c in configs),
+            workers_ignore_signals=workers_ignore_signals,
         )
-        vector_env_cls = ThreadedVectorEnv
-    else:
-        vector_env_cls = VectorEnv
-
-    envs = vector_env_cls(
-        make_env_fn=make_gym_from_config,
-        env_fn_args=tuple((c,) for c in configs),
-        workers_ignore_signals=workers_ignore_signals,
-    )
-    return envs
+
+        if config.habitat.simulator.renderer.enable_batch_renderer:
+            envs.initialize_batch_renderer(config)
+
+        return envs
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/env_spec.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/env_spec.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/obs_transformers.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/obs_transformers.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/rollout_storage.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/rollout_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 from habitat_baselines.common.storage import Storage
 from habitat_baselines.common.tensor_dict import DictTree, TensorDict
 from habitat_baselines.rl.models.rnn_state_encoder import (
     build_pack_info_from_dones,
     build_rnn_build_seq_info,
 )
 from habitat_baselines.utils.common import get_action_space_info
+from habitat_baselines.utils.timing import g_timer
 
 
 @baseline_registry.register_storage
 class RolloutStorage(Storage):
     r"""Class for storing rollout information for RL trainers."""
 
     def __init__(
         self,
         numsteps,
         num_envs,
         observation_space,
         action_space,
-        recurrent_hidden_state_size,
-        num_recurrent_layers=1,
+        actor_critic,
         is_double_buffered: bool = False,
     ):
         action_shape, discrete_actions = get_action_space_info(action_space)
 
         self.buffers = TensorDict()
         self.buffers["observations"] = TensorDict()
 
@@ -50,16 +50,16 @@
                     dtype=observation_space.spaces[sensor].dtype,
                 )
             )
 
         self.buffers["recurrent_hidden_states"] = torch.zeros(
             numsteps + 1,
             num_envs,
-            num_recurrent_layers,
-            recurrent_hidden_state_size,
+            actor_critic.num_recurrent_layers,
+            actor_critic.recurrent_hidden_size,
         )
 
         self.buffers["rewards"] = torch.zeros(numsteps + 1, num_envs, 1)
         self.buffers["value_preds"] = torch.zeros(numsteps + 1, num_envs, 1)
         self.buffers["returns"] = torch.zeros(numsteps + 1, num_envs, 1)
 
         self.buffers["action_log_probs"] = torch.zeros(
@@ -105,14 +105,15 @@
         )
         return self.current_rollout_step_idxs[0]
 
     def to(self, device):
         self.buffers.map_in_place(lambda v: v.to(device))
         self.device = device
 
+    @g_timer.avg_time("rollout_storage.insert", level=1)
     def insert(
         self,
         next_observations=None,
         next_recurrent_hidden_states=None,
         actions=None,
         action_log_probs=None,
         value_preds=None,
@@ -166,14 +167,15 @@
     def after_update(self):
         self.buffers[0] = self.buffers[self.current_rollout_step_idx]
 
         self.current_rollout_step_idxs = [
             0 for _ in self.current_rollout_step_idxs
         ]
 
+    @g_timer.avg_time("rollout_storage.compute_returns", level=1)
     def compute_returns(self, next_value, use_gae, gamma, tau):
         if use_gae:
             assert isinstance(self.buffers["value_preds"], torch.Tensor)
             self.buffers["value_preds"][
                 self.current_rollout_step_idx
             ] = next_value
             gae = 0.0
@@ -198,15 +200,15 @@
                 self.buffers["returns"][step] = (
                     gamma
                     * self.buffers["returns"][step + 1]
                     * self.buffers["masks"][step + 1]
                     + self.buffers["rewards"][step]
                 )
 
-    def recurrent_generator(
+    def data_generator(
         self,
         advantages: Optional[torch.Tensor],
         num_mini_batch: int,
     ) -> Iterator[DictTree]:
         assert isinstance(self.buffers["returns"], torch.Tensor)
         num_environments = self.buffers["returns"].size(1)
         assert num_environments >= num_mini_batch, (
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/storage.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/storage.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/tensor_dict.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/tensor_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
+    Protocol,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import numpy as np
 import torch
-from typing_extensions import Protocol
 
 TensorLike = Union[torch.Tensor, np.ndarray, numbers.Real]
 DictTree = Dict[str, Union[TensorLike, "DictTree"]]  # type: ignore
 TensorIndexType = Union[
     int,
     slice,
     torch.Tensor,
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/tensorboard_utils.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/tensorboard_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/common/windowed_running_mean.py` & `habitat-baselines-0.2.520230729/habitat_baselines/common/windowed_running_mean.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/config/default.py` & `habitat-baselines-0.2.520230729/habitat_baselines/config/default.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/config/default_structured_configs.py` & `habitat-baselines-0.2.520230729/habitat_baselines/config/default_structured_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,14 +260,16 @@
     # PDDL action name.
     pddl_action_names: Optional[List[str]] = None
 
 
 @dataclass
 class HierarchicalPolicyConfig(HabitatBaselinesBaseConfig):
     high_level_policy: Dict[str, Any] = MISSING
+    # Names of the skills to not load.
+    ignore_skills: List[str] = field(default_factory=list)
     defined_skills: Dict[str, HrlDefinedSkillConfig] = field(
         default_factory=dict
     )
     use_skills: Dict[str, str] = field(default_factory=dict)
 
 
 @dataclass
@@ -380,14 +382,34 @@
 @dataclass
 class ProfilingConfig(HabitatBaselinesBaseConfig):
     capture_start_step: int = -1
     num_steps_to_capture: int = -1
 
 
 @dataclass
+class VectorEnvFactoryConfig(HabitatBaselinesBaseConfig):
+    """
+    `_target_` points to the `VectorEnvFactory` to setup the vectorized
+    environment. Defaults to the Habitat vectorized environment setup.
+    """
+
+    _target_: str = "habitat_baselines.common.HabitatVectorEnvFactory"
+
+
+@dataclass
+class HydraCallbackConfig(HabitatBaselinesBaseConfig):
+    """
+    Generic callback option for Hydra. Used to create the `_target_` class or
+    call the `_target_` method.
+    """
+
+    _target_: Optional[str] = None
+
+
+@dataclass
 class HabitatBaselinesConfig(HabitatBaselinesBaseConfig):
     # task config can be a list of configs like "A.yaml,B.yaml"
     # If habitat_baselines.evaluate is true, the run will be in evaluation mode
     # replaces --run-type eval when true
     evaluate: bool = False
     trainer_name: str = "ppo"
     updater_name: str = "PPO"
@@ -409,14 +431,16 @@
     # Number of model updates between checkpoints
     checkpoint_interval: int = -1
     total_num_steps: float = -1.0
     log_interval: int = 10
     log_file: str = "train.log"
     force_blind_policy: bool = False
     verbose: bool = True
+    # Creates the vectorized environment.
+    vector_env_factory: VectorEnvFactoryConfig = VectorEnvFactoryConfig()
     eval_keys_to_include_in_name: List[str] = field(default_factory=list)
     # For our use case, the CPU side things are mainly memory copies
     # and nothing of substantive compute. PyTorch has been making
     # more and more memory copies parallel, but that just ends up
     # slowing those down dramatically and reducing our perf.
     # This forces it to be single threaded.  The default
     # value is left as false as it's different from how
@@ -426,14 +450,21 @@
     # Weights and Biases config
     wb: WBConfig = WBConfig()
     # When resuming training or evaluating, will use the original
     # training config if load_resume_state_config is True
     load_resume_state_config: bool = True
     eval: EvalConfig = EvalConfig()
     profiling: ProfilingConfig = ProfilingConfig()
+    # Whether to log the infos that are only logged to a single process to the
+    # CLI along with the other metrics.
+    should_log_single_proc_infos: bool = False
+    # Called every time a checkpoint is saved.
+    # Function signature: fn(save_file_path: str) -> None
+    # If not specified, there is no callback.
+    on_save_ckpt_callback: Optional[HydraCallbackConfig] = None
 
 
 @dataclass
 class HabitatBaselinesRLConfig(HabitatBaselinesConfig):
     rl: RLConfig = RLConfig()
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/data/data.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/data/data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/data/eqa_cnn_pretrain_data.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/data/eqa_cnn_pretrain_data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/data/nav_data.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/data/nav_data.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/metrics.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/metrics.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/models/models.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/models/models.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/eqa_cnn_pretrain_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/pacman_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/pacman_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/il/trainers/vqa_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/il/trainers/vqa_trainer.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/algo/ddppo.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/algo/ddppo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Meta Platforms, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Tuple
+from typing import Optional, Union
 
 import numpy as np
 import torch
 from torch import distributed as distrib
 
 from habitat_baselines.common.baseline_registry import baseline_registry
 from habitat_baselines.rl.ppo import PPO
@@ -19,30 +19,50 @@
         return type(inp)((k, _recursive_apply(v, fn)) for k, v in inp.items())
     elif isinstance(inp, (tuple, list)):
         return type(inp)(_recursive_apply(v, fn) for v in inp)
     else:
         return fn(inp)
 
 
+def _convert_to_numpy_safe(t: Optional[torch.Tensor]) -> torch.Tensor:
+    """
+    Moves any tensors on the CPU to numpy arrays. Leaves other values unaffected.
+    """
+
+    if t is not None and t.device.type == "cpu":
+        return t.numpy()
+    return t
+
+
 def _cpu_to_numpy(inp):
-    return _recursive_apply(
-        inp, lambda t: t.numpy() if t.device.type == "cpu" else t
-    )
+    return _recursive_apply(inp, _convert_to_numpy_safe)
+
+
+def _numpy_to_cpu_safe(
+    t: Optional[Union[np.ndarray, torch.Tensor]]
+) -> Optional[torch.Tensor]:
+    """
+    Moves numpy arrays to torch CPU tensors.
+    """
+
+    if t is not None and isinstance(t, np.ndarray):
+        return torch.from_numpy(t)
+    return t
 
 
 def _numpy_to_cpu(inp):
     return _recursive_apply(
         inp,
-        lambda t: torch.from_numpy(t) if isinstance(t, np.ndarray) else t,
+        _numpy_to_cpu_safe,
     )
 
 
 def distributed_var_mean(
     values: torch.Tensor,
-) -> Tuple[torch.Tensor, torch.Tensor]:
+) -> Union[torch.Tensor, torch.Tensor]:
     r"""Computes the mean and variances of a tensor over multiple workers.
 
     This method is equivalent to first collecting all versions of values and
     then computing the mean and variance locally over that
 
     :param values: (*,) shaped tensors to compute mean and variance over.  Assumed
                         to be solely the workers local copy of this tensor,
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/ddp_utils.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/resnet.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/resnet_policy.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/resnet_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 from gym import spaces
 from torch import nn as nn
 from torch.nn import functional as F
+from torchvision import transforms as T
+from torchvision.transforms import functional as TF
 
 from habitat.tasks.nav.instance_image_nav_task import InstanceImageGoalSensor
 from habitat.tasks.nav.nav import (
     EpisodicCompassSensor,
     EpisodicGPSSensor,
     HeadingSensor,
     ImageGoalSensor,
@@ -35,14 +37,19 @@
 )
 from habitat_baselines.rl.ppo import Net, NetPolicy
 from habitat_baselines.utils.common import get_num_actions
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
+try:
+    import clip
+except ImportError:
+    clip = None
+
 
 @baseline_registry.register_policy
 class PointNavResNetPolicy(NetPolicy):
     def __init__(
         self,
         observation_space: spaces.Dict,
         action_space,
@@ -54,14 +61,31 @@
         normalize_visual_inputs: bool = False,
         force_blind_policy: bool = False,
         policy_config: "DictConfig" = None,
         aux_loss_config: Optional["DictConfig"] = None,
         fuse_keys: Optional[List[str]] = None,
         **kwargs,
     ):
+        """
+        Keyword arguments:
+        rnn_type: RNN layer type; one of ["GRU", "LSTM"]
+        backbone: Visual encoder backbone; one of ["resnet18", "resnet50", "resneXt50", "se_resnet50", "se_resneXt50", "se_resneXt101", "resnet50_clip_avgpool", "resnet50_clip_attnpool"]
+        """
+
+        assert backbone in [
+            "resnet18",
+            "resnet50",
+            "resneXt50",
+            "se_resnet50",
+            "se_resneXt50",
+            "se_resneXt101",
+            "resnet50_clip_avgpool",
+            "resnet50_clip_attnpool",
+        ], f"{backbone} backbone is not recognized."
+
         if policy_config is not None:
             discrete_actions = (
                 policy_config.action_distribution_type == "categorical"
             )
             self.action_distribution_type = (
                 policy_config.action_distribution_type
             )
@@ -235,14 +259,129 @@
 
         x = self.running_mean_and_var(x)
         x = self.backbone(x)
         x = self.compression(x)
         return x
 
 
+class ResNetCLIPEncoder(nn.Module):
+    def __init__(
+        self,
+        observation_space: spaces.Dict,
+        pooling="attnpool",
+    ):
+        super().__init__()
+
+        self.rgb = "rgb" in observation_space.spaces
+        self.depth = "depth" in observation_space.spaces
+
+        # Determine which visual observations are present
+        self.visual_keys = [
+            k
+            for k, v in observation_space.spaces.items()
+            if len(v.shape) > 1 and k != ImageGoalSensor.cls_uuid
+        ]
+
+        # Count total # of channels
+        self._n_input_channels = sum(
+            observation_space.spaces[k].shape[2] for k in self.visual_keys
+        )
+
+        if not self.is_blind:
+            if clip is None:
+                raise ImportError(
+                    "Need to install CLIP (run `pip install git+https://github.com/openai/CLIP.git@40f5484c1c74edd83cb9cf687c6ab92b28d8b656`)"
+                )
+
+            model, preprocess = clip.load("RN50")
+
+            # expected input: C x H x W (np.uint8 in [0-255])
+            self.preprocess = T.Compose(
+                [
+                    # resize and center crop to 224
+                    preprocess.transforms[0],
+                    preprocess.transforms[1],
+                    # already tensor, but want float
+                    T.ConvertImageDtype(torch.float),
+                    # normalize with CLIP mean, std
+                    preprocess.transforms[4],
+                ]
+            )
+            # expected output: C x H x W (np.float32)
+
+            self.backbone = model.visual
+
+            if self.rgb and self.depth:
+                self.backbone.attnpool = nn.Identity()
+                self.output_shape = (2048,)  # type: Tuple
+            elif pooling == "none":
+                self.backbone.attnpool = nn.Identity()
+                self.output_shape = (2048, 7, 7)
+            elif pooling == "avgpool":
+                self.backbone.attnpool = nn.Sequential(
+                    nn.AdaptiveAvgPool2d(output_size=(1, 1)), nn.Flatten()
+                )
+                self.output_shape = (2048,)
+            else:
+                self.output_shape = (1024,)
+
+            for param in self.backbone.parameters():
+                param.requires_grad = False
+            for module in self.backbone.modules():
+                if "BatchNorm" in type(module).__name__:
+                    module.momentum = 0.0
+            self.backbone.eval()
+
+    @property
+    def is_blind(self):
+        return self._n_input_channels == 0
+
+    def forward(self, observations: Dict[str, torch.Tensor]) -> torch.Tensor:  # type: ignore
+        if self.is_blind:
+            return None
+
+        cnn_input = []
+        if self.rgb:
+            rgb_observations = observations["rgb"]
+            rgb_observations = rgb_observations.permute(
+                0, 3, 1, 2
+            )  # BATCH x CHANNEL x HEIGHT X WIDTH
+            rgb_observations = torch.stack(
+                [self.preprocess(rgb_image) for rgb_image in rgb_observations]
+            )  # [BATCH x CHANNEL x HEIGHT X WIDTH] in torch.float32
+            rgb_x = self.backbone(rgb_observations).float()
+            cnn_input.append(rgb_x)
+
+        if self.depth:
+            depth_observations = observations["depth"][
+                ..., 0
+            ]  # [BATCH x HEIGHT X WIDTH]
+            ddd = torch.stack(
+                [depth_observations] * 3, dim=1
+            )  # [BATCH x 3 x HEIGHT X WIDTH]
+            ddd = torch.stack(
+                [
+                    self.preprocess(
+                        TF.convert_image_dtype(depth_map, torch.uint8)
+                    )
+                    for depth_map in ddd
+                ]
+            )  # [BATCH x CHANNEL x HEIGHT X WIDTH] in torch.float32
+            depth_x = self.backbone(ddd).float()
+            cnn_input.append(depth_x)
+
+        if self.rgb and self.depth:
+            x = F.adaptive_avg_pool2d(cnn_input[0] + cnn_input[1], 1)
+            x = x.flatten(1)
+        else:
+            x = torch.cat(cnn_input, dim=1)
+
+        return x
+
+
 class PointNavResNetNet(Net):
     """Network which passes the input image through CNN and concatenates
     goal vector with CNN's output and passes that through RNN.
     """
 
     PRETRAINED_VISUAL_FEATURES_KEY = "visual_features"
     prev_action_embedding: nn.Module
@@ -405,30 +544,45 @@
                 {
                     k: observation_space.spaces[k]
                     for k in fuse_keys
                     if len(observation_space.spaces[k].shape) == 3
                 }
             )
 
-        self.visual_encoder = ResNetEncoder(
-            use_obs_space,
-            baseplanes=resnet_baseplanes,
-            ngroups=resnet_baseplanes // 2,
-            make_backbone=getattr(resnet, backbone),
-            normalize_visual_inputs=normalize_visual_inputs,
-        )
-
-        if not self.visual_encoder.is_blind:
-            self.visual_fc = nn.Sequential(
-                nn.Flatten(),
-                nn.Linear(
-                    np.prod(self.visual_encoder.output_shape), hidden_size
-                ),
-                nn.ReLU(True),
+        if backbone.startswith("resnet50_clip"):
+            self.visual_encoder = ResNetCLIPEncoder(
+                observation_space
+                if not force_blind_policy
+                else spaces.Dict({}),
+                pooling="avgpool" if "avgpool" in backbone else "attnpool",
             )
+            if not self.visual_encoder.is_blind:
+                self.visual_fc = nn.Sequential(
+                    nn.Linear(
+                        self.visual_encoder.output_shape[0], hidden_size
+                    ),
+                    nn.ReLU(True),
+                )
+        else:
+            self.visual_encoder = ResNetEncoder(
+                use_obs_space,
+                baseplanes=resnet_baseplanes,
+                ngroups=resnet_baseplanes // 2,
+                make_backbone=getattr(resnet, backbone),
+                normalize_visual_inputs=normalize_visual_inputs,
+            )
+
+            if not self.visual_encoder.is_blind:
+                self.visual_fc = nn.Sequential(
+                    nn.Flatten(),
+                    nn.Linear(
+                        np.prod(self.visual_encoder.output_shape), hidden_size
+                    ),
+                    nn.ReLU(True),
+                )
 
         self.state_encoder = build_rnn_state_encoder(
             (0 if self.is_blind else self._hidden_size) + rnn_input_size,
             self._hidden_size,
             rnn_type=rnn_type,
             num_layers=num_recurrent_layers,
         )
@@ -444,14 +598,18 @@
         return self.visual_encoder.is_blind
 
     @property
     def num_recurrent_layers(self):
         return self.state_encoder.num_recurrent_layers
 
     @property
+    def recurrent_hidden_size(self):
+        return self._hidden_size
+
+    @property
     def perception_embedding_size(self):
         return self._hidden_size
 
     def forward(
         self,
         observations: Dict[str, torch.Tensor],
         rnn_hidden_states,
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ddppo/policy/running_mean_and_var.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/fixed_policy.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/fixed_policy.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,36 +5,45 @@
 from typing import List, Tuple
 
 import torch
 
 from habitat.tasks.rearrange.multi_task.rearrange_pddl import parse_func
 from habitat_baselines.common.logging import baselines_logger
 from habitat_baselines.rl.hrl.hl.high_level_policy import HighLevelPolicy
+from habitat_baselines.rl.ppo.policy import PolicyActionData
 
 
 class FixedHighLevelPolicy(HighLevelPolicy):
     """
     Executes a fixed sequence of high-level actions as specified by the
     `solution` field of the PDDL problem file.
-    :property _solution_actions: List of tuples were first tuple element is the
-        action name and the second is the action arguments.
+    :property _solution_actions: List of tuples where the first tuple element
+        is the action name and the second is the action arguments. Stores a plan
+        for each environment.
     """
 
-    _solution_actions: List[Tuple[str, List[str]]]
+    _solution_actions: List[List[Tuple[str, List[str]]]]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self._solution_actions = self._parse_solution_actions(
-            self._pddl_prob.solution
-        )
+        self._solution_actions = [
+            self._parse_solution_actions() for _ in range(self._num_envs)
+        ]
 
         self._next_sol_idxs = torch.zeros(self._num_envs, dtype=torch.int32)
 
-    def _parse_solution_actions(self, solution):
+    def _parse_solution_actions(self) -> List[Tuple[str, List[str]]]:
+        """
+        Returns the sequence of actions to execute as a list of:
+        - The action name.
+        - A list of the action arguments.
+        """
+        solution = self._pddl_prob.solution
+
         solution_actions = []
         for i, hl_action in enumerate(solution):
             sol_action = (
                 hl_action.name,
                 [x.name for x in hl_action.param_values],
             )
             solution_actions.append(sol_action)
@@ -63,20 +72,22 @@
 
         Args:
             batch_idx: The index of the current environment.
 
         Returns:
             The next index to be used from the list of solution actions.
         """
-        if self._next_sol_idxs[batch_idx] >= len(self._solution_actions):
+        if self._next_sol_idxs[batch_idx] >= len(
+            self._solution_actions[batch_idx]
+        ):
             baselines_logger.info(
                 f"Calling for immediate end with {self._next_sol_idxs[batch_idx]}"
             )
             immediate_end[batch_idx] = True
-            return len(self._solution_actions) - 1
+            return len(self._solution_actions[batch_idx]) - 1
         else:
             return self._next_sol_idxs[batch_idx].item()
 
     def get_next_skill(
         self,
         observations,
         rnn_hidden_states,
@@ -89,22 +100,24 @@
         next_skill = torch.zeros(self._num_envs)
         skill_args_data = [None for _ in range(self._num_envs)]
         immediate_end = torch.zeros(self._num_envs, dtype=torch.bool)
         for batch_idx, should_plan in enumerate(plan_masks):
             if should_plan == 1.0:
                 use_idx = self._get_next_sol_idx(batch_idx, immediate_end)
 
-                skill_name, skill_args = self._solution_actions[use_idx]
+                skill_name, skill_args = self._solution_actions[batch_idx][
+                    use_idx
+                ]
                 baselines_logger.info(
                     f"Got next element of the plan with {skill_name}, {skill_args}"
                 )
                 if skill_name not in self._skill_name_to_idx:
                     raise ValueError(
                         f"Could not find skill named {skill_name} in {self._skill_name_to_idx}"
                     )
                 next_skill[batch_idx] = self._skill_name_to_idx[skill_name]
 
                 skill_args_data[batch_idx] = skill_args  # type: ignore[call-overload]
 
                 self._next_sol_idxs[batch_idx] += 1
 
-        return next_skill, skill_args_data, immediate_end, {}
+        return next_skill, skill_args_data, immediate_end, PolicyActionData()
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/high_level_policy.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/high_level_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, List, Tuple
 
 import gym.spaces as spaces
 import torch
 import torch.nn as nn
 
 from habitat.tasks.rearrange.multi_task.pddl_domain import PddlProblem
+from habitat_baselines.rl.ppo.policy import PolicyActionData
 
 
 class HighLevelPolicy(nn.Module):
     """
     High level policy that selects from low-level skills.
     """
 
@@ -32,14 +33,21 @@
     def to(self, device):
         self._device = device
         return super().to(device)
 
     def get_value(self, observations, rnn_hidden_states, prev_actions, masks):
         raise NotImplementedError()
 
+    @property
+    def should_load_agent_state(self) -> bool:
+        """
+        If we need to load the state dict of the high-level policy.
+        """
+        return False
+
     def evaluate_actions(
         self,
         observations,
         rnn_hidden_states,
         prev_actions,
         masks,
         action,
@@ -64,15 +72,15 @@
         observations,
         rnn_hidden_states: torch.Tensor,
         prev_actions: torch.Tensor,
         masks: torch.Tensor,
         plan_masks: torch.Tensor,
         deterministic: bool,
         log_info: List[Dict[str, Any]],
-    ) -> Tuple[torch.Tensor, List[Any], torch.BoolTensor, Dict[str, Any]]:
+    ) -> Tuple[torch.Tensor, List[Any], torch.BoolTensor, PolicyActionData]:
         """
         Get the next skill to be executed.
 
         Args:
             observations: Current observations.
             rnn_hidden_states: Current hidden states of the RNN.
             prev_actions: Previous actions taken.
@@ -82,21 +90,18 @@
 
         Returns:
             A tuple containing:
             - next_skill: Next skill to be executed.
             - skill_args_data: Arguments for the next skill.
             - immediate_end: Binary masks indicating which environment(s) should
                 end immediately.
-            - Information for PolicyActionData
+            - PolicyActionData information for learning.
         """
         raise NotImplementedError()
 
-    def create_hl_info(self) -> Dict[str, Any]:
-        return {}
-
     def apply_mask(self, mask: torch.Tensor) -> None:
         """
         Called before every step with the mask information at the current step.
         """
 
     def get_policy_components(self) -> List[nn.Module]:
         """
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hl/neural_policy.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hl/neural_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from habitat_baselines.common.logging import baselines_logger
 from habitat_baselines.rl.ddppo.policy import resnet
 from habitat_baselines.rl.ddppo.policy.resnet_policy import ResNetEncoder
 from habitat_baselines.rl.hrl.hl.high_level_policy import HighLevelPolicy
 from habitat_baselines.rl.models.rnn_state_encoder import (
     build_rnn_state_encoder,
 )
-from habitat_baselines.rl.ppo.policy import CriticHead
+from habitat_baselines.rl.ppo.policy import CriticHead, PolicyActionData
 from habitat_baselines.utils.common import CategoricalNet
 
 
 class NeuralHighLevelPolicy(HighLevelPolicy):
     """
     A trained high-level policy that selects low-level skills and their skill
     inputs. Is limited to discrete skills and discrete skill inputs. The policy
@@ -77,16 +77,17 @@
             self._hidden_size,
             rnn_type=self._config.rnn_type,
             num_layers=self._config.num_rnn_layers,
         )
         self._policy = CategoricalNet(self._hidden_size, self._n_actions)
         self._critic = CriticHead(self._hidden_size)
 
-    def create_hl_info(self):
-        return {"actions": None}
+    @property
+    def should_load_agent_state(self):
+        return True
 
     def _setup_actions(self) -> List[PddlAction]:
         all_actions = self._pddl_prob.get_possible_actions()
         all_actions = [
             ac for ac in all_actions if ac.name in self._config.allowed_actions
         ]
         if not self._config.allow_other_place:
@@ -150,15 +151,15 @@
         observations,
         rnn_hidden_states,
         prev_actions,
         masks,
         action,
         rnn_build_seq_info,
     ):
-        features, _ = self.forward(
+        features, rnn_hidden_states = self.forward(
             observations, rnn_hidden_states, masks, rnn_build_seq_info
         )
         distribution = self._policy(features)
         value = self._critic(features)
         action_log_probs = distribution.log_probs(action)
         distribution_entropy = distribution.entropy()
 
@@ -207,14 +208,14 @@
             ]
             log_info[batch_idx]["nn_action"] = use_ac.compact_str
 
         return (
             next_skill,
             skill_args_data,
             immediate_end,
-            {
-                "action_log_probs": action_log_probs,
-                "values": values,
-                "actions": skill_sel,
-                "rnn_hidden_states": rnn_hidden_states,
-            },
+            PolicyActionData(
+                action_log_probs=action_log_probs,
+                values=values,
+                actions=skill_sel,
+                rnn_hidden_states=rnn_hidden_states,
+            ),
         )
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hrl_ppo.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_ppo.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/hrl_rollout_storage.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/hrl_rollout_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         current_step = TensorDict(
             {k: v for k, v in current_step.items() if v is not None}
         )
 
         if should_inserts is None:
             should_inserts = self._last_should_inserts
         assert should_inserts is not None
+        # Starts as shape [batch_size, 1]
+        should_inserts = should_inserts.flatten()
 
         if should_inserts.sum() == 0:
             return
 
         env_idxs = torch.arange(self._num_envs)
         if rewards is not None:
             # Accumulate rewards between updates.
@@ -162,17 +164,15 @@
                 - self.buffers["value_preds"][step]
             )
             gae = delta + gamma * tau * gae * self.buffers["masks"][step + 1]
             self.buffers["returns"][step] = (  # type: ignore
                 gae + self.buffers["value_preds"][step]  # type: ignore
             )
 
-    def recurrent_generator(
-        self, advantages, num_batches
-    ) -> Iterator[DictTree]:
+    def data_generator(self, advantages, num_batches) -> Iterator[DictTree]:
         """
         Generates data batches based on the data that has been written to the
         rollout buffer.
         """
 
         num_environments = advantages.size(1)
         dones_cpu = (
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/__init__.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/art_obj.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/art_obj.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/nav.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nav.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,23 @@
             action_space,
             filtered_obs_space,
             filtered_action_space,
             batch_size,
             should_keep_hold_state=True,
         )
 
+    @property
+    def required_obs_keys(self):
+        # Potentially additional sensors are required to determine termination
+        return super().required_obs_keys + [
+            TargetGoalGpsCompassSensor.cls_uuid,
+            NavGoalPointGoalSensor.cls_uuid,
+            TargetStartGpsCompassSensor.cls_uuid,
+        ]
+
     def _get_filtered_obs(self, observations, cur_batch_idx) -> TensorDict:
         ret_obs = super()._get_filtered_obs(observations, cur_batch_idx)
 
         if NavGoalPointGoalSensor.cls_uuid in ret_obs:
             for i, batch_i in enumerate(cur_batch_idx):
                 if self._cur_skill_args[batch_i].is_target:
                     replace_sensor = TargetGoalGpsCompassSensor.cls_uuid
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/nn_skill.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/nn_skill.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,20 @@
             else:
                 break
 
         self._internal_log(
             f"Skill {self._config.skill_name}: action offset {self._ac_start}, action length {self._ac_len}"
         )
 
+    @property
+    def required_obs_keys(self):
+        return super().required_obs_keys + list(
+            self._filtered_obs_space.spaces.keys()
+        )
+
     def parameters(self):
         if self._wrap_policy is not None:
             return self._wrap_policy.parameters()
         else:
             return []
 
     @property
@@ -94,22 +100,23 @@
         self,
         skill_arg,
         batch_idxs,
         observations,
         rnn_hidden_states,
         prev_actions,
     ):
-        super().on_enter(
+        ret = super().on_enter(
             skill_arg,
             batch_idxs,
             observations,
             rnn_hidden_states,
             prev_actions,
         )
         self._did_want_done *= 0.0
+        return ret
 
     def _get_filtered_obs(self, observations, cur_batch_idx) -> TensorDict:
         return TensorDict(
             {
                 k: observations[k]
                 for k in self._filtered_obs_space.spaces.keys()
             }
@@ -165,15 +172,15 @@
         else:
             try:
                 ckpt_dict = torch.load(
                     config.load_ckpt_file, map_location="cpu"
                 )
             except FileNotFoundError as e:
                 raise FileNotFoundError(
-                    "Could not load neural network weights for skill."
+                    f"Could not load neural network weights for skill from ckpt {config.load_ckpt_file}"
                 ) from e
 
             policy_cfg = ckpt_dict["config"]
 
         policy = baseline_registry.get_policy(config.name)
 
         expected_obs_keys = policy_cfg.habitat.gym.obs_keys
@@ -214,20 +221,15 @@
         )
 
         actor_critic = policy.from_config(
             policy_cfg, filtered_obs_space, filtered_action_space
         )
         if len(ckpt_dict) > 0:
             try:
-                actor_critic.load_state_dict(
-                    {  # type: ignore
-                        k[len("actor_critic.") :]: v
-                        for k, v in ckpt_dict["state_dict"].items()
-                    }
-                )
+                actor_critic.load_state_dict(ckpt_dict["state_dict"])
 
             except Exception as e:
                 raise ValueError(
                     f"Could not load checkpoint for skill {config.skill_name} from {config.load_ckpt_file}"
                 ) from e
 
         return cls(
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/noop.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/noop.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/oracle_nav.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/oracle_nav.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/pick.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/pick.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/place.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/place.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return [self._cur_skill_args[i].targ for i in batch_idx]
 
     def _mask_pick(self, action, observations):
         # Mask out the grasp if the object is already released.
         is_not_holding = 1 - observations[IsHoldingSensor.cls_uuid].view(-1)
         for i in torch.nonzero(is_not_holding):
             # Do not regrasp the object once it is released.
-            action[i, self._grip_ac_idx] = -1.0
+            action.actions[i, self._grip_ac_idx] = -1.0
         return action
 
     def _is_skill_done(
         self, observations, rnn_hidden_states, prev_actions, masks, batch_idx
     ) -> torch.BoolTensor:
         # Is the agent not holding an object and is the end-effector at the
         # resting position?
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/reset.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/reset.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         )
 
         return ret
 
     def _parse_skill_arg(self, skill_arg: str):
         return None
 
+    @property
+    def required_obs_keys(self) -> List[str]:
+        return super().required_obs_keys + ["joint"]
+
     def _is_skill_done(
         self, observations, rnn_hidden_states, prev_actions, masks, batch_idx
     ):
         current_joint_pos = observations["joint"].cpu().numpy()
 
         return (
             torch.as_tensor(
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/skill.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/skill.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,30 +52,27 @@
                 action_space, "pddl_apply_action"
             )
         else:
             self._pddl_ac_start = None
         if self._apply_postconds and self._pddl_ac_start is None:
             raise ValueError(f"Could not find PDDL action in skill {self}")
 
-        self._delay_term: List[Optional[bool]] = [
-            None for _ in range(self._batch_size)
-        ]
-
         self._grip_ac_idx = 0
         found_grip = False
         for k, space in action_space.items():
             if k != "arm_action":
                 self._grip_ac_idx += get_num_actions(space)
             else:
                 # The last actioin in the arm action is the grip action.
                 self._grip_ac_idx += get_num_actions(space) - 1
                 found_grip = True
                 break
         if not found_grip and not self.should_ignore_grip:
             raise ValueError(f"Could not find grip action in {action_space}")
+
         self._stop_action_idx, _ = find_action_range(
             action_space, "rearrange_stop"
         )
 
     def _internal_log(self, s):
         baselines_logger.debug(
             f"Skill {self._config.skill_name} @ step {self._cur_skill_step}: {s}"
@@ -181,18 +178,14 @@
               indicates the skill to return control to HL policy.
             - `bad_terminate`: Shape (batch_size,) size tensor where 1
               indicates the skill should immediately end the episode.
         """
         is_skill_done = self._is_skill_done(
             observations, rnn_hidden_states, prev_actions, masks, batch_idx
         ).cpu()
-        if is_skill_done.sum() > 0:
-            self._internal_log(
-                f"Requested skill termination {is_skill_done}",
-            )
 
         cur_skill_step = self._cur_skill_step[batch_idx]
 
         bad_terminate = torch.zeros(
             cur_skill_step.shape,
             device=cur_skill_step.device,
             dtype=torch.bool,
@@ -204,34 +197,19 @@
             else:
                 is_skill_done = is_skill_done | over_max_len
 
         is_skill_done |= hl_wants_skill_term
 
         new_actions = torch.zeros_like(actions)
         for i, env_i in enumerate(batch_idx):
-            if self._delay_term[env_i]:
-                self._internal_log(
-                    "Terminating skill due to delayed termination."
-                )
-                self._delay_term[env_i] = False
-                is_skill_done[i] = True
-            elif self._apply_postconds and is_skill_done[i]:
+            if self._apply_postconds and is_skill_done[i]:
                 new_actions[i] = self._apply_postcond(
                     actions, log_info, skill_name[i], env_i, i
                 )
-                self._delay_term[env_i] = True
-                is_skill_done[i] = False
-                self._internal_log(
-                    "Applying PDDL action and terminating on the next step."
-                )
 
-        if bad_terminate.sum() > 0:
-            self._internal_log(
-                f"Bad terminating due to timeout {cur_skill_step}, {bad_terminate}",
-            )
         return is_skill_done, bad_terminate, new_actions
 
     def on_enter(
         self,
         skill_arg: List[str],
         batch_idxs: List[int],
         observations,
@@ -252,15 +230,15 @@
                 )
             self._cur_skill_args[batch_idx] = self._parse_skill_arg(
                 skill_arg[i]
             )
 
         return (
             rnn_hidden_states[batch_idxs] * 0.0,
-            prev_actions[batch_idxs] * 0.0,
+            prev_actions[batch_idxs] * 0,
         )
 
     def set_pddl_problem(self, pddl_prob):
         self._pddl_problem = pddl_prob
         self._entities_list = self._pddl_problem.get_ordered_entities_list()
         self._action_ordering = self._pddl_problem.get_ordered_actions()
 
@@ -344,7 +322,18 @@
         rnn_hidden_states,
         prev_actions,
         masks,
         cur_batch_idx,
         deterministic=False,
     ) -> PolicyActionData:
         raise NotImplementedError()
+
+    @property
+    def required_obs_keys(self) -> List[str]:
+        """
+        Which keys from the observation dictionary this skill requires to
+        compute actions and termination conditions.
+        """
+        if self._should_keep_hold_state:
+            return [IsHoldingSensor.cls_uuid]
+        else:
+            return []
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/skills/wait.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/skills/wait.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/hrl/utils.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/hrl/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     end_idx = get_num_actions(action_space[search_key])
     for k in action_space:
         if k == search_key:
             found = True
             break
         start_idx += get_num_actions(action_space[k])
     if not found:
-        raise ValueError(f"Could not find stop action in {action_space}")
-    return start_idx, end_idx
+        raise ValueError(f"Could not find {search_key} in {action_space}")
+    return start_idx, start_idx + end_idx
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/models/action_embedding.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/action_embedding.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/models/rnn_state_encoder.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/rnn_state_encoder.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/models/simple_cnn.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/models/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/__init__.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/agent_access_mgr.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/agent_access_mgr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 import gym.spaces as spaces
 
 from habitat_baselines.common.env_spec import EnvironmentSpec
 from habitat_baselines.common.storage import Storage
 from habitat_baselines.rl.ppo.policy import Policy
 from habitat_baselines.rl.ppo.updater import Updater
@@ -111,29 +111,33 @@
         """
         raise NotImplementedError()
 
     @abstractmethod
     def load_state_dict(self, state: Dict) -> None:
         raise NotImplementedError()
 
-    @property
-    @abstractmethod
-    def hidden_state_shape(self) -> Tuple[int]:
-        """
-        The shape of the tensor to track the hidden state, such as the RNN hidden state.
-        """
-        raise NotImplementedError()
-
     @abstractmethod
     def after_update(self) -> None:
         """
         Must be called by the trainer after the updater has called `update` and
         the rollout `after_update` is called.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def pre_rollout(self) -> None:
         """
         Called before a rollout is collected.
         """
         raise NotImplementedError()
+
+    @abstractmethod
+    def _create_storage(
+        self,
+        num_envs: int,
+        env_spec: EnvironmentSpec,
+        actor_critic: Policy,
+        policy_action_space: spaces.Space,
+        config: "DictConfig",
+        device,
+    ) -> Storage:
+        pass
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/cpc_aux_loss.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/cpc_aux_loss.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/policy.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     GaussianNet,
     get_num_actions,
 )
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
+from habitat_baselines.utils.timing import g_timer
+
 
 @dataclass
 class PolicyActionData:
     """
     Information returned from the `Policy.act` method representing the
     information from an agent's action.
 
@@ -51,15 +53,15 @@
         `take_actions` is None, then this is also the action executed in the
         environment.
     :property rnn_hidden_states: Actor hidden states.
     :property action_log_probs: The log probabilities of the actions under the
         current policy.
     """
 
-    rnn_hidden_states: torch.Tensor
+    rnn_hidden_states: Optional[torch.Tensor] = None
     actions: Optional[torch.Tensor] = None
     values: Optional[torch.Tensor] = None
     action_log_probs: Optional[torch.Tensor] = None
     take_actions: Optional[torch.Tensor] = None
     policy_info: Optional[List[Dict[str, Any]]] = None
     should_inserts: Optional[torch.BoolTensor] = None
 
@@ -93,17 +95,27 @@
     def should_load_agent_state(self):
         return True
 
     @property
     def num_recurrent_layers(self) -> int:
         return 0
 
+    @property
+    def recurrent_hidden_size(self) -> int:
+        return 0
+
     def forward(self, *x):
         raise NotImplementedError
 
+    @property
+    def visual_encoder(self) -> Optional[nn.Module]:
+        """
+        Gets the visual encoder for the policy.
+        """
+
     def get_policy_action_space(
         self, env_action_space: spaces.Space
     ) -> spaces.Space:
         return env_action_space
 
     def _get_policy_components(self) -> List[nn.Module]:
         return []
@@ -202,14 +214,22 @@
             self.aux_loss_modules[aux_loss_name] = aux_loss(
                 action_space,
                 self.net,
                 **cfg,
             )
 
     @property
+    def recurrent_hidden_size(self) -> int:
+        return self.net.recurrent_hidden_size
+
+    @property
+    def visual_encoder(self) -> Optional[nn.Module]:
+        return self.net.visual_encoder
+
+    @property
     def should_load_agent_state(self):
         return True
 
     @property
     def num_recurrent_layers(self) -> int:
         return self.net.num_recurrent_layers
 
@@ -242,14 +262,15 @@
         return PolicyActionData(
             values=value,
             actions=action,
             action_log_probs=action_log_probs,
             rnn_hidden_states=rnn_hidden_states,
         )
 
+    @g_timer.avg_time("net_policy.get_value", level=1)
     def get_value(self, observations, rnn_hidden_states, prev_actions, masks):
         features, _, _ = self.net(
             observations, rnn_hidden_states, prev_actions, masks
         )
         return self.critic(features)
 
     def evaluate_actions(
@@ -367,14 +388,19 @@
     @property
     @abc.abstractmethod
     def num_recurrent_layers(self):
         pass
 
     @property
     @abc.abstractmethod
+    def recurrent_hidden_size(self):
+        pass
+
+    @property
+    @abc.abstractmethod
     def is_blind(self):
         pass
 
     @property
     @abc.abstractmethod
     def perception_embedding_size(self) -> int:
         pass
@@ -432,14 +458,18 @@
         return self.visual_encoder.is_blind
 
     @property
     def num_recurrent_layers(self):
         return self.state_encoder.num_recurrent_layers
 
     @property
+    def recurrent_hidden_size(self):
+        return self._hidden_size
+
+    @property
     def perception_embedding_size(self):
         return self._hidden_size
 
     def forward(
         self,
         observations,
         rnn_hidden_states,
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/ppo.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,38 +20,40 @@
 from habitat_baselines.rl.ppo.policy import NetPolicy
 from habitat_baselines.rl.ppo.updater import Updater
 from habitat_baselines.rl.ver.ver_rollout_storage import VERRolloutStorage
 from habitat_baselines.utils.common import (
     LagrangeInequalityCoefficient,
     inference_mode,
 )
+from habitat_baselines.utils.timing import g_timer
 
 EPS_PPO = 1e-5
 
 
 @baseline_registry.register_updater
 class PPO(nn.Module, Updater):
     entropy_coef: Union[float, LagrangeInequalityCoefficient]
 
     @classmethod
     def from_config(cls, actor_critic: NetPolicy, config):
-        config = {k.lower(): v for k, v in config.items()}
-        param_dict = dict(actor_critic=actor_critic)
-        sig = inspect.signature(cls.__init__)
-        for p in sig.parameters.values():
-            if p.name == "self" or p.name in param_dict:
-                continue
-
-            assert p.name in config, "{} parameter '{}' not in config".format(
-                cls.__name__, p.name
-            )
-
-            param_dict[p.name] = config[p.name]
-
-        return cls(**param_dict)
+        return cls(
+            actor_critic=actor_critic,
+            clip_param=config.clip_param,
+            ppo_epoch=config.ppo_epoch,
+            num_mini_batch=config.num_mini_batch,
+            value_loss_coef=config.value_loss_coef,
+            entropy_coef=config.entropy_coef,
+            lr=config.lr,
+            eps=config.eps,
+            max_grad_norm=config.max_grad_norm,
+            use_clipped_value_loss=config.use_clipped_value_loss,
+            use_normalized_advantage=config.use_normalized_advantage,
+            entropy_target_factor=config.entropy_target_factor,
+            use_adaptive_entropy_pen=config.use_adaptive_entropy_pen,
+        )
 
     def __init__(
         self,
         actor_critic: NetPolicy,
         clip_param: float,
         ppo_epoch: int,
         num_mini_batch: int,
@@ -94,17 +96,24 @@
                 init_alpha=entropy_coef,
                 alpha_max=1.0,
                 alpha_min=1e-4,
                 greater_than=True,
             ).to(device=self.device)
 
         self.use_normalized_advantage = use_normalized_advantage
+        self.optimizer = self._create_optimizer(lr, eps)
 
-        params = list(filter(lambda p: p.requires_grad, self.parameters()))
+        self.non_ac_params = [
+            p
+            for name, p in self.named_parameters()
+            if not name.startswith("actor_critic.")
+        ]
 
+    def _create_optimizer(self, lr, eps):
+        params = list(filter(lambda p: p.requires_grad, self.parameters()))
         if len(params) > 0:
             optim_cls = optim.Adam
             optim_kwargs = dict(
                 params=params,
                 lr=lr,
                 eps=eps,
             )
@@ -115,23 +124,17 @@
                 try:
                     import torch.optim._multi_tensor
                 except ImportError:
                     pass
                 else:
                     optim_cls = torch.optim._multi_tensor.Adam
 
-            self.optimizer = optim_cls(**optim_kwargs)
+            return optim_cls(**optim_kwargs)
         else:
-            self.optimizer = None
-
-        self.non_ac_params = [
-            p
-            for name, p in self.named_parameters()
-            if not name.startswith("actor_critic.")
-        ]
+            return None
 
     def forward(self, *x):
         raise NotImplementedError
 
     def get_advantages(self, rollouts: RolloutStorage) -> Tensor:
         advantages = (
             rollouts.buffers["returns"]  # type: ignore
@@ -153,14 +156,15 @@
         return torch.var_mean(x)
 
     def _set_grads_to_none(self):
         for pg in self.optimizer.param_groups:
             for p in pg["params"]:
                 p.grad = None
 
+    @g_timer.avg_time("ppo.update_from_batch", level=1)
     def _update_from_batch(self, batch, epoch, rollouts, learner_metrics):
         """
         Performs a gradient update from the minibatch.
         """
 
         def record_min_mean_max(t: torch.Tensor, prefix: str):
             for name, op in (
@@ -180,15 +184,15 @@
             aux_loss_res,
         ) = self._evaluate_actions(
             batch["observations"],
             batch["recurrent_hidden_states"],
             batch["prev_actions"],
             batch["masks"],
             batch["actions"],
-            batch["rnn_build_seq_info"],
+            batch.get("rnn_build_seq_info", None),
         )
 
         ratio = torch.exp(action_log_probs - batch["action_log_probs"])
 
         surr1 = batch["advantages"] * ratio
         surr2 = batch["advantages"] * (
             torch.clamp(
@@ -299,15 +303,15 @@
     ) -> Dict[str, float]:
         advantages = self.get_advantages(rollouts)
 
         learner_metrics: Dict[str, List[Any]] = collections.defaultdict(list)
 
         for epoch in range(self.ppo_epoch):
             profiling_wrapper.range_push("PPO.update epoch")
-            data_generator = rollouts.recurrent_generator(
+            data_generator = rollouts.data_generator(
                 advantages, self.num_mini_batch
             )
 
             for _bid, batch in enumerate(data_generator):
                 self._update_from_batch(
                     batch, epoch, rollouts, learner_metrics
                 )
@@ -322,14 +326,15 @@
                     torch.stack(
                         [torch.as_tensor(v, dtype=torch.float32) for v in vs]
                     ).mean()
                 )
                 for k, vs in learner_metrics.items()
             }
 
+    @g_timer.avg_time("ppo.eval_actions", level=1)
     def _evaluate_actions(self, *args, **kwargs):
         r"""Internal method that calls Policy.evaluate_actions.  This is used instead of calling
         that directly so that that call can be overrided with inheritance
         """
         return self.actor_critic.evaluate_actions(*args, **kwargs)
 
     def before_backward(self, loss: Tensor) -> Tensor:
@@ -363,7 +368,19 @@
         [h.wait() for h in handles]
 
         return grad_norm
 
     def after_step(self) -> None:
         if isinstance(self.entropy_coef, LagrangeInequalityCoefficient):
             self.entropy_coef.project_into_bounds()
+
+    def after_update(self):
+        pass
+
+    def get_resume_state(self):
+        return {
+            "optim_state": self.optimizer.state_dict(),
+        }
+
+    def load_state_dict(self, state):
+        if "optim_state" in state:
+            self.optimizer.load_state_dict(state["optim_state"])
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/ppo_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/ppo_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 # LICENSE file in the root directory of this source tree.
 
 import contextlib
 import os
 import random
 import time
 from collections import defaultdict, deque
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
+import hydra
 import numpy as np
 import torch
 import tqdm
 from omegaconf import OmegaConf
 
 from habitat import VectorEnv, logger
 from habitat.config import read_write
@@ -22,17 +23,17 @@
 from habitat.tasks.rearrange.rearrange_sensors import GfxReplayMeasure
 from habitat.tasks.rearrange.utils import write_gfx_replay
 from habitat.utils import profiling_wrapper
 from habitat.utils.visualizations.utils import (
     observations_to_image,
     overlay_frame,
 )
+from habitat_baselines.common import VectorEnvFactory
 from habitat_baselines.common.base_trainer import BaseRLTrainer
 from habitat_baselines.common.baseline_registry import baseline_registry
-from habitat_baselines.common.construct_vector_env import construct_envs
 from habitat_baselines.common.env_spec import EnvironmentSpec
 from habitat_baselines.common.obs_transformers import (
     apply_obs_transforms_batch,
     apply_obs_transforms_obs_space,
     get_active_obs_transforms,
 )
 from habitat_baselines.common.tensorboard_utils import (
@@ -48,15 +49,14 @@
     load_resume_state,
     rank0_only,
     requeue_job,
     save_resume_state,
 )
 from habitat_baselines.rl.ddppo.policy import PointNavResNetNet
 from habitat_baselines.rl.ppo.agent_access_mgr import AgentAccessMgr
-from habitat_baselines.rl.ppo.policy import NetPolicy
 from habitat_baselines.rl.ppo.single_agent_access_mgr import (  # noqa: F401.
     SingleAgentAccessMgr,
 )
 from habitat_baselines.utils.common import (
     batch_obs,
     generate_video,
     get_action_space_info,
@@ -64,14 +64,15 @@
     is_continuous_action_space,
 )
 from habitat_baselines.utils.info_dict import (
     NON_SCALAR_METRICS,
     extract_scalars_from_info,
     extract_scalars_from_infos,
 )
+from habitat_baselines.utils.timing import g_timer
 
 
 @baseline_registry.register_trainer(name="ddppo")
 @baseline_registry.register_trainer(name="ppo")
 class PPOTrainer(BaseRLTrainer):
     r"""Trainer class for PPO algorithm
     Paper: https://arxiv.org/abs/1707.06347.
@@ -135,25 +136,46 @@
             **kwargs,
         )
 
     def _init_envs(self, config=None, is_eval: bool = False):
         if config is None:
             config = self.config
 
-        self.envs = construct_envs(
+        env_factory: VectorEnvFactory = hydra.utils.instantiate(
+            config.habitat_baselines.vector_env_factory
+        )
+        self.envs = env_factory.construct_envs(
             config,
             workers_ignore_signals=is_slurm_batch_job(),
             enforce_scenes_greater_eq_environments=is_eval,
+            is_first_rank=(
+                not torch.distributed.is_initialized()
+                or torch.distributed.get_rank() == 0
+            ),
         )
+
         self._env_spec = EnvironmentSpec(
             observation_space=self.envs.observation_spaces[0],
             action_space=self.envs.action_spaces[0],
             orig_action_space=self.envs.orig_action_spaces[0],
         )
 
+        # The measure keys that should only be logged on rank0 and nowhere
+        # else. They will be excluded from all other workers and only reported
+        # from the single worker.
+        self._rank0_keys: Set[str] = set(
+            list(self.config.habitat.task.rank0_env0_measure_names)
+            + list(self.config.habitat.task.rank0_measure_names)
+        )
+
+        # Information on measures that declared in `self._rank0_keys` or
+        # to be only reported on rank0. This is seperately logged from
+        # `self.window_episode_stats`.
+        self._single_proc_infos: Dict[str, List[float]] = {}
+
     def _init_train(self, resume_state=None):
         if resume_state is None:
             resume_state = load_resume_state(self.config)
 
         if resume_state is not None:
             if not self.config.habitat_baselines.load_resume_state_config:
                 raise FileExistsError(
@@ -247,20 +269,23 @@
 
         self._is_static_encoder = (
             not self.config.habitat_baselines.rl.ddppo.train_encoder
         )
         self._ppo_cfg = self.config.habitat_baselines.rl.ppo
 
         observations = self.envs.reset()
+        observations = self.envs.post_step(observations)
         batch = batch_obs(observations, device=self.device)
         batch = apply_obs_transforms_batch(batch, self.obs_transforms)  # type: ignore
 
         if self._is_static_encoder:
-            assert isinstance(self._agent.actor_critic, NetPolicy)
-            self._encoder = self._agent.actor_critic.net.visual_encoder
+            self._encoder = self._agent.actor_critic.visual_encoder
+            assert (
+                self._encoder is not None
+            ), "Visual encoder is not specified for this actor"
             with inference_mode():
                 batch[
                     PointNavResNetNet.PRETRAINED_VISUAL_FEATURES_KEY
                 ] = self._encoder(batch)
 
         self._agent.rollouts.insert_first_observations(batch)
 
@@ -269,16 +294,14 @@
             count=torch.zeros(self.envs.num_envs, 1),
             reward=torch.zeros(self.envs.num_envs, 1),
         )
         self.window_episode_stats = defaultdict(
             lambda: deque(maxlen=self._ppo_cfg.reward_window_size)
         )
 
-        self.env_time = 0.0
-        self.pth_time = 0.0
         self.t_start = time.time()
 
     @rank0_only
     @profiling_wrapper.RangeContext("save_checkpoint")
     def save_checkpoint(
         self, file_name: str, extra_state: Optional[Dict] = None
     ) -> None:
@@ -293,26 +316,29 @@
         checkpoint = {
             **self._agent.get_save_state(),
             "config": self.config,
         }
         if extra_state is not None:
             checkpoint["extra_state"] = extra_state  # type: ignore
 
-        torch.save(
-            checkpoint,
-            os.path.join(
-                self.config.habitat_baselines.checkpoint_folder, file_name
-            ),
+        save_file_path = os.path.join(
+            self.config.habitat_baselines.checkpoint_folder, file_name
         )
+        torch.save(checkpoint, save_file_path)
         torch.save(
             checkpoint,
             os.path.join(
                 self.config.habitat_baselines.checkpoint_folder, "latest.pth"
             ),
         )
+        if self.config.habitat_baselines.on_save_ckpt_callback is not None:
+            hydra.utils.call(
+                self.config.habitat_baselines.on_save_ckpt_callback,
+                save_file_path=save_file_path,
+            )
 
     def load_checkpoint(self, checkpoint_path: str, *args, **kwargs) -> Dict:
         r"""Load checkpoint of specified path as a dict.
 
         Args:
             checkpoint_path: path of target checkpoint
             *args: additional positional args
@@ -326,170 +352,170 @@
     def _compute_actions_and_step_envs(self, buffer_index: int = 0):
         num_envs = self.envs.num_envs
         env_slice = slice(
             int(buffer_index * num_envs / self._agent.nbuffers),
             int((buffer_index + 1) * num_envs / self._agent.nbuffers),
         )
 
-        t_sample_action = time.time()
-
-        # Sample actions
-        with inference_mode():
+        with g_timer.avg_time("trainer.sample_action"), inference_mode():
+            # Sample actions
             step_batch = self._agent.rollouts.get_current_step(
                 env_slice, buffer_index
             )
 
             profiling_wrapper.range_push("compute actions")
             action_data = self._agent.actor_critic.act(
                 step_batch["observations"],
                 step_batch["recurrent_hidden_states"],
                 step_batch["prev_actions"],
                 step_batch["masks"],
             )
 
-        self.pth_time += time.time() - t_sample_action
-
         profiling_wrapper.range_pop()  # compute actions
 
-        t_step_env = time.time()
-
-        for index_env, act in zip(
-            range(env_slice.start, env_slice.stop),
-            action_data.env_actions.cpu().unbind(0),
-        ):
-            if is_continuous_action_space(self._env_spec.action_space):
-                # Clipping actions to the specified limits
-                act = np.clip(
-                    act.numpy(),
-                    self._env_spec.action_space.low,
-                    self._env_spec.action_space.high,
-                )
-            else:
-                act = act.item()
-            self.envs.async_step_at(index_env, act)
-
-        self.env_time += time.time() - t_step_env
+        with g_timer.avg_time("trainer.obs_insert"):
+            for index_env, act in zip(
+                range(env_slice.start, env_slice.stop),
+                action_data.env_actions.cpu().unbind(0),
+            ):
+                if is_continuous_action_space(self._env_spec.action_space):
+                    # Clipping actions to the specified limits
+                    act = np.clip(
+                        act.numpy(),
+                        self._env_spec.action_space.low,
+                        self._env_spec.action_space.high,
+                    )
+                else:
+                    act = act.item()
+                self.envs.async_step_at(index_env, act)
 
-        self._agent.rollouts.insert(
-            next_recurrent_hidden_states=action_data.rnn_hidden_states,
-            actions=action_data.actions,
-            action_log_probs=action_data.action_log_probs,
-            value_preds=action_data.values,
-            buffer_index=buffer_index,
-            should_inserts=action_data.should_inserts,
-        )
+        with g_timer.avg_time("trainer.obs_insert"):
+            self._agent.rollouts.insert(
+                next_recurrent_hidden_states=action_data.rnn_hidden_states,
+                actions=action_data.actions,
+                action_log_probs=action_data.action_log_probs,
+                value_preds=action_data.values,
+                buffer_index=buffer_index,
+                should_inserts=action_data.should_inserts,
+            )
 
     def _collect_environment_result(self, buffer_index: int = 0):
         num_envs = self.envs.num_envs
         env_slice = slice(
             int(buffer_index * num_envs / self._agent.nbuffers),
             int((buffer_index + 1) * num_envs / self._agent.nbuffers),
         )
 
-        t_step_env = time.time()
-        outputs = [
-            self.envs.wait_step_at(index_env)
-            for index_env in range(env_slice.start, env_slice.stop)
-        ]
-
-        observations, rewards_l, dones, infos = [
-            list(x) for x in zip(*outputs)
-        ]
-
-        self.env_time += time.time() - t_step_env
-
-        t_update_stats = time.time()
-        batch = batch_obs(observations, device=self.device)
-        batch = apply_obs_transforms_batch(batch, self.obs_transforms)  # type: ignore
+        with g_timer.avg_time("trainer.step_env"):
+            outputs = [
+                self.envs.wait_step_at(index_env)
+                for index_env in range(env_slice.start, env_slice.stop)
+            ]
 
-        rewards = torch.tensor(
-            rewards_l,
-            dtype=torch.float,
-            device=self.current_episode_reward.device,
-        )
-        rewards = rewards.unsqueeze(1)
+            observations, rewards_l, dones, infos = [
+                list(x) for x in zip(*outputs)
+            ]
 
-        not_done_masks = torch.tensor(
-            [[not done] for done in dones],
-            dtype=torch.bool,
-            device=self.current_episode_reward.device,
-        )
-        done_masks = torch.logical_not(not_done_masks)
+        with g_timer.avg_time("trainer.update_stats"):
+            observations = self.envs.post_step(observations)
+            batch = batch_obs(observations, device=self.device)
+            batch = apply_obs_transforms_batch(batch, self.obs_transforms)  # type: ignore
 
-        self.current_episode_reward[env_slice] += rewards
-        current_ep_reward = self.current_episode_reward[env_slice]
-        self.running_episode_stats["reward"][env_slice] += current_ep_reward.where(done_masks, current_ep_reward.new_zeros(()))  # type: ignore
-        self.running_episode_stats["count"][env_slice] += done_masks.float()  # type: ignore
-        for k, v_k in extract_scalars_from_infos(infos).items():
-            v = torch.tensor(
-                v_k,
+            rewards = torch.tensor(
+                rewards_l,
                 dtype=torch.float,
                 device=self.current_episode_reward.device,
-            ).unsqueeze(1)
-            if k not in self.running_episode_stats:
-                self.running_episode_stats[k] = torch.zeros_like(
-                    self.running_episode_stats["count"]
-                )
-            self.running_episode_stats[k][env_slice] += v.where(done_masks, v.new_zeros(()))  # type: ignore
+            )
+            rewards = rewards.unsqueeze(1)
+
+            not_done_masks = torch.tensor(
+                [[not done] for done in dones],
+                dtype=torch.bool,
+                device=self.current_episode_reward.device,
+            )
+            done_masks = torch.logical_not(not_done_masks)
+
+            self.current_episode_reward[env_slice] += rewards
+            current_ep_reward = self.current_episode_reward[env_slice]
+            self.running_episode_stats["reward"][env_slice] += current_ep_reward.where(done_masks, current_ep_reward.new_zeros(()))  # type: ignore
+            self.running_episode_stats["count"][env_slice] += done_masks.float()  # type: ignore
+
+            self._single_proc_infos = extract_scalars_from_infos(
+                infos,
+                ignore_keys=set(
+                    k for k in infos[0].keys() if k not in self._rank0_keys
+                ),
+            )
+            extracted_infos = extract_scalars_from_infos(
+                infos, ignore_keys=self._rank0_keys
+            )
+            for k, v_k in extracted_infos.items():
+                v = torch.tensor(
+                    v_k,
+                    dtype=torch.float,
+                    device=self.current_episode_reward.device,
+                ).unsqueeze(1)
+                if k not in self.running_episode_stats:
+                    self.running_episode_stats[k] = torch.zeros_like(
+                        self.running_episode_stats["count"]
+                    )
+                self.running_episode_stats[k][env_slice] += v.where(done_masks, v.new_zeros(()))  # type: ignore
 
-        self.current_episode_reward[env_slice].masked_fill_(done_masks, 0.0)
+            self.current_episode_reward[env_slice].masked_fill_(
+                done_masks, 0.0
+            )
 
         if self._is_static_encoder:
-            with inference_mode():
+            with inference_mode(), g_timer.avg_time("trainer.visual_features"):
                 batch[
                     PointNavResNetNet.PRETRAINED_VISUAL_FEATURES_KEY
                 ] = self._encoder(batch)
 
         self._agent.rollouts.insert(
             next_observations=batch,
             rewards=rewards,
             next_masks=not_done_masks,
             buffer_index=buffer_index,
         )
 
         self._agent.rollouts.advance_rollout(buffer_index)
 
-        self.pth_time += time.time() - t_update_stats
-
         return env_slice.stop - env_slice.start
 
     @profiling_wrapper.RangeContext("_collect_rollout_step")
     def _collect_rollout_step(self):
         self._compute_actions_and_step_envs()
         return self._collect_environment_result()
 
     @profiling_wrapper.RangeContext("_update_agent")
+    @g_timer.avg_time("trainer.update_agent")
     def _update_agent(self):
-        t_update_model = time.time()
-
         with inference_mode():
             step_batch = self._agent.rollouts.get_last_step()
-
             next_value = self._agent.actor_critic.get_value(
                 step_batch["observations"],
-                step_batch["recurrent_hidden_states"],
+                step_batch.get("recurrent_hidden_states", None),
                 step_batch["prev_actions"],
                 step_batch["masks"],
             )
 
         self._agent.rollouts.compute_returns(
             next_value,
             self._ppo_cfg.use_gae,
             self._ppo_cfg.gamma,
             self._ppo_cfg.tau,
         )
 
         self._agent.train()
 
         losses = self._agent.updater.update(self._agent.rollouts)
-        self._agent.rollouts.after_update()
 
+        self._agent.rollouts.after_update()
         self._agent.after_update()
 
-        self.pth_time += time.time() - t_update_model
         return losses
 
     def _coalesce_post_step(
         self, losses: Dict[str, float], count_steps_delta: int
     ) -> Dict[str, float]:
         stats_ordering = sorted(self.running_episode_stats.keys())
         stats = torch.stack(
@@ -552,49 +578,62 @@
         }
 
         for k, v in metrics.items():
             writer.add_scalar(f"metrics/{k}", v, self.num_steps_done)
         for k, v in losses.items():
             writer.add_scalar(f"learner/{k}", v, self.num_steps_done)
 
+        for k, v in self._single_proc_infos.items():
+            writer.add_scalar(k, np.mean(v), self.num_steps_done)
+
         fps = self.num_steps_done / ((time.time() - self.t_start) + prev_time)
+
+        # Log perf metrics.
         writer.add_scalar("perf/fps", fps, self.num_steps_done)
 
+        for timer_name, timer_val in g_timer.items():
+            writer.add_scalar(
+                f"perf/{timer_name}",
+                timer_val.mean,
+                self.num_steps_done,
+            )
+
         # log stats
         if (
             self.num_updates_done % self.config.habitat_baselines.log_interval
             == 0
         ):
             logger.info(
                 "update: {}\tfps: {:.3f}\t".format(
                     self.num_updates_done,
                     fps,
                 )
             )
 
             logger.info(
-                "update: {}\tenv-time: {:.3f}s\tpth-time: {:.3f}s\t"
-                "frames: {}".format(
-                    self.num_updates_done,
-                    self.env_time,
-                    self.pth_time,
-                    self.num_steps_done,
-                )
+                f"Num updates: {self.num_updates_done}\tNum frames {self.num_steps_done}"
             )
 
             logger.info(
                 "Average window size: {}  {}".format(
                     len(self.window_episode_stats["count"]),
                     "  ".join(
                         "{}: {:.3f}".format(k, v / deltas["count"])
                         for k, v in deltas.items()
                         if k != "count"
                     ),
                 )
             )
+            perf_stats_str = " ".join(
+                [f"{k}: {v.mean:.3f}" for k, v in g_timer.items()]
+            )
+            logger.info(f"\tPerf Stats: {perf_stats_str}")
+            if self.config.habitat_baselines.should_log_single_proc_infos:
+                for k, v in self._single_proc_infos.items():
+                    logger.info(f" - {k}: {np.mean(v):.3f}")
 
     def should_end_early(self, rollout_step) -> bool:
         if not self._is_distributed:
             return False
         # This is where the preemption of workers happens.  If a
         # worker detects it will be a straggler, it preempts itself!
         return (
@@ -624,16 +663,14 @@
             torch.distributed.barrier()
 
         resume_run_id = None
         if resume_state is not None:
             self._agent.load_state_dict(resume_state)
 
             requeue_stats = resume_state["requeue_stats"]
-            self.env_time = requeue_stats["env_time"]
-            self.pth_time = requeue_stats["pth_time"]
             self.num_steps_done = requeue_stats["num_steps_done"]
             self.num_updates_done = requeue_stats["num_updates_done"]
             self._last_checkpoint_percent = requeue_stats[
                 "_last_checkpoint_percent"
             ]
             count_checkpoints = requeue_stats["count_checkpoints"]
             prev_time = requeue_stats["prev_time"]
@@ -658,16 +695,14 @@
                 profiling_wrapper.on_start_step()
                 profiling_wrapper.range_push("train update")
 
                 self._agent.pre_rollout()
 
                 if rank0_only() and self._should_save_resume_state():
                     requeue_stats = dict(
-                        env_time=self.env_time,
-                        pth_time=self.pth_time,
                         count_checkpoints=count_checkpoints,
                         num_steps_done=self.num_steps_done,
                         num_updates_done=self.num_updates_done,
                         _last_checkpoint_percent=self._last_checkpoint_percent,
                         prev_time=(time.time() - self.t_start) + prev_time,
                         running_episode_stats=self.running_episode_stats,
                         window_episode_stats=dict(self.window_episode_stats),
@@ -693,41 +728,44 @@
                     return
 
                 self._agent.eval()
                 count_steps_delta = 0
                 profiling_wrapper.range_push("rollouts loop")
 
                 profiling_wrapper.range_push("_collect_rollout_step")
-                for buffer_index in range(self._agent.nbuffers):
-                    self._compute_actions_and_step_envs(buffer_index)
-
-                for step in range(self._ppo_cfg.num_steps):
-                    is_last_step = (
-                        self.should_end_early(step + 1)
-                        or (step + 1) == self._ppo_cfg.num_steps
-                    )
-
+                with g_timer.avg_time("trainer.rollout_collect"):
                     for buffer_index in range(self._agent.nbuffers):
-                        count_steps_delta += self._collect_environment_result(
-                            buffer_index
+                        self._compute_actions_and_step_envs(buffer_index)
+
+                    for step in range(self._ppo_cfg.num_steps):
+                        is_last_step = (
+                            self.should_end_early(step + 1)
+                            or (step + 1) == self._ppo_cfg.num_steps
                         )
 
-                        if (buffer_index + 1) == self._agent.nbuffers:
-                            profiling_wrapper.range_pop()  # _collect_rollout_step
+                        for buffer_index in range(self._agent.nbuffers):
+                            count_steps_delta += (
+                                self._collect_environment_result(buffer_index)
+                            )
 
-                        if not is_last_step:
                             if (buffer_index + 1) == self._agent.nbuffers:
-                                profiling_wrapper.range_push(
-                                    "_collect_rollout_step"
-                                )
+                                profiling_wrapper.range_pop()  # _collect_rollout_step
+
+                            if not is_last_step:
+                                if (buffer_index + 1) == self._agent.nbuffers:
+                                    profiling_wrapper.range_push(
+                                        "_collect_rollout_step"
+                                    )
 
-                            self._compute_actions_and_step_envs(buffer_index)
+                                self._compute_actions_and_step_envs(
+                                    buffer_index
+                                )
 
-                    if is_last_step:
-                        break
+                        if is_last_step:
+                            break
 
                 profiling_wrapper.range_pop()  # rollouts loop
 
                 if self._is_distributed:
                     self.num_rollouts_done_store.add("num_done", 1)
 
                 losses = self._update_agent()
@@ -778,15 +816,15 @@
         # a hierarchial policy
         if self.config.habitat_baselines.eval.should_load_ckpt:
             # map_location="cpu" is almost always better than mapping to a CUDA device.
             ckpt_dict = self.load_checkpoint(
                 checkpoint_path, map_location="cpu"
             )
             step_id = ckpt_dict["extra_state"]["step"]
-            print(step_id)
+            logger.info(f"Loaded checkpoint trained for {step_id} steps")
         else:
             ckpt_dict = {"config": None}
 
         config = self._get_resume_state_config_or_new_config(
             ckpt_dict["config"]
         )
 
@@ -818,28 +856,33 @@
             self._agent.policy_action_space
         )
 
         if self._agent.actor_critic.should_load_agent_state:
             self._agent.load_state_dict(ckpt_dict)
 
         observations = self.envs.reset()
+        observations = self.envs.post_step(observations)
         batch = batch_obs(observations, device=self.device)
         batch = apply_obs_transforms_batch(batch, self.obs_transforms)  # type: ignore
 
         current_episode_reward = torch.zeros(
             self.envs.num_envs, 1, device="cpu"
         )
 
         test_recurrent_hidden_states = torch.zeros(
             (
                 self.config.habitat_baselines.num_environments,
-                *self._agent.hidden_state_shape,
+                self._agent.actor_critic.num_recurrent_layers,
+                self._agent.actor_critic.recurrent_hidden_size,
             ),
             device=self.device,
         )
+        should_update_recurrent_hidden_states = (
+            np.prod(test_recurrent_hidden_states.shape) != 0
+        )
         prev_actions = torch.zeros(
             self.config.habitat_baselines.num_environments,
             *action_shape,
             device=self.device,
             dtype=torch.long if discrete_actions else torch.float,
         )
         not_done_masks = torch.zeros(
@@ -849,17 +892,29 @@
             dtype=torch.bool,
         )
         stats_episodes: Dict[
             Any, Any
         ] = {}  # dict of dicts that stores stats per episode
         ep_eval_count: Dict[Any, int] = defaultdict(lambda: 0)
 
-        rgb_frames: List[List[np.ndarray]] = [
-            [] for _ in range(self.config.habitat_baselines.num_environments)
-        ]
+        if len(self.config.habitat_baselines.eval.video_option) > 0:
+            # Add the first frame of the episode to the video.
+            rgb_frames: List[List[np.ndarray]] = [
+                [
+                    observations_to_image(
+                        {k: v[env_idx] for k, v in batch.items()}, {}
+                    )
+                ]
+                for env_idx in range(
+                    self.config.habitat_baselines.num_environments
+                )
+            ]
+        else:
+            rgb_frames = None
+
         if len(self.config.habitat_baselines.eval.video_option) > 0:
             os.makedirs(self.config.habitat_baselines.video_dir, exist_ok=True)
 
         number_of_eval_episodes = (
             self.config.habitat_baselines.test_episode_count
         )
         evals_per_ep = self.config.habitat_baselines.eval.evals_per_ep
@@ -902,19 +957,21 @@
                         action_data.rnn_hidden_states
                     )
                     prev_actions.copy_(action_data.actions)  # type: ignore
                 else:
                     for i, should_insert in enumerate(
                         action_data.should_inserts
                     ):
-                        if should_insert.item():
+                        if not should_insert.item():
+                            continue
+                        if should_update_recurrent_hidden_states:
                             test_recurrent_hidden_states[
                                 i
                             ] = action_data.rnn_hidden_states[i]
-                            prev_actions[i].copy_(action_data.actions[i])  # type: ignore
+                        prev_actions[i].copy_(action_data.actions[i])  # type: ignore
             # NB: Move actions to CPU.  If CUDA tensors are
             # sent in to env.step(), that will create CUDA contexts
             # in the subprocesses.
             if is_continuous_action_space(self._env_spec.action_space):
                 # Clipping actions to the specified limits
                 step_data = [
                     np.clip(
@@ -928,19 +985,24 @@
                 step_data = [a.item() for a in action_data.env_actions.cpu()]
 
             outputs = self.envs.step(step_data)
 
             observations, rewards_l, dones, infos = [
                 list(x) for x in zip(*outputs)
             ]
+            # Note that `policy_infos` represents the information about the
+            # action BEFORE `observations` (the action used to transition to
+            # `observations`).
             policy_infos = self._agent.actor_critic.get_extra(
                 action_data, infos, dones
             )
             for i in range(len(policy_infos)):
                 infos[i].update(policy_infos[i])
+
+            observations = self.envs.post_step(observations)
             batch = batch_obs(  # type: ignore
                 observations,
                 device=self.device,
             )
             batch = apply_obs_transforms_batch(batch, self.obs_transforms)  # type: ignore
 
             not_done_masks = torch.tensor(
@@ -964,27 +1026,40 @@
                             next_episodes_info[i].episode_id,
                         )
                     ]
                     == evals_per_ep
                 ):
                     envs_to_pause.append(i)
 
+                # Exclude the keys from `_rank0_keys` from displaying in the video
+                disp_info = {
+                    k: v
+                    for k, v in infos[i].items()
+                    if k not in self._rank0_keys
+                }
+
                 if len(self.config.habitat_baselines.eval.video_option) > 0:
                     # TODO move normalization / channel changing out of the policy and undo it here
                     frame = observations_to_image(
-                        {k: v[i] for k, v in batch.items()}, infos[i]
+                        {k: v[i] for k, v in batch.items()}, disp_info
                     )
                     if not not_done_masks[i].item():
                         # The last frame corresponds to the first frame of the next episode
                         # but the info is correct. So we use a black frame
-                        frame = observations_to_image(
-                            {k: v[i] * 0.0 for k, v in batch.items()}, infos[i]
+                        final_frame = observations_to_image(
+                            {k: v[i] * 0.0 for k, v in batch.items()},
+                            disp_info,
                         )
-                    frame = overlay_frame(frame, infos[i])
-                    rgb_frames[i].append(frame)
+                        final_frame = overlay_frame(final_frame, disp_info)
+                        rgb_frames[i].append(final_frame)
+                        # The starting frame of the next episode will be the final element..
+                        rgb_frames[i].append(frame)
+                    else:
+                        frame = overlay_frame(frame, disp_info)
+                        rgb_frames[i].append(frame)
 
                 # episode ended
                 if not not_done_masks[i].item():
                     pbar.update()
                     episode_stats = {
                         "reward": current_episode_reward[i].item()
                     }
@@ -1001,24 +1076,26 @@
                     if (
                         len(self.config.habitat_baselines.eval.video_option)
                         > 0
                     ):
                         generate_video(
                             video_option=self.config.habitat_baselines.eval.video_option,
                             video_dir=self.config.habitat_baselines.video_dir,
-                            images=rgb_frames[i],
-                            episode_id=current_episodes_info[i].episode_id,
+                            # Since the final frame is the start frame of the next episode.
+                            images=rgb_frames[i][:-1],
+                            episode_id=f"{current_episodes_info[i].episode_id}_{ep_eval_count[k]}",
                             checkpoint_idx=checkpoint_index,
-                            metrics=extract_scalars_from_info(infos[i]),
+                            metrics=extract_scalars_from_info(disp_info),
                             fps=self.config.habitat_baselines.video_fps,
                             tb_writer=writer,
                             keys_to_include_in_name=self.config.habitat_baselines.eval_keys_to_include_in_name,
                         )
 
-                        rgb_frames[i] = []
+                        # Since the starting frame of the next episode is the final frame.
+                        rgb_frames[i] = rgb_frames[i][-1:]
 
                     gfx_str = infos[i].get(GfxReplayMeasure.cls_uuid, "")
                     if gfx_str != "":
                         write_gfx_replay(
                             gfx_str,
                             self.config.habitat.task,
                             current_episodes_info[i].episode_id,
@@ -1046,17 +1123,20 @@
 
         pbar.close()
         assert (
             len(ep_eval_count) >= number_of_eval_episodes
         ), f"Expected {number_of_eval_episodes} episodes, got {len(ep_eval_count)}."
 
         aggregated_stats = {}
-        for stat_key in next(iter(stats_episodes.values())).keys():
+        all_ks = set()
+        for ep in stats_episodes.values():
+            all_ks.update(ep.keys())
+        for stat_key in all_ks:
             aggregated_stats[stat_key] = np.mean(
-                [v[stat_key] for v in stats_episodes.values()]
+                [v[stat_key] for v in stats_episodes.values() if stat_key in v]
             )
 
         for k, v in aggregated_stats.items():
             logger.info(f"Average episode {k}: {v:.4f}")
 
         step_id = checkpoint_index
         if "extra_state" in ckpt_dict and "step" in ckpt_dict["extra_state"]:
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ppo/single_agent_access_mgr.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ppo/single_agent_access_mgr.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,29 +75,62 @@
         else:
             self._lr_scheduler = LambdaLR(
                 optimizer=self._updater.optimizer,
                 lr_lambda=lambda _: lr_schedule_fn(self._percent_done_fn()),
             )
         if resume_state is not None:
             self._updater.load_state_dict(resume_state["state_dict"])
-            self._updater.optimizer.load_state_dict(
-                resume_state["optim_state"]
+            self._updater.load_state_dict(
+                {
+                    "actor_critic." + k: v
+                    for k, v, in resume_state["state_dict"].items()
+                }
             )
         self._policy_action_space = self._actor_critic.get_policy_action_space(
             self._env_spec.action_space
         )
 
     @property
     def nbuffers(self):
         return self._nbuffers
 
+    def _create_storage(
+        self,
+        num_envs: int,
+        env_spec: EnvironmentSpec,
+        actor_critic: Policy,
+        policy_action_space: spaces.Space,
+        config: "DictConfig",
+        device,
+    ) -> Storage:
+        """
+        Default behavior for setting up and initializing the rollout storage.
+        """
+
+        obs_space = get_rollout_obs_space(
+            env_spec.observation_space, actor_critic, config
+        )
+        ppo_cfg = config.habitat_baselines.rl.ppo
+        rollouts = baseline_registry.get_storage(
+            config.habitat_baselines.rollout_storage_name
+        )(
+            numsteps=ppo_cfg.num_steps,
+            num_envs=num_envs,
+            observation_space=obs_space,
+            action_space=policy_action_space,
+            actor_critic=actor_critic,
+            is_double_buffered=ppo_cfg.use_double_buffered_sampler,
+        )
+        rollouts.to(device)
+        return rollouts
+
     def post_init(self, create_rollouts_fn: Optional[Callable] = None) -> None:
         # Create the rollouts storage.
         if create_rollouts_fn is None:
-            create_rollouts_fn = default_create_rollouts
+            create_rollouts_fn = self._create_storage
 
         policy_action_space = self._actor_critic.get_policy_action_space(
             self._env_spec.action_space
         )
         self._rollouts = create_rollouts_fn(
             num_envs=self._num_envs,
             env_spec=self._env_spec,
@@ -165,15 +198,15 @@
                 {
                     k[len(prefix) :]: v
                     for k, v in pretrained_state["state_dict"].items()
                     if k.startswith(prefix)
                 }
             )
         if self._is_static_encoder:
-            for param in actor_critic.net.visual_encoder.parameters():
+            for param in actor_critic.visual_encoder.parameters():
                 param.requires_grad_(False)
 
         if self._config.habitat_baselines.rl.ddppo.reset_critic:
             nn.init.orthogonal_(actor_critic.critic.fc.weight)
             nn.init.constant_(actor_critic.critic.fc.bias, 0)
 
         actor_critic.to(self._device)
@@ -190,15 +223,15 @@
     @property
     def updater(self) -> Updater:
         return self._updater
 
     def get_resume_state(self) -> Dict[str, Any]:
         ret = {
             "state_dict": self._actor_critic.state_dict(),
-            "optim_state": self._updater.optimizer.state_dict(),
+            **self._updater.get_resume_state(),
         }
         if self._lr_scheduler is not None:
             ret["lr_sched_state"] = (self._lr_scheduler.state_dict(),)
         return ret
 
     def get_save_state(self):
         return {"state_dict": self._actor_critic.state_dict()}
@@ -212,32 +245,25 @@
 
     def load_ckpt_state_dict(self, ckpt: Dict) -> None:
         self._actor_critic.load_state_dict(ckpt["state_dict"])
 
     def load_state_dict(self, state: Dict) -> None:
         self._actor_critic.load_state_dict(state["state_dict"])
         if self._updater is not None:
-            if "optim_state" in state:
-                self._actor_critic.load_state_dict(state["optim_state"])
+            self._updater.load_state_dict(state)
             if "lr_sched_state" in state:
-                self._actor_critic.load_state_dict(state["lr_sched_state"])
-
-    @property
-    def hidden_state_shape(self):
-        return (
-            self.actor_critic.num_recurrent_layers,
-            self._ppo_cfg.hidden_size,
-        )
+                self._lr_scheduler.load_state_dict(state["lr_sched_state"])
 
     def after_update(self):
         if (
             self._ppo_cfg.use_linear_lr_decay
             and self._lr_scheduler is not None
         ):
             self._lr_scheduler.step()  # type: ignore
+        self._updater.after_update()
 
     def pre_rollout(self):
         if self._ppo_cfg.use_linear_clip_decay:
             self._updater.clip_param = self._ppo_cfg.clip_param * (
                 1 - self._percent_done_fn()
             )
 
@@ -245,55 +271,24 @@
 def get_rollout_obs_space(obs_space, actor_critic, config):
     """
     Helper to get the observation space for the rollout storage when using a
     frozen visual encoder.
     """
 
     if not config.habitat_baselines.rl.ddppo.train_encoder:
-        encoder = actor_critic.net.visual_encoder
+        encoder = actor_critic.visual_encoder
         obs_space = spaces.Dict(
             {
                 PointNavResNetNet.PRETRAINED_VISUAL_FEATURES_KEY: spaces.Box(
                     low=np.finfo(np.float32).min,
                     high=np.finfo(np.float32).max,
                     shape=encoder.output_shape,
                     dtype=np.float32,
                 ),
                 **obs_space.spaces,
             }
         )
     return obs_space
 
 
-def default_create_rollouts(
-    num_envs: int,
-    env_spec: EnvironmentSpec,
-    actor_critic: NetPolicy,
-    policy_action_space: spaces.Space,
-    config: "DictConfig",
-    device,
-) -> Storage:
-    """
-    Default behavior for setting up and initializing the rollout storage.
-    """
-
-    obs_space = get_rollout_obs_space(
-        env_spec.observation_space, actor_critic, config
-    )
-    ppo_cfg = config.habitat_baselines.rl.ppo
-    rollouts = baseline_registry.get_storage(
-        config.habitat_baselines.rollout_storage_name
-    )(
-        ppo_cfg.num_steps,
-        num_envs,
-        obs_space,
-        policy_action_space,
-        ppo_cfg.hidden_size,
-        num_recurrent_layers=actor_critic.num_recurrent_layers,
-        is_double_buffered=ppo_cfg.use_double_buffered_sampler,
-    )
-    rollouts.to(device)
-    return rollouts
-
-
 def linear_lr_schedule(percent_done: float) -> float:
     return 1 - percent_done
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/environment_worker.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/environment_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 from habitat.gym.gym_env_obs_dict_wrapper import EnvObsDictWrapper
 from habitat_baselines.common.tensor_dict import NDArrayDict, TensorDict
 from habitat_baselines.rl.ver.queue import BatchedQueue
 from habitat_baselines.rl.ver.task_enums import (
     EnvironmentWorkerTasks,
     ReportWorkerTasks,
 )
-from habitat_baselines.rl.ver.timing import Timing
 from habitat_baselines.rl.ver.worker_common import (
     ProcessBase,
     WorkerBase,
     WorkerQueues,
 )
 from habitat_baselines.utils.common import (
     inference_mode,
     is_continuous_action_space,
 )
+from habitat_baselines.utils.timing import Timing
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
 
 MIN_SCENES_PER_ENV = 16
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/inference_worker.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/inference_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 from habitat_baselines.rl.ppo.policy import NetPolicy
 from habitat_baselines.rl.ver.task_enums import (
     EnvironmentWorkerTasks,
     InferenceWorkerTasks,
     PreemptionDeciderTasks,
     ReportWorkerTasks,
 )
-from habitat_baselines.rl.ver.timing import Timing
 from habitat_baselines.rl.ver.ver_rollout_storage import VERRolloutStorage
 from habitat_baselines.rl.ver.worker_common import (
     InferenceWorkerSync,
     ProcessBase,
     RolloutEarlyEnds,
     WorkerBase,
     WorkerQueues,
 )
 from habitat_baselines.utils.common import batch_obs, inference_mode
+from habitat_baselines.utils.timing import Timing
 
 if TYPE_CHECKING:
     from omegaconf import DictConfig
 
 
 @attr.s(auto_attribs=True)
 class InferenceWorkerProcess(ProcessBase):
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/preemption_decider.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/preemption_decider.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/queue.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/queue.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/report_worker.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/report_worker.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/task_enums.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/task_enums.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/ver_rollout_storage.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_rollout_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,30 +133,28 @@
 
     next_hidden_states: torch.Tensor
     next_prev_actions: torch.Tensor
     current_policy_version: torch.Tensor
 
     def __init__(
         self,
-        variable_experience: bool,
         numsteps,
         num_envs,
         observation_space,
         action_space,
-        recurrent_hidden_state_size,
-        num_recurrent_layers=1,
+        actor_critic,
+        variable_experience: bool,
         is_double_buffered: bool = False,
     ):
         super().__init__(
             numsteps,
             num_envs,
             observation_space,
             action_space,
-            recurrent_hidden_state_size,
-            num_recurrent_layers,
+            actor_critic,
             is_double_buffered,
         )
         self.use_is_coeffs = variable_experience
 
         if self.use_is_coeffs:
             self.buffers["is_coeffs"] = torch.ones_like(
                 self.buffers["returns"]
@@ -565,21 +563,21 @@
             assert torch.isfinite(returns_t).long().sum() == (
                 self.num_steps * self._num_envs
             ), returns_t.squeeze().numpy()[self.select_inds]
 
         self.buffers["returns"].copy_(returns_t, non_blocking=True)
         self.current_rollout_step_idxs[0] = self.num_steps
 
-    def recurrent_generator(
+    def data_generator(
         self,
         advantages: Optional[torch.Tensor],
         num_mini_batch: int,
     ) -> Iterator[DictTree]:
         if not self.variable_experience:
-            yield from super().recurrent_generator(advantages, num_mini_batch)
+            yield from super().data_generator(advantages, num_mini_batch)
         else:
             for mb_inds in generate_ver_mini_batches(
                 num_mini_batch,
                 self.sequence_lengths,
                 self.num_seqs_at_step,
                 self.select_inds,
                 self.last_sequence_in_batch_mask,
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/ver_trainer.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/ver_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 from habitat_baselines.rl.ver.inference_worker import (
     InferenceWorker,
     InferenceWorkerProcess,
 )
 from habitat_baselines.rl.ver.preemption_decider import PreemptionDeciderWorker
 from habitat_baselines.rl.ver.report_worker import ReportWorker
 from habitat_baselines.rl.ver.task_enums import ReportWorkerTasks
-from habitat_baselines.rl.ver.timing import Timing
 from habitat_baselines.rl.ver.ver_rollout_storage import VERRolloutStorage
 from habitat_baselines.rl.ver.worker_common import (
     InferenceWorkerSync,
     WorkerBase,
     WorkerQueues,
 )
 from habitat_baselines.utils.common import cosine_decay, inference_mode
+from habitat_baselines.utils.timing import Timing
 
 try:
     torch.backends.cudnn.allow_tf32 = True
     torch.backends.cuda.matmul.allow_tf32 = True
 except AttributeError:
     pass
 
@@ -71,20 +71,24 @@
             self.config.habitat_baselines.rl.agent.type
         )(
             config=self.config,
             env_spec=self._env_spec,
             is_distrib=self._is_distributed,
             device=self.device,
             resume_state=resume_state,
-            num_envs=len(self.environment_workers),
+            num_envs=self.config.habitat_baselines.num_environments,
             percent_done_fn=self.percent_done,
             **kwargs,
         )
 
     def _init_train(self, resume_state):
+        assert (
+            not self.config.habitat.simulator.renderer.enable_batch_renderer
+        ), "VER trainer does not support batch rendering."
+
         if self._is_distributed:
             local_rank, world_rank, _ = get_distrib_size()
 
             with read_write(self.config):
                 self.config.habitat_baselines.torch_gpu_id = local_rank
                 self.config.habitat.simulator.habitat_sim_v0.gpu_device_id = (
                     local_rank
@@ -234,16 +238,15 @@
             self.config,
         )
         storage_kwargs = {
             "variable_experience": self.ver_config.variable_experience,
             "numsteps": ppo_cfg.num_steps,
             "num_envs": len(self.environment_workers),
             "action_space": self._env_spec.action_space,
-            "recurrent_hidden_state_size": ppo_cfg.hidden_size,
-            "num_recurrent_layers": self._agent.actor_critic.net.num_recurrent_layers,
+            "actor_critic": self._agent.actor_critic,
             "observation_space": rollouts_obs_space,
         }
 
         def create_ver_rollouts_fn(
             device,
             **kwargs,
         ):
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/rl/ver/worker_common.py` & `habitat-baselines-0.2.520230729/habitat_baselines/rl/ver/worker_common.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/run.py` & `habitat-baselines-0.2.520230729/habitat_baselines/run.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/utils/common.py` & `habitat-baselines-0.2.520230729/habitat_baselines/utils/common.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines/utils/visualizations/utils.py` & `habitat-baselines-0.2.520230729/habitat_baselines/utils/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines.egg-info/PKG-INFO` & `habitat-baselines-0.2.520230729/habitat_baselines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-baselines
-Version: 0.2.420230405
+Version: 0.2.520230729
 Summary: Habitat-Baselines: Embodied AI baselines.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-baselines-0.2.420230405/habitat_baselines.egg-info/SOURCES.txt` & `habitat-baselines-0.2.520230729/habitat_baselines.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 habitat_baselines/agents/__init__.py
 habitat_baselines/agents/ppo_agents.py
 habitat_baselines/agents/simple_agents.py
 habitat_baselines/common/__init__.py
 habitat_baselines/common/base_il_trainer.py
 habitat_baselines/common/base_trainer.py
 habitat_baselines/common/baseline_registry.py
-habitat_baselines/common/construct_vector_env.py
+habitat_baselines/common/env_factory.py
 habitat_baselines/common/env_spec.py
+habitat_baselines/common/habitat_env_factory.py
 habitat_baselines/common/logging.py
 habitat_baselines/common/obs_transformers.py
 habitat_baselines/common/rollout_storage.py
 habitat_baselines/common/storage.py
 habitat_baselines/common/tensor_dict.py
 habitat_baselines/common/tensorboard_utils.py
 habitat_baselines/common/windowed_running_mean.py
@@ -90,16 +91,16 @@
 habitat_baselines/rl/ver/environment_worker.py
 habitat_baselines/rl/ver/inference_worker.py
 habitat_baselines/rl/ver/preemption_decider.py
 habitat_baselines/rl/ver/queue.py
 habitat_baselines/rl/ver/report_worker.py
 habitat_baselines/rl/ver/requirements.txt
 habitat_baselines/rl/ver/task_enums.py
-habitat_baselines/rl/ver/timing.py
 habitat_baselines/rl/ver/ver_rollout_storage.py
 habitat_baselines/rl/ver/ver_trainer.py
 habitat_baselines/rl/ver/worker_common.py
 habitat_baselines/utils/__init__.py
 habitat_baselines/utils/common.py
 habitat_baselines/utils/info_dict.py
+habitat_baselines/utils/timing.py
 habitat_baselines/utils/visualizations/__init__.py
 habitat_baselines/utils/visualizations/utils.py
```

### Comparing `habitat-baselines-0.2.420230405/setup.py` & `habitat-baselines-0.2.520230729/setup.py`

 * *Files identical despite different names*

