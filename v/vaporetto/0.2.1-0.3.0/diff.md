# Comparing `tmp/vaporetto-0.2.1.tar.gz` & `tmp/vaporetto-0.3.0.tar.gz`

## Comparing `vaporetto-0.2.1.tar` & `vaporetto-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 vaporetto-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     4133 2023-04-01 14:08:29.000000 vaporetto-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      159 2023-04-01 14:08:29.000000 vaporetto-0.2.1/.readthedocs.yaml
--rw-r--r--   0     1001      123      562 2023-04-01 14:08:29.000000 vaporetto-0.2.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123     9723 2023-04-01 14:08:29.000000 vaporetto-0.2.1/LICENSE-APACHE
--rw-r--r--   0     1001      123     1023 2023-04-01 14:08:29.000000 vaporetto-0.2.1/LICENSE-MIT
--rw-r--r--   0     1001      123     2758 2023-04-01 14:08:29.000000 vaporetto-0.2.1/README.md
--rw-r--r--   0     1001      123      500 2023-04-01 14:08:29.000000 vaporetto-0.2.1/docs/source/api.rst
--rw-r--r--   0     1001      123      184 2023-04-01 14:08:29.000000 vaporetto-0.2.1/docs/source/conf.py
--rw-r--r--   0     1001      123     1390 2023-04-01 14:08:29.000000 vaporetto-0.2.1/docs/source/examples.rst
--rw-r--r--   0     1001      123      411 2023-04-01 14:08:29.000000 vaporetto-0.2.1/docs/source/index.rst
--rw-r--r--   0     1001      123      461 2023-04-01 14:08:29.000000 vaporetto-0.2.1/noxfile.py
--rw-r--r--   0     1001      123      106 2023-04-01 14:08:29.000000 vaporetto-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123      107 2023-04-01 14:08:29.000000 vaporetto-0.2.1/requirements-dev.txt
--rw-r--r--   0     1001      123    14583 2023-04-01 14:08:29.000000 vaporetto-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123      318 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/README.md
--rw-r--r--   0     1001      123        0 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/__init__.py
--rw-r--r--   0     1001      123      311 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/data/model.zst
--rw-r--r--   0     1001      123  1120767 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/data/wagahaiwa_nekodearu.txt
--rw-r--r--   0     1001      123      304 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/dataset.py
--rw-r--r--   0     1001      123     2279 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/test_comparison_cat.py
--rw-r--r--   0     1001      123     2207 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/test_comparison_count.py
--rw-r--r--   0     1001      123     2970 2023-04-01 14:08:29.000000 vaporetto-0.2.1/tests/test_vaporetto.py
--rw-r--r--   0     1001      123      929 2023-04-01 14:08:29.000000 vaporetto-0.2.1/vaporetto.pyi
--rw-r--r--   0     1001      123    13335 2023-04-01 14:08:52.000000 vaporetto-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 vaporetto-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 vaporetto-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     4393 2023-04-13 07:01:31.000000 vaporetto-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      159 2023-04-13 07:01:31.000000 vaporetto-0.3.0/.readthedocs.yaml
+-rw-r--r--   0     1001      123      562 2023-04-13 07:01:31.000000 vaporetto-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     9723 2023-04-13 07:01:31.000000 vaporetto-0.3.0/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1023 2023-04-13 07:01:31.000000 vaporetto-0.3.0/LICENSE-MIT
+-rw-r--r--   0     1001      123     3486 2023-04-13 07:01:31.000000 vaporetto-0.3.0/README.md
+-rw-r--r--   0     1001      123      500 2023-04-13 07:01:31.000000 vaporetto-0.3.0/docs/source/api.rst
+-rw-r--r--   0     1001      123      184 2023-04-13 07:01:31.000000 vaporetto-0.3.0/docs/source/conf.py
+-rw-r--r--   0     1001      123     2083 2023-04-13 07:01:31.000000 vaporetto-0.3.0/docs/source/examples.rst
+-rw-r--r--   0     1001      123      411 2023-04-13 07:01:31.000000 vaporetto-0.3.0/docs/source/index.rst
+-rw-r--r--   0     1001      123      461 2023-04-13 07:01:31.000000 vaporetto-0.3.0/noxfile.py
+-rw-r--r--   0     1001      123      106 2023-04-13 07:01:31.000000 vaporetto-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      107 2023-04-13 07:01:31.000000 vaporetto-0.3.0/requirements-dev.txt
+-rw-r--r--   0     1001      123    14252 2023-04-13 07:01:31.000000 vaporetto-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123      318 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/README.md
+-rw-r--r--   0     1001      123        0 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/__init__.py
+-rw-r--r--   0     1001      123      311 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/data/vaporetto.model.zst
+-rw-r--r--   0     1001      123  1120767 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/data/wagahaiwa_nekodearu.txt
+-rw-r--r--   0     1001      123      304 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/dataset.py
+-rw-r--r--   0     1001      123     2279 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/test_comparison_cat.py
+-rw-r--r--   0     1001      123     2207 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/test_comparison_count.py
+-rw-r--r--   0     1001      123     2976 2023-04-13 07:01:31.000000 vaporetto-0.3.0/tests/test_vaporetto.py
+-rw-r--r--   0     1001      123      929 2023-04-13 07:01:31.000000 vaporetto-0.3.0/vaporetto.pyi
+-rw-r--r--   0     1001      123    11660 2023-04-13 07:01:41.000000 vaporetto-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 vaporetto-0.3.0/PKG-INFO
```

### Comparing `vaporetto-0.2.1/Cargo.toml` & `vaporetto-0.3.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "python-vaporetto"
-version = "0.2.1"
+version = "0.3.0"
 edition = "2021"
 authors = ["Koichi Akabe <vbkaisetsu@gmail.com>"]
 description = "Python wrapper of Vaporetto tokenizer"
 readme = "README.md"
 license = "MIT OR Apache-2.0"
 homepage = "https://github.com/daac-tools/python-vaporetto"
 repository = "https://github.com/daac-tools/python-vaporetto"
@@ -13,10 +13,9 @@
 name = "vaporetto"
 crate-type = ["cdylib"]
 
 [dependencies]
 hashbrown = "0.13.2"  # MIT or Apache-2.0
 ouroboros = "0.15.6"  # MIT or Apache-2.0
 pyo3 = { version = "0.18.2", features = ["extension-module"] }  # Apache-2.0
-ruzstd = "0.3.0"  # MIT
 vaporetto_rust = { package = "vaporetto", version = "0.6.3", features = ["kytea"] }  # MIT or Apache-2.0
 vaporetto_rules = "0.6.3"  # MIT or Apache-2.0
```

### Comparing `vaporetto-0.2.1/.github/workflows/CI.yml` & `vaporetto-0.3.0/.github/workflows/CI.yml`

 * *Files 15% similar despite different names*

```diff
@@ -27,18 +27,21 @@
       uses: PyO3/maturin-action@v1
       with:
         manylinux: auto
         args: -i ${{ matrix.python-version }} --release
     - name: Test package
       run: |
         python -m pip install --upgrade pip
-        pip install pytest mypy
+        pip install pytest mypy zstandard
+        python -c "import zstandard;zstandard.ZstdDecompressor().copy_stream(open('tests/data/vaporetto.model.zst','rb'),open('tests/data/vaporetto.model','wb'))"
         pip install vaporetto --no-index --find-links target/wheels --force-reinstall
         mypy --strict tests
         pytest tests/test_vaporetto.py
+        python -m doctest README.md
+        python -m doctest docs/source/examples.rst
 
   pack-sdist:
     needs: [ test ]
     if: "startsWith(github.ref, 'refs/tags/')"
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
```

### Comparing `vaporetto-0.2.1/CONTRIBUTING.md` & `vaporetto-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/LICENSE-APACHE` & `vaporetto-0.3.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/LICENSE-MIT` & `vaporetto-0.3.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/README.md` & `vaporetto-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -33,49 +33,83 @@
 ```
 
 ## Example Usage
 
 python-vaporetto does not contain model files.
 To perform tokenization, follow [the document of Vaporetto](https://github.com/daac-tools/vaporetto) to download distribution models or train your own models beforehand.
 
+Check the version number as shown below to use compatible models:
+
+```python
+>>> import vaporetto
+>>> vaporetto.VAPORETTO_VERSION
+'0.6.3'
+
+```
+
+Examples:
+
 ```python
 # Import vaporetto module
-import vaporetto
+>>> import vaporetto
 
 # Load the model file
-with open('path/to/model.zst', 'rb') as fp:
-    model = fp.read()
+>>> with open('tests/data/vaporetto.model', 'rb') as fp:
+...     model = fp.read()
 
 # Create an instance of the Vaporetto
-tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
+>>> tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
 
 # Tokenize
-tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
-#=> 'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
+>>> tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
+'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
+
+>>> tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
+
+>>> len(tokens)
+6
+
+>>> tokens[0].surface()
+'まぁ'
+
+>>> tokens[0].tag(0)
+'名詞'
+
+>>> tokens[0].tag(1)
+'マー'
+
+>>> [token.surface() for token in tokens]
+['まぁ', '社長', 'は', '火星', '猫', 'だ']
+
+```
+
+## Note for distributed models
+
+The distributed models are compressed in zstd format. If you want to load these compressed models,
+you must decompress them outside the API.
+
+```python
+>>> import vaporetto
+>>> import zstandard  # zstandard package in PyPI
+
+>>> dctx = zstandard.ZstdDecompressor()
+>>> with open('tests/data/vaporetto.model.zst', 'rb') as fp:
+...    with dctx.stream_reader(fp) as dict_reader:
+...        tokenizer = vaporetto.Vaporetto(dict_reader.read(), predict_tags = True)
 
-tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
-len(tokens)
-#=> 6
-tokens[0].surface()
-#=> 'まぁ'
-tokens[0].tag(0)
-#=> '名詞'
-tokens[0].tag(1)
-#=> 'マー'
-[token.surface() for token in tokens]
-#=> ['まぁ', '社長', 'は', '火星', '猫', 'だ']
 ```
 
+## Note for KyTea's models
+
 You can also use KyTea's models as follows:
 
 ```python
-with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:
-    model = fp.read()
+>>> with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:  # doctest: +SKIP
+...     tokenizer = vaporetto.Vaporetto.create_from_kytea_model(fp.read())
 
-tokenizer = vaporetto.Vaporetto.create_from_kytea_model(model)
 ```
 
 Note: Vaporetto does not support tag prediction with KyTea's models.
 
 ## [Speed Comparison](https://github.com/daac-tools/python-vaporetto/wiki/Speed-Comparison)
 
 ## License
```

### Comparing `vaporetto-0.2.1/docs/source/examples.rst` & `vaporetto-0.3.0/docs/source/examples.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Example usage
 =============
 
 python-vaporetto does not contain model files. To perform tokenization, follow `the document of
 Vaporetto <https://github.com/daac-tools/vaporetto>`_ to download distribution models or train
 your own models beforehand.
 
+You can check the version number as shown below to use compatible models:
+
+.. code-block:: python
+
+   >>> import vaporetto
+   >>> vaporetto.VAPORETTO_VERSION
+   '0.6.3'
+
 Tokenize with Vaporetto model
 -----------------------------
 
 The following example tokenizes a string using a Vaporetto model.
 
 .. code-block:: python
 
    >>> import vaporetto
-   >>> with open('path/to/model.zst', 'rb') as fp:
-   >>>     model = fp.read()
+   >>> with open('tests/data/vaporetto.model', 'rb') as fp:
+   ...     model = fp.read()
 
    >>> tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
 
    >>> tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
    'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
 
    >>> tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
@@ -29,19 +37,30 @@
    >>> tokens[0].tag(0)
    '名詞'
    >>> tokens[0].tag(1)
    'マー'
    >>> [token.surface() for token in tokens]
    ['まぁ', '社長', 'は', '火星', '猫', 'だ']
 
+The distributed models are compressed in zstd format. If you want to load these compressed models,
+you must decompress them outside the API:
+
+.. code-block:: python
+
+   >>> import vaporetto
+   >>> import zstandard  # zstandard package in PyPI
+
+   >>> dctx = zstandard.ZstdDecompressor()
+   >>> with open('tests/data/vaporetto.model.zst', 'rb') as fp:
+   ...     with dctx.stream_reader(fp) as dict_reader:
+   ...         tokenizer = vaporetto.Vaporetto(dict_reader.read(), predict_tags = True)
 
 Tokenize with KyTea model
 -------------------------
 
 If you want to use a KyTea model, use ``create_from_kytea_model()`` instead.
 
 .. code-block:: python
 
-    >>> with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:
-    >>>     model = fp.read()
-
-    >>> tokenizer = vaporetto.Vaporetto.create_from_kytea_model(model)
+    >>> import vaporetto
+    >>> with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:  # doctest: +SKIP
+    ...     tokenizer = vaporetto.Vaporetto.create_from_kytea_model(fp.read())
```

### Comparing `vaporetto-0.2.1/src/lib.rs` & `vaporetto-0.3.0/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use std::fmt::Write;
-use std::io::Read;
 
 use pyo3::{exceptions::PyValueError, prelude::*, types::PyUnicode};
 
 use hashbrown::HashMap;
 use ouroboros::self_referencing;
 use vaporetto_rules::{
     sentence_filters::{ConcatGraphemeClustersFilter, KyteaWsConstFilter},
@@ -207,17 +206,16 @@
     }
 }
 
 /// Python binding of Vaporetto tokenizer.
 ///
 /// Examples:
 ///     >>> import vaporetto
-///     >>> with open('path/to/model.zst', 'rb') as fp:
-///     >>>     model = fp.read()
-///     >>> tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
+///     >>> with open('path/to/vaporetto.model', 'rb') as fp:
+///     ...     tokenizer = vaporetto.Vaporetto(fp.read(), predict_tags = True)
 ///     >>> tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
 ///     'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
 ///     >>> tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
 ///     >>> len(tokens)
 ///     6
 ///     >>> tokens[0].surface()
 ///     'まぁ'
@@ -314,22 +312,16 @@
     fn new(
         py: Python,
         model: &[u8],
         predict_tags: bool,
         wsconst: &str,
         norm: bool,
     ) -> PyResult<Self> {
-        let mut buf = vec![];
         let (model, _) = py.allow_threads(|| {
-            let mut decoder = ruzstd::StreamingDecoder::new(model)
-                .map_err(|e| PyValueError::new_err(e.to_string()))?;
-            decoder
-                .read_to_end(&mut buf)
-                .map_err(|e| PyValueError::new_err(e.to_string()))?;
-            Model::read_slice(&buf).map_err(|e| PyValueError::new_err(e.to_string()))
+            Model::read_slice(&model).map_err(|e| PyValueError::new_err(e.to_string()))
         })?;
         Self::create_internal(py, model, predict_tags, wsconst, norm)
     }
 
     /// Create a new Vaporetto instance from a KyTea's model.
     ///
     /// Vaporetto does not support tag prediction with KyTea's model.
```

### Comparing `vaporetto-0.2.1/tests/data/wagahaiwa_nekodearu.txt` & `vaporetto-0.3.0/tests/data/wagahaiwa_nekodearu.txt`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/tests/test_comparison_cat.py` & `vaporetto-0.3.0/tests/test_comparison_cat.py`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/tests/test_comparison_count.py` & `vaporetto-0.3.0/tests/test_comparison_count.py`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/tests/test_vaporetto.py` & `vaporetto-0.3.0/tests/test_vaporetto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import pathlib
 
 import vaporetto
 
-MODEL_PATH = pathlib.PurePath(__file__).parent / 'data/model.zst'
+MODEL_PATH = pathlib.PurePath(__file__).parent / 'data/vaporetto.model'
 
 
 def test_tokenlist_empty() -> None:
     with open(MODEL_PATH, 'rb') as fp:
         tokenizer = vaporetto.Vaporetto(fp.read())
     tokens = tokenizer.tokenize('')
```

### Comparing `vaporetto-0.2.1/vaporetto.pyi` & `vaporetto-0.3.0/vaporetto.pyi`

 * *Files identical despite different names*

### Comparing `vaporetto-0.2.1/Cargo.lock` & `vaporetto-0.3.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -53,20 +53,14 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "byteorder"
-version = "1.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
-
-[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "daachorse"
@@ -87,17 +81,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -136,15 +130,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f7d21ccd03305a674437ee1248f3ab5d4b1db095cf1caf49f1713ddf61956b7"
 dependencies = [
  "Inflector",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
@@ -171,15 +165,15 @@
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -188,17 +182,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.2"
@@ -241,36 +235,35 @@
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "python-vaporetto"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "hashbrown",
  "ouroboros",
  "pyo3",
- "ruzstd",
  "vaporetto",
  "vaporetto_rules",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
@@ -286,107 +279,49 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "ruzstd"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a15e661f0f9dac21f3494fe5d23a6338c0ac116a2d22c2b63010acd89467ffe"
-dependencies = [
- "byteorder",
- "thiserror",
- "twox-hash",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
-name = "static_assertions"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
-
-[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "syn"
-version = "2.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
-name = "thiserror"
-version = "1.0.40"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
-dependencies = [
- "thiserror-impl",
-]
-
-[[package]]
-name = "thiserror-impl"
-version = "1.0.40"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.12",
-]
-
-[[package]]
-name = "twox-hash"
-version = "1.6.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
-dependencies = [
- "cfg-if",
- "static_assertions",
-]
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-segmentation"
```

### Comparing `vaporetto-0.2.1/PKG-INFO` & `vaporetto-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaporetto
-Version: 0.2.1
+Version: 0.3.0
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: Python wrapper of Vaporetto tokenizer
 Home-Page: https://github.com/daac-tools/python-vaporetto
 Author: Koichi Akabe <vbkaisetsu@gmail.com>
 Author-email: Koichi Akabe <vbkaisetsu@gmail.com>
 License: MIT OR Apache-2.0
@@ -46,49 +46,83 @@
 ```
 
 ## Example Usage
 
 python-vaporetto does not contain model files.
 To perform tokenization, follow [the document of Vaporetto](https://github.com/daac-tools/vaporetto) to download distribution models or train your own models beforehand.
 
+Check the version number as shown below to use compatible models:
+
+```python
+>>> import vaporetto
+>>> vaporetto.VAPORETTO_VERSION
+'0.6.3'
+
+```
+
+Examples:
+
 ```python
 # Import vaporetto module
-import vaporetto
+>>> import vaporetto
 
 # Load the model file
-with open('path/to/model.zst', 'rb') as fp:
-    model = fp.read()
+>>> with open('tests/data/vaporetto.model', 'rb') as fp:
+...     model = fp.read()
 
 # Create an instance of the Vaporetto
-tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
+>>> tokenizer = vaporetto.Vaporetto(model, predict_tags = True)
 
 # Tokenize
-tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
-#=> 'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
+>>> tokenizer.tokenize_to_string('まぁ社長は火星猫だ')
+'まぁ/名詞/マー 社長/名詞/シャチョー は/助詞/ワ 火星/名詞/カセー 猫/名詞/ネコ だ/助動詞/ダ'
+
+>>> tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
+
+>>> len(tokens)
+6
+
+>>> tokens[0].surface()
+'まぁ'
+
+>>> tokens[0].tag(0)
+'名詞'
+
+>>> tokens[0].tag(1)
+'マー'
+
+>>> [token.surface() for token in tokens]
+['まぁ', '社長', 'は', '火星', '猫', 'だ']
+
+```
+
+## Note for distributed models
+
+The distributed models are compressed in zstd format. If you want to load these compressed models,
+you must decompress them outside the API.
+
+```python
+>>> import vaporetto
+>>> import zstandard  # zstandard package in PyPI
+
+>>> dctx = zstandard.ZstdDecompressor()
+>>> with open('tests/data/vaporetto.model.zst', 'rb') as fp:
+...    with dctx.stream_reader(fp) as dict_reader:
+...        tokenizer = vaporetto.Vaporetto(dict_reader.read(), predict_tags = True)
 
-tokens = tokenizer.tokenize('まぁ社長は火星猫だ')
-len(tokens)
-#=> 6
-tokens[0].surface()
-#=> 'まぁ'
-tokens[0].tag(0)
-#=> '名詞'
-tokens[0].tag(1)
-#=> 'マー'
-[token.surface() for token in tokens]
-#=> ['まぁ', '社長', 'は', '火星', '猫', 'だ']
 ```
 
+## Note for KyTea's models
+
 You can also use KyTea's models as follows:
 
 ```python
-with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:
-    model = fp.read()
+>>> with open('path/to/jp-0.4.7-5.mod', 'rb') as fp:  # doctest: +SKIP
+...     tokenizer = vaporetto.Vaporetto.create_from_kytea_model(fp.read())
 
-tokenizer = vaporetto.Vaporetto.create_from_kytea_model(model)
 ```
 
 Note: Vaporetto does not support tag prediction with KyTea's models.
 
 ## [Speed Comparison](https://github.com/daac-tools/python-vaporetto/wiki/Speed-Comparison)
 
 ## License
```

