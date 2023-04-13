# Comparing `tmp/textrl-0.2.15.tar.gz` & `tmp/textrl-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textrl-0.2.15.tar", last modified: Mon Mar 27 14:02:23 2023, max compression
+gzip compressed data, was "textrl-0.2.16.tar", last modified: Thu Apr 13 18:19:35 2023, max compression
```

## Comparing `textrl-0.2.15.tar` & `textrl-0.2.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-03-27 14:02:23.827245 textrl-0.2.15/
--rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.15/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.15/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    11516 2023-03-27 14:02:23.826842 textrl-0.2.15/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    10799 2023-03-27 14:00:43.000000 textrl-0.2.15/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-03-27 14:02:23.820310 textrl-0.2.15/example/
--rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.15/example/2022-12-10-textrl-elon-musk.ipynb
--rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.15/requirement.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2023-03-27 14:02:23.827398 textrl-0.2.15/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-03-27 13:57:04.000000 textrl-0.2.15/setup.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-03-27 14:02:23.824984 textrl-0.2.15/textrl/
--rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.15/textrl/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)    13002 2023-03-27 13:11:50.000000 textrl-0.2.15/textrl/actor.py
--rw-r--r--   0 voidful    (501) staff       (20)     1140 2022-12-05 09:09:02.000000 textrl-0.2.15/textrl/dump.py
--rw-r--r--   0 voidful    (501) staff       (20)     6325 2023-03-27 13:18:12.000000 textrl-0.2.15/textrl/environment.py
--rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.15/textrl/evaluator.py
--rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.15/textrl/trainer.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-03-27 14:02:23.826403 textrl-0.2.15/textrl.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    11516 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      416 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)       50 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/entry_points.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.15/textrl.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)       17 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        7 2023-03-27 14:02:23.000000 textrl-0.2.15/textrl.egg-info/top_level.txt
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-13 18:19:35.562080 textrl-0.2.16/
+-rw-r--r--   0 voidful    (501) staff       (20)     4206 2022-12-05 09:09:02.000000 textrl-0.2.16/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)     1064 2023-02-09 14:54:56.000000 textrl-0.2.16/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    11516 2023-04-13 18:19:35.561837 textrl-0.2.16/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    10799 2023-03-27 14:00:43.000000 textrl-0.2.16/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-13 18:19:35.556412 textrl-0.2.16/example/
+-rw-r--r--   0 voidful    (501) staff       (20)     7679 2023-03-27 13:57:09.000000 textrl-0.2.16/example/2022-12-10-textrl-elon-musk.ipynb
+-rw-r--r--   0 voidful    (501) staff       (20)       61 2022-12-05 09:17:42.000000 textrl-0.2.16/requirement.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2023-04-13 18:19:35.562130 textrl-0.2.16/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)     1095 2023-04-13 18:16:05.000000 textrl-0.2.16/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-13 18:19:35.558186 textrl-0.2.16/textrl/
+-rw-r--r--   0 voidful    (501) staff       (20)      184 2023-02-13 19:45:54.000000 textrl-0.2.16/textrl/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)    13336 2023-04-13 18:15:01.000000 textrl-0.2.16/textrl/actor.py
+-rw-r--r--   0 voidful    (501) staff       (20)     1140 2022-12-05 09:09:02.000000 textrl-0.2.16/textrl/dump.py
+-rw-r--r--   0 voidful    (501) staff       (20)     6325 2023-04-13 15:23:00.000000 textrl-0.2.16/textrl/environment.py
+-rw-r--r--   0 voidful    (501) staff       (20)    23448 2023-02-13 19:43:59.000000 textrl-0.2.16/textrl/evaluator.py
+-rw-r--r--   0 voidful    (501) staff       (20)     7511 2023-02-13 19:43:59.000000 textrl-0.2.16/textrl/trainer.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2023-04-13 18:19:35.561563 textrl-0.2.16/textrl.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    11516 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      416 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       50 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/entry_points.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2022-12-05 09:10:02.000000 textrl-0.2.16/textrl.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)       17 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        7 2023-04-13 18:19:35.000000 textrl-0.2.16/textrl.egg-info/top_level.txt
```

### Comparing `textrl-0.2.15/.gitignore` & `textrl-0.2.16/.gitignore`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/LICENSE` & `textrl-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/PKG-INFO` & `textrl-0.2.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.15
+Version: 0.2.16
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

### Comparing `textrl-0.2.15/README.md` & `textrl-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/example/2022-12-10-textrl-elon-musk.ipynb` & `textrl-0.2.16/example/2022-12-10-textrl-elon-musk.ipynb`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/setup.py` & `textrl-0.2.16/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='textrl',
-    version='0.2.15',
+    version='0.2.16',
     description='TextRL - use reinforcement learning to adjust text generation results.',
     url='https://github.com/voidful/TextRL',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

### Comparing `textrl-0.2.15/textrl/actor.py` & `textrl-0.2.16/textrl/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def forward(self, hidden):
         for module in self.module_list:
             hidden = module(hidden)[0]
         return hidden
 
 
 class TextRLActor:
-    def __init__(self, env, model, tokenizer, gpu_id=0,
+    def __init__(self, env, model, tokenizer, optimizer='sgd', gpu_id=0,
                  unfreeze_layer_from_past=0,
                  act_deterministically=True,
                  temperature=1.0,
                  top_k=0,
                  top_p=1.0,
                  repetition_penalty=1.0):
         self.agent = None
@@ -44,24 +44,25 @@
         self.model = model
         self.obs_size = model.config.hidden_size
         self.converter = self.model.lm_head
         self.act_deterministically = act_deterministically
         self.temperature = temperature
         self.top_k = top_k
         self.top_p = top_p
+        self.optimizer = optimizer
         self.repetition_penalty = repetition_penalty
         self.unfreeze_layer_from_past = unfreeze_layer_from_past
 
         parents = [parent[0] for parent in model.named_children()]
         if 'transformer' in parents:  # gpt2/bloom:
             transformers_model = model.transformer
         elif 'model' in parents:  # bart
             transformers_model = model.model
-        elif 'encoder' in parents:  # t5
-            transformers_model = model.encoder
+        elif 'decoder' in parents:  # t5
+            transformers_model = model.decoder
         else:
             raise ValueError('model not supported')
 
         if unfreeze_layer_from_past > 0:
             self.middle_model = HFModelListModule(list(transformers_model.children())
                                                   [get_modulelist_pos(transformers_model)]
                                                   [-self.unfreeze_layer_from_past:])
@@ -79,20 +80,26 @@
             SoftmaxCategoricalHead(self.env,
                                    temperature=self.temperature,
                                    top_k=self.top_k,
                                    top_p=self.top_p,
                                    repetition_penalty=self.repetition_penalty)
         )
         vf = torch.nn.Sequential(
-            torch.nn.Linear(self.obs_size, self.obs_size//2),
-            torch.nn.Linear(self.obs_size//2, self.obs_size//4),
-            torch.nn.Linear(self.obs_size//4, 1)
+            torch.nn.Linear(self.obs_size, self.obs_size // 2),
+            torch.nn.Linear(self.obs_size // 2, self.obs_size // 4),
+            torch.nn.Linear(self.obs_size // 4, 1)
         )
         model = pfrl.nn.Branched(policy, vf)
-        opt = torch.optim.SGD(model.parameters(), lr=lr)
+        if isinstance(self.optimizer, str):
+            if self.optimizer.lower() == 'adamw':
+                opt = torch.optim.AdamW(model.parameters(), lr=lr)
+            else:
+                opt = torch.optim.SGD(model.parameters(), lr=lr)
+        else:
+            opt = self.optimizer
         model = model.cuda()
         agent = TextPPO(
             model,
             opt,
             gpu=self.gpu_id,
             update_interval=update_interval,
             minibatch_size=minibatch_size,
@@ -286,25 +293,25 @@
         loss_policy = -torch.mean(
             torch.min(
                 (prob_ratio * advs),
                 (torch.clamp(prob_ratio, 1 - self.clip_eps, 1 + self.clip_eps) * advs),
             ),
         )
         if self.clip_eps_vf is None:
-            loss_value_func = F.mse_loss(vs_pred, vs_teacher)
+            loss_value_func = F.mse_loss(vs_pred.squeeze(), vs_teacher.squeeze())
         else:
             clipped_vs_pred = _elementwise_clip(
                 vs_pred,
                 vs_pred_old - self.clip_eps_vf,
                 vs_pred_old + self.clip_eps_vf,
             )
             loss_value_func = torch.mean(
                 torch.max(
-                    F.mse_loss(vs_pred, vs_teacher, reduction="none"),
-                    F.mse_loss(clipped_vs_pred, vs_teacher, reduction="none"),
+                    F.mse_loss(vs_pred.squeeze(), vs_teacher, reduction="none"),
+                    F.mse_loss(clipped_vs_pred.squeeze(), vs_teacher, reduction="none"),
                 )
             )
         loss_entropy = -torch.mean(entropy)
 
         self.value_loss_record.append(float(loss_value_func))
         self.policy_loss_record.append(float(loss_policy))
         loss = (
```

### Comparing `textrl-0.2.15/textrl/dump.py` & `textrl-0.2.16/textrl/dump.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/textrl/environment.py` & `textrl-0.2.16/textrl/environment.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/textrl/evaluator.py` & `textrl-0.2.16/textrl/evaluator.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/textrl/trainer.py` & `textrl-0.2.16/textrl/trainer.py`

 * *Files identical despite different names*

### Comparing `textrl-0.2.15/textrl.egg-info/PKG-INFO` & `textrl-0.2.16/textrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textrl
-Version: 0.2.15
+Version: 0.2.16
 Summary: TextRL - use reinforcement learning to adjust text generation results.
 Home-page: https://github.com/voidful/TextRL
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: transformer huggingface nlp generation reinforcement learning deep learning
 Platform: UNKNOWN
```

