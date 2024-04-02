# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.15.5.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.15.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.15.5.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

