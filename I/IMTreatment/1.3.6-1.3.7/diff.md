# Comparing `tmp/IMTreatment-1.3.6.tar.gz` & `tmp/IMTreatment-1.3.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMTreatment-1.3.6.tar", last modified: Wed Dec 13 16:05:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

