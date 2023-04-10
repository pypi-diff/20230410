# Comparing `tmp/elapid-0.3.8.tar.gz` & `tmp/elapid-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elapid-0.3.8.tar", last modified: Fri Sep  9 01:06:44 2022, max compression
+gzip compressed data, was "elapid-0.3.9.tar", last modified: Fri Sep  9 16:38:01 2022, max compression
```

## Comparing `elapid-0.3.8.tar` & `elapid-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 01:06:44.000000 elapid-0.3.8/
--rw-r--r--   0 cba       (1000) cba       (1000)     1077 2021-06-26 05:24:58.000000 elapid-0.3.8/LICENSE
--rw-r--r--   0 cba       (1000) cba       (1000)      150 2022-05-10 22:35:05.000000 elapid-0.3.8/MANIFEST.in
--rw-r--r--   0 cba       (1000) cba       (1000)     5602 2022-09-09 01:06:44.000000 elapid-0.3.8/PKG-INFO
--rw-r--r--   0 cba       (1000) cba       (1000)     5051 2022-09-06 17:30:49.000000 elapid-0.3.8/README.md
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 01:06:44.000000 elapid-0.3.8/elapid/
--rw-r--r--   0 cba       (1000) cba       (1000)      401 2022-05-02 20:10:05.000000 elapid-0.3.8/elapid/__init__.py
--rw-r--r--   0 cba       (1000) cba       (1000)        8 2022-09-09 01:05:17.000000 elapid-0.3.8/elapid/__version__.py
--rw-r--r--   0 cba       (1000) cba       (1000)     1856 2022-09-09 01:05:17.000000 elapid-0.3.8/elapid/config.py
--rw-r--r--   0 cba       (1000) cba       (1000)    27535 2022-09-08 04:45:29.000000 elapid-0.3.8/elapid/features.py
--rw-r--r--   0 cba       (1000) cba       (1000)    26446 2022-09-08 04:45:29.000000 elapid-0.3.8/elapid/geo.py
--rw-r--r--   0 cba       (1000) cba       (1000)    21085 2022-09-09 01:05:17.000000 elapid-0.3.8/elapid/models.py
--rw-r--r--   0 cba       (1000) cba       (1000)     3689 2022-04-29 18:45:43.000000 elapid-0.3.8/elapid/stats.py
--rw-r--r--   0 cba       (1000) cba       (1000)     3171 2022-05-10 23:20:30.000000 elapid-0.3.8/elapid/types.py
--rw-r--r--   0 cba       (1000) cba       (1000)     7779 2022-09-09 01:05:17.000000 elapid-0.3.8/elapid/utils.py
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 01:06:44.000000 elapid-0.3.8/elapid.egg-info/
--rw-r--r--   0 cba       (1000) cba       (1000)     5602 2022-09-09 01:06:43.000000 elapid-0.3.8/elapid.egg-info/PKG-INFO
--rw-r--r--   0 cba       (1000) cba       (1000)      381 2022-09-09 01:06:44.000000 elapid-0.3.8/elapid.egg-info/SOURCES.txt
--rw-r--r--   0 cba       (1000) cba       (1000)        1 2022-09-09 01:06:43.000000 elapid-0.3.8/elapid.egg-info/dependency_links.txt
--rw-r--r--   0 cba       (1000) cba       (1000)      139 2022-09-09 01:06:43.000000 elapid-0.3.8/elapid.egg-info/requires.txt
--rw-r--r--   0 cba       (1000) cba       (1000)        7 2022-09-09 01:06:43.000000 elapid-0.3.8/elapid.egg-info/top_level.txt
--rw-r--r--   0 cba       (1000) cba       (1000)      113 2022-09-08 04:45:49.000000 elapid-0.3.8/requirements-dev.txt
--rw-r--r--   0 cba       (1000) cba       (1000)      139 2021-12-18 10:45:31.000000 elapid-0.3.8/requirements.txt
--rw-r--r--   0 cba       (1000) cba       (1000)       38 2022-09-09 01:06:44.000000 elapid-0.3.8/setup.cfg
--rw-r--r--   0 cba       (1000) cba       (1000)     1279 2022-05-10 22:36:08.000000 elapid-0.3.8/setup.py
+drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.030368 elapid-0.3.9/
+-rw-r--r--   0 cba       (1000) cba       (1000)     1077 2021-06-26 05:24:58.000000 elapid-0.3.9/LICENSE
+-rw-r--r--   0 cba       (1000) cba       (1000)      121 2022-09-09 06:53:10.000000 elapid-0.3.9/MANIFEST.in
+-rw-r--r--   0 cba       (1000) cba       (1000)     5595 2022-09-09 16:38:01.030368 elapid-0.3.9/PKG-INFO
+-rw-r--r--   0 cba       (1000) cba       (1000)     5051 2022-09-06 17:30:49.000000 elapid-0.3.9/README.md
+drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.026366 elapid-0.3.9/elapid/
+-rw-r--r--   0 cba       (1000) cba       (1000)      401 2022-05-02 20:10:05.000000 elapid-0.3.9/elapid/__init__.py
+-rw-r--r--   0 cba       (1000) cba       (1000)        8 2022-09-09 06:28:12.000000 elapid-0.3.9/elapid/__version__.py
+-rw-r--r--   0 cba       (1000) cba       (1000)     1863 2022-09-09 01:11:05.000000 elapid-0.3.9/elapid/config.py
+-rw-r--r--   0 cba       (1000) cba       (1000)    27535 2022-09-08 04:45:29.000000 elapid-0.3.9/elapid/features.py
+-rw-r--r--   0 cba       (1000) cba       (1000)    26446 2022-09-08 04:45:29.000000 elapid-0.3.9/elapid/geo.py
+-rw-r--r--   0 cba       (1000) cba       (1000)    24197 2022-09-09 06:53:10.000000 elapid-0.3.9/elapid/models.py
+-rw-r--r--   0 cba       (1000) cba       (1000)     3689 2022-04-29 18:45:43.000000 elapid-0.3.9/elapid/stats.py
+-rw-r--r--   0 cba       (1000) cba       (1000)     3171 2022-05-10 23:20:30.000000 elapid-0.3.9/elapid/types.py
+-rw-r--r--   0 cba       (1000) cba       (1000)     7778 2022-09-09 06:11:01.000000 elapid-0.3.9/elapid/utils.py
+drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.029368 elapid-0.3.9/elapid.egg-info/
+-rw-r--r--   0 cba       (1000) cba       (1000)     5595 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/PKG-INFO
+-rw-r--r--   0 cba       (1000) cba       (1000)      360 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/SOURCES.txt
+-rw-r--r--   0 cba       (1000) cba       (1000)        1 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/dependency_links.txt
+-rw-r--r--   0 cba       (1000) cba       (1000)      170 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/requires.txt
+-rw-r--r--   0 cba       (1000) cba       (1000)        7 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/top_level.txt
+-rw-r--r--   0 cba       (1000) cba       (1000)      164 2022-09-09 06:53:10.000000 elapid-0.3.9/requirements.txt
+-rw-r--r--   0 cba       (1000) cba       (1000)       38 2022-09-09 16:38:01.030368 elapid-0.3.9/setup.cfg
+-rw-r--r--   0 cba       (1000) cba       (1000)     1458 2022-09-09 06:53:10.000000 elapid-0.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elapid-0.3.8/LICENSE` & `elapid-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/PKG-INFO` & `elapid-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: elapid
-Version: 0.3.8
+Version: 0.3.9
 Summary: Species distribution modeling support tools
 Home-page: https://elapid.org
 Author: Christopher Anderson
 Author-email: cbanders@stanford.edu
 License: MIT
 Keywords: biogeography,ecology,conservation,SDM,species distribution modeling,maxent
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0,<3.9.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elapid
 
 <img src="https://earth-chris.github.io/elapid/img/amazon.jpg" alt="the amazon"/>
```

### Comparing `elapid-0.3.8/README.md` & `elapid-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/elapid/config.py` & `elapid-0.3.9/elapid/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     tolerance: float = 1e-7
 
     # elasticnet lambda type to use ('best' or 'last')
     use_lambdas: str = "best"
     n_lambdas: int = 100
 
     # method for weighting presence samples
-    weights: Union[str, float] = "balance"
+    class_weights: Union[str, float] = "balanced"
 
 
 # maxent default regularization parameters (from the maxnet R package)
 class RegularizationConfig:
     linear: list = [[0, 10, 30, 100], [1, 1, 0.2, 0.05]]
     quadratic: list = [[0, 10, 17, 30, 100], [1.3, 0.8, 0.5, 0.25, 0.05]]
     product: list = [[0, 10, 17, 30, 100], [2.6, 1.6, 0.9, 0.55, 0.05]]
```

### Comparing `elapid-0.3.8/elapid/features.py` & `elapid-0.3.9/elapid/features.py`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/elapid/geo.py` & `elapid-0.3.9/elapid/geo.py`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/elapid/models.py` & `elapid-0.3.9/elapid/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 """Classes for training species distribution models."""
 from typing import List, Tuple, Union
+from warnings import warn
 
 import numpy as np
 import pandas as pd
-from glmnet.logistic import LogitNet
 from sklearn.base import BaseEstimator
+from sklearn.exceptions import NotFittedError
+from sklearn.linear_model import LogisticRegression
 
 from elapid import features as _features
 from elapid.config import MaxentConfig, NicheEnvelopeConfig
 from elapid.types import ArrayLike, Number, validate_feature_types
-from elapid.utils import make_band_labels, n_cpus
+from elapid.utils import NCPUS, make_band_labels
+
+# handle windows systems without functioning gfortran compilers
+FORCE_SKLEARN = False
+try:
+    from glmnet.logistic import LogitNet
+
+except ModuleNotFoundError:
+    warn(
+        "Failed to import glmnet: using sklearn for Maxent. Interpret results with caution.",
+        category=RuntimeWarning,
+    )
+    FORCE_SKLEARN = True
 
 
 class MaxentModel(BaseEstimator):
     """Model estimator for Maxent-style species distribution models."""
 
-    feature_types_: list = MaxentConfig.feature_types
-    tau_: float = MaxentConfig.tau
-    clamp_: bool = MaxentConfig.clamp
-    convergence_tolerance_: float = MaxentConfig.tolerance
-    beta_multiplier_: float = MaxentConfig.beta_multiplier
-    beta_hinge_: float = MaxentConfig.beta_hinge
-    beta_lqp_: float = MaxentConfig.beta_lqp
-    beta_threshold_: float = MaxentConfig.beta_threshold
-    beta_categorical_: float = MaxentConfig.beta_categorical
-    n_hinge_features_: int = MaxentConfig.n_hinge_features
-    n_threshold_features_: int = MaxentConfig.n_threshold_features
-    scorer_: str = MaxentConfig.scorer
-    use_lambdas_: str = MaxentConfig.use_lambdas
-    n_lambdas_: str = MaxentConfig.n_lambdas
+    # passed to __init__
+    feature_types: list = MaxentConfig.feature_types
+    tau: float = MaxentConfig.tau
+    clamp: bool = MaxentConfig.clamp
+    scorer: str = MaxentConfig.scorer
+    beta_multiplier: float = MaxentConfig.beta_multiplier
+    beta_hinge: float = MaxentConfig.beta_hinge
+    beta_lqp: float = MaxentConfig.beta_lqp
+    beta_threshold: float = MaxentConfig.beta_threshold
+    beta_categorical: float = MaxentConfig.beta_categorical
+    n_hinge_features: int = MaxentConfig.n_hinge_features
+    n_threshold_features: int = MaxentConfig.n_threshold_features
+    convergence_tolerance: float = MaxentConfig.tolerance
+    use_lambdas: str = MaxentConfig.use_lambdas
+    n_lambdas: str = MaxentConfig.n_lambdas
+    class_weights: Union[str, float] = None
+    n_cpus: int = NCPUS
+    use_sklearn: bool = False
+
+    # computed during model fitting
     initialized_: bool = False
-    beta_scores_: np.array = None
-    entropy_: float = 0.0
-    alpha_: float = 0.0
     estimator: BaseEstimator = None
-    transformer: _features.MaxentFeatureTransformer = None
-    weights_: np.ndarray = None
+    preprocessor: BaseEstimator = None
+    transformer: BaseEstimator = None
     regularization_: np.ndarray = None
+    sample_weights_: np.ndarray = None
     lambdas_: np.ndarray = None
-    weight_strategy_: Union[str, float] = None
-    n_cpus_ = n_cpus
+    beta_scores_: np.array = None
+    entropy_: float = 0.0
+    alpha_: float = 0.0
 
     def __init__(
         self,
         feature_types: Union[list, str] = MaxentConfig.feature_types,
         tau: float = MaxentConfig.tau,
         clamp: bool = MaxentConfig.clamp,
         scorer: str = MaxentConfig.scorer,
@@ -53,16 +72,17 @@
         beta_threshold: float = MaxentConfig.beta_lqp,
         beta_categorical: float = MaxentConfig.beta_categorical,
         n_hinge_features: int = MaxentConfig.n_hinge_features,
         n_threshold_features: int = MaxentConfig.n_threshold_features,
         convergence_tolerance: float = MaxentConfig.tolerance,
         use_lambdas: str = MaxentConfig.use_lambdas,
         n_lambdas: int = MaxentConfig.n_lambdas,
-        weights: Union[str, float] = MaxentConfig.weights,
-        n_cpus: int = n_cpus,
+        class_weights: Union[str, float] = MaxentConfig.class_weights,
+        n_cpus: int = NCPUS,
+        use_sklearn: bool = FORCE_SKLEARN,
     ):
         """Create a maxent model object.
 
         Args:
             feature_types: maxent feature types to fit. must be in string "lqphta" or
                 list ["linear", "quadratic", "product", "hinge", "threshold", "auto"]
             tau: maxent prevalence value for scaling logistic output
@@ -70,230 +90,255 @@
             scorer: sklearn scoring function for model training
             beta_multiplier: scaler for all regularization parameters.
                 higher values drop more coeffiecients
             beta_lqp: linear, quadratic and product feature regularization scaler
             beta_hinge: hinge feature regularization scaler
             beta_threshold: threshold feature regularization scaler
             beta_categorical: categorical feature regularization scaler
+            n_hinge_features: the number of hinge features to fit in feature transformation
+            n_threshold_features: the number of thresholds to fit in feature transformation
             convergence_tolerance: model convergence tolerance level
             use_lambdas: guide for which model lambdas to select (either "best" or "last")
             n_lambdas: number of lamba values to fit models with
-            weights: strategy for weighting presence samples.
+            class_weights: strategy for weighting presence samples.
                 pass "balance" to compute the ratio based on sample frequency
                 or pass a float for the presence:background weight ratio
+                the R `maxnet` package uses a value of 100 as default
             n_cpus: threads to use during model training
-        """
-        self.feature_types_ = validate_feature_types(feature_types)
-        self.tau_ = tau
-        self.clamp_ = clamp
-        self.convergence_tolerance_ = convergence_tolerance
-        self.beta_multiplier_ = beta_multiplier
-        self.beta_hinge_ = beta_hinge
-        self.beta_lqp_ = beta_lqp
-        self.beta_threshold_ = beta_threshold
-        self.beta_categorical_ = beta_categorical
-        self.n_hinge_features_ = n_hinge_features
-        self.n_threshold_features_ = n_threshold_features
-        self.n_cpus_ = n_cpus
-        self.scorer_ = scorer
-        self.use_lambdas_ = use_lambdas
-        self.n_lambdas_ = n_lambdas
-        self.weight_strategy_ = weights
+            use_sklearn: force using `sklearn` for fitting logistic regression.
+                turned off by default to use `glmnet` for fitting.
+                this feature was turned on to support Windows users
+                who install the package without a fortran compiler.
+        """
+        self.feature_types = validate_feature_types(feature_types)
+        self.tau = tau
+        self.clamp = clamp
+        self.scorer = scorer
+        self.beta_multiplier = beta_multiplier
+        self.beta_hinge = beta_hinge
+        self.beta_lqp = beta_lqp
+        self.beta_threshold = beta_threshold
+        self.beta_categorical = beta_categorical
+        self.n_hinge_features = n_hinge_features
+        self.n_threshold_features = n_threshold_features
+        self.convergence_tolerance = convergence_tolerance
+        self.n_cpus = n_cpus
+        self.use_lambdas = use_lambdas
+        self.n_lambdas = n_lambdas
+        self.class_weights = class_weights
+        self.use_sklearn = use_sklearn
 
     def fit(
         self,
         x: ArrayLike,
         y: ArrayLike,
         categorical: List[int] = None,
         labels: list = None,
-        is_features: bool = False,
-        feature_labels: list = None,
+        preprocessor: BaseEstimator = None,
     ) -> None:
         """Trains a maxent model using a set of covariates and presence/background points.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             y: array-like of shape (n_samples,) with binary presence/background (1/0) values
             categorical: indices for which columns are categorical
             labels: covariate labels. ignored if x is a pandas DataFrame
-            is_features: specify that x data has been transformed from covariates to features
-            feature_labels: list of length n_features, with labels identifying each column's feature type
-                with options ["linear", "quadratic", "product", "threshold", "hinge", "categorical"]
-                must be set if `is_features=True`
+            preprocessor: an `sklearn` transformer with a .transform() and/or
+                a .fit_transform() method. Some examples include a PCA() object or a
+                RobustScaler().
         """
+        # clear state variables
+        self.alpha_ = 0.0
+        self.entropy_ = 0.0
+
         # format the input data
         y = format_occurrence_data(y)
 
-        # fit the feature transformer
-        if is_features:
-            features = x
-            assert feature_labels is not None, "feature_labels must be set if is_features=True"
+        # apply preprocessing
+        if preprocessor is not None:
+            self.preprocessor = preprocessor
+            try:
+                x = self.preprocessor.transform(x)
+            except NotFittedError:
+                x = self.preprocessor.fit_transform(x)
 
-        else:
-            self.transformer = _features.MaxentFeatureTransformer(
-                feature_types=self.feature_types_,
-                clamp=self.clamp_,
-                n_hinge_features=self.n_hinge_features_,
-                n_threshold_features=self.n_threshold_features_,
-            )
-            features = self.transformer.fit_transform(x, categorical=categorical, labels=labels)
-            feature_labels = self.transformer.feature_names_
+        # fit the feature transformer
+        self.transformer = _features.MaxentFeatureTransformer(
+            feature_types=self.feature_types,
+            clamp=self.clamp,
+            n_hinge_features=self.n_hinge_features,
+            n_threshold_features=self.n_threshold_features,
+        )
+        features = self.transformer.fit_transform(x, categorical=categorical, labels=labels)
+        feature_labels = self.transformer.feature_names_
 
         # compute sample weights
-        if self.weight_strategy_ == "balance":
-            pbr = len(y) / y.sum()
-        else:
-            pbr = self.weight_strategy_
+        pbr = len(y) / y.sum() if self.class_weights == "balanced" else self.class_weights
+        self.sample_weights_ = _features.compute_weights(y, pbr=pbr)
 
-        self.weights_ = _features.compute_weights(y, pbr=pbr)
+        # model fitting with sklearn
+        if self.use_sklearn:
+            C = estimate_C_from_betas(self.beta_multiplier)
+            self.initialize_sklearn_model(C)
+            self.estimator.fit(features, y, sample_weight=self.sample_weights_)
+            self.beta_scores_ = self.estimator.coef_[0]
 
-        # set feature regularization parameters
-        self.regularization_ = _features.compute_regularization(
-            y,
-            features,
-            feature_labels=feature_labels,
-            beta_multiplier=self.beta_multiplier_,
-            beta_threshold=self.beta_threshold_,
-            beta_hinge=self.beta_hinge_,
-            beta_categorical=self.beta_categorical_,
-        )
+        # model fitting with glmnet
+        else:
+            # set feature regularization parameters
+            self.regularization_ = _features.compute_regularization(
+                y,
+                features,
+                feature_labels=feature_labels,
+                beta_multiplier=self.beta_multiplier,
+                beta_lqp=self.beta_lqp,
+                beta_threshold=self.beta_threshold,
+                beta_hinge=self.beta_hinge,
+                beta_categorical=self.beta_categorical,
+            )
 
-        # get model lambda scores to initialize the glm
-        self.lambdas_ = _features.compute_lambdas(y, self.weights_, self.regularization_, n_lambdas=self.n_lambdas_)
+            # get model lambda scores to initialize the glm
+            self.lambdas_ = _features.compute_lambdas(
+                y, self.sample_weights_, self.regularization_, n_lambdas=self.n_lambdas
+            )
 
-        # model fitting
-        self.initialize_model(lambdas=self.lambdas_)
-        self.estimator.fit(
-            features,
-            y,
-            sample_weight=self.weights_,
-            relative_penalties=self.regularization_,
-        )
+            # model fitting
+            self.initialize_glmnet_model(lambdas=self.lambdas_)
+            self.estimator.fit(
+                features,
+                y,
+                sample_weight=self.sample_weights_,
+                relative_penalties=self.regularization_,
+            )
+
+            # get the beta values based on which lambda selection method to use
+            if self.use_lambdas == "last":
+                self.beta_scores_ = self.estimator.coef_path_[0, :, -1]
+            elif self.use_lambdas == "best":
+                self.beta_scores_ = self.estimator.coef_path_[0, :, self.estimator.lambda_max_inx_]
 
-        # get the beta values based on which lamba selection method to use
-        if self.use_lambdas_ == "last":
-            self.beta_scores_ = self.estimator.coef_path_[0, :, -1]
-        elif self.use_lambdas_ == "best":
-            self.beta_scores_ = self.estimator.coef_path_[0, :, self.estimator.lambda_max_inx_]
+        # store initialization state
+        self.initialized_ = True
 
         # apply maxent-specific transformations
-        raw = self.predict(features[y == 0], transform="raw", is_features=True)
+        raw = self.predict(x[y == 0], transform="raw")
 
         # alpha is a normalizing constant that ensures that f1(z) integrates (sums) to 1
         self.alpha_ = maxent_alpha(raw)
 
         # the distance from f(z) is the relative entropy of f1(z) WRT f(z)
         self.entropy_ = maxent_entropy(raw)
 
-    def predict(self, x: ArrayLike, transform: str = "cloglog", is_features: bool = False) -> ArrayLike:
+    def predict(self, x: ArrayLike, transform: str = "cloglog") -> ArrayLike:
         """Applies a model to a set of covariates or features. Requires that a model has been fit.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             transform: maxent model transformation type. select from
                 ["raw", "logistic", "cloglog"].
-            is_features: flag that x data has already been transformed from covariates to features
 
         Returns:
             predictions: array-like of shape (n_samples,) with model predictions
         """
-        assert self.initialized_, "Model must be fit first"
+        if not self.initialized_:
+            raise NotFittedError("Model must be fit first")
 
         # feature transformations
-        features = x if is_features else self.transformer.transform(x)
+        x = x if self.preprocessor is None else self.preprocessor.transform(x)
+        features = x if self.transformer is None else self.transformer.transform(x)
 
         # apply the model
         engma = np.matmul(features, self.beta_scores_) + self.alpha_
 
         # scale based on the transform type
         if transform == "raw":
-            return np.exp(engma)
+            return maxent_raw_transform(engma)
 
         elif transform == "logistic":
-            # below is R's maxnet (tau-free) logistic formulation
-            # return 1 / (1 + np.exp(-self.entropy_ - engma))
-            # use the java formulation instead
-            logratio = np.exp(engma) * np.exp(self.entropy_)
-            return (self.tau_ * logratio) / ((1 - self.tau_) + (self.tau_ * logratio))
+            return maxent_logistic_transform(engma, self.entropy_, self.tau)
 
         elif transform == "cloglog":
-            # below is R's maxent cloglog formula
-            # return 1 - np.exp(0 - np.exp(self.entropy_ + engma))
-            # use java again
-            return 1 - np.exp(-np.exp(engma) * np.exp(self.entropy_))
+            return maxent_cloglog_transform(engma, self.entropy_)
 
     def fit_predict(
         self,
         x: ArrayLike,
         y: ArrayLike,
         categorical: list = None,
         labels: list = None,
+        preprocessor: BaseEstimator = None,
         transform: str = "cloglog",
-        is_features: bool = False,
-        feature_labels: list = None,
     ) -> ArrayLike:
         """Trains and applies a model to x/y data.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             y: array-like of shape (n_samples,) with binary presence/background (1/0) values
             categorical: column indices indicating which columns are categorical
             labels: Covariate labels. Ignored if x is a pandas DataFrame
+            preprocessor: an `sklearn` transformer with a .transform() and/or
+                a .fit_transform() method. Some examples include a PCA() object or a
+                RobustScaler().
             transform: maxent model transformation type. select from
                 ["raw", "logistic", "cloglog"].
-            is_features: specify that x data has already been transformed from covariates to features
-            feature_labels: list of length n_features, with labels identifying each column's feature type
-                with options ["linear", "quadratic", "product", "threshold", "hinge", "categorical"]
-                must be set if `is_features=True`
 
         Returns:
             predictions: Array-like of shape (n_samples,) with model predictions
         """
-        self.fit(x, y, categorical=categorical, labels=labels, is_features=is_features, feature_labels=feature_labels)
-        predictions = self.predict(x, transform=transform, is_features=is_features)
+        self.fit(x, y, categorical=categorical, labels=labels, preprocessor=preprocessor)
+        predictions = self.predict(x, transform=transform)
 
         return predictions
 
-    def initialize_model(
+    def initialize_glmnet_model(
         self,
         lambdas: np.array,
         alpha: float = 1,
         standardize: bool = False,
-        fit_intercept: bool = False,
+        fit_intercept: bool = True,
     ) -> None:
         """Creates the Logistic Regression with elastic net penalty model object.
 
         Args:
             lambdas: array of model lambda values. get from elapid.features.compute_lambdas()
             alpha: elasticnet mixing parameter. alpha=1 for lasso, alpha=0 for ridge
             standardize: specify coefficient normalization
             fit_intercept: include an intercept parameter
-
-        Returns:
-            None. updates the self.estimator with an sklearn-style model estimator
         """
         self.estimator = LogitNet(
             alpha=alpha,
             lambda_path=lambdas,
             standardize=standardize,
             fit_intercept=fit_intercept,
-            scoring=self.scorer_,
-            n_jobs=self.n_cpus_,
-            tol=self.convergence_tolerance_,
+            scoring=self.scorer,
+            n_jobs=self.n_cpus,
+            tol=self.convergence_tolerance,
         )
 
-        self.alpha_ = 0.0
-        self.entropy_ = 0.0
-        self.initialized_ = True
+    def initialize_sklearn_model(self, C: float, fit_intercept: bool = True) -> None:
+        """Creates an sklearn Logisticregression estimator with L1 penalties.
+
+        Args:
+            C: the regularization parameter
+            fit_intercept: include an intercept parameter
+        """
+        self.estimator = LogisticRegression(
+            C=C,
+            fit_intercept=fit_intercept,
+            penalty="l1",
+            solver="liblinear",
+            tol=self.convergence_tolerance,
+            max_iter=self.n_lambdas,
+        )
 
 
 class NicheEnvelopeModel(BaseEstimator):
     """Model estimator for niche envelope-style models."""
 
-    percentile_range_: Tuple[float, float] = None
+    percentile_range: Tuple[float, float] = None
     feature_mins_: np.ndarray = None
     feature_maxs_: np.ndarray = None
     categorical_estimator: BaseEstimator = None
     categorical_: list = None
     continuous_: list = None
     categorical_pd_: list = None
     continuous_pd_: list = None
@@ -304,15 +349,15 @@
 
         Args:
             percentile_range: covariate values within this range are flagged as suitable habitat
                 using a narrow range like [10, 90] drops more areas from suitability maps
                 while [0, 100] creates an envelope around the full range of observed
                 covariates at all y==1 locations.
         """
-        self.percentile_range_ = percentile_range
+        self.percentile_range = percentile_range
         self.categorical_estimator = _features.CategoricalTransformer()
 
     def _format_covariate_data(self, x: ArrayLike) -> Tuple[np.array, np.array]:
         """Reads input x data and formats it to consistent array dtypes.
 
         Args:
             x: array-like of shape (n_samples, n_features)
@@ -386,16 +431,16 @@
         """
         # format the input x/y data
         self._format_labels_and_dtypes(x, categorical=categorical, labels=labels)
         con, cat = self._format_covariate_data(x)
         y = format_occurrence_data(y)
 
         # estimate the feature range of the continuous data
-        self.feature_mins_ = np.percentile(con[y == 1], self.percentile_range_[0], axis=0)
-        self.feature_maxs_ = np.percentile(con[y == 1], self.percentile_range_[1], axis=0)
+        self.feature_mins_ = np.percentile(con[y == 1], self.percentile_range[0], axis=0)
+        self.feature_maxs_ = np.percentile(con[y == 1], self.percentile_range[1], axis=0)
 
         # one-hot encode the categorical data and label the classes with
         if cat is not None:
             ohe = self.categorical_estimator.fit_transform(cat)
             self.in_categorical_ = np.any(ohe[y == 1], axis=0)
 
     def predict(self, x: ArrayLike, overlay: str = "average") -> np.ndarray:
@@ -480,28 +525,83 @@
     Returns:
         entropy: background distribution entropy score
     """
     scaled = raw / np.sum(raw)
     return -np.sum(scaled * np.log(scaled))
 
 
+def maxent_raw_transform(engma: np.ndarray) -> np.ndarray:
+    """Compute maxent's raw suitability score
+
+    Args:
+        engma: calibrated maxent linear model output
+
+    Returns:
+        the log-linear raw scores for each sample
+    """
+    return np.exp(engma)
+
+
+def maxent_logistic_transform(engma: np.ndarray, entropy: float, tau: float = MaxentConfig.tau) -> np.ndarray:
+    """Compute maxent's logistic suitability score
+
+    Args:
+        engma: calibrated maxent linear model output
+        entropy: the calibrated model entropy score
+        tau: the prevalence scaler. lower values indicate rarer species.
+
+    Returns:
+        the tau-scaled logistic scores for each sample
+    """
+    # maxnet's (tau-free) logistic formulation:
+    # return 1 / (1 + np.exp(-entropy - engma))
+    # use java's formulation instead
+    logratio = np.exp(engma) * np.exp(entropy)
+    return (tau * logratio) / ((1 - tau) + (tau * logratio))
+
+
+def maxent_cloglog_transform(engma: np.ndarray, entropy: float) -> np.ndarray:
+    """Compute maxent's cumulative log-log suitability score
+
+    Args:
+        engma: calibrated maxent linear model output
+        entropy: the calibrated model entropy score
+
+    Returns:
+        the cloglog scores for each sample
+    """
+    return 1 - np.exp(-np.exp(engma) * np.exp(entropy))
+
+
 def format_occurrence_data(y: ArrayLike) -> ArrayLike:
     """Reads input y data and formats it to consistent 1d array dtypes.
 
     Args:
         y: array-like of shape (n_samples,) or (n_samples, 1)
 
     Returns:
-        formatted uin8 ndarray of shape (n_samples,)
+        formatted uint8 ndarray of shape (n_samples,)
 
     Raises:
         np.AxisError: an array with 2 or more columns is passed
     """
     if not isinstance(y, np.ndarray):
         y = np.array(y)
 
     if y.ndim > 1:
-        if y.shape[1] > 1:
+        if y.shape[1] > 1 or y.ndim > 2:
             raise np.AxisError(f"Multi-column y data passed of shape {y.shape}. Must be 1d or 1 column.")
         y = y.flatten()
 
     return y.astype("uint8")
+
+
+def estimate_C_from_betas(beta_multiplier: float) -> float:
+    """Convert the maxent-format beta_multiplier to an sklearn-format C regularization parameter.
+
+    Args:
+        beta_multiplier: the maxent beta regularization scaler
+
+    Returns:
+        a C factor approximating the level of regularization passed to glmnet
+    """
+    return 2 / (1 - np.exp(-beta_multiplier))
```

### Comparing `elapid-0.3.8/elapid/stats.py` & `elapid-0.3.9/elapid/stats.py`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/elapid/types.py` & `elapid-0.3.9/elapid/types.py`

 * *Files identical despite different names*

### Comparing `elapid-0.3.8/elapid/utils.py` & `elapid-0.3.9/elapid/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import rasterio as rio
 
 from elapid.types import Number
 
-n_cpus = mp.cpu_count()
+NCPUS = mp.cpu_count()
 
 
 class NoDataException(Exception):
     pass
 
 
 def repeat_array(x: np.array, length: int = 1, axis: int = 0) -> np.ndarray:
```

### Comparing `elapid-0.3.8/elapid.egg-info/PKG-INFO` & `elapid-0.3.9/elapid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: elapid
-Version: 0.3.8
+Version: 0.3.9
 Summary: Species distribution modeling support tools
 Home-page: https://elapid.org
 Author: Christopher Anderson
 Author-email: cbanders@stanford.edu
 License: MIT
 Keywords: biogeography,ecology,conservation,SDM,species distribution modeling,maxent
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0,<3.9.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elapid
 
 <img src="https://earth-chris.github.io/elapid/img/amazon.jpg" alt="the amazon"/>
```

### Comparing `elapid-0.3.8/setup.py` & `elapid-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
+import platform
 
 from setuptools import setup
 
 this_dir, this_path = os.path.split(os.path.abspath(__file__))
 version = open(os.path.join(this_dir, "elapid", "__version__.py")).read().strip('"\n')
 long_description = open(os.path.join(this_dir, "README.md"), "r", encoding="utf-8").read()
 requirements = open(os.path.join(this_dir, "requirements.txt"), "r", encoding="utf-8").read().strip().split()
 
+# remove glmnet requirement for windows installs
+if platform.system() != "Linux":
+    [requirements.pop(idx) for idx, pkg in enumerate(requirements) if "glmnet" in pkg]
+
 setup_args = {
     "name": "elapid",
     "version": version,
     "url": "https://elapid.org",
     "license": "MIT",
     "author": "Christopher Anderson",
     "author_email": "cbanders@stanford.edu",
@@ -24,15 +29,15 @@
         "SDM",
         "species distribution modeling",
         "maxent",
     ],
     "packages": ["elapid"],
     "include_package_data": True,
     "install_requires": requirements,
-    "python_requires": ">=3.7.0,<3.9.0",
+    "python_requires": ">=3.7.0",
     "platforms": "any",
     "classifiers": [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 }
```

