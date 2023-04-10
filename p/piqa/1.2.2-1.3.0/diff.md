# Comparing `tmp/piqa-1.2.2.tar.gz` & `tmp/piqa-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqa-1.2.2.tar", last modified: Tue Mar 29 16:57:50 2022, max compression
+gzip compressed data, was "piqa-1.3.0.tar", last modified: Mon Apr 10 18:36:30 2023, max compression
```

## Comparing `piqa-1.2.2.tar` & `piqa-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-03-29 16:57:50.379420 piqa-1.2.2/
--rwxrwxrwx   0 francois  (1000) francois  (1000)     7951 2022-03-29 16:57:50.377419 piqa-1.2.2/PKG-INFO
--rwxrwxrwx   0 francois  (1000) francois  (1000)     5995 2022-02-12 20:39:24.000000 piqa-1.2.2/README.md
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-03-29 16:57:50.267419 piqa-1.2.2/piqa/
--rwxrwxrwx   0 francois  (1000) francois  (1000)      446 2022-02-12 20:39:24.000000 piqa-1.2.2/piqa/__init__.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     9531 2022-02-13 10:24:43.000000 piqa-1.2.2/piqa/fsim.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     9009 2022-02-13 10:28:30.000000 piqa-1.2.2/piqa/gmsd.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     5161 2022-02-13 11:22:29.000000 piqa-1.2.2/piqa/haarpsi.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     6711 2022-02-13 10:24:55.000000 piqa-1.2.2/piqa/lpips.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     5774 2022-02-13 10:29:34.000000 piqa-1.2.2/piqa/mdsi.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     2904 2022-02-12 20:39:24.000000 piqa-1.2.2/piqa/psnr.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     9640 2022-03-29 15:34:02.000000 piqa-1.2.2/piqa/ssim.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     2367 2022-02-12 20:39:24.000000 piqa-1.2.2/piqa/tv.py
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-03-29 16:57:50.367420 piqa-1.2.2/piqa/utils/
--rwxrwxrwx   0 francois  (1000) francois  (1000)     3578 2022-02-12 20:39:24.000000 piqa-1.2.2/piqa/utils/__init__.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     3242 2022-03-29 16:37:48.000000 piqa-1.2.2/piqa/utils/color.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     5887 2022-02-12 20:39:24.000000 piqa-1.2.2/piqa/utils/complex.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)    10296 2022-03-29 16:03:07.000000 piqa-1.2.2/piqa/utils/functional.py
--rwxrwxrwx   0 francois  (1000) francois  (1000)     8040 2022-02-13 10:24:56.000000 piqa-1.2.2/piqa/vsi.py
-drwxrwxrwx   0 francois  (1000) francois  (1000)        0 2022-03-29 16:57:50.316420 piqa-1.2.2/piqa.egg-info/
--rwxrwxrwx   0 francois  (1000) francois  (1000)     7951 2022-03-29 16:57:49.000000 piqa-1.2.2/piqa.egg-info/PKG-INFO
--rwxrwxrwx   0 francois  (1000) francois  (1000)      382 2022-03-29 16:57:50.000000 piqa-1.2.2/piqa.egg-info/SOURCES.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)        1 2022-03-29 16:57:49.000000 piqa-1.2.2/piqa.egg-info/dependency_links.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)       32 2022-03-29 16:57:49.000000 piqa-1.2.2/piqa.egg-info/requires.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)        5 2022-03-29 16:57:49.000000 piqa-1.2.2/piqa.egg-info/top_level.txt
--rwxrwxrwx   0 francois  (1000) francois  (1000)       38 2022-03-29 16:57:50.380419 piqa-1.2.2/setup.cfg
--rwxrwxrwx   0 francois  (1000) francois  (1000)     1205 2022-03-29 16:44:14.000000 piqa-1.2.2/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-03-26 10:06:00.000000 piqa-1.3.0/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5815 2023-04-10 18:36:30.581264 piqa-1.3.0/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4994 2023-04-10 18:33:28.000000 piqa-1.3.0/README.md
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.577264 piqa-1.3.0/piqa/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      320 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5241 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/fid.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9181 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/fsim.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9119 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/gmsd.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5170 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/haarpsi.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4990 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/lpips.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5547 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/mdsi.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2995 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/psnr.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9782 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/ssim.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2438 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/tv.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/piqa/utils/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3024 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3856 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/color.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    11466 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/utils/functional.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     7714 2023-04-10 18:33:28.000000 piqa-1.3.0/piqa/vsi.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 18:36:30.581264 piqa-1.3.0/piqa.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5815 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      390 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       34 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-04-10 18:36:30.000000 piqa-1.3.0/piqa.egg-info/top_level.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      899 2023-04-10 18:36:30.581264 piqa-1.3.0/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-04-10 18:33:28.000000 piqa-1.3.0/setup.py
```

### Comparing `piqa-1.2.2/README.md` & `piqa-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,126 @@
-<p align="center"><img src="https://raw.githubusercontent.com/francois-rozet/piqa/master/banner.svg" width="80%"></p>
+Metadata-Version: 2.1
+Name: piqa
+Version: 1.3.0
+Summary: PyTorch Image Quality Assessment
+Home-page: https://github.com/francois-rozet/piqa
+Author: François Rozet
+Author-email: francois.rozet@outlook.com
+License: MIT License
+Project-URL: Documentation, https://piqa.readthedocs.io
+Project-URL: Source, https://github.com/francois-rozet/piqa
+Project-URL: Tracker, https://github.com/francois-rozet/piqa/issues
+Keywords: torch,vision,image,quality,metrics
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-> PIQA is not endorsed by Facebook, Inc.; PyTorch, the PyTorch logo and any related marks are trademarks of Facebook, Inc.
+<p align="center"><img src="https://raw.githubusercontent.com/francois-rozet/piqa/master/docs/images/banner.svg" width="80%"></p>
 
 # PyTorch Image Quality Assessment
 
-The `piqa` package is a collection of measures and metrics for image quality assessment in various image processing tasks such as denoising, super-resolution, image interpolation, etc. It relies only on [PyTorch](https://github.com/pytorch/pytorch) and takes advantage of its efficiency and automatic differentiation.
-
-PIQA is directly inspired from the [`piq`](https://github.com/photosynthesis-team/piq) project, but focuses on the conciseness, readability and understandability of its (sub-)modules, such that anyone can easily reuse and/or adapt them to its needs.
-
-However, conciseness should never be at the expense of efficiency; PIQA's implementations are up to 3 times faster than those of other IQA PyTorch packages like [`kornia`](https://github.com/kornia/kornia), [`piq`](https://github.com/photosynthesis-team/piq) and [`IQA-pytorch`](https://github.com/dingkeyan93/IQA-optimization).
+PIQA is a collection of PyTorch metrics for image quality assessment in various image processing tasks such as generation, denoising, super-resolution, interpolation, etc. It focuses on the efficiency, conciseness and understandability of its (sub-)modules, such that anyone can easily reuse and/or adapt them to its needs.
 
 > PIQA should be pronounced *pika* (like Pikachu ⚡️)
 
 ## Installation
 
-The `piqa` package is available on [PyPI](https://pypi.org/project/piqa/), which means it is installable with `pip`:
+The `piqa` package is available on [PyPI](https://pypi.org/project/piqa), which means it is installable via `pip`.
 
-```bash
+```
 pip install piqa
 ```
 
-Alternatively, if you need the latest features, you can install it using
+Alternatively, if you need the latest features, you can install it from the repository.
 
-```bash
-pip install git+https://github.com/francois-rozet/piqa
 ```
-
-or copy the package directly to your project, with
-
-```bash
-git clone https://github.com/francois-rozet/piqa
-cp -R piqa/piqa <path/to/project>/piqa
+pip install git+https://github.com/francois-rozet/piqa
 ```
 
-## Documentation
-
-The [documentation](https://francois-rozet.github.io/piqa/) of this package is generated automatically by [`Sphinx`](https://pypi.org/project/Sphinx/).
-
 ## Getting started
 
-In `piqa`, each metric is associated to a class, child of `torch.nn.Module`, which has to be instantiated to evaluate the metric.
+In `piqa`, each metric is associated to a class, child of `torch.nn.Module`, which has to be instantiated to evaluate the metric. All metrics are differentiable and support CPU and GPU (CUDA).
 
 ```python
 import torch
+import piqa
 
 # PSNR
-from piqa import PSNR
-
 x = torch.rand(5, 3, 256, 256)
 y = torch.rand(5, 3, 256, 256)
 
-psnr = PSNR()
+psnr = piqa.PSNR()
 l = psnr(x, y)
 
 # SSIM
-from piqa import SSIM
-
 x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
 y = torch.rand(5, 3, 256, 256).cuda()
 
-ssim = SSIM().cuda()
+ssim = piqa.SSIM().cuda()
 l = 1 - ssim(x, y)
 l.backward()
 ```
 
 Like `torch.nn` built-in components, these classes are based on functional definitions of the metrics, which are less user-friendly, but more versatile.
 
 ```python
-import torch
-
 from piqa.ssim import ssim
 from piqa.utils.functional import gaussian_kernel
 
-x = torch.rand(5, 3, 256, 256)
-y = torch.rand(5, 3, 256, 256)
-
-kernel = gaussian_kernel(11, sigma=1.5).repeat(3, 1, 1)
+kernel = gaussian_kernel(11, sigma=1.5).expand(3, 11, 11)
 
-l = ssim(x, y, kernel=kernel, channel_avg=False)
+l = 1 - ssim(x, y, kernel=kernel)
 ```
 
-### Metrics
+For more information, check out the documentation at [piqa.readthedocs.io](https://piqa.readthedocs.io).
 
-| Acronym | Class     | Range    | Objective | Year | Metric                                                                                               |
-|:-------:|:---------:|:--------:|:---------:|:----:|------------------------------------------------------------------------------------------------------|
-| TV      | `TV`      | `[0, ∞]` | /         | 1937 | [Total Variation](https://en.wikipedia.org/wiki/Total_variation)                                     |
-| PSNR    | `PSNR`    | `[0, ∞]` | max       | /    | [Peak Signal-to-Noise Ratio](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio)               |
-| SSIM    | `SSIM`    | `[0, 1]` | max       | 2004 | [Structural Similarity](https://en.wikipedia.org/wiki/Structural_similarity)                         |
-| MS-SSIM | `MS_SSIM` | `[0, 1]` | max       | 2004 | [Multi-Scale Structural Similarity](https://ieeexplore.ieee.org/document/1292216/)                   |
-| LPIPS   | `LPIPS`   | `[0, ∞]` | min       | 2018 | [Learned Perceptual Image Patch Similarity](https://arxiv.org/abs/1801.03924)                        |
-| GMSD    | `GMSD`    | `[0, ∞]` | min       | 2013 | [Gradient Magnitude Similarity Deviation](https://arxiv.org/abs/1308.3052)                           |
-| MS-GMSD | `MS_GMSD` | `[0, ∞]` | min       | 2017 | [Multi-Scale Gradient Magnitude Similarity Deviation](https://ieeexplore.ieee.org/document/7952357)  |
-| MDSI    | `MDSI`    | `[0, ∞]` | min       | 2016 | [Mean Deviation Similarity Index](https://arxiv.org/abs/1608.07433)                                  |
-| HaarPSI | `HaarPSI` | `[0, 1]` | max       | 2018 | [Haar Perceptual Similarity Index](https://arxiv.org/abs/1607.06140)                                 |
-| VSI     | `VSI`     | `[0, 1]` | max       | 2014 | [Visual Saliency-based Index](https://ieeexplore.ieee.org/document/6873260)                          |
-| FSIM    | `FSIM`    | `[0, 1]` | max       | 2011 | [Feature Similarity](https://ieeexplore.ieee.org/document/5705575)                                   |
+### Available metrics
 
-### JIT
+| Class     | Range  | Objective | Year | Metric                                                                                               |
+|:---------:|:------:|:---------:|:----:|------------------------------------------------------------------------------------------------------|
+| `TV`      | [0, ∞] | /         | 1937 | [Total Variation](https://en.wikipedia.org/wiki/Total_variation)                                     |
+| `PSNR`    | [0, ∞] | max       | /    | [Peak Signal-to-Noise Ratio](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio)               |
+| `SSIM`    | [0, 1] | max       | 2004 | [Structural Similarity](https://en.wikipedia.org/wiki/Structural_similarity)                         |
+| `MS_SSIM` | [0, 1] | max       | 2004 | [Multi-Scale Structural Similarity](https://ieeexplore.ieee.org/document/1292216/)                   |
+| `LPIPS`   | [0, ∞] | min       | 2018 | [Learned Perceptual Image Patch Similarity](https://arxiv.org/abs/1801.03924)                        |
+| `GMSD`    | [0, ∞] | min       | 2013 | [Gradient Magnitude Similarity Deviation](https://arxiv.org/abs/1308.3052)                           |
+| `MS_GMSD` | [0, ∞] | min       | 2017 | [Multi-Scale Gradient Magnitude Similarity Deviation](https://ieeexplore.ieee.org/document/7952357)  |
+| `MDSI`    | [0, ∞] | min       | 2016 | [Mean Deviation Similarity Index](https://arxiv.org/abs/1608.07433)                                  |
+| `HaarPSI` | [0, 1] | max       | 2018 | [Haar Perceptual Similarity Index](https://arxiv.org/abs/1607.06140)                                 |
+| `VSI`     | [0, 1] | max       | 2014 | [Visual Saliency-based Index](https://ieeexplore.ieee.org/document/6873260)                          |
+| `FSIM`    | [0, 1] | max       | 2011 | [Feature Similarity](https://ieeexplore.ieee.org/document/5705575)                                   |
+| `FID`     | [0, ∞] | min       | 2017 | [Fréchet Inception Distance](https://arxiv.org/abs/1706.08500)                                       |
 
-Most functional components of `piqa` support  PyTorch's JIT, *i.e.* [TorchScript](https://pytorch.org/docs/stable/jit.html), which is a way to create serializable and optimizable functions from PyTorch code.
+### Tracing
 
-By default, jitting is disabled for those components. To enable it, the `PIQA_JIT` environment variable has to be set to `1`. To do so temporarily,
+All metrics of `piqa` support [PyTorch's tracing](https://pytorch.org/docs/stable/generated/torch.jit.trace.html), which optimizes their execution, especially on GPU.
 
-* UNIX-like `bash`
-
-```bash
-export PIQA_JIT=1
-```
-
-* Windows `cmd`
-
-```cmd
-set PIQA_JIT=1
-```
-
-* Microsoft `PowerShell`
+```python
+ssim = piqa.SSIM().cuda()
+ssim_traced = torch.jit.trace(ssim, (x, y))
 
-```powershell
-$env:PIQA_JIT=1
+l = 1 - ssim_traced(x, y)  # should be faster ¯\_(ツ)_/¯
 ```
 
 ### Assert
 
-PIQA uses type assertions to raise meaningful messages when an object-oriented component doesn't receive an input of the expected type. This feature eases a lot early prototyping and debugging, but it might hurt a little the performances.
-
-If you need the absolute best performances, the assertions can be disabled with the Python flag [`-O`](https://docs.python.org/3/using/cmdline.html#cmdoption-o). For example,
+PIQA uses type assertions to raise meaningful messages when a metric doesn't receive an input of the expected type. This feature eases a lot early prototyping and debugging, but it might hurt a little the performances. If you need the absolute best performances, the assertions can be disabled with the Python flag [`-O`](https://docs.python.org/3/using/cmdline.html#cmdoption-o). For example,
 
-```bash
+```
 python -O your_awesome_code_using_piqa.py
 ```
 
 Alternatively, you can disable PIQA's type assertions within your code with
 
 ```python
-from piqa.utils import set_debug
-set_debug(False)
+piqa.utils.set_debug(False)
 ```
+
+## Contributing
+
+If you have a question, an issue or would like to contribute, please read our [contributing guidelines](https://github.com/francois-rozet/piqa/blob/master/CONTRIBUTING.md).
```

### Comparing `piqa-1.2.2/piqa/fsim.py` & `piqa-1.3.0/piqa/fsim.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,142 +2,144 @@
 
 This module implements the FSIM in PyTorch.
 
 Original:
     https://www4.comp.polyu.edu.hk/~cslzhang/IQA/FSIM/FSIM.htm
 
 References:
-    .. [Zhang2011] FSIM: A Feature Similarity Index for Image Quality Assessment (Zhang et al., 2011)
+    | FSIM: A Feature Similarity Index for Image Quality Assessment (Zhang et al., 2011)
+    | https://ieeexplore.ieee.org/document/5705575
 
-    .. [Kovesi1999] Image Features From Phase Congruency (Kovesi, 1999)
+    | Image Features From Phase Congruency (Kovesi, 1999)
 """
 
 import math
 import torch
 import torch.fft as fft
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
-from .utils import complex as cx
+from .utils import assert_type
 from .utils.color import ColorConv
 from .utils.functional import (
     scharr_kernel,
     gradient_kernel,
     filter_grid,
     log_gabor,
     channel_conv,
     l2_norm,
+    downsample,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def fsim(
     x: Tensor,
     y: Tensor,
     pc_x: Tensor,
     pc_y: Tensor,
     kernel: Tensor,
-    value_range: float = 1.,
+    value_range: float = 1.0,
     t1: float = 0.85,
-    t2: float = 160. / (255. ** 2),
-    t3: float = 200. / (255. ** 2),
-    t4: float = 200. / (255. ** 2),
+    t2: float = 160 / 255 ** 2,
+    t3: float = 200 / 255 ** 2,
+    t4: float = 200 / 255 ** 2,
     lmbda: float = 0.03,
 ) -> Tensor:
-    r"""Returns the FSIM between :math:`x` and :math:`y`,
-    without color space conversion and downsampling.
+    r"""Returns the FSIM between :math:`x` and :math:`y`, without color space
+    conversion and downsampling.
 
     Args:
         x: An input tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         y: A target tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         pc_x: The input phase congruency, :math:`(N, H, W)`.
         pc_y: The target phase congruency, :math:`(N, H, W)`.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Zhang2011]_.
+        For the remaining arguments, refer to Zhang et al. (2011).
 
     Returns:
         The FSIM vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> filters = pc_filters(x)
         >>> pc_x = phase_congruency(x[:, :1], filters)
         >>> pc_y = phase_congruency(y[:, :1], filters)
         >>> kernel = gradient_kernel(scharr_kernel())
         >>> l = fsim(x, y, pc_x, pc_y, kernel)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     t2 *= value_range ** 2
     t3 *= value_range ** 2
     t4 *= value_range ** 2
 
     y_x, y_y = x[:, :1], y[:, :1]
 
     # Phase congruency similarity
     pc_m = torch.max(pc_x, pc_y)
     s_pc = (2 * pc_x * pc_y + t1) / (pc_x ** 2 + pc_y ** 2 + t1)
 
     # Gradient magnitude similarity
-    pad = kernel.size(-1) // 2
+    pad = kernel.shape[-1] // 2
 
-    g_x = l2_norm(channel_conv(y_x, kernel, padding=pad), dims=[1])
-    g_y = l2_norm(channel_conv(y_y, kernel, padding=pad), dims=[1])
+    g_x = l2_norm(channel_conv(y_x, kernel, padding=pad), dim=1)
+    g_y = l2_norm(channel_conv(y_y, kernel, padding=pad), dim=1)
 
     s_g = (2 * g_x * g_y + t2) / (g_x ** 2 + g_y ** 2 + t2)
 
     # Chrominance similarity
     s_l = s_pc * s_g
 
-    if x.size(1) == 3:
+    if x.shape[1] == 3:
         i_x, i_y = x[:, 1], y[:, 1]
         q_x, q_y = x[:, 2], y[:, 2]
 
         s_i = (2 * i_x * i_y + t3) / (i_x ** 2 + i_y ** 2 + t3)
         s_q = (2 * q_x * q_y + t4) / (q_x ** 2 + q_y ** 2 + t4)
 
         s_iq = s_i * s_q
-        s_iq = cx.complx(s_iq, torch.zeros_like(s_iq))
-        s_iq_lambda =  cx.real(cx.pow(s_iq, lmbda))
+        s_iq = torch.complex(s_iq, torch.zeros_like(s_iq))
+        s_iq_lambda = (s_iq ** lmbda).real
 
         s_l = s_l * s_iq_lambda
 
     # Feature similarity
     fs = (s_l * pc_m).sum(dim=(-1, -2)) / pc_m.sum(dim=(-1, -2))
 
     return fs
 
 
-@_jit
+@torch.jit.script_if_tracing
 def pc_filters(
     x: Tensor,
     scales: int = 4,
     orientations: int = 4,
-    wavelength: float = 6.,
-    factor: float = 2.,
+    wavelength: float = 6.0,
+    factor: float = 2.0,
     sigma_f: float = 0.5978,  # -log(0.55)
     sigma_theta: float = 0.6545,  # pi / (4 * 1.2)
 ) -> Tensor:
     r"""Returns the log-Gabor filters for :func:`phase_congruency`.
 
     Args:
         x: An input tensor, :math:`(*, H, W)`.
         scales: The number of scales, :math:`S_1`.
         orientations: The number of orientations, :math:`S_2`.
 
     Note:
-        For the remaining arguments, refer to [Kovesi1999]_.
+        For the remaining arguments, refer to Kovesi (1999).
 
     Returns:
         The filters tensor, :math:`(S_1, S_2, H, W)`.
     """
 
     r, theta = filter_grid(x)
 
@@ -155,15 +157,15 @@
     radial = torch.stack(radial)
 
     # Angular
     cos_theta = torch.cos(theta)
     sin_theta = torch.sin(theta)
 
     theta_j = math.pi * torch.arange(orientations).to(x) / orientations
-    theta_j = theta_j.view(orientations, 1, 1)
+    theta_j = theta_j.reshape(orientations, 1, 1)
 
     ## Measure (theta - theta_j) in the sine/cosine domains
     ## to prevent wrap-around errors
     delta_sin = sin_theta * theta_j.cos() - cos_theta * theta_j.sin()
     delta_cos = cos_theta * theta_j.cos() + sin_theta * theta_j.sin()
     delta_theta = torch.atan2(delta_sin, delta_cos)
 
@@ -171,119 +173,109 @@
 
     # Combination
     filters = lowpass * radial[:, None] * angular[None, :]
 
     return filters
 
 
-@_jit
+@torch.jit.script_if_tracing
 def phase_congruency(
     x: Tensor,
     filters: Tensor,
-    value_range: float = 1.,
-    k: float = 2.,
+    value_range: float = 1.0,
+    k: float = 2.0,
     rescale: float = 1.7,
     eps: float = 1e-8,
 ) -> Tensor:
     r"""Returns the Phase Congruency (PC) of :math:`x`.
 
     Args:
         x: An input tensor, :math:`(N, 1, H, W)`.
         filters: The frequency domain filters, :math:`(S_1, S_2, H, W)`.
-        value_range: The value range :math:`L` of the input (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the input (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Kovesi1999]_.
+        For the remaining arguments, refer to Kovesi (1999).
 
     Returns:
         The PC tensor, :math:`(N, H, W)`.
 
     Example:
         >>> x = torch.rand(5, 1, 256, 256)
         >>> filters = pc_filters(x)
         >>> pc = phase_congruency(x, filters)
-        >>> pc.size()
+        >>> pc.shape
         torch.Size([5, 256, 256])
     """
 
-    x = x * (255. / value_range)
+    x = x * (255 / value_range)
 
     # Filters
     M_hat = filters
-    M = fft.ifft2(M_hat)
-    M = cx.real(torch.view_as_real(M))
+    M = fft.ifft2(M_hat).real
 
     # Even & odd (real and imaginary) responses
-    eo = fft.ifft2(fft.fft2(x[:, None]) * M_hat)
-    eo = torch.view_as_real(eo)
-
-    # Amplitude
-    A = cx.mod(eo)
+    eo = fft.ifft2(fft.fft2(x)[:, None] * M_hat)
 
     # Expected E^2
-    A2 = A[:, 0] ** 2
-    median_A2, _ = A2.flatten(-2).median(dim=-1)
+    A = eo.abs()
+    A2 = A[:, 0].square()
+    median_A2 = A2.flatten(-2).median(dim=-1).values
     expect_A2 = median_A2 / math.log(2)
 
-    expect_M2_hat = (M_hat[0] ** 2).mean(dim=(-1, -2))
+    expect_M2_hat = M_hat[0].square().mean(dim=(-1, -2))
     expect_MiMj = (M[:, None] * M[None, :]).sum(dim=(0, 1, 3, 4))
 
     expect_E2 = expect_A2 * expect_MiMj / expect_M2_hat
 
     # Threshold
     sigma_G = expect_E2.sqrt()
-    mu_R = sigma_G * (math.pi / 2) ** 0.5
-    sigma_R = sigma_G * (2 - math.pi / 2) ** 0.5
+    mu_R = sigma_G * math.sqrt(math.pi / 2)
+    sigma_R = sigma_G * math.sqrt(2 - math.pi / 2)
 
     T = mu_R + k * sigma_R
-    T = T / rescale  # emprirical rescaling
+    T = T / rescale  # empirical rescaling
     T = T[..., None, None]
 
     # Phase deviation
-    FH = eo.sum(dim=1, keepdim=True)
-    phi_eo = FH / (cx.mod(FH)[..., None] + eps)
+    fh = eo.sum(dim=1, keepdim=True)
+    fh = fh / (fh.abs() + eps)
+
+    dot = eo.real * fh.real + eo.imag * fh.imag
+    cross = eo.real * fh.imag - eo.imag * fh.real
 
-    E = cx.dot(eo, phi_eo) - cx.dot(eo, cx.turn(phi_eo)).abs()
-    E = E.sum(dim=1)
+    E = (dot - cross.abs()).sum(dim=1)
 
     # Phase congruency
     pc = (E - T).relu().sum(dim=1) / (A.sum(dim=(1, 2)) + eps)
 
     return pc
 
 
 class FSIM(nn.Module):
-    r"""Creates a criterion that measures the FSIM
-    between an input and a target.
+    r"""Measures the FSIM between an input and a target.
 
-    Before applying :func:`fsim`, the input and target are converted from
-    RBG to Y(IQ) and downsampled by a factor :math:`\frac{\min(H, W)}{256}`.
+    Before applying :func:`fsim`, the input and target are converted from RBG to Y(IQ)
+    and downsampled to a 256-ish resolution.
 
     Args:
         chromatic: Whether to use the chromatic channels (IQ) or not.
         downsample: Whether downsampling is enabled or not.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-            If `None`, use the Scharr kernel instead.
+            If :py:`None`, use the Scharr kernel instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`fsim`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`fsim`.
 
     Example:
-        >>> criterion = FSIM().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = FSIM()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = 1 - criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         chromatic: bool = True,
@@ -294,48 +286,51 @@
     ):
         super().__init__()
 
         if kernel is None:
             kernel = gradient_kernel(scharr_kernel())
 
         self.register_buffer('kernel', kernel)
-        self.register_buffer('filters', torch.zeros((0, 0, 0, 0)))
 
         self.convert = ColorConv('RGB', 'YIQ' if chromatic else 'Y')
         self.downsample = downsample
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The FSIM vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # Downsample
         if self.downsample:
-            _, _, h, w = input.size()
-            M = round(min(h, w) / 256)
-
-            if M > 1:
-                input = F.avg_pool2d(input, kernel_size=M, ceil_mode=True)
-                target = F.avg_pool2d(target, kernel_size=M, ceil_mode=True)
+            x = downsample(x, 256)
+            y = downsample(y, 256)
 
         # RGB to Y(IQ)
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # Phase congruency
-        if self.filters.shape[-2:] != input.shape[-2:]:
-            self.filters = pc_filters(input)
+        filters = pc_filters(x)
 
-        pc_input = phase_congruency(input[:, :1], self.filters, self.value_range)
-        pc_target = phase_congruency(target[:, :1], self.filters, self.value_range)
+        pc_x = phase_congruency(x[:, :1], filters, self.value_range)
+        pc_y = phase_congruency(y[:, :1], filters, self.value_range)
 
         # FSIM
-        l = fsim(input, target, pc_input, pc_target, kernel=self.kernel, **self.kwargs)
+        l = fsim(x, y, pc_x, pc_y, kernel=self.kernel, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/gmsd.py` & `piqa-1.3.0/piqa/gmsd.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,194 +3,187 @@
 
 This module implements the GMSD and MS-GMSD in PyTorch.
 
 Original:
     https://www4.comp.polyu.edu.hk/~cslzhang/IQA/GMSD/GMSD.htm
 
 References:
-    .. [Xue2013] Gradient Magnitude Similarity Deviation: An Highly Efficient Perceptual Image Quality Index (Xue et al., 2013)
+    | Gradient Magnitude Similarity Deviation: An Highly Efficient Perceptual Image Quality Index (Xue et al., 2013)
+    | https://arxiv.org/abs/1308.3052
 
-    .. [Zhang2017] Gradient Magnitude Similarity Deviation on multiple scales for color image quality assessment (Zhang et al., 2017)
+    | Gradient Magnitude Similarity Deviation on multiple scales for color image quality assessment (Zhang et al., 2017)
+    | https://ieeexplore.ieee.org/document/7952357
 """
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
+from .utils import assert_type
 from .utils.color import ColorConv
 from .utils.functional import (
     prewitt_kernel,
     gradient_kernel,
     channel_conv,
     l2_norm,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def gmsd(
     x: Tensor,
     y: Tensor,
     kernel: Tensor,
-    value_range: float = 1.,
-    c: float = 170. / (255. ** 2),
-    alpha: float = 0.,
+    value_range: float = 1.0,
+    c: float = 170 / 255 ** 2,
+    alpha: float = 0.0,
 ) -> Tensor:
-    r"""Returns the GMSD between :math:`x` and :math:`y`,
-    without color space conversion and downsampling.
+    r"""Returns the GMSD between :math:`x` and :math:`y`, without color space
+    conversion and downsampling.
 
-    :math:`\text{GMSD}(x, y)` is the standard deviation of the Gradient
-    Magnitude Similarity (GMS).
+    :math:`\text{GMSD}(x, y)` is the standard deviation of the Gradient Magnitude
+    Similarity (GMS).
 
     .. math::
         \text{GMS}(x, y) &= \frac{(2 - \alpha) \text{GM}(x) \text{GM}(y) + C}
             {\text{GM}(x)^2 + \text{GM}(y)^2 - \alpha \text{GM}(x) \text{GM}(y) + C} \\
         \text{GM}(z) &= \left\| \nabla z \right\|_2
 
     where :math:`\nabla z` is the result of a gradient convolution over :math:`z`.
 
     Args:
         x: An input tensor, :math:`(N, 1, H, W)`.
         y: A target tensor, :math:`(N, 1, H, W)`.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Xue2013]_.
+        For the remaining arguments, refer to Xue et al. (2013).
 
     Returns:
         The GMSD vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 1, 256, 256)
         >>> y = torch.rand(5, 1, 256, 256)
         >>> kernel = gradient_kernel(prewitt_kernel())
         >>> l = gmsd(x, y, kernel)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     c *= value_range ** 2
 
     # Gradient magnitude
-    pad = kernel.size(-1) // 2
+    pad = kernel.shape[-1] // 2
 
-    gm_x = l2_norm(channel_conv(x, kernel, padding=pad), dims=[1])
-    gm_y = l2_norm(channel_conv(y, kernel, padding=pad), dims=[1])
+    gm_x = l2_norm(channel_conv(x, kernel, padding=pad), dim=1)
+    gm_y = l2_norm(channel_conv(y, kernel, padding=pad), dim=1)
 
     gm_xy = gm_x * gm_y
 
     # Gradient magnitude similarity
-    gms_num = (2. - alpha) * gm_xy + c
-    gms_den = gm_x ** 2 + gm_y ** 2 + c
-
-    if alpha > 0.:
-        gms_den = gms_den - alpha * gm_xy
-
+    gms_num = (2 - alpha) * gm_xy + c
+    gms_den = gm_x ** 2 + gm_y ** 2 - alpha * gm_xy + c
     gms = gms_num / gms_den
 
     # Gradient magnitude similarity deviation
     gmsd = torch.std(gms, dim=(-1, -2))
 
     return gmsd
 
 
-@_jit
+@torch.jit.script_if_tracing
 def ms_gmsd(
     x: Tensor,
     y: Tensor,
     kernel: Tensor,
     weights: Tensor,
-    value_range: float = 1.,
-    c: float = 170. / (255. ** 2),
+    value_range: float = 1.0,
+    c: float = 170 / 255 ** 2,
     alpha: float = 0.5,
 ) -> Tensor:
-    r"""Returns the MS-GMSD between :math:`x` and :math:`y`,
-    without color space conversion.
+    r"""Returns the MS-GMSD between :math:`x` and :math:`y`, without color space
+    conversion.
 
     .. math::
-        \text{MS-GMSD}(x, y) =
-            \sqrt{\sum^{M}_{i = 1} w_i \text{GMSD}(x^i, y^i) ** 2}
+        \text{MS-GMSD}(x, y) = \sqrt{\sum^{M}_{i = 1} w_i \text{GMSD}(x^i, y^i)^2}
 
-    where :math:`x^i` and :math:`y^i` are obtained by downsampling
-    the initial tensors by a factor :math:`2^{i - 1}`.
+    where :math:`x^i` and :math:`y^i` are obtained by downsampling the initial tensors
+    by a factor :math:`2^{i - 1}`.
 
     Args:
         x: An input tensor, :math:`(N, 1, H, W)`.
         y: A target tensor, :math:`(N, 1, H, W)`.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
         weights: The weights :math:`w_i` of the scales, :math:`(M,)`.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Zhang2017]_.
+        For the remaining arguments, refer to Zhang et al. (2017).
 
     Returns:
         The MS-GMSD vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 1, 256, 256)
         >>> y = torch.rand(5, 1, 256, 256)
         >>> kernel = gradient_kernel(prewitt_kernel())
         >>> weights = torch.rand(4)
         >>> l = ms_gmsd(x, y, kernel, weights)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     gmsds = []
 
     for i in range(weights.numel()):
         if i > 0:
             x = F.avg_pool2d(x, kernel_size=2, ceil_mode=True)
             y = F.avg_pool2d(y, kernel_size=2, ceil_mode=True)
 
-        gmsds.append(gmsd(
-            x, y, kernel,
-            value_range=value_range,
-            c=c, alpha=alpha,
-        ))
+        gmsds.append(
+            gmsd(
+                x, y,
+                kernel=kernel,
+                value_range=value_range,
+                c=c,
+                alpha=alpha,
+            )
+        )
 
-    msgmsd = weights * torch.stack(gmsds, dim=-1) ** 2
+    msgmsd = weights * torch.stack(gmsds, dim=-1).square()
     msgmsd = msgmsd.sum(dim=-1).sqrt()
 
     return msgmsd
 
 
 class GMSD(nn.Module):
-    r"""Creates a criterion that measures the GMSD
-    between an input and a target.
+    r"""Measures the GMSD between an input and a target.
 
-    Before applying :func:`gmsd`, the input and target are converted from
-    RBG to Y, the luminance color space, and downsampled by a factor 2.
+    Before applying :func:`gmsd`, the input and target are converted from RBG to Y, the
+    luminance color space, and downsampled by a factor 2.
 
     Args:
         downsample: Whether downsampling is enabled or not.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-            If `None`, use the Prewitt kernel instead.
+            If :py:`None`, use the Prewitt kernel instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-
-    Note:
-        `**kwargs` are passed to :func:`gmsd`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`gmsd`.
 
     Example:
-        >>> criterion = GMSD().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = GMSD()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         downsample: bool = True,
@@ -204,76 +197,77 @@
             kernel = gradient_kernel(prewitt_kernel())
 
         self.register_buffer('kernel', kernel)
 
         self.convert = ColorConv('RGB', 'Y')
         self.downsample = downsample
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The GMSD vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # Downsample
         if self.downsample:
-            input = F.avg_pool2d(input, 2, ceil_mode=True)
-            target = F.avg_pool2d(target, 2, ceil_mode=True)
+            x = F.avg_pool2d(x, 2, ceil_mode=True)
+            y = F.avg_pool2d(y, 2, ceil_mode=True)
 
         # RGB to Y
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # GMSD
-        l = gmsd(input, target, kernel=self.kernel, **self.kwargs)
+        l = gmsd(x, y, kernel=self.kernel, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
 
 
 class MS_GMSD(nn.Module):
-    r"""Creates a criterion that measures the MS-GMSD
-    between an input and a target.
+    r"""Measures the MS-GMSD between an input and a target.
 
     Before applying :func:`ms_gmsd`, the input and target are converted from
     RBG to Y, the luminance color space.
 
     Args:
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-            If `None`, use the Prewitt kernel instead.
+            If :py:`None`, use the Prewitt kernel instead.
         weights: The weights of the scales, :math:`(M,)`.
-            If `None`, use the :const:`MS_GMSD.WEIGHTS` instead.
+            If :py:`None`, use the :const:`MS_GMSD.WEIGHTS` instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`ms_gmsd`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`ms_gmsd`.
 
     Example:
-        >>> criterion = MS_GMSD().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = MS_GMSD()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     WEIGHTS: Tensor = torch.tensor([0.096, 0.596, 0.289, 0.019])
-    r"""Scale weights of [Zhang2017]_."""
+    r"""Scale weights of Zhang et al. (2017)."""
 
     def __init__(
         self,
         kernel: Tensor = None,
         weights: Tensor = None,
         reduction: str = 'mean',
         **kwargs,
@@ -287,33 +281,41 @@
             weights = self.WEIGHTS
 
         self.register_buffer('kernel', kernel)
         self.register_buffer('weights', weights)
 
         self.convert = ColorConv('RGB', 'Y')
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The MS-GMSD vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # RGB to Y
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # MS-GMSD
         l = ms_gmsd(
-            input,
-            target,
+            x, y,
             kernel=self.kernel,
             weights=self.weights,
             **self.kwargs,
         )
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/haarpsi.py` & `piqa-1.3.0/piqa/haarpsi.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,152 +2,145 @@
 
 This module implements the HaarPSI in PyTorch.
 
 Original:
     https://github.com/rgcda/haarpsi
 
 Wikipedia:
-    https://en.wikipedia.org/wiki/Haar_wavelet
+    https://wikipedia.org/wiki/Haar_wavelet
 
 References:
-    .. [Reisenhofer2018] A Haar Wavelet-Based Perceptual Similarity Index for Image Quality Assessment (Reisenhofer et al., 2018)
+    | A Haar Wavelet-Based Perceptual Similarity Index for Image Quality Assessment (Reisenhofer et al., 2018)
+    | https://arxiv.org/abs/1607.06140
 """
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
+from .utils import assert_type
 from .utils.color import ColorConv
 from .utils.functional import (
     haar_kernel,
     gradient_kernel,
     channel_conv,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def haarpsi(
     x: Tensor,
     y: Tensor,
     n_kernels: int = 3,
-    value_range: float = 1.,
-    c: float = 30. / (255. ** 2),
+    value_range: float = 1.0,
+    c: float = 30 / 255 ** 2,
     alpha: float = 4.2,
 ) -> Tensor:
-    r"""Returns the HaarPSI between :math:`x` and :math:`y`,
-    without color space conversion.
+    r"""Returns the HaarPSI between :math:`x` and :math:`y`, without color space
+    conversion.
 
     Args:
         x: An input tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         y: A target tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         n_kernels: The number of Haar wavelet kernels to use.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Reisenhofer2018]_.
+        For the remaining arguments, refer to Reisenhofer et al. (2018).
 
     Returns:
         The HaarPSI vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> l = haarpsi(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     c *= value_range ** 2
 
     # Y
     y_x, y_y = x[:, :1], y[:, :1]
 
-    ## Gradient(s)
-    g_xy: List[Tuple[Tensor, Tensor]] = []
+    ## Gradient similarity(ies)
+    gs = []
 
     for j in range(1, n_kernels + 1):
         kernel_size = int(2 ** j)
 
         ### Haar wavelet kernel
         kernel = gradient_kernel(haar_kernel(kernel_size)).to(x.device)
 
         ### Haar filter (gradient)
         pad = kernel_size // 2
 
         g_x = channel_conv(y_x, kernel, padding=pad)[..., 1:, 1:].abs()
         g_y = channel_conv(y_y, kernel, padding=pad)[..., 1:, 1:].abs()
 
-        g_xy.append((g_x, g_y))
-
-    ## Gradient similarity(ies)
-    gs = []
-    for g_x, g_y in g_xy[:-1]:
-        gs.append((2. * g_x * g_y + c) / (g_x ** 2 + g_y ** 2 + c))
+        if j < n_kernels:
+            gs.append((2 * g_x * g_y + c) / (g_x ** 2 + g_y ** 2 + c))
+        else:
+            gs.append(g_x)
+            gs.append(g_y)
 
     ## Local similarity(ies)
-    ls = torch.stack(gs, dim=-1).sum(dim=-1) / 2.  # (N, 2, H, W)
+    ls = torch.stack(gs[:-2], dim=-1).mean(dim=-1)  # (N, 2, H, W)
 
     ## Weight(s)
-    w = torch.stack(g_xy[-1], dim=-1).max(dim=-1)[0]  # (N, 2, H, W)
+    w = torch.maximum(gs[-2], gs[-1])  # (N, 2, H, W)
 
     # IQ
-    if x.size(1) == 3:
+    if x.shape[1] == 3:
         iq_x, iq_y = x[:, 1:], y[:, 1:]
 
         ## Mean filter
         m_x = F.avg_pool2d(iq_x, 2, stride=1, padding=1)[..., 1:, 1:].abs()
         m_y = F.avg_pool2d(iq_y, 2, stride=1, padding=1)[..., 1:, 1:].abs()
 
         ## Chromatic similarity(ies)
-        cs = (2. * m_x * m_y + c) / (m_x ** 2 + m_y ** 2 + c)
+        cs = (2 * m_x * m_y + c) / (m_x ** 2 + m_y ** 2 + c)
 
         ## Local similarity(ies)
-        ls = torch.cat([ls, cs.mean(1, True)], dim=1)  # (N, 3, H, W)
+        ls = torch.cat((ls, cs.mean(dim=1, keepdim=True)), dim=1)  # (N, 3, H, W)
 
         ## Weight(s)
-        w = torch.cat([w, w.mean(1, True)], dim=1)  # (N, 3, H, W)
+        w = torch.cat((w, w.mean(dim=1, keepdim=True)), dim=1)  # (N, 3, H, W)
 
     # HaarPSI
     hs = torch.sigmoid(ls * alpha)
     hpsi = (hs * w).sum(dim=(-1, -2, -3)) / w.sum(dim=(-1, -2, -3))
     hpsi = (torch.logit(hpsi) / alpha) ** 2
 
     return hpsi
 
 
 class HaarPSI(nn.Module):
-    r"""Creates a criterion that measures the HaarPSI
-    between an input and a target.
+    r"""Measures the HaarPSI between an input and a target.
 
     Before applying :func:`haarpsi`, the input and target are converted from
     RBG to Y(IQ) and downsampled by a factor 2.
 
     Args:
         chromatic: Whether to use the chromatic channels (IQ) or not.
         downsample: Whether downsampling is enabled or not.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`haarpsi`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`haarpsi`.
 
     Example:
-        >>> criterion = HaarPSI().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = HaarPSI()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = 1 - criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         chromatic: bool = True,
@@ -156,32 +149,41 @@
         **kwargs,
     ):
         super().__init__()
 
         self.convert = ColorConv('RGB', 'YIQ' if chromatic else 'Y')
         self.downsample = downsample
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The HaarPSI vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
-            device=self.convert.device,
+            x, y,
+            device=self.convert.weight.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # Downsample
         if self.downsample:
-            input = F.avg_pool2d(input, 2, ceil_mode=True)
-            target = F.avg_pool2d(target, 2, ceil_mode=True)
+            x = F.avg_pool2d(x, 2, ceil_mode=True)
+            y = F.avg_pool2d(y, 2, ceil_mode=True)
 
         # RGB to Y(IQ)
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # HaarPSI
-        l = haarpsi(input, target, **self.kwargs)
+        l = haarpsi(x, y, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/lpips.py` & `piqa-1.3.0/piqa/lpips.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,220 +2,171 @@
 
 This module implements the LPIPS in PyTorch.
 
 Original:
     https://github.com/richzhang/PerceptualSimilarity
 
 References:
-    .. [Zhang2018] The Unreasonable Effectiveness of Deep Features as a Perceptual Metric (Zhang et al., 2018)
-
-    .. [Deng2009] ImageNet: A large-scale hierarchical image database (Deng et al, 2009)
+    | The Unreasonable Effectiveness of Deep Features as a Perceptual Metric (Zhang et al., 2018)
+    | https://arxiv.org/abs/1801.03924
 """
 
-import inspect
-import os
 import torch
 import torch.nn as nn
-import torchvision.models as models
-import torch.hub as hub
+import torchvision
 
 from torch import Tensor
-from typing import Dict, List
+from typing import *
 
-from .utils import _jit, assert_type, reduce_tensor
-from .utils.functional import l2_norm
+from .utils import assert_type
+from .utils.color import ImageNetNorm
+from .utils.functional import l2_norm, reduce_tensor
 
 
 ORIGIN: str = 'https://github.com/richzhang/PerceptualSimilarity'
-SHIFT: Tensor = torch.tensor([0.485, 0.456, 0.406])
-SCALE: Tensor = torch.tensor([0.229, 0.224, 0.225])
 
 
-def get_weights(
-    network: str = 'alex',
-    version: str = 'v0.1',
-) -> Dict[str, Tensor]:
+def get_weights(network: str = 'alex', version: str = 'v0.1') -> List[Tensor]:
     r"""Returns the official LPIPS weights for `network`.
 
     Args:
         network: Specifies the perception network that is used:
-            `'alex'` | `'squeeze'` | `'vgg'`.
+            `'alex'`, `'squeeze'` or `'vgg'`.
         version: Specifies the official version release:
-            `'v0.0'` | `'v0.1'`.
-
-    Example:
-        >>> w = get_weights(network='alex')
-        >>> w.keys()
-        dict_keys(['0.1.weight', '1.1.weight', '2.1.weight', '3.1.weight', '4.1.weight'])
+            `'v0.0'` or `'v0.1'`.
     """
 
-    # Load from URL
-    weights = hub.load_state_dict_from_url(
+    weights = torch.hub.load_state_dict_from_url(
         f'{ORIGIN}/raw/master/lpips/weights/{version}/{network}.pth',
         map_location='cpu',
     )
 
-    # Format keys
-    weights = {
-        k.replace('lin', '').replace('.model', ''): v
-        for (k, v) in weights.items()
-    }
-
-    return weights
+    return [w.flatten() for w in weights.values()]
 
 
-class Intermediary(nn.Module):
-    r"""Module that catches and returns the outputs of indermediate
-    target layers of a sequential module during its forward pass.
+class Perceptual(nn.Module):
+    r"""Perceptual network that intercepts and returns the output of target layers
+    within its foward pass.
 
     Args:
-        layers: A sequential module.
-        targets: A list of target layer indexes.
+        layers: A list of layers.
+        targets: A list of target layer indices.
     """
 
-    def __init__(self, layers: nn.Sequential, targets: List[int]):
+    def __init__(self, layers: List[nn.Module], targets: List[int]):
         super().__init__()
 
-        self.layers = nn.ModuleList()
-        j = 0
-
-        seq: List[nn.Module] = []
+        self.blocks = nn.ModuleList()
 
-        for i, layer in enumerate(layers):
-            seq.append(layer)
+        i = 0
+        for j in targets:
+            self.blocks.append(nn.Sequential(*layers[i : j + 1]))
+            i = j + 1
 
-            if i == targets[j]:
-                self.layers.append(nn.Sequential(*seq))
-                seq.clear()
+    def forward(self, x: Tensor) -> List[Tensor]:
+        y = []
 
-                j += 1
-                if j == len(targets):
-                    break
+        for block in self.blocks:
+            x = block(x)
+            y.append(x)
 
-    def forward(self, input: Tensor) -> List[Tensor]:
-        output = []
-
-        for layer in self.layers:
-            input = layer(input)
-            output.append(input)
-
-        return output
+        return y
 
 
 class LPIPS(nn.Module):
-    r"""Creates a criterion that measures the LPIPS
-    between an input :math:`x` and a target :math:`y`.
+    r"""Measures the LPIPS between an input and a target.
 
     .. math::
         \text{LPIPS}(x, y) = \sum_{l \, \in \, \mathcal{F}}
             w_l \cdot \text{MSE}(\phi_l(x), \phi_l(y))
 
-    where :math:`\phi_l` represents the normalized output of an intermediate
-    layer :math:`l` in a perceptual network :math:`\mathcal{F}`.
-
-    Note:
-        :class:`LPIPS` is a trainable metric. For more details, refer to [Zhang2018]_.
+    where :math:`\phi_l` represents the normalized output of an intermediate layer
+    :math:`l` in a perceptual network :math:`\mathcal{F}` and :math:`w_l` are the
+    official weights of Zhang et al. (2018).
 
     Args:
         network: Specifies the perceptual network :math:`\mathcal{F}` to use:
-            `'alex'` | `'squeeze'` | `'vgg'`.
-        scaling: Whether the input and target need to be scaled w.r.t. [Deng2009]_.
-        dropout: Whether dropout is used or not.
-        pretrained: Whether the official weights :math:`w_l` are used or not.
-        eval: Whether to initialize the object in evaluation mode or not.
+            `'alex'`, `'squeeze'` or `'vgg'`.
+        epsilon: A numerical stability term.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
 
     Example:
-        >>> criterion = LPIPS().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = LPIPS()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         network: str = 'alex',
-        scaling: bool = True,
-        dropout: bool = False,
-        pretrained: bool = True,
-        eval: bool = True,
+        epsilon: float = 1e-10,
         reduction: str = 'mean',
     ):
         super().__init__()
 
-        # ImageNet scaling
-        self.scaling = scaling
-        self.register_buffer('shift', SHIFT.view(1, -1, 1, 1))
-        self.register_buffer('scale', SCALE.view(1, -1, 1, 1))
+        # ImageNet normalization
+        self.normalize = ImageNetNorm()
 
         # Perception layers
         if network == 'alex':  # AlexNet
-            layers = models.alexnet(pretrained=True).features
+            layers = torchvision.models.alexnet(weights='DEFAULT').features
             targets = [1, 4, 7, 9, 11]
-            channels = [64, 192, 384, 256, 256]
         elif network == 'squeeze':  # SqueezeNet
-            layers = models.squeezenet1_1(pretrained=True).features
+            layers = torchvision.models.squeezenet1_1(weights='DEFAULT').features
             targets = [1, 4, 7, 9, 10, 11, 12]
-            channels = [64, 128, 256, 384, 384, 512, 512]
         elif network == 'vgg':  # VGG16
-            layers = models.vgg16(pretrained=True).features
+            layers = torchvision.models.vgg16(weights='DEFAULT').features
             targets = [3, 8, 15, 22, 29]
-            channels = [64, 128, 256, 512, 512]
         else:
-            raise ValueError(f'Unknown network architecture {network}')
-
-        self.net = Intermediary(layers, targets)
-        for p in self.net.parameters():
-            p.requires_grad = False
+            raise ValueError(f"Unknown network architecture {network}")
 
-        # Linear comparators
-        self.lins = nn.ModuleList([
-            nn.Sequential(
-                nn.Dropout(inplace=True) if dropout else nn.Identity(),
-                nn.Conv2d(c, 1, kernel_size=1, bias=False),
-            ) for c in channels
-        ])
+        self.net = Perceptual(list(layers), targets)
+        self.net.eval()
 
-        if pretrained:
-            self.lins.load_state_dict(get_weights(network=network))
+        # Weights
+        self.weights = nn.ParameterList(get_weights(network=network))
 
-        if eval:
-            self.eval()
+        # Disable gradients
+        for p in self.parameters():
+            p.requires_grad = False
 
+        self.epsilon = epsilon
         self.reduction = reduction
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The LPIPS vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
-            device=self.shift.device,
+            x, y,
+            device=self.normalize.shift.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., 1.) if self.scaling else (0., -1.),
+            value_range=(0.0, 1.0),
         )
 
-        # ImageNet scaling
-        if self.scaling:
-            input = (input - self.shift) / self.scale
-            target = (target - self.shift) / self.scale
+        # ImageNet normalization
+        x = self.normalize(x)
+        y = self.normalize(y)
 
         # LPIPS
-        residuals = []
-
-        for lin, fx, fy in zip(self.lins, self.net(input), self.net(target)):
-            fx = fx / l2_norm(fx, dims=[1], keepdim=True)
-            fy = fy / l2_norm(fy, dims=[1], keepdim=True)
+        lpips = 0
 
-            mse = ((fx - fy) ** 2).mean(dim=(-1, -2), keepdim=True)
-            residuals.append(lin(mse).flatten())
+        for w, fx, fy in zip(self.weights, self.net(x), self.net(y)):
+            fx = fx / (l2_norm(fx, dim=1, keepdim=True) + self.epsilon)
+            fy = fy / (l2_norm(fy, dim=1, keepdim=True) + self.epsilon)
 
-        l = torch.stack(residuals, dim=-1).sum(dim=-1)
+            mse = (fx - fy).square().mean(dim=(-1, -2))
+            lpips = lpips + mse @ w
 
-        return reduce_tensor(l, self.reduction)
+        return reduce_tensor(lpips, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/mdsi.py` & `piqa-1.3.0/piqa/mdsi.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,151 +2,145 @@
 
 This module implements the MDSI in PyTorch.
 
 Original:
     https://www.mathworks.com/matlabcentral/fileexchange/59809-mdsi-ref-dist-combmethod
 
 References:
-    .. [Nafchi2016] Mean Deviation Similarity Index: Efficient and Reliable Full-Reference Image Quality Evaluator (Nafchi et al., 2016)
+    | Mean Deviation Similarity Index: Efficient and Reliable Full-Reference Image Quality Evaluator (Nafchi et al., 2016)
+    | https://arxiv.org/abs/1608.07433
 """
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
-from .utils import complex as cx
+from .utils import assert_type
 from .utils.color import ColorConv
 from .utils.functional import (
     prewitt_kernel,
     gradient_kernel,
     channel_conv,
     l2_norm,
+    downsample,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def mdsi(
     x: Tensor,
     y: Tensor,
     kernel: Tensor,
     combination: str = 'sum',
-    value_range: float = 1.,
-    c1: float = 140. / (255. ** 2),
-    c2: float = 55. / (255. ** 2),
-    c3: float = 550. / (255. ** 2),
+    value_range: float = 1.0,
+    c1: float = 140 / 255 ** 2,
+    c2: float = 55 / 255 ** 2,
+    c3: float = 550 / 255 ** 2,
     alpha: float = 0.6,  # 'sum'
     beta: float = 0.1,  # 'prod'
     gamma: float = 0.2,  # 'prod'
-    rho: float = 1.,
+    rho: float = 1.0,
     q: float = 0.25,
     o: float = 0.25,
 ) -> Tensor:
-    r"""Returns the MDSI between :math:`x` and :math:`y`,
-    without downsampling and color space conversion.
+    r"""Returns the MDSI between :math:`x` and :math:`y`, without color space
+    conversion and downsampling.
 
     Args:
         x: An input tensor, :math:`(N, 3, H, W)`.
         y: A target tensor, :math:`(N, 3, H, W)`.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-        combination: Specifies the scheme to combine the gradient
-            and chromaticity similarities (GS, CS): `'sum'` | `'prod'`.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        combination: Specifies the scheme to combine the gradient and chromaticity
+            similarities (GS, CS): `'sum'` or `'prod'`.
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Nafchi2016]_.
+        For the remaining arguments, refer to Nafchi et al. (2016).
 
     Returns:
         The MDSI vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 1, 256, 256)
         >>> y = torch.rand(5, 1, 256, 256)
         >>> kernel = gradient_kernel(prewitt_kernel())
         >>> l = mdsi(x, y, kernel)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     c1 *= value_range ** 2
     c2 *= value_range ** 2
     c3 *= value_range ** 2
 
     l_x, hm_x = x[:, :1], x[:, 1:]
     l_y, hm_y = y[:, :1], y[:, 1:]
 
     # Gradient magnitude
-    pad = kernel.size(-1) // 2
+    pad = kernel.shape[-1] // 2
 
-    gm_x = l2_norm(channel_conv(l_x, kernel, padding=pad), dims=[1])
-    gm_y = l2_norm(channel_conv(l_y, kernel, padding=pad), dims=[1])
-    gm_avg = l2_norm(channel_conv(l_x + l_y, kernel, padding=pad), dims=[1]) / 2
+    gm_x = l2_norm(channel_conv(l_x, kernel, padding=pad), dim=1)
+    gm_y = l2_norm(channel_conv(l_y, kernel, padding=pad), dim=1)
+    gm_avg = l2_norm(channel_conv(l_x + l_y, kernel, padding=pad), dim=1) / 2
 
     gm_x_sq, gm_y_sq, gm_avg_sq = gm_x ** 2, gm_y ** 2, gm_avg ** 2
 
     # Gradient similarity
-    gs_x_y = (2. * gm_x * gm_y + c1) / (gm_x_sq + gm_y_sq + c1)
-    gs_x_avg = (2. * gm_x * gm_avg + c2) / (gm_x_sq + gm_avg_sq + c2)
-    gs_y_avg = (2. * gm_y * gm_avg + c2) / (gm_y_sq + gm_avg_sq + c2)
+    gs_x_y = (2 * gm_x * gm_y + c1) / (gm_x_sq + gm_y_sq + c1)
+    gs_x_avg = (2 * gm_x * gm_avg + c2) / (gm_x_sq + gm_avg_sq + c2)
+    gs_y_avg = (2 * gm_y * gm_avg + c2) / (gm_y_sq + gm_avg_sq + c2)
 
     gs = gs_x_y + gs_x_avg - gs_y_avg
 
     # Chromaticity similarity
-    cs_num = 2. * (hm_x * hm_y).sum(dim=1) + c3
+    cs_num = 2 * (hm_x * hm_y).sum(dim=1) + c3
     cs_den = (hm_x ** 2 + hm_y ** 2).sum(dim=1) + c3
     cs = cs_num / cs_den
 
     # Gradient-chromaticity similarity
-    gs = cx.complx(gs, torch.zeros_like(gs))
-    cs = cx.complx(cs, torch.zeros_like(cs))
+    gs = torch.complex(gs, torch.zeros_like(gs))
+    cs = torch.complex(cs, torch.zeros_like(cs))
 
     if combination == 'prod':
-        gcs = cx.prod(cx.pow(gs, gamma), cx.pow(cs, beta))
+        gcs = gs ** gamma * cs ** beta
     else:  # combination == 'sum'
-        gcs = alpha * gs + (1. - alpha) * cs
+        gcs = alpha * gs + (1 - alpha) * cs
 
     # Mean deviation similarity
-    gcs_q = cx.pow(gcs, q)
+    gcs_q = gcs ** q
     gcs_q_avg = gcs_q.mean(dim=(-2, -3), keepdim=True)
-    score = cx.mod(gcs_q - gcs_q_avg, squared=True) ** (rho / 2)
+    score = (gcs_q - gcs_q_avg).abs() ** rho
     mds = score.mean(dim=(-1, -2)) ** (o / rho)
 
     return mds
 
 
 class MDSI(nn.Module):
-    r"""Creates a criterion that measures the MDSI
-    between an input and a target.
+    r"""Measures the MDSI between an input and a target.
 
-    Before applying :func:`mdsi`, the input and target are converted from
-    RBG to LHM and downsampled by a factor :math:`\frac{\min(H, W)}{256}`.
+    Before applying :func:`mdsi`, the input and target are converted from RBG to LHM and
+    downsampled to a 256-ish resolution.
 
     Args:
         downsample: Whether downsampling is enabled or not.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-            If `None`, use the Prewitt kernel instead.
+            If :py:`None`, use the Prewitt kernel instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`mdsi`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`mdsi`.
 
     Example:
-        >>> criterion = MDSI().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = MDSI()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         downsample: bool = True,
@@ -160,36 +154,41 @@
             kernel = gradient_kernel(prewitt_kernel())
 
         self.register_buffer('kernel', kernel)
 
         self.convert = ColorConv('RGB', 'LHM')
         self.downsample = downsample
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The MDSI vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # Downsample
         if self.downsample:
-            _, _, h, w = input.size()
-            M = round(min(h, w) / 256)
-
-            if M > 1:
-                input = F.avg_pool2d(input, kernel_size=M, ceil_mode=True)
-                target = F.avg_pool2d(target, kernel_size=M, ceil_mode=True)
+            x = downsample(x, 256)
+            y = downsample(y, 256)
 
         # RGB to LHM
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # MDSI
-        l = mdsi(input, target, kernel=self.kernel, **self.kwargs)
+        l = mdsi(x, y, kernel=self.kernel, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/psnr.py` & `piqa-1.3.0/piqa/psnr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 r"""Peak Signal-to-Noise Ratio (PSNR)
 
 This module implements the PSNR in PyTorch.
 
 Wikipedia:
-    https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio
+    https://wikipedia.org/wiki/Peak_signal-to-noise_ratio
 """
 
 import torch
 import torch.nn as nn
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
+from .utils import assert_type
+from .utils.functional import reduce_tensor
 
 
-@_jit
+@torch.jit.script_if_tracing
 def mse(x: Tensor, y: Tensor) -> Tensor:
     r"""Returns the Mean Squared Error (MSE) between :math:`x` and :math:`y`.
 
     .. math::
         \text{MSE}(x, y) = \frac{1}{\text{size}(x)} \sum_i (x_i - y_i)^2
 
     Args:
@@ -28,89 +29,90 @@
     Returns:
         The MSE vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> l = mse(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
-    return ((x - y) ** 2).view(x.size(0), -1).mean(dim=-1)
+    return (x - y).square().reshape(x.shape[0], -1).mean(dim=-1)
 
 
-@_jit
+@torch.jit.script_if_tracing
 def psnr(
     x: Tensor,
     y: Tensor,
     epsilon: float = 1e-8,
-    value_range: float = 1.,
+    value_range: float = 1.0,
 ) -> Tensor:
     r"""Returns the PSNR between :math:`x` and :math:`y`.
 
     .. math::
         \text{PSNR}(x, y) = 10 \log_{10} \left( \frac{L^2}{\text{MSE}(x, y)} \right)
 
     Args:
         x: An input tensor, :math:`(N, *)`.
         y: A target tensor, :math:`(N, *)`.
         epsilon: A numerical stability term.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Returns:
         The PSNR vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> l = psnr(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     return 10 * torch.log10(value_range ** 2 / (mse(x, y) + epsilon))
 
 
 class PSNR(nn.Module):
-    r"""Creates a criterion that measures the PSNR
-    between an input and a target.
+    r"""Measures the PSNR between an input and a target.
 
     Args:
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`psnr`.
-
-    Shapes:
-        input: :math:`(N, *)`
-        target: :math:`(N, *)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`psnr`.
 
     Example:
         >>> criterion = PSNR()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = -criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(self, reduction: str = 'mean', **kwargs):
         super().__init__()
 
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, *)`.
+            y: A target tensor, :math:`(N, *)`.
+
+        Returns:
+            The PSNR vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             dim_range=(1, -1),
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
-        l = psnr(input, target, **self.kwargs)
+        l = psnr(x, y, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/ssim.py` & `piqa-1.3.0/piqa/ssim.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,101 +2,103 @@
 
 This module implements the SSIM and MS-SSIM in PyTorch.
 
 Original:
     https://ece.uwaterloo.ca/~z70wang/research/ssim/
 
 Wikipedia:
-    https://en.wikipedia.org/wiki/Structural_similarity
+    https://wikipedia.org/wiki/Structural_similarity
 
 References:
-    .. [Wang2004a] Image quality assessment: From error visibility to structural similarity (Wang et al., 2004)
+    | Image quality assessment: From error visibility to structural similarity (Wang et al., 2004)
+    | https://ieeexplore.ieee.org/document/1284395
 
-    .. [Wang2004b] Multiscale structural similarity for image quality assessment (Wang et al., 2004)
+    | Multiscale structural similarity for image quality assessment (Wang et al., 2003)
+    | https://ieeexplore.ieee.org/document/1292216
 """
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
-from typing import Tuple
+from typing import *
 
-from .utils import _jit, assert_type, reduce_tensor
+from .utils import assert_type
 from .utils.functional import (
     gaussian_kernel,
     kernel_views,
     channel_convs,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def ssim(
     x: Tensor,
     y: Tensor,
     kernel: Tensor,
     channel_avg: bool = True,
     padding: bool = False,
-    value_range: float = 1.,
+    value_range: float = 1.0,
     k1: float = 0.01,
     k2: float = 0.03,
 ) -> Tuple[Tensor, Tensor]:
-    r"""Returns the SSIM and Contrast Sensitivity (CS) between
-    :math:`x` and :math:`y`.
+    r"""Returns the SSIM and Contrast Sensitivity (CS) between :math:`x` and :math:`y`.
 
     .. math::
-        \text{SSIM}(x, y) &=
+        \text{SSIM}(x, y) & =
             \frac{2 \mu_x \mu_y + C_1}{\mu^2_x + \mu^2_y + C_1} \text{CS}(x, y) \\
-        \text{CS}(x, y) &=
+        \text{CS}(x, y) & =
             \frac{2 \sigma_{xy} + C_2}{\sigma^2_x + \sigma^2_y + C_2}
 
     where :math:`\mu_x`, :math:`\mu_y`, :math:`\sigma^2_x`, :math:`\sigma^2_y` and
-    :math:`\sigma_{xy}` are the results of a smoothing convolution over
-    :math:`x`, :math:`y`, :math:`(x - \mu_x)^2`, :math:`(y - \mu_y)^2` and
-    :math:`(x - \mu_x)(y - \mu_y)`, respectively.
-
-    In practice, SSIM and CS are averaged over the spatial dimensions.
-    If `channel_avg` is `True`, they are also averaged over the channels.
-
-    Note:
-        The number of spatial dimensions is not limited to 2. You can also apply
-        :func:`ssim` (and :class:`SSIM`) on images with 3, or even more, dimensions.
+    :math:`\sigma_{xy}` are the results of a smoothing convolution over :math:`x`,
+    :math:`y`, :math:`(x - \mu_x)^2`, :math:`(y - \mu_y)^2` and :math:`(x - \mu_x)(y -
+    \mu_y)`, respectively.
+
+    In practice, SSIM and CS are averaged over the spatial dimensions. If `channel_avg`
+    is :py:`True`, they are also averaged over the channels.
+
+    Tip:
+        :func:`ssim` and :class:`SSIM` can be applied to images with 1, 2 or even
+        3 spatial dimensions.
 
     Args:
         x: An input tensor, :math:`(N, C, H, *)`.
         y: A target tensor, :math:`(N, C, H, *)`.
         kernel: A smoothing kernel, :math:`(C, 1, K)`.
         channel_avg: Whether to average over the channels or not.
         padding: Whether to pad with :math:`\frac{K}{2}` zeros the spatial
             dimensions or not.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Wang2004a]_.
+        For the remaining arguments, refer to Wang et al. (2004).
 
     Returns:
         The SSIM and CS tensors, both :math:`(N, C)` or :math:`(N,)`
         depending on `channel_avg`.
 
     Example:
         >>> x = torch.rand(5, 3, 64, 64, 64)
         >>> y = torch.rand(5, 3, 64, 64, 64)
         >>> kernel = gaussian_kernel(7).repeat(3, 1, 1)
         >>> ss, cs = ssim(x, y, kernel)
-        >>> ss.size(), cs.size()
+        >>> ss.shape, cs.shape
         (torch.Size([5]), torch.Size([5]))
     """
 
     c1 = (k1 * value_range) ** 2
     c2 = (k2 * value_range) ** 2
 
     window = kernel_views(kernel, x.dim() - 2)
 
     if padding:
-        pad = kernel.size(-1) // 2
+        pad = kernel.shape[-1] // 2
     else:
         pad = 0
 
     # Mean (mu)
     mu_x = channel_convs(x, window, pad)
     mu_y = channel_convs(y, window, pad)
 
@@ -106,122 +108,116 @@
 
     # Variance (sigma)
     sigma_xx = channel_convs(x ** 2, window, pad) - mu_xx
     sigma_yy = channel_convs(y ** 2, window, pad) - mu_yy
     sigma_xy = channel_convs(x * y, window, pad) - mu_xy
 
     # Contrast sensitivity (CS)
-    cs = (2. * sigma_xy + c2) / (sigma_xx + sigma_yy + c2)
+    cs = (2 * sigma_xy + c2) / (sigma_xx + sigma_yy + c2)
 
     # Structural similarity (SSIM)
-    ss = (2. * mu_xy + c1) / (mu_xx + mu_yy + c1) * cs
+    ss = (2 * mu_xy + c1) / (mu_xx + mu_yy + c1) * cs
 
     # Average
     if channel_avg:
         ss, cs = ss.flatten(1), cs.flatten(1)
     else:
         ss, cs = ss.flatten(2), cs.flatten(2)
 
     return ss.mean(dim=-1), cs.mean(dim=-1)
 
 
-@_jit
+@torch.jit.script_if_tracing
 def ms_ssim(
     x: Tensor,
     y: Tensor,
     kernel: Tensor,
     weights: Tensor,
     padding: bool = False,
-    value_range: float = 1.,
+    value_range: float = 1.0,
     k1: float = 0.01,
     k2: float = 0.03,
 ) -> Tensor:
     r"""Returns the MS-SSIM between :math:`x` and :math:`y`.
 
     .. math::
         \text{MS-SSIM}(x, y) = \text{SSIM}(x^M, y^M)^{\gamma_M}
             \prod^{M - 1}_{i = 1} \text{CS}(x^i, y^i)^{\gamma_i}
 
-    where :math:`x^i` and :math:`y^i` are obtained by downsampling
-    the initial tensors by a factor :math:`2^{i - 1}`.
+    where :math:`x^i` and :math:`y^i` are obtained by downsampling the initial tensors
+    by a factor :math:`2^{i - 1}`.
 
     Args:
         x: An input tensor, :math:`(N, C, H, W)`.
         y: A target tensor, :math:`(N, C, H, W)`.
         kernel: A smoothing kernel, :math:`(C, 1, K)`.
         weights: The weights :math:`\gamma_i` of the scales, :math:`(M,)`.
         padding: Whether to pad with :math:`\frac{K}{2}` zeros the spatial
             dimensions or not.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Wang2004b]_.
+        For the remaining arguments, refer to Wang et al. (2003).
 
     Returns:
         The MS-SSIM vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> kernel = gaussian_kernel(7).repeat(3, 1, 1)
         >>> weights = torch.rand(5)
         >>> l = ms_ssim(x, y, kernel, weights)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     css = []
 
     m = weights.numel()
     for i in range(m):
         if i > 0:
             x = F.avg_pool2d(x, kernel_size=2, ceil_mode=True)
             y = F.avg_pool2d(y, kernel_size=2, ceil_mode=True)
 
         ss, cs = ssim(
-            x, y, kernel,
+            x, y,
+            kernel=kernel,
             channel_avg=False,
             padding=padding,
             value_range=value_range,
-            k1=k1, k2=k2,
+            k1=k1,
+            k2=k2,
         )
 
         css.append(torch.relu(cs) if i + 1 < m else torch.relu(ss))
 
     msss = torch.stack(css, dim=-1) ** weights
     msss = msss.prod(dim=-1).mean(dim=-1)
 
     return msss
 
 
 class SSIM(nn.Module):
-    r"""Creates a criterion that measures the SSIM
-    between an input and a target.
+    r"""Measures the SSIM between an input and a target.
 
     Args:
         window_size: The size of the window.
         sigma: The standard deviation of the window.
         n_channels: The number of channels :math:`C`.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`ssim`.
-
-    Shapes:
-        input: :math:`(N, C, H, *)`
-        target: :math:`(N, C, H, *)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`ssim`.
 
     Example:
-        >>> criterion = SSIM().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = SSIM()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = 1 - criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         window_size: int = 11,
@@ -233,64 +229,65 @@
         super().__init__()
 
         kernel = gaussian_kernel(window_size, sigma)
 
         self.register_buffer('kernel', kernel.repeat(n_channels, 1, 1))
 
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, C, H, W)`.
+            y: A target tensor, :math:`(N, C, H, W)`.
+
+        Returns:
+            The SSIM vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(3, 5),
-            n_channels=self.kernel.size(0),
-            value_range=(0., self.value_range),
+            n_channels=self.kernel.shape[0],
+            value_range=(0.0, self.value_range),
         )
 
-        l = ssim(input, target, kernel=self.kernel, **self.kwargs)[0]
+        l = ssim(x, y, kernel=self.kernel, **self.kwargs)[0]
 
         return reduce_tensor(l, self.reduction)
 
 
 class MS_SSIM(nn.Module):
-    r"""Creates a criterion that measures the MS-SSIM
-    between an input and a target.
+    r"""Measures the MS-SSIM between an input and a target.
 
     Args:
         window_size: The size of the window.
         sigma: The standard deviation of the window.
         n_channels: The number of channels :math:`C`.
         weights: The weights of the scales, :math:`(M,)`.
-            If `None`, use :const:`MS_SSIM.WEIGHTS` instead.
+            If :py:`None`, use :const:`MS_SSIM.WEIGHTS` instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`ms_ssim`.
-
-    Shapes:
-        input: :math:`(N, C, H, W)`
-        target: :math:`(N, C, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`ms_ssim`.
 
     Example:
-        >>> criterion = MS_SSIM().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = MS_SSIM()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = 1 - criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     WEIGHTS: Tensor = torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333])
-    r"""Scale weights of [Wang2004b]_."""
+    r"""Scale weights of Wang et al. (2003)."""
 
     def __init__(
         self,
         window_size: int = 11,
         sigma: float = 1.5,
         n_channels: int = 3,
         weights: Tensor = None,
@@ -305,27 +302,36 @@
 
         if weights is None:
             weights = self.WEIGHTS
 
         self.register_buffer('weights', weights)
 
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, C, H, W)`.
+            y: A target tensor, :math:`(N, C, H, W)`.
+
+        Returns:
+            The MS-SSIM vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
-            n_channels=self.kernel.size(0),
-            value_range=(0., self.value_range),
+            n_channels=self.kernel.shape[0],
+            value_range=(0.0, self.value_range),
         )
 
         l = ms_ssim(
-            input, target,
+            x, y,
             kernel=self.kernel,
             weights=self.weights,
             **self.kwargs,
         )
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/tv.py` & `piqa-1.3.0/piqa/tv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 r"""Total Variation (TV)
 
 This module implements the TV in PyTorch.
 
 Wikipedia:
-    https://en.wikipedia.org/wiki/Total_variation
+    https://wikipedia.org/wiki/Total_variation
 """
 
 import torch
 import torch.nn as nn
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
+from .utils import assert_type
+from .utils.functional import reduce_tensor
 
 
-@_jit
+@torch.jit.script_if_tracing
 def tv(x: Tensor, norm: str = 'L1') -> Tensor:
     r"""Returns the TV of :math:`x`.
 
     With `'L1'`,
 
     .. math::
         \text{TV}(x) = \sum_{i, j}
@@ -31,23 +32,23 @@
         \text{TV}(x) = \left( \sum_{c, i, j}
             (x_{c, i+1, j} - x_{c, i, j})^2 +
             (x_{c, i, j+1} - x_{c, i, j})^2 \right)^{\frac{1}{2}}
 
     Args:
         x: An input tensor, :math:`(*, C, H, W)`.
         norm: Specifies the norm funcion to apply:
-            `'L1'` | `'L2'` | `'L2_squared'`.
+            `'L1'`, `'L2'` or `'L2_squared'`.
 
     Returns:
         The TV tensor, :math:`(*,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> l = tv(x)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     w_var = torch.diff(x, dim=-1)
     h_var = torch.diff(x, dim=-2)
 
     if norm == 'L1':
@@ -62,41 +63,43 @@
     if norm == 'L2':
         var = torch.sqrt(var)
 
     return var
 
 
 class TV(nn.Module):
-    r"""Creates a criterion that measures the TV of an input.
+    r"""Measures the TV of an input.
 
     Args:
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`tv`.
-
-    Shapes:
-        input: :math:`(*, C, H, W)`
-        output: :math:`(*,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`tv`.
 
     Example:
         >>> criterion = TV()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
         >>> l = criterion(x)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(self, reduction: str = 'mean', **kwargs):
         super().__init__()
 
         self.reduction = reduction
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor) -> Tensor:
-        assert_type(input, dim_range=(3, -1))
+    def forward(self, x: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, C, H, W)`.
+
+        Returns:
+            The TV vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
+        assert_type(x, dim_range=(4, 4))
 
-        l = tv(input, **self.kwargs)
+        l = tv(x, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

### Comparing `piqa-1.2.2/piqa/utils/__init__.py` & `piqa-1.3.0/piqa/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 r"""Miscellaneous tools and general purpose components"""
 
-import os
 import torch
 
-from torch import Tensor
-from typing import List, Tuple
-
-
-if os.getenv('PIQA_JIT') == '1':
-    _jit = torch.jit.script
-else:
-    _jit = lambda f: f
+from torch import Tensor, Size
+from typing import *
 
 
 __piqa_debug__ = __debug__
 
 def set_debug(mode: bool = False) -> bool:
     r"""Sets and returns whether debugging is enabled or not.
-    If `__debug__` is `False`, this function has not effect.
+    If `__debug__` is :py:`False`, this function has not effect.
 
     Example:
         >>> set_debug(False)
         False
     """
 
     global __piqa_debug__
 
     __piqa_debug__ = __debug__ and mode
 
     return __piqa_debug__
 
 
-def broadcastable(*shapes) -> bool:
+def broadcastable(*shapes: Size) -> bool:
     r"""Returns whether `shapes` are broadcastable.
 
     Example:
         >>> x = torch.rand(3, 2, 1)
         >>> y = torch.rand(1, 2, 3)
         >>> z = torch.rand(2, 2, 2)
         >>> broadcastable(x.shape, y.shape)
@@ -49,73 +42,51 @@
     except RuntimeError as e:
         return False
     else:
         return True
 
 
 def assert_type(
-    *tensors,
+    *tensors: Tensor,
     device: torch.device = None,
     dim_range: Tuple[int, int] = None,
     n_channels: int = None,
     value_range: Tuple[float, float] = None,
 ) -> None:
     r"""Asserts that the types, devices, shapes and values of `tensors` are
     valid with respect to some requirements.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> assert_type(x, y, dim_range=(4, 4), n_channels=3)
     """
 
-    if not __piqa_debug__:
+    if torch.jit.is_tracing() or not __piqa_debug__:
         return
 
     if device is None:
         device = tensors[0].device
 
     shapes = [tuple(t.shape) for t in tensors]
+
     assert broadcastable(*shapes), f"Expected all tensors to have broadcastable shapes, but got {shapes}."
 
     for t in tensors:
         assert t.device == device, f"Expected all tensors to be on the same device, but got {str(t.device)} and {str(device)}."
 
         if dim_range is None:
             pass
         elif dim_range[0] == dim_range[1]:
-            assert t.dim() == dim_range[0], f"Expected number of dimensions to be ' {dim_range[0]}, but got {t.dim()}."
+            assert t.dim() == dim_range[0], f"Expected number of dimensions to be {dim_range[0]}, but got {t.dim()}."
         elif dim_range[0] < dim_range[1]:
             assert dim_range[0] <= t.dim(), f"Expected number of dimensions to be greater or equal to {dim_range[0]}, but got {t.dim()}."
             assert t.dim() <= dim_range[1], f"Expected number of dimensions to be lower or equal to {dim_range[1]}, but got {t.dim()}."
         else:
             assert dim_range[0] <= t.dim(), f"Expected number of dimensions to be greater or equal to {dim_range[0]}, but got {t.dim()}."
 
         if n_channels is not None:
-            assert t.size(1) == n_channels, f"Expected number of channels to be {n_channels}, but got {t.size(1)}."
+            assert t.shape[1] == n_channels, f"Expected number of channels to be {n_channels}, but got {t.shape[1]}."
 
         if value_range is not None:
             assert value_range[0] <= t.min(), f"Expected all values to be greater or equal to {value_range[0]}, but got {t.min().item()}."
             assert t.max() <= value_range[1], f"Expected all values to be lower or equal to {value_range[1]}, but got {t.max().item()}."
-
-
-@_jit
-def reduce_tensor(x: Tensor, reduction: str = 'mean') -> Tensor:
-    r"""Returns the reduction of :math:`x`.
-
-    Args:
-        x: A tensor, :math:`(*,)`.
-        reduction: Specifies the reduction type:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Example:
-        >>> x = torch.arange(5)
-        >>> reduce_tensor(x, reduction='sum')
-        tensor(10)
-    """
-
-    if reduction == 'mean':
-        return x.mean()
-    elif reduction == 'sum':
-        return x.sum()
-
-    return x
```

### Comparing `piqa-1.2.2/piqa/utils/color.py` & `piqa-1.3.0/piqa/utils/color.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,15 @@
 r"""Color space conversion tools"""
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
-from typing import Tuple
-
-
-def spatial(x: Tensor) -> int:
-    r"""Returns the number of spatial dimensions of :math:`x`.
-
-    Args:
-        x: A tensor, :math:`(N, C, *)`.
-    """
-
-    return len(x.shape) - 2
-
-
-def color_conv(
-    x: Tensor,
-    weight: Tensor,
-) -> Tensor:
-    r"""Returns the color convolution of :math:`x` with the kernel `weight`.
-
-    Args:
-        x: A tensor, :math:`(N, C, *)`.
-        weight: A weight kernel, :math:`(C', C)`.
-    """
-
-    return F.linear(x.transpose(1, -1), weight).transpose(1, -1)
+from typing import *
 
 
 RGB_TO_YIQ = torch.tensor([
     [0.299, 0.587, 0.114],
     [0.5969, -0.2746, -0.3213],
     [0.2115, -0.5227, 0.3112],
 ])
@@ -56,91 +32,129 @@
     ('RGB', 'Y'): RGB_TO_YIQ[:1],  # GMSD
     ('RGB', 'LHM'): RGB_TO_LHM,  # MDSI
     ('RGB', 'LMN'): RGB_TO_LMN,  # VSI
     ('RGB', 'L'): RGB_TO_LMN[:1],  # VSI
 }
 
 
+def color_conv(
+    x: Tensor,
+    weight: Tensor,
+    bias: Optional[Tensor] = None,
+) -> Tensor:
+    r"""Returns the color convolution of :math:`x` with the kernel `weight`.
+
+    Args:
+        x: A tensor, :math:`(N, C, *)`.
+        weight: A weight kernel, :math:`(C', C)`.
+        bias: A bias vector, :math:`(C',)`.
+    """
+
+    return F.linear(x.movedim(1, -1), weight, bias).movedim(-1, 1)
+
+
 class ColorConv(nn.Module):
     r"""Color convolution module.
 
     Args:
         src: The source color space (e.g. `'RGB'`).
         dst: The destination color space (e.g. `'YIQ'`).
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> conv = ColorConv('RGB', 'YIQ')
         >>> y = conv(x)
-        >>> y.size()
+        >>> y.shape
         torch.Size([5, 3, 256, 256])
     """
 
     def __init__(self, src: str, dst: str):
         super().__init__()
 
         assert (src, dst) in _WEIGHTS, f"Unknown {src} to {dst} conversion"
 
         self.register_buffer('weight', _WEIGHTS[(src, dst)])
 
-    @property
-    def device(self) -> torch.device:
-        return self.weight.device
-
     def forward(self, x: Tensor) -> Tensor:
         return color_conv(x, self.weight)
 
 
-def rgb_to_xyz(x: Tensor, value_range: float = 1.) -> Tensor:
+def rgb_to_xyz(x: Tensor, value_range: float = 1.0) -> Tensor:
     r"""Converts from sRGB to (CIE) XYZ.
 
     Wikipedia:
-        https://en.wikipedia.org/wiki/SRGB
+        https://wikipedia.org/wiki/SRGB
+
+    Args:
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
     """
 
     x = x / value_range
-
-    mask = x <= 0.04045
-    left = x / 12.92
-    right = ((x + 0.055) / 1.055) ** 2.4
-
-    x = torch.where(mask, left, right)
+    x = torch.where(
+        x <= 0.04045,
+        x / 12.92,
+        ((x + 0.055) / 1.055) ** 2.4,
+    )
 
     weight = torch.tensor([
         [0.4124564, 0.3575761, 0.1804375],
         [0.2126729, 0.7151522, 0.0721750],
         [0.0193339, 0.1191920, 0.9503041],
     ])
 
     return color_conv(x, weight.to(x))
 
 
-def xyz_to_lab(
-    x: Tensor,
-    illuminants: Tuple[float, float, float] = (0.956797052643698, 1., 0.9214805860173273),
-) -> Tensor:
+def xyz_to_lab(x: Tensor) -> Tensor:
     r"""Converts from (CIE) XYZ to (CIE) LAB.
 
     Wikipedia:
-        https://en.wikipedia.org/wiki/CIELAB_color_space
+        https://wikipedia.org/wiki/CIELAB_color_space
     """
 
-    scale = torch.tensor(illuminants).view((3,) + (1,) * spatial(x))
-    x = x / scale.to(x)
-
+    illuminants = torch.tensor([0.964212, 1.0, 0.825188])  # D50
     delta = 6 / 29
 
-    mask = x > delta ** 3
-    left = x ** (1 / 3)
-    right = x / (3 * delta ** 2) + 4 / 29
-
-    x = torch.where(mask, left, right)
+    x = color_conv(x, torch.diag(illuminants.to(x)))
+    x = torch.where(
+        x > delta ** 3,
+        x ** (1 / 3),
+        x / (3 * delta ** 2) + 4 / 29,
+    )
 
     weight = torch.tensor([
-        [0., 116., 0.],
-        [500., -500., 0.],
-        [0., 200., -200.],
+        [0.0, 116.0, 0.0],
+        [500.0, -500.0, 0.0],
+        [0.0, 200.0, -200.0],
     ])
 
-    bias = torch.tensor([-16., 0., 0.]).view(scale.shape)
+    bias = torch.tensor([-16.0, 0.0, 0.0])
 
-    return color_conv(x, weight.to(x)) + bias.to(x)
+    return color_conv(x, weight.to(x), bias.to(x))
+
+
+class ImageNetNorm(nn.Module):
+    r"""Normalizes channels with respect to ImageNet's mean and standard deviation.
+
+    References:
+        | ImageNet: A large-scale hierarchical image database (Deng et al, 2009)
+        | https://ieeexplore.ieee.org/document/5206848
+
+    Example:
+        >>> x = torch.rand(5, 3, 256, 256)
+        >>> normalize = ImageNetNorm()
+        >>> x = normalize(x)
+        >>> x.shape
+        torch.Size([5, 3, 256, 256])
+    """
+
+    MEAN: Tensor = torch.tensor([0.485, 0.456, 0.406])
+    STD: Tensor = torch.tensor([0.229, 0.224, 0.225])
+
+    def __init__(self):
+        super().__init__()
+
+        self.register_buffer('shift', self.MEAN.reshape(3, 1, 1))
+        self.register_buffer('scale', self.STD.reshape(3, 1, 1))
+
+    def forward(self, x: Tensor) -> Tensor:
+        return (x - self.shift) / self.scale
```

### Comparing `piqa-1.2.2/piqa/utils/functional.py` & `piqa-1.3.0/piqa/utils/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 r"""General purpose tensor functionals"""
 
+import math
 import torch
 import torch.fft as fft
-import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
-from typing import List, Tuple, Union
+from typing import *
 
 
 def channel_conv(
     x: Tensor,
     kernel: Tensor,
-    padding: int = 0,  # Union[int, Tuple[int, ...]]
+    padding: int = 0,
 ) -> Tensor:
     r"""Returns the channel-wise convolution of :math:`x` with the kernel `kernel`.
 
     Args:
         x: A tensor, :math:`(N, C, *)`.
         kernel: A kernel, :math:`(C', 1, *)`.
         padding: The implicit paddings on both sides of the input dimensions.
 
     Example:
-        >>> x = torch.arange(25, dtype=torch.float).view(1, 1, 5, 5)
+        >>> x = torch.arange(25).float().reshape(1, 1, 5, 5)
         >>> x
         tensor([[[[ 0.,  1.,  2.,  3.,  4.],
                   [ 5.,  6.,  7.,  8.,  9.],
                   [10., 11., 12., 13., 14.],
                   [15., 16., 17., 18., 19.],
                   [20., 21., 22., 23., 24.]]]])
         >>> kernel = torch.ones((1, 1, 3, 3))
         >>> channel_conv(x, kernel)
         tensor([[[[ 54.,  63.,  72.],
                   [ 99., 108., 117.],
                   [144., 153., 162.]]]])
     """
 
-    D = len(kernel.shape) - 2
+    D = kernel.dim() - 2
 
     assert D <= 3, "PyTorch only supports 1D, 2D or 3D convolutions."
 
     if D == 3:
-        return F.conv3d(x, kernel, padding=padding, groups=x.size(-4))
+        return F.conv3d(x, kernel, padding=padding, groups=x.shape[-4])
     elif D == 2:
-        return F.conv2d(x, kernel, padding=padding, groups=x.size(-3))
+        return F.conv2d(x, kernel, padding=padding, groups=x.shape[-3])
     elif D == 1:
-        return F.conv1d(x, kernel, padding=padding, groups=x.size(-2))
+        return F.conv1d(x, kernel, padding=padding, groups=x.shape[-2])
     else:
-        return F.linear(x, kernel.expand(x.size(-1)))
+        return F.linear(x, kernel.expand(x.shape[-1]))
 
 
 def channel_convs(
     x: Tensor,
     kernels: List[Tensor],
-    padding: int = 0,  # Union[int, Tuple[int, ...]]
+    padding: int = 0,
 ) -> Tensor:
-    r"""Returns the channel-wise convolution of :math:`x` with
-    the series of kernel `kernels`.
+    r"""Returns the channel-wise convolution of :math:`x` with the series of
+    kernel `kernels`.
 
     Args:
         x: A tensor, :math:`(N, C, *)`.
         kernels: A list of kernels, each :math:`(C', 1, *)`.
         padding: The implicit paddings on both sides of the input dimensions.
 
     Example:
-        >>> x = torch.arange(25, dtype=torch.float).view(1, 1, 5, 5)
+        >>> x = torch.arange(25).float().reshape(1, 1, 5, 5)
         >>> x
         tensor([[[[ 0.,  1.,  2.,  3.,  4.],
                   [ 5.,  6.,  7.,  8.,  9.],
                   [10., 11., 12., 13., 14.],
                   [15., 16., 17., 18., 19.],
                   [20., 21., 22., 23., 24.]]]])
         >>> kernels = [torch.ones((1, 1, 3, 1)), torch.ones((1, 1, 1, 3))]
@@ -86,208 +86,207 @@
         x = channel_conv(x, k)
 
     return x
 
 
 def gaussian_kernel(
     size: int,
-    sigma: float = 1.
+    sigma: float = 1.0,
 ) -> Tensor:
     r"""Returns the 1-dimensional Gaussian kernel of size :math:`K`.
 
     .. math::
         G(x) = \gamma \exp \left(\frac{(x - \mu)^2}{2 \sigma^2}\right)
 
     where :math:`\gamma` is such that
 
     .. math:: \sum_{x = 1}^{K} G(x) = 1
 
     and :math:`\mu = \frac{1 + K}{2}`.
 
-    Args:
-        size: The kernel size :math:`K`.
-        sigma: The standard deviation :math:`\sigma` of the distribution.
-
-    Returns:
-        The kernel vector, :math:`(K,)`.
+    Wikipedia:
+        https://wikipedia.org/wiki/Gaussian_blur
 
     Note:
         An :math:`N`-dimensional Gaussian kernel is separable, meaning that
         applying it is equivalent to applying a series of :math:`N` 1-dimensional
         Gaussian kernels, which has a lower computational complexity.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Gaussian_blur
+    Args:
+        size: The kernel size :math:`K`.
+        sigma: The standard deviation :math:`\sigma` of the distribution.
+
+    Returns:
+        The kernel vector, :math:`(K,)`.
 
     Example:
         >>> gaussian_kernel(5, sigma=1.5)
         tensor([0.1201, 0.2339, 0.2921, 0.2339, 0.1201])
     """
 
     kernel = torch.arange(size, dtype=torch.float)
     kernel -= (size - 1) / 2
-    kernel = kernel ** 2 / (2. * sigma ** 2)
+    kernel = kernel ** 2 / (2 * sigma ** 2)
     kernel = torch.exp(-kernel)
     kernel /= kernel.sum()
 
     return kernel
 
 
 def kernel_views(kernel: Tensor, n: int = 2) -> List[Tensor]:
-    r"""Returns the :math:`N`-dimensional views of the 1-dimensional
-    kernel `kernel`.
+    r"""Returns the :math:`N`-dimensional views of the 1-dimensional kernel `kernel`.
 
     Args:
         kernel: A kernel, :math:`(C, 1, K)`.
         n: The number of dimensions :math:`N`.
 
     Returns:
         The list of views, each :math:`(C, 1, \underbrace{1, \dots, 1}_{i}, K, \underbrace{1, \dots, 1}_{N - i - 1})`.
 
     Example:
         >>> kernel = gaussian_kernel(5, sigma=1.5).repeat(3, 1, 1)
-        >>> kernel.size()
+        >>> kernel.shape
         torch.Size([3, 1, 5])
         >>> views = kernel_views(kernel, n=2)
-        >>> views[0].size(), views[1].size()
+        >>> views[0].shape, views[1].shape
         (torch.Size([3, 1, 5, 1]), torch.Size([3, 1, 1, 5]))
     """
 
     if n == 1:
         return [kernel]
     elif n == 2:
         return [kernel.unsqueeze(-1), kernel.unsqueeze(-2)]
 
     # elif n > 2:
-    c, _, k = kernel.size()
+    c, _, k = kernel.shape
 
     shape: List[int] = [c, 1] + [1] * n
     views = []
 
     for i in range(2, n + 2):
         shape[i] = k
-        views.append(kernel.view(shape))
+        views.append(kernel.reshape(shape))
         shape[i] = 1
 
     return views
 
 
 def haar_kernel(size: int) -> Tensor:
     r"""Returns the horizontal Haar kernel.
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Haar_wavelet
+
     Args:
         size: The kernel (even) size :math:`K`.
 
     Returns:
         The kernel, :math:`(K, K)`.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Haar_wavelet
-
     Example:
         >>> haar_kernel(2)
         tensor([[ 0.5000, -0.5000],
                 [ 0.5000, -0.5000]])
     """
 
     return torch.outer(
         torch.ones(size) / size,
-        torch.tensor([1., -1.]).repeat_interleave(size // 2),
+        torch.tensor([1.0, -1.0]).repeat_interleave(size // 2),
     )
 
 
 def prewitt_kernel() -> Tensor:
     r"""Returns the Prewitt kernel.
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Prewitt_operator
+
     Returns:
         The kernel, :math:`(3, 3)`.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Prewitt_operator
-
     Example:
         >>> prewitt_kernel()
         tensor([[ 0.3333,  0.0000, -0.3333],
                 [ 0.3333,  0.0000, -0.3333],
                 [ 0.3333,  0.0000, -0.3333]])
     """
 
     return torch.outer(
-        torch.tensor([1., 1., 1.]) / 3,
-        torch.tensor([1., 0., -1.]),
+        torch.tensor([1.0, 1.0, 1.0]) / 3,
+        torch.tensor([1.0, 0.0, -1.0]),
     )
 
 
 def sobel_kernel() -> Tensor:
     r"""Returns the Sobel kernel.
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Sobel_operator
+
     Returns:
         The kernel, :math:`(3, 3)`.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Sobel_operator
-
     Example:
         >>> sobel_kernel()
         tensor([[ 0.2500,  0.0000, -0.2500],
                 [ 0.5000,  0.0000, -0.5000],
                 [ 0.2500,  0.0000, -0.2500]])
     """
 
     return torch.outer(
-        torch.tensor([1., 2., 1.]) / 4,
-        torch.tensor([1., 0., -1.]),
+        torch.tensor([1.0, 2.0, 1.0]) / 4,
+        torch.tensor([1.0, 0.0, -1.0]),
     )
 
 
 def scharr_kernel() -> Tensor:
     r"""Returns the Scharr kernel.
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Scharr_operator
+
     Returns:
         The kernel, :math:`(3, 3)`.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Scharr_operator
-
     Example:
         >>> scharr_kernel()
         tensor([[ 0.1875,  0.0000, -0.1875],
                 [ 0.6250,  0.0000, -0.6250],
                 [ 0.1875,  0.0000, -0.1875]])
     """
 
     return torch.outer(
-        torch.tensor([3., 10., 3.]) / 16,
-        torch.tensor([1., 0., -1.]),
+        torch.tensor([3.0, 10.0, 3.0]) / 16,
+        torch.tensor([1.0, 0.0, -1.0]),
     )
 
 
 def gradient_kernel(kernel: Tensor) -> Tensor:
     r"""Returns `kernel` transformed into a gradient.
 
     Args:
         kernel: A convolution kernel, :math:`(K, K)`.
 
     Returns:
         The gradient kernel, :math:`(2, 1, K, K)`.
 
     Example:
         >>> g = gradient_kernel(prewitt_kernel())
-        >>> g.size()
+        >>> g.shape
         torch.Size([2, 1, 3, 3])
     """
 
-    return torch.stack([kernel, kernel.t()]).unsqueeze(1)
+    return torch.stack((kernel, kernel.t())).unsqueeze(1)
 
 
 def filter_grid(x: Tensor) -> Tuple[Tensor, Tensor]:
     r"""Returns the (quadrant-shifted) frequency grid for :math:`x`.
 
     Args:
-        x: An input tensor, :math:`(*, H, W)`.
+        x: A tensor, :math:`(*, H, W)`.
 
     Returns:
         The radius and phase tensors, both :math:`(H, W)`.
 
     Example:
         >>> x = torch.rand(5, 5)
         >>> r, phi = filter_grid(x)
@@ -301,83 +300,137 @@
         tensor([[-0.0000, -1.5708, -1.5708,  1.5708,  1.5708],
                 [-0.0000, -0.7854, -1.1071,  1.1071,  0.7854],
                 [-0.0000, -0.4636, -0.7854,  0.7854,  0.4636],
                 [-3.1416, -2.6779, -2.3562,  2.3562,  2.6779],
                 [-3.1416, -2.3562, -2.0344,  2.0344,  2.3562]])
     """
 
-    u, v = [
-        (torch.arange(n).to(x) - n // 2) / (n - n % 2)
-        for n in x.shape[-2:]
-    ]
-    u, v = fft.ifftshift(u[:, None]), fft.ifftshift(v[None, :])
+    H, W = x.shape[-2:]
+
+    u = (torch.arange(H).to(x) - H // 2) / (H - H % 2)
+    v = (torch.arange(W).to(x) - W // 2) / (W - W % 2)
+
+    u = fft.ifftshift(u)[:, None]
+    v = fft.ifftshift(v)[None, :]
 
-    r = (u ** 2 + v ** 2).sqrt()
+    r = torch.sqrt(u ** 2 + v ** 2)
     phi = torch.atan2(-v, u)
 
     return r, phi
 
 
 def log_gabor(f: Tensor, f_0: float, sigma_f: float) -> Tensor:
     r"""Returns the log-Gabor filter of :math:`f`.
 
     .. math::
         G(f) = \exp \left( - \frac{\log(f / f_0)^2}{2 \sigma_f^2} \right)
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Log_Gabor_filter
+
     Args:
         f: A frequency tensor, :math:`(*,)`.
         f_0: The center frequency :math:`f_0`.
         sigma_f: The bandwidth (log-)deviation :math:`\sigma_f`.
 
     Returns:
         The filter tensor, :math:`(*,)`.
 
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Log_Gabor_filter
-
     Example:
         >>> x = torch.rand(5, 5)
         >>> r, phi = filter_grid(x)
-        >>> log_gabor(r, 1., 1.)
+        >>> log_gabor(r, 1.0, 1.0)
         tensor([[0.0000, 0.3825, 0.7864, 0.7864, 0.3825],
                 [0.3825, 0.5825, 0.8444, 0.8444, 0.5825],
                 [0.7864, 0.8444, 0.9417, 0.9417, 0.8444],
                 [0.7864, 0.8444, 0.9417, 0.9417, 0.8444],
                 [0.3825, 0.5825, 0.8444, 0.8444, 0.5825]])
     """
 
-    return torch.exp(- (f / f_0).log() ** 2 / (2 * sigma_f ** 2))
+    return torch.exp(-(f / f_0).log() ** 2 / (2 * sigma_f ** 2))
 
 
 def l2_norm(
     x: torch.Tensor,
-    dims: List[int],
+    dim: int,
     keepdim: bool = False,
 ) -> torch.Tensor:
     r"""Returns the :math:`L_2` norm of :math:`x`.
 
     .. math:
         L_2(x) = \left\| x \right\|_2 = \sqrt{\sum_i x^2_i}
 
+    Wikipedia:
+        https://wikipedia.org/wiki/Norm_(mathematics)
+
     Args:
         x: A tensor, :math:`(*,)`.
-        dims: The dimensions along which to calculate the norm.
-        keepdim: Whether the output tensor has `dims` retained or not.
-
-    Wikipedia:
-        https://en.wikipedia.org/wiki/Norm_(mathematics)
+        dim: The dimension along which to calculate the norm.
+        keepdim: Whether the output tensor has `dim` retained or not.
 
     Example:
-        >>> x = torch.arange(9).float().view(3, 3)
+        >>> x = torch.arange(9).float().reshape(3, 3)
         >>> x
         tensor([[0., 1., 2.],
                 [3., 4., 5.],
                 [6., 7., 8.]])
-        >>> l2_norm(x, dims=[0])
+        >>> l2_norm(x, dim=0)
         tensor([6.7082, 8.1240, 9.6437])
     """
 
-    x = x ** 2
-    x = x.sum(dim=dims, keepdim=keepdim)
+    x = x.square()
+    x = x.sum(dim=dim, keepdim=keepdim)
     x = x.sqrt()
 
     return x
+
+
+@torch.jit.script_if_tracing
+def downsample(x: Tensor, resolution: int = 256):
+    r"""Downsamples :math:`x` to a target resolution.
+
+    Args:
+        x: A tensor, :math:`(N, C, H, W)`.
+        resolution: The target resolution :math:`R`.
+
+    Returns:
+        The downsampled tensor, :math:`(N, C, H / f, W / f)` where :math:`f = \lfloor
+        \frac{\min(H, W)}{R} \rfloor`.
+
+    Example:
+        >>> x = torch.rand(5, 3, 1920, 1080)
+        >>> x = downsample(x, resolution=256)
+        >>> x.shape
+        torch.Size([5, 3, 480, 270])
+    """
+
+    N, C, H, W = x.shape
+
+    factor = math.floor(min(H, W) / resolution)
+
+    if factor > 1:
+        return F.avg_pool2d(x, kernel_size=factor, ceil_mode=True)
+    else:
+        return x
+
+
+@torch.jit.script_if_tracing
+def reduce_tensor(x: Tensor, reduction: str = 'mean') -> Tensor:
+    r"""Returns the reduction of :math:`x`.
+
+    Args:
+        x: A tensor, :math:`(*,)`.
+        reduction: Specifies the reduction type:
+            `'none'`, `'mean'` or `'sum'`.
+
+    Example:
+        >>> x = torch.arange(5)
+        >>> reduce_tensor(x, reduction='sum')
+        tensor(10)
+    """
+
+    if reduction == 'mean':
+        return x.mean()
+    elif reduction == 'sum':
+        return x.sum()
+
+    return x
```

### Comparing `piqa-1.2.2/piqa/vsi.py` & `piqa-1.3.0/piqa/vsi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,196 +1,196 @@
 r"""Visual Saliency-based Index (VSI)
 
 This module implements the VSI in PyTorch.
 
 Original:
-    https://sse.tongji.edu.cn/linzhang/IQA/VSI/VSI.htm
+    https://www.putianjian.net/linzhang/IQA/VSI/VSI.html
 
 Wikipedia:
-    https://en.wikipedia.org/wiki/Salience_(neuroscience)#Visual_saliency_modeling
+    https://wikipedia.org/wiki/Salience_(neuroscience)#Visual_saliency_modeling
 
 References:
-    .. [Zhang2014] VSI: A Visual Saliency-Induced Index for Perceptual Image Quality Assessment (Zhang et al., 2014)
+    | VSI: A Visual Saliency-Induced Index for Perceptual Image Quality Assessment (Zhang et al., 2014)
+    | https://ieeexplore.ieee.org/document/6873260
 
-    .. [Zhang2013] SDSP: A novel saliency detection method by combining simple priors (Zhang et al., 2013)
+    | SDSP: A novel saliency detection method by combining simple priors (Zhang et al., 2013)
+    | https://ieeexplore.ieee.org/document/6738036
 """
 
 import torch
 import torch.fft as fft
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
-from .utils import _jit, assert_type, reduce_tensor
-from .utils import complex as cx
+from .utils import assert_type
 from .utils.color import ColorConv, rgb_to_xyz, xyz_to_lab
 from .utils.functional import (
     scharr_kernel,
     gradient_kernel,
     filter_grid,
     log_gabor,
     channel_conv,
     l2_norm,
+    downsample,
+    reduce_tensor,
 )
 
 
-@_jit
+@torch.jit.script_if_tracing
 def vsi(
     x: Tensor,
     y: Tensor,
     vs_x: Tensor,
     vs_y: Tensor,
     kernel: Tensor,
-    value_range: float = 1.,
+    value_range: float = 1.0,
     c1: float = 1.27,
-    c2: float = 386. / (255. ** 2),
-    c3: float = 130. / (255. ** 2),
+    c2: float = 386 / 255 ** 2,
+    c3: float = 130 / 255 ** 2,
     alpha: float = 0.4,
     beta: float = 0.02,
 ) -> Tensor:
-    r"""Returns the VSI between :math:`x` and :math:`y`,
-    without downsampling and color space conversion.
+    r"""Returns the VSI between :math:`x` and :math:`y`, without color space
+    conversion and downsampling.
 
     Args:
         x: An input tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         y: A target tensor, :math:`(N, 3 \text{ or } 1, H, W)`.
         vs_x: The input visual saliency, :math:`(N, H, W)`.
         vs_y: The target visual saliency, :math:`(N, H, W)`.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-        value_range: The value range :math:`L` of the inputs (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the inputs (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Zhang2014]_.
+        For the remaining arguments, refer to Zhang et al. (2014).
 
     Returns:
         The VSI vector, :math:`(N,)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> y = torch.rand(5, 3, 256, 256)
         >>> filtr = sdsp_filter(x)
         >>> vs_x, vs_y = sdsp(x, filtr), sdsp(y, filtr)
         >>> kernel = gradient_kernel(scharr_kernel())
         >>> l = vsi(x, y, vs_x, vs_y, kernel)
-        >>> l.size()
+        >>> l.shape
         torch.Size([5])
     """
 
     c2 *= value_range ** 2
     c3 *= value_range ** 2
 
     l_x, l_y = x[:, :1], y[:, :1]
 
     # Visual saliency similarity
     vs_m = torch.max(vs_x, vs_y)
     s_vs = (2 * vs_x * vs_y + c1) / (vs_x ** 2 + vs_y ** 2 + c1)
 
     # Gradient magnitude similarity
-    pad = kernel.size(-1) // 2
+    pad = kernel.shape[-1] // 2
 
-    g_x = l2_norm(channel_conv(l_x, kernel, padding=pad), dims=[1])
-    g_y = l2_norm(channel_conv(l_y, kernel, padding=pad), dims=[1])
+    g_x = l2_norm(channel_conv(l_x, kernel, padding=pad), dim=1)
+    g_y = l2_norm(channel_conv(l_y, kernel, padding=pad), dim=1)
 
     s_g = (2 * g_x * g_y + c2) / (g_x ** 2 + g_y ** 2 + c2)
 
     # Chorminance similarity
-    if x.size(1) == 3:
+    if x.shape[1] == 3:
         mn_x, mn_y = x[:, 1:], y[:, 1:]
 
         s_c = (2 * mn_x * mn_y + c3) / (mn_x ** 2 + mn_y ** 2 + c3)
         s_c = s_c.prod(dim=1)
 
-        s_c = cx.complx(s_c, torch.zeros_like(s_c))
-        s_c_beta = cx.real(cx.pow(s_c, beta))
+        s_c = torch.complex(s_c, torch.zeros_like(s_c))
+        s_c_beta = (s_c ** beta).real
 
         s_vs = s_vs * s_c_beta
 
     # Visual Saliency-based Index
     s = s_vs * s_g ** alpha
     vsi = (s * vs_m).sum(dim=(-1, -2)) / vs_m.sum(dim=(-1, -2))
 
     return vsi
 
 
-@_jit
+@torch.jit.script_if_tracing
 def sdsp_filter(
     x: Tensor,
     omega_0: float = 0.021,
     sigma_f: float = 1.34,
 ) -> Tensor:
     r"""Returns the log-Gabor filter for :func:`sdsp`.
 
     Args:
         x: An input tensor, :math:`(*, H, W)`.
 
     Note:
-        For the remaining arguments, refer to [Zhang2013]_.
+        For the remaining arguments, refer to Zhang et al. (2013).
 
     Returns:
         The filter tensor, :math:`(H, W)`.
     """
 
     r, _ = filter_grid(x)
     filtr = log_gabor(r, omega_0, sigma_f)
     filtr = filtr * (r <= 0.5)  # low-pass filter
 
     return filtr
 
 
-@_jit
+@torch.jit.script_if_tracing
 def sdsp(
     x: Tensor,
     filtr: Tensor,
-    value_range: float = 1.,
+    value_range: float = 1.0,
     sigma_c: float = 0.001,
-    sigma_d: float = 145.,
+    sigma_d: float = 145.0,
 ) -> Tensor:
     r"""Detects salient regions from :math:`x`.
 
     Args:
         x: An input tensor, :math:`(N, 3, H, W)`.
         filtr: The frequency domain filter, :math:`(H, W)`.
-        value_range: The value range :math:`L` of the input (usually `1.` or `255`).
+        value_range: The value range :math:`L` of the input (usually 1 or 255).
 
     Note:
-        For the remaining arguments, refer to [Zhang2013]_.
+        For the remaining arguments, refer to Zhang et al. (2013).
 
     Returns:
         The visual saliency tensor, :math:`(N, H, W)`.
 
     Example:
         >>> x = torch.rand(5, 3, 256, 256)
         >>> filtr = sdsp_filter(x)
         >>> vs = sdsp(x, filtr)
-        >>> vs.size()
+        >>> vs.shape
         torch.Size([5, 256, 256])
     """
 
     x_lab = xyz_to_lab(rgb_to_xyz(x, value_range))
 
     # Frequency prior
-    x_f = fft.ifft2(fft.fft2(x_lab) * filtr)
-    x_f = cx.real(torch.view_as_real(x_f))
-
-    s_f = l2_norm(x_f, dims=[1])
+    x_f = fft.ifft2(fft.fft2(x_lab) * filtr).real
+    s_f = l2_norm(x_f, dim=1)
 
     # Color prior
     x_ab = x_lab[:, 1:]
 
-    lo, _ = x_ab.flatten(-2).min(dim=-1)
-    up, _ = x_ab.flatten(-2).max(dim=-1)
+    lo = x_ab.flatten(-2).min(dim=-1).values
+    up = x_ab.flatten(-2).max(dim=-1).values
 
-    lo = lo.view(lo.shape + (1, 1))
-    up = up.view(lo.shape)
-    span = torch.where(up > lo, up - lo, torch.tensor(1.).to(lo))
+    lo = lo.reshape(lo.shape + (1, 1))
+    up = up.reshape(lo.shape)
 
-    x_ab = (x_ab - lo) / span
+    x_ab = (x_ab - lo) / (up - lo + 1e-8)
 
-    s_c = 1. - torch.exp(-torch.sum(x_ab ** 2, dim=1) / sigma_c ** 2)
+    s_c = 1 - torch.exp(-x_ab.square().sum(dim=1) / sigma_c ** 2)
 
     # Location prior
     a, b = [
         torch.arange(n).to(x) - (n - 1) / 2
         for n in x.shape[-2:]
     ]
 
@@ -199,44 +199,36 @@
     # Visual saliency
     vs = s_f * s_c * s_d
 
     return vs
 
 
 class VSI(nn.Module):
-    r"""Creates a criterion that measures the VSI
-    between an input and a target.
+    r"""Measures the VSI between an input and a target.
 
-    Before applying :func:`vsi`, the input and target are converted from
-    RBG to L(MN) and downsampled by a factor :math:`\frac{\min(H, W)}{256}`.
+    Before applying :func:`vsi`, the input and target are converted from RBG to L(MN)
+    and downsampled to a 256-ish resolution.
 
     The visual saliency maps of the input and target are determined by :func:`sdsp`.
 
     Args:
         chromatic: Whether to use the chromatic channels (MN) or not.
         downsample: Whether downsampling is enabled or not.
         kernel: A gradient kernel, :math:`(2, 1, K, K)`.
-            If `None`, use the Scharr kernel instead.
+            If :py:`None`, use the Scharr kernel instead.
         reduction: Specifies the reduction to apply to the output:
-            `'none'` | `'mean'` | `'sum'`.
-
-    Note:
-        `**kwargs` are passed to :func:`vsi`.
-
-    Shapes:
-        input: :math:`(N, 3, H, W)`
-        target: :math:`(N, 3, H, W)`
-        output: :math:`(N,)` or :math:`()` depending on `reduction`
+            `'none'`, `'mean'` or `'sum'`.
+        kwargs: Keyword arguments passed to :func:`vsi`.
 
     Example:
-        >>> criterion = VSI().cuda()
-        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True).cuda()
-        >>> y = torch.rand(5, 3, 256, 256).cuda()
+        >>> criterion = VSI()
+        >>> x = torch.rand(5, 3, 256, 256, requires_grad=True)
+        >>> y = torch.rand(5, 3, 256, 256)
         >>> l = 1 - criterion(x, y)
-        >>> l.size()
+        >>> l.shape
         torch.Size([])
         >>> l.backward()
     """
 
     def __init__(
         self,
         chromatic: bool = True,
@@ -247,48 +239,51 @@
     ):
         super().__init__()
 
         if kernel is None:
             kernel = gradient_kernel(scharr_kernel())
 
         self.register_buffer('kernel', kernel)
-        self.register_buffer('filter', torch.zeros((0, 0)))
 
         self.convert = ColorConv('RGB', 'LMN' if chromatic else 'L')
         self.downsample = downsample
         self.reduction = reduction
-        self.value_range = kwargs.get('value_range', 1.)
+        self.value_range = kwargs.get('value_range', 1.0)
         self.kwargs = kwargs
 
-    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        r"""
+        Args:
+            x: An input tensor, :math:`(N, 3, H, W)`.
+            y: A target tensor, :math:`(N, 3, H, W)`.
+
+        Returns:
+            The VSI vector, :math:`(N,)` or :math:`()` depending on `reduction`.
+        """
+
         assert_type(
-            input, target,
+            x, y,
             device=self.kernel.device,
             dim_range=(4, 4),
             n_channels=3,
-            value_range=(0., self.value_range),
+            value_range=(0.0, self.value_range),
         )
 
         # Downsample
         if self.downsample:
-            _, _, h, w = input.size()
-            M = round(min(h, w) / 256)
-
-            if M > 1:
-                input = F.avg_pool2d(input, kernel_size=M, ceil_mode=True)
-                target = F.avg_pool2d(target, kernel_size=M, ceil_mode=True)
+            x = downsample(x, 256)
+            y = downsample(y, 256)
 
         # Visual saliency
-        if self.filter.shape != input.shape[-2:]:
-            self.filter = sdsp_filter(input)
+        filtr = sdsp_filter(x)
 
-        vs_input = sdsp(input, self.filter, self.value_range)
-        vs_target = sdsp(target, self.filter, self.value_range)
+        vs_x = sdsp(x, filtr, self.value_range)
+        vs_y = sdsp(y, filtr, self.value_range)
 
         # RGB to L(MN)
-        input = self.convert(input)
-        target = self.convert(target)
+        x = self.convert(x)
+        y = self.convert(y)
 
         # VSI
-        l = vsi(input, target, vs_input, vs_target, kernel=self.kernel, **self.kwargs)
+        l = vsi(x, y, vs_x, vs_y, kernel=self.kernel, **self.kwargs)
 
         return reduce_tensor(l, self.reduction)
```

