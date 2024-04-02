# Comparing `tmp/edgeimpulse_api-1.48.7.tar.gz` & `tmp/edgeimpulse_api-1.49.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.48.7.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

