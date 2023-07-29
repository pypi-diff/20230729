# Comparing `tmp/xpag-0.2.0-py3-none-any.whl.zip` & `tmp/xpag-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,69 @@
-Zip file size: 55026 bytes, number of entries: 40
--rw-r--r--  2.0 unx      211 b- defN 23-Jul-12 09:50 xpag/__init__.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-12 09:50 xpag/agents/__init__.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Jul-12 09:50 xpag/agents/agent.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:50 xpag/agents/sac/__init__.py
--rw-r--r--  2.0 unx     5594 b- defN 23-Jul-12 09:50 xpag/agents/sac/sac.py
--rw-r--r--  2.0 unx    18793 b- defN 23-Jul-12 09:50 xpag/agents/sac/sac_from_jaxrl.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:50 xpag/agents/sdqn/__init__.py
--rw-r--r--  2.0 unx    22289 b- defN 23-Jul-12 09:50 xpag/agents/sdqn/sdqn.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:50 xpag/agents/td3/__init__.py
--rw-r--r--  2.0 unx    15288 b- defN 23-Jul-12 09:50 xpag/agents/td3/td3.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 09:50 xpag/agents/tqc/__init__.py
--rw-r--r--  2.0 unx    13028 b- defN 23-Jul-12 09:50 xpag/agents/tqc/tqc.py
--rw-r--r--  2.0 unx      160 b- defN 23-Jul-12 09:50 xpag/buffers/__init__.py
--rw-r--r--  2.0 unx    11221 b- defN 23-Jul-12 09:50 xpag/buffers/buffer.py
--rw-r--r--  2.0 unx     5236 b- defN 23-Jul-12 09:50 xpag/buffers/jax_buffer.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-12 09:50 xpag/plotting/__init__.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jul-12 09:50 xpag/plotting/plotting.py
--rw-r--r--  2.0 unx     2841 b- defN 23-Jul-12 09:50 xpag/samplers/HER.py
--rw-r--r--  2.0 unx      182 b- defN 23-Jul-12 09:50 xpag/samplers/__init__.py
--rw-r--r--  2.0 unx     2941 b- defN 23-Jul-12 09:50 xpag/samplers/jax_sampler.py
--rw-r--r--  2.0 unx     1917 b- defN 23-Jul-12 09:50 xpag/samplers/sampler.py
--rw-r--r--  2.0 unx       71 b- defN 23-Jul-12 09:50 xpag/setters/__init__.py
--rw-r--r--  2.0 unx     3734 b- defN 23-Jul-12 09:50 xpag/setters/setter.py
--rw-r--r--  2.0 unx      438 b- defN 23-Jul-12 09:50 xpag/tools/__init__.py
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-12 09:50 xpag/tools/eval.py
--rw-r--r--  2.0 unx     7603 b- defN 23-Jul-12 09:50 xpag/tools/learn.py
--rw-r--r--  2.0 unx     3225 b- defN 23-Jul-12 09:50 xpag/tools/logging.py
--rw-r--r--  2.0 unx     4708 b- defN 23-Jul-12 09:50 xpag/tools/replay.py
--rw-r--r--  2.0 unx      899 b- defN 23-Jul-12 09:50 xpag/tools/timing.py
--rw-r--r--  2.0 unx     6933 b- defN 23-Jul-12 09:50 xpag/tools/utils.py
--rw-r--r--  2.0 unx      179 b- defN 23-Jul-12 09:50 xpag/wrappers/__init__.py
--rw-r--r--  2.0 unx     8189 b- defN 23-Jul-12 09:50 xpag/wrappers/brax_vec_env.py
--rw-r--r--  2.0 unx     6099 b- defN 23-Jul-12 09:50 xpag/wrappers/goalenv_wrapper.py
--rw-r--r--  2.0 unx    10148 b- defN 23-Jul-12 09:50 xpag/wrappers/gym_vec_env.py
--rw-r--r--  2.0 unx      936 b- defN 23-Jul-12 09:50 xpag/wrappers/reset_done.py
--rw-r--r--  2.0 unx     1517 b- defN 23-Jul-12 09:50 xpag-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    15098 b- defN 23-Jul-12 09:50 xpag-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 09:50 xpag-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-12 09:50 xpag-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3184 b- defN 23-Jul-12 09:50 xpag-0.2.0.dist-info/RECORD
-40 files, 183267 bytes uncompressed, 50004 bytes compressed:  72.7%
+Zip file size: 79287 bytes, number of entries: 67
+-rw-r--r--  2.0 unx      211 b- defN 23-Jul-29 14:59 xpag/__init__.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-29 14:59 xpag/agents/__init__.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Jul-29 14:59 xpag/agents/agent.py
+-rw-r--r--  2.0 unx     1705 b- defN 23-Jul-29 14:59 xpag/agents/all_agents.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/sac/__init__.py
+-rw-r--r--  2.0 unx     5610 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/sac/sac.py
+-rw-r--r--  2.0 unx    18793 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/sac/sac_from_jaxrl.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/sdqn/__init__.py
+-rw-r--r--  2.0 unx    22301 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/sdqn/sdqn.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/td3/__init__.py
+-rw-r--r--  2.0 unx    15292 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/td3/td3.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/tqc/__init__.py
+-rw-r--r--  2.0 unx    13044 b- defN 23-Jul-29 14:59 xpag/agents/flax_agents/tqc/tqc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/__init__.py
+-rw-r--r--  2.0 unx     4739 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/rljax_interface.py
+-rw-r--r--  2.0 unx      290 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/__init__.py
+-rw-r--r--  2.0 unx     7913 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/ddpg.py
+-rw-r--r--  2.0 unx    10275 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/sac.py
+-rw-r--r--  2.0 unx     6579 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/sac_discor.py
+-rw-r--r--  2.0 unx     2289 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/td3.py
+-rw-r--r--  2.0 unx     4597 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/tqc.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/base_class/__init__.py
+-rw-r--r--  2.0 unx     5200 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/base_class/actor_critic.py
+-rw-r--r--  2.0 unx     3459 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/base_class/base_algorithm.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/misc/__init__.py
+-rw-r--r--  2.0 unx     4297 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/algorithm/misc/discor_mixin.py
+-rw-r--r--  2.0 unx      342 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/network/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/network/actor.py
+-rw-r--r--  2.0 unx     1213 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/network/base.py
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/network/critic.py
+-rw-r--r--  2.0 unx     1357 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/network/initializer.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/__init__.py
+-rw-r--r--  2.0 unx     2631 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/distribution.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/input.py
+-rw-r--r--  2.0 unx      826 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/loss.py
+-rw-r--r--  2.0 unx     1914 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/optim.py
+-rw-r--r--  2.0 unx     1330 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/preprocess.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-29 14:59 xpag/agents/rljax_agents/util/saving.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jul-29 14:59 xpag/buffers/__init__.py
+-rw-r--r--  2.0 unx    11221 b- defN 23-Jul-29 14:59 xpag/buffers/buffer.py
+-rw-r--r--  2.0 unx     5236 b- defN 23-Jul-29 14:59 xpag/buffers/jax_buffer.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-29 14:59 xpag/plotting/__init__.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jul-29 14:59 xpag/plotting/plotting.py
+-rw-r--r--  2.0 unx     2841 b- defN 23-Jul-29 14:59 xpag/samplers/HER.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-29 14:59 xpag/samplers/__init__.py
+-rw-r--r--  2.0 unx     2941 b- defN 23-Jul-29 14:59 xpag/samplers/jax_sampler.py
+-rw-r--r--  2.0 unx     1917 b- defN 23-Jul-29 14:59 xpag/samplers/sampler.py
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-29 14:59 xpag/setters/__init__.py
+-rw-r--r--  2.0 unx     3734 b- defN 23-Jul-29 14:59 xpag/setters/setter.py
+-rw-r--r--  2.0 unx      438 b- defN 23-Jul-29 14:59 xpag/tools/__init__.py
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-29 14:59 xpag/tools/eval.py
+-rw-r--r--  2.0 unx     7741 b- defN 23-Jul-29 14:59 xpag/tools/learn.py
+-rw-r--r--  2.0 unx     3225 b- defN 23-Jul-29 14:59 xpag/tools/logging.py
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jul-29 14:59 xpag/tools/replay.py
+-rw-r--r--  2.0 unx      899 b- defN 23-Jul-29 14:59 xpag/tools/timing.py
+-rw-r--r--  2.0 unx     6933 b- defN 23-Jul-29 14:59 xpag/tools/utils.py
+-rw-r--r--  2.0 unx      179 b- defN 23-Jul-29 14:59 xpag/wrappers/__init__.py
+-rw-r--r--  2.0 unx     8189 b- defN 23-Jul-29 14:59 xpag/wrappers/brax_vec_env.py
+-rw-r--r--  2.0 unx     6099 b- defN 23-Jul-29 14:59 xpag/wrappers/goalenv_wrapper.py
+-rw-r--r--  2.0 unx    10148 b- defN 23-Jul-29 14:59 xpag/wrappers/gym_vec_env.py
+-rw-r--r--  2.0 unx      936 b- defN 23-Jul-29 14:59 xpag/wrappers/reset_done.py
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jul-29 14:59 xpag-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15747 b- defN 23-Jul-29 14:59 xpag-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 14:59 xpag-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-29 14:59 xpag-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5997 b- defN 23-Jul-29 14:59 xpag-0.2.1.dist-info/RECORD
+67 files, 254274 bytes uncompressed, 69637 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -3,39 +3,120 @@
 
 Filename: xpag/agents/__init__.py
 Comment: 
 
 Filename: xpag/agents/agent.py
 Comment: 
 
-Filename: xpag/agents/sac/__init__.py
+Filename: xpag/agents/all_agents.py
 Comment: 
 
-Filename: xpag/agents/sac/sac.py
+Filename: xpag/agents/flax_agents/__init__.py
 Comment: 
 
-Filename: xpag/agents/sac/sac_from_jaxrl.py
+Filename: xpag/agents/flax_agents/sac/__init__.py
 Comment: 
 
-Filename: xpag/agents/sdqn/__init__.py
+Filename: xpag/agents/flax_agents/sac/sac.py
 Comment: 
 
-Filename: xpag/agents/sdqn/sdqn.py
+Filename: xpag/agents/flax_agents/sac/sac_from_jaxrl.py
 Comment: 
 
-Filename: xpag/agents/td3/__init__.py
+Filename: xpag/agents/flax_agents/sdqn/__init__.py
 Comment: 
 
-Filename: xpag/agents/td3/td3.py
+Filename: xpag/agents/flax_agents/sdqn/sdqn.py
 Comment: 
 
-Filename: xpag/agents/tqc/__init__.py
+Filename: xpag/agents/flax_agents/td3/__init__.py
 Comment: 
 
-Filename: xpag/agents/tqc/tqc.py
+Filename: xpag/agents/flax_agents/td3/td3.py
+Comment: 
+
+Filename: xpag/agents/flax_agents/tqc/__init__.py
+Comment: 
+
+Filename: xpag/agents/flax_agents/tqc/tqc.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/rljax_interface.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/ddpg.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/sac.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/sac_discor.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/td3.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/tqc.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/base_class/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/base_class/actor_critic.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/base_class/base_algorithm.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/misc/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/algorithm/misc/discor_mixin.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/network/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/network/actor.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/network/base.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/network/critic.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/network/initializer.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/__init__.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/distribution.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/input.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/loss.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/optim.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/preprocess.py
+Comment: 
+
+Filename: xpag/agents/rljax_agents/util/saving.py
 Comment: 
 
 Filename: xpag/buffers/__init__.py
 Comment: 
 
 Filename: xpag/buffers/buffer.py
 Comment: 
@@ -99,23 +180,23 @@
 
 Filename: xpag/wrappers/gym_vec_env.py
 Comment: 
 
 Filename: xpag/wrappers/reset_done.py
 Comment: 
 
-Filename: xpag-0.2.0.dist-info/LICENSE
+Filename: xpag-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: xpag-0.2.0.dist-info/METADATA
+Filename: xpag-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: xpag-0.2.0.dist-info/WHEEL
+Filename: xpag-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: xpag-0.2.0.dist-info/top_level.txt
+Filename: xpag-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xpag-0.2.0.dist-info/RECORD
+Filename: xpag-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xpag/__init__.py

```diff
@@ -2,8 +2,8 @@
 from xpag import plotting
 from xpag import wrappers
 from xpag import buffers
 from xpag import samplers
 from xpag import agents
 from xpag import setters
 
-__version__ = "0.2.0"  # -version-
+__version__ = "0.2.1"  # -version-
```

## xpag/agents/__init__.py

```diff
@@ -1,7 +1,2 @@
-from xpag.agents.agent import (
-    Agent,
-)
-from xpag.agents.sac.sac import SAC
-from xpag.agents.td3.td3 import TD3
-from xpag.agents.tqc.tqc import TQC
-from xpag.agents.sdqn.sdqn import SDQN, SDQNSetter
+from xpag.agents.agent import Agent
+from xpag.agents.all_agents import SAC, TD3, TQC, SDQN, SDQNSetter
```

## xpag/tools/learn.py

```diff
@@ -56,18 +56,20 @@
         start_training_after_x_steps (int): the number of inital steps with random
             actions before starting using and training the agent.
         max_steps (int): the maximum number of steps in the environment before stopping
             the learning (remark: if there n rollouts in parallel, one call to
             env.step() counts as n steps).
         evaluate_every_x_steps (int): the number of steps between two evaluations of the
             agent (remark: if there n rollouts in parallel, one call to
-            env.step() counts as n steps).
+            env.step() counts as n steps). With the default value, np.inf, there is no
+            evaluation.
         save_agent_every_x_steps (int): it defines how often the agent is saved to
             the disk (remark: if there n rollouts in parallel, one call to
-            env.step() counts as n steps).
+            env.step() counts as n steps). With the default value, np.inf, the agent
+            is never saved.
         save_dir (str): the directory in which the config, agent, plots, evaluation
             episodes and logs are saved.
         save_episode (bool): if True, the evaluation episodes are saved.
         plot_projection (Callable): a function with 2D outputs from either the
             observation space or the achieved/desired goal space (in the case of a
             goal-based environment). It is used to plot evaluation episodes.
         custom_eval_function (Callable): a custom function used to replace the
```

## Comparing `xpag/agents/sac/sac.py` & `xpag/agents/flax_agents/sac/sac.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022-2023, CNRS.
 #
 # Licensed under the BSD 3-Clause License.
 
 import os
 from xpag.agents.agent import Agent
-from xpag.agents.sac.sac_from_jaxrl import Batch, SACLearner
+from xpag.agents.flax_agents.sac.sac_from_jaxrl import Batch, SACLearner
 from xpag.tools.utils import squeeze
 import functools
 from typing import Callable, Any, Tuple
 import flax
 import jax
 import jax.numpy as jnp
 import numpy as np
@@ -22,15 +22,15 @@
     actions: jnp.ndarray,
 ) -> Tuple[jnp.ndarray]:
     return jnp.minimum(
         *critic_apply_fn({"params": critic_params}, observations, actions)
     )
 
 
-class SAC(Agent):
+class FlaxSAC(Agent):
     """
     Interface to the SAC agent from JAXRL (https://github.com/ikostrikov/jaxrl)
 
     Methods:
 
     - :meth:`value` - computes Q-values given a batch of observations and a batch of
         actions.
@@ -62,15 +62,15 @@
         "target_entropy": the target entropy; if None, it will be set
         to -action_dim / 2
         "target_update_period" (default=1): defines how often a soft update of the
         target critic is performed
         "tau" (default=5e-2): the soft update coefficient
         "policy_final_fc_init_scale" (default=1.): scale parameter for the
         initialization of the final fully connected layers of the actor network
-    - :attr:`sac` - the SACLearner object that contains and trains the agent and critic
+    - :attr:`sac` - the SACLearner object that contains and trains the actor and critic
         networks
     """
 
     def __init__(self, observation_dim, action_dim, params=None):
 
         self._config_string = str(list(locals().items())[1:])
         super().__init__("SAC", observation_dim, action_dim, params)
```

## Comparing `xpag/agents/sac/sac_from_jaxrl.py` & `xpag/agents/flax_agents/sac/sac_from_jaxrl.py`

 * *Files identical despite different names*

## Comparing `xpag/agents/sdqn/sdqn.py` & `xpag/agents/flax_agents/sdqn/sdqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     critic_low_optimizer_state: optax.OptState
     critic_low_params: Params
     target_critic_low_params: Params
     key: PRNGKey
     steps: jnp.ndarray
 
 
-class SDQN(Agent):
+class FlaxSDQN(Agent):
     def __init__(
         self,
         observation_dim,
         action_dim,
         params=None,
     ):
         """
@@ -560,16 +560,16 @@
             rewards,
             new_observations,
             mask,
         )
         return metrics
 
 
-class SDQNSetter(Setter):
-    def __init__(self, sdqn_agent: SDQN):
+class FlaxSDQNSetter(Setter):
+    def __init__(self, sdqn_agent: FlaxSDQN):
         super().__init__("SDQNSetter")
         self.agent = sdqn_agent
 
     def reset(self, env, observation, info, eval_mode=False):
         return observation, info
 
     def reset_done(self, env, observation, info, done, eval_mode=False):
```

## Comparing `xpag/agents/td3/td3.py` & `xpag/agents/flax_agents/td3/td3.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     q_optimizer_state: optax.OptState
     q_params: Params
     target_q_params: Params
     key: PRNGKey
     steps: jnp.ndarray
 
 
-class TD3(Agent):
+class FlaxTD3(Agent):
     def __init__(
         self,
         observation_dim,
         action_dim,
         params=None,
     ):
         """
```

## Comparing `xpag/agents/tqc/tqc.py` & `xpag/agents/flax_agents/tqc/tqc.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import os
 from xpag.agents.agent import Agent
-from xpag.agents.sac.sac_from_jaxrl import (
+from xpag.agents.flax_agents.sac.sac_from_jaxrl import (
     PRNGKey,
     InfoDict,
     Params,
     Batch,
     SACLearner,
     Model,
     MLP,
@@ -331,15 +331,15 @@
         self.critic = new_critic
         self.target_critic = new_target_critic
         self.temp = new_temp
 
         return info
 
 
-class TQC(Agent):
+class FlaxTQC(Agent):
     def __init__(self, observation_dim, action_dim, params=None):
         """
         Interface to TQC agent
         """
 
         self._config_string = str(list(locals().items())[1:])
         super().__init__("TQC", observation_dim, action_dim, params)
```

## Comparing `xpag-0.2.0.dist-info/LICENSE` & `xpag-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xpag-0.2.0.dist-info/METADATA` & `xpag-0.2.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpag
-Version: 0.2.0
+Version: 0.2.1
 Summary: xpag: Exploring Agents
 Home-page: https://github.com/perrin-isir/xpag
 Author: Nicolas Perrin-Gilbert
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil (>=5.8.0)
@@ -13,21 +13,22 @@
 Requires-Dist: joblib (>=1.1.0)
 Requires-Dist: gymnasium (>=0.28.1)
 Requires-Dist: Pillow (>=9.0.1)
 Requires-Dist: ipywidgets (>=7.6.5)
 Requires-Dist: jax (>=0.4.8)
 Requires-Dist: optax (>=0.1.2)
 Requires-Dist: flax (>=0.6.3)
+Requires-Dist: haiku (>=0.0.10)
 Requires-Dist: brax (>=0.9.1)
 Requires-Dist: tensorflow-probability (>=0.15.0)
 Requires-Dist: mediapy (>=1.1.4)
 
 # ![alt text](https://raw.githubusercontent.com/perrin-isir/xpag/main/logo.png "xpag logo")
 
-![version](https://img.shields.io/badge/version-0.2.0-blue)
+![version](https://img.shields.io/badge/version-0.2.1-blue)
 [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/perrin-isir/xpag/docs.yml?branch=main&label=docs)](https://perrin-isir.github.io/xpag/)
 [![PyPI version](https://img.shields.io/pypi/v/xpag)](https://pypi.org/project/xpag/)
 
 
 *xpag* ("e**xp**loring **ag**ents") is a modular reinforcement learning library with JAX agents, currently in beta version.
 
@@ -107,15 +108,15 @@
 
 The *xpag-tutorials* repository contains a list of tutorials (colab notebooks) for *xpag*:  
 [https://github.com/perrin-isir/xpag-tutorials](https://github.com/perrin-isir/xpag-tutorials)
 
 
 -----
 ## Short documentation
-<details><summary><B><I>xpag</I>: a platform for goal-conditioned RL</B></summary>
+<details><summary><B><I>xpag</I>: a platform for RL, goal-conditioned RL, and more.</B></summary>
 
 *xpag* allows standard reinforcement learning, but it has been designed with
 goal-conditioned reinforcement learning (GCRL) in mind (check out the [train_gmazes.ipynb](https://colab.research.google.com/github/perrin-isir/xpag-tutorials/blob/main/train_gmazes.ipynb)
 tutorial for a simple example of GCRL). 
 
 In GCRL, agents have a goal, which is part of the input they take, and the reward mainly depends on 
 the degree of achievement of that goal. Beyond the usual modules in 
@@ -256,15 +257,16 @@
 
   Other people who contributed to *xpag*:
   - Olivier Serris (ISIR)
   - Alexandre Chenu (ISIR)
   - Stéphane Caron (Inria)
   - Fabian Schramm (Inria)
 
-* The [SAC agent](https://github.com/perrin-isir/xpag/blob/main/xpag/agents/sac) is based on the implementation of SAC in [JAXRL](https://github.com/ikostrikov/jaxrl), and some elements of the [TQC agent](https://github.com/perrin-isir/xpag/blob/main/xpag/agents/tqc) come from the implementation of TQC in [RLJAX](https://github.com/ku2482/rljax).
+* There is an interface to agents from the [RLJAX](https://github.com/ku2482/rljax) library (see [rljax_interface.py](https://github.com/perrin-isir/xpag/blob/main/xpag/agents/rljax_agents/rljax_interface.py)). This provides [haiku](https://github.com/deepmind/dm-haiku) versions of [DDPG](https://arxiv.org/abs/1509.02971), [TD3](https://arxiv.org/abs/1802.09477), [TQC](https://arxiv.org/abs/2005.04269), [SAC](https://arxiv.org/abs/1812.05905) and SAC with [DisCor](https://arxiv.org/abs/2003.07305).
+* The [flax](https://github.com/google/flax) version of the [SAC agent](https://github.com/perrin-isir/xpag/blob/main/xpag/agents/flax_agents/sac) is based on the implementation of SAC in [JAXRL](https://github.com/ikostrikov/jaxrl), and some elements of the flax version of the [TQC agent](https://github.com/perrin-isir/xpag/blob/main/xpag/agents/flax_agents/tqc) come from the implementation of TQC in [RLJAX](https://github.com/ku2482/rljax).
 
 -----
 ## Citing the project
 To cite this repository in publications:
 
 ```bibtex
 @misc{xpag,
```

