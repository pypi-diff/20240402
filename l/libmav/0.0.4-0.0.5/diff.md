# Comparing `tmp/libmav-0.0.4.tar.gz` & `tmp/libmav-0.0.5-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmav-0.0.4.tar", last modified: Wed Nov 22 12:25:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

