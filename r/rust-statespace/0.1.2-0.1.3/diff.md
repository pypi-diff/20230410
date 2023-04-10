# Comparing `tmp/rust_statespace-0.1.2.tar.gz` & `tmp/rust_statespace-0.1.3.tar.gz`

## Comparing `rust_statespace-0.1.2.tar` & `rust_statespace-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.2/Cargo.toml
--rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/.gitignore
--rw-r--r--   0      501       20    32753 2023-04-10 14:44:01.000000 rust_statespace-0.1.2/Cargo.lock
--rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.2/data/nile.csv
--rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.2/pyproject.toml
--rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.2/requirements_rust.txt
--rw-r--r--   0      501       20     5850 2023-04-10 14:43:24.000000 rust_statespace-0.1.2/src/glm.rs
--rw-r--r--   0      501       20     1639 2023-04-08 13:48:17.000000 rust_statespace-0.1.2/src/lib.rs
--rw-r--r--   0      501       20      876 2023-04-08 13:37:57.000000 rust_statespace-0.1.2/src/main.rs
--rw-r--r--   0      501       20     1097 2023-04-08 13:31:03.000000 rust_statespace-0.1.2/src/read_data.rs
--rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 rust_statespace-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20     2800 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/.gitignore
+-rw-r--r--   0      501       20    32753 2023-04-10 15:41:45.000000 rust_statespace-0.1.3/Cargo.lock
+-rw-r--r--   0      501       20      942 2023-04-08 13:39:46.000000 rust_statespace-0.1.3/data/nile.csv
+-rw-r--r--   0      501       20      377 2023-04-07 13:29:27.000000 rust_statespace-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20      188 2023-04-08 10:11:03.000000 rust_statespace-0.1.3/requirements_rust.txt
+-rw-r--r--   0      501       20     7600 2023-04-10 15:40:34.000000 rust_statespace-0.1.3/src/glm.rs
+-rw-r--r--   0      501       20     1757 2023-04-10 15:36:10.000000 rust_statespace-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20      892 2023-04-10 15:41:06.000000 rust_statespace-0.1.3/src/main.rs
+-rw-r--r--   0      501       20     1097 2023-04-08 13:31:03.000000 rust_statespace-0.1.3/src/read_data.rs
+-rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 rust_statespace-0.1.3/PKG-INFO
```

### Comparing `rust_statespace-0.1.2/.github/workflows/CI.yml` & `rust_statespace-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.2/.gitignore` & `rust_statespace-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.2/Cargo.lock` & `rust_statespace-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
  "getrandom 0.2.9",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "rust_statespace"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "csv",
  "ndarray",
  "ndarray-linalg",
  "numpy",
  "pyo3",
 ]
```

### Comparing `rust_statespace-0.1.2/data/nile.csv` & `rust_statespace-0.1.3/data/nile.csv`

 * *Files identical despite different names*

### Comparing `rust_statespace-0.1.2/src/glm.rs` & `rust_statespace-0.1.3/src/glm.rs`

 * *Files 19% similar despite different names*

```diff
@@ -32,104 +32,130 @@
             Z: Z,
             R: R,
             y: y
         }
     }
 
     // Run Kalman Filter on instance variables
-    pub fn kalman_filter(&self) -> Result<(Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>), Box<dyn Error>> {
+    pub fn kalman_filter(&self) -> Result<(Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>, Array3<f64>), Box<dyn Error>> {
 
         let T = self.y.len();
         let p = self.T.ncols();
         let s: usize = self.Z.nrows();
 
         let mut axes_iterator: Array3<f64> = Array3::zeros((1, 1, T));
 
-        let mut a_3d: Array3<f64> = Array3::zeros((p, 1, T));
-        let mut v_3d: Array3<f64> = Array3::zeros((s, 1, T));
-        let mut F_3d: Array3<f64> = Array3::zeros((s, s, T));
-        let mut P_3d: Array3<f64> = Array3::zeros((p, p, T));
-        let mut K_3d: Array3<f64> = Array3::zeros((p, s, T));
+        let mut a_3d:   Array3<f64> = Array3::zeros((p, 1, T));
+        let mut att_3d: Array3<f64> = Array3::zeros((p, 1, T));
+        let mut v_3d:   Array3<f64> = Array3::zeros((s, 1, T));
+        let mut F_3d:   Array3<f64> = Array3::zeros((s, s, T));
+        let mut P_3d:   Array3<f64> = Array3::zeros((p, p, T));
+        let mut Ptt_3d: Array3<f64> = Array3::zeros((p, p, T));
+        let mut M_3d:   Array3<f64> = Array3::zeros((p, s, T));
+        let mut K_3d:   Array3<f64> = Array3::zeros((p, s, T));
         
-        let mut a_prev: Array2<f64> = Array2::zeros((p, 1));
-        let mut v_prev: Array2<f64> = Array2::zeros((s, 1));
-        let mut F_prev: Array2<f64> = Array2::zeros((s, s));
-        let mut P_prev: Array2<f64> = Array2::zeros((p, p));
-        let mut K_prev: Array2<f64> = Array2::zeros((p, s));
+        let mut a_prev:   Array2<f64> = Array2::zeros((p, 1));
+        let mut att_prev: Array2<f64> = Array2::zeros((p, 1));
+        let mut v_prev:   Array2<f64> = Array2::zeros((s, 1));
+        let mut F_prev:   Array2<f64> = Array2::zeros((s, s));
+        let mut P_prev:   Array2<f64> = Array2::zeros((p, p));
+        let mut Ptt_prev: Array2<f64> = Array2::zeros((p, p));
+        let mut M_prev:   Array2<f64> = Array2::zeros((p, s));
+        let mut K_prev:   Array2<f64> = Array2::zeros((p, s));
 
         // need to enumerate to use i
         for (i, _) in axes_iterator.axis_iter_mut(Axis(2)).enumerate() {
             
             // retrieve slices of the data
-            let mut a_temp: ArrayViewMut2<f64> = a_3d.slice_mut(s![..,..,i]);
-            let mut v_temp: ArrayViewMut2<f64> = v_3d.slice_mut(s![..,..,i]);
-            let mut F_temp: ArrayViewMut2<f64> = F_3d.slice_mut(s![..,..,i]);
-            let mut P_temp: ArrayViewMut2<f64> = P_3d.slice_mut(s![..,..,i]);
-            let mut K_temp: ArrayViewMut2<f64> = K_3d.slice_mut(s![..,..,i]);
+            let mut a_temp:   ArrayViewMut2<f64> = a_3d.slice_mut(s![..,..,i]);
+            let mut att_temp: ArrayViewMut2<f64> = att_3d.slice_mut(s![..,..,i]);
+            let mut v_temp:   ArrayViewMut2<f64> = v_3d.slice_mut(s![..,..,i]);
+            let mut F_temp:   ArrayViewMut2<f64> = F_3d.slice_mut(s![..,..,i]);
+            let mut P_temp:   ArrayViewMut2<f64> = P_3d.slice_mut(s![..,..,i]);
+            let mut Ptt_temp: ArrayViewMut2<f64> = Ptt_3d.slice_mut(s![..,..,i]);
+            let mut M_temp:   ArrayViewMut2<f64> = M_3d.slice_mut(s![..,..,i]);
+            let mut K_temp:   ArrayViewMut2<f64> = K_3d.slice_mut(s![..,..,i]);
             
             // in first iteration: set first values of a and P and compute corresponding v and F
             // TODO: add diffuse initialization
+            // TODO: add incasting
             if i == 0 {
 
-                // get y_0
-                let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
-
                 // set a_0 and P_0
                 a_temp.assign(&arr2(&[[0.0], [0.0]]));
                 P_temp.assign(&arr2(&[[1.0, 0.0], [0.0, 1.0]]));
 
+                // get y_0
+                let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
+
                 // get first error and error variance: v and F
                 v_temp.assign(&(
                     &y_temp - &self.Z.dot(&a_temp))
                 );
+                
                 F_temp.assign(&(
                     &self.Z.dot(&P_temp.dot(&self.Z.t())) + &self.H
                 ));
 
-                // compute Kalman gain
-                K_temp.assign(&(
-                    &self.T.dot(
-                        &P_temp.dot(
-                            &self.Z.t().dot(
-                                &F_temp.inv().unwrap()
-                            )
+                // compute incasted Kalman gain M
+                M_temp.assign(&(
+                    &P_temp.dot(
+                        &self.Z.t().dot(
+                            &F_temp.inv().unwrap()
                         )
                     )
                 ));
 
+                // compute Kalman gain K
+                K_temp.assign(&(
+                    &self.T.dot(
+                        &M_temp)
+                ));
+                
+                // compute incasted att
+                att_temp.assign(&(
+                    &a_temp + &M_temp.dot(&v_temp)
+                ));
+
+                // compute incasted Ptt
+                Ptt_temp.assign(&(
+                    &P_temp - 
+                        &M_temp.dot(&F_temp.dot(&M_temp.t()))
+                ));
+
                 // persist lagged a in memory
                 a_prev.assign(&a_temp);
                 P_prev.assign(&P_temp);
+                M_prev.assign(&M_temp);
                 K_prev.assign(&K_temp);
                 v_prev.assign(&v_temp);
                 F_prev.assign(&F_temp);
+                att_prev.assign(&att_temp);
+                Ptt_prev.assign(&Ptt_temp);
             }
 
             else {
 
                 // get new a_i and assign to mutable a_3d slice
                 a_temp.assign(&(
-                    &self.T.dot(&a_prev) + &K_prev.dot(&v_prev)
+                    &self.T.dot(&att_prev)
                 ));
 
                 // get new P_i and assign to mutable slide of P_3d
                 P_temp.assign(&
                     (&self.T.dot(
-                        &P_prev.dot(
+                        &Ptt_prev.dot(
                             &self.T.t()
                         )
                     ) + &self.R.dot(
                             &self.Q.dot(
                                 &self.R.t()
-                        )
-                    ) + &K_prev.dot(
-                            &F_prev.dot(
-                                &K_prev.t()
-                        )
-                    ))
+                            )
+                        ) 
+                    )
                 ); 
                 
                 // get current y
                 let y_temp: ArrayView2<f64> = self.y.slice(s![.., .., i]);
                 
                 // get prediction error
                 v_temp.assign(&(
@@ -137,35 +163,53 @@
                 ));
 
                 // get prediction error variance
                 F_temp.assign(&(
                     &self.Z.dot(&P_temp.dot(&self.Z.t())) + &self.H
                 ));
 
-                // compute Kalman gain
-                K_temp.assign(&(
-                    &self.T.dot(
-                        &P_temp.dot(
-                            &self.Z.t().dot(
-                                &F_temp.inv().unwrap()
-                            )
+                // compute incasted Kalman gain M
+                M_temp.assign(&(
+                    &P_temp.dot(
+                        &self.Z.t().dot(
+                            &F_temp.inv().unwrap()
                         )
                     )
                 ));
 
+                // compute Kalman gain K
+                K_temp.assign(&(
+                    &self.T.dot(
+                        &M_temp)
+                ));
+
+                // compute incasted att
+                att_temp.assign(&(
+                    &a_temp + &M_temp.dot(&v_temp)
+                ));
+
+                // compute incasted Ptt
+                Ptt_temp.assign(&(
+                    &P_temp - 
+                        &M_temp.dot(&F_temp.dot(&M_temp.t()))
+                ));
+
                 // persist lagged a in memory
                 a_prev.assign(&a_temp);
                 P_prev.assign(&P_temp);
+                M_prev.assign(&M_temp);
                 K_prev.assign(&K_temp);
                 v_prev.assign(&v_temp);
                 F_prev.assign(&F_temp);
+                att_prev.assign(&att_temp);
+                Ptt_prev.assign(&Ptt_temp);
             }
         }
 
-        Ok((a_3d, P_3d, v_3d, F_3d, K_3d))
+        Ok((a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d))
 
     }
 
     // function that loads data
     pub fn print_shapes(&self) {
         print!("T shape: {:?} \n", self.T.shape());
         print!("H shape: {:?} \n", self.H.shape());
```

### Comparing `rust_statespace-0.1.2/src/lib.rs` & `rust_statespace-0.1.3/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         R: PyReadonlyArray2<f64>,
         y: PyReadonlyArray3<f64>,
     ) -> 
     (&'py PyArray3<f64>, 
     &'py PyArray3<f64>,
     &'py PyArray3<f64>,
     &'py PyArray3<f64>,
+    &'py PyArray3<f64>,
+    &'py PyArray3<f64>,
     &'py PyArray3<f64>)
      {
         
         // get owned representations of the data
         let T = T.as_array().to_owned();
         let H = H.as_array().to_owned();
         let Q = Q.as_array().to_owned();
@@ -36,18 +38,18 @@
         let R = R.as_array().to_owned();
         let y = y.as_array().to_owned();
 
         // instantiate the GLM
         let LLTM = GLM::new(T, H, Q, Z, R, y);
 
         // run the kalman filter
-        let (a_3d, P_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
+        let (a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
 
         // return the arrays as numpy arrays
-        ((a_3d).into_pyarray(py), (P_3d).into_pyarray(py), (v_3d).into_pyarray(py), (F_3d).into_pyarray(py), (K_3d).into_pyarray(py))
+        ((a_3d).into_pyarray(py), (att_3d).into_pyarray(py), (P_3d).into_pyarray(py), (Ptt_3d).into_pyarray(py), (v_3d).into_pyarray(py), (F_3d).into_pyarray(py), (K_3d).into_pyarray(py))
     }
 
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `rust_statespace-0.1.2/src/main.rs` & `rust_statespace-0.1.3/src/main.rs`

 * *Files 22% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     let H = arr2(&[[1.0]]);
     let Q = arr2(&[[1.0, 0.0], [0.0, 1.0]]);
     let Z = arr2(&[[1.0, 0.0]]);
     let R = arr2(&[[1.0, 0.0], [0.0, 1.0]]);
 
     let LLTM = GLM::new(T, H, Q, Z, R, y);
     LLTM.print_shapes();
-    let (a_3d, P_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
+    let (a_3d, att_3d, P_3d, Ptt_3d, v_3d, F_3d, K_3d) = LLTM.kalman_filter().unwrap();
 
     println!("{}", &LLTM.y);
     println!("{}", a_3d.slice(s![0, .., ..]));
 
 }
```

### Comparing `rust_statespace-0.1.2/src/read_data.rs` & `rust_statespace-0.1.3/src/read_data.rs`

 * *Files identical despite different names*

