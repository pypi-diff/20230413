# Comparing `tmp/sbx-rl-0.6.0.tar.gz` & `tmp/sbx-rl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbx-rl-0.6.0.tar", last modified: Sat Mar 18 14:55:29 2023, max compression
+gzip compressed data, was "sbx-rl-0.7.0.tar", last modified: Thu Apr 13 15:45:46 2023, max compression
```

## Comparing `sbx-rl-0.6.0.tar` & `sbx-rl-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.184344 sbx-rl-0.6.0/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2022-09-29 08:05:01.000000 sbx-rl-0.6.0/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2022-09-29 07:49:26.000000 sbx-rl-0.6.0/NOTICE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1586 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3247 2022-12-12 15:58:04.000000 sbx-rl-0.6.0/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1646 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.176344 sbx-rl-0.6.0/sbx/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      387 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.176344 sbx-rl-0.6.0/sbx/common/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 08:03:49.000000 sbx-rl-0.6.0/sbx/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      955 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3865 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7156 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4004 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      405 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/common/type_aliases.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.176344 sbx-rl-0.6.0/sbx/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10943 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2919 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/sbx/droq/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/droq/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2545 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/droq/droq.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/sbx/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7153 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14271 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 07:49:33.000000 sbx-rl-0.6.0/sbx/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/sbx/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7497 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13741 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/sbx/tqc/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.6.0/sbx/tqc/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7642 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/tqc/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17073 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/tqc/tqc.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/sbx/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/sbx_rl.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1586 2023-03-18 14:55:29.000000 sbx-rl-0.6.0/sbx_rl.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      688 2023-03-18 14:55:29.000000 sbx-rl-0.6.0/sbx_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-03-18 14:55:29.000000 sbx-rl-0.6.0/sbx_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      167 2023-03-18 14:55:29.000000 sbx-rl-0.6.0/sbx_rl.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        4 2023-03-18 14:55:29.000000 sbx-rl-0.6.0/sbx_rl.egg-info/top_level.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-03-18 14:55:29.184344 sbx-rl-0.6.0/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2757 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-03-18 14:55:29.180344 sbx-rl-0.6.0/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2345 2023-03-18 14:54:58.000000 sbx-rl-0.6.0/tests/test_run.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2022-09-29 08:05:01.000000 sbx-rl-0.7.0/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2022-09-29 07:49:26.000000 sbx-rl-0.7.0/NOTICE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1586 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3247 2022-12-12 15:58:04.000000 sbx-rl-0.7.0/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1151 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.980846 sbx-rl-0.7.0/sbx/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      387 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.980846 sbx-rl-0.7.0/sbx/common/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 08:03:49.000000 sbx-rl-0.7.0/sbx/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      955 2023-03-18 14:54:58.000000 sbx-rl-0.7.0/sbx/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4745 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7688 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4583 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      405 2023-03-18 14:54:58.000000 sbx-rl-0.7.0/sbx/common/type_aliases.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.980846 sbx-rl-0.7.0/sbx/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10833 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3036 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.980846 sbx-rl-0.7.0/sbx/droq/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/droq/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2840 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/droq/droq.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/sbx/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7244 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14478 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 07:49:33.000000 sbx-rl-0.7.0/sbx/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/sbx/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7758 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14800 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/sbx/tqc/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.7.0/sbx/tqc/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7897 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/tqc/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18102 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/tqc/tqc.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/sbx/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/sbx_rl.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1586 2023-04-13 15:45:46.000000 sbx-rl-0.7.0/sbx_rl.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      688 2023-04-13 15:45:46.000000 sbx-rl-0.7.0/sbx_rl.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 15:45:46.000000 sbx-rl-0.7.0/sbx_rl.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      167 2023-04-13 15:45:46.000000 sbx-rl-0.7.0/sbx_rl.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        4 2023-04-13 15:45:46.000000 sbx-rl-0.7.0/sbx_rl.egg-info/top_level.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2757 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 15:45:46.984846 sbx-rl-0.7.0/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2847 2023-04-13 15:45:25.000000 sbx-rl-0.7.0/tests/test_run.py
```

### Comparing `sbx-rl-0.6.0/LICENSE` & `sbx-rl-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.6.0/NOTICE` & `sbx-rl-0.7.0/NOTICE`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.6.0/PKG-INFO` & `sbx-rl-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbx-rl
-Version: 0.6.0
+Version: 0.7.0
 Summary: Jax version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/araffin/sbx
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbx-rl-0.6.0/README.md` & `sbx-rl-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.6.0/pyproject.toml` & `sbx-rl-0.7.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -25,37 +25,27 @@
 inputs = ["sbx"]
 disable = []
 
 [tool.mypy]
 ignore_missing_imports = true
 follow_imports = "silent"
 show_error_codes = true
-exclude = """(?x)(
-    sbx/common/on_policy_algorithm.py$
-    | sbx/common/off_policy_algorithm.py$
-    | sbx/ppo/ppo.py$
-    | sbx/dqn/dqn.py$
-    | sbx/common/policies.py$
-  )"""
+# exclude = """(?x)(
+#     sbx/common/policies.py$
+#   )"""
 
 [tool.pytest.ini_options]
 # Deterministic ordering for tests; useful for pytest-xdist.
 env = [
 	"PYTHONHASHSEED=0"
 ]
 
 filterwarnings = [
     # Tensorboard warnings
     "ignore::DeprecationWarning:tensorboard",
-    # Gym warnings
-    "ignore:Parameters to load are deprecated.:DeprecationWarning",
-    "ignore:the imp module is deprecated in favour of importlib:PendingDeprecationWarning",
-    "ignore::UserWarning:gym",
-		"ignore:SelectableGroups dict interface is deprecated.:DeprecationWarning",
-		"ignore:`np.bool` is a deprecated alias for the builtin `bool`:DeprecationWarning",
 ]
 markers = [
     "expensive: marks tests as expensive (deselect with '-m \"not expensive\"')"
 ]
 
 [tool.coverage.run]
 disable_warnings = ["couldnt-parse"]
```

### Comparing `sbx-rl-0.6.0/sbx/common/distributions.py` & `sbx-rl-0.7.0/sbx/common/distributions.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.6.0/sbx/common/off_policy_algorithm.py` & `sbx-rl-0.7.0/sbx/common/off_policy_algorithm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-import gym
 import jax
 import numpy as np
-from stable_baselines3.common.buffers import ReplayBuffer
+from gymnasium import spaces
+from stable_baselines3 import HerReplayBuffer
+from stable_baselines3.common.buffers import DictReplayBuffer, ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, Schedule
 
 
 class OffPolicyAlgorithmJax(OffPolicyAlgorithm):
@@ -35,27 +36,29 @@
         support_multi_env: bool = False,
         monitor_wrapper: bool = True,
         seed: Optional[int] = None,
         use_sde: bool = False,
         sde_sample_freq: int = -1,
         use_sde_at_warmup: bool = False,
         sde_support: bool = True,
-        supported_action_spaces: Optional[Tuple[gym.spaces.Space, ...]] = None,
+        supported_action_spaces: Optional[Tuple[Type[spaces.Space], ...]] = None,
     ):
         super().__init__(
             policy=policy,
             env=env,
             learning_rate=learning_rate,
             buffer_size=buffer_size,
             learning_starts=learning_starts,
             batch_size=batch_size,
             tau=tau,
             gamma=gamma,
             train_freq=train_freq,
             gradient_steps=gradient_steps,
+            replay_buffer_class=replay_buffer_class,
+            replay_buffer_kwargs=replay_buffer_kwargs,
             action_noise=action_noise,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             use_sde_at_warmup=use_sde_at_warmup,
             policy_kwargs=policy_kwargs,
             tensorboard_log=tensorboard_log,
             verbose=verbose,
@@ -73,32 +76,43 @@
         return [], []
 
     def _excluded_save_params(self) -> List[str]:
         excluded = super()._excluded_save_params()
         excluded.remove("policy")
         return excluded
 
-    def set_random_seed(self, seed: int) -> None:
+    def set_random_seed(self, seed: Optional[int]) -> None:  # type: ignore[override]
         super().set_random_seed(seed)
         if seed is None:
             # Sample random seed
             seed = np.random.randint(2**14)
         self.key = jax.random.PRNGKey(seed)
 
     def _setup_model(self) -> None:
+        if self.replay_buffer_class is None:  # type: ignore[has-type]
+            if isinstance(self.observation_space, spaces.Dict):
+                self.replay_buffer_class = DictReplayBuffer
+            else:
+                self.replay_buffer_class = ReplayBuffer
+
         self._setup_lr_schedule()
         # By default qf_learning_rate = pi_learning_rate
         self.qf_learning_rate = self.qf_learning_rate or self.lr_schedule(1)
         self.set_random_seed(self.seed)
+        # Make a local copy as we should not pickle
+        # the environment when using HerReplayBuffer
+        replay_buffer_kwargs = self.replay_buffer_kwargs.copy()
+        if issubclass(self.replay_buffer_class, HerReplayBuffer):  # type: ignore[arg-type]
+            assert self.env is not None, "You must pass an environment when using `HerReplayBuffer`"
+            replay_buffer_kwargs["env"] = self.env
 
-        self.replay_buffer_class = ReplayBuffer
-        self.replay_buffer = self.replay_buffer_class(
+        self.replay_buffer = self.replay_buffer_class(  # type: ignore[misc]
             self.buffer_size,
             self.observation_space,
             self.action_space,
             device="cpu",  # force cpu device to easy torch -> numpy conversion
             n_envs=self.n_envs,
             optimize_memory_usage=self.optimize_memory_usage,
-            **self.replay_buffer_kwargs,
+            **replay_buffer_kwargs,
         )
         # Convert train freq parameter to TrainFreq object
         self._convert_train_freq()
```

### Comparing `sbx-rl-0.6.0/sbx/common/on_policy_algorithm.py` & `sbx-rl-0.7.0/sbx/common/on_policy_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
-import gym
+import gymnasium as gym
 import jax
 import numpy as np
 import torch as th
+from gymnasium import spaces
 from stable_baselines3.common.buffers import RolloutBuffer
 from stable_baselines3.common.callbacks import BaseCallback
 from stable_baselines3.common.on_policy_algorithm import OnPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, Schedule
 from stable_baselines3.common.vec_env import VecEnv
 
+from sbx.ppo.policies import Actor, Critic, PPOPolicy
+
 OnPolicyAlgorithmSelf = TypeVar("OnPolicyAlgorithmSelf", bound="OnPolicyAlgorithmJax")
 
 
 class OnPolicyAlgorithmJax(OnPolicyAlgorithm):
+    policy: PPOPolicy  # type: ignore[assignment]
+    actor: Actor
+    vf: Critic
+
     def __init__(
         self,
         policy: Union[str, Type[BasePolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule],
         n_steps: int,
         gamma: float,
@@ -31,18 +38,18 @@
         tensorboard_log: Optional[str] = None,
         monitor_wrapper: bool = True,
         policy_kwargs: Optional[Dict[str, Any]] = None,
         verbose: int = 0,
         seed: Optional[int] = None,
         device: str = "auto",
         _init_setup_model: bool = True,
-        supported_action_spaces: Optional[Tuple[gym.spaces.Space, ...]] = None,
+        supported_action_spaces: Optional[Tuple[Type[spaces.Space], ...]] = None,
     ):
         super().__init__(
-            policy=policy,
+            policy=policy,  # type: ignore[arg-type]
             env=env,
             learning_rate=learning_rate,
             n_steps=n_steps,
             gamma=gamma,
             gae_lambda=gae_lambda,
             ent_coef=ent_coef,
             vf_coef=vf_coef,
@@ -64,15 +71,15 @@
         return [], []
 
     def _excluded_save_params(self) -> List[str]:
         excluded = super()._excluded_save_params()
         excluded.remove("policy")
         return excluded
 
-    def set_random_seed(self, seed: int) -> None:
+    def set_random_seed(self, seed: Optional[int]) -> None:  # type: ignore[override]
         super().set_random_seed(seed)
         if seed is None:
             # Sample random seed
             seed = np.random.randint(2**14)
         self.key = jax.random.PRNGKey(seed)
 
     def _setup_model(self) -> None:
@@ -163,29 +170,39 @@
             for idx, done in enumerate(dones):
                 if (
                     done
                     and infos[idx].get("terminal_observation") is not None
                     and infos[idx].get("TimeLimit.truncated", False)
                 ):
                     terminal_obs = self.policy.prepare_obs(infos[idx]["terminal_observation"])[0]
-                    terminal_value = np.array(self.vf.apply(self.policy.vf_state.params, terminal_obs).flatten())
+                    terminal_value = np.array(
+                        self.vf.apply(  # type: ignore[union-attr]
+                            self.policy.vf_state.params,
+                            terminal_obs,
+                        ).flatten()
+                    )
 
                     rewards[idx] += self.gamma * terminal_value
 
             rollout_buffer.add(
-                self._last_obs,  # type: ignore[has-type]
+                self._last_obs,  # type: ignore
                 actions,
                 rewards,
-                self._last_episode_starts,  # type: ignore[has-type]
+                self._last_episode_starts,  # type: ignore
                 th.as_tensor(values),
                 th.as_tensor(log_probs),
             )
-            self._last_obs = new_obs
+            self._last_obs = new_obs  # type: ignore[assignment]
             self._last_episode_starts = dones
 
-        values = np.array(self.vf.apply(self.policy.vf_state.params, self.policy.prepare_obs(new_obs)[0]).flatten())
+        values = np.array(
+            self.vf.apply(  # type: ignore[union-attr]
+                self.policy.vf_state.params,
+                self.policy.prepare_obs(new_obs)[0],  # type: ignore[arg-type]
+            ).flatten()
+        )
 
         rollout_buffer.compute_returns_and_advantage(last_values=th.as_tensor(values), dones=dones)
 
         callback.on_rollout_end()
 
         return True
```

### Comparing `sbx-rl-0.6.0/sbx/common/policies.py` & `sbx-rl-0.7.0/sbx/common/policies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import copy
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union, no_type_check
 
-import gym
 import jax
 import numpy as np
+from gymnasium import spaces
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.preprocessing import is_image_space, maybe_transpose
 from stable_baselines3.common.utils import is_vectorized_observation
 
 
 class BaseJaxPolicy(BasePolicy):
     def __init__(self, *args, **kwargs):
@@ -24,14 +24,15 @@
         return action
 
     @staticmethod
     @jax.jit
     def select_action(actor_state, obervations):
         return actor_state.apply_fn(actor_state.params, obervations).mode()
 
+    @no_type_check
     def predict(
         self,
         observation: Union[np.ndarray, Dict[str, np.ndarray]],
         state: Optional[Tuple[np.ndarray, ...]] = None,
         episode_start: Optional[np.ndarray] = None,
         deterministic: bool = False,
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
@@ -40,60 +41,69 @@
         observation, vectorized_env = self.prepare_obs(observation)
 
         actions = self._predict(observation, deterministic=deterministic)
 
         # Convert to numpy, and reshape to the original action shape
         actions = np.array(actions).reshape((-1, *self.action_space.shape))
 
-        if isinstance(self.action_space, gym.spaces.Box):
+        if isinstance(self.action_space, spaces.Box):
             if self.squash_output:
                 # Clip due to numerical instability
                 actions = np.clip(actions, -1, 1)
                 # Rescale to proper domain when using squashing
                 actions = self.unscale_action(actions)
             else:
                 # Actions could be on arbitrary scale, so clip the actions to avoid
                 # out of bound error (e.g. if sampling from a Gaussian distribution)
                 actions = np.clip(actions, self.action_space.low, self.action_space.high)
 
         # Remove batch dimension if needed
         if not vectorized_env:
-            actions = actions.squeeze(axis=0)
+            actions = actions.squeeze(axis=0)  # type: ignore[call-overload]
 
         return actions, state
 
     def prepare_obs(self, observation: Union[np.ndarray, Dict[str, np.ndarray]]) -> Tuple[np.ndarray, bool]:
         vectorized_env = False
         if isinstance(observation, dict):
-            raise NotImplementedError()
-            # # need to copy the dict as the dict in VecFrameStack will become a torch tensor
+            assert isinstance(self.observation_space, spaces.Dict)
+            # Minimal dict support: flatten
+            keys = list(self.observation_space.keys())
+            vectorized_env = is_vectorized_observation(observation[keys[0]], self.observation_space[keys[0]])
+
+            # Add batch dim and concatenate
+            observation = np.concatenate(
+                [observation[key].reshape(-1, *self.observation_space[key].shape) for key in keys],
+                axis=1,
+            )
+            # need to copy the dict as the dict in VecFrameStack will become a torch tensor
             # observation = copy.deepcopy(observation)
             # for key, obs in observation.items():
             #     obs_space = self.observation_space.spaces[key]
             #     if is_image_space(obs_space):
             #         obs_ = maybe_transpose(obs, obs_space)
             #     else:
             #         obs_ = np.array(obs)
             #     vectorized_env = vectorized_env or is_vectorized_observation(obs_, obs_space)
             #     # Add batch dimension if needed
-            #     observation[key] = obs_.reshape((-1,) + self.observation_space[key].shape)
+            #     observation[key] = obs_.reshape((-1, *self.observation_space[key].shape))
 
         elif is_image_space(self.observation_space):
             # Handle the different cases for images
             # as PyTorch use channel first format
             observation = maybe_transpose(observation, self.observation_space)
 
         else:
             observation = np.array(observation)
 
-        if not isinstance(observation, dict):
-            # Dict obs need to be handled separately
+        if not isinstance(self.observation_space, spaces.Dict):
+            assert isinstance(observation, np.ndarray)
             vectorized_env = is_vectorized_observation(observation, self.observation_space)
             # Add batch dimension if needed
-            observation = observation.reshape((-1, *self.observation_space.shape))
+            observation = observation.reshape((-1, *self.observation_space.shape))  # type: ignore[misc]
 
         assert isinstance(observation, np.ndarray)
         return observation, vectorized_env
 
     def set_training_mode(self, mode: bool) -> None:
         # self.actor.set_training_mode(mode)
         # self.critic.set_training_mode(mode)
```

### Comparing `sbx-rl-0.6.0/sbx/dqn/dqn.py` & `sbx-rl-0.7.0/sbx/dqn/dqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import warnings
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
-import gym
+import gymnasium as gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
-from stable_baselines3.common.preprocessing import maybe_transpose
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
-from stable_baselines3.common.utils import get_linear_fn, is_vectorized_observation
+from stable_baselines3.common.utils import get_linear_fn
 
 from sbx.common.off_policy_algorithm import OffPolicyAlgorithmJax
 from sbx.common.type_aliases import ReplayBufferSamplesNp, RLTrainState
 from sbx.dqn.policies import DQNPolicy
 
 
 class DQN(OffPolicyAlgorithmJax):
     policy_aliases: Dict[str, Type[DQNPolicy]] = {  # type: ignore[assignment]
         "MlpPolicy": DQNPolicy,
     }
     # Linear schedule will be defined in `_setup_model()`
     exploration_schedule: Schedule
+    policy: DQNPolicy
 
     def __init__(
         self,
         policy,
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 1e-4,
         buffer_size: int = 1_000_000,  # 1e6
@@ -58,15 +58,15 @@
             train_freq=train_freq,
             gradient_steps=gradient_steps,
             policy_kwargs=policy_kwargs,
             tensorboard_log=tensorboard_log,
             verbose=verbose,
             seed=seed,
             sde_support=False,
-            supported_action_spaces=(gym.spaces.Discrete),
+            supported_action_spaces=(gym.spaces.Discrete,),
             support_multi_env=True,
         )
 
         self.exploration_initial_eps = exploration_initial_eps
         self.exploration_final_eps = exploration_final_eps
         self.exploration_fraction = exploration_fraction
         self.target_update_interval = target_update_interval
@@ -95,22 +95,24 @@
                     f"update interval ({self.n_envs} > {self.target_update_interval}), "
                     "therefore the target network will be updated after each call to env.step() "
                     f"which corresponds to {self.n_envs} steps."
                 )
 
             self.target_update_interval = max(self.target_update_interval // self.n_envs, 1)
 
-        if self.policy is None:  # type: ignore[has-type]
-            self.policy = self.policy_class(  # pytype:disable=not-instantiable
+        if not hasattr(self, "policy") or self.policy is None:
+            # pytype:disable=not-instantiable
+            self.policy = self.policy_class(  # type: ignore[assignment]
                 self.observation_space,
                 self.action_space,
                 self.lr_schedule,
-                **self.policy_kwargs,  # pytype:disable=not-instantiable
+                **self.policy_kwargs,
             )
-            assert isinstance(self.policy, DQNPolicy)
+            # pytype:enable=not-instantiable
+
             self.key = self.policy.build(self.key, self.lr_schedule)
             self.qf = self.policy.qf
 
     def learn(
         self,
         total_timesteps: int,
         callback: MaybeCallback = None,
@@ -240,15 +242,15 @@
         :param state: The last states (can be None, used in recurrent policies)
         :param episode_start: The last masks (can be None, used in recurrent policies)
         :param deterministic: Whether or not to return deterministic actions.
         :return: the model's action and the next state
             (used in recurrent policies)
         """
         if not deterministic and np.random.rand() < self.exploration_rate:
-            if is_vectorized_observation(maybe_transpose(observation, self.observation_space), self.observation_space):
+            if self.policy.is_vectorized_observation(observation):
                 if isinstance(observation, dict):
                     n_batch = observation[list(observation.keys())[0]].shape[0]
                 else:
                     n_batch = observation.shape[0]
                 action = np.array([self.action_space.sample() for _ in range(n_batch)])
             else:
                 action = np.array(self.action_space.sample())
```

### Comparing `sbx-rl-0.6.0/sbx/dqn/policies.py` & `sbx-rl-0.7.0/sbx/dqn/policies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import flax.linen as nn
-import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
+from gymnasium import spaces
 from stable_baselines3.common.type_aliases import Schedule
 
 from sbx.common.policies import BaseJaxPolicy
 from sbx.common.type_aliases import RLTrainState
 
 
 class QNetwork(nn.Module):
@@ -23,18 +23,20 @@
         x = nn.Dense(self.n_units)(x)
         x = nn.relu(x)
         x = nn.Dense(self.n_actions)(x)
         return x
 
 
 class DQNPolicy(BaseJaxPolicy):
+    action_space: spaces.Discrete  # type: ignore[assignment]
+
     def __init__(
         self,
-        observation_space: gym.spaces.Space,
-        action_space: gym.spaces.Space,
+        observation_space: spaces.Space,
+        action_space: spaces.Discrete,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         features_extractor_class=None,
         features_extractor_kwargs: Optional[Dict[str, Any]] = None,
         normalize_images: bool = True,
         optimizer_class: Callable[..., optax.GradientTransformation] = optax.adam,
         optimizer_kwargs: Optional[Dict[str, Any]] = None,
@@ -50,20 +52,20 @@
 
         if net_arch is not None:
             assert isinstance(net_arch, list)
             self.n_units = net_arch[0]
         else:
             self.n_units = 256
 
-    def build(self, key, lr_schedule: Schedule) -> None:
+    def build(self, key: jax.random.KeyArray, lr_schedule: Schedule) -> jax.random.KeyArray:
         key, qf_key = jax.random.split(key, 2)
 
         obs = jnp.array([self.observation_space.sample()])
 
-        self.qf = QNetwork(n_actions=self.action_space.n, n_units=self.n_units)
+        self.qf = QNetwork(n_actions=int(self.action_space.n), n_units=self.n_units)
 
         self.qf_state = RLTrainState.create(
             apply_fn=self.qf.apply,
             params=self.qf.init({"params": qf_key}, obs),
             target_params=self.qf.init({"params": qf_key}, obs),
             tx=self.optimizer_class(
                 learning_rate=lr_schedule(1),  # type: ignore[call-arg]
```

### Comparing `sbx-rl-0.6.0/sbx/droq/droq.py` & `sbx-rl-0.7.0/sbx/droq/droq.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
+from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.type_aliases import GymEnv, Schedule
 
 from sbx.tqc.policies import TQCPolicy
 from sbx.tqc.tqc import TQC
 
 
@@ -27,14 +28,16 @@
         gradient_steps: int = 2,
         # policy_delay = gradient_steps to follow original implementation
         policy_delay: int = 2,
         top_quantiles_to_drop_per_net: int = 2,
         dropout_rate: float = 0.01,
         layer_norm: bool = True,
         action_noise: Optional[ActionNoise] = None,
+        replay_buffer_class: Optional[Type[ReplayBuffer]] = None,
+        replay_buffer_kwargs: Optional[Dict[str, Any]] = None,
         ent_coef: Union[str, float] = "auto",
         use_sde: bool = False,
         sde_sample_freq: int = -1,
         use_sde_at_warmup: bool = False,
         tensorboard_log: Optional[str] = None,
         policy_kwargs: Optional[Dict[str, Any]] = None,
         verbose: int = 0,
@@ -52,14 +55,16 @@
             batch_size=batch_size,
             tau=tau,
             gamma=gamma,
             train_freq=train_freq,
             gradient_steps=gradient_steps,
             policy_delay=policy_delay,
             action_noise=action_noise,
+            replay_buffer_class=replay_buffer_class,
+            replay_buffer_kwargs=replay_buffer_kwargs,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             use_sde_at_warmup=use_sde_at_warmup,
             top_quantiles_to_drop_per_net=top_quantiles_to_drop_per_net,
             ent_coef=ent_coef,
             policy_kwargs=policy_kwargs,
             tensorboard_log=tensorboard_log,
```

### Comparing `sbx-rl-0.6.0/sbx/ppo/policies.py` & `sbx-rl-0.7.0/sbx/ppo/policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import flax.linen as nn
-import gym
+import gymnasium as gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 import tensorflow_probability
 from flax.linen.initializers import constant
 from flax.training.train_state import TrainState
-from gym import spaces
+from gymnasium import spaces
 from stable_baselines3.common.type_aliases import Schedule
 
 from sbx.common.policies import BaseJaxPolicy
 
 tfp = tensorflow_probability.substrates.jax
 tfd = tfp.distributions
 
@@ -105,41 +105,41 @@
                 self.n_units = net_arch["pi"][0]
         else:
             self.n_units = 64
         self.use_sde = use_sde
 
         self.key = self.noise_key = jax.random.PRNGKey(0)
 
-    def build(self, key, lr_schedule: Schedule, max_grad_norm: float) -> None:
+    def build(self, key: jax.random.KeyArray, lr_schedule: Schedule, max_grad_norm: float) -> jax.random.KeyArray:
         key, actor_key, vf_key = jax.random.split(key, 3)
         # Keep a key for the actor
         key, self.key = jax.random.split(key, 2)
         # Initialize noise
         self.reset_noise()
 
         obs = jnp.array([self.observation_space.sample()])
 
         if isinstance(self.action_space, spaces.Box):
             actor_kwargs = {
-                "action_dim": np.prod(self.action_space.shape),
+                "action_dim": int(np.prod(self.action_space.shape)),
                 "continuous": True,
             }
         elif isinstance(self.action_space, spaces.Discrete):
             actor_kwargs = {
-                "action_dim": self.action_space.n,
+                "action_dim": int(self.action_space.n),
                 "continuous": False,
             }
         else:
             raise NotImplementedError(f"{self.action_space}")
 
         self.actor = Actor(
             n_units=self.n_units,
             log_std_init=self.log_std_init,
             activation_fn=self.activation_fn,
-            **actor_kwargs,
+            **actor_kwargs,  # type: ignore[arg-type]
         )
         # Hack to make gSDE work without modifying internal SB3 code
         self.actor.reset_noise = self.reset_noise
 
         self.actor_state = TrainState.create(
             apply_fn=self.actor.apply,
             params=self.actor.init(actor_key, obs),
```

### Comparing `sbx-rl-0.6.0/sbx/ppo/ppo.py` & `sbx-rl-0.7.0/sbx/ppo/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 from typing import Any, Dict, Optional, Type, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from flax.training.train_state import TrainState
-from gym import spaces
+from gymnasium import spaces
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 from stable_baselines3.common.utils import explained_variance, get_schedule_fn
 
 from sbx.common.on_policy_algorithm import OnPolicyAlgorithmJax
 from sbx.ppo.policies import PPOPolicy
 
 PPOSelf = TypeVar("PPOSelf", bound="PPO")
@@ -69,14 +69,15 @@
     """
 
     policy_aliases: Dict[str, Type[PPOPolicy]] = {  # type: ignore[assignment]
         "MlpPolicy": PPOPolicy,
         # "CnnPolicy": ActorCriticCnnPolicy,
         # "MultiInputPolicy": MultiInputActorCriticPolicy,
     }
+    policy: PPOPolicy  # type: ignore[assignment]
 
     def __init__(
         self,
         policy: Union[str, Type[PPOPolicy]],
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 3e-4,
         n_steps: int = 2048,
@@ -162,22 +163,23 @@
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
 
-        if self.policy is None:  # type: ignore[has-type]
-            self.policy = self.policy_class(  # pytype:disable=not-instantiable
+        if not hasattr(self, "policy") or self.policy is None:  # type: ignore[has-type]
+            # pytype:disable=not-instantiable
+            self.policy = self.policy_class(  # type: ignore[assignment]
                 self.observation_space,
                 self.action_space,
                 self.lr_schedule,
-                **self.policy_kwargs,  # pytype:disable=not-instantiable
+                **self.policy_kwargs,
             )
-            assert isinstance(self.policy, PPOPolicy)
+            # pytype:enable=not-instantiable
 
             self.key = self.policy.build(self.key, self.lr_schedule, self.max_grad_norm)
 
             self.key, ent_key = jax.random.split(self.key, 2)
 
             self.actor = self.policy.actor
             self.vf = self.policy.vf
@@ -253,15 +255,15 @@
         # self._update_learning_rate(self.policy.optimizer)
         # Compute current clip range
         clip_range = self.clip_range_schedule(self._current_progress_remaining)
 
         # train for n_epochs epochs
         for _ in range(self.n_epochs):
             # JIT only one update
-            for rollout_data in self.rollout_buffer.get(self.batch_size):
+            for rollout_data in self.rollout_buffer.get(self.batch_size):  # type: ignore[attr-defined]
                 if isinstance(self.action_space, spaces.Discrete):
                     # Convert discrete action from float to int
                     actions = rollout_data.actions.flatten().numpy().astype(np.int32)
                 else:
                     actions = rollout_data.actions.numpy()
 
                 (self.policy.actor_state, self.policy.vf_state), (pg_loss, value_loss) = self._one_update(
@@ -275,15 +277,18 @@
                     clip_range=clip_range,
                     ent_coef=self.ent_coef,
                     vf_coef=self.vf_coef,
                     normalize_advantage=self.normalize_advantage,
                 )
 
         self._n_updates += self.n_epochs
-        explained_var = explained_variance(self.rollout_buffer.values.flatten(), self.rollout_buffer.returns.flatten())
+        explained_var = explained_variance(
+            self.rollout_buffer.values.flatten(),  # type: ignore[attr-defined]
+            self.rollout_buffer.returns.flatten(),  # type: ignore[attr-defined]
+        )
 
         # Logs
         # self.logger.record("train/entropy_loss", np.mean(entropy_losses))
         # self.logger.record("train/policy_gradient_loss", np.mean(pg_losses))
         # TODO: use mean instead of one point
         self.logger.record("train/value_loss", value_loss.item())
         # self.logger.record("train/approx_kl", np.mean(approx_kl_divs))
```

### Comparing `sbx-rl-0.6.0/sbx/sac/policies.py` & `sbx-rl-0.7.0/sbx/sac/policies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,50 @@
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 import flax.linen as nn
-import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 import tensorflow_probability
 from flax.training.train_state import TrainState
+from gymnasium import spaces
 from stable_baselines3.common.type_aliases import Schedule
 
 from sbx.common.distributions import TanhTransformedDistribution
 from sbx.common.policies import BaseJaxPolicy
 from sbx.common.type_aliases import RLTrainState
 
 tfp = tensorflow_probability.substrates.jax
 tfd = tfp.distributions
 
 
 class Critic(nn.Module):
+    net_arch: Sequence[int]
     use_layer_norm: bool = False
     dropout_rate: Optional[float] = None
-    n_units: int = 256
 
     @nn.compact
     def __call__(self, x: jnp.ndarray, action: jnp.ndarray) -> jnp.ndarray:
         x = jnp.concatenate([x, action], -1)
-        x = nn.Dense(self.n_units)(x)
-        if self.dropout_rate is not None and self.dropout_rate > 0:
-            x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
-        if self.use_layer_norm:
-            x = nn.LayerNorm()(x)
-        x = nn.relu(x)
-        x = nn.Dense(self.n_units)(x)
-        if self.dropout_rate is not None and self.dropout_rate > 0:
-            x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
-        if self.use_layer_norm:
-            x = nn.LayerNorm()(x)
-        x = nn.relu(x)
+        for n_units in self.net_arch:
+            x = nn.Dense(n_units)(x)
+            if self.dropout_rate is not None and self.dropout_rate > 0:
+                x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
+            if self.use_layer_norm:
+                x = nn.LayerNorm()(x)
+            x = nn.relu(x)
         x = nn.Dense(1)(x)
         return x
 
 
 class VectorCritic(nn.Module):
+    net_arch: Sequence[int]
     use_layer_norm: bool = False
     dropout_rate: Optional[float] = None
-    n_units: int = 256
     n_critics: int = 2
 
     @nn.compact
     def __call__(self, obs: jnp.ndarray, action: jnp.ndarray):
         # Idea taken from https://github.com/perrin-isir/xpag
         # Similar to https://github.com/tinkoff-ai/CORL for PyTorch
         vmap_critic = nn.vmap(
@@ -59,49 +54,50 @@
             in_axes=None,
             out_axes=0,
             axis_size=self.n_critics,
         )
         q_values = vmap_critic(
             use_layer_norm=self.use_layer_norm,
             dropout_rate=self.dropout_rate,
-            n_units=self.n_units,
+            net_arch=self.net_arch,
         )(obs, action)
         return q_values
 
 
 class Actor(nn.Module):
+    net_arch: Sequence[int]
     action_dim: int
-    n_units: int = 256
     log_std_min: float = -20
     log_std_max: float = 2
 
     def get_std(self):
         # Make it work with gSDE
         return jnp.array(0.0)
 
     @nn.compact
     def __call__(self, x: jnp.ndarray) -> tfd.Distribution:  # type: ignore[name-defined]
-        x = nn.Dense(self.n_units)(x)
-        x = nn.relu(x)
-        x = nn.Dense(self.n_units)(x)
-        x = nn.relu(x)
+        for n_units in self.net_arch:
+            x = nn.Dense(n_units)(x)
+            x = nn.relu(x)
         mean = nn.Dense(self.action_dim)(x)
         log_std = nn.Dense(self.action_dim)(x)
         log_std = jnp.clip(log_std, self.log_std_min, self.log_std_max)
         dist = TanhTransformedDistribution(
             tfd.MultivariateNormalDiag(loc=mean, scale_diag=jnp.exp(log_std)),
         )
         return dist
 
 
 class SACPolicy(BaseJaxPolicy):
+    action_space: spaces.Box  # type: ignore[assignment]
+
     def __init__(
         self,
-        observation_space: gym.spaces.Space,
-        action_space: gym.spaces.Space,
+        observation_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         dropout_rate: float = 0.0,
         layer_norm: bool = False,
         # activation_fn: Type[nn.Module] = nn.ReLU,
         use_sde: bool = False,
         # Note: most gSDE parameters are not used
@@ -125,36 +121,42 @@
             optimizer_class=optimizer_class,
             optimizer_kwargs=optimizer_kwargs,
             squash_output=True,
         )
         self.dropout_rate = dropout_rate
         self.layer_norm = layer_norm
         if net_arch is not None:
-            assert isinstance(net_arch, list)
-            self.n_units = net_arch[0]
+            if isinstance(net_arch, list):
+                self.net_arch_pi = self.net_arch_qf = net_arch
+            else:
+                self.net_arch_pi = net_arch["pi"]
+                self.net_arch_qf = net_arch["qf"]
         else:
-            self.n_units = 256
+            self.net_arch_pi = self.net_arch_qf = [256, 256]
         self.n_critics = n_critics
         self.use_sde = use_sde
 
         self.key = self.noise_key = jax.random.PRNGKey(0)
 
-    def build(self, key, lr_schedule: Schedule, qf_learning_rate: float) -> None:
+    def build(self, key: jax.random.KeyArray, lr_schedule: Schedule, qf_learning_rate: float) -> jax.random.KeyArray:
         key, actor_key, qf_key, dropout_key = jax.random.split(key, 4)
         # Keep a key for the actor
         key, self.key = jax.random.split(key, 2)
         # Initialize noise
         self.reset_noise()
 
-        obs = jnp.array([self.observation_space.sample()])
+        if isinstance(self.observation_space, spaces.Dict):
+            obs = jnp.array([spaces.flatten(self.observation_space, self.observation_space.sample())])
+        else:
+            obs = jnp.array([self.observation_space.sample()])
         action = jnp.array([self.action_space.sample()])
 
         self.actor = Actor(
-            action_dim=np.prod(self.action_space.shape),
-            n_units=self.n_units,
+            action_dim=int(np.prod(self.action_space.shape)),
+            net_arch=self.net_arch_pi,
         )
         # Hack to make gSDE work without modifying internal SB3 code
         self.actor.reset_noise = self.reset_noise
 
         self.actor_state = TrainState.create(
             apply_fn=self.actor.apply,
             params=self.actor.init(actor_key, obs),
@@ -163,15 +165,15 @@
                 **self.optimizer_kwargs,
             ),
         )
 
         self.qf = VectorCritic(
             dropout_rate=self.dropout_rate,
             use_layer_norm=self.layer_norm,
-            n_units=self.n_units,
+            net_arch=self.net_arch_qf,
             n_critics=self.n_critics,
         )
 
         self.qf_state = RLTrainState.create(
             apply_fn=self.qf.apply,
             params=self.qf.init(
                 {"params": qf_key, "dropout": dropout_key},
```

### Comparing `sbx-rl-0.6.0/sbx/sac/sac.py` & `sbx-rl-0.7.0/sbx/sac/sac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
 import flax
 import flax.linen as nn
-import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
+from gymnasium import spaces
+from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 
 from sbx.common.off_policy_algorithm import OffPolicyAlgorithmJax
 from sbx.common.type_aliases import ReplayBufferSamplesNp, RLTrainState
 from sbx.sac.policies import SACPolicy
 
@@ -36,16 +37,21 @@
         self.param("dummy_param", init_fn=lambda key: jnp.full((), self.ent_coef_init))
         return self.ent_coef_init
 
 
 class SAC(OffPolicyAlgorithmJax):
     policy_aliases: Dict[str, Type[SACPolicy]] = {  # type: ignore[assignment]
         "MlpPolicy": SACPolicy,
+        # Minimal dict support using flatten()
+        "MultiInputPolicy": SACPolicy,
     }
 
+    policy: SACPolicy
+    action_space: spaces.Box  # type: ignore[assignment]
+
     def __init__(
         self,
         policy,
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 3e-4,
         qf_learning_rate: Optional[float] = None,
         buffer_size: int = 1_000_000,  # 1e6
@@ -53,14 +59,16 @@
         batch_size: int = 256,
         tau: float = 0.005,
         gamma: float = 0.99,
         train_freq: Union[int, Tuple[int, str]] = 1,
         gradient_steps: int = 1,
         policy_delay: int = 1,
         action_noise: Optional[ActionNoise] = None,
+        replay_buffer_class: Optional[Type[ReplayBuffer]] = None,
+        replay_buffer_kwargs: Optional[Dict[str, Any]] = None,
         ent_coef: Union[str, float] = "auto",
         use_sde: bool = False,
         sde_sample_freq: int = -1,
         use_sde_at_warmup: bool = False,
         tensorboard_log: Optional[str] = None,
         policy_kwargs: Optional[Dict[str, Any]] = None,
         verbose: int = 0,
@@ -77,52 +85,54 @@
             learning_starts=learning_starts,
             batch_size=batch_size,
             tau=tau,
             gamma=gamma,
             train_freq=train_freq,
             gradient_steps=gradient_steps,
             action_noise=action_noise,
+            replay_buffer_class=replay_buffer_class,
+            replay_buffer_kwargs=replay_buffer_kwargs,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             use_sde_at_warmup=use_sde_at_warmup,
             policy_kwargs=policy_kwargs,
             tensorboard_log=tensorboard_log,
             verbose=verbose,
             seed=seed,
-            supported_action_spaces=(gym.spaces.Box),
+            supported_action_spaces=(spaces.Box,),
             support_multi_env=True,
         )
 
         self.policy_delay = policy_delay
         self.ent_coef_init = ent_coef
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
 
-        if self.policy is None:  # type: ignore[has-type]
+        if not hasattr(self, "policy") or self.policy is None:
             # pytype: disable=not-instantiable
             self.policy = self.policy_class(  # type: ignore[assignment]
                 self.observation_space,
                 self.action_space,
                 self.lr_schedule,
                 **self.policy_kwargs,
             )
             # pytype: enable=not-instantiable
 
-            assert isinstance(self.policy, SACPolicy)
+            assert isinstance(self.qf_learning_rate, float)
 
             self.key = self.policy.build(self.key, self.lr_schedule, self.qf_learning_rate)
 
             self.key, ent_key = jax.random.split(self.key, 2)
 
-            self.actor = self.policy.actor
-            self.qf = self.policy.qf
+            self.actor = self.policy.actor  # type: ignore[assignment]
+            self.qf = self.policy.qf  # type: ignore[assignment]
 
             # The entropy coefficient or entropy can be learned automatically
             # see Automating Entropy Adjustment for Maximum Entropy RL section
             # of https://arxiv.org/abs/1812.05905
             if isinstance(self.ent_coef_init, str) and self.ent_coef_init.startswith("auto"):
                 # Default initial value of ent_coef when learned
                 ent_coef_init = 1.0
@@ -130,18 +140,19 @@
                     ent_coef_init = float(self.ent_coef_init.split("_")[1])
                     assert ent_coef_init > 0.0, "The initial value of ent_coef must be greater than 0"
 
                 # Note: we optimize the log of the entropy coeff which is slightly different from the paper
                 # as discussed in https://github.com/rail-berkeley/softlearning/issues/37
                 self.ent_coef = EntropyCoef(ent_coef_init)
             else:
-                # Force conversion to float
-                # this will throw an error if a malformed string (different from 'auto')
-                # is passed
-                self.ent_coef = ConstantEntropyCoef(self.ent_coef_init)
+                # This will throw an error if a malformed string (different from 'auto') is passed
+                assert isinstance(
+                    self.ent_coef_init, float
+                ), f"Entropy coef must be float when not equal to 'auto', actual: {self.ent_coef_init}"
+                self.ent_coef = ConstantEntropyCoef(self.ent_coef_init)  # type: ignore[assignment]
 
             self.ent_coef_state = TrainState.create(
                 apply_fn=self.ent_coef.apply,
                 params=self.ent_coef.init(ent_key)["params"],
                 tx=optax.adam(
                     learning_rate=self.learning_rate,
                 ),
@@ -172,19 +183,28 @@
         # Sample all at once for efficiency (so we can jit the for loop)
         data = self.replay_buffer.sample(batch_size * gradient_steps, env=self._vec_normalize_env)
         # Pre-compute the indices where we need to update the actor
         # This is a hack in order to jit the train loop
         # It will compile once per value of policy_delay_indices
         policy_delay_indices = {i: True for i in range(gradient_steps) if ((self._n_updates + i + 1) % self.policy_delay) == 0}
         policy_delay_indices = flax.core.FrozenDict(policy_delay_indices)
+
+        if isinstance(data.observations, dict):
+            keys = list(self.observation_space.keys())
+            obs = np.concatenate([data.observations[key].numpy() for key in keys], axis=1)
+            next_obs = np.concatenate([data.next_observations[key].numpy() for key in keys], axis=1)
+        else:
+            obs = data.observations.numpy()
+            next_obs = data.next_observations.numpy()
+
         # Convert to numpy
         data = ReplayBufferSamplesNp(
-            data.observations.numpy(),
+            obs,
             data.actions.numpy(),
-            data.next_observations.numpy(),
+            next_obs,
             data.dones.numpy().flatten(),
             data.rewards.numpy().flatten(),
         )
 
         (
             self.policy.qf_state,
             self.policy.actor_state,
```

### Comparing `sbx-rl-0.6.0/sbx/tqc/policies.py` & `sbx-rl-0.7.0/sbx/tqc/policies.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,78 @@
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 import flax.linen as nn
-import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 import tensorflow_probability
 from flax.training.train_state import TrainState
+from gymnasium import spaces
 from stable_baselines3.common.type_aliases import Schedule
 
 from sbx.common.distributions import TanhTransformedDistribution
 from sbx.common.policies import BaseJaxPolicy
 from sbx.common.type_aliases import RLTrainState
 
 tfp = tensorflow_probability.substrates.jax
 tfd = tfp.distributions
 
 
 class Critic(nn.Module):
+    net_arch: Sequence[int]
     use_layer_norm: bool = False
     dropout_rate: Optional[float] = None
     n_quantiles: int = 25
-    n_units: int = 256
 
     @nn.compact
     def __call__(self, x: jnp.ndarray, a: jnp.ndarray, training: bool = False) -> jnp.ndarray:
         x = jnp.concatenate([x, a], -1)
-        x = nn.Dense(self.n_units)(x)
-        if self.dropout_rate is not None and self.dropout_rate > 0:
-            x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
-        if self.use_layer_norm:
-            x = nn.LayerNorm()(x)
-        x = nn.relu(x)
-        x = nn.Dense(self.n_units)(x)
-        if self.dropout_rate is not None and self.dropout_rate > 0:
-            x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
-        if self.use_layer_norm:
-            x = nn.LayerNorm()(x)
-        x = nn.relu(x)
+        for n_units in self.net_arch:
+            x = nn.Dense(n_units)(x)
+            if self.dropout_rate is not None and self.dropout_rate > 0:
+                x = nn.Dropout(rate=self.dropout_rate)(x, deterministic=False)
+            if self.use_layer_norm:
+                x = nn.LayerNorm()(x)
+            x = nn.relu(x)
         x = nn.Dense(self.n_quantiles)(x)
         return x
 
 
 class Actor(nn.Module):
+    net_arch: Sequence[int]
     action_dim: int
-    n_units: int = 256
     log_std_min: float = -20
     log_std_max: float = 2
 
     def get_std(self):
         # Make it work with gSDE
         return jnp.array(0.0)
 
     @nn.compact
     def __call__(self, x: jnp.ndarray) -> tfd.Distribution:  # type: ignore[name-defined]
-        x = nn.Dense(self.n_units)(x)
-        x = nn.relu(x)
-        x = nn.Dense(self.n_units)(x)
-        x = nn.relu(x)
+        for n_units in self.net_arch:
+            x = nn.Dense(n_units)(x)
+            x = nn.relu(x)
         mean = nn.Dense(self.action_dim)(x)
         log_std = nn.Dense(self.action_dim)(x)
         log_std = jnp.clip(log_std, self.log_std_min, self.log_std_max)
         dist = TanhTransformedDistribution(
             tfd.MultivariateNormalDiag(loc=mean, scale_diag=jnp.exp(log_std)),
         )
         return dist
 
 
 class TQCPolicy(BaseJaxPolicy):
+    action_space: spaces.Box  # type: ignore[assignment]
+
     def __init__(
         self,
-        observation_space: gym.spaces.Space,
-        action_space: gym.spaces.Space,
+        observation_space: spaces.Space,
+        action_space: spaces.Box,
         lr_schedule: Schedule,
         net_arch: Optional[Union[List[int], Dict[str, List[int]]]] = None,
         dropout_rate: float = 0.0,
         layer_norm: bool = False,
         top_quantiles_to_drop_per_net: int = 2,
         n_quantiles: int = 25,
         # activation_fn: Type[nn.Module] = nn.ReLU,
@@ -102,41 +98,48 @@
             optimizer_class=optimizer_class,
             optimizer_kwargs=optimizer_kwargs,
             squash_output=True,
         )
         self.dropout_rate = dropout_rate
         self.layer_norm = layer_norm
         if net_arch is not None:
-            assert isinstance(net_arch, list)
-            self.n_units = net_arch[0]
+            if isinstance(net_arch, list):
+                self.net_arch_pi = self.net_arch_qf = net_arch
+            else:
+                self.net_arch_pi = net_arch["pi"]
+                self.net_arch_qf = net_arch["qf"]
         else:
-            self.n_units = 256
+            self.net_arch_pi = self.net_arch_qf = [256, 256]
         self.n_quantiles = n_quantiles
         self.n_critics = n_critics
         self.top_quantiles_to_drop_per_net = top_quantiles_to_drop_per_net
         # Sort and drop top k quantiles to control overestimation.
         quantiles_total = self.n_quantiles * self.n_critics
         top_quantiles_to_drop_per_net = self.top_quantiles_to_drop_per_net
         self.n_target_quantiles = quantiles_total - top_quantiles_to_drop_per_net * self.n_critics
         self.use_sde = use_sde
 
         self.key = self.noise_key = jax.random.PRNGKey(0)
 
-    def build(self, key, lr_schedule: Schedule, qf_learning_rate: float) -> None:
+    def build(self, key: jax.random.KeyArray, lr_schedule: Schedule, qf_learning_rate: float) -> jax.random.KeyArray:
         key, actor_key, qf1_key, qf2_key = jax.random.split(key, 4)
         key, dropout_key1, dropout_key2, self.key = jax.random.split(key, 4)
         # Initialize noise
         self.reset_noise()
 
-        obs = jnp.array([self.observation_space.sample()])
+        if isinstance(self.observation_space, spaces.Dict):
+            obs = jnp.array([spaces.flatten(self.observation_space, self.observation_space.sample())])
+        else:
+            obs = jnp.array([self.observation_space.sample()])
+
         action = jnp.array([self.action_space.sample()])
 
         self.actor = Actor(
-            action_dim=np.prod(self.action_space.shape),
-            n_units=self.n_units,
+            action_dim=int(np.prod(self.action_space.shape)),
+            net_arch=self.net_arch_pi,
         )
         # Hack to make gSDE work without modifying internal SB3 code
         self.actor.reset_noise = self.reset_noise
 
         self.actor_state = TrainState.create(
             apply_fn=self.actor.apply,
             params=self.actor.init(actor_key, obs),
@@ -145,15 +148,15 @@
                 **self.optimizer_kwargs,
             ),
         )
 
         self.qf = Critic(
             dropout_rate=self.dropout_rate,
             use_layer_norm=self.layer_norm,
-            n_units=self.n_units,
+            net_arch=self.net_arch_qf,
             n_quantiles=self.n_quantiles,
         )
 
         self.qf1_state = RLTrainState.create(
             apply_fn=self.qf.apply,
             params=self.qf.init(
                 {"params": qf1_key, "dropout": dropout_key1},
```

### Comparing `sbx-rl-0.6.0/sbx/tqc/tqc.py` & `sbx-rl-0.7.0/sbx/tqc/tqc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
 import flax
 import flax.linen as nn
-import gym
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
+from gymnasium import spaces
+from stable_baselines3.common.buffers import ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.type_aliases import GymEnv, MaybeCallback, Schedule
 
 from sbx.common.off_policy_algorithm import OffPolicyAlgorithmJax
 from sbx.common.type_aliases import ReplayBufferSamplesNp, RLTrainState
 from sbx.tqc.policies import TQCPolicy
 
@@ -36,16 +37,21 @@
         self.param("dummy_param", init_fn=lambda key: jnp.full((), self.ent_coef_init))
         return self.ent_coef_init
 
 
 class TQC(OffPolicyAlgorithmJax):
     policy_aliases: Dict[str, Type[TQCPolicy]] = {  # type: ignore[assignment]
         "MlpPolicy": TQCPolicy,
+        # Minimal dict support using flatten()
+        "MultiInputPolicy": TQCPolicy,
     }
 
+    policy: TQCPolicy
+    action_space: spaces.Box  # type: ignore[assignment]
+
     def __init__(
         self,
         policy,
         env: Union[GymEnv, str],
         learning_rate: Union[float, Schedule] = 3e-4,
         qf_learning_rate: Optional[float] = None,
         buffer_size: int = 1_000_000,  # 1e6
@@ -54,14 +60,16 @@
         tau: float = 0.005,
         gamma: float = 0.99,
         train_freq: Union[int, Tuple[int, str]] = 1,
         gradient_steps: int = 1,
         policy_delay: int = 1,
         top_quantiles_to_drop_per_net: int = 2,
         action_noise: Optional[ActionNoise] = None,
+        replay_buffer_class: Optional[Type[ReplayBuffer]] = None,
+        replay_buffer_kwargs: Optional[Dict[str, Any]] = None,
         ent_coef: Union[str, float] = "auto",
         use_sde: bool = False,
         sde_sample_freq: int = -1,
         use_sde_at_warmup: bool = False,
         tensorboard_log: Optional[str] = None,
         policy_kwargs: Optional[Dict[str, Any]] = None,
         verbose: int = 0,
@@ -78,51 +86,53 @@
             learning_starts=learning_starts,
             batch_size=batch_size,
             tau=tau,
             gamma=gamma,
             train_freq=train_freq,
             gradient_steps=gradient_steps,
             action_noise=action_noise,
+            replay_buffer_class=replay_buffer_class,
+            replay_buffer_kwargs=replay_buffer_kwargs,
             use_sde=use_sde,
             sde_sample_freq=sde_sample_freq,
             use_sde_at_warmup=use_sde_at_warmup,
             policy_kwargs=policy_kwargs,
             tensorboard_log=tensorboard_log,
             verbose=verbose,
             seed=seed,
-            supported_action_spaces=(gym.spaces.Box),
+            supported_action_spaces=(spaces.Box,),
             support_multi_env=True,
         )
 
         self.policy_delay = policy_delay
         self.ent_coef_init = ent_coef
         self.policy_kwargs["top_quantiles_to_drop_per_net"] = top_quantiles_to_drop_per_net
 
         if _init_setup_model:
             self._setup_model()
 
     def _setup_model(self) -> None:
         super()._setup_model()
 
-        if self.policy is None:  # type: ignore[has-type]
+        if not hasattr(self, "policy") or self.policy is None:
             # pytype: disable=not-instantiable
             self.policy = self.policy_class(  # type: ignore[assignment]
                 self.observation_space,
                 self.action_space,
                 self.lr_schedule,
                 **self.policy_kwargs,
             )
             # pytype: enable=not-instantiable
-            assert isinstance(self.policy, TQCPolicy)
+            assert isinstance(self.qf_learning_rate, float)
 
             self.key = self.policy.build(self.key, self.lr_schedule, self.qf_learning_rate)
 
             self.key, ent_key = jax.random.split(self.key, 2)
 
-            self.actor = self.policy.actor
+            self.actor = self.policy.actor  # type: ignore[assignment]
             self.qf = self.policy.qf
 
             # The entropy coefficient or entropy can be learned automatically
             # see Automating Entropy Adjustment for Maximum Entropy RL section
             # of https://arxiv.org/abs/1812.05905
             if isinstance(self.ent_coef_init, str) and self.ent_coef_init.startswith("auto"):
                 # Default initial value of ent_coef when learned
@@ -131,18 +141,19 @@
                     ent_coef_init = float(self.ent_coef_init.split("_")[1])
                     assert ent_coef_init > 0.0, "The initial value of ent_coef must be greater than 0"
 
                 # Note: we optimize the log of the entropy coeff which is slightly different from the paper
                 # as discussed in https://github.com/rail-berkeley/softlearning/issues/37
                 self.ent_coef = EntropyCoef(ent_coef_init)
             else:
-                # Force conversion to float
-                # this will throw an error if a malformed string (different from 'auto')
-                # is passed
-                self.ent_coef = ConstantEntropyCoef(self.ent_coef_init)
+                # This will throw an error if a malformed string (different from 'auto') is passed
+                assert isinstance(
+                    self.ent_coef_init, float
+                ), f"Entropy coef must be float when not equal to 'auto', actual: {self.ent_coef_init}"
+                self.ent_coef = ConstantEntropyCoef(self.ent_coef_init)  # type: ignore[assignment]
 
             self.ent_coef_state = TrainState.create(
                 apply_fn=self.ent_coef.apply,
                 params=self.ent_coef.init(ent_key)["params"],
                 tx=optax.adam(
                     learning_rate=self.learning_rate,
                 ),
@@ -174,23 +185,30 @@
         data = self.replay_buffer.sample(batch_size * gradient_steps, env=self._vec_normalize_env)
         # Pre-compute the indices where we need to update the actor
         # This is a hack in order to jit the train loop
         # It will compile once per value of policy_delay_indices
         policy_delay_indices = {i: True for i in range(gradient_steps) if ((self._n_updates + i + 1) % self.policy_delay) == 0}
         policy_delay_indices = flax.core.FrozenDict(policy_delay_indices)
 
+        if isinstance(data.observations, dict):
+            keys = list(self.observation_space.keys())
+            obs = np.concatenate([data.observations[key].numpy() for key in keys], axis=1)
+            next_obs = np.concatenate([data.next_observations[key].numpy() for key in keys], axis=1)
+        else:
+            obs = data.observations.numpy()
+            next_obs = data.next_observations.numpy()
+
         # Convert to numpy
         data = ReplayBufferSamplesNp(
-            data.observations.numpy(),
+            obs,
             data.actions.numpy(),
-            data.next_observations.numpy(),
+            next_obs,
             data.dones.numpy().flatten(),
             data.rewards.numpy().flatten(),
         )
-
         (
             self.policy.qf1_state,
             self.policy.qf2_state,
             self.policy.actor_state,
             self.ent_coef_state,
             self.key,
             (qf1_loss_value, qf2_loss_value, actor_loss_value, ent_coef_value),
```

### Comparing `sbx-rl-0.6.0/sbx_rl.egg-info/PKG-INFO` & `sbx-rl-0.7.0/sbx_rl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbx-rl
-Version: 0.6.0
+Version: 0.7.0
 Summary: Jax version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/araffin/sbx
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbx-rl-0.6.0/sbx_rl.egg-info/SOURCES.txt` & `sbx-rl-0.7.0/sbx_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.6.0/setup.py` & `sbx-rl-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 setup(
     name="sbx-rl",
     packages=[package for package in find_packages() if package.startswith("sbx")],
     package_data={"sbx": ["py.typed", "version.txt"]},
     install_requires=[
-        "stable_baselines3>=1.8.0a9",
+        "stable_baselines3>=2.0.0a4",
         "jax",
         "jaxlib",
         "flax",
         "optax",
         "tqdm",
         "rich",
         "tensorflow_probability",
```

### Comparing `sbx-rl-0.6.0/tests/test_run.py` & `sbx-rl-0.7.0/tests/test_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from typing import Optional, Type
+
 import numpy as np
 import pytest
+from stable_baselines3 import HerReplayBuffer
 from stable_baselines3.common.env_util import make_vec_env
+from stable_baselines3.common.envs import BitFlippingEnv
 from stable_baselines3.common.evaluation import evaluate_policy
 
 from sbx import DQN, PPO, SAC, TQC, DroQ
 
 
 def test_droq(tmp_path):
     model = DroQ(
@@ -53,27 +57,27 @@
         use_sde=True,
         qf_learning_rate=1e-3,
     )
     model.learn(200)
 
 
 @pytest.mark.parametrize("model_class", [SAC])
-def test_sac(model_class):
+def test_sac(model_class: Type[SAC]) -> None:
     model = model_class(
         "MlpPolicy",
         "Pendulum-v1",
         verbose=1,
         gradient_steps=1,
         learning_rate=1e-3,
     )
     model.learn(110)
 
 
 @pytest.mark.parametrize("env_id", ["Pendulum-v1", "CartPole-v1"])
-def test_ppo(env_id):
+def test_ppo(env_id: str) -> None:
     model = PPO(
         "MlpPolicy",
         env_id,
         verbose=1,
         n_steps=64,
         n_epochs=2,
     )
@@ -85,7 +89,15 @@
         "MlpPolicy",
         "CartPole-v1",
         verbose=1,
         gradient_steps=-1,
         target_update_interval=10,
     )
     model.learn(128)
+
+
+@pytest.mark.parametrize("replay_buffer_class", [None, HerReplayBuffer])
+def test_dict(replay_buffer_class: Optional[Type[HerReplayBuffer]]) -> None:
+    env = BitFlippingEnv(n_bits=2, continuous=True)
+    model = SAC("MultiInputPolicy", env, replay_buffer_class=replay_buffer_class)
+
+    model.learn(int(200), progress_bar=True)
```

