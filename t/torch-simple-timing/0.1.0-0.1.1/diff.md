# Comparing `tmp/torch_simple_timing-0.1.0.tar.gz` & `tmp/torch_simple_timing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_simple_timing-0.1.0.tar", max compression
+gzip compressed data, was "torch_simple_timing-0.1.1.tar", max compression
```

## Comparing `torch_simple_timing-0.1.0.tar` & `torch_simple_timing-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.0/LICENSE
--rw-r--r--   0        0        0     2184 2023-04-12 22:55:21.554921 torch_simple_timing-0.1.0/README.md
--rw-r--r--   0        0        0      648 2023-04-12 22:55:21.558133 torch_simple_timing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      825 2023-04-12 22:55:21.558606 torch_simple_timing-0.1.0/torch_simple_timing/__init__.py
--rw-r--r--   0        0        0     8293 2023-04-12 22:55:21.559088 torch_simple_timing-0.1.0/torch_simple_timing/clock.py
--rw-r--r--   0        0        0    13131 2023-04-12 22:55:21.559797 torch_simple_timing-0.1.0/torch_simple_timing/timer.py
--rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.0/torch_simple_timing/utils.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.0/setup.py
--rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2184 2023-04-12 22:55:21.554921 torch_simple_timing-0.1.1/README.md
+-rw-r--r--   0        0        0      648 2023-04-12 23:03:08.880583 torch_simple_timing-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      825 2023-04-12 22:55:21.558606 torch_simple_timing-0.1.1/torch_simple_timing/__init__.py
+-rw-r--r--   0        0        0     8293 2023-04-12 22:55:21.559088 torch_simple_timing-0.1.1/torch_simple_timing/clock.py
+-rw-r--r--   0        0        0    13131 2023-04-12 22:55:21.559797 torch_simple_timing-0.1.1/torch_simple_timing/timer.py
+-rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.1/torch_simple_timing/utils.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.1/setup.py
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.1/PKG-INFO
```

### Comparing `torch_simple_timing-0.1.0/LICENSE` & `torch_simple_timing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/README.md` & `torch_simple_timing-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/pyproject.toml` & `torch_simple_timing-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "torch-simple-timing"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple package to time CPU/GPU/Multi-GPU ops"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_simple_timing"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 torch = ">=1.11"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 ipython = "^8.12.0"
 sphinx = "^6.1.3"
 myst-parser = "^1.0.0"
```

### Comparing `torch_simple_timing-0.1.0/torch_simple_timing/__init__.py` & `torch_simple_timing-0.1.1/torch_simple_timing/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/torch_simple_timing/clock.py` & `torch_simple_timing-0.1.1/torch_simple_timing/clock.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/torch_simple_timing/timer.py` & `torch_simple_timing-0.1.1/torch_simple_timing/timer.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/torch_simple_timing/utils.py` & `torch_simple_timing-0.1.1/torch_simple_timing/utils.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.0/setup.py` & `torch_simple_timing-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.11']
 
 setup_kwargs = {
     'name': 'torch-simple-timing',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
     'long_description': '# Torch Simple Timing\n\nA simple yet versatile package to time CPU/GPU/Multi-GPU ops.\n\n1. "*I want to time operations once*"\n   1. That\'s what a `Clock` is for\n2. "*I want to time the same operations multiple times*"\n   1. That\'s what a `Timer` is for\n\nIn simple terms:\n\n* A `Clock` is an object (and context-manager) that will compute the ellapsed time between its `start()` (or `__enter__`) and `stop()` (or `__exit__`)\n* A `Timer` will internally manage clocks so that you can focus on readability and not data structures\n\n## Installation\n\n```\npip install torch_simple_timing\n```\n\n## How to use\n\n### A `Clock`\n\n```python\nfrom torch_simple_parsing import Clock\nimport torch\n\nt = torch.rand(2000, 2000)\ngpu = torch.cuda.is_available()\n\nwith Clock(gpu=gpu) as context_clock:\n    torch.inverse(t @ t.T)\n\nclock = Clock(gpu=gpu).start()\ntorch.inverse(t @ t.T)\nclock.stop()\n\nprint(context_clock.duration) # 0.29688501358032227\nprint(clock.duration)         # 0.292896032333374\n```\n\nMore examples, including bout how to easily share data structures using a `store` can be found in the [documentation]().\n\n### A `Timer`\n\n```python\nfrom torch_simple_timing import Timer\nimport torch\n\ndevice = torch.device("cuda" if torch.cuda.is_available() else "cpu")\n\nX = torch.rand(5000, 5000, device=device)\nY = torch.rand(5000, 100, device=device)\nmodel = torch.nn.Linear(5000, 100).to(device)\noptimizer = torch.optim.Adam(model.parameters())\n\ngpu = device.type == "cuda"\ntimer = Timer(gpu=gpu)\n\nfor epoch in range(10):\n    timer.mark("epoch").start()\n    for b in range(50):\n        x = X[b*100: (b+1)*100]\n        y = Y[b*100: (b+1)*100]\n        optimizer.zero_grad()\n        with timer.mark("forward", ignore=epoch>0):\n            p = model(x)\n        loss = torch.nn.functional.cross_entropy(p, y)\n        with timer.mark("backward", ignore=epoch>0):\n            loss.backward()\n        optimizer.step()\n    timer.mark("epoch").stop()\n\nstats = timer.stats()\n# use stats for display and/or logging\n# wandb.summary.update(stats)\nprint(timer.display(stats=stats, precision=5))\n```\n\n```\nepoch    : 0.25064 ± 0.02728 (n=10)\nforward  : 0.00226 ± 0.00526 (n=50)\nbackward : 0.00209 ± 0.00387 (n=50)\n```\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `torch_simple_timing-0.1.0/PKG-INFO` & `torch_simple_timing-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: torch-simple-timing
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple package to time CPU/GPU/Multi-GPU ops
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: torch (>=1.11)
 Description-Content-Type: text/markdown
 
 # Torch Simple Timing
```

