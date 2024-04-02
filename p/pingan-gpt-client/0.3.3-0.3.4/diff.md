# Comparing `tmp/pingan_gpt_client-0.3.3.tar.gz` & `tmp/pingan_gpt_client-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingan_gpt_client-0.3.3.tar", max compression
+gzip compressed data, was "pingan_gpt_client-0.3.4.tar", max compression
```

## Comparing `pingan_gpt_client-0.3.3.tar` & `pingan_gpt_client-0.3.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9804 2024-03-19 06:20:55.982732 pingan_gpt_client-0.3.3/README.md
--rw-r--r--   0        0        0        0 2024-01-31 02:28:42.065698 pingan_gpt_client-0.3.3/pingan_gpt_client/__init__.py
--rw-r--r--   0        0        0    10151 2024-03-19 06:27:34.169716 pingan_gpt_client-0.3.3/pingan_gpt_client/pingan_gpt.py
--rw-r--r--   0        0        0      461 2024-03-19 06:21:33.312187 pingan_gpt_client-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    10471 1970-01-01 00:00:00.000000 pingan_gpt_client-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-04-02 12:41:21.538908 pingan_gpt_client-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-01-31 02:28:42.065698 pingan_gpt_client-0.3.4/pingan_gpt_client/__init__.py
+-rw-r--r--   0        0        0    10151 2024-03-19 06:27:34.169716 pingan_gpt_client-0.3.4/pingan_gpt_client/pingan_gpt.py
+-rw-r--r--   0        0        0      440 2024-04-02 12:41:53.663309 pingan_gpt_client-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 pingan_gpt_client-0.3.4/PKG-INFO
```

### Comparing `pingan_gpt_client-0.3.3/pingan_gpt_client/pingan_gpt.py` & `pingan_gpt_client-0.3.4/pingan_gpt_client/pingan_gpt.py`

 * *Files identical despite different names*

