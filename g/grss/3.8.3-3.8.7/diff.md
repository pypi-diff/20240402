# Comparing `tmp/grss-3.8.3.tar.gz` & `tmp/grss-3.8.7-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grss-3.8.3.tar", last modified: Thu Mar 28 04:53:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

