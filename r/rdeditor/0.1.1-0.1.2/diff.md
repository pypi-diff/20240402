# Comparing `tmp/rdeditor-0.1.1.tar.gz` & `tmp/rdeditor-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdeditor-0.1.1.tar", last modified: Tue Apr  2 12:41:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

