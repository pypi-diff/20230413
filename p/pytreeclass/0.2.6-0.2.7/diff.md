# Comparing `tmp/pytreeclass-0.2.6.tar.gz` & `tmp/pytreeclass-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.2.6.tar", last modified: Mon Apr 10 21:31:08 2023, max compression
+gzip compressed data, was "pytreeclass-0.2.7.tar", last modified: Thu Apr 13 18:00:40 2023, max compression
```

## Comparing `pytreeclass-0.2.6.tar` & `pytreeclass-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28366 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25031 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.423071 pytreeclass-0.2.6/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28366 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-10 21:31:08.000000 pytreeclass-0.2.6/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:31:08.427071 pytreeclass-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-10 21:30:57.000000 pytreeclass-0.2.6/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29181 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28305 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.141738 pytreeclass-0.2.7/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29181 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 18:00:40.000000 pytreeclass-0.2.7/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:40.145738 pytreeclass-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17430 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-13 18:00:30.000000 pytreeclass-0.2.7/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.2.6/LICENSE` & `pytreeclass-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/PKG-INFO` & `pytreeclass-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.6
+Version: 0.2.7
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -294,42 +294,66 @@
 
 Parameters are defined in `Tree` at the top of class definition similar to defining
 `dataclasses.dataclass` field.
 Lets optimize our parameters
 
 ```python
 
+import pytreeclass as pytc
+import jax
+import jax.numpy as jnp
+
+
+@pytc.treeclass
+class Tree:
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
+
+    def __call__(self, x):
+        return self.a + self.b[0] + self.c + x
+
+
+tree = Tree()
+
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
     # apply a small gradient step
-    return jax.tree_util.tree_map(lambda x, g: x - 1e-3*g, tree, grads)
+    return jax.tree_util.tree_map(lambda x, g: x - 1e-3 * g, tree, grads)
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-#Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
-tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
+tree = jaxable_tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+# the previous line is equivalent to:
+# >>> tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
 # Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+
 ```
 
 </details>
 
 #### ☝️ Advanced Indexing with `.at[]` <a id="Indexing">
 
 <details> <summary>Out-of-place updates using mask, attribute name or index</summary>
@@ -545,56 +569,65 @@
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
 
 ```python
 import functools as ft
 import pytreeclass as pytc
+import jax
+import jax.tree_util as jtu
+import jax.numpy as jnp
+
 
 @ft.partial(pytc.treeclass, leafwise=True)
 class Tree:
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
 
 tree + 100
 # Tree(a=101, b=(102.0, 103.0), c=f32[3](μ=105.00, σ=0.82, ∈[104.00,106.00]))
 
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = jtu.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
-    return tree - grads*1e-3  # <--- eliminate `tree_map`
+    return tree - grads * 1e-3  # <--- eliminate `tree_map`
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-# Tree(a=#1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
 tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
-# Tree(a=1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 ```
 
 </details>
 
 <details> <summary>Eliminate tree_map using bcmap + treeclass(..., leafwise=True) </summary>
 
 TDLR
@@ -952,14 +985,15 @@
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
+<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
 
 `**` Always frozen. non-frozen is not supported.
```

### Comparing `pytreeclass-0.2.6/README.md` & `pytreeclass-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -271,42 +271,66 @@
 
 Parameters are defined in `Tree` at the top of class definition similar to defining
 `dataclasses.dataclass` field.
 Lets optimize our parameters
 
 ```python
 
+import pytreeclass as pytc
+import jax
+import jax.numpy as jnp
+
+
+@pytc.treeclass
+class Tree:
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
+
+    def __call__(self, x):
+        return self.a + self.b[0] + self.c + x
+
+
+tree = Tree()
+
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
     # apply a small gradient step
-    return jax.tree_util.tree_map(lambda x, g: x - 1e-3*g, tree, grads)
+    return jax.tree_util.tree_map(lambda x, g: x - 1e-3 * g, tree, grads)
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-#Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
-tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
+tree = jaxable_tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+# the previous line is equivalent to:
+# >>> tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
 # Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+
 ```
 
 </details>
 
 #### ☝️ Advanced Indexing with `.at[]` <a id="Indexing">
 
 <details> <summary>Out-of-place updates using mask, attribute name or index</summary>
@@ -522,56 +546,65 @@
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
 
 ```python
 import functools as ft
 import pytreeclass as pytc
+import jax
+import jax.tree_util as jtu
+import jax.numpy as jnp
+
 
 @ft.partial(pytc.treeclass, leafwise=True)
 class Tree:
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
 
 tree + 100
 # Tree(a=101, b=(102.0, 103.0), c=f32[3](μ=105.00, σ=0.82, ∈[104.00,106.00]))
 
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = jtu.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
-    return tree - grads*1e-3  # <--- eliminate `tree_map`
+    return tree - grads * 1e-3  # <--- eliminate `tree_map`
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-# Tree(a=#1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
 tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
-# Tree(a=1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 ```
 
 </details>
 
 <details> <summary>Eliminate tree_map using bcmap + treeclass(..., leafwise=True) </summary>
 
 TDLR
@@ -929,14 +962,15 @@
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
+<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
 
 `**` Always frozen. non-frozen is not supported.
```

### Comparing `pytreeclass-0.2.6/docs/conf.py` & `pytreeclass-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/pytreeclass/__init__.py` & `pytreeclass-0.2.7/pytreeclass/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 from pytreeclass._src.tree_decorator import field, fields, is_treeclass, treeclass
-from pytreeclass._src.tree_freeze import (
-    ImmutableWrapper,
-    freeze,
-    is_frozen,
-    is_nondiff,
-    unfreeze,
-)
+from pytreeclass._src.tree_freeze import freeze, is_frozen, is_nondiff, unfreeze
 from pytreeclass._src.tree_indexer import bcmap, is_tree_equal, tree_indexer
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
@@ -39,19 +33,18 @@
     "tree_summary",
     "tree_trace_summary",
     # freeze/unfreeze utils
     "is_nondiff",
     "is_frozen",
     "freeze",
     "unfreeze",
-    "ImmutableWrapper",
     # masking and indexing utils
     "bcmap",
     "tree_indexer",
     "register_pytree_node_trace",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
```

### Comparing `pytreeclass-0.2.6/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.2.7/pytreeclass/_src/tree_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import suppress
 from types import FunctionType, MappingProxyType
 from typing import Any, Callable, NamedTuple, Sequence, TypeVar
 
 import jax.tree_util as jtu
 from typing_extensions import dataclass_transform
 
-from pytreeclass._src.tree_freeze import ImmutableWrapper, tree_hash
+from pytreeclass._src.tree_freeze import tree_hash
 from pytreeclass._src.tree_indexer import (
     _conditional_mutable_method,
     _leafwise_transform,
     _mutable_context,
     is_tree_equal,
     tree_copy,
     tree_indexer,
@@ -21,27 +21,30 @@
 from pytreeclass._src.tree_pprint import tree_repr, tree_str
 from pytreeclass._src.tree_trace import register_pytree_node_trace
 
 _NOT_SET = type("NOT_SET", (), {"__repr__": lambda _: "?"})()
 _MUTABLE_TYPES = (list, dict, set)
 _ANNOTATIONS = "__annotations__"
 _POST_INIT = "__post_init__"
-_VARS = "__dict__"
-_FIELD_MAP = "__field_map__"
+_FIELDS = "__fields__"
 T = TypeVar("T")
 
 
 PyTree = Any
 
 """Define a class decorator that is compatible with JAX's transformation."""
 
 
-def is_treeclass(item: Any) -> bool:
-    """Returns `True` if an instance of class is decorated by `treeclass`"""
-    return hasattr(item, _FIELD_MAP)
+def is_treeclass(node: Any) -> bool:
+    """Returns `True` if class or instance is a `treeclass`."""
+    # use `_setattr` as a proxy for `treeclass` as overriding `__setattr__
+    # or `__delattr__` is not allowed, this behavior is similar
+    # to `dataclasses.dataclass(frozen=True)` restriction.
+    klass = node if isinstance(node, type) else type(node)
+    return getattr(klass, "__setattr__", None) is _setattr
 
 
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
     default: Any = _NOT_SET
     factory: Any = None
@@ -50,15 +53,34 @@
     kw_only: bool = False
     pos_only: bool = False
     metadata: MappingProxyType[str, Any] | None = None
     callbacks: Sequence[Any] = ()
     alias: str | None = None
 
     def __hash__(self) -> int:
-        return tree_hash(self)
+        # since `_generate_init_code` is caching the `fields`, then it is better
+        # only hash arguments that are used in generating the init code string
+        # this is avoid rewrtining the same final init code string multiple times.
+        return tree_hash(
+            (
+                self.name,
+                self.default,
+                self.factory,
+                self.init,
+                self.kw_only,
+                self.pos_only,
+                self.alias,
+            )
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        return hash(self) == hash(other)
+
+    def __repr__(self) -> str:
+        return tree_repr(self)
 
 
 def field(
     *,
     default: Any = _NOT_SET,
     factory: Callable | None = None,
     init: bool = True,
@@ -159,18 +181,18 @@
         callbacks=callbacks,
         alias=alias,
     )
 
 
 def fields(item: Any) -> Sequence[Field]:
     """Get the fields of a `treeclass` instance."""
-    if not hasattr(item, _FIELD_MAP):
+    if not hasattr(item, _FIELDS):
         raise TypeError(f"Cannot get fields of {item!r}.")
 
-    return tuple(vars(item)[_FIELD_MAP].values())
+    return tuple(vars(item)[_FIELDS].values())
 
 
 @ft.lru_cache
 def _generate_field_map(klass: type) -> dict[str, Field]:
     # get all the fields of the class and its base classes
     # get the fields of the class and its base classes
     field_map = dict()
@@ -192,15 +214,15 @@
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
     if _ANNOTATIONS not in vars(klass):
         return field_map
 
     for name in (annotation_map := vars(klass)[_ANNOTATIONS]):
         # get the value associated with the type hint
         # in essence will skip any non type-hinted attributes
-        value = getattr(klass, name, _NOT_SET)
+        value = vars(klass).get(name, _NOT_SET)
         # at this point we stick to the type hint provided by the user
         # inconsistency between the type hint and the value will be handled later
         type = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
             # and not recommended. so raise an error
@@ -298,39 +320,34 @@
     body = "\tdef __init__(self, " + head[:-2] + "):\n" + body
     # use closure to be able to reference default values of all types
     body = f"def closure(field_map):\n{body}\n\treturn __init__"
     return body.expandtabs(4)
 
 
 def _generate_init(klass: type) -> FunctionType:
-    # generate the field map for the class
     field_map = _generate_field_map(klass)
-    # generate init method
     local_namespace = dict()  # type: ignore
     global_namespace = vars(sys.modules[klass.__module__])
-
-    # generate the init method code string
-    # in here, we generate the function head and body and add `default`/`factory`
-    exec(_generate_init_code(field_map.values()), global_namespace, local_namespace)
+    init_code = _generate_init_code(tuple(field_map.values()))
+    exec(init_code, global_namespace, local_namespace)
     method = local_namespace["closure"](field_map)
 
-    # inject the method into the class namespace
     return FunctionType(
         code=method.__code__,
         globals=global_namespace,
         name=method.__name__,
         argdefs=method.__defaults__,
         closure=method.__closure__,
     )
 
 
 @_conditional_mutable_method
 def _setattr(tree: PyTree, key: str, value: Any) -> None:
     # setattr under `_mutable_context` context otherwise raise an error
-    if key in (field_map := vars(tree)[_FIELD_MAP]):
+    if key in (field_map := vars(tree)[_FIELDS]):
         # apply the callbacks on setting the value
         # check if the key is a field name
         for callback in field_map[key].callbacks:
             try:
                 # callback is a function that takes the value of the field
                 # and returns a modified value
                 value = callback(value)
@@ -340,16 +357,16 @@
 
     if is_treeclass(value):
         # auto registers the instance value if it is a registered `treeclass`
         # this behavior is similar to PyTorch behavior in `nn.Module`
         # with instances of `Parameter`/`Module`.
         # the behavior is useful to avoid repetitive code pattern in field definition and
         # and initialization inside init method.
-        F = Field(type=type(value), init=False, name=key)
-        vars(tree)[_FIELD_MAP] = {**vars(tree)[_FIELD_MAP], **{key: F}}
+        kv = {key: Field(type=type(value), init=False, name=key)}
+        vars(tree)[_FIELDS] = MappingProxyType({**vars(tree)[_FIELDS], **kv})
 
     vars(tree)[key] = value  # type: ignore
 
 
 @_conditional_mutable_method
 def _delattr(tree, key: str) -> None:
     # delete the attribute under `_mutable_context` context
@@ -357,24 +374,25 @@
     del vars(tree)[key]
 
 
 def _init_wrapper(init_func: Callable) -> Callable:
     @ft.wraps(init_func)
     def wrapper(tree, *a, **k) -> None:
         with _mutable_context(tree):
-            vars(tree)[_FIELD_MAP] = dict(_generate_field_map(type(tree)))
+            kvs = dict(_generate_field_map(type(tree)))
+            vars(tree)[_FIELDS] = MappingProxyType(kvs)
             output = init_func(tree, *a, **k)
 
             if post_init_func := getattr(type(tree), _POST_INIT, None):
                 # to simplify the logic, we call the post init method
                 # even if the init method is not code-generated.
                 post_init_func(tree)
 
         # handle non-initialized fields
-        if len(keys := set(vars(tree)[_FIELD_MAP]) - set(vars(tree))) > 0:
+        if len(keys := set(kvs) - set(vars(tree))) > 0:
             msg = f"Uninitialized fields: ({', '.join(keys)}) "
             msg += f"in class `{type(tree).__name__}`"
             raise AttributeError(msg)
         return output
 
     return wrapper
 
@@ -392,15 +410,15 @@
     vars(tree).update(zip(treedef[0], leaves))
     return tree
 
 
 def _tree_flatten(tree: PyTree):
     """Flatten rule for `treeclass` to use with `jax.tree_flatten`."""
     static, dynamic = dict(vars(tree)), dict()
-    for key in static[_FIELD_MAP]:
+    for key in static[_FIELDS]:
         dynamic[key] = static.pop(key)
     return list(dynamic.values()), (tuple(dynamic.keys()), static)
 
 
 def _tree_trace(tree: PyTree) -> list[tuple[Any, Any, Any, Any]]:
     """Trace flatten rule to be used with the `tree_trace` module."""
     leaves, (keys, _) = _tree_flatten(tree)
@@ -424,55 +442,14 @@
         register_pytree_node_trace(klass, _tree_trace)
         # register the flatten/unflatten rules with jax
         jtu.register_pytree_node(klass, _tree_flatten, ft.partial(_tree_unflatten, klass))  # type: ignore
 
     return klass
 
 
-def _tree_unwrap(value: Any) -> Any:
-    # enables the transparent wrapper behavior iniside `treeclass` wrapped classes
-    def is_leaf(x: Any) -> bool:
-        return isinstance(x, ImmutableWrapper) or is_treeclass(x)
-
-    def unwrap(value: Any) -> Any:
-        return value.unwrap() if isinstance(value, ImmutableWrapper) else value
-
-    return jtu.tree_map(unwrap, value, is_leaf=is_leaf)
-
-
-def _getattribute_wrapper(getattribute_method: Callable[[T, str], Any]):
-    # this current approach replaces the older metdata based approach
-    # that is used in `dataclasses`-based libraries like `flax.struct.dataclass` and v0.1 of `treeclass`.
-    # the metadata approach is defined at class variable and can not be changed at runtime while the current
-    # approach is more flexible because it can be changed at runtime using `tree_map` or by using `at`
-    # moreover, metadata-based approach falls short when handling nested data structures values.
-    # for example if a field value is a tuple of (1, 2, 3), then metadata-based approach will only be able
-    # to freeze the whole tuple, but not its elements.
-    # with the current approach, we can use `tree_map`/ or direct application to freeze certain tuple elements
-    # and leave the rest of the tuple as is.
-    # another pro of the current approach is that the field metadata is not checked during flattening/unflattening
-    # so in essence, it's more efficient than the metadata-based approach during applying `jax` transformations
-    # that flatten/unflatten the tree.
-    # Example: when fetching `tree.a` it will be unwrapped
-    # >>> @pytc.treeclass
-    # ... class Tree:
-    # ...    a:int = pytc.freeze(1)
-    # >>> tree = Tree()
-    # >>> tree
-    # Tree(a=#1)  # frozen value is displayed in the repr with a prefix `#`
-    # >>> tree.a
-    # 1  # the value is unwrapped when accessed directly
-    @ft.wraps(getattribute_method)
-    def wrapper(tree, key: str) -> Any:
-        value = getattribute_method(tree, key)
-        return _tree_unwrap(value) if key in getattribute_method(tree, _VARS) else value
-
-    return wrapper
-
-
 def _init_subclass_wrapper(init_subclass_method: Callable) -> Callable:
     # Non-decorated subclasses uses the base `treeclass` leaves only
     # this behavior is aligned with `dataclasses` not registering non-decorated
     # subclasses dataclass fields. for example:
     # >>> @treeclass
     # ... class A:
     # ...   a:int=1
@@ -516,18 +493,17 @@
     if "__init__" not in vars(klass):
         # generate the init method in case it is not defined by the user
         setattr(klass, "__init__", _generate_init(klass))
 
     for key, wrapper in (
         ("__init__", _init_wrapper),
         ("__init_subclass__", _init_subclass_wrapper),
-        ("__getattribute__", _getattribute_wrapper),
     ):
-        # wrappers to enable the field initialization,
-        # callback functionality and transparent wrapper behavior
+        # wrappers to enable the field initialization, and registering
+        # the class with jax
         setattr(klass, key, wrapper(getattr(klass, key)))
 
     # basic optional methods
     for key, method in (
         ("__repr__", tree_repr),
         ("__str__", tree_str),
         ("__copy__", tree_copy),
@@ -539,15 +515,15 @@
             # keep the original method if it is defined by the user
             # this behavior similar is to `dataclasses.dataclass`
             setattr(klass, key, method)
 
     return klass
 
 
-@dataclass_transform(field_specifiers=(field, Field))
+@dataclass_transform(field_specifiers=(field, Field), frozen_default=True)
 def treeclass(klass: type[T], *, leafwise: bool = False) -> type[T]:
     """Convert a class to a JAX compatible tree structure.
 
     Args:
         klass: class to be converted to a `treeclass`
         leafwise: Wether to generate leafwise math operations methods. Defaults to `False`.
```

### Comparing `pytreeclass-0.2.6/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.2.7/pytreeclass/_src/tree_freeze.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,77 +25,43 @@
 
 
 def tree_hash(tree: PyTree) -> int:
     hashed = jtu.tree_map(_hash_node, jtu.tree_leaves(tree))
     return hash((*hashed, jtu.tree_structure(tree)))
 
 
-class ImmutableWrapper:
-    """Base class for all immutable wrappers that gets a special treatment inside `treeclass` wrapped classes.
-    In essence, this wrapper is rendered transparent inside `treeclass` wrapped classes
-    so that the wrapped value can be accessed directly, without the need to call `unwrap`.
-    This behavior is useful for myriads of use cases, such as freezing a value to avoid updating it
-    by `jax` transformations, or wrapping a value to make it hashable.
-
-    Example:
-        >>> import jax.tree_util as jut
-        >>> import pytreeclass as pytc
-        >>> @jtu.register_pytree_node_class
-        ... class TransparentWrapper(pytc.ImmutableWrapper):
-        ...    def __repr__(self):
-        ...        return f"TransparentWrapper({self.__wrapped__!r})"
-        ...    def tree_flatten(self):
-        ...        # return the unwrapped value as a tuple
-        ...        return (self.unwrap(),), None
-        ...    @classmethod
-        ...    def tree_unflatten(cls, _, xs):
-        ...        return TransparentWrapper(xs[0])
-
-        >>> @pytc.treeclass
-        ... class Tree:
-        ...    a:int = TransparentWrapper(1)
-        >>> tree = Tree()
-        >>> # no need to unwrap the value when accessing it
-        >>> assert type(tree.a)  is int
-        >>> print(tree)
-        Tree(a=TransparentWrapper(1))
-        >>> jtu.tree_leaves(tree)
-        [1]
-        >>> jtu.tree_leaves(tree, is_leaf=lambda x: isinstance(x, TransparentWrapper))
-        [TransparentWrapper(1)]
-    """
-
+class _ImmutableWrapper:
     def __init__(self, x: Any) -> None:
         # disable composition of Wrappers
-        vars(self)[_WRAPPED] = x.unwrap() if isinstance(x, ImmutableWrapper) else x
+        vars(self)[_WRAPPED] = x.unwrap() if isinstance(x, _ImmutableWrapper) else x
 
     def unwrap(self) -> Any:
         return getattr(self, _WRAPPED)
 
     def __setattr__(self, _, __) -> None:
         raise AttributeError("Cannot assign to frozen instance.")
 
     def __delattr__(self, _: str) -> None:
         raise AttributeError("Cannot delete from frozen instance.")
 
 
-class _HashableWrapper(ImmutableWrapper):
+class _HashableWrapper(_ImmutableWrapper):
     # used to wrap metadata to make it hashable
     # this is intended to wrap frozen values to avoid error when comparing
     # the metadata.
     def __eq__(self, rhs: Any) -> bool:
         if not isinstance(rhs, _HashableWrapper):
             return False
         return _hash_node(self.unwrap()) == _hash_node(rhs.unwrap())
 
     def __hash__(self) -> int:
         return tree_hash(self.unwrap())
 
 
-class FrozenWrapper(ImmutableWrapper):
+class FrozenWrapper(_ImmutableWrapper):
     def __repr__(self):
         return f"#{self.unwrap()!r}"
 
     def __eq__(self, rhs: Any) -> bool:
         if not isinstance(rhs, FrozenWrapper):
             return False
         return self.unwrap() == rhs.unwrap()
@@ -140,14 +106,16 @@
         [101, #2, 103]
 
         >>> @pytc.treeclass
         ... class Test:
         ...     a: float
         ...     @jax.value_and_grad
         ...     def __call__(self, x):
+        ...         # unfreeze `a` to update it
+        ...         self = jax.tree_util.tree_map(pytc.unfreeze, self, is_leaf=pytc.is_frozen)
         ...         return x ** self.a
 
         >>> # without `freeze` wrapping `a`, `a` will be updated
         >>> value, grad = Test(a = 2.)(2.)
         >>> print(f"value: {value}\ngrad: {grad}")
         value: 4.0
         grad: Test(a=2.7725887)
@@ -176,15 +144,14 @@
 
     Example:
         >>> import pytreeclass as pytc
         >>> import jax.tree_util as jtu
         >>> frozen_value = pytc.freeze(1)
         >>> pytc.unfreeze(frozen_value)
         1
-
         >>> # usage with `jax.tree_map`
         >>> frozen_tree = jtu.tree_map(pytc.freeze, {"a": 1, "b": 2})
         >>> unfrozen_tree = jtu.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
         >>> unfrozen_tree
         {'a': 1, 'b': 2}
     """
     return x.unwrap() if isinstance(x, FrozenWrapper) else x
```

### Comparing `pytreeclass-0.2.6/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.2.7/pytreeclass/_src/tree_indexer.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.2.7/pytreeclass/_src/tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,16 @@
 ) -> str:
     if depth == 0:
         fmt = "..."
     else:
         kvs = node._asdict().items()
         fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
         fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
-    fmt = "namedtuple(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
+    name = type(node).__name__
+    fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
     return _format_width(fmt, width)
 
 
 def _dataclass_pprint(
     node: Any,
     indent: int,
     kind: PrintKind,
```

### Comparing `pytreeclass-0.2.6/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.2.7/pytreeclass/_src/tree_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,15 @@
 def register_pytree_node_trace(
     klass: type,
     trace_func: Callable[[Any], list[tuple[str, Any, tuple[int, int], Any]]],
 ) -> None:
     """
     Args:
         klass: The class of the object to be traced.
-        trace_func:
-            A function that takes an instance of type `klass` and defines the flatten rule
+        trace_func:A function that takes an instance of type `klass` and defines the flatten rule
             for the object (name, type, index, metadata) for each leaf in the object.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> class UserList(list):
         ...     pass
```

### Comparing `pytreeclass-0.2.6/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.2.7/pytreeclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.2.6
+Version: 0.2.7
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -294,42 +294,66 @@
 
 Parameters are defined in `Tree` at the top of class definition similar to defining
 `dataclasses.dataclass` field.
 Lets optimize our parameters
 
 ```python
 
+import pytreeclass as pytc
+import jax
+import jax.numpy as jnp
+
+
+@pytc.treeclass
+class Tree:
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
+
+    def __call__(self, x):
+        return self.a + self.b[0] + self.c + x
+
+
+tree = Tree()
+
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
     # apply a small gradient step
-    return jax.tree_util.tree_map(lambda x, g: x - 1e-3*g, tree, grads)
+    return jax.tree_util.tree_map(lambda x, g: x - 1e-3 * g, tree, grads)
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-#Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
-tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
+tree = jaxable_tree.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+# the previous line is equivalent to:
+# >>> tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
 # Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
+
 ```
 
 </details>
 
 #### ☝️ Advanced Indexing with `.at[]` <a id="Indexing">
 
 <details> <summary>Out-of-place updates using mask, attribute name or index</summary>
@@ -545,56 +569,65 @@
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
 
 ```python
 import functools as ft
 import pytreeclass as pytc
+import jax
+import jax.tree_util as jtu
+import jax.numpy as jnp
+
 
 @ft.partial(pytc.treeclass, leafwise=True)
 class Tree:
-    a:int = 1
-    b:tuple[float] = (2.,3.)
-    c:jax.Array = jnp.array([4.,5.,6.])
+    a: int = 1
+    b: tuple[float] = (2., 3.)
+    c: jax.Array = jnp.array([4., 5., 6.])
 
     def __call__(self, x):
         return self.a + self.b[0] + self.c + x
 
+
 tree = Tree()
 
 tree + 100
 # Tree(a=101, b=(102.0, 103.0), c=f32[3](μ=105.00, σ=0.82, ∈[104.00,106.00]))
 
+
 @jax.grad
-def loss_func(tree:Tree, x:jax.Array):
+def loss_func(tree: Tree, x: jax.Array):
+    tree = jtu.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)  # <--- unfreeze the tree before calling it
     preds = jax.vmap(tree)(x)  # <--- vectorize the tree call over the leading axis
     return jnp.mean(preds**2)  # <--- return the mean squared error
 
+
 @jax.jit
-def train_step(tree:Tree, x:jax.Array):
+def train_step(tree: Tree, x: jax.Array):
     grads = loss_func(tree, x)
-    return tree - grads*1e-3  # <--- eliminate `tree_map`
+    return tree - grads * 1e-3  # <--- eliminate `tree_map`
+
 
 # lets freeze the non-differentiable parts of the tree
 # in essence any non inexact type should be frozen to
 # make the tree differentiable and work with jax transformations
 jaxable_tree = jax.tree_util.tree_map(lambda x: pytc.freeze(x) if pytc.is_nondiff(x) else x, tree)
 
 for epoch in range(1_000):
-    jaxable_tree = train_step(jaxable_tree, jnp.ones([10,1]))
+    jaxable_tree = train_step(jaxable_tree, jnp.ones([10, 1]))
 
 print(jaxable_tree)
 # **the `frozen` params have "#" prefix**
-# Tree(a=#1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=#1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 
 
 # unfreeze the tree
 tree = jax.tree_util.tree_map(pytc.unfreeze, jaxable_tree, is_leaf=pytc.is_frozen)
 print(tree)
-# Tree(a=1, b=(-4.7176366, 3.0), c=[2.4973059 2.760783  3.024264 ])
+# Tree(a=1, b=(-4.2826524, 3.0), c=[2.3924797 2.905778  3.4190805])
 ```
 
 </details>
 
 <details> <summary>Eliminate tree_map using bcmap + treeclass(..., leafwise=True) </summary>
 
 TDLR
@@ -952,14 +985,15 @@
 <tr><td align="center">Generated eq method</td> <td align="center">✅✅*</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support slots</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Keyword-only args</td> <td align="center">✅</td>  <td align="center">✅ 3.10+</td></tr>
 <tr><td align="center">Positional-only args</td> <td align="center">✅</td>  <td align="center"></td></tr>
 <tr><td align="center">Frozen instance</td> <td align="center">✅**</td>  <td align="center">✅</td></tr>
 <tr><td align="center">Match args support</td> <td align="center"></td>  <td align="center">✅</td></tr>
 <tr><td align="center">Support callbacks</td> <td align="center">✅</td>  <td align="center"></td></tr>
+<tr><td align="center">Support alias name</td> <td align="center">✅</td>  <td align="center"></td></tr>
 </table>
 
 </div>
 
 `*` Either compare the whole instance and return `True/False` or treating it leafwise using `treeclass(..., leafwise=True)` and retrurn `Tree(a=True, ....)`
 
 `**` Always frozen. non-frozen is not supported.
```

### Comparing `pytreeclass-0.2.6/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.2.7/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/setup.py` & `pytreeclass-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/tests/test_indexing.py` & `pytreeclass-0.2.7/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/tests/test_nn.py` & `pytreeclass-0.2.7/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/tests/test_tree_freeze.py` & `pytreeclass-0.2.7/tests/test_tree_freeze.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,15 @@
         act: Callable = jax.nn.tanh
 
         def __call__(self, x):
             return self.act(x + self.a)
 
     @jax.value_and_grad
     def loss_func(model):
+        model = model.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
         return jnp.mean((model(1.0) - 0.5) ** 2)
 
     @jax.jit
     def update(model):
         value, grad = loss_func(model)
         return value, model - 1e-3 * grad
```

### Comparing `pytreeclass-0.2.6/tests/test_tree_operator.py` & `pytreeclass-0.2.7/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/tests/test_tree_pprint.py` & `pytreeclass-0.2.7/tests/test_tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,37 +52,37 @@
 r1 = Repr1()
 
 
 def test_repr():
     assert (
         tree_repr(r1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa', \n    b:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb', \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=namedtuple(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa', \n    b:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb', \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
     )
 
     assert (
         tree_repr(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=namedtuple(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[0], \n  o=c64[2]\n)"
     )
 
     assert tree_repr(r1, depth=0) == "Repr1(...)"
 
 
 def test_str():
     assert (
         tree_str(r1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa, \n    b:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb, \n    c:\n      [[1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]]\n  }, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=namedtuple(b=1, c=2), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa, \n    b:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb, \n    c:\n      [[1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]]\n  }, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(b=1, c=2), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
     )
 
     assert (
         tree_str(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=namedtuple(...), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(...), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
     )
 
 
 def test_tree_summary():
     assert (
         tree_summary(r1, depth=0)
         == "┌────┬─────┬─────┐\n│Name│Type │Count│\n├────┼─────┼─────┤\n│Σ   │Repr1│1    │\n└────┴─────┴─────┘"
@@ -106,15 +106,15 @@
     return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
 
 
 def test_tree_diagram():
     assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1"
 
     # trunk-ignore(flake8/E501)
-    out = "Repr1\n├── a=1\n├── b='string'\n├── c=1.0\n├── d='aaaaa'\n├── e=[...]\n├── f={...}\n├── g={...}\n├── h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── k=(...)\n├── l=namedtuple(...)\n├── m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── n=bool[0]\n└── o=c64[2]"
+    out = "Repr1\n├── a=1\n├── b='string'\n├── c=1.0\n├── d='aaaaa'\n├── e=[...]\n├── f={...}\n├── g={...}\n├── h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── k=(...)\n├── l=a(...)\n├── m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── n=bool[0]\n└── o=c64[2]"
 
     assert tree_diagram(r1, depth=1) == out
     assert tree_indent(r1, depth=1) == _tree_to_indent(out)
 
 
 def test_custom_jax_class():
     @jtu.register_pytree_node_class
@@ -147,15 +147,15 @@
     assert tree_str(Test) == str(Test)
 
 
 def test_tree_mermaid():
     assert (
         tree_mermaid(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=namedtuple(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[0]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
+        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e=[...]</b>")\n    id0 --- id6("</b>f={...}</b>")\n    id0 --- id7("</b>g={...}</b>")\n    id0 --- id8("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>k=(...)</b>")\n    id0 --- id12("</b>l=a(...)</b>")\n    id0 --- id13("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>n=bool[0]</b>")\n    id0 --- id15("</b>o=c64[2]</b>")\n'
     )
     assert (
         tree_mermaid(r1, depth=2)
         # trunk-ignore(flake8/E501)
         == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>[\'b\']=1</b>")\n    id23 --- id25("</b>[\'c\']=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>a=1</b>")\n    id0 --- id2("</b>b=\'string\'</b>")\n    id0 --- id3("</b>c=1.0</b>")\n    id0 --- id4("</b>d=\'aaaaa\'</b>")\n    id0 --- id5("</b>e:list</b>")\n    id0 --- id11("</b>f={1, 2, 3}</b>")\n    id0 --- id12("</b>g:dict</b>")\n    id0 --- id16("</b>h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>k:tuple</b>")\n    id0 --- id23("</b>l:a</b>")\n    id0 --- id26("</b>m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>n=bool[0]</b>")\n    id0 --- id28("</b>o=c64[2]</b>")\n'
     )
```

### Comparing `pytreeclass-0.2.6/tests/test_tree_viz_util.py` & `pytreeclass-0.2.7/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.2.6/tests/test_treeclass.py` & `pytreeclass-0.2.7/tests/test_treeclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,25 @@
 
 
 def test_field_metadata():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: int = pytc.field(default=1, metadata={"a": 1})
 
-    assert Test().__field_map__["a"].metadata["a"] == 1
+    assert Test().__fields__["a"].metadata["a"] == 1
+
+
+def test_is_treeclass():
+    @ft.partial(pytc.treeclass, leafwise=True)
+    class Test:
+        a: int = 1
+
+    assert pytc.is_treeclass(Test)
+    assert pytc.is_treeclass(Test())
+    assert not pytc.is_treeclass(int)
 
 
 def test_field_mutually_exclusive():
     with pytest.raises(ValueError):
         pytc.field(default=1, factory=lambda: 1)
 
     with pytest.raises(ValueError):
@@ -118,15 +128,17 @@
     assert tree._name == "test"
 
     with pytest.raises(TypeError):
         pytc.field(alias=1)
 
 
 def test_field_hash():
-    hash(pytc.field(default=1)) == hash(pytc.field(default=1))
+    f1 = pytc.field(default=1.0, callbacks=[lambda x: x])
+    f2 = pytc.field(default=1.0)
+    hash(f1) == hash(f2)
 
 
 def test_field_nondiff():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: jnp.ndarray
         b: jnp.ndarray
@@ -478,15 +490,15 @@
 def test_treeclass_frozen_field():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: int = pytc.field(callbacks=[pytc.freeze])
 
     t = Test(1)
 
-    assert t.a == 1
+    assert t.a == pytc.freeze(1)
     assert jtu.tree_leaves(t) == []
 
 
 def test_key_error():
     @ft.partial(pytc.treeclass, leafwise=True)
     class Test:
         a: int = pytc.field()
@@ -735,11 +747,19 @@
         def add_param(self, name, param):
             return setattr(self, name, param)
 
     tree = Tree()
 
     _, tree_with_weight = tree.at["add_param"]("weight", Parameter(3))
 
-    assert tree.__field_map__ != tree_with_weight.__field_map__
+    assert tree.__fields__ != tree_with_weight.__fields__
     assert tree_with_weight.weight == Parameter(3)
     assert "weight" not in vars(tree)
-    assert "weight" not in tree.__field_map__
+    assert "weight" not in tree.__fields__
+
+
+def test_field_repr():
+    assert (
+        repr(pytc.field())
+        # trunk-ignore(flake8/E501)
+        == "Field(\n  name=None, \n  type=None, \n  default=?, \n  factory=None, \n  init=True, \n  repr=True, \n  kw_only=False, \n  pos_only=False, \n  metadata=None, \n  callbacks=(), \n  alias=None\n)"
+    )
```

### Comparing `pytreeclass-0.2.6/tests/test_under_jit.py` & `pytreeclass-0.2.7/tests/test_under_jit.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     model = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jax.random.PRNGKey(0))
     x = jnp.linspace(0, 1, 100)[:, None]
     y = x**3 + jax.random.uniform(jax.random.PRNGKey(0), (100, 1)) * 0.01
 
     @jax.value_and_grad
     def loss_func(model, x, y):
+        model = model.at[...].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
         return jnp.mean((model(x) - y) ** 2)
 
     @jax.jit
     def update(model, x, y):
         value, grads = loss_func(model, x, y)
         return value, jtu.tree_map(lambda x, y: x - 1e-3 * y, model, grads)
```

