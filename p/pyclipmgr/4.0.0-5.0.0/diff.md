# Comparing `tmp/pyclipmgr-4.0.0.tar.gz` & `tmp/pyclipmgr-5.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-4.0.0.tar", last modified: Tue Apr  2 09:46:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

