# Comparing `tmp/globsters-0.0.2.tar.gz` & `tmp/globsters-0.0.3-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

