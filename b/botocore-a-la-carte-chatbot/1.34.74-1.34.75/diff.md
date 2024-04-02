# Comparing `tmp/botocore-a-la-carte-chatbot-1.34.74.tar.gz` & `tmp/botocore_a_la_carte_chatbot-1.34.75-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-chatbot-1.34.74.tar", last modified: Sat Mar 30 00:57:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

