# Comparing `tmp/fastdatetime-0.3.1.tar.gz` & `tmp/fastdatetime-0.3.2.tar.gz`

## Comparing `fastdatetime-0.3.1.tar` & `fastdatetime-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 fastdatetime-0.3.1/Cargo.toml
--rw-r--r--   0      501       20      223 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/.cargo/config.toml
--rw-r--r--   0      501       20     9143 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/.github/workflows/CI.yaml
--rw-r--r--   0      501       20     3176 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/.gitignore
--rw-r--r--   0      501       20       85 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/.vscode/settings.json
--rw-r--r--   0      501       20      517 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/COPYRIGHT.md
--rw-r--r--   0      501       20    11356 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/LICENSE-APACHE
--rw-r--r--   0      501       20     1089 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/LICENSE-MIT
--rw-r--r--   0      501       20     3575 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/README.md
--rw-r--r--   0      501       20      409 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/pyproject.toml
--rw-r--r--   0      501       20       28 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/fastdatetime/__init__.py
--rw-r--r--   0      501       20      259 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/fastdatetime/fastdatetime.pyi
--rw-r--r--   0      501       20        0 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/fastdatetime/py.typed
--rw-r--r--   0      501       20       95 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/requirements-dev.txt
--rw-r--r--   0      501       20     2028 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/perf/test_iso8601_performance.py
--rw-r--r--   0      501       20      646 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/perf/test_parse_performance.py
--rw-r--r--   0      501       20     1258 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/perf/test_ymd_performance.py
--rw-r--r--   0      501       20       95 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/pytest.ini
--rw-r--r--   0      501       20     2538 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/unit/test_conformance.py
--rw-r--r--   0      501       20     1499 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/python/tests/unit/test_strptime.py
--rw-r--r--   0      501       20     2033 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/src/datetime_utils.rs
--rw-r--r--   0      501       20     1411 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/src/interop.rs
--rw-r--r--   0      501       20     5310 2022-08-31 19:56:47.000000 fastdatetime-0.3.1/src/lib.rs
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 fastdatetime-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 fastdatetime-0.3.2/Cargo.toml
+-rw-r--r--   0      501       20      223 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/.cargo/config.toml
+-rw-r--r--   0      501       20     6538 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/.github/workflows/CI.yaml
+-rw-r--r--   0      501       20     3176 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/.gitignore
+-rw-r--r--   0      501       20       85 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/.vscode/settings.json
+-rw-r--r--   0      501       20      517 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/COPYRIGHT.md
+-rw-r--r--   0      501       20    11356 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/LICENSE-APACHE
+-rw-r--r--   0      501       20     1089 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/LICENSE-MIT
+-rw-r--r--   0      501       20     3575 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/README.md
+-rw-r--r--   0      501       20      500 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/pyproject.toml
+-rw-r--r--   0      501       20       28 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/fastdatetime/__init__.py
+-rw-r--r--   0      501       20      259 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/fastdatetime/fastdatetime.pyi
+-rw-r--r--   0      501       20        0 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/fastdatetime/py.typed
+-rw-r--r--   0      501       20       95 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/requirements-dev.txt
+-rw-r--r--   0      501       20     2028 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/perf/test_iso8601_performance.py
+-rw-r--r--   0      501       20      646 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/perf/test_parse_performance.py
+-rw-r--r--   0      501       20     1258 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/perf/test_ymd_performance.py
+-rw-r--r--   0      501       20       95 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/pytest.ini
+-rw-r--r--   0      501       20     2538 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/unit/test_conformance.py
+-rw-r--r--   0      501       20     1499 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/python/tests/unit/test_strptime.py
+-rw-r--r--   0      501       20     2033 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/src/datetime_utils.rs
+-rw-r--r--   0      501       20     1411 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/src/interop.rs
+-rw-r--r--   0      501       20     5328 2023-04-13 11:51:05.000000 fastdatetime-0.3.2/src/lib.rs
+-rw-r--r--   0      501       20    24590 2023-04-13 11:51:12.000000 fastdatetime-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 fastdatetime-0.3.2/PKG-INFO
```

### Comparing `fastdatetime-0.3.1/.github/workflows/CI.yaml` & `fastdatetime-0.3.2/.github/workflows/CI.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -12,280 +12,193 @@
       - 'releases/**'
 
 jobs:
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install Rust toolchain
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@stable
         with:
-          toolchain: stable
-          target: aarch64-apple-darwin
-          profile: minimal
-          default: true
+          targets: aarch64-apple-darwin
       - name: Build Rust crate
         run: cargo build --release
       - name: Run Rust unit tests
         run: cargo test --no-default-features --release
       - name: Build Python wheels (x86_64)
         uses: messense/maturin-action@v1
         with:
           target: x86_64
-          args: -i python --release --out dist
+          args: -i python --release --out dist --sdist
       - name: Install Python wheels (x86_64)
         run: |
           pip install fastdatetime --no-index --find-links dist --force-reinstall
       - name: Build Python wheels (universal2)
-        if: ${{ matrix.python-version >= '3.8' || matrix.python-version == '3.10' }}
+        if: ${{ matrix.python-version >= '3.8' || contains(fromJson('["3.10", "3.11"]'), matrix.python-version) }}
         uses: messense/maturin-action@v1
         with:
-          args: -i python --release --universal2 --out dist --no-sdist
+          args: -i python --release --universal2 --out dist
       - name: Install Python wheels (universal2)
-        if: ${{ matrix.python-version >= '3.8' }}
+        if: ${{ matrix.python-version >= '3.8' || contains(fromJson('["3.10", "3.11"]'), matrix.python-version) }}
         run: |
           pip install fastdatetime --no-index --find-links dist --force-reinstall
       - name: Run Python unit tests
         run: |
           pip install -r python/requirements-dev.txt
           python -m pytest -v python/tests/unit
       - name: Upload Python wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         target: [x64]
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: ${{ matrix.target }}
-      - name: Update rustup
-        run: rustup self update
       - name: Install Rust toolchain
-        uses: actions-rs/toolchain@v1
-        with:
-          toolchain: stable
-          profile: minimal
-          default: true
+        uses: dtolnay/rust-toolchain@stable
       - name: Build Rust crate
         if: matrix.target == 'x64'
         run: cargo build --release
       - name: Run Rust unit tests
         if: matrix.target == 'x64'
         run: cargo test --no-default-features --release
       - name: Build Python wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: -i python --release --out dist --no-sdist
+          args: -i python --release --out dist
       - name: Install Python wheels
         run: |
           pip install fastdatetime --no-index --find-links dist --force-reinstall
       - name: Run Python unit tests
         run: |
           pip install -r python/requirements-dev.txt
           python -m pytest -v python/tests/unit
       - name: Upload Python wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         target: [x86_64, i686]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Install Rust toolchain
-      uses: actions-rs/toolchain@v1
-      with:
-        toolchain: stable
-        profile: minimal
-        default: true
+      uses: dtolnay/rust-toolchain@stable
     - name: Build Rust crate
       run: cargo build --release
     - name: Run Rust unit tests
       run: cargo test --no-default-features --release
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Build Python wheels
       uses: messense/maturin-action@v1
       with:
         target: ${{ matrix.target }}
         manylinux: auto
-        args: -i python${{ matrix.python-version }} --release --out dist --no-sdist
+        args: -i python${{ matrix.python-version }} --release --out dist
     - name: Run Python unit tests
       if: matrix.target == 'x86_64'
       run: |
         pip install fastdatetime --no-index --find-links dist --force-reinstall
         pip install -r python/requirements-dev.txt
         python -m pytest -v python/tests/unit
     - name: Run Python benchmarks
       if: matrix.target == 'x86_64'
       run: |
         pip install -r python/requirements-dev.txt
         python -m pytest -v --benchmark-only python/tests/perf
     - name: Upload Python wheels
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   linux-cross:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: [
-          { version: '3.7', abi: 'cp37-cp37m' },
-          { version: '3.8', abi: 'cp38-cp38' },
-          { version: '3.9', abi: 'cp39-cp39' },
-          { version: '3.10', abi: 'cp310-cp310' },
+          '3.7',
+          '3.8',
+          '3.9',
+          '3.10',
+          '3.11',
         ]
-        target: [aarch64, armv7, s390x, ppc64le, ppc64]
-        include:
-          - python:
-              version: 3.7
-              abi: pp37-pypy37_pp73
-            target: aarch64
-          - python:
-              version: 3.8
-              abi: pp38-pypy38_pp73
-            target: aarch64
+        target: [aarch64, armv7]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Build Python wheels
       uses: messense/maturin-action@v1
-      env:
-        PYO3_CROSS_LIB_DIR: /opt/python/${{ matrix.python.abi }}
       with:
         target: ${{ matrix.target }}
         manylinux: auto
-        args: -i python3.9 --release --out dist --no-sdist 
-    - uses: uraimo/run-on-arch-action@v2.0.5
-      # run-on-arch-action doesn't have ppc64 support
-      # skipped cross compiled pypy wheel tests for now
-      if: ${{ matrix.target != 'ppc64' && !startsWith(matrix.python.abi, 'pp') }}
+        args: -i ${{ matrix.python }} --release --out dist
+    - uses: uraimo/run-on-arch-action@v2.3.0
       name: Install Python wheels
       with:
         arch: ${{ matrix.target }}
         distro: ubuntu20.04
         githubToken: ${{ github.token }}
         # Mount the dist directory as /artifacts in the container
         dockerRunArgs: |
           --volume "${PWD}/dist:/artifacts"
         install: |
           apt-get update
           apt-get install -y --no-install-recommends python3 python3-venv software-properties-common
           add-apt-repository ppa:deadsnakes/ppa
           apt-get update
-          apt-get install -y curl python3.7-venv python3.9-venv python3.10-venv
+          apt-get install -y curl python3.7-venv python3.9-venv python3.10-venv python3.11-venv
         run: |
           ls -lrth /artifacts
-          PYTHON=python${{ matrix.python.version }}
+          PYTHON=python${{ matrix.python }}
           $PYTHON -m venv venv
           venv/bin/pip install -U pip
           venv/bin/pip install fastdatetime --no-index --find-links /artifacts --force-reinstall
           venv/bin/python -c 'import fastdatetime'
     - name: Upload Python wheels
-      uses: actions/upload-artifact@v2
-      with:
-        name: wheels
-        path: dist
-
-  pypy-linux:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python: [
-          { version: pypy-3.7, abi: pp37-pypy37_pp73 },
-          { version: pypy-3.8, abi: pp38-pypy38_pp73 },
-        ]
-    steps:
-    - uses: actions/checkout@v2
-    - uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python.version }}
-    - name: Build Pypy wheels
-      uses: messense/maturin-action@v1
-      with:
-        target: ${{ matrix.target }}
-        manylinux: auto
-        args: -i /opt/python/${{ matrix.python.abi }}/bin/pypy --release --out dist --no-sdist 
-    - name: Run Pypy import check
-      run: |
-        pip install fastdatetime --no-index --find-links dist
-        pypy -c "import fastdatetime"
-    - name: Upload Pypy wheels
-      uses: actions/upload-artifact@v2
-      with:
-        name: wheels
-        path: dist
-
-  pypy-macos:
-    runs-on: macos-latest
-    strategy:
-      matrix:
-        python-version: [ pypy-3.7, pypy-3.8 ]
-    steps:
-    - uses: actions/checkout@v2
-    - name: Install Rust toolchain
-      uses: actions-rs/toolchain@v1
-      with:
-        toolchain: stable
-        profile: minimal
-        default: true
-    - uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install maturin
-      run: pip install maturin
-    - name: Build Pypy wheels
-      run: |
-        maturin build -i $(which pypy) --release --out dist
-        ls -l dist
-    - name: Run Pypy import check
-      run: |
-        pip install fastdatetime --no-index --find-links dist
-        pypy -c "import fastdatetime"
-    - name: Upload Pypy wheels
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [ macos, windows, linux, linux-cross, pypy-linux, pypy-macos ]
+    needs: [ macos, windows, linux, linux-cross ]
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: wheels
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: 3.9
+          python-version: '3.10'
       - name: Publish to PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
         run: |
-          pip install --upgrade wheel pip setuptools twine
+          pip install --upgrade twine
           twine upload --skip-existing *
```

### Comparing `fastdatetime-0.3.1/.gitignore` & `fastdatetime-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/COPYRIGHT.md` & `fastdatetime-0.3.2/COPYRIGHT.md`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/LICENSE-APACHE` & `fastdatetime-0.3.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/LICENSE-MIT` & `fastdatetime-0.3.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/README.md` & `fastdatetime-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/python/tests/perf/test_iso8601_performance.py` & `fastdatetime-0.3.2/python/tests/perf/test_iso8601_performance.py`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/python/tests/perf/test_parse_performance.py` & `fastdatetime-0.3.2/python/tests/perf/test_parse_performance.py`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/python/tests/perf/test_ymd_performance.py` & `fastdatetime-0.3.2/python/tests/perf/test_ymd_performance.py`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/python/tests/unit/test_conformance.py` & `fastdatetime-0.3.2/python/tests/unit/test_conformance.py`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/python/tests/unit/test_strptime.py` & `fastdatetime-0.3.2/python/tests/unit/test_strptime.py`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/src/datetime_utils.rs` & `fastdatetime-0.3.2/src/datetime_utils.rs`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/src/interop.rs` & `fastdatetime-0.3.2/src/interop.rs`

 * *Files identical despite different names*

### Comparing `fastdatetime-0.3.1/src/lib.rs` & `fastdatetime-0.3.2/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 use chrono::format::{parse, Parsed, StrftimeItems};
 
-use pyo3::{once_cell::GILOnceCell, prelude::*};
+use pyo3::once_cell::GILOnceCell;
+use pyo3::prelude::*;
 use time_fmt::parse::{
     parse_date_time_maybe_with_zone, parse_strict_date_time_maybe_with_zone, TimeZoneSpecifier,
 };
 use time_tz::{Offset, TimeZone};
 
 mod datetime_utils;
 mod interop;
 
 use interop::TryIntoPy;
 
 static DEFAULT_PARSER: GILOnceCell<dtparse::Parser> = GILOnceCell::new();
 
-#[pyfunction(date_string, "/", "*", dayfirst = "false", yearfirst = "false")]
+#[pyfunction]
 #[pyo3(name = "parse")]
+#[pyo3(signature = (date_string, /, *, dayfirst=false, yearfirst=false))]
 fn parse_from_py(
     py: Python<'_>,
     date_string: &str,
     dayfirst: Option<bool>,
     yearfirst: Option<bool>,
 ) -> PyResult<PyObject> {
     let (datetime, _offset, _tokens) = DEFAULT_PARSER
```

### Comparing `fastdatetime-0.3.1/PKG-INFO` & `fastdatetime-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: fastdatetime
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: Like datetime, but fast
 Keywords: datetime,parsing,iso8601,rfc3339
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://github.com/m1so/fastdatetime
 
 <div align="center">
 
 # fastdatetime
 
 Like `datetime`, but fast 🚀
```

