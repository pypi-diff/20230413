# Comparing `tmp/pytest_mpiexec-0.0.1.dev0.tar.gz` & `tmp/pytest_mpiexec-0.0.1a1.tar.gz`

## Comparing `pytest_mpiexec-0.0.1.dev0.tar` & `pytest_mpiexec-0.0.1a1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/.flake8
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/examples/conftest.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/examples/test_mpi.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/pytest_mpiexec/__init__.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/pytest_mpiexec/pytest_plugin.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/.flake8
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/examples/conftest.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/examples/test_mpi.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/pytest_mpiexec/__init__.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/pytest_mpiexec/pytest_plugin.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/tests/test_mpiexec.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/README.md
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pytest_mpiexec-0.0.1a1/PKG-INFO
```

### Comparing `pytest_mpiexec-0.0.1.dev0/.pre-commit-config.yaml` & `pytest_mpiexec-0.0.1a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_mpiexec-0.0.1.dev0/examples/test_mpi.py` & `pytest_mpiexec-0.0.1a1/examples/test_mpi.py`

 * *Files identical despite different names*

### Comparing `pytest_mpiexec-0.0.1.dev0/pytest_mpiexec/pytest_plugin.py` & `pytest_mpiexec-0.0.1a1/pytest_mpiexec/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_mpiexec-0.0.1.dev0/.gitignore` & `pytest_mpiexec-0.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_mpiexec-0.0.1.dev0/LICENSE` & `pytest_mpiexec-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mpiexec-0.0.1.dev0/pyproject.toml` & `pytest_mpiexec-0.0.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "py311",
 ]
 
 [tool.tbump]
 github_url = "https://github.com/minrk/pytest-mpiexec"
 
 [tool.tbump.version]
-current = "0.0.1.dev0"
+current = "0.0.1a1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `pytest_mpiexec-0.0.1.dev0/PKG-INFO` & `pytest_mpiexec-0.0.1a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mpiexec
-Version: 0.0.1.dev0
+Version: 0.0.1a1
 Summary: pytest plugin for running individual tests with mpiexec
 Project-URL: Documentation, https://github.com/minrk/pytest-mpiexec#readme
 Project-URL: Issues, https://github.com/minrk/pytest-mpiexec/issues
 Project-URL: Source, https://github.com/minrk/pytest-mpiexec
 Author-email: Min RK <benjaminrk@gmail.com>
 License: MIT License
         
@@ -39,11 +39,45 @@
 Requires-Dist: pytest-reportlog
 Description-Content-Type: text/markdown
 
 # pytest-mpixec
 
 pytest plugin for running individual tests with mpiexec
 
-Prior art:
+A test marked with `mark.mpiexec` will be run in a separate instance with mpiexec,
+instead of in the current process.
 
-- pytest-mpi (helpers for tests run inside mpi)
-- pytest-easyMPI (similar goal to this one, doesn't work with more complex fixtures)
+The subprocess test will be run with pytest,
+so fixtures and everything should still work!
+
+The number of processes can be parametrized if you parametrize an argument called `mpiexec_n`.
+
+## Try it out
+
+```
+pip install pytest-mpiexec
+```
+
+And write tests that use mpiexec:
+
+```python
+from mpi4py import MPI
+
+@pytest.mark.mpiexec(n=2)
+def test_my_mpi_code(fixtures):
+
+@pytest.mark.mpiexec
+@pytest.mark.parametrize("mpiexec_n", [1, 2, 3])
+def test_my_mpi_code(mpiexec_n):
+    assert MPI.COMM_WORLD.size == mpiexec_n
+
+```
+
+## Caveats
+
+If you use module or session-scoped fixtures, another instance will be running,
+so these can't conflict with other pytest runs (e.g. conflicting on ports, files, etc.)
+
+## Prior art
+
+- pytest-mpi (helpers for tests run inside mpi - compatible with this package!)
+- pytest-easyMPI (similar goal to this one, but takes a different approach)
```

