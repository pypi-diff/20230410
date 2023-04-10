# Comparing `tmp/zerodose-0.0.5.tar.gz` & `tmp/zerodose-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerodose-0.0.5.tar", max compression
+gzip compressed data, was "zerodose-0.0.6.tar", max compression
```

## Comparing `zerodose-0.0.5.tar` & `zerodose-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-04-04 13:19:34.890469 zerodose-0.0.5/LICENSE
--rw-r--r--   0        0        0     2132 2023-04-04 13:19:34.890469 zerodose-0.0.5/README.md
--rw-r--r--   0        0        0     1941 2023-04-04 13:19:47.966524 zerodose-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       16 2023-04-04 13:19:34.894469 zerodose-0.0.5/src/zerodose/__init__.py
--rw-r--r--   0        0        0     7315 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/__main__.py
--rw-r--r--   0        0        0     1642 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/dataset.py
--rw-r--r--   0        0        0     1935 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/inference.py
--rw-r--r--   0        0        0     2856 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/models.py
--rw-r--r--   0        0        0     4703 2023-04-04 13:19:34.894469 zerodose-0.0.5/src/zerodose/networks.py
--rw-r--r--   0        0        0      480 2023-04-04 13:19:34.894469 zerodose-0.0.5/src/zerodose/paths.py
--rw-r--r--   0        0        0      411 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/abnormality.py
--rw-r--r--   0        0        0     4392 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/full.py
--rw-r--r--   0        0        0     2740 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/niftyreg.py
--rw-r--r--   0        0        0     1895 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/normalization.py
--rw-r--r--   0        0        0     2135 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/pipeline/synthetization.py
--rw-r--r--   0        0        0     3132 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/processing.py
--rw-r--r--   0        0        0        0 2023-04-04 13:19:34.894469 zerodose-0.0.5/src/zerodose/py.typed
--rw-r--r--   0        0        0     7965 2023-04-04 13:19:47.966524 zerodose-0.0.5/src/zerodose/utils.py
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 zerodose-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-10 08:06:31.736736 zerodose-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2132 2023-04-10 08:06:31.736736 zerodose-0.0.6/README.md
+-rw-r--r--   0        0        0     2113 2023-04-10 08:06:46.652793 zerodose-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/__init__.py
+-rw-r--r--   0        0        0     7370 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/__main__.py
+-rw-r--r--   0        0        0     1523 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/dataset.py
+-rw-r--r--   0        0        0     2240 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/inference.py
+-rw-r--r--   0        0        0     3247 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/models.py
+-rw-r--r--   0        0        0     4703 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/networks.py
+-rw-r--r--   0        0        0      480 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/paths.py
+-rw-r--r--   0        0        0      470 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/pipeline/__init__.py
+-rw-r--r--   0        0        0     1954 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/pipeline/abnormality.py
+-rw-r--r--   0        0        0     2298 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/pipeline/full.py
+-rw-r--r--   0        0        0     3044 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/pipeline/main.py
+-rw-r--r--   0        0        0     3854 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/pipeline/niftyreg.py
+-rw-r--r--   0        0        0     1895 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/pipeline/normalization.py
+-rw-r--r--   0        0        0     2137 2023-04-10 08:06:46.652793 zerodose-0.0.6/src/zerodose/pipeline/synthetization.py
+-rw-r--r--   0        0        0     3132 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/processing.py
+-rw-r--r--   0        0        0        0 2023-04-10 08:06:31.740736 zerodose-0.0.6/src/zerodose/py.typed
+-rw-r--r--   0        0        0     8509 2023-04-10 08:06:46.656792 zerodose-0.0.6/src/zerodose/utils.py
+-rw-r--r--   0        0        0    11366 2023-04-10 08:06:46.656792 zerodose-0.0.6/src/zerodose/visualizations.py
+-rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 zerodose-0.0.6/PKG-INFO
```

### Comparing `zerodose-0.0.5/LICENSE` & `zerodose-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/README.md` & `zerodose-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/pyproject.toml` & `zerodose-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zerodose"
-version = "0.0.5"
+version = "0.0.6"
 description = "Zerodose"
 authors = ["Christian Hinge <christian.hinge@regionh.dk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ChristianHinge/zerodose"
 repository = "https://github.com/ChristianHinge/zerodose"
 documentation = "https://zerodose.readthedocs.io"
@@ -17,14 +17,19 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 click = ">=8.0.1"
 torch = ">=1.0.0"
 torchio = "^0.18.0"
 niftyreg = "^1.5.70rc1"
+matplotlib = {version = "^3.7.1", optional = true}
+opencv-python = {version = "^4.7.0.72", optional = true}
+
+[tool.poetry.extras]
+plotting = ["matplotlib","opencv-python"]
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `zerodose-0.0.5/src/zerodose/__main__.py` & `zerodose-0.0.6/src/zerodose/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Sequence
 from typing import Union
 
 import click
 
 from zerodose.pipeline import create_abnormality_maps
 from zerodose.pipeline import normalize_to_pet
-from zerodose.pipeline import run_full
+from zerodose.pipeline import run_with_registration
 from zerodose.pipeline import synthesize_baselines
 from zerodose.utils import _create_output_fname
 
 
 @click.group()
 @click.version_option()
 def main() -> None:
@@ -304,63 +304,66 @@
     "--no-img",
     "no_image",
     is_flag=True,
     default=False,
     help="Print verbose output.",
 )
 
+no_reg_pet_to_mr_option = click.option(
+    "--no-pet-rigid",
+    "no_reg_pet_to_mr",
+    is_flag=True,
+    default=False,
+    help="Print verbose output.",
+)
+
 
 @mri_option_single
 @mask_option_single
 @pet_option_single
 @sbpet_output_option_single
 @abn_output_option_single
 @img_output_option_single
-@no_registration_option
-@no_abnormality_option
-@no_normalization_option
+@no_reg_pet_to_mr_option
 @no_image_option
 @verbose_option
 @device_option
 @outputspace_option
 @main.command()
-def run(
+def pipeline(
     mri_fname,
     mask_fname,
     pet_fname,
     out_sbpet,
     out_abn,
     out_img,
-    no_registration,
-    no_abnormality,
-    no_normalization,
+    no_reg_pet_to_mr,
     no_image,
     verbose,
     device,
     outputspace,
 ):
     """Run full pipeline."""
-    do_registration = not no_registration
-    do_abnormality = not no_abnormality
-    do_normalization = not no_normalization
+    reg_pet_to_mr = not no_reg_pet_to_mr
     do_image = not no_image
 
     if out_sbpet is None:
         out_sbpet = _create_output_fname(pet_fname, suffix="_sb")
     if out_abn is None:
         out_abn = _create_output_fname(pet_fname, suffix="_abn")
+    if out_img is None and do_image:
+        out_img = _create_output_fname(
+            pet_fname, suffix="_abn_figure", file_type=".png"
+        )
 
-    run_full(
+    run_with_registration(
         mri_fname=mri_fname,
         mask_fname=mask_fname,
         out_sbpet=out_sbpet,
         pet_fname=pet_fname,
         out_abn=out_abn,
         out_img=out_img,
-        do_registration=do_registration,
-        do_abnormality=do_abnormality,
-        do_normalization=do_normalization,
-        do_image=do_image,
+        reg_pet_to_mri=reg_pet_to_mr,
         verbose=verbose,
         device=device,
         outputspace=outputspace,
     )
```

### Comparing `zerodose-0.0.5/src/zerodose/dataset.py` & `zerodose-0.0.6/src/zerodose/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,41 +8,36 @@
 from zerodose.processing import PadAndCropMNI
 from zerodose.processing import ToFloat32
 
 
 class SubjectDataset(tio.data.SubjectsDataset):
     """Dataset class for the ZeroDose project."""
 
-    def __init__(self, mri_fnames, mask_fnames, out_fnames):
+    def __init__(self, mri_fnames, mask_fnames, pet_fnames=None):
         """Initialize the dataset."""
         transforms = self._get_augmentation_transform_val()
 
         subjects = [
-            self._make_subject_predict(mr_f, ma_f, ou_f)
-            for mr_f, ma_f, ou_f in zip(  # noqa
+            self._make_subject_predict(mr_f, ma_f)
+            for mr_f, ma_f in zip(  # noqa
                 mri_fnames,
                 mask_fnames,
-                out_fnames,
             )
         ]
-        super().__init__(subjects, transforms)
-
-    def _make_subject_dict(self, mr_path, mask_path) -> dict:
-        subject_dict: Dict[Any, Any] = {}
-        mri = mr_path
-        mask = mask_path
 
-        subject_dict["mr"] = tio.ScalarImage(mri)
-        subject_dict["mask"] = tio.LabelMap(mask)
+        if pet_fnames is not None:
+            for sub, pet_fname in zip(subjects, pet_fnames):  # noqa
+                sub.add_image(tio.ScalarImage(pet_fname), "pet")
 
-        return subject_dict
+        super().__init__(subjects, transforms)
 
-    def _make_subject_predict(self, mr_path, mask_path, out_fname) -> tio.Subject:
-        subject_dict = self._make_subject_dict(mr_path, mask_path)
-        subject_dict["out_fname"] = out_fname
+    def _make_subject_predict(self, mr_path, mask_path) -> tio.Subject:
+        subject_dict: Dict[Any, Any] = {}
+        subject_dict["mr"] = tio.ScalarImage(mr_path)
+        subject_dict["mask"] = tio.LabelMap(mask_path)
         return tio.Subject(subject_dict)
 
     def _get_augmentation_transform_val(self) -> tio.Compose:
         augmentations = [
             Binarize(include=["mask"]),
             tio.transforms.ZNormalization(include=["mr"], masking_method="mask"),
             PadAndCropMNI(),
```

### Comparing `zerodose-0.0.5/src/zerodose/inference.py` & `zerodose-0.0.6/src/zerodose/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,19 @@
     stride = (2,)
 
     sbpet_tensor = _infer_single_subject(
         model, sub, patch_size, patch_overlap, batch_size, sd_weight, device
     )
 
     return sbpet_tensor
+
+
+def get_inference_params():
+    """Returns the default parameters for inference stitching."""
+    stride = 2
+    params = {
+        "patch_size": (32, 192, 192),
+        "patch_overlap": (32 - stride, 192 - stride, 192 - stride),
+        "batch_size": 1,
+        "sd_weight": 5,
+    }
+    return params
```

### Comparing `zerodose-0.0.5/src/zerodose/networks.py` & `zerodose-0.0.6/src/zerodose/networks.py`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/src/zerodose/pipeline/abnormality.py` & `zerodose-0.0.6/src/zerodose/pipeline/abnormality.py`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/src/zerodose/pipeline/niftyreg.py` & `zerodose-0.0.6/src/zerodose/pipeline/niftyreg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 """Niftyreg wrapper for torchio."""
+import os
 import tempfile
 
 import niftyreg  # type: ignore
 import numpy as np
 
-from zerodose.utils import binarize
 from zerodose.utils import get_mni_template
 
 
+def _rigid_pet_to_ref(pet_path, ref_path):
+    with tempfile.TemporaryDirectory() as tempdir:
+        out_rigid = os.path.join(tempdir, "rigid.txt")
+        out_temp = os.path.join(tempdir, "out.nii.gz")
+        niftyreg.main(
+            [
+                "aladin",
+                "-flo",
+                pet_path,
+                "-ref",
+                ref_path,
+                "-res",
+                out_temp,
+                "-aff",
+                out_rigid,
+                "-voff",
+                "-rigOnly",
+            ],
+        )
+        mat_rig = _read_matrix_nifty(out_rigid)
+        return mat_rig
+
+
 def from_mni(
     ref_fname,
     in_affine_fname,
     float_fname,
     out_fname,
 ):
     """Resample a floating image to a reference image using an affine matrix."""
@@ -41,49 +64,74 @@
     in_mri_fname,
     in_mask_fname,
     in_pet_fname,
     out_mri_fname,
     out_mask_fname,
     out_pet_fname,
     out_affine_fname,
+    reg_pet_to_mri=True,
 ):
     """Resample a floating image to a reference image using an affine matrix."""
-    ref = get_mni_template()
+    ref = get_mni_template("mask")
+
     niftyreg.main(
         [
             "aladin",
             "-flo",
-            in_mri_fname,
+            in_mask_fname,
             "-ref",
             ref,
             "-res",
-            out_mri_fname,
+            out_mask_fname,
             "-aff",
             out_affine_fname,
             "-speeeeed",
             "-voff",
         ],
     )
+
     in_affine = out_affine_fname
+
     niftyreg.main(
         [
             "resample",
             "-ref",
             ref,
             "-flo",
             in_mask_fname,
             "-res",
             out_mask_fname,
             "-aff",
             in_affine,
+            "-inter",
+            "0",
+        ]
+    )
+
+    niftyreg.main(
+        [
+            "resample",
+            "-ref",
+            ref,
+            "-flo",
+            in_mri_fname,
+            "-res",
+            out_mri_fname,
+            "-aff",
+            in_affine,
             "-voff",
         ]
     )
 
-    binarize(out_mask_fname, out_mask_fname)
+    if reg_pet_to_mri and in_pet_fname is not None:
+        mat_rig = _rigid_pet_to_ref(in_pet_fname, in_mri_fname)
+        mat_aff = _read_matrix_nifty(in_affine)
+        mat_aff = mat_rig @ mat_aff
+        _save_matrix_nifty(mat_aff, in_affine)
+
     if in_pet_fname is not None:
         niftyreg.main(
             [
                 "resample",
                 "-ref",
                 ref,
                 "-flo",
```

### Comparing `zerodose-0.0.5/src/zerodose/pipeline/normalization.py` & `zerodose-0.0.6/src/zerodose/pipeline/normalization.py`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/src/zerodose/pipeline/synthetization.py` & `zerodose-0.0.6/src/zerodose/pipeline/synthetization.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         raise Exception(
             """The number of input files {} mask files {}
             and output files {} must be identical""".format(
                 len(mri_fnames), len(mask_fnames), len(out_fnames)
             )
         )
 
-    dataset = SubjectDataset(mri_fnames, mask_fnames, out_fnames)
+    dataset = SubjectDataset(mri_fnames, mask_fnames)
     model = utils.get_model()
 
     model = model.to(device)
     model.eval()
     patch_size = (32, 192, 192)
     patch_overlap = (32 - stride, 192 - stride, 192 - stride)
 
-    for sub in dataset:  # type: ignore
+    for i, sub in enumerate(dataset):  # type: ignore
         if verbose:
             print(f"Synthesizing sbPET for {sub.mr.path}")
 
         sbpet_tensor = _infer_single_subject(
             model, sub, patch_size, patch_overlap, batch_size, sd_weight, device
         )
 
@@ -64,9 +64,9 @@
 
         sub.add_image(sbpet_img, "sbpet")
         sub.remove_image("mr")
         sub = inverse_transform(sub)
 
         if save_output:
             if verbose:
-                print(f"Saving to {sub.out_fname}")
-            sub["sbpet"].save(sub.out_fname)
+                print(f"Saving to {out_fnames[i]}")
+            sub["sbpet"].save(out_fnames[i])
```

### Comparing `zerodose-0.0.5/src/zerodose/processing.py` & `zerodose-0.0.6/src/zerodose/processing.py`

 * *Files identical despite different names*

### Comparing `zerodose-0.0.5/src/zerodose/utils.py` & `zerodose-0.0.6/src/zerodose/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,40 +6,72 @@
 import tempfile
 from typing import List
 from typing import Literal
 from typing import Tuple
 from typing import Union
 from urllib.request import urlopen
 
-import nibabel as nib
+import nibabel as nib  # type: ignore
 import torch
 import torch.nn as nn
 from torch.nn import functional
 
 from zerodose.models import ZeroDose
 from zerodose.paths import folder_with_parameter_files
 from zerodose.paths import folder_with_templates
 
 
+def save_nifty(data: torch.Tensor, filename_out: str, affine_ref: str) -> None:
+    """Saves a nifty file."""
+    save_directory = os.path.dirname(filename_out)
+    if not os.path.exists(save_directory):
+        os.makedirs(save_directory)
+
+    func = nib.load(affine_ref).affine  # type: ignore
+    data_npy = data.squeeze().cpu().detach().numpy()
+    ni_img = nib.Nifti1Image(data_npy, func)
+    nib.save(ni_img, filename_out)
+
+
+def load_nifty(fname: str) -> torch.Tensor:
+    """Loads a nifty file and returns it as a torch tensor."""
+    return torch.from_numpy(nib.load(fname).get_fdata()).float()  # type: ignore
+
+
+def get_mni_template(img="mr") -> str:
+    """Returns the path to the t1 MNI template. If missing, downloads the template."""
+    if os.environ.get("GITHUB_ACTIONS"):
+        raise Exception(
+            """MNI templates should not be downloaded
+            when running GitHub Actions"""
+        )
+    else:
+        _maybe_download_mni_template()
+        return _get_mni_template_fname(img=img)
+
+
 def binarize(img_path, out_path, threshold=0.5):
     """Binarize an image."""
     img = nib.load(img_path)
     data = img.get_fdata()
     data[data > threshold] = 1
     img = nib.Nifti1Image(data, img.affine, img.header)
     nib.save(img, out_path)
 
 
 def _get_model_fname() -> str:
     """Returns the path to the parameter file for the given fold."""
     return os.path.join(folder_with_parameter_files, "model_1.pt")
 
 
-def _get_mni_template_fname():
-    return os.path.join(folder_with_templates, "t1.nii")
+def _get_mni_template_fname(img="mr"):
+    if img == "mr":
+        return os.path.join(folder_with_templates, "t1.nii")
+    elif img == "mask":
+        return os.path.join(folder_with_templates, "mask.nii")
 
 
 def _download_file(url: str, filename: str) -> None:
     data = urlopen(url).read()  # noqa
     with open(filename, "wb") as f:
         f.write(data)
 
@@ -70,20 +102,24 @@
 
 def _maybe_download_mni_template(
     force_overwrite: bool = False, verbose: bool = True
 ) -> None:
     if not os.path.isdir(folder_with_templates):
         _maybe_mkdir_p(folder_with_templates)
 
-    out_filename = _get_mni_template_fname()
+    out_mri = _get_mni_template_fname(img="mr")
+    out_mask = _get_mni_template_fname(img="mask")
 
-    if force_overwrite and os.path.isfile(out_filename):
-        os.remove(out_filename)
+    if force_overwrite and os.path.isfile(out_mri):
+        os.remove(out_mri)
 
-    if not os.path.isfile(out_filename):
+    if force_overwrite and os.path.isfile(out_mri):
+        os.remove(out_mask)
+
+    if not os.path.isfile(out_mri) or not os.path.isfile(out_mask):
         with tempfile.TemporaryDirectory() as tempdirname:
             url = (
                 "https://www.bic.mni.mcgill.ca/~vfonov/icbm/"
                 "2009/mni_icbm152_nlin_sym_09a_nifti.zip"
             )
             filename = os.path.join(tempdirname, "mni_icbm152_nlin_sym_09a_nifti.zip")
             if verbose:
@@ -93,15 +129,21 @@
                 print("Unpacking MNI template", url, "...")
             shutil.unpack_archive(filename, tempdirname)
             t1 = os.path.join(
                 tempdirname,
                 "mni_icbm152_nlin_sym_09a",
                 "mni_icbm152_t1_tal_nlin_sym_09a.nii",
             )
-            shutil.copy(t1, out_filename)
+            mask = os.path.join(
+                tempdirname,
+                "mni_icbm152_nlin_sym_09a",
+                "mni_icbm152_t1_tal_nlin_sym_09a_mask.nii",
+            )
+            shutil.copy(t1, out_mri)
+            shutil.copy(mask, out_mask)
 
 
 def _maybe_mkdir_p(directory: str) -> None:
     """Creates a directory if it does not exist yet."""
     if not os.path.exists(directory):
         os.makedirs(directory)
 
@@ -178,43 +220,14 @@
     )
     gaussian_vec = gaussian_vec.unsqueeze(1).unsqueeze(1)
     weight = torch.ones(ps)
     weight *= gaussian_vec
     return weight.unsqueeze(0).unsqueeze(0)
 
 
-def save_nifty(data: torch.Tensor, filename_out: str, affine_ref: str) -> None:
-    """Saves a nifty file."""
-    save_directory = os.path.dirname(filename_out)
-    if not os.path.exists(save_directory):
-        os.makedirs(save_directory)
-
-    func = nib.load(affine_ref).affine
-    data = data.squeeze().cpu().detach().numpy()
-    ni_img = nib.Nifti1Image(data, func)
-    nib.save(ni_img, filename_out)
-
-
-def load_nifty(fname: str) -> torch.Tensor:
-    """Loads a nifty file and returns it as a torch tensor."""
-    return torch.from_numpy(nib.load(fname).get_fdata()).float()
-
-
-def get_mni_template() -> str:
-    """Returns the path to the t1 MNI template. If missing, downloads the template."""
-    if os.environ.get("GITHUB_ACTIONS"):
-        raise Exception(
-            """MNI templates may not be downloaded by
-            pytests that do not have a 'slow' marker"""
-        )
-    else:
-        _maybe_download_mni_template()
-        return _get_mni_template_fname()
-
-
 def get_model(
     model_type: Literal["standard", "dummy", "determine"] = "determine"
 ) -> ZeroDose:
     """Returns the ZeroDose model and loads the parameters."""
     if model_type == "determine":
         if os.environ.get("ZERODOSE_USE_DUMMY_MODEL"):
             model_type = "dummy"
```

### Comparing `zerodose-0.0.5/PKG-INFO` & `zerodose-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: zerodose
-Version: 0.0.5
+Version: 0.0.6
 Summary: Zerodose
 Home-page: https://github.com/ChristianHinge/zerodose
 License: MIT
 Author: Christian Hinge
 Author-email: christian.hinge@regionh.dk
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: plotting
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "plotting"
 Requires-Dist: niftyreg (>=1.5.70rc1,<2.0.0)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0) ; extra == "plotting"
 Requires-Dist: torch (>=1.0.0)
 Requires-Dist: torchio (>=0.18.0,<0.19.0)
 Project-URL: Changelog, https://github.com/ChristianHinge/zerodose/releases
 Project-URL: Documentation, https://zerodose.readthedocs.io
 Project-URL: Repository, https://github.com/ChristianHinge/zerodose
 Description-Content-Type: text/markdown
```

