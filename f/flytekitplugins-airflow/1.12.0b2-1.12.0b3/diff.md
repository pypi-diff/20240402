# Comparing `tmp/flytekitplugins-airflow-1.12.0b2.tar.gz` & `tmp/flytekitplugins_airflow-1.12.0b3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-airflow-1.12.0b2.tar", last modified: Fri Mar 29 21:24:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

