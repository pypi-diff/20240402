# Comparing `tmp/rayoptics-0.8.5.tar.gz` & `tmp/rayoptics-0.8.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayoptics-0.8.5.tar", last modified: Wed Oct 12 07:08:22 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

