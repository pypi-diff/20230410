# Comparing `tmp/rust_statespace-0.1.3.tar.gz` & `tmp/rust_statespace-0.1.4.tar.gz`

## Comparing `rust_statespace-0.1.3.tar` & `rust_statespace-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.3/Cargo.toml
--rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/.gitignore
--rw-r--r--   0      501       20    32753 2023-04-10 15:41:45.000000 rust_statespace-0.1.3/Cargo.lock
--rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.3/data/nile.csv
--rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/pyproject.toml
--rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.3/requirements_rust.txt
--rw-r--r--   0      501       20     7600 2023-04-10 15:40:34.000000 rust_statespace-0.1.3/src/glm.rs
--rw-r--r--   0      501       20     1757 2023-04-10 15:36:10.000000 rust_statespace-0.1.3/src/lib.rs
--rw-r--r--   0      501       20      892 2023-04-10 15:41:06.000000 rust_statespace-0.1.3/src/main.rs
--rw-r--r--   0      501       20     1097 2023-04-08 13:31:03.000000 rust_statespace-0.1.3/src/read_data.rs
--rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/.gitignore
+-rw-r--r--   0      501       20    32753 2023-04-10 16:04:47.000000 rust_statespace-0.1.4/Cargo.lock
+-rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.4/data/nile.csv
+-rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.4/pyproject.toml
+-rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.4/requirements_rust.txt
+-rw-r--r--   0      501       20     7607 2023-04-10 16:03:50.000000 rust_statespace-0.1.4/src/glm.rs
+-rw-r--r--   0      501       20     1839 2023-04-10 15:54:51.000000 rust_statespace-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20      862 2023-04-10 15:59:48.000000 rust_statespace-0.1.4/src/main.rs
+-rw-r--r--   0      501       20     1041 2023-04-10 15:57:34.000000 rust_statespace-0.1.4/src/read_data.rs
+-rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.4/PKG-INFO
```

### Comparing `rust_statespace-0.1.3/.github/workflows/CI.yml` & `rust_statespace-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.3/.gitignore` & `rust_statespace-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.3/Cargo.lock` & `rust_statespace-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
  "getrandom 0.2.9",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "rust_statespace"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "csv",
  "ndarray",
  "ndarray-linalg",
  "numpy",
  "pyo3",
 ]
```

### Comparing `rust_statespace-0.1.3/data/nile.csv` & `rust_statespace-0.1.4/data/nile.csv`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.3/src/glm.rs` & `rust_statespace-0.1.4/src/glm.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             Z: Z,
             R: R,
             y: y
         }
     }
 
     // Run Kalman Filter on instance variables
-    pub fn kalman_filter(&self) -> Result<(Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>), Box<dyn Error>> {
+    pub fn kalman_filter(&self) -> Result<(Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>), Box<dyn Error>> {
 
         let T = self.y.len();
         let p = self.T.ncols();
         let s: usize = self.Z.nrows();
 
         let mut axes_iterator: Array3<f64> = Array3::zeros((1, 1, T));
 
@@ -78,24 +78,24 @@
             // in first iteration: set first values of a and P and compute corresponding v and F
             // TODO: add diffuse initialization
             // TODO: add incasting
             if i == 0 {
 
                 // set a_0 and P_0
                 a_temp.assign(&arr2(&[[0.0], [0.0]]));
-                P_temp.assign(&arr2(&[[1.0, 0.0], [0.0, 1.0]]));
+                P_temp.assign(&arr2(&[[1.0e4, 0.0], [0.0, 1.0e4]]));
 
                 // get y_0
                 let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
 
                 // get first error and error variance: v and F
                 v_temp.assign(&(
                     &y_temp - &self.Z.dot(&a_temp))
                 );
-                
+
                 F_temp.assign(&(
                     &self.Z.dot(&P_temp.dot(&self.Z.t())) + &self.H
                 ));
 
                 // compute incasted Kalman gain M
                 M_temp.assign(&(
                     &P_temp.dot(
@@ -201,15 +201,15 @@
                 v_prev.assign(&v_temp);
                 F_prev.assign(&F_temp);
                 att_prev.assign(&att_temp);
                 Ptt_prev.assign(&Ptt_temp);
             }
         }
 
-        Ok((a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d))
+        Ok((a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d, M_3d))
 
     }
 
     // function that loads data
     pub fn print_shapes(&self) {
         print!("T shape: {:?} \n", self.T.shape());
         print!("H shape: {:?} \n", self.H.shape());
```

### Comparing `rust_statespace-0.1.3/src/lib.rs` & `rust_statespace-0.1.4/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mod glm;
 
-use numpy::ndarray::{ArrayD, ArrayViewD, ArrayViewMutD};
-use numpy::{IntoPyArray, PyArrayDyn, PyReadonlyArrayDyn, PyReadonlyArray2, PyReadonlyArray3, PyArray2, PyArray3};
+use numpy::{IntoPyArray, PyReadonlyArray2, PyReadonlyArray3, PyArray3};
 use pyo3::{pymodule, types::PyModule, PyResult, Python};
+use ndarray::*;
 use glm::GLM;
 
 #[pymodule]
 fn rust_statespace(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
 
     // wrapper of kalman filter
     #[allow(non_snake_case)]
@@ -17,39 +17,40 @@
         T: PyReadonlyArray2<f64>,
         H: PyReadonlyArray2<f64>,
         Q: PyReadonlyArray2<f64>,
         Z: PyReadonlyArray2<f64>,
         R: PyReadonlyArray2<f64>,
         y: PyReadonlyArray3<f64>,
     ) -> 
-    (&'py PyArray3<f64>, 
-    &'py PyArray3<f64>,
-    &'py PyArray3<f64>,
-    &'py PyArray3<f64>,
-    &'py PyArray3<f64>,
-    &'py PyArray3<f64>,
-    &'py PyArray3<f64>)
+        (&'py PyArray3<f64>, 
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>,
+        &'py PyArray3<f64>)
      {
         
         // get owned representations of the data
-        let T = T.as_array().to_owned();
-        let H = H.as_array().to_owned();
-        let Q = Q.as_array().to_owned();
-        let Z = Z.as_array().to_owned();
-        let R = R.as_array().to_owned();
-        let y = y.as_array().to_owned();
+        let T: Array2<f64> = T.as_array().to_owned();
+        let H: Array2<f64> = H.as_array().to_owned();
+        let Q: Array2<f64> = Q.as_array().to_owned();
+        let Z: Array2<f64> = Z.as_array().to_owned();
+        let R: Array2<f64> = R.as_array().to_owned();
+        let y: Array3<f64> = y.as_array().to_owned();
 
         // instantiate the GLM
         let LLTM = GLM::new(T, H, Q, Z, R, y);
 
         // run the kalman filter
-        let (a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
+        let (a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d, M_3d) = LLTM.kalman_filter().unwrap();
 
         // return the arrays as numpy arrays
-        ((a_3d).into_pyarray(py), (att_3d).into_pyarray(py), (P_3d).into_pyarray(py), (Ptt_3d).into_pyarray(py), (v_3d).into_pyarray(py), (F_3d).into_pyarray(py), (K_3d).into_pyarray(py))
+        ((a_3d).into_pyarray(py), (att_3d).into_pyarray(py), (P_3d).into_pyarray(py), (Ptt_3d).into_pyarray(py), (v_3d).into_pyarray(py), (F_3d).into_pyarray(py), (K_3d).into_pyarray(py), (M_3d).into_pyarray(py))
     }
 
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `rust_statespace-0.1.3/src/read_data.rs` & `rust_statespace-0.1.4/src/read_data.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 use std::{
-    env,
     error::Error,
-    ffi::OsString,
     fs::File,
-    process,
     f64
 };
 
-use ndarray::{Array1, Array2, array};
+use ndarray::{Array1};
 
 // This module should:
 // 1. A load data function
 // 1.1. Check if file exists in data directory
 // 1.2. Check if filetype is csv
 // 1.3. Load data into csv
```

