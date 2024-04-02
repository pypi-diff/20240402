# Comparing `tmp/mlpfile-0.2.1.tar.gz` & `tmp/mlpfile-0.3.0-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpfile-0.2.1.tar", last modified: Mon Sep 11 19:23:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

