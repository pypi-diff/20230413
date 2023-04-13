# Comparing `tmp/rust_statespace-0.1.4.tar.gz` & `tmp/rust_statespace-0.1.5.tar.gz`

## Comparing `rust_statespace-0.1.4.tar` & `rust_statespace-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.4/Cargo.toml
--rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/.gitignore
--rw-r--r--   0      501       20    32753 2023-04-10 16:04:47.000000 rust_statespace-0.1.4/Cargo.lock
--rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.4/data/nile.csv
--rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/pyproject.toml
--rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.4/requirements_rust.txt
--rw-r--r--   0      501       20     7607 2023-04-10 16:03:50.000000 rust_statespace-0.1.4/src/glm.rs
--rw-r--r--   0      501       20     1839 2023-04-10 15:54:51.000000 rust_statespace-0.1.4/src/lib.rs
--rw-r--r--   0      501       20      862 2023-04-10 15:59:48.000000 rust_statespace-0.1.4/src/main.rs
--rw-r--r--   0      501       20     1041 2023-04-10 15:57:34.000000 rust_statespace-0.1.4/src/read_data.rs
--rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.5/Cargo.toml
+-rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.5/.gitignore
+-rw-r--r--   0      501       20    32753 2023-04-13 15:16:30.000000 rust_statespace-0.1.5/Cargo.lock
+-rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.5/data/nile.csv
+-rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.5/pyproject.toml
+-rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.5/requirements_rust.txt
+-rw-r--r--   0      501       20     7595 2023-04-13 15:19:20.000000 rust_statespace-0.1.5/src/glm.rs
+-rw-r--r--   0      501       20     1839 2023-04-10 15:54:51.000000 rust_statespace-0.1.5/src/lib.rs
+-rw-r--r--   0      501       20      862 2023-04-10 15:59:48.000000 rust_statespace-0.1.5/src/main.rs
+-rw-r--r--   0      501       20     1041 2023-04-10 15:57:34.000000 rust_statespace-0.1.5/src/read_data.rs
+-rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.5/PKG-INFO
```

### Comparing `rust_statespace-0.1.4/.github/workflows/CI.yml` & `rust_statespace-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.4/.gitignore` & `rust_statespace-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.4/Cargo.lock` & `rust_statespace-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
  "getrandom 0.2.9",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "rust_statespace"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "csv",
  "ndarray",
  "ndarray-linalg",
  "numpy",
  "pyo3",
 ]
```

### Comparing `rust_statespace-0.1.4/data/nile.csv` & `rust_statespace-0.1.5/data/nile.csv`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.4/src/glm.rs` & `rust_statespace-0.1.5/src/glm.rs`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
             
             // in first iteration: set first values of a and P and compute corresponding v and F
             // TODO: add diffuse initialization
             // TODO: add incasting
             if i == 0 {
 
                 // set a_0 and P_0
-                a_temp.assign(&arr2(&[[0.0], [0.0]]));
-                P_temp.assign(&arr2(&[[1.0e4, 0.0], [0.0, 1.0e4]]));
+                a_temp.assign(&Array2::zeros((p, 1)));
+                P_temp.assign(&(1e6 * &Array2::eye(p)));
 
                 // get y_0
                 let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
 
                 // get first error and error variance: v and F
                 v_temp.assign(&(
                     &y_temp - &self.Z.dot(&a_temp))
```

### Comparing `rust_statespace-0.1.4/src/lib.rs` & `rust_statespace-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.4/src/main.rs` & `rust_statespace-0.1.5/src/main.rs`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.4/src/read_data.rs` & `rust_statespace-0.1.5/src/read_data.rs`

 * *Files identical despite different names*

