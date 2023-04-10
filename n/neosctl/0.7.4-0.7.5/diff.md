# Comparing `tmp/neosctl-0.7.4.tar.gz` & `tmp/neosctl-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.7.4.tar", max compression
+gzip compressed data, was "neosctl-0.7.5.tar", max compression
```

## Comparing `neosctl-0.7.4.tar` & `neosctl-0.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2655 2023-03-17 10:04:08.038125 neosctl-0.7.4/README.md
--rw-r--r--   0        0        0       22 2023-03-17 10:04:08.038125 neosctl-0.7.4/neosctl/__init__.py
--rw-r--r--   0        0        0     4478 2023-03-17 10:04:08.038125 neosctl-0.7.4/neosctl/auth.py
--rw-r--r--   0        0        0     4526 2023-03-17 10:04:08.038125 neosctl-0.7.4/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-03-17 10:04:08.038125 neosctl-0.7.4/neosctl/constant.py
--rw-r--r--   0        0        0      723 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/consume.py
--rw-r--r--   0        0        0     3730 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/iam.py
--rw-r--r--   0        0        0     4989 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/kafka.py
--rw-r--r--   0        0        0    13423 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/metadata.py
--rw-r--r--   0        0        0     8769 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/product.py
--rw-r--r--   0        0        0     4420 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/profile.py
--rw-r--r--   0        0        0     3062 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/registry.py
--rw-r--r--   0        0        0     6509 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/schema.py
--rw-r--r--   0        0        0     5884 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/secret.py
--rw-r--r--   0        0        0    10601 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/source.py
--rw-r--r--   0        0        0    14825 2023-03-17 10:04:08.039125 neosctl-0.7.4/neosctl/spark.py
--rw-r--r--   0        0        0    12105 2023-03-17 10:04:08.040125 neosctl-0.7.4/neosctl/storage.py
--rw-r--r--   0        0        0     8339 2023-03-17 10:04:08.040125 neosctl-0.7.4/neosctl/util.py
--rw-r--r--   0        0        0     2712 2023-03-17 10:04:08.040125 neosctl-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 neosctl-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-04-10 08:51:16.732342 neosctl-0.7.5/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/__init__.py
+-rw-r--r--   0        0        0     4478 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/auth.py
+-rw-r--r--   0        0        0     4526 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/constant.py
+-rw-r--r--   0        0        0      723 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/consume.py
+-rw-r--r--   0        0        0     3730 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/iam.py
+-rw-r--r--   0        0        0     4989 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/kafka.py
+-rw-r--r--   0        0        0    15038 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/metadata.py
+-rw-r--r--   0        0        0     7010 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/product.py
+-rw-r--r--   0        0        0     4420 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/profile.py
+-rw-r--r--   0        0        0     3062 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/registry.py
+-rw-r--r--   0        0        0     7189 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/schema.py
+-rw-r--r--   0        0        0     5884 2023-04-10 08:51:16.733343 neosctl-0.7.5/neosctl/secret.py
+-rw-r--r--   0        0        0    10601 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/source.py
+-rw-r--r--   0        0        0    13142 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/spark.py
+-rw-r--r--   0        0        0    12105 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/storage.py
+-rw-r--r--   0        0        0     8339 2023-04-10 08:51:16.734342 neosctl-0.7.5/neosctl/util.py
+-rw-r--r--   0        0        0     2712 2023-04-10 08:51:16.734342 neosctl-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 neosctl-0.7.5/PKG-INFO
```

### Comparing `neosctl-0.7.4/README.md` & `neosctl-0.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.7.4
+# Core CLI v0.7.5
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.7.4/neosctl/auth.py` & `neosctl-0.7.5/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/cli.py` & `neosctl-0.7.5/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/consume.py` & `neosctl-0.7.5/neosctl/consume.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/iam.py` & `neosctl-0.7.5/neosctl/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/kafka.py` & `neosctl-0.7.5/neosctl/kafka.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/metadata.py` & `neosctl-0.7.5/neosctl/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import httpx
 import typer
 
-from neosctl import util
+from neosctl import schema, util
 from neosctl.auth import ensure_login
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 product_app = typer.Typer()
 tag_app = typer.Typer()
@@ -435,14 +435,72 @@
         )
 
     r = _request(ctx)
 
     process_response(r)
 
 
+@product_app.command("quality-rules")
+def quality_rules(
+    ctx: typer.Context,
+) -> None:
+    """Get quality expectations rules."""
+
+    @ensure_login
+    def _request(ctx: typer.Context) -> httpx.Response:
+        return util.get(
+            ctx,
+            _metadata_url(ctx, "/quality/rules"),
+        )
+
+    r = _request(ctx)
+
+    process_response(r)
+
+
+@product_app.command("edit-quality-expectations")
+def edit_product_quality_expectations(
+    ctx: typer.Context,
+    product_identifier: str = typer.Argument(
+        ...,
+        help="Data Product identifier",
+        callback=util.sanitize,
+    ),
+    filepath: str = typer.Option(
+        ...,
+        "--filepath",
+        "-f",
+        help="Filepath of the details json payload",
+        callback=util.sanitize,
+    ),
+) -> None:
+    """Update data product quality expectations."""
+
+    @ensure_login
+    def _request(ctx: typer.Context, uqe: schema.UpdateQualityExpectations) -> httpx.Response:
+        return util.put(
+            ctx,
+            _metadata_url(ctx, f"/product/{product_identifier}/quality/expectation"),
+            json=uqe.dict(exclude_none=True, by_alias=True),
+        )
+
+    fp = util.get_file_location(filepath)
+    details = util.load_object_file(fp, "")
+
+    uqe = schema.UpdateQualityExpectations(
+        custom_details=details["custom_details"],  # type: ignore[reportGeneralTypeIssues]
+        weights=details["weights"],  # type: ignore[reportGeneralTypeIssues]
+        thresholds=details["thresholds"],  # type: ignore[reportGeneralTypeIssues]
+    )
+
+    r = _request(ctx, uqe)
+
+    process_response(r)
+
+
 @product_app.command("quality-expectations")
 def product_quality_expectations(
     ctx: typer.Context,
     product_identifier: str = typer.Argument(
         ...,
         help="Data Product identifier",
         callback=util.sanitize,
```

### Comparing `neosctl-0.7.4/neosctl/product.py` & `neosctl-0.7.5/neosctl/product.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,30 @@
-import json
-import mimetypes
-import pathlib
 import sys
 import typing
 
 import httpx
 
 if sys.platform != "win32":
     import jq
 else:
     jq = None
 
 import typer
 
-from neosctl import constant, schema, util
+from neosctl import schema, util
 from neosctl.auth import ensure_login
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _product_url(ctx: typer.Context) -> str:
     return "{}/product".format(ctx.obj.get_gateway_api_url().rstrip("/"))
 
 
-special_delimiters = {
-    r"\t": "\t",
-}
-
-
-@app.command(name="template")
-def template(
-    ctx: typer.Context,
-    name: str = typer.Argument(..., help="Data Product name", callback=util.sanitize),
-    filepath: str = typer.Option(..., "--filepath", "-f", help="Filepath of the csv template", callback=util.sanitize),
-    output_dir: str = typer.Option(
-        ...,
-        "--output-dir",
-        "-o",
-        help="Output directory for the json template",
-        callback=util.sanitize,
-    ),
-    delimiter: str = typer.Option(",", "--delimiter", "-d", help="csv delimiter", callback=util.sanitize),
-    quotechar: typing.Optional[str] = typer.Option(
-        None,
-        "--quote-char",
-        "-q",
-        help="csv quote char",
-        callback=util.sanitize,
-    ),
-) -> None:
-    """Generate a data product schema template from a csv.
-
-    Given a csv with a header row, generate a template field schema.
-    """
-
-    @ensure_login
-    def _request(ctx: typer.Context, f: typing.IO, mime_type: typing.Optional[str]) -> httpx.Response:
-        params = {k: v for k, v in [("delimiter", delimiter), ("quotechar", quotechar)] if v is not None}
-
-        return util.post(
-            ctx,
-            f"{_product_url(ctx)}/template",
-            params=params,
-            files={"csv_file": ("upload.csv", f, mime_type)},
-        )
-
-    fp = util.get_file_location(filepath)
-    mime_type = mimetypes.guess_type(fp)
-
-    with fp.open("rb") as f:
-        r = _request(ctx, f, mime_type[0])
-
-    if r.status_code >= constant.BAD_REQUEST_CODE:
-        process_response(r)
-
-    fp = pathlib.Path(output_dir) / f"{name}.json"
-    with fp.open("w") as f:
-        json.dump(r.json(), f, indent=4)
-
-
 @app.command(name="create")
 def create(
     ctx: typer.Context,
     name: str = typer.Argument(..., help="Data Product name", callback=util.sanitize),
     description: typing.Optional[str] = typer.Option(
         None,
         "--description",
```

### Comparing `neosctl-0.7.4/neosctl/profile.py` & `neosctl-0.7.5/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/registry.py` & `neosctl-0.7.5/neosctl/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/schema.py` & `neosctl-0.7.5/neosctl/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
 
 class IcebergTableProperties(pydantic.BaseModel):
     format: Optional[str] = None  # noqa: A003
     partitioning: Optional[List[str]] = None
     location: Optional[str] = None
     format_version: Optional[int] = None
-    orc_bloom_filter_columns: Optional[List[str]] = None
-    orc_bloom_filter_fpp: Optional[float] = None
 
 
 class StreamingSchemaBase(pydantic.BaseModel):
     type: Literal["streaming"]  # noqa: A003
     fields: Optional[List[FieldDefinition]]
     iceberg_table_properties: Optional[IcebergTableProperties] = None
 
@@ -82,14 +80,47 @@
     fields: List[FieldDefinition]
 
 
 class UpdateDataProductSchema(pydantic.BaseModel):
     details: Union[StreamingDataProductSchema, StoredDataProductSchema] = pydantic.Field(..., discriminator="type")
 
 
+class ExpectationItem(pydantic.BaseModel):
+    expectation_type: str
+    kwargs: dict
+    meta: dict
+
+
+class ExpectationWeights(pydantic.BaseModel):
+    accuracy: float
+    completeness: float
+    consistency: float
+    uniqueness: float
+    validity: float
+
+
+class ExpectationColumnThresholds(BaseModel):
+    accuracy: Union[float, None]
+    completeness: Union[float, None]
+    consistency: Union[float, None]
+    uniqueness: Union[float, None]
+    validity: Union[float, None]
+
+
+class ExpectationThresholds(BaseModel):
+    table: float
+    columns: Dict[str, ExpectationColumnThresholds]
+
+
+class UpdateQualityExpectations(pydantic.BaseModel):
+    custom_details: List[ExpectationItem]
+    weights: Union[ExpectationWeights, None]
+    thresholds: Union[ExpectationThresholds, None]
+
+
 class RegisterCore(BaseModel):
     partition: str
     name: str
 
 
 class RemoveCore(BaseModel):
     urn: str
```

### Comparing `neosctl-0.7.4/neosctl/secret.py` & `neosctl-0.7.5/neosctl/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/source.py` & `neosctl-0.7.5/neosctl/source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/spark.py` & `neosctl-0.7.5/neosctl/spark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mimetypes
 import typing
 
 import httpx
 import typer
 
 from neosctl import util
 from neosctl.auth import ensure_login
@@ -341,72 +340,14 @@
         )
 
     r = _request(ctx)
     process_response(r)
 
 
 @app.command()
-def csv_job(
-    ctx: typer.Context,
-    product_identifier: str = typer.Argument(
-        ...,
-        help="Data Product identifier",
-        callback=util.sanitize,
-    ),
-    delimiter: str = typer.Option(",", "--delimiter", "-d", help="csv delimiter", callback=util.sanitize),
-    quotechar: typing.Optional[str] = typer.Option(
-        None,
-        "--quote-char",
-        "-q",
-        help="csv quote char",
-        callback=util.sanitize,
-    ),
-    csv_write_mode: typing.Optional[str] = typer.Option(
-        None,
-        "--write-mode",
-        "-w",
-        help="csv write mode [overwrite|append]",
-        callback=util.sanitize,
-    ),
-    job_filepath: str = typer.Option(..., "--job-filepath", "-f", callback=util.sanitize),
-) -> None:
-    """Ingest a csv file into a data product.
-
-    Upload a csv file for processing into a data product.
-    """
-
-    @ensure_login
-    def _request(ctx: typer.Context, f: typing.IO, mime_type: typing.Optional[str]) -> httpx.Response:
-        params = {
-            k: v
-            for k, v in [
-                ("delimiter", delimiter),
-                ("quotechar", quotechar),
-                ("csv_write_mode", csv_write_mode),
-            ]
-            if v is not None
-        }
-
-        return util.post(
-            ctx,
-            f"{_spark_url(product_identifier, ctx.obj.gateway_api_url)}/csv",
-            params=params,
-            files={"csv_file": ("upload.csv", f, mime_type)},
-        )
-
-    fp = util.get_file_location(job_filepath)
-    mime_type = mimetypes.guess_type(fp)
-
-    with fp.open("rb") as f:
-        r = _request(ctx, f, mime_type[0])
-
-    process_response(r)
-
-
-@app.command()
 def schedule_job(
     ctx: typer.Context,
     product_identifier: str = typer.Argument(
         ...,
         help="Data Product identifier",
         callback=util.sanitize,
     ),
```

### Comparing `neosctl-0.7.4/neosctl/storage.py` & `neosctl-0.7.5/neosctl/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/neosctl/util.py` & `neosctl-0.7.5/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.4/pyproject.toml` & `neosctl-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.7.4"
+version = "0.7.5"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.7.4/PKG-INFO` & `neosctl-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.7.4
+Version: 0.7.5
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 Requires-Dist: jq (>=1.4.0,<2.0.0) ; sys_platform != "win32"
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (>=4.4.0,<5.0.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.7.4
+# Core CLI v0.7.5
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

