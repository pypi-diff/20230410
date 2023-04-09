# Comparing `tmp/texturize-0.8.0.tar.gz` & `tmp/texturize-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texturize-0.8.0.tar", last modified: Fri Jun 26 14:10:07 2020, max compression
+gzip compressed data, was "texturize-0.9.0.tar", last modified: Sat Jul  4 11:02:07 2020, max compression
```

## Comparing `texturize-0.8.0.tar` & `texturize-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0    35181 2020-06-09 18:00:29.438988 texturize-0.8.0/LICENSE
--rw-r--r--   0        0        0      884 2020-06-26 14:06:13.955106 texturize-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3550 2020-06-26 14:04:28.084754 texturize-0.8.0/README.rst
--rw-r--r--   0        0        0      113 2020-06-26 14:06:08.325032 texturize-0.8.0/src/texturize/__init__.py
--rw-r--r--   0        0        0     4960 2020-06-17 18:28:09.879251 texturize-0.8.0/src/texturize/__main__.py
--rw-r--r--   0        0        0     8664 2020-06-26 14:04:56.963196 texturize-0.8.0/src/texturize/api.py
--rw-r--r--   0        0        0     2468 2020-06-25 21:21:34.704275 texturize-0.8.0/src/texturize/app.py
--rw-r--r--   0        0        0     5359 2020-06-26 12:44:18.438860 texturize-0.8.0/src/texturize/critics.py
--rw-r--r--   0        0        0     6179 2020-06-26 13:31:36.642845 texturize-0.8.0/src/texturize/io.py
--rw-r--r--   0        0        0    16730 2020-06-26 10:46:26.054896 texturize-0.8.0/src/texturize/match.py
--rw-r--r--   0        0        0     1217 2020-06-15 16:52:21.338632 texturize-0.8.0/src/texturize/patch.py
--rw-r--r--   0        0        0     6003 2020-06-25 21:45:11.074613 texturize-0.8.0/src/texturize/solvers.py
--rw-r--r--   0        0        0     4545 2020-06-26 14:10:07.864638 texturize-0.8.0/setup.py
--rw-r--r--   0        0        0     4429 2020-06-26 14:10:07.864638 texturize-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35181 2020-06-09 18:00:29.438988 texturize-0.9.0/LICENSE
+-rw-r--r--   0        0        0      880 2020-07-04 11:00:59.801999 texturize-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6007 2020-06-29 11:32:29.672802 texturize-0.9.0/README.rst
+-rw-r--r--   0        0        0      113 2020-07-04 11:00:48.884059 texturize-0.9.0/src/texturize/__init__.py
+-rw-r--r--   0        0        0     5754 2020-07-04 09:54:44.826602 texturize-0.9.0/src/texturize/__main__.py
+-rw-r--r--   0        0        0     2854 2020-07-03 16:06:34.438262 texturize-0.9.0/src/texturize/api.py
+-rw-r--r--   0        0        0     4032 2020-07-03 10:27:02.591353 texturize-0.9.0/src/texturize/app.py
+-rw-r--r--   0        0        0     3454 2020-07-04 09:27:27.633666 texturize-0.9.0/src/texturize/commands.py
+-rw-r--r--   0        0        0     5359 2020-07-02 17:00:19.242435 texturize-0.9.0/src/texturize/critics.py
+-rw-r--r--   0        0        0     6221 2020-07-02 19:21:51.056753 texturize-0.9.0/src/texturize/io.py
+-rw-r--r--   0        0        0     3206 2020-07-02 18:11:51.665000 texturize-0.9.0/src/texturize/logger.py
+-rw-r--r--   0        0        0    16730 2020-06-26 10:46:26.054896 texturize-0.9.0/src/texturize/match.py
+-rw-r--r--   0        0        0     1217 2020-06-15 16:52:21.338632 texturize-0.9.0/src/texturize/patch.py
+-rw-r--r--   0        0        0     6003 2020-07-02 20:42:35.572475 texturize-0.9.0/src/texturize/solvers.py
+-rw-r--r--   0        0        0     7004 2020-07-04 11:02:07.753767 texturize-0.9.0/setup.py
+-rw-r--r--   0        0        0     6819 2020-07-04 11:02:07.755766 texturize-0.9.0/PKG-INFO
```

### Comparing `texturize-0.8.0/LICENSE` & `texturize-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texturize-0.8.0/pyproject.toml` & `texturize-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "texturize"
 description = "🤖🖌️ Automatically generate new textures similar to a source photograph."
-version = "0.8.0"
+version = "0.9.0"
 authors = ["Alex J. Champandard <445208+alexjc@users.noreply.github.com>"]
 readme = "README.rst"
 repository = "https://github.com/photogeniq/neural-texturize"
 license = "AGPL-3.0"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Topic :: Multimedia :: Graphics",
 ]
 packages = [
     { include = "texturize", from = "src" },
 ]
 
 [tool.poetry.scripts]
```

### Comparing `texturize-0.8.0/src/texturize/__main__.py` & `texturize-0.9.0/src/texturize/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 r"""                         _   _            _              _         
   _ __   ___ _   _ _ __ __ _| | | |_ _____  _| |_ _   _ _ __(_)_______ 
  | '_ \ / _ \ | | | '__/ _` | | | __/ _ \ \/ / __| | | | '__| |_  / _ \
  | | | |  __/ |_| | | | (_| | | | ||  __/>  <| |_| |_| | |  | |/ /  __/
  |_| |_|\___|\__,_|_|  \__,_|_|  \__\___/_/\_\\__|\__,_|_|  |_/___\___|
 
 Usage:
-    texturize SOURCE... [--size=WxH] [--output=FILE] [--variations=V] [--seed=SEED]
-                        [--mode=MODE] [--octaves=O] [--threshold=H] [--iterations=I]
-                        [--device=DEVICE] [--precision=PRECISION] [--quiet] [--verbose]
+    texturize remix SOURCE... [options]
+    texturize remake TARGET like SOURCE [options]
     texturize --help
 
 Examples:
-    texturize samples/grass.webp --size=1440x960 --output=result.png
-    texturize samples/gravel.png --iterations=200 --precision=1e-5
-    texturize samples/sand.tiff  --output=tmp/{source}-{octave}.webp
-    texturize samples/brick.jpg  --device=cpu
+    texturize remix samples/grass.webp --size=1440x960 --output=result.png
+    texturize remix samples/gravel.png --iterations=200 --precision=1e-5
+    texturize remix samples/sand.tiff  --output=tmp/{source}-{octave}.webp
+    texturize remix samples/brick.jpg  --device=cpu
 
 Options:
     SOURCE                  Path to source image to use as texture.
     -s WxH, --size=WxH      Output resolution as WIDTHxHEIGHT. [default: 640x480]
     -o FILE, --output=FILE  Filename for saving the result, includes format variables.
                             [default: {source}_gen{variation}.png]
     --variations=V          Number of images to generate at same time. [default: 1]
@@ -39,35 +38,37 @@
 #
 # neural-texturize is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Affero General Public License version 3. This program is distributed
 # in the hope that it will be useful but WITHOUT ANY WARRANTY; without even the implied
 # warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 #
 
+import os
 import glob
 import itertools
 
 import docopt
-import progressbar
 from schema import Schema, Use, And, Or
 
 import torch
 
 from . import __version__
-from .api import process_single_file, ansi, ConsoleLog
+from . import api, io, commands
+from .logger import ansi, ConsoleLog
 
 
 def validate(config):
     # Determine the shape of output tensor (H, W) from specified resolution.
     def split_size(size: str):
         return tuple(map(int, size.split("x")))
 
     sch = Schema(
         {
             "SOURCE": [str],
+            "TARGET": Or(None, str),
             "size": And(Use(split_size), tuple),
             "output": str,
             "variations": Use(int),
             "seed": Or(None, Use(int)),
             "mode": Or("patch", "gram", "hist"),
             "octaves": Use(int),
             "threshold": Use(float),
@@ -82,38 +83,59 @@
     )
     return sch.validate({k.replace("--", ""): v for k, v in config.items()})
 
 
 def main():
     # Parse the command-line options based on the script's documentation.
     config = docopt.docopt(__doc__[356:], version=__version__, help=False)
+    command = [cmd for cmd in ("remix", "remake") if config[cmd]][0]
+
     # Ensure the user-specified values are correct.
     config = validate(config)
-    filenames, seed, quiet, verbose, help = [
-        config.pop(k) for k in ("SOURCE", "seed", "quiet", "verbose", "help")
+    sources, target, output, seed, mode = [
+        config.pop(k) for k in ("SOURCE", "TARGET", "output", "seed", "mode")
     ]
 
     # Setup the output logging and display the logo!
-    log = ConsoleLog(quiet, verbose)
+    log = ConsoleLog(config.pop("quiet"), config.pop("verbose"))
     log.notice(ansi.PINK + "    " + __doc__[:356] + ansi.ENDC)
-    if help is True:
+    if config.pop("help") is True:
         log.notice(__doc__[356:])
         return
 
     # Scan all the files based on the patterns specified.
-    files = itertools.chain.from_iterable(glob.glob(s) for s in filenames)
+    files = itertools.chain.from_iterable(glob.glob(s) for s in sources)
     for filename in files:
         # If there's a random seed, use the same for all images.
         if seed is not None:
             torch.manual_seed(seed)
             torch.cuda.manual_seed(seed)
 
+        source_img = io.load_image_from_file(filename)
+        target_img = io.load_image_from_file(target) if target else None
+
+        if command == "remix":
+            cmd = commands.Remix(source_img, mode=mode)
+        if command == "remake":
+            cmd = commands.Remake(source_img, target_img, mode=mode)
+            config["octaves"] = 1
+            config["size"] = target_img.size
+
         # Process the files one by one, each may have multiple variations.
         try:
-            result = process_single_file(filename, log, **config)
+            config["output"] = output
+            config["output"] = config["output"].replace(
+                "{source}", os.path.splitext(os.path.basename(filename))[0]
+            )
+            if target:
+                config["output"] = config["output"].replace(
+                    "{target}", os.path.splitext(os.path.basename(target))[0]
+                )
+
+            result = api.process_single_command(cmd, log, **config)
             log.notice(ansi.PINK + "\n=> result:", result, ansi.ENDC)
         except KeyboardInterrupt:
             print(ansi.PINK + "\nCTRL+C detected, interrupting..." + ansi.ENDC)
             break
 
 
 if __name__ == "__main__":
```

### Comparing `texturize-0.8.0/src/texturize/app.py` & `texturize-0.9.0/src/texturize/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,88 @@
 # neural-texturize — Copyright (c) 2020, Novelty Factory KG.  See LICENSE for details.
 
 import os
 
 import torch
 import torch.nn.functional as F
-
 from creativeai.image.encoders import models
 
-from .critics import GramMatrixCritic, PatchCritic
-from .solvers import SolverLBFGS, MultiCriticObjective
+from .critics import GramMatrixCritic, PatchCritic, HistogramCritic
+from .app import TextureSynthesizer, Application, Result
 from .io import *
 
 
-class TextureSynthesizer:
-    def __init__(self, device, encoder, lr, threshold, max_iter):
-        self.device = device
-        self.encoder = encoder
-        self.threshold = threshold
-        self.max_iter = max_iter
-        self.learning_rate = lr
-
-    def prepare(self, critics, image):
-        """Extract the features from the source texture and initialize the critics.
-        """
-        feats = dict(self.encoder.extract(image, [c.get_layers() for c in critics]))
-        for critic in critics:
-            critic.from_features(feats)
-
-    def run(self, log, seed_img, critics):
-        """Run the optimizer on the image according to the loss returned by the critics.
-        """
-        image = seed_img.to(self.device).requires_grad_(True)
-
-        obj = MultiCriticObjective(self.encoder, critics)
-        opt = SolverLBFGS(obj, image, lr=self.learning_rate)
-
-        progress = log.create_progress_bar(self.max_iter)
-
-        try:
-            for i, loss, lr, retries in self._iterate(opt):
-                # Constrain the image to the valid color range.
-                image.data.clamp_(0.0, 1.0)
-
-                # Update the progress bar with the result!
-                progress.update(i, loss=loss)
-
-                # Return back to the user...
-                yield loss, image, lr, retries
-
-            progress.max_value = i + 1
-        finally:
-            progress.finish()
-
-    def _iterate(self, opt):
-        previous, plateau = float("+inf"), 0
-        for i in range(self.max_iter):
-            # Perform one step of the optimization.
-            loss, scores, progress = opt.step()
-
-            if not progress:
-                continue
-
-            # Return this iteration to the caller...
-            yield i, loss, opt.lr, opt.retries
-
-            # See if we can terminate the optimization early.
-            if i > 10 and abs(loss - previous) <= self.threshold:
-                plateau += 1
-                if plateau > 2:
-                    break
-            else:
-                plateau = 0
+@torch.no_grad()
+def process_iterations(
+    cmd,
+    log: object = None,
+    size: tuple = None,
+    octaves: int = -1,
+    variations: int = 1,
+    iterations: int = 200,
+    threshold: float = 1e-5,
+    device: str = None,
+    precision: str = None,
+):
+    """Synthesize a new texture and return a PyTorch tensor at each iteration.
+    """
+
+    # Setup the application to use throughout the synthesis.
+    app = Application(log, device, precision)
+
+    # Encoder used by all the critics at every octave.
+    encoder = models.VGG11(pretrained=True, pool_type=torch.nn.AvgPool2d)
+    encoder = encoder.to(device=app.device, dtype=app.precision)
+    app.encoder = encoder
+
+    # Coarse-to-fine rendering, number of octaves specified by user.
+    seed = None
+    for octave, scale in enumerate(2 ** s for s in range(octaves - 1, -1, -1)):
+        app.log.info(f"\n OCTAVE #{octave} ")
+        app.log.debug("<- scale:", f"1/{scale}")
+
+        critics = cmd.prepare_critics(app, scale)
+
+        result_size = (variations, 3, size[1] // scale, size[0] // scale)
+        seed = cmd.prepare_seed_tensor(app, result_size, previous=seed)
+        app.log.debug("<- seed:", tuple(seed.shape[2:]), "\n")
+
+        for result in app.process_octave(
+            seed,
+            app.encoder,
+            critics,
+            octave,
+            scale,
+            threshold=threshold,
+            iterations=iterations,
+        ):
+            yield result
+
+        seed = result.images
+        del result
+
+
+@torch.no_grad()
+def process_octaves(cmd, **kwargs):
+    """Synthesize a new texture from sources and return a PyTorch tensor at each octave.
+    """
+    for r in process_iterations(cmd, **kwargs):
+        if r.iteration >= 0:
+            continue
+
+        yield Result(
+            r.images, r.octave, r.scale, -r.iteration, r.loss, r.rate, r.retries
+        )
+
+
+def process_single_command(cmd, log: object, output: str = None, **config: dict):
+    for result in process_octaves(cmd, log=log, **config):
+        images = save_tensor_to_images(result.images)
+        filenames = []
+        for i, image in enumerate(images):
+            # Save the files for each octave to disk.
+            filename = output.format(octave=result.octave, variation=i,)
+            image.resize(size=config["size"], resample=0).save(filename)
+            log.debug("\n=> output:", filename)
+            filenames.append(filename)
 
-            previous = min(loss, previous)
+    return filenames
```

### Comparing `texturize-0.8.0/src/texturize/critics.py` & `texturize-0.9.0/src/texturize/critics.py`

 * *Files identical despite different names*

### Comparing `texturize-0.8.0/src/texturize/io.py` & `texturize-0.9.0/src/texturize/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import time
 import random
 import urllib
 import asyncio
 from io import BytesIO
 
 import PIL.Image
+import torch
 import torchvision.transforms.functional as V
 
 
 def load_tensor_from_file(filename, device, mode="RGB"):
     image = load_image_from_file(filename, mode)
     return load_tensor_from_image(image, device)
 
 
 def load_image_from_file(filename, mode="RGB"):
     return PIL.Image.open(filename).convert(mode)
 
 
-def load_tensor_from_image(image, device):
-    return V.to_tensor(image).unsqueeze(0).to(device)
+def load_tensor_from_image(image, device, dtype=torch.float32):
+    return V.to_tensor(image).unsqueeze(0).to(device, dtype)
 
 
 def load_image_from_url(url, mode="RGB"):
     response = urllib.request.urlopen(url)
     buffer = BytesIO(response.read())
     return PIL.Image.open(buffer).convert(mode)
```

### Comparing `texturize-0.8.0/src/texturize/match.py` & `texturize-0.9.0/src/texturize/match.py`

 * *Files identical despite different names*

### Comparing `texturize-0.8.0/src/texturize/patch.py` & `texturize-0.9.0/src/texturize/patch.py`

 * *Files identical despite different names*

### Comparing `texturize-0.8.0/src/texturize/solvers.py` & `texturize-0.9.0/src/texturize/solvers.py`

 * *Files identical despite different names*

