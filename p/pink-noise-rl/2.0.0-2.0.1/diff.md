# Comparing `tmp/pink_noise_rl-2.0.0.tar.gz` & `tmp/pink_noise_rl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pink_noise_rl-2.0.0.tar", max compression
+gzip compressed data, was "pink_noise_rl-2.0.1.tar", max compression
```

## Comparing `pink_noise_rl-2.0.0.tar` & `pink_noise_rl-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-12-01 19:23:33.638474 pink_noise_rl-2.0.0/LICENSE
--rw-r--r--   0        0        0     3132 2023-03-16 16:28:59.056121 pink_noise_rl-2.0.0/README.md
--rw-r--r--   0        0        0      129 2023-03-16 16:28:59.057074 pink_noise_rl-2.0.0/pink/__init__.py
--rw-r--r--   0        0        0     4443 2023-03-16 16:28:59.057485 pink_noise_rl-2.0.0/pink/cnrl.py
--rw-r--r--   0        0        0     4132 2023-03-16 16:28:59.057894 pink_noise_rl-2.0.0/pink/colorednoise.py
--rw-r--r--   0        0        0     7856 2023-03-16 16:28:59.058215 pink_noise_rl-2.0.0/pink/sb3.py
--rw-r--r--   0        0        0     1552 2023-03-16 16:28:59.058751 pink_noise_rl-2.0.0/pink/tonic.py
--rw-r--r--   0        0        0      457 2023-03-16 16:28:59.059201 pink_noise_rl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 pink_noise_rl-2.0.0/setup.py
--rw-r--r--   0        0        0     3841 1970-01-01 00:00:00.000000 pink_noise_rl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-12-01 19:23:33.638474 pink_noise_rl-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3132 2023-03-16 16:28:59.056121 pink_noise_rl-2.0.1/README.md
+-rw-r--r--   0        0        0      129 2023-03-16 16:28:59.057074 pink_noise_rl-2.0.1/pink/__init__.py
+-rw-r--r--   0        0        0     4951 2023-04-13 13:07:59.361603 pink_noise_rl-2.0.1/pink/cnrl.py
+-rw-r--r--   0        0        0     4132 2023-03-16 16:28:59.057894 pink_noise_rl-2.0.1/pink/colorednoise.py
+-rw-r--r--   0        0        0     7856 2023-03-16 16:28:59.058215 pink_noise_rl-2.0.1/pink/sb3.py
+-rw-r--r--   0        0        0     1552 2023-03-16 16:28:59.058751 pink_noise_rl-2.0.1/pink/tonic.py
+-rw-r--r--   0        0        0      457 2023-04-13 13:08:38.532456 pink_noise_rl-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 pink_noise_rl-2.0.1/setup.py
+-rw-r--r--   0        0        0     3841 1970-01-01 00:00:00.000000 pink_noise_rl-2.0.1/PKG-INFO
```

### Comparing `pink_noise_rl-2.0.0/LICENSE` & `pink_noise_rl-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pink_noise_rl-2.0.0/README.md` & `pink_noise_rl-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pink_noise_rl-2.0.0/pink/cnrl.py` & `pink_noise_rl-2.0.1/pink/cnrl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import numpy as np
+
 from . import colorednoise as cn
 
 
 class ColoredNoiseProcess():
     """Infinite colored noise process.
 
     Implemented as a buffer: every `size[-1]` samples, a cut to a new time series starts. As this cut influences the
     PSD of the combined signal, the maximum period (1 / low-frequency cutoff) can be specified.
 
     Methods
     -------
-    sample()
-        Sample a single timestep from the colored nosie process.
+    sample(T=1)
+        Sample `T` timesteps from the colored noise process.
+    reset()
+        Reset the buffer with a new time series.
     """
     def __init__(self, beta, size, scale=1, max_period=None, rng=None):
         """Infinite colored noise process.
 
         Implemented as a buffer: every `size[-1]` samples, a cut to a new time series starts. As this cut influences
         the PSD of the combined signal, the maximum period (1 / low-frequency cutoff) can be specified.
 
@@ -45,49 +49,65 @@
         # The last component of size is the time index
         try:
             self.size = list(size)
         except TypeError:
             self.size = [size]
         self.time_steps = self.size[-1]
 
-        # Set first time-step such that buffer will be initialized
-        self.idx = self.time_steps
+        # Fill buffer and reset index
+        self.reset()
+
+    def reset(self):
+        """Reset the buffer with a new time series."""
+        self.buffer = cn.powerlaw_psd_gaussian(
+                exponent=self.beta, size=self.size, fmin=self.minimum_frequency, rng=self.rng)
+        self.idx = 0
 
-    def sample(self):
+    def sample(self, T=1):
         """
-        Sample a single timestep from the colored nosie process.
+        Sample `T` timesteps from the colored noise process.
 
         The buffer is automatically refilled when necessary.
 
+        Parameters
+        ----------
+        T : int, optional, by default 1
+            Number of samples to draw
+
         Returns
         -------
         array_like
-            Sampled vector of shape `size[:-1]`
+            Sampled vector of shape `(*size[:-1], T)`
         """
-        self.idx += 1    # Next time step
-
-        # Refill buffer if depleted
-        if self.idx >= self.time_steps:
-            self.buffer = cn.powerlaw_psd_gaussian(
-                exponent=self.beta, size=self.size, fmin=self.minimum_frequency, rng=self.rng)
-            self.idx = 0
+        n = 0
+        ret = []
+        while n < T:
+            if self.idx >= self.time_steps:
+                self.reset()
+            m = min(T - n, self.time_steps - self.idx)
+            ret.append(self.buffer[..., self.idx:(self.idx + m)])
+            n += m
+            self.idx += m
 
-        return self.scale * self.buffer[..., self.idx]
+        ret = self.scale * np.concatenate(ret, axis=-1)
+        return ret if n > 1 else ret[..., 0]
 
 
 class PinkNoiseProcess(ColoredNoiseProcess):
     """Infinite pink noise process.
 
     Implemented as a buffer: every `size[-1]` samples, a cut to a new time series starts. As this cut influences the
     PSD of the combined signal, the maximum period (1 / low-frequency cutoff) can be specified.
 
     Methods
     -------
-    sample()
-        Sample a single timestep from the pink nosie process.
+    sample(T=1)
+        Sample `T` timesteps from the pink noise process.
+    reset()
+        Reset the buffer with a new time series.
     """
     def __init__(self, size, scale=1, max_period=None, rng=None):
         """Infinite pink noise process.
 
         Implemented as a buffer: every `size[-1]` samples, a cut to a new time series starts. As this cut influences
         the PSD of the combined signal, the maximum period (1 / low-frequency cutoff) can be specified.
```

### Comparing `pink_noise_rl-2.0.0/pink/colorednoise.py` & `pink_noise_rl-2.0.1/pink/colorednoise.py`

 * *Files identical despite different names*

### Comparing `pink_noise_rl-2.0.0/pink/sb3.py` & `pink_noise_rl-2.0.1/pink/sb3.py`

 * *Files identical despite different names*

### Comparing `pink_noise_rl-2.0.0/pink/tonic.py` & `pink_noise_rl-2.0.1/pink/tonic.py`

 * *Files identical despite different names*

### Comparing `pink_noise_rl-2.0.0/setup.py` & `pink_noise_rl-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy']
 
 setup_kwargs = {
     'name': 'pink-noise-rl',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Pink noise for exploration in reinforcement learning',
     'long_description': '# Colored Action Noise for Deep RL\n\nThis repository contains easy-to-use implementations of pink noise and general colored noise for use as action noise in deep reinforcement learning. Included are the following classes:\n- `ColoredNoiseProcess` and `PinkNoiseProcess` for general use, based on the [colorednoise](https://github.com/felixpatzelt/colorednoise) library\n- `ColoredActionNoise` and `PinkActionNoise` to be used with deterministic policy algorithms like DDPG and TD3 in Stable Baselines3, both are subclasses of `stable_baselines3.common.noise.ActionNoise`\n- `ColoredNoiseDist`, `PinkNoiseDist` to be used with stochastic policy algorithms like SAC in Stable Baselines3\n- `MPO_CN` for using colored noise (incl. pink noise) with MPO using the Tonic RL library.\n\nFor more information, please see our paper: [Pink Noise Is All You Need: Colored Noise Exploration in Deep Reinforcement Learning](https://bit.ly/pink-noise-rl) (ICLR 2023 Spotlight).\n\n## Installation\nYou can install the library via pip:\n```\npip install pink-noise-rl\n```\nNote: In Python, the import statement is simply `import pink`.\n\n## Usage\nWe provide minimal examples for using pink noise on SAC, TD3 and MPO below. An example comparing pink noise with the default action noise of SAC is included in the `examples` directory.\n\n### Stable Baselines3: SAC, TD3\n```python\nimport gym\nfrom stable_baselines3 import SAC, TD3\n\n# All classes mentioned above can be imported from `pink`\nfrom pink import PinkNoiseDist, PinkActionNoise\n\n# Initialize environment\nenv = gym.make("MountainCarContinuous-v0")\nseq_len = env._max_episode_steps\naction_dim = env.action_space.shape[-1]\n```\n\n#### SAC\n```python\n# Initialize agent\nmodel = SAC("MlpPolicy", env)\n\n# Set action noise\nmodel.actor.action_dist = PinkNoiseDist(seq_len, action_dim)\n\n# Train agent\nmodel.learn(total_timesteps=100_000)\n```\n\n#### TD3\n```python\n# Initialize agent\nmodel = TD3("MlpPolicy", env)\n\n# Set action noise\nnoise_scale = 0.3\nmodel.action_noise = PinkActionNoise(noise_scale, seq_len, action_dim)\n\n# Train agent\nmodel.learn(total_timesteps=100_000)\n```\n\n### Tonic: MPO\n```python\nimport gym\nfrom tonic import Trainer\nfrom pink import MPO_CN\n\n# Initialize environment\nenv = gym.make("MountainCarContinuous-v0")\nseq_len = env._max_episode_steps\n\n# Initialize agent with pink noise\nbeta = 1\nmodel = MPO_CN()\nmodel.initialize(beta, seq_len, env.observation_space, env.action_space)\n\n# Train agent\ntrainer = tonic.Trainer(steps=100_000)\ntrainer.initialize(model, env)\ntrainer.run()\n```\n\n\n## Citing\nIf you use this code in your research, please cite our paper:\n```bibtex\n@inproceedings{eberhard-2023-pink,\n  title = {Pink Noise Is All You Need: Colored Noise Exploration in Deep Reinforcement Learning},\n  author = {Eberhard, Onno and Hollenstein, Jakob and Pinneri, Cristina and Martius, Georg},\n  booktitle = {Proceedings of the Eleventh International Conference on Learning Representations (ICLR 2023)},\n  month = may,\n  year = {2023},\n  url = {https://openreview.net/forum?id=hQ9V5QN27eS}\n}\n```\n\nIf there are any problems, or if you have a question, don\'t hesitate to open an issue here on GitHub.\n',
     'author': 'Onno Eberhard',
     'author_email': 'onnoeberhard@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/martius-lab/pink-noise-rl',
```

### Comparing `pink_noise_rl-2.0.0/PKG-INFO` & `pink_noise_rl-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pink-noise-rl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Pink noise for exploration in reinforcement learning
 Home-page: https://github.com/martius-lab/pink-noise-rl
 License: MIT
 Author: Onno Eberhard
 Author-email: onnoeberhard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

