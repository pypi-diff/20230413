# Comparing `tmp/jaxrie-3.tar.gz` & `tmp/jaxrie-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-3.tar", last modified: Tue Apr 11 06:37:21 2023, max compression
+gzip compressed data, was "jaxrie-4.tar", last modified: Wed Apr 12 22:21:58 2023, max compression
```

## Comparing `jaxrie-3.tar` & `jaxrie-4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-3/README.md
--rw-r--r--   0        0        0     3959 2023-04-11 06:37:21.819071 jaxrie-3/pyproject.toml
--rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-3/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-11 06:36:55.909478 jaxrie-3/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-3/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-3/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-3/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-3/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-3/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-3/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-11 06:13:42.344173 jaxrie-3/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-3/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2342 2023-04-11 06:23:40.424342 jaxrie-3/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-3/src/jaxrie/py.typed
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-3/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-4/README.md
+-rw-r--r--   0        0        0     3959 2023-04-12 22:21:58.309314 jaxrie-4/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-4/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-12 22:20:31.621114 jaxrie-4/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-4/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-4/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-4/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-4/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-4/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-4/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-4/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-4/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-4/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-4/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-4/PKG-INFO
```

### Comparing `jaxrie-3/pyproject.toml` & `jaxrie-4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     "jaxlib>=0.4.6",
     "dm-haiku>=0.0.9",
     "optax>=0.1.4",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "3"
+version = "4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-3/src/jaxrie/manifold/base.py` & `jaxrie-4/src/jaxrie/manifold/base.py`

 * *Files identical despite different names*

### Comparing `jaxrie-3/src/jaxrie/manifold/lorentz.py` & `jaxrie-4/src/jaxrie/manifold/lorentz.py`

 * *Files identical despite different names*

### Comparing `jaxrie-3/src/jaxrie/manifold/math.py` & `jaxrie-4/src/jaxrie/manifold/math.py`

 * *Files identical despite different names*

### Comparing `jaxrie-3/src/jaxrie/manifold/stereographic.py` & `jaxrie-4/src/jaxrie/manifold/stereographic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-3/src/jaxrie/modules/basic.py` & `jaxrie-4/src/jaxrie/modules/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,124 +53,124 @@
 class HAct(hk.Module):
   """Hyperbolic Activation Layer."""
 
   def __init__(
       self,
       activation: Callable[[Array], Array],
       manifold: Manifold,
-      cin: ArrayLike | None = None,
-      cout: ArrayLike | None = None,
+      kin: ArrayLike | None = None,
+      kout: ArrayLike | None = None,
       name: str | None = None,
   ) -> None:
     """Initialize the layer."""
     super().__init__(name=name)
     self.m = manifold
     self.activation = activation
 
-    self.tcin = cin is None
-    self.tcout = cout is None
-    self.cin = -1.0 if self.tcin else cin
-    self.cout = -1.0 if self.tcout else cout
+    self.tkin = kin is None
+    self.tkout = kout is None
+    self.kin = -1.0 if self.tkin else kin
+    self.kout = -1.0 if self.tkout else kout
 
   def __call__(self, x: Array) -> Array:
     """Apply the layer."""
     dtype = x.dtype
-    self.cin = jnp.array(self.cin, dtype=dtype)
-    self.cout = jnp.array(self.cout, dtype=dtype)
-    if self.tcin:
-      self.cin = hk.get_parameter("cin", (), init=hk.initializers.Constant(self.cin))
-    if self.tcout:
-      self.cout = hk.get_parameter("cout", (), init=hk.initializers.Constant(self.cout))
+    self.kin = jnp.array(self.kin, dtype=dtype)
+    self.kout = jnp.array(self.kout, dtype=dtype)
+    if self.tkin:
+      self.kin = hk.get_parameter("kin", (), init=hk.initializers.Constant(self.kin))
+    if self.tkout:
+      self.kout = hk.get_parameter("kout", (), init=hk.initializers.Constant(self.kout))
 
     return self.m.proj(
-        self.m.expmap0(self.activation(self.m.logmap0(x, self.cin)), self.cout),
-        self.cout,
+        self.m.expmap0(self.activation(self.m.logmap0(x, self.kin)), self.kout),
+        self.kout,
     )
 
 
 class HLinear(hk.Module):
   """Hyperbolic Linear Layer."""
 
   def __init__(
       self,
       out_features: int,
       manifold: Manifold,
-      c: ArrayLike | None = None,
+      k: ArrayLike | None = None,
       with_bias: bool = True,
       w_init: hk.initializers.Initializer | None = None,
       b_init: hk.initializers.Initializer | None = None,
       name: str | None = None,
   ) -> None:
     """Initialize the layer."""
     super().__init__(name=name)
     self.out_features = out_features
     self.m = manifold
 
-    self.tc = c is None
-    self.c = -1.0 if c is None else c
+    self.tk = k is None
+    self.k = -1.0 if k is None else k
     self.w_init = w_init
     self.b_init = b_init or hk.initializers.Constant(0.0)
     self.with_bias = with_bias
 
   def __call__(self, x: Array) -> Array:
     """Apply the layer."""
     dtype = x.dtype
     input_size = self.input_size = x.shape[-1]
     w_init = self.w_init
 
-    self.c = jnp.array(self.c, dtype=dtype)
-    if self.tc:
-      self.c = hk.get_parameter("c", (), init=hk.initializers.Constant(self.c))
+    self.k = jnp.array(self.k, dtype=dtype)
+    if self.tk:
+      self.k = hk.get_parameter("k", (), init=hk.initializers.Constant(self.k))
 
     if w_init is None:
       stddev = 1.0 / jnp.sqrt(input_size)
       w_init = hk.initializers.TruncatedNormal(stddev=stddev)
     w = hk.get_parameter("w", [input_size, self.out_features], dtype, init=w_init)
 
-    out = self.m.proj(self.m.matmull(x, w, self.c), self.c)
+    out = self.m.proj(self.m.matmull(x, w, self.k), self.k)
 
     if self.with_bias:
       b = hk.get_parameter("b", [self.out_features], dtype, init=self.b_init)
-      out = self.m.proj(self.m.adde(out, b, self.c), self.c)
+      out = self.m.proj(self.m.adde(out, b, self.k), self.k)
 
     return out
 
 
 class HGCN(hk.Module):
   """Hyperbolic Graph Convolutional Network."""
 
   def __init__(
       self,
       out_features: int,
       manifold: Manifold,
-      c: ArrayLike | None = None,
+      k: ArrayLike | None = None,
       with_bias: bool = True,
       w_init: hk.initializers.Initializer | None = None,
       b_init: hk.initializers.Initializer | None = None,
       name: str | None = None,
   ) -> None:
     """Initialize the layer."""
     super().__init__(name=name)
     self.out_features = out_features
     self.m = manifold
 
-    self.tc = c is None
-    self.c = -1.0 if c is None else c
+    self.tk = k is None
+    self.k = -1.0 if k is None else k
     self.with_bias = with_bias
 
     w_init = w_init or hk.initializers.VarianceScaling(1.0, "fan_avg", "uniform")
 
     self.linear = HLinear(
         out_features,
         manifold,
-        c=c,
+        k=k,
         with_bias=with_bias,
         w_init=w_init,
         b_init=b_init,
         name="hlinear",
     )
 
   def __call__(self, x: Array, adj: Array) -> Array:
     """Apply the layer."""
     out = self.linear(x)
-    self.c = self.linear.c
-    return self.m.proj(self.m.matmulr(adj, out, self.c), self.c)
+    self.k = self.linear.k
+    return self.m.proj(self.m.matmulr(adj, out, self.k), self.k)
```

### Comparing `jaxrie-3/src/jaxrie/nets/basic.py` & `jaxrie-4/src/jaxrie/nets/basic.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,29 +53,27 @@
   """A simple MLP."""
 
   def __init__(
       self,
       layers: Sequence[int],
       manifold: Manifold,
       activation: Callable[[Array], Array] = jax.nn.relu,
-      c: ArrayLike | None = None,
+      k: ArrayLike | None = None,
       with_bias: bool = True,
       w_init: hk.initializers.Initializer | None = None,
       b_init: hk.initializers.Initializer | None = None,
       name: str | None = None,
   ) -> None:
     """Initialize the Hyperbolic MLP."""
     super().__init__(name=name)
     self.layers = list(
-        map(lambda o: HLinear(o, manifold, c, with_bias, w_init, b_init), layers)
+        map(lambda o: HLinear(o, manifold, k, with_bias, w_init, b_init), layers)
     )
     self.m = manifold
-    self.activation = HAct(activation, manifold, c, c)
-    self.tc = c is None
-    self.c = -1.0 if self.tc else c
+    self.activation = HAct(activation, manifold, k, k)
 
   def __call__(
       self, x: Array, dropout: float | None = None, train: bool = True
   ) -> Array:
     """Forward pass."""
     for layer in self.layers[:-1]:
       x = self.activation(layer(x))
```

