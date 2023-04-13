# Comparing `tmp/torch_simple_timing-0.1.1.tar.gz` & `tmp/torch_simple_timing-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_simple_timing-0.1.1.tar", max compression
+gzip compressed data, was "torch_simple_timing-0.1.2.tar", max compression
```

## Comparing `torch_simple_timing-0.1.1.tar` & `torch_simple_timing-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.1/LICENSE
--rw-r--r--   0        0        0     2184 2023-04-12 22:55:21.554921 torch_simple_timing-0.1.1/README.md
--rw-r--r--   0        0        0      648 2023-04-12 23:03:08.880583 torch_simple_timing-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      825 2023-04-12 22:55:21.558606 torch_simple_timing-0.1.1/torch_simple_timing/__init__.py
--rw-r--r--   0        0        0     8293 2023-04-12 22:55:21.559088 torch_simple_timing-0.1.1/torch_simple_timing/clock.py
--rw-r--r--   0        0        0    13131 2023-04-12 22:55:21.559797 torch_simple_timing-0.1.1/torch_simple_timing/timer.py
--rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.1/torch_simple_timing/utils.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.1/setup.py
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3354 2023-04-13 15:09:59.550673 torch_simple_timing-0.1.2/README.md
+-rw-r--r--   0        0        0      648 2023-04-13 15:06:02.423029 torch_simple_timing-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      841 2023-04-12 23:05:33.657687 torch_simple_timing-0.1.2/torch_simple_timing/__init__.py
+-rw-r--r--   0        0        0     8293 2023-04-12 22:55:21.559088 torch_simple_timing-0.1.2/torch_simple_timing/clock.py
+-rw-r--r--   0        0        0    13141 2023-04-13 15:05:18.652967 torch_simple_timing-0.1.2/torch_simple_timing/timer.py
+-rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.2/torch_simple_timing/utils.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.2/setup.py
+-rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.2/PKG-INFO
```

### Comparing `torch_simple_timing-0.1.1/LICENSE` & `torch_simple_timing-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.1/pyproject.toml` & `torch_simple_timing-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-simple-timing"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple package to time CPU/GPU/Multi-GPU ops"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_simple_timing"}]
 
 [tool.poetry.dependencies]
```

### Comparing `torch_simple_timing-0.1.1/torch_simple_timing/__init__.py` & `torch_simple_timing-0.1.2/torch_simple_timing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 2. "*I want to time the same operations multiple times*"
 
    * That's what a :class:`~torch_simple_timing.timer.Timer` is for
 
 In simple terms:
 
-* A :class:`~torch_simple_timing.clock.Clock` is an object (and context-manager) that will compute the elapsed
-    time between its :meth:`~torch_simple_timing.clock.Clock.start()` (or :meth:`~torch_simple_timing.clock.Clock.__enter__`) and :meth:`~torch_simple_timing.clock.Clock.stop()` (or :meth:`~torch_simple_timing.clock.Clock.__exit__`)
-* A :class:`~torch_simple_timing.timer.Timer` will internally manage clocks so that you can focus on readability
-    and not data structures
+* A :class:`~torch_simple_timing.clock.Clock` is an object (and context-manager) that
+    will compute the elapsed
+    time between its :meth:`~torch_simple_timing.clock.Clock.start()`
+    (or :meth:`~torch_simple_timing.clock.Clock.__enter__`) and
+    :meth:`~torch_simple_timing.clock.Clock.stop()`
+    (or :meth:`~torch_simple_timing.clock.Clock.__exit__`)
+* A :class:`~torch_simple_timing.timer.Timer` will internally manage clocks so that you
+    can focus on readability and not data structures
 
 """
 from .clock import Clock  # noqa: F401
 from .timer import Timer  # noqa: F401
```

### Comparing `torch_simple_timing-0.1.1/torch_simple_timing/clock.py` & `torch_simple_timing-0.1.2/torch_simple_timing/clock.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.1/torch_simple_timing/timer.py` & `torch_simple_timing-0.1.2/torch_simple_timing/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from torch_simple_timing import Timer
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     gpu = device.type == "cuda"
     timer = Timer(gpu=gpu)
 
     # manual start
-    timer.mark("init").start()
+    timer.clock("init").start()
 
     batches = 32
     bs = 64
     n = batches * bs
     dim = 64
     labels = 10
     hidden = 1024
@@ -64,28 +64,28 @@
         Linear(hidden, hidden),
         ReLU(),
         Linear(hidden, labels),
     ).to(device)
     optimizer = torch.optim.Adam(model.parameters())
     loss_func = torch.nn.CrossEntropyLoss()
 
-    timer.mark("init").stop()
+    timer.clock("init").stop()
 
-    with timer.mark("train-loop"):
+    with timer.clock("train-loop"):
         for epoch in range(epochs):
-            with timer.mark("train-epoch"):
+            with timer.clock("train-epoch"):
                 for batch in range(batches):
                     optimizer.zero_grad()
                     # only time the first 2 epochs
-                    with timer.mark("train-batch", ignore=epoch > 2):
-                        with timer.mark("forward"):
+                    with timer.clock("train-batch", ignore=epoch > 2):
+                        with timer.clock("forward"):
                             pred = model(t[batch * bs : (batch + 1) * bs])
-                        with timer.mark("loss", ignore=epoch > 2):
+                        with timer.clock("loss", ignore=epoch > 2):
                             loss = loss_func(pred, y[batch * bs : (batch + 1) * bs])
-                        with timer.mark("backward", ignore=epoch > 2):
+                        with timer.clock("backward", ignore=epoch > 2):
                             loss.backward()
                         optimizer.step()
 
                     if batch % 10 == 0:
                         print(f"Epoch {epoch}, batch {batch}, loss {loss.item():.3f}")
 
     # compute mean/std stats for each clock in the timer
@@ -155,15 +155,15 @@
             self.times = {}
             self.clocks = {}
         else:
             for k in keys:
                 self.times.pop(k, None)
                 self.clocks.pop(k, None)
 
-    def mark(
+    def clock(
         self,
         name: str,
         ignore: Optional[bool] = None,
         gpu: Optional[bool] = None,
     ) -> Clock:
         """
         Create a new ``Clock`` object with name ``name`` and add it to the ``Timer``.
@@ -178,15 +178,15 @@
 
             If ``ignore`` is not ``None``, the ``Clock`` 's ``ignore`` attribute will be
             updated.
 
         .. warning::
 
             Don't forget to call ``.start()`` and ``.stop()`` on the returned ``Clock``
-            if you're not using ``timer.mark()`` as a context manager.
+            if you're not using ``timer.clock()`` as a context manager.
 
         Args:
             name (str): A name for the requested clock.
             ignore (Optional[bool], optional): Whether to ignore this clock and don't
                 time anything. This is useful in case timing slows you down (because of
                 :func:`torch.cuda.synchronize()` and :func:`torch.distributed.barrier()`) and
                 you only want to time the first epoch for instance. Defaults to
```

### Comparing `torch_simple_timing-0.1.1/torch_simple_timing/utils.py` & `torch_simple_timing-0.1.2/torch_simple_timing/utils.py`

 * *Files identical despite different names*

