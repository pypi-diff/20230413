# Comparing `tmp/auto_vicuna-0.2.0.tar.gz` & `tmp/auto_vicuna-0.2.1.tar.gz`

## Comparing `auto_vicuna-0.2.0.tar` & `auto_vicuna-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.sourcery.yaml
--rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/InteractiveManual.ipynb
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/clean_all.sh
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/convert_llama_names.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/qa.sh
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/run_pylint.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/special_tokens_map.json
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/style.sh
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/tokenizer_config.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/__init__.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/__main__.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/config.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/conversation.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/src/auto_vicuna/plugins.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/LICENSE
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/README.md
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 auto_vicuna-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.sourcery.yaml
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/InteractiveManual.ipynb
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/clean_all.sh
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/convert_llama_names.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/qa.sh
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/run_pylint.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/special_tokens_map.json
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/style.sh
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/tokenizer_config.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/__init__.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/__main__.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/config.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/conversation.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/src/auto_vicuna/plugins.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/README.md
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 auto_vicuna-0.2.1/PKG-INFO
```

### Comparing `auto_vicuna-0.2.0/.coveragerc` & `auto_vicuna-0.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/.pre-commit-config.yaml` & `auto_vicuna-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/.sourcery.yaml` & `auto_vicuna-0.2.1/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/InteractiveManual.ipynb` & `auto_vicuna-0.2.1/InteractiveManual.ipynb`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/convert_llama_names.py` & `auto_vicuna-0.2.1/convert_llama_names.py`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/pylintrc` & `auto_vicuna-0.2.1/pylintrc`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/tokenizer_config.json` & `auto_vicuna-0.2.1/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/src/auto_vicuna/__main__.py` & `auto_vicuna-0.2.1/src/auto_vicuna/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     num_gpus: int = 1,
     device: str = DEVICE,
     debug: bool = False,
     load_8bit: bool = False,
     plugins_path: Path = Path(os.getcwd()) / "plugins",
 ) -> None:
     """Auto-Vicuna: A Python package for automatically generating Vicuna randomness."""
-    click.echo(f"Auto-Vicuna\n===========\nVersion: 0.1.0\nWeights: {vicuna_weights}")
+    click.echo(f"Auto-Vicuna\n===========\nVersion: 0.2.1\nWeights: {vicuna_weights}")
     click.echo(f"Device: {device}\nTorch version: {torch.__version__}")
     if "cpu" in torch.__version__:
         click.echo("\nError: CPU not supported. Install a GPU version of PyTorch.")
         click.echo("See https://pytorch.org/get-started/locally/ for more info.\n")
         sys.exit(1)
     try:
         model, tokenizer = load_model(
```

### Comparing `auto_vicuna-0.2.0/src/auto_vicuna/chat.py` & `auto_vicuna-0.2.1/src/auto_vicuna/chat.py`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/src/auto_vicuna/conversation.py` & `auto_vicuna-0.2.1/src/auto_vicuna/conversation.py`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/src/auto_vicuna/plugins.py` & `auto_vicuna-0.2.1/src/auto_vicuna/plugins.py`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/.gitignore` & `auto_vicuna-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/LICENSE` & `auto_vicuna-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/README.md` & `auto_vicuna-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_vicuna-0.2.0/pyproject.toml` & `auto_vicuna-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto_vicuna"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "An experiment with Vicuna."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `auto_vicuna-0.2.0/PKG-INFO` & `auto_vicuna-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vicuna
-Version: 0.2.0
+Version: 0.2.1
 Summary: An experiment with Vicuna.
 Project-URL: Homepage, https://github.com/BillSchumacher/Auto-Vicuna
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Auto-Vicuna/issues
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

