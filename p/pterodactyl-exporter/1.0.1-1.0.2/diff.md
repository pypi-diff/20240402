# Comparing `tmp/pterodactyl_exporter-1.0.1.tar.gz` & `tmp/pterodactyl_exporter-1.0.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pterodactyl_exporter-1.0.1.tar", last modified: Sat Mar 30 09:51:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

