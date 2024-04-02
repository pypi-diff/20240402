# Comparing `tmp/adelie-1.1.25.tar.gz` & `tmp/adelie-1.1.26-cp39-cp39-macosx_14_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelie-1.1.25.tar", last modified: Mon Apr  1 14:52:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

