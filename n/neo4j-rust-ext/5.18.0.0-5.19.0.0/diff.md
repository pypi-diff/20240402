# Comparing `tmp/neo4j_rust_ext-5.18.0.0.tar.gz` & `tmp/neo4j_rust_ext-5.19.0.0-cp38-cp38-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

