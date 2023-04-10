# Comparing `tmp/lifeomic_patient_ml_types-7.2.1.tar.gz` & `tmp/lifeomic_patient_ml_types-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.2.1.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.3.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.2.1.tar` & `lifeomic_patient_ml_types-7.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13031 2023-04-05 18:41:36.544912 lifeomic_patient_ml_types-7.2.1/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-04-05 18:42:55.972662 lifeomic_patient_ml_types-7.2.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.2.1/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.2.1/PKG-INFO
+-rw-r--r--   0        0        0    13999 2023-04-10 13:04:24.063575 lifeomic_patient_ml_types-7.3.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-04-10 13:05:47.262969 lifeomic_patient_ml_types-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.3.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.3.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.2.1/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.3.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,60 @@
     labelDefinition: LabelsDefinitionInput
 
 
 class ClassificationProblem(MlProblemDefinitionBase):
     labelDefinition: LabelsDefinition
 
 
+class ImageSegmentationArea(BaseModel):
+    """
+    A run-length encoded (RLE) 4 channel color image, representing the mask for a single label.
+    """
+
+    class Config:
+        extra = Extra.forbid
+
+    id: str
+    """
+    The ID of the label this mask is for.
+    """
+    rle: List[int]
+    """
+    The run-length encoded mask; an array of 8-bit unsigned integers.
+    """
+
+
+class ImageSegmentationLabelData(BaseModel):
+    """
+    A raw image segmentation, in the format LabelStudio provides.
+    """
+
+    class Config:
+        extra = Extra.forbid
+
+    labelType: Literal["imgSeg"]
+    projectId: str
+    """
+    The ID of the LifeOmic project the label file is saved under.
+    """
+    height: int
+    """
+    The height of the segmentation mask in pixels.
+    """
+    width: int
+    """
+    The width of the segmentation mask in pixels.
+    """
+    areas: List[ImageSegmentationArea]
+
+
+class LabelFileData(BaseModel):
+    __root__: ImageSegmentationLabelData
+
+
 class LabelBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     isConfirmed: Optional[bool] = None
     """
     A confirmed label is believed to be correct and may be used during training and evaluation.
```

### Comparing `lifeomic_patient_ml_types-7.2.1/pyproject.toml` & `lifeomic_patient_ml_types-7.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.2.1"
+version = "7.3.0"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

