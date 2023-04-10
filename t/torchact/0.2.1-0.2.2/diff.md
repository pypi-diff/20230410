# Comparing `tmp/torchact-0.2.1.tar.gz` & `tmp/torchact-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchact-0.2.1.tar", last modified: Mon Apr 10 15:30:33 2023, max compression
+gzip compressed data, was "torchact-0.2.2.tar", last modified: Mon Apr 10 15:35:24 2023, max compression
```

## Comparing `torchact-0.2.1.tar` & `torchact-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 15:30:33.171489 torchact-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-04-10 15:26:26.000000 torchact-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4134 2023-04-10 15:30:33.170475 torchact-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3103 2023-04-10 15:26:26.000000 torchact-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 15:30:33.172589 torchact-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1703 2023-04-10 15:26:26.000000 torchact-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:30:33.141497 torchact-0.2.1/torchact/
--rw-rw-rw-   0        0        0       48 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/__config__.py
--rw-rw-rw-   0        0        0      465 2023-04-10 15:27:07.000000 torchact-0.2.1/torchact/__init__.py
--rw-rw-rw-   0        0        0      947 2023-04-10 15:27:02.000000 torchact-0.2.1/torchact/ab_relu.py
--rw-rw-rw-   0        0        0      878 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/elu.py
--rw-rw-rw-   0        0        0      975 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/leaky_relu.py
--rw-rw-rw-   0        0        0      644 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/log_sigmoid.py
--rw-rw-rw-   0        0        0      827 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/log_softmax.py
--rw-rw-rw-   0        0        0      740 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/relu.py
--rw-rw-rw-   0        0        0      615 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/sigmoid.py
--rw-rw-rw-   0        0        0      917 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/sinlu.py
--rw-rw-rw-   0        0        0      839 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/softmax.py
--rw-rw-rw-   0        0        0      573 2023-04-10 15:26:26.000000 torchact-0.2.1/torchact/step.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:30:33.167883 torchact-0.2.1/torchact.egg-info/
--rw-rw-rw-   0        0        0     4134 2023-04-10 15:30:32.000000 torchact-0.2.1/torchact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-10 15:30:32.000000 torchact-0.2.1/torchact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 15:30:32.000000 torchact-0.2.1/torchact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 15:30:32.000000 torchact-0.2.1/torchact.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 15:35:24.304191 torchact-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-10 15:26:26.000000 torchact-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4134 2023-04-10 15:35:24.302909 torchact-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3103 2023-04-10 15:26:26.000000 torchact-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 15:35:24.304191 torchact-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1703 2023-04-10 15:26:26.000000 torchact-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 15:35:24.275664 torchact-0.2.2/torchact/
+-rw-rw-rw-   0        0        0       48 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/__config__.py
+-rw-rw-rw-   0        0        0      465 2023-04-10 15:34:55.000000 torchact-0.2.2/torchact/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-04-10 15:34:23.000000 torchact-0.2.2/torchact/ab_relu.py
+-rw-rw-rw-   0        0        0      878 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/elu.py
+-rw-rw-rw-   0        0        0      975 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/leaky_relu.py
+-rw-rw-rw-   0        0        0      644 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/log_sigmoid.py
+-rw-rw-rw-   0        0        0      827 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/log_softmax.py
+-rw-rw-rw-   0        0        0      740 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/relu.py
+-rw-rw-rw-   0        0        0      615 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/sigmoid.py
+-rw-rw-rw-   0        0        0      917 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/sinlu.py
+-rw-rw-rw-   0        0        0      839 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/softmax.py
+-rw-rw-rw-   0        0        0      573 2023-04-10 15:26:26.000000 torchact-0.2.2/torchact/step.py
+drwxrwxrwx   0        0        0        0 2023-04-10 15:35:24.300350 torchact-0.2.2/torchact.egg-info/
+-rw-rw-rw-   0        0        0     4134 2023-04-10 15:35:23.000000 torchact-0.2.2/torchact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-10 15:35:24.000000 torchact-0.2.2/torchact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 15:35:23.000000 torchact-0.2.2/torchact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 15:35:23.000000 torchact-0.2.2/torchact.egg-info/top_level.txt
```

### Comparing `torchact-0.2.1/LICENSE` & `torchact-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/PKG-INFO` & `torchact-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchact
-Version: 0.2.1
+Version: 0.2.2
 Summary: TorchAct, collection of activation function for PyTorch.
 Home-page: https://github.com/kaintels/torchact
 Author: Seungwoo Han
 Author-email: seungwoohan0108@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `torchact-0.2.1/README.md` & `torchact-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/setup.py` & `torchact-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/ab_relu.py` & `torchact-0.2.2/torchact/ab_relu.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,10 +22,13 @@
 
     def __init__(self, alpha: float = 1.0, inplace: bool = FALSE_CONDITION):
         super(ABReLU, self).__init__()
         self.alpha = alpha
         self.inplace = inplace
 
     def forward(self, x):
-        beta = self.alpha * torch.mean(x)
+        if len(x.shape) < 2:
+            beta = self.alpha * torch.mean(x)
+        else:
+            beta = self.alpha * torch.mean(x, -2)
         x_out = x - beta
-        return torch.clip(x_out, min=0)
+        return torch.clip(x_out, min=0)
```

### Comparing `torchact-0.2.1/torchact/elu.py` & `torchact-0.2.2/torchact/elu.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/leaky_relu.py` & `torchact-0.2.2/torchact/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/log_sigmoid.py` & `torchact-0.2.2/torchact/log_sigmoid.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/log_softmax.py` & `torchact-0.2.2/torchact/log_softmax.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/relu.py` & `torchact-0.2.2/torchact/relu.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/sigmoid.py` & `torchact-0.2.2/torchact/sigmoid.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/sinlu.py` & `torchact-0.2.2/torchact/sinlu.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/softmax.py` & `torchact-0.2.2/torchact/softmax.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact/step.py` & `torchact-0.2.2/torchact/step.py`

 * *Files identical despite different names*

### Comparing `torchact-0.2.1/torchact.egg-info/PKG-INFO` & `torchact-0.2.2/torchact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchact
-Version: 0.2.1
+Version: 0.2.2
 Summary: TorchAct, collection of activation function for PyTorch.
 Home-page: https://github.com/kaintels/torchact
 Author: Seungwoo Han
 Author-email: seungwoohan0108@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
```

