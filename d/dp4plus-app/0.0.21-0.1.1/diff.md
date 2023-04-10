# Comparing `tmp/dp4plus_app-0.0.21.tar.gz` & `tmp/dp4plus_app-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp4plus_app-0.0.21.tar", last modified: Wed Apr  5 19:11:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

