# Comparing `tmp/pmpt-1.0.1.8510971585.tar.gz` & `tmp/pmpt-1.0.1.post8487904168-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmpt-1.0.1.8510971585.tar", last modified: Mon Apr  1 17:00:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

