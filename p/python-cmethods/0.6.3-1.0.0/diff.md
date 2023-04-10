# Comparing `tmp/python-cmethods-0.6.3.tar.gz` & `tmp/python_cmethods-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cmethods-0.6.3.tar", last modified: Wed Mar 22 18:52:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

