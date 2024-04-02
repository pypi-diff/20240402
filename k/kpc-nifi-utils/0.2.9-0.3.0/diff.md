# Comparing `tmp/kpc_nifi_utils-0.2.9.tar.gz` & `tmp/kpc_nifi_utils-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kpc_nifi_utils-0.2.9.tar", last modified: Wed Mar 24 13:28:04 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

