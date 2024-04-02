# Comparing `tmp/decent-dp-0.5.0.tar.gz` & `tmp/decent_dp-0.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decent-dp-0.5.0.tar", last modified: Tue Mar 26 15:17:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

