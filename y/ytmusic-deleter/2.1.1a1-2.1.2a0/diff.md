# Comparing `tmp/ytmusic_deleter-2.1.1a1.tar.gz` & `tmp/ytmusic_deleter-2.1.2a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.1.1a1.tar", last modified: Sat Mar 23 01:26:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

