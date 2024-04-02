# Comparing `tmp/comiccrawler-2024.3.25.tar.gz` & `tmp/comiccrawler-2024.4.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comiccrawler-2024.3.25.tar", last modified: Mon Mar 25 06:20:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

