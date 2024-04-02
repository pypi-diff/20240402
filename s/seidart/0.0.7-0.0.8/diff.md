# Comparing `tmp/seidart-0.0.7.tar.gz` & `tmp/seidart-0.0.8-cp311-cp311-manylinux_2_24_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seidart-0.0.7.tar", last modified: Tue Apr  2 02:27:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

