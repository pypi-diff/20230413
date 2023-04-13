# Comparing `tmp/jit_env-0.1.0.tar.gz` & `tmp/jit_env-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jit_env-0.1.0.tar", last modified: Tue Apr 11 07:42:30 2023, max compression
+gzip compressed data, was "dist/jit_env-0.1.1.tar", last modified: Thu Apr 13 07:54:52 2023, max compression
```

## Comparing `jit_env-0.1.0.tar` & `jit_env-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.458306 jit_env-0.1.0/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.0/LICENSE
--rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.0/MANIFEST.in
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5573 2023-04-11 07:42:28.458306 jit_env-0.1.0/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-11 07:42:07.000000 jit_env-0.1.0/README.md
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.373406 jit_env-0.1.0/jit_env/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.0/jit_env/__init__.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.0/jit_env/_compat_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    13334 2023-04-11 06:27:58.000000 jit_env-0.1.0/jit_env/_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.0/jit_env/_core_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.0/jit_env/_specs_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    11689 2023-04-11 06:25:55.000000 jit_env-0.1.0/jit_env/_wrappers_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.0/jit_env/compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.0/jit_env/specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-11 07:41:44.000000 jit_env-0.1.0/jit_env/version.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    13538 2023-04-10 14:43:14.000000 jit_env-0.1.0/jit_env/wrappers.py
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-11 07:42:28.443133 jit_env-0.1.0/jit_env.egg-info/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5573 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)      436 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/SOURCES.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/dependency_links.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/requires.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-11 07:42:27.000000 jit_env-0.1.0/jit_env.egg-info/top_level.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.0/requirements.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.0/requirements_dev.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-11 07:42:28.458306 jit_env-0.1.0/setup.cfg
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1840 2023-04-10 08:18:00.000000 jit_env-0.1.0/setup.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.745051 jit_env-0.1.1/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.1/LICENSE
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-13 07:54:52.745051 jit_env-0.1.1/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-11 07:42:07.000000 jit_env-0.1.1/README.md
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.650741 jit_env-0.1.1/jit_env/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.1/jit_env/__init__.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.1/jit_env/_compat_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    13759 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/_core.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.1/jit_env/_core_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.1/jit_env/_specs_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    13284 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/_wrappers_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.1/jit_env/compat.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/py.typed
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.1/jit_env/specs.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-13 07:54:46.000000 jit_env-0.1.1/jit_env/version.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14216 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/wrappers.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.737495 jit_env-0.1.1/jit_env.egg-info/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-13 07:54:52.000000 jit_env-0.1.1/jit_env.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/requires.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/top_level.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.1/requirements.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.1/requirements_dev.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-13 07:54:52.745051 jit_env-0.1.1/setup.cfg
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.1/setup.py
```

### Comparing `jit_env-0.1.0/LICENSE` & `jit_env-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/PKG-INFO` & `jit_env-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: jit_env
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
 ![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
```

### Comparing `jit_env-0.1.0/README.md` & `jit_env-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/__init__.py` & `jit_env-0.1.1/jit_env/__init__.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/_compat_test.py` & `jit_env-0.1.1/jit_env/_compat_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/_core.py` & `jit_env-0.1.1/jit_env/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,19 @@
     """Interface for defining Environment logic for RL-Agents. """
 
     def __str__(self) -> str:
         """Returns a minimal representation of the Environment Structure."""
         return self.__class__.__name__
 
     def __repr__(self) -> str:
-        """Returns a complete informative representation of self."""
+        """Returns a complete informative representation of self.
+
+        Opposed to `str`, the class should be reconstructable from the
+        `repr` information.
+        """
         return self.__str__()
 
     @property
     def unwrapped(self) -> Environment:
         """Helper function to support unpacking Composite Environments."""
         return self
 
@@ -270,14 +274,22 @@
         super().__init__()
         self._env = env
 
     def __str__(self) -> str:
         """Returns a recursive composition structure of all Wrappers."""
         return f"{self.__class__.__name__}({str(self.env)})"
 
+    def __repr__(self) -> str:
+        """Returns a recursive complete informative representation of self.
+
+        Opposed to `str`, the Wrapped class hierarchy should be
+        reconstructable from the `repr` information.
+        """
+        return f"{self.__class__.__name__}(env={repr(self.env)})"
+
     @property
     def env(self):
         """Helper function to unpack Composite Environments by one level."""
         return self._env
 
     @property
     def unwrapped(self) -> Environment:
```

### Comparing `jit_env-0.1.0/jit_env/_core_test.py` & `jit_env-0.1.1/jit_env/_core_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/_specs_test.py` & `jit_env-0.1.1/jit_env/_specs_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/_wrappers_test.py` & `jit_env-0.1.1/jit_env/_wrappers_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,54 @@
 import jax
 from jax import numpy as jnp
 
 import jit_env
 from jit_env import wrappers, specs
 
 
-@pytest.mark.usefixtures('dummy_env')
-def test_repr(dummy_env: jit_env.Environment):
-    wrapped = wrappers.Jit(dummy_env)
+class TestRepr:
 
-    assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
-                           f'{dummy_env.__class__.__name__})'
+    def test_empty(self, dummy_env: jit_env.Environment):
+        wrapped = jit_env.Wrapper(dummy_env)
 
-    # Since Jit doesn't modify `repr` or str this should hold.
-    assert repr(wrapped) == str(wrapped)
+        assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
+                               f'{dummy_env.__class__.__name__})'
+        assert repr(wrapped) == f'{wrapped.__class__.__name__}(' \
+                                f'env={dummy_env.__class__.__name__})'
+
+    @pytest.mark.usefixtures('dummy_env')
+    def test_jit(self, dummy_env: jit_env.Environment):
+        wrapped = wrappers.Jit(dummy_env)
+
+        assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
+                               f'{dummy_env.__class__.__name__})'
+        assert repr(wrapped) == f'{wrapped.__class__.__name__}(' \
+                                f'env={dummy_env.__class__.__name__},' \
+                                f'jit_kwargs={{}})'
+
+    @pytest.mark.usefixtures('dummy_env')
+    def test_vmap(self, dummy_env: jit_env.Environment):
+        wrapped = wrappers.Vmap(dummy_env)
+
+        assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
+                               f'{dummy_env.__class__.__name__})'
+        assert repr(wrapped) == f'{wrapped.__class__.__name__}(' \
+                                f'env={dummy_env.__class__.__name__},' \
+                                f'step_vmap_kwargs={{}})'
+
+    @pytest.mark.usefixtures('dummy_env')
+    def test_tile(self, dummy_env: jit_env.Environment, num: int = 2):
+        wrapped = wrappers.Tile(dummy_env, num=num, in_axes=(0, None))
+
+        assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
+                               f'{dummy_env.__class__.__name__})'
+        assert repr(wrapped) == f'{wrapped.__class__.__name__}(' \
+                                f'env={dummy_env.__class__.__name__},' \
+                                f'num={num},' \
+                                f'step_vmap_kwargs={{\'in_axes\': (0, None)}})'
 
 
 def test_unwrap(dummy_env: jit_env.Environment):
     wrapped = wrappers.Jit(dummy_env)
     doubly_wrapped = wrappers.Vmap(wrapped)
 
     assert wrapped.unwrapped is dummy_env
```

### Comparing `jit_env-0.1.0/jit_env/compat.py` & `jit_env-0.1.1/jit_env/compat.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/specs.py` & `jit_env-0.1.1/jit_env/specs.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.0/jit_env/wrappers.py` & `jit_env-0.1.1/jit_env/wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,23 @@
                 keyword arguments passed to jax.jit for both `env.step` and
                 `env.reset`. Defer to the jax documentation for up-to-date
                 documentation on the keyword arguments.
         """
 
         super().__init__(env)
 
+        self._jit_kwargs = jit_kwargs
         self._step_fun = _jax.jit(env.step, **jit_kwargs)
         self._reset_fun = _jax.jit(env.reset, **jit_kwargs)
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(" \
+               f"env={repr(self.env)}," \
+               f"jit_kwargs={self._jit_kwargs})"
+
     def reset(
             self,
             key: _jax.random.KeyArray
     ) -> tuple[_core.State, _core.TimeStep]:
         return self._reset_fun(key)
 
     def step(
@@ -77,17 +83,24 @@
             **step_vmap_kwargs:
                 keyword arguments passed to jax.vmap only for `env.step`.
                 Defer to the jax documentation for up-to-date documentation
                 on the keyword arguments.
         """
         super().__init__(env)
 
+        self._step_vmap_kwargs = step_vmap_kwargs
+
         self._step_fun = _jax.vmap(env.step, **step_vmap_kwargs)
         self._reset_fun = _jax.vmap(env.reset)
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(" \
+               f"env={repr(self.env)}," \
+               f"step_vmap_kwargs={self._step_vmap_kwargs})"
+
     def reset(
             self,
             key: _jax.random.KeyArray  # (Batch, dim_key)
     ) -> tuple[_core.State, _core.TimeStep]:
         return self._reset_fun(key)
 
     def step(
@@ -179,14 +192,20 @@
     size Key Array. As a result, the environment-spec can be properly
     specified, which is done by the `BatchSpecMixin`.
 
     The constructor is called first through `BatchSpecMixin` which
     simultaneously requires the user to define the batch-size as `num`.
     """
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(" \
+               f"env={repr(self.env)}," \
+               f"num={self.num}," \
+               f"step_vmap_kwargs={self._step_vmap_kwargs})"
+
     def reset(
             self,
             key: _jax.random.KeyArray
     ) -> tuple[_core.State, _core.TimeStep]:
         return super().reset(_jax.random.split(key, num=self.num))
```

### Comparing `jit_env-0.1.0/jit_env.egg-info/PKG-INFO` & `jit_env-0.1.1/jit_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: jit-env
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
 ![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
```

### Comparing `jit_env-0.1.0/setup.py` & `jit_env-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     description='A Jax interface for Reinforcement Learning environments.',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author='Joery A. de Vries',
     author_email="J.A.deVries@tudelft.nl",
     keywords='reinforcement-learning python machine learning jax',
     packages=find_packages(),
+    package_data={'jit_env': ['py.typed']},
     url='https://github.com/joeryjoery/jit_env',
     license='MIT',
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     install_requires=_req,
     extras_require={'dev': _req_dev},
     classifiers=[
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Testing :: Mocking',
         'Topic :: Software Development :: Testing :: Unit'
     ]
 )
```

