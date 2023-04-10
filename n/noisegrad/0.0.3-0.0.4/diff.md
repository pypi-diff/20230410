# Comparing `tmp/noisegrad-0.0.3.tar.gz` & `tmp/noisegrad-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisegrad-0.0.3.tar", last modified: Sun Apr  9 22:02:45 2023, max compression
+gzip compressed data, was "noisegrad-0.0.4.tar", last modified: Mon Apr 10 18:56:52 2023, max compression
```

## Comparing `noisegrad-0.0.3.tar` & `noisegrad-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1146 2023-04-09 22:02:38.024743 noisegrad-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1959 2023-04-09 22:02:38.024743 noisegrad-0.0.3/README.md
--rw-r--r--   0        0        0      124 2023-04-09 22:02:38.032743 noisegrad-0.0.3/noisegrad/__init__.py
--rw-r--r--   0        0        0     2943 2023-04-09 22:02:38.032743 noisegrad-0.0.3/noisegrad/explainers.py
--rw-r--r--   0        0        0     6645 2023-04-09 22:02:38.032743 noisegrad-0.0.3/noisegrad/noisegrad.py
--rw-r--r--   0        0        0       64 2023-04-09 22:02:38.032743 noisegrad-0.0.3/noisegrad/py.typed
--rw-r--r--   0        0        0     2575 2023-04-09 22:02:38.032743 noisegrad-0.0.3/noisegrad/utils.py
--rw-r--r--   0        0        0     6357 2023-04-09 22:02:38.032743 noisegrad-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 noisegrad-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1146 2023-04-10 18:56:41.272130 noisegrad-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1959 2023-04-10 18:56:41.272130 noisegrad-0.0.4/README.md
+-rw-r--r--   0        0        0      124 2023-04-10 18:56:41.280131 noisegrad-0.0.4/noisegrad/__init__.py
+-rw-r--r--   0        0        0     3839 2023-04-10 18:56:41.280131 noisegrad-0.0.4/noisegrad/explainers.py
+-rw-r--r--   0        0        0     6707 2023-04-10 18:56:41.280131 noisegrad-0.0.4/noisegrad/noisegrad.py
+-rw-r--r--   0        0        0       64 2023-04-10 18:56:41.280131 noisegrad-0.0.4/noisegrad/py.typed
+-rw-r--r--   0        0        0     2575 2023-04-10 18:56:41.280131 noisegrad-0.0.4/noisegrad/utils.py
+-rw-r--r--   0        0        0     6357 2023-04-10 18:56:41.280131 noisegrad-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 noisegrad-0.0.4/PKG-INFO
```

### Comparing `noisegrad-0.0.3/LICENSE.md` & `noisegrad-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.3/README.md` & `noisegrad-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.3/noisegrad/explainers.py` & `noisegrad-0.0.4/noisegrad/explainers.py`

 * *Files 27% similar despite different names*

```diff
@@ -74,22 +74,48 @@
                 kwargs.get("img_size", 224),
                 kwargs.get("img_size", 224),
             )
             .cpu()
             .data
         )
 
+    def explain_integrated_gradients(
+        model: nn.Module,
+        input_embeddings: torch.Tensor,
+        y_batch: torch.Tensor,
+        num_steps: int = 10,
+        **kwargs,
+    ) -> torch.Tensor:
+        def predict_fn(x):
+            return model(None, inputs_embeds=x, **kwargs)
+
+        explainer = IntegratedGradients(predict_fn)
+        grads = explainer.attribute(
+            inputs=input_embeddings, n_steps=num_steps, target=y_batch
+        )
+
+        scores = torch.linalg.norm(grads, dim=-1)
+
+        return scores
+
+
+def explain_gradient_norm(
+    model: nn.Module, input_embeddings: torch.Tensor, y_batch: torch.Tensor, **kwargs
+) -> torch.Tensor:
+    logits = model(None, inputs_embeds=input_embeddings, **kwargs)
+    logits_for_class = logits_for_labels(logits, y_batch)
+    grads = torch.autograd.grad(torch.unbind(logits_for_class), input_embeddings)[0]
+    scores = torch.linalg.norm(grads, dim=-1)
+    return scores
+
 
 def explain_gradient_x_input(
-    model: nn.Module,
-    input_embeddings: torch.Tensor,
-    y_batch: torch.Tensor,
-    attention_mask: torch.Tensor | None,
+    model: nn.Module, input_embeddings: torch.Tensor, y_batch: torch.Tensor, **kwargs
 ) -> torch.Tensor:
-    logits = model(None, attention_mask, inputs_embeds=input_embeddings).logits
+    logits = model(None, **kwargs, inputs_embeds=input_embeddings).logits
     logits_for_class = logits_for_labels(logits, y_batch)
     grads = torch.autograd.grad(torch.unbind(logits_for_class), input_embeddings)[0]
     return torch.sum(grads * input_embeddings, dim=-1).detach()
 
 
 def logits_for_labels(logits: torch.Tensor, y_batch: torch.Tensor) -> torch.Tensor:
-    return logits[torch.arange(0, logits.shape[0], dtype=torch.int64), y_batch]
+    return logits[torch.arange(0, logits.shape[0], dtype=torch.int), y_batch]
```

### Comparing `noisegrad-0.0.3/noisegrad/noisegrad.py` & `noisegrad-0.0.4/noisegrad/noisegrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,23 @@
 import torch.nn as nn
 from tqdm.auto import tqdm
 
 NoiseType = Literal["multiplicative", "additive"]
 
 
 class ExplanationFn(Protocol):
-
-    def __call__(self, mode: nn.Module, x_batch: torch.Tensor, y_batch: torch.Tensor, *args, **kwargs) -> torch.Tensor: ...
+    def __call__(
+        self,
+        mode: nn.Module,
+        x_batch: torch.Tensor,
+        y_batch: torch.Tensor,
+        *args,
+        **kwargs,
+    ) -> torch.Tensor:
+        ...
 
 
 class NoiseGradConfig(NamedTuple):
     """
     mean:
         Mean of normal distribution, from which noise added to weights is sampled.
     std:
```

### Comparing `noisegrad-0.0.3/noisegrad/utils.py` & `noisegrad-0.0.4/noisegrad/utils.py`

 * *Files identical despite different names*

### Comparing `noisegrad-0.0.3/pyproject.toml` & `noisegrad-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "noisegrad"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3"  # Required
+version = "0.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A explanation enhancement method."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `noisegrad-0.0.3/PKG-INFO` & `noisegrad-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisegrad
-Version: 0.0.3
+Version: 0.0.4
 Summary: A explanation enhancement method.
 Keywords: explainable ai,xai,machine learning,deep learning
 Author-email: Kirill Bykov <kirill.bykov@campus.tu-berlin.de>, Anna Hedström <anna.hedstroem@tu-berlin.de>, Shinichi Nakajima <nakajima@tu-berlin.de>, "Marina M.-C. Höhne" <marina.hoehne@tu-berlin.de>, Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Maintainer-email: Kirill Bykov <kirill.bykov@campus.tu-berlin.de>, Anna Hedström <anna.hedstroem@tu-berlin.de>, Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

