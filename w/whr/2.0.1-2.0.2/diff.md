# Comparing `tmp/whr-2.0.1.tar.gz` & `tmp/whr-2.0.2-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whr-2.0.1.tar", last modified: Sun Mar 31 15:05:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

