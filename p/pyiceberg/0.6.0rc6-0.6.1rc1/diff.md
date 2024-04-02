# Comparing `tmp/pyiceberg-0.6.0rc6.tar.gz` & `tmp/pyiceberg-0.6.1rc1-cp39-cp39-macosx_14_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiceberg-0.6.0rc6.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

