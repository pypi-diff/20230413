# Comparing `tmp/jaxrie-7.tar.gz` & `tmp/jaxrie-8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-7.tar", last modified: Thu Apr 13 02:13:07 2023, max compression
+gzip compressed data, was "jaxrie-8.tar", last modified: Thu Apr 13 18:34:57 2023, max compression
```

## Comparing `jaxrie-7.tar` & `jaxrie-8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-7/README.md
--rw-r--r--   0        0        0     3959 2023-04-13 02:13:07.887664 jaxrie-7/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-13 02:05:54.392649 jaxrie-7/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-13 02:12:42.523822 jaxrie-7/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-7/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4120 2023-04-13 02:10:13.893763 jaxrie-7/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     4749 2023-04-12 22:31:42.778318 jaxrie-7/src/jaxrie/manifold/euclidean.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-7/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-7/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-7/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-7/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-7/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-7/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-7/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-7/src/jaxrie/py.typed
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-7/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-8/README.md
+-rw-r--r--   0        0        0     3959 2023-04-13 18:34:57.659852 jaxrie-8/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-13 02:05:54.392649 jaxrie-8/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-13 18:34:34.058886 jaxrie-8/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-8/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4120 2023-04-13 02:10:13.893763 jaxrie-8/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     4567 2023-04-13 18:30:08.539578 jaxrie-8/src/jaxrie/manifold/euclidean.py
+-rw-r--r--   0        0        0     1434 2023-04-13 18:31:44.775171 jaxrie-8/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    21849 2023-04-13 18:31:44.712690 jaxrie-8/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5122 2023-04-13 18:30:08.411332 jaxrie-8/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-8/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4753 2023-04-13 17:54:44.533901 jaxrie-8/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-8/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-8/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-8/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-8/PKG-INFO
```

### Comparing `jaxrie-7/pyproject.toml` & `jaxrie-8/pyproject.toml`

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
-version = "7"
+version = "8"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-7/src/jaxrie/manifold/base.py` & `jaxrie-8/src/jaxrie/manifold/base.py`

 * *Files identical despite different names*

### Comparing `jaxrie-7/src/jaxrie/manifold/euclidean.py` & `jaxrie-8/src/jaxrie/manifold/euclidean.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,99 +42,99 @@
 Array = jax.Array
 
 
 class Euclidean(Manifold):
   """The universal Stereographic projection model."""
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold with curvature k."""
     del k, eps
     return x + y
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold (left H, right E) with curvature k."""
     return Euclidean.add(x, y, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def sub(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius subtraction on manifold with curvature k."""
     return Euclidean.add(x, -y, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def mul(r: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius multiplication on manifold with curvature k."""
     del k, eps
     return r * x
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matvec(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius matrix vector multiplication on manifold with curvature k."""
     del k, eps
     return m @ x
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmul(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius matrix multiplication on manifold with curvature k."""
     del k, eps
     return x1 @ x2
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmull(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left H, right E) with curvature k."""
     return Euclidean.matmul(x1, x2, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmulr(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left E, right H) with curvature k."""
     return Euclidean.matmul(x1, x2, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def expmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     del k, eps
     return x + y
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def logmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     del k, eps
     return y - x
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def expmap0(u: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     del k, eps
     return u
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def logmap0(y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     del k, eps
     return y
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Euclidean gradient to Riemannian gradient."""
     del x, k, eps
     return grad
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Projection on manifold with curvature k."""
     del k, eps
     return x
```

### Comparing `jaxrie-7/src/jaxrie/manifold/lorentz.py` & `jaxrie-8/src/jaxrie/manifold/lorentz.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,11 +44,11 @@
 Array = jax.Array
 
 
 class Lorentz(Manifold):
     """Lorentz model."""
 
     @staticmethod
-    @partial(jax.jit, inline=True)
+    @jax.jit
     def add(x: Array, y: Array, k: ArrayLike) -> Array:
         """Addition on manifold with curvature k."""
         pass
```

### Comparing `jaxrie-7/src/jaxrie/manifold/math.py` & `jaxrie-8/src/jaxrie/manifold/math.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 EPS = 1e-15
 HALF_EPS = 1e-7
 
 FN = TypeVar("FN", bound=Callable)
 
 
-@partial(jax.jit, static_argnames=("axis", "ids", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "ids", "keepdims"))
 def select_dim(
     x: Array,
     axis: int,
     ids: tuple[int | None, int | None, int | None] | int,
     keepdims: bool = True,
 ) -> Array:
   """Select the dim-th dimension of x."""
@@ -70,267 +70,265 @@
   axes = isinstance(ids, tuple) and slice(*ids) or ids
   idx = max(naxis, 0) * (slice(None),) + (axes,) + (x.ndim - naxis - 1) * (slice(None),)
   if keepdims:
     return x[idx][..., None]
   return x[idx]
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def safe_div(x: Array, y: Array, eps: float = EPS) -> Array:
   """Safe division."""
   return jnp.divide(x, jnp.maximum(y, eps))
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def safe_sqrt(x: Array, eps: float = EPS) -> Array:
   """Safe square root."""
   return jnp.sqrt(jnp.maximum(x, eps))
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def safe_arctanh(x: Array, eps: float = HALF_EPS) -> Array:
   """Safe arctanh."""
   return jnp.arctanh(jnp.clip(x, -1 + eps, 1 - eps))
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def radius(k: ArrayLike, eps: float = EPS) -> Array:
   """Radius with curvature k in ."""
   return jnp.reciprocal(safe_sqrt(jnp.abs(k), eps=eps))
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def origin(k: ArrayLike, eps: float = EPS) -> Array:
   """Origin of x."""
   return safe_sqrt(radius(k, eps=eps), eps=eps)
 
 
-@partial(jax.jit, static_argnames=("size",), inline=True)
+@partial(jax.jit, static_argnames=("size",))
 def sh_metric(size: int, k: ArrayLike = -1.0) -> Array:
   """SH metric.
 
   k < 0: Lorentz   -1, 1, 1, ...
   other: Euclidean  1, 1, 1, ...
   """
   return jnp.ones(size).at[0].set(jnp.sign(k))
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def sink(x: Array, k: ArrayLike) -> Array:
   """Sine function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
           lambda: jnp.sinh(x),
           lambda: jnp.sin(x),
       ),
   )
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def cosk(x: Array, k: ArrayLike) -> Array:
   """Cosine function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
           lambda: jnp.cosh(x),
           lambda: jnp.cos(x),
       ),
   )
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def tank(x: Array, k: ArrayLike) -> Array:
   """Tangent function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
           lambda: jnp.tanh(x),
           lambda: jnp.tan(x),
       ),
   )
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def arctank(x: Array, k: ArrayLike) -> Array:
   """Arctangent function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
-          lambda: jnp.arctanh(x),
+          lambda: safe_arctanh(x),
           lambda: jnp.arctan(x),
       ),
   )
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def arcsink(x: Array, k: ArrayLike) -> Array:
   """Arcsine function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
           lambda: jnp.arcsinh(x),
           lambda: jnp.arcsin(x),
       ),
   )
 
 
-@partial(jax.jit, inline=True)
+@jax.jit
 def arccosk(x: Array, k: ArrayLike) -> Array:
   """Arccosine function with curvature k."""
   k = jnp.asarray(k, dtype=x.dtype)
   return jax.lax.cond(
       k == 0,
       lambda: x,
       lambda: jax.lax.cond(
           k < 0,
           lambda: jnp.arccosh(x),
           lambda: jnp.arccos(x),
       ),
   )
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def lambda_x(x: Array, k: ArrayLike, axis: int = -1, keepdims: bool = False) -> Array:
   """Calculate the conformal factor."""
-  return 2 / (1 + k * sqnorm(x, axis=axis, keepdims=keepdims))
+  return safe_div(2, (1 + k * sqnorm(x, axis=axis, keepdims=keepdims)))
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def inner(x: Array, y: Array, axis: int = -1, keepdims: bool = False) -> Array:
   """Inner product of two vectors."""
   if x.ndim == 0:
     x = x[None]
   return jnp.sum(x * y, axis=axis, keepdims=keepdims)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def tangent_inner(
     x: Array, u: Array, v: Array, k: ArrayLike, axis: int = -1, keepdims: bool = False
 ) -> Array:
   """Inner product of two tangent vectors."""
   return (lambda_x(x, k, axis=axis, keepdims=keepdims) ** 2) * inner(
       u, v, axis=axis, keepdims=keepdims
   )
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def minkowski_inner(
     x: Array, y: Array, k: ArrayLike = -1.0, axis: int = -1, keepdims: bool = False
 ) -> Array:
   """Minkowski inner product of two vectors."""
   xy = x * y
   if xy.ndim == 0:
     xy = xy[None]
   g = sh_metric(xy.shape[axis], k=k)
   return jnp.sum(g * xy, axis=axis, keepdims=keepdims)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def sqnorm(x: Array, axis: int = -1, keepdims: bool = False) -> Array:
   """Squared norm of a vector."""
   if x.ndim == 1:
     x = x[None]
   return inner(x, x, axis=axis, keepdims=keepdims)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def tangent_sqnorm(
     x: Array, u: Array, k: ArrayLike, axis: int = -1, keepdims: bool = False
 ) -> Array:
   """Squared norm of a tangent vector."""
   return tangent_inner(x, u, u, k, axis=axis, keepdims=keepdims)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims"))
 def minkowski_sqnorm(
     x: Array, k: ArrayLike = -1.0, axis: int = -1, keepdims: bool = False
 ) -> Array:
   """Squared norm of a vector in Minkowski space."""
   if x.ndim == 1:
     x = x[None]
   return minkowski_inner(x, x, k=k, axis=axis, keepdims=keepdims)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"))
 def norm(x: Array, axis: int = -1, keepdims: bool = False, eps: float = EPS) -> Array:
   """Norm of a vector."""
   return safe_sqrt(sqnorm(x, axis=axis, keepdims=keepdims), eps=eps)
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"))
 def tangent_norm(
     x: Array,
     u: Array,
     k: ArrayLike,
     axis: int = -1,
     keepdims: bool = False,
     eps: float = EPS,
 ) -> Array:
   """Norm of a tangent vector."""
   return lambda_x(x, k, axis=axis, keepdims=keepdims) * norm(
       u, axis=axis, keepdims=keepdims, eps=eps
   )
 
 
-@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "keepdims", "eps"))
 def minkowski_norm(
     x: Array,
     k: ArrayLike = -1.0,
     axis: int = -1,
     keepdims: bool = False,
     eps: float = EPS,
 ) -> Array:
   """Norm of a vector in Minkowski space."""
   return safe_sqrt(minkowski_sqnorm(x, k=k, axis=axis, keepdims=keepdims), eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius addition of two vectors x.y in manifold with curvature k."""
   sqnx = k * sqnorm(x, axis=-1, keepdims=True)
   sqny = k * sqnorm(y, axis=-1, keepdims=True)
   xy = k * inner(x, y, axis=-1, keepdims=True)
   num = (1 - 2 * xy - sqny) * x + (1 + sqnx) * y
   denom = 1 - 2 * xy + sqnx * sqny
   return safe_div(num, denom, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius addition of two vectors x(in H) & y(in E) with curvature k."""
-  return stereo_expmap(
-      x, stereo_ptrans0(x, y, k, eps=eps), k, eps=eps
-  )
+  return stereo_expmap(x, stereo_ptrans0(x, y, k, eps=eps), k, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_scala_mul(alpha: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius multiplication of a vector by a scalar in manifold with curvature k."""
   c = radius(k, eps=eps)
   x_norm = norm(x, axis=-1, keepdims=True, eps=eps) / c
   return tank(alpha * arctank(x_norm, k), k) * x / x_norm
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_matvec_mul(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius multiplication of a matrix by a vector in manifold with curvature k."""
   if x.ndim > 1:
     raise ValueError("x must be a vector, use mobius_matmul instead.")
   axis = -1
   c = radius(k, eps=eps)
   x_norm = norm(x, axis=axis, keepdims=True, eps=eps)
@@ -345,23 +343,23 @@
           jnp.prod(mx == 0, axis=axis, keepdims=True),
           jnp.zeros_like(res),
           res,
       ),
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_matmulh(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius matrix multiplication in H with curvature k."""
   return stereo_expmap0(
       stereo_logmap0(x1, k, eps=eps) @ stereo_logmap0(x2, k, eps=eps), k, eps=eps
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_matmull(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius matrix multiplication (left H, right E) with curvature k."""
   axis = -1
   c = radius(k, eps=eps)
   x_norm = norm(x1, axis=axis, keepdims=True, eps=eps)
   xx = x1 @ x2
   xx_norm = norm(xx, axis=axis, keepdims=True, eps=eps)
@@ -374,15 +372,15 @@
           jnp.prod(xx == 0, axis=axis, keepdims=True),
           jnp.zeros_like(res),
           res,
       ),
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def mobius_matmulr(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius matrix multiplication (left H, right E) with curvature k."""
   # return stereo_expmap0(x1 @ stereo_logmap0(x2, k, eps=eps), k, eps=eps)
   axis = -1
   c = radius(k, eps=eps)
   x_norm = norm(x2.swapaxes(-1, -2), axis=axis, keepdims=True, eps=eps)
   xx = x2.swapaxes(-1, -2) @ x1.swapaxes(-1, -2)
@@ -397,203 +395,203 @@
           jnp.zeros_like(res),
           res,
       ),
   ).swapaxes(-1, -2)
 
 
 # TODO: implement mobius_left_matmul
-# @partial(jax.jit, static_argnames=("eps",), inline=True)
+# @partial(jax.jit, static_argnames=("eps",))
 def mobius_left_matmul(_m: Array, _x: Array, _k: ArrayLike, _eps: float = EPS) -> Array:
   """Mobius matrix multiplication in manifold with curvature k."""
   raise NotImplementedError
 
 
 # def mobius_fn(fn: FN) -> FN:
 #     """Mobius function composition in manifold with curvature k."""
 
 #     def wrap(*args, **kwds) ->
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH addition of two vectors x.y in SH manifold with curvature k."""
   return sh_expmap(
       x,
       sh_ptrans0(x, sh_logmap0(y, k, eps=eps), k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH addition of two vectors x in L, y in E with curvature k."""
   return sh_expmap(
       x,
       sh_ptrans0(x, y, k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_scalar_mul(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH mix space scalar multiplication with curvature k."""
   return sh_expmap0(
       m * sh_logmap0(x, k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_matmulh(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH hyberbolic space matrix multiplication with curvature k."""
   return sh_expmap0(
       sh_logmap0(m, k, eps=eps) @ sh_logmap0(x, k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_matmull(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH mix space matrix multiplication (left L, right E) with curvature k."""
   return sh_expmap0(
       sh_logmap0(m, k, eps=eps) @ x,
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_matmulr(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """SH mix space matrix multiplication (left E, right L) with curvature k."""
   return sh_expmap0(
       m @ sh_logmap0(x, k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def gyration(u: Array, v: Array, a: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Gyration of a vector u around a vector v in manifold with curvature k."""
   return mobius_add(
       -mobius_add(u, v, k, eps=eps),
       mobius_add(u, mobius_add(v, a, k, eps=eps), k, eps=eps),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def stereo_proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Project x on the manifold with curvature k."""
   c = radius(k, eps=eps)
   x_norm = norm(x, axis=-1, keepdims=True, eps=eps)
   return jax.lax.select(
       x_norm > jnp.full_like(x, c),
       c * x / x_norm,
       x,
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Project x on the manifold with curvature k."""
   x_norm = minkowski_sqnorm(x, k=0, axis=-1, keepdims=True)
   return x.at[..., :1].set(safe_sqrt(x_norm - (1 / k), eps=eps))
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def stereo_dist(
     x: Array, y: Array, k: ArrayLike, axis: int = -1, eps: float = EPS
 ) -> Array:
   """Distance between two vectors in manifold with curvature k."""
   c = radius(k, eps=eps)
   return 2 * c * arctank(norm(mobius_add(-x, y, k, eps=eps), axis=axis, eps=eps) / c, k)
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def sh_dist(
     x: Array, y: Array, k: ArrayLike, axis: int = -1, eps: float = EPS
 ) -> Array:
   """Distance between two vectors in manifold with curvature k."""
   c = radius(k, eps=eps)
   return c * arccosk(k * minkowski_inner(x, y, k=k, axis=axis, keepdims=True), k)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def stereo_ptrans(
     x: Array, y: Array, v: Array, k: ArrayLike, eps: float = EPS
 ) -> Array:
   """Compute the parallel transport of v from x to y."""
   return (
       gyration(y, -x, v, k, eps=eps)
       * lambda_x(x, k, axis=-1, keepdims=True)
       / lambda_x(y, k, axis=-1, keepdims=True)
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def stereo_ptrans0(y: Array, v: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Compute the parallel transport of v from the origin to y."""
   # NOTE: we do not need to depend on addition.  Thus, we can
   #       implement addition with parallel transport.
   # return stereo_ptrans(jnp.zeros_like(y), y, v, k, eps=eps)
   del eps
   return (
       v
       * lambda_x(jnp.zeros_like(y), k, axis=-1, keepdims=True)
       / lambda_x(y, k, axis=-1, keepdims=True)
   )
 
 
-# @partial(jax.jit, static_argnames=("eps",), inline=True)
+# @partial(jax.jit, static_argnames=("eps",))
 def _sh_ptrans_v1(
     x: Array, y: Array, v: Array, k: ArrayLike, eps: float = EPS
 ) -> Array:
   """Compute the parallel transport of v from x to y with curvature k."""
   logxy = sh_logmap(x, y, k, eps=eps)
   logyx = sh_logmap(y, x, k, eps=eps)
   return v - (
       minkowski_inner(logxy, v, k=k, axis=-1, keepdims=True)
       / (sh_dist(x, y, k, axis=-1) ** 2)
   ) * (logxy + logyx)
 
 
-# @partial(jax.jit, static_argnames=("eps",), inline=True)
+# @partial(jax.jit, static_argnames=("eps",))
 def _sh_ptrans(x: Array, y: Array, v: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Compute the parallel transport of v from x to y with curvature k."""
   return v - safe_div(
       k * minkowski_inner(y, v, k=k, axis=-1, keepdims=True),
       1 + k * minkowski_inner(x, y, k=k, axis=-1, keepdims=True),
       eps=eps,
   ) * (x + y)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_ptrans(x: Array, y: Array, v: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Compute the parallel transport of v from x to y with curvature k."""
   return jax.lax.cond(
       jnp.all(x == y),
       lambda: v,  # Avoild div 0
       lambda: _sh_ptrans(x, y, v, k, eps=eps),
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_ptrans0(y: Array, v: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Compute the parallel transport of v from the origin to y with curvature k."""
   c = radius(k, eps=eps)
   return sh_ptrans(jnp.zeros_like(y).at[..., 0].set(c), y, v, k, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def stereo_expmap(
     x: Array, u: Array, k: ArrayLike, axis: int = -1, eps: float = EPS
 ) -> Array:
   """Exponential map of a tangent vector u at x in manifold with curvature k."""
   c = radius(k, eps=eps)
   return mobius_add(
       x,
@@ -601,97 +599,99 @@
       * tank(tangent_norm(x, u, k, axis, keepdims=True, eps=eps) / 2 / c, k)
       * (u / norm(u, axis=axis, keepdims=True, eps=eps)),
       k,
       eps=eps,
   )
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def stereo_expmap0(u: Array, k: ArrayLike, axis: int = -1, eps: float = EPS) -> Array:
   """Exponential map at the origin."""
   return stereo_expmap(jnp.zeros_like(u), u, k, axis=axis, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_expmap(x: Array, u: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Exponential map of a tangent vector u at x in L manifold with curvature k."""
   c = radius(k, eps=eps)
   u_norm = minkowski_norm(u, k=k, axis=-1, keepdims=True, eps=eps) / c
   return (cosk(u_norm, k) * x) + (sink(u_norm, k) * (u / u_norm))
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_expmap0(u: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Exponential map at the origin with curvature k."""
   c = radius(k, eps=eps)
   x = jnp.zeros_like(u).at[..., 0].set(c)
   u = u.at[..., 0].set(0)
   return sh_expmap(x, u, k, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_expmap00(u: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Exponential map at the origin with 0 prepend with curvature k."""
   c = radius(k, eps=eps)
   u = jnp.concatenate([jnp.zeros_like(u[..., :1]), u], axis=-1)
   x = jnp.zeros_like(u).at[..., 0].set(c)
   return sh_expmap(x, u, k, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def stereo_logmap(
     x: Array, y: Array, k: ArrayLike, axis: int = -1, eps: float = EPS
 ) -> Array:
   """Logarithmic map of a hyperbolic vector y at x in manifold with curvature k."""
   c = radius(k, eps=eps)
   sub = mobius_add(-x, y, k, eps=eps)
   return (
       2
       * c
       * arctank(norm(sub, axis=axis, keepdims=True, eps=eps) / c, k)
-      * (sub / tangent_norm(x, sub, k, axis=axis, keepdims=True, eps=eps))
+      * safe_div(
+          sub, tangent_norm(x, sub, k, axis=axis, keepdims=True, eps=eps), eps=eps
+      )
   )
 
 
-@partial(jax.jit, static_argnames=("axis", "eps"), inline=True)
+@partial(jax.jit, static_argnames=("axis", "eps"))
 def stereo_logmap0(y: Array, k: ArrayLike, axis: int = -1, eps: float = EPS) -> Array:
   """Logarithmic map at the origin."""
   return stereo_logmap(jnp.zeros_like(y), y, k, axis=axis, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_logmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Logarithmic map of a SH vector y at x in manifold with curvature k."""
   num = y - k * minkowski_inner(x, y, k=k, axis=-1, keepdims=True) * x
   return sh_dist(x, y, k, axis=-1, eps=eps) * (
       num / minkowski_norm(num, k=k, axis=-1, keepdims=True, eps=eps)
   )
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_logmap0(y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Logarithmic map at the origin with curvature k."""
   c = radius(k, eps=eps)
   x = jnp.zeros_like(y).at[..., 0].set(c)
   return sh_logmap(x, y, k, eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_logmap00(y: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Logarithmic map at the origin with 0 prepend with curvature k."""
   return sh_logmap0(y, k, eps=eps)[..., 1:]
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def stereo_egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Convert Euclidean gradient to Riemannian gradient."""
   return safe_div(grad, lambda_x(x, k, axis=-1, keepdims=True), eps=eps)
 
 
-@partial(jax.jit, static_argnames=("eps",), inline=True)
+@partial(jax.jit, static_argnames=("eps",))
 def sh_egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Convert Euclidean gradient to Riemannian gradient."""
   del eps
   grad = grad.at[..., 0].mul(-1)
   return grad - minkowski_inner(x, grad, k=k, axis=-1, keepdims=True) * (x * k)
```

### Comparing `jaxrie-7/src/jaxrie/manifold/stereographic.py` & `jaxrie-8/src/jaxrie/manifold/stereographic.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,89 +56,89 @@
 Array = jax.Array
 
 
 class Stereographic(Manifold):
   """The universal Stereographic projection model."""
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold with curvature k."""
     return mobius_add(x, y, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold (left H, right E) with curvature k."""
     return mobius_adde(x, y, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def sub(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius subtraction on manifold with curvature k."""
     return mobius_add(x, -y, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def mul(r: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius multiplication on manifold with curvature k."""
     return mobius_scala_mul(r, x, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matvec(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius matrix vector multiplication on manifold with curvature k."""
     return mobius_matvec_mul(m, x, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmul(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius matrix multiplication on manifold with curvature k."""
     return mobius_matmulh(x1, x2, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmull(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left H, right E) with curvature k."""
     return mobius_matmull(x1, x2, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def matmulr(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left E, right H) with curvature k."""
     return mobius_matmulr(x1, x2, k, eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def expmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     return stereo_expmap(x, y, k, axis=-1, eps=eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def logmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     return stereo_logmap(x, y, k, axis=-1, eps=eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def expmap0(u: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     return stereo_expmap0(u, k, axis=-1, eps=eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def logmap0(y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     return stereo_logmap0(y, k, axis=-1, eps=eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Euclidean gradient to Riemannian gradient."""
     return stereo_egrad2rgrad(x, grad, k, eps=eps)
 
   @staticmethod
-  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  @partial(jax.jit, static_argnames=("eps",))
   def proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Projection on manifold with curvature k."""
     return stereo_proj(x, k, eps=eps)
```

### Comparing `jaxrie-7/src/jaxrie/modules/basic.py` & `jaxrie-8/src/jaxrie/modules/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,17 +148,14 @@
       b_init: hk.initializers.Initializer | None = None,
       name: str | None = None,
   ) -> None:
     """Initialize the layer."""
     super().__init__(name=name)
     self.out_features = out_features
     self.m = manifold
-
-    self.tk = k is None
-    self.k = -1.0 if k is None else k
     self.with_bias = with_bias
 
     w_init = w_init or hk.initializers.VarianceScaling(1.0, "fan_avg", "uniform")
 
     self.linear = HLinear(
         out_features,
         manifold,
```

### Comparing `jaxrie-7/src/jaxrie/nets/basic.py` & `jaxrie-8/src/jaxrie/nets/basic.py`

 * *Files identical despite different names*

