# Comparing `tmp/pzflow-3.0.3.tar.gz` & `tmp/pzflow-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzflow-3.0.3.tar", max compression
+gzip compressed data, was "pzflow-3.1.0.tar", max compression
```

## Comparing `pzflow-3.0.3.tar` & `pzflow-3.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-02-03 06:14:54.216585 pzflow-3.0.3/LICENSE
--rw-r--r--   0        0        0     3018 2023-02-03 06:14:54.216704 pzflow-3.0.3/README.md
--rw-r--r--   0        0        0     1293 2023-02-03 06:40:33.078982 pzflow-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      135 2023-02-03 06:40:33.079096 pzflow-3.0.3/pzflow/__init__.py
--rw-r--r--   0        0        0    29958 2023-02-03 06:14:54.226135 pzflow-3.0.3/pzflow/bijectors.py
--rw-r--r--   0        0        0    18084 2023-02-03 06:40:33.079260 pzflow-3.0.3/pzflow/distributions.py
--rw-r--r--   0        0        0   800708 2023-02-03 06:14:54.228590 pzflow-3.0.3/pzflow/example_files/checkerboard-data.pkl
--rw-r--r--   0        0        0  2219977 2023-02-03 06:14:54.236794 pzflow-3.0.3/pzflow/example_files/city-data.pkl
--rw-r--r--   0        0        0  1158452 2023-02-03 06:14:54.243130 pzflow-3.0.3/pzflow/example_files/example-flow.pzflow.pkl
--rw-r--r--   0        0        0  5600784 2023-02-03 06:14:54.275089 pzflow-3.0.3/pzflow/example_files/galaxy-data.pkl
--rw-r--r--   0        0        0  1600708 2023-02-03 06:14:54.284005 pzflow-3.0.3/pzflow/example_files/two-moons-data.pkl
--rw-r--r--   0        0        0     4847 2023-02-03 06:14:54.284171 pzflow-3.0.3/pzflow/examples.py
--rw-r--r--   0        0        0    42816 2023-02-03 06:14:54.284386 pzflow-3.0.3/pzflow/flow.py
--rw-r--r--   0        0        0    25027 2023-02-03 06:14:54.284652 pzflow-3.0.3/pzflow/flowEnsemble.py
--rw-r--r--   0        0        0     8206 2023-02-03 06:14:54.284767 pzflow-3.0.3/pzflow/utils.py
--rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 pzflow-3.0.3/setup.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 pzflow-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-04-06 21:13:39.820423 pzflow-3.1.0/LICENSE
+-rw-r--r--   0        0        0     3018 2023-04-06 21:13:39.823423 pzflow-3.1.0/README.md
+-rw-r--r--   0        0        0     1293 2023-04-12 19:35:47.784964 pzflow-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-04-12 19:35:47.786965 pzflow-3.1.0/pzflow/__init__.py
+-rw-r--r--   0        0        0    29958 2023-04-06 21:13:39.927422 pzflow-3.1.0/pzflow/bijectors.py
+-rw-r--r--   0        0        0    18084 2023-04-11 18:20:35.939054 pzflow-3.1.0/pzflow/distributions.py
+-rw-r--r--   0        0        0   800708 2023-04-06 21:13:39.948422 pzflow-3.1.0/pzflow/example_files/checkerboard-data.pkl
+-rw-r--r--   0        0        0  2219977 2023-04-06 21:13:39.991422 pzflow-3.1.0/pzflow/example_files/city-data.pkl
+-rw-r--r--   0        0        0  1158452 2023-04-06 21:13:40.016421 pzflow-3.1.0/pzflow/example_files/example-flow.pzflow.pkl
+-rw-r--r--   0        0        0  5600784 2023-04-06 21:13:40.135421 pzflow-3.1.0/pzflow/example_files/galaxy-data.pkl
+-rw-r--r--   0        0        0  1600708 2023-04-06 21:13:40.169420 pzflow-3.1.0/pzflow/example_files/two-moons-data.pkl
+-rw-r--r--   0        0        0     4847 2023-04-06 21:13:40.172420 pzflow-3.1.0/pzflow/examples.py
+-rw-r--r--   0        0        0    45183 2023-04-12 19:35:47.793964 pzflow-3.1.0/pzflow/flow.py
+-rw-r--r--   0        0        0    25652 2023-04-12 19:35:47.798964 pzflow-3.1.0/pzflow/flowEnsemble.py
+-rw-r--r--   0        0        0     8206 2023-04-11 20:07:53.618947 pzflow-3.1.0/pzflow/utils.py
+-rw-r--r--   0        0        0     3902 2023-04-13 19:05:29.602088 pzflow-3.1.0/setup.py
+-rw-r--r--   0        0        0     3821 2023-04-13 19:05:29.602379 pzflow-3.1.0/PKG-INFO
```

### Comparing `pzflow-3.0.3/LICENSE` & `pzflow-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/README.md` & `pzflow-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pyproject.toml` & `pzflow-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pzflow"
-version = "3.0.3"
+version = "3.1.0"
 description = "Probabilistic modeling of tabular data with normalizing flows."
 authors = ["John Franklin Crenshaw <jfcrenshaw@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/jfcrenshaw/pzflow"
 readme = "README.md"
```

### Comparing `pzflow-3.0.3/pzflow/bijectors.py` & `pzflow-3.1.0/pzflow/bijectors.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/distributions.py` & `pzflow-3.1.0/pzflow/distributions.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/example_files/checkerboard-data.pkl` & `pzflow-3.1.0/pzflow/example_files/checkerboard-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/example_files/city-data.pkl` & `pzflow-3.1.0/pzflow/example_files/city-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/example_files/example-flow.pzflow.pkl` & `pzflow-3.1.0/pzflow/example_files/example-flow.pzflow.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/example_files/galaxy-data.pkl` & `pzflow-3.1.0/pzflow/example_files/galaxy-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/example_files/two-moons-data.pkl` & `pzflow-3.1.0/pzflow/example_files/two-moons-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/examples.py` & `pzflow-3.1.0/pzflow/examples.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/pzflow/flow.py` & `pzflow-3.1.0/pzflow/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,14 @@
                     "If providing a dictionary, please do not provide any other parameters."
                 )
         if file is not None and _dictionary is not None:
             raise ValueError("Only provide file or _dictionary, not both.")
 
         # if file or dictionary is provided, load everything from it
         if file is not None or _dictionary is not None:
-
             save_dict = self._save_dict()
             if file is not None:
                 with open(file, "rb") as handle:
                     save_dict.update(pickle.load(handle))
             else:
                 save_dict.update(_dictionary)
 
@@ -289,15 +288,17 @@
 
         # check if params were passed
         bijector_params = params if params is not None else bijector_params
 
         # save the bijector params along with the latent params
         self._params = (self.latent._params, bijector_params)
 
-    def _set_default_bijector(self, inputs: pd.DataFrame, seed: int = 0) -> None:
+    def _set_default_bijector(
+        self, inputs: pd.DataFrame, seed: int = 0
+    ) -> None:
         # Set the default bijector
         # which is ShiftBounds -> RollingSplineCoupling
 
         # get the min/max for each data column
         data = inputs[list(self.data_columns)].to_numpy()
         mins = data.min(axis=0)
         maxs = data.max(axis=0)
@@ -307,15 +308,15 @@
             0
             if self.conditional_columns is None
             else len(self.conditional_columns)
         )
 
         self.set_bijector(
             Chain(
-                ShiftBounds(mins, maxs, 4.),
+                ShiftBounds(mins, maxs, 4.0),
                 RollingSplineCoupling(
                     len(self.data_columns), n_conditions=n_conditions
                 ),
             ),
             seed=seed,
         )
 
@@ -552,15 +553,14 @@
 
         # empty array to hold pdfs
         pdfs = jnp.zeros((nrows, len(grid)))
 
         # if marginalization rules were passed, we will loop over the rules
         # and repeatedly call this method
         if marg_rules is not None:
-
             # if the flag is NaN, we must use jnp.isnan to check for flags
             if np.isnan(marg_rules["flag"]):
 
                 def check_flags(data):
                     return np.isnan(data)
 
             # else we use jnp.isclose to check for flags
@@ -593,15 +593,14 @@
 
             # we will keep track of all the rows we've already calculated
             # posteriors for
             already_done = unflagged_idx
 
             # now we will loop over the rules in marg_rules
             for name, rule in marg_rules.items():
-
                 # ignore the flag, because that's not a column in the data
                 if name == "flag":
                     continue
 
                 # get the list of new rows for which we need to calculate posteriors
                 flagged_idx = inputs[check_flags(inputs[name])].index.tolist()
                 flagged_idx = list(set(flagged_idx).difference(already_done))
@@ -661,18 +660,16 @@
                 )
 
                 # add these flagged indices to the list of rows already done
                 already_done += flagged_idx
 
         # now for the main posterior calculation loop
         else:
-
             # loop through batches
             for batch_idx in range(0, nrows, batch_size):
-
                 # get the data batch
                 # and, if this is a conditional flow, the correpsonding conditions
                 batch = inputs.iloc[batch_idx : batch_idx + batch_size]
 
                 # if not drawing samples, just grab batch and conditions
                 if err_samples is None:
                     conditions = self._get_conditions(batch)
@@ -866,31 +863,36 @@
 
         with open(file, "wb") as handle:
             pickle.dump(save_dict, handle, recurse=True)
 
     def train(
         self,
         inputs: pd.DataFrame,
+        val_set: pd.DataFrame = None,
         epochs: int = 100,
         batch_size: int = 1024,
         optimizer: Callable = None,
         loss_fn: Callable = None,
         convolve_errs: bool = False,
         patience: int = None,
+        best_params: bool = True,
         seed: int = 0,
         verbose: bool = False,
         progress_bar: bool = False,
     ) -> list:
         """Trains the normalizing flow on the provided inputs.
 
         Parameters
         ----------
         inputs : pd.DataFrame
             Data on which to train the normalizing flow.
             Must have columns matching `self.data_columns`.
+        val_set : pd.DataFrame; default=None
+            Validation set, of same format as inputs. If provided,
+            validation loss will be calculated at the end of each epoch.
         epochs : int; default=100
             Number of epochs to train.
         batch_size : int; default=1024
             Batch size for training.
         optimizer : optax optimizer
             An optimizer from Optax. default = optax.adam(learning_rate=1e-3)
             see https://optax.readthedocs.io/en/latest/index.html for more.
@@ -902,29 +904,38 @@
             each epoch of training. Method will look for error columns in
             `inputs`. Error columns must end in `_err`. E.g. the error column
             for the variable `u` must be `u_err`. Zero error assumed for
             any missing error columns. The error distribution is set during
             flow instantiation.
         patience : int; optional
             Factor that controls early stopping. Training will stop if the
-            loss doesn't decrease for this number of epochs.
+            loss doesn't decrease for this number of epochs. Note if a
+            validation set is provided, the validation loss is used.
+        best_params : bool; default=True
+            Whether to use the params from the epoch with the lowest loss.
+            Note if a validation set is provided, the epoch with the lowest
+            validation loss is chosen. If False, the params from the final
+            epoch are saved.
         seed : int; default=0
             A random seed to control the batching and the (optional)
             error sampling and creating the default bijector (the latter
             only happens if you didn't set up the bijector during Flow
             instantiation).
         verbose : bool; default=False
             If true, print the training loss every 5% of epochs.
         progress_bar : bool; default=False
             If true, display a tqdm progress bar during training.
 
         Returns
         -------
         list
-            List of training losses from every epoch.
+            List of training losses from every epoch. If no val_set provided,
+            these are just training losses. If val_set is provided, then the
+            first element is the list of training losses, while the second is
+            the list of validation losses.
         """
 
         # split the seed
         rng = np.random.default_rng(seed)
         batch_seed, bijector_seed = rng.integers(1e9, size=2)
 
         # if the bijector is None, set the default bijector
@@ -994,33 +1005,42 @@
 
         if verbose:
             print(f"Training {epochs} epochs \nLoss:")
 
         # save the initial loss
         X = jnp.array(inputs[columns].to_numpy())
         C = self._get_conditions(inputs)
-        losses = [loss_fn(model_params, X, C)]
+        losses = [loss_fn(model_params, X, C).item()]
+
+        if val_set is not None:
+            Xval = jnp.array(val_set[columns].to_numpy())
+            Cval = self._get_conditions(val_set)
+            val_losses = [loss_fn(model_params, Xval, Cval).item()]
+
         if verbose:
-            print(f"(0) {losses[-1]:.4f}")
+            if val_set is None:
+                print(f"(0) {losses[-1]:.4f}")
+            else:
+                print(f"(0) {losses[-1]:.4f}  {val_losses[-1]:.4f}")
 
         # initialize variables for early stopping
         best_loss = jnp.inf
+        best_param_vals = model_params
         early_stopping_counter = 0
 
         # loop through training
         loop = tqdm(range(epochs)) if progress_bar else range(epochs)
         for epoch in loop:
             # new permutation of batches
             permute_key, sample_key, key = random.split(key, num=3)
             idx = random.permutation(permute_key, inputs.shape[0])
             X = inputs.iloc[idx]
 
             # loop through batches and step optimizer
             for batch_idx in range(0, len(X), batch_size):
-
                 # if sampling from the error distribution, this returns a
                 # Gaussian sample of the batch. Else just returns batch as a
                 # jax array
                 batch = get_batch(
                     sample_key,
                     X.iloc[batch_idx : batch_idx + batch_size],
                     type="data",
@@ -1040,43 +1060,74 @@
 
             # save end-of-epoch training loss
             losses.append(
                 loss_fn(
                     model_params,
                     jnp.array(X[columns].to_numpy()),
                     self._get_conditions(X),
-                )
+                ).item()
             )
 
+            # and validation loss
+            if val_set is not None:
+                val_losses.append(loss_fn(model_params, Xval, Cval).item())
+
             # if verbose, print current loss
             if verbose and (
                 epoch % max(int(0.05 * epochs), 1) == 0
                 or (epoch + 1) == epochs
             ):
-                print(f"({epoch+1}) {losses[-1]:.4f}")
+                if val_set is None:
+                    print(f"({epoch+1}) {losses[-1]:.4f}")
+                else:
+                    print(
+                        f"({epoch+1}) {losses[-1]:.4f}  {val_losses[-1]:.4f}"
+                    )
 
             # if patience provided, we need to check for early stopping
-            if patience is not None:
+            if patience is not None or best_loss:
+                if val_set is None:
+                    tracked_losses = losses
+                else:
+                    tracked_losses = val_losses
 
                 # if loss didn't improve, increase counter
                 # and check early stopping criterion
-                if losses[-1] >= best_loss or jnp.isclose(
-                    losses[-1], best_loss
+                if tracked_losses[-1] >= best_loss or jnp.isclose(
+                    tracked_losses[-1], best_loss
                 ):
                     early_stopping_counter += 1
 
                     # check if the early stopping criterion is met
-                    if early_stopping_counter >= patience:
+                    if (
+                        patience is not None
+                        and early_stopping_counter >= patience
+                    ):
                         print(
                             "Early stopping criterion is met.",
-                            f"Training stopping after epoch {epoch}.",
+                            f"Training stopping after epoch {epoch+1}.",
                         )
                         break
                 # if this is the best loss, reset the counter
                 else:
-                    best_loss = losses[-1]
+                    best_loss = tracked_losses[-1]
+                    best_param_vals = model_params
                     early_stopping_counter = 0
 
+            # break if the training loss is NaN
+            if not np.isfinite(losses[-1]):
+                print(
+                    f"Training stopping after epoch {epoch+1}",
+                    "because training loss diverged.",
+                )
+                break
+
         # update the flow parameters with the final training state
-        self._params = model_params
+        if best_params:
+            self._params = best_param_vals
+        else:
+            self._params = model_params
 
-        return losses
+        if val_set is None:
+            return losses
+        else:
+            return [losses, val_losses]
```

### Comparing `pzflow-3.0.3/pzflow/flowEnsemble.py` & `pzflow-3.1.0/pzflow/flowEnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         ):
             raise ValueError(
                 "If providing a file, please do not provide any other parameters."
             )
 
         # if file is provided, load everything from the file
         if file is not None:
-
             # load the file
             with open(file, "rb") as handle:
                 save_dict = pickle.load(handle)
 
             # make sure the saved file is for this class
             c = save_dict.pop("class")
             if c != self.__class__.__name__:
@@ -502,31 +501,36 @@
 
         with open(file, "wb") as handle:
             pickle.dump(save_dict, handle, recurse=True)
 
     def train(
         self,
         inputs: pd.DataFrame,
+        val_set: pd.DataFrame = None,
         epochs: int = 50,
         batch_size: int = 1024,
         optimizer: Callable = None,
         loss_fn: Callable = None,
         convolve_errs: bool = False,
         patience: int = None,
+        best_params: bool = True,
         seed: int = 0,
         verbose: bool = False,
         progress_bar: bool = False,
     ) -> dict:
         """Trains the normalizing flows on the provided inputs.
 
         Parameters
         ----------
         inputs : pd.DataFrame
             Data on which to train the normalizing flows.
             Must have columns matching self.data_columns.
+        val_set : pd.DataFrame; default=None
+            Validation set, of same format as inputs. If provided,
+            validation loss will be calculated at the end of each epoch.
         epochs : int; default=50
             Number of epochs to train.
         batch_size : int; default=1024
             Batch size for training.
         optimizer : optax optimizer
             An optimizer from Optax. default = optax.adam(learning_rate=1e-3)
             see https://optax.readthedocs.io/en/latest/index.html for more.
@@ -539,14 +543,19 @@
             `inputs`. Error columns must end in `_err`. E.g. the error column
             for the variable `u` must be `u_err`. Zero error assumed for
             any missing error columns. The error distribution is set during
             ensemble instantiation.
         patience : int; optional
             Factor that controls early stopping. Training will stop if the
             loss doesn't decrease for this number of epochs.
+        best_params : bool; default=True
+            Whether to use the params from the epoch with the lowest loss.
+            Note if a validation set is provided, the epoch with the lowest
+            validation loss is chosen. If False, the params from the final
+            epoch are saved.
         seed : int; default=0
             A random seed to control the batching and the (optional)
             error sampling.
         verbose : bool; default=False
             If true, print the training loss every 5% of epochs.
         progress_bar : bool; default=False
             If true, display a tqdm progress bar during training.
@@ -561,25 +570,26 @@
         # generate random seeds for each flow
         rng = np.random.default_rng(seed)
         seeds = rng.integers(1e9, size=len(self._ensemble))
 
         loss_dict = dict()
 
         for i, (name, flow) in enumerate(self._ensemble.items()):
-
             if verbose:
                 print(name)
 
             loss_dict[name] = flow.train(
                 inputs=inputs,
+                val_set=val_set,
                 epochs=epochs,
                 batch_size=batch_size,
                 optimizer=optimizer,
                 loss_fn=loss_fn,
                 convolve_errs=convolve_errs,
                 patience=patience,
+                best_params=best_params,
                 seed=seeds[i],
                 verbose=verbose,
                 progress_bar=progress_bar,
             )
 
         return loss_dict
```

### Comparing `pzflow-3.0.3/pzflow/utils.py` & `pzflow-3.1.0/pzflow/utils.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.0.3/setup.py` & `pzflow-3.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
  'jaxlib>=0.4.2,<0.5.0',
  'optax>=0.1.4,<0.2.0',
  'pandas>=1.1',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'pzflow',
-    'version': '3.0.3',
+    'version': '3.1.0',
     'description': 'Probabilistic modeling of tabular data with normalizing flows.',
     'long_description': '![build](https://github.com/jfcrenshaw/pzflow/workflows/build/badge.svg)\n[![codecov](https://codecov.io/gh/jfcrenshaw/pzflow/branch/main/graph/badge.svg?token=qR5cey0swQ)](https://codecov.io/gh/jfcrenshaw/pzflow)\n[![PyPI version](https://badge.fury.io/py/pzflow.svg)](https://badge.fury.io/py/pzflow)\n[![DOI](https://zenodo.org/badge/327498448.svg)](https://zenodo.org/badge/latestdoi/327498448)\n[![Docs](https://img.shields.io/badge/Docs-https%3A%2F%2Fjfcrenshaw.github.io%2Fpzflow%2F-red)](https://jfcrenshaw.github.io/pzflow/)\n\n# PZFlow\n\nPZFlow is a python package for probabilistic modeling of tabular data with normalizing flows.\n\nIf your data consists of continuous variables that can be put into a Pandas DataFrame, pzflow can model the joint probability distribution of your data set.\n\nThe `Flow` class makes building and training a normalizing flow simple.\nIt also allows you to easily sample from the normalizing flow (e.g., for forward modeling or data augmentation), and calculate posteriors over any of your variables.\n\nThere are several tutorial notebooks in the [docs](https://jfcrenshaw.github.io/pzflow/tutorials/).\n\n## Installation\n\nSee the instructions in the [docs](https://jfcrenshaw.github.io/pzflow/install/).\n\n## Citation\n\nWe are preparing a paper on pzflow.\nIf you use this package in your research, please check back here for a citation before publication.\nIn the meantime, please cite the [Zenodo release](https://zenodo.org/badge/latestdoi/327498448).\n\n### Sources\n\nPZFlow was originally designed for forward modeling of photometric redshifts as a part of the Creation Module of the [DESC](https://lsstdesc.org/) [RAIL](https://github.com/LSSTDESC/RAIL) project.\nThe idea to use normalizing flows for photometric redshifts originated with [Bryce Kalmbach](https://github.com/jbkalmbach).\nThe earliest version of the normalizing flow in RAIL was based on a notebook by [Francois Lanusse](https://github.com/eiffl) and included contributions from [Alex Malz](https://github.com/aimalz).\n\nThe functional jax structure of the bijectors was originally based on [`jax-flows`](https://github.com/ChrisWaites/jax-flows) by [Chris Waites](https://github.com/ChrisWaites). The implementation of the Neural Spline Coupling is largely based on the [Tensorflow implementation](https://github.com/tensorflow/probability/blob/master/tensorflow_probability/python/bijectors/rational_quadratic_spline.py), with some inspiration from [`nflows`](https://github.com/bayesiains/nflows/).\n\nNeural Spline Flows are based on the following papers:\n\n  > [NICE: Non-linear Independent Components Estimation](https://arxiv.org/abs/1410.8516)\\\n  > Laurent Dinh, David Krueger, Yoshua Bengio\\\n  > _arXiv:1410.8516_\n\n  > [Density estimation using Real NVP](https://arxiv.org/abs/1605.08803)\\\n  > Laurent Dinh, Jascha Sohl-Dickstein, Samy Bengio\\\n  > _arXiv:1605.08803_\n\n  > [Neural Spline Flows](https://arxiv.org/abs/1906.04032)\\\n  > Conor Durkan, Artur Bekasov, Iain Murray, George Papamakarios\\\n  > _arXiv:1906.04032_\n',
     'author': 'John Franklin Crenshaw',
     'author_email': 'jfcrenshaw@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/jfcrenshaw/pzflow',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8.1,<4.0.0',
 }
```

### Comparing `pzflow-3.0.3/PKG-INFO` & `pzflow-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pzflow
-Version: 3.0.3
+Version: 3.1.0
 Summary: Probabilistic modeling of tabular data with normalizing flows.
 Home-page: https://github.com/jfcrenshaw/pzflow
 License: MIT
 Author: John Franklin Crenshaw
 Author-email: jfcrenshaw@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: jax (>=0.4.2,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.2,<0.5.0)
 Requires-Dist: optax (>=0.1.4,<0.2.0)
 Requires-Dist: pandas (>=1.1)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/jfcrenshaw/pzflow
```

