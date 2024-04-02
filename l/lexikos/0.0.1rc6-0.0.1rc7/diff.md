# Comparing `tmp/lexikos-0.0.1rc6.tar.gz` & `tmp/lexikos-0.0.1rc7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc6.tar", last modified: Fri Jul  7 10:18:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

