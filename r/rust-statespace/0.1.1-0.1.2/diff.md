# Comparing `tmp/rust_statespace-0.1.1.tar.gz` & `tmp/rust_statespace-0.1.2.tar.gz`

## Comparing `rust_statespace-0.1.1.tar` & `rust_statespace-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 rust_statespace-0.1.1/Cargo.toml
--rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.1/.gitignore
--rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.1/pyproject.toml
--rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.1/requirements_rust.txt
--rw-r--r--   0      501       20     6047 2023-04-07 15:21:03.000000 rust_statespace-0.1.1/src/glm.rs
--rw-r--r--   0      501       20        0 2023-04-07 13:32:17.000000 rust_statespace-0.1.1/src/kalman.rs
--rw-r--r--   0      501       20     1548 2023-04-08 10:21:21.000000 rust_statespace-0.1.1/src/lib.rs
--rw-r--r--   0      501       20    31710 2023-04-08 10:21:56.000000 rust_statespace-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/.gitignore
+-rw-r--r--   0      501       20    32753 2023-04-10 14:44:01.000000 rust_statespace-0.1.2/Cargo.lock
+-rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.2/data/nile.csv
+-rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.2/requirements_rust.txt
+-rw-r--r--   0      501       20     5850 2023-04-10 14:43:24.000000 rust_statespace-0.1.2/src/glm.rs
+-rw-r--r--   0      501       20     1639 2023-04-08 13:48:17.000000 rust_statespace-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20      876 2023-04-08 13:37:57.000000 rust_statespace-0.1.2/src/main.rs
+-rw-r--r--   0      501       20     1097 2023-04-08 13:31:03.000000 rust_statespace-0.1.2/src/read_data.rs
+-rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.2/PKG-INFO
```

### Comparing `rust_statespace-0.1.1/.github/workflows/CI.yml` & `rust_statespace-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.1/.gitignore` & `rust_statespace-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.1/src/glm.rs` & `rust_statespace-0.1.2/src/glm.rs`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 
 use std::{
     f64,
     error::Error,
 };
 
 // only put the variables required to compute filters in the struct
-// 1. 
 #[allow(non_snake_case)]
 pub struct GLM {
 
     // fixed
-    T: Array2<f64>,
-    H: Array2<f64>,
-    Q: Array2<f64>,
-    Z: Array2<f64>,
-    R: Array2<f64>,
-    y: Array3<f64>,
+    pub T: Array2<f64>,
+    pub H: Array2<f64>,
+    pub Q: Array2<f64>,
+    pub Z: Array2<f64>,
+    pub R: Array2<f64>,
+    pub y: Array3<f64>,
 
-    // filters
 }
 
 #[allow(non_snake_case, dead_code)]
 impl GLM {
 
     // create a new Gaussian Linear Model
     pub fn new(T: Array2<f64>, H: Array2<f64>, Q: Array2<f64>, Z: Array2<f64>, R: Array2<f64>, y:Array3<f64>) -> GLM {
@@ -37,44 +35,47 @@
         }
     }
 
     // Run Kalman Filter on instance variables
     pub fn kalman_filter(&self) -> Result<(Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>), Box<dyn Error>> {
 
         let T = self.y.len();
-        let mut axes_iterator: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((1, 1, T));
+        let p = self.T.ncols();
+        let s: usize = self.Z.nrows();
 
-        let mut a_3d: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((2, 1, T));
-        let mut v_3d: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((1, 1, T));
-        let mut F_3d: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((1, 1, T));
-        let mut P_3d: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((2, 2, T));
-        let mut K_3d: ArrayBase<OwnedRepr<f64>, _> = Array3::zeros((2, 1, T));
+        let mut axes_iterator: Array3<f64> = Array3::zeros((1, 1, T));
+
+        let mut a_3d: Array3<f64> = Array3::zeros((p, 1, T));
+        let mut v_3d: Array3<f64> = Array3::zeros((s, 1, T));
+        let mut F_3d: Array3<f64> = Array3::zeros((s, s, T));
+        let mut P_3d: Array3<f64> = Array3::zeros((p, p, T));
+        let mut K_3d: Array3<f64> = Array3::zeros((p, s, T));
         
-        let mut a_prev: ArrayBase<OwnedRepr<f64>, _> = Array2::zeros((2, 1));
-        let mut v_prev: ArrayBase<OwnedRepr<f64>, _> = Array2::zeros((1, 1));
-        let mut F_prev: ArrayBase<OwnedRepr<f64>, _> = Array2::zeros((1, 1));
-        let mut P_prev: ArrayBase<OwnedRepr<f64>, _> = Array2::zeros((2, 2));
-        let mut K_prev: ArrayBase<OwnedRepr<f64>, _> = Array2::zeros((2, 1));
+        let mut a_prev: Array2<f64> = Array2::zeros((p, 1));
+        let mut v_prev: Array2<f64> = Array2::zeros((s, 1));
+        let mut F_prev: Array2<f64> = Array2::zeros((s, s));
+        let mut P_prev: Array2<f64> = Array2::zeros((p, p));
+        let mut K_prev: Array2<f64> = Array2::zeros((p, s));
 
         // need to enumerate to use i
         for (i, _) in axes_iterator.axis_iter_mut(Axis(2)).enumerate() {
             
             // retrieve slices of the data
-            let mut a_temp: ArrayBase<ViewRepr<&mut f64>, _> = a_3d.slice_mut(s![..,..,i]);
-            let mut v_temp: ArrayBase<ViewRepr<&mut f64>, _> = v_3d.slice_mut(s![..,..,i]);
-            let mut F_temp: ArrayBase<ViewRepr<&mut f64>, _> = F_3d.slice_mut(s![..,..,i]);
-            let mut P_temp: ArrayBase<ViewRepr<&mut f64>, _> = P_3d.slice_mut(s![..,..,i]);
-            let mut K_temp: ArrayBase<ViewRepr<&mut f64>, _> = K_3d.slice_mut(s![..,..,i]);
-
+            let mut a_temp: ArrayViewMut2<f64> = a_3d.slice_mut(s![..,..,i]);
+            let mut v_temp: ArrayViewMut2<f64> = v_3d.slice_mut(s![..,..,i]);
+            let mut F_temp: ArrayViewMut2<f64> = F_3d.slice_mut(s![..,..,i]);
+            let mut P_temp: ArrayViewMut2<f64> = P_3d.slice_mut(s![..,..,i]);
+            let mut K_temp: ArrayViewMut2<f64> = K_3d.slice_mut(s![..,..,i]);
+            
             // in first iteration: set first values of a and P and compute corresponding v and F
             // TODO: add diffuse initialization
             if i == 0 {
 
                 // get y_0
-                let y_temp: ArrayBase<ViewRepr<&f64>, _> = self.y.slice(s![.., .., i]);
+                let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
 
                 // set a_0 and P_0
                 a_temp.assign(&arr2(&[[0.0], [0.0]]));
                 P_temp.assign(&arr2(&[[1.0, 0.0], [0.0, 1.0]]));
 
                 // get first error and error variance: v and F
                 v_temp.assign(&(
@@ -124,15 +125,15 @@
                             &F_prev.dot(
                                 &K_prev.t()
                         )
                     ))
                 ); 
                 
                 // get current y
-                let y_temp: ArrayBase<ViewRepr<&f64>, _> = self.y.slice(s![.., .., i]);
+                let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
                 
                 // get prediction error
                 v_temp.assign(&(
                     &y_temp - &self.Z.dot(&a_temp)
                 ));
 
                 // get prediction error variance
```

### Comparing `rust_statespace-0.1.1/src/lib.rs` & `rust_statespace-0.1.2/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mod glm;
 
 use numpy::ndarray::{ArrayD, ArrayViewD, ArrayViewMutD};
-use numpy::{IntoPyArray, PyArrayDyn, PyReadonlyArrayDyn, PyReadonlyArray2, PyReadonlyArray3, PyArray3};
+use numpy::{IntoPyArray, PyArrayDyn, PyReadonlyArrayDyn, PyReadonlyArray2, PyReadonlyArray3, PyArray2, PyArray3};
 use pyo3::{pymodule, types::PyModule, PyResult, Python};
 use glm::GLM;
 
 #[pymodule]
 fn rust_statespace(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
 
     // wrapper of kalman filter
@@ -32,19 +32,21 @@
         let T = T.as_array().to_owned();
         let H = H.as_array().to_owned();
         let Q = Q.as_array().to_owned();
         let Z = Z.as_array().to_owned();
         let R = R.as_array().to_owned();
         let y = y.as_array().to_owned();
 
-        // instantiate the 
+        // instantiate the GLM
         let LLTM = GLM::new(T, H, Q, Z, R, y);
 
+        // run the kalman filter
         let (a_3d, P_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
 
+        // return the arrays as numpy arrays
         ((a_3d).into_pyarray(py), (P_3d).into_pyarray(py), (v_3d).into_pyarray(py), (F_3d).into_pyarray(py), (K_3d).into_pyarray(py))
     }
 
     Ok(())
 }
 
 #[cfg(test)]
```

### Comparing `rust_statespace-0.1.1/Cargo.lock` & `rust_statespace-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
+name = "csv"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
+dependencies = [
+ "csv-core",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "csv-core"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "dirs"
 version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30baa043103c9d0c2a57cf537cc2f35623889dc0d405e6c3cccfadbc81c71309"
 dependencies = [
  "dirs-sys",
 ]
@@ -291,14 +312,20 @@
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "itoa"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
 name = "lapack"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "041b3cb380f92a53e317ea046d0e715d2302dae6d2f426bdf3ccf27a36ef40e9"
 dependencies = [
  "lapack-sys",
  "libc",
@@ -370,14 +397,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "916806ba0031cd542105d916a97c8572e1fa6dd79c9c51e7eb43a09ec2dd84c1"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
+name = "memchr"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+
+[[package]]
 name = "miniz_oxide"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
@@ -759,16 +792,17 @@
  "getrandom 0.2.9",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "rust_statespace"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
+ "csv",
  "ndarray",
  "ndarray-linalg",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
@@ -803,14 +837,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
  "base64 0.21.0",
 ]
 
 [[package]]
+name = "ryu"
+version = "1.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+
+[[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
```

