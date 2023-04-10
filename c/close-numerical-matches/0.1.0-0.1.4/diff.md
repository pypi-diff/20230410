# Comparing `tmp/close-numerical-matches-0.1.0.tar.gz` & `tmp/close_numerical_matches-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/close-numerical-matches-0.1.0.tar", last modified: Sun Jul 11 10:52:17 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

