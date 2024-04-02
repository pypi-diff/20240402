# Comparing `tmp/modlee-0.0.1.post6.tar.gz` & `tmp/modlee-0.0.1.post7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modlee-0.0.1.post6.tar", last modified: Mon Apr  1 18:30:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

