# Comparing `tmp/hahomematic-2024.3.1.tar.gz` & `tmp/hahomematic-2024.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.3.1.tar", last modified: Tue Mar 12 14:24:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

