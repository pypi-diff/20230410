# Comparing `tmp/formkit_ninja-0.1.6a9.tar.gz` & `tmp/formkit_ninja-0.1.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.1.6a9.tar", max compression
+gzip compressed data, was "formkit_ninja-0.1.7a1.tar", max compression
```

## Comparing `formkit_ninja-0.1.6a9.tar` & `formkit_ninja-0.1.7a1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      813 2023-01-12 08:15:06.575969 formkit_ninja-0.1.6a9/README.md
--rw-r--r--   0        0        0        0 2023-01-12 08:07:03.327754 formkit_ninja-0.1.6a9/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-01-12 08:07:03.327754 formkit_ninja-0.1.6a9/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    13076 2023-01-17 16:21:09.217069 formkit_ninja-0.1.6a9/formkit_ninja/admin.py
--rw-r--r--   0        0        0     1171 2023-01-12 08:07:03.327754 formkit_ninja-0.1.6a9/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-01-12 08:12:59.487316 formkit_ninja-0.1.6a9/formkit_ninja/fields.py
--rw-r--r--   0        0        0    12965 2023-03-15 14:10:18.572029 formkit_ninja-0.1.6a9/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-01-12 08:07:03.327754 formkit_ninja-0.1.6a9/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     1962 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     8369 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0     1947 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0002_remove_formkitschemanode_children_and_more.py
--rw-r--r--   0        0        0     1477 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0003_alter_formcomponents_options_formkitschemanode_group_and_more.py
--rw-r--r--   0        0        0     2276 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0004_alter_formkitschemanode_group_nodechildren_and_more.py
--rw-r--r--   0        0        0      878 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0005_delete_schemacondition_and_more.py
--rw-r--r--   0        0        0      468 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0006_formkitschemanode_placeholder.py
--rw-r--r--   0        0        0      610 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0007_alter_formcomponents_options_and_more.py
--rw-r--r--   0        0        0      732 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/0008_rename_new_values_formkitschemanode_node_and_more.py
--rw-r--r--   0        0        0        0 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0    10728 2023-03-15 14:10:18.572029 formkit_ninja-0.1.6a9/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-01-12 08:07:03.328754 formkit_ninja-0.1.6a9/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1035 2023-03-22 04:20:56.997224 formkit_ninja-0.1.6a9/pyproject.toml
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 formkit_ninja-0.1.6a9/setup.py
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.1.6a9/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.1.7a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.1.7a1/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    12921 2023-04-10 00:27:29.051854 formkit_ninja-0.1.7a1/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     1511 2023-04-10 00:27:28.771846 formkit_ninja-0.1.7a1/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.1.7a1/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    13135 2023-04-10 00:27:29.083855 formkit_ninja-0.1.7a1/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.1.7a1/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     8369 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1947 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0002_remove_formkitschemanode_children_and_more.py
+-rw-r--r--   0        0        0     1477 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0003_alter_formcomponents_options_formkitschemanode_group_and_more.py
+-rw-r--r--   0        0        0     2276 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0004_alter_formkitschemanode_group_nodechildren_and_more.py
+-rw-r--r--   0        0        0      878 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0005_delete_schemacondition_and_more.py
+-rw-r--r--   0        0        0      468 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0006_formkitschemanode_placeholder.py
+-rw-r--r--   0        0        0      610 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0007_alter_formcomponents_options_and_more.py
+-rw-r--r--   0        0        0      732 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/0008_rename_new_values_formkitschemanode_node_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0    10539 2023-04-10 00:01:32.869811 formkit_ninja-0.1.7a1/formkit_ninja/models.py
+-rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.1.7a1/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1201 2023-04-10 00:27:59.308716 formkit_ninja-0.1.7a1/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.1.7a1/PKG-INFO
```

### Comparing `formkit_ninja-0.1.6a9/README.md` & `formkit_ninja-0.1.7a1/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/admin.py` & `formkit_ninja-0.1.7a1/formkit_ninja/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,22 +144,19 @@
         """
         Updates the JSON field(s) from the fields specified in the `_json_fields` dict
         """
 
         for field, keys in self._json_fields.items():
             # Populate a JSON field in a model named "form"
             # from a set of standard form elements
-            data = getattr(self.instance, field, {})
-            if not isinstance(data, dict):
-                # This is a bit unexpected
-                raise ValueError("Expected a JSON dict object here")
-            logger.debug(data)
-            data.update({key: self.cleaned_data[key] for key in keys})
-            logger.debug(data)
-            setattr(self.instance, field, data)
+            data = {}
+            for key in keys:
+                if cleaned_data := self.cleaned_data[key]:
+                    data[key] = cleaned_data
+        setattr(self.instance, field, data)
         return super().save(commit=commit)
 
 
 class NewFormKitForm(forms.ModelForm):
     class Meta:
         model = models.FormKitSchemaNode
         fields = ("node_type", "description")
@@ -336,14 +333,17 @@
     class Meta:
         model = models.FormKitSchema
         exclude = ("name",)
 
 
 @admin.register(models.FormKitSchemaNode)
 class FormKitSchemaNodeAdmin(OrderedInlineModelAdminMixin, admin.ModelAdmin):
+
+    list_display = ["id", "label", "node_type"]
+
     def get_inlines(self, request, obj: models.FormKitSchemaNode | None):
 
         if not obj:
             return []
 
         formkit_node_type = (obj.node or {}).get("formkit", None)
 
@@ -385,35 +385,35 @@
         change: None = None,
         **kwargs,
     ):
         if not obj:
             return NewFormKitForm
 
         try:
-            node_type: FORMKIT_TYPE = obj.node.get("node_type")
+            node_type: FORMKIT_TYPE = obj.node_type
         except (AttributeError, KeyError) as E:
             warnings.warn("Expected a 'Node' with a 'NodeType' in the admin form")
             warnings.warn(f"{E}")
 
         if node_type == "condition":
             return FormKitConditionForm
 
-        elif node_type == "formkit":
+        elif node_type == "$formkit":
             formkit_node_type = (obj.node or {}).get("formkit", None)
             if formkit_node_type == "group":
                 return enlangished_class(FormKitNodeGroupForm)
             return enlangished_class(FormKitNodeForm)
 
-        elif node_type == "el":
+        elif node_type == "$el":
             return enlangished_class(FormKitElementForm)
 
         elif node_type == "text":
             return enlangished_class(FormKitTextNode)
 
-        elif node_type == "component":
+        elif node_type == "$cmp":
             return enlangished_class(FormKitComponentForm)
 
         else:
             return super().get_form(request, obj, change, **kwargs)
 
 
 @admin.register(models.Option)
```

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/api.py` & `formkit_ninja-0.1.7a1/formkit_ninja/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.shortcuts import get_object_or_404
 from ninja import ModelSchema, Router
+from pydantic import UUID4
 
 from formkit_ninja import formkit_schema, models
 
 router = Router(tags=["FormKit"])
 
 
 class FormKitSchemaIn(ModelSchema):
@@ -40,7 +41,19 @@
     exclude_none=True,
     by_alias=True,
 )
 def get_schemas(request, schema_id: int):
     schema: models.FormKitSchema = get_object_or_404(models.FormKitSchema.objects, id=schema_id)
     model = schema.to_pydantic()
     return model
+
+
+@router.get(
+    "node/{node_id}",
+    response=formkit_schema.FormKitNode,
+    exclude_none=True,
+    by_alias=True,
+)
+def get_node(request, node_id: UUID4):
+    node: models.FormKitSchemaNode = get_object_or_404(models.FormKitSchemaNode.objects, id=node_id)
+    instance = node.get_node()
+    return instance
```

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/fields.py` & `formkit_ninja-0.1.7a1/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.1.7a1/formkit_ninja/formkit_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     html_id: str = Field(None, alias="id")
     name: str | None = Field(None)
     label: str | None = Field(None)
     help: str | None = Field(None)
     validation: str | None = Field(None)
     validationLabel: str | None = Field(None, alias="validation-label")
     validationVisibility: str | None = Field(None, alias="validation-visibility")
+    validationMessages: str | dict[str, str] = Field(None, alias="validation-messages")
     placeholder: str | None = Field(None)
     value: str | None = Field(None)
     prefixIcon: str | None = Field(None, alias="prefix-icon")
     classes: dict[str, str] | None = Field(None)
 
     class Config:
         allow_population_by_field_name = True
@@ -153,14 +154,17 @@
 
 
 class NumberNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["number"] = "number"
     dollar_formkit: str = Field(default="number", alias="$formkit")
     text: str | None
+    max: int | None = None
+    min: int | None = None
+    step: int | None = None
 
 
 class PasswordNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["password"] = "password"
     dollar_formkit: str = Field(default="password", alias="$formkit")
     name: str | None
```

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.1.7a1/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0002_remove_formkitschemanode_children_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0002_remove_formkitschemanode_children_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0003_alter_formcomponents_options_formkitschemanode_group_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0003_alter_formcomponents_options_formkitschemanode_group_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0004_alter_formkitschemanode_group_nodechildren_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0004_alter_formkitschemanode_group_nodechildren_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0005_delete_schemacondition_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0005_delete_schemacondition_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0007_alter_formcomponents_options_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0007_alter_formcomponents_options_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/migrations/0008_rename_new_values_formkitschemanode_node_and_more.py` & `formkit_ninja-0.1.7a1/formkit_ninja/migrations/0008_rename_new_values_formkitschemanode_node_and_more.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.1.6a9/formkit_ninja/models.py` & `formkit_ninja-0.1.7a1/formkit_ninja/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 import uuid
-from typing import Iterable, Type, TypedDict
+from typing import Iterable, Type, TypedDict, get_args
 
 from django.db import models
 from django.utils.functional import cached_property
 from ordered_model.models import OrderedModel
 from pydantic import BaseModel
 from pydantic.utils import ROOT_KEY
 
@@ -175,22 +175,16 @@
         ("$cmp", "Component"),
         ("text", "Text"),
         ("condition", "Condition"),
         ("$formkit", "FormKit"),
         ("$el", "Element"),
         ("raw", "Raw JSON"),
     )
-    FORMKIT_CHOICES = [
-        ("text", "text"),
-        ("number", "number"),
-        ("group", "group"),
-        ("button", "button"),
-        ("radio", "radio"),
-        ("select", "select"),
-    ]
+    FORMKIT_CHOICES = [(t, t) for t in get_args(formkit_schema.FORMKIT_TYPE)]
+
     ELEMENT_TYPE_CHOICES = [("p", "p"), ("h1", "h1"), ("h2", "h2")]
     node_type = models.CharField(max_length=256, choices=NODE_TYPE_CHOICES, blank=True, help_text="")
     description = models.TextField(
         null=True,
         blank=True,
         help_text="Decribe the type of data / reason for this component",
     )
@@ -244,17 +238,14 @@
     def get_node(self) -> formkit_schema.FormKitNode:
         """
         Return a "decorated" node instance
         with restored options and translated fields
         """
         return formkit_schema.FormKitNode.parse_obj(self.get_node_values())
 
-    def __str__(self):
-        return TranslatedValues.get_str(self.label)
-
     def save(self, *args, **kwargs):
         super().save(*args, **kwargs)
 
     @classmethod
     def from_pydantic(
         cls, input_models: Iterable[formkit_schema.FormKitNode]
     ) -> Iterable[tuple["FormKitSchemaNode", Iterable[Option]]]:
```

### Comparing `formkit_ninja-0.1.6a9/pyproject.toml` & `formkit_ninja-0.1.7a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.1.6a9"
+version = "0.1.7a1"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
@@ -13,23 +13,30 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 django-ninja = "^0.21.0"
 Django = "^4.1.5"
 django-ordered-model = "^3.6"
 pydantic = "<2"
 
+[tool.poetry.group.docs]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-django = "^4.5.2"
 isort = "^5.11.4"
 black = "^22.12.0"
 flake8 = "^6.0.0"
 django-extensions = "^3.2.1"
 rich = "^13.1.0"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.1.6"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.format]
 max-line-length = "119"
```

### Comparing `formkit_ninja-0.1.6a9/PKG-INFO` & `formkit_ninja-0.1.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.1.6a9
+Version: 0.1.7a1
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

