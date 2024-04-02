# Comparing `tmp/sybil_engine-6.5.1.tar.gz` & `tmp/sybil_engine-6.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.5.1.tar", last modified: Sat Mar 30 16:20:26 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

