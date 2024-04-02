# Comparing `tmp/pytorch_rocm_gtt-0.1.1.tar.gz` & `tmp/pytorch_rocm_gtt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_rocm_gtt-0.1.1.tar", max compression
+gzip compressed data, was "pytorch_rocm_gtt-0.1.2.tar", max compression
```

## Comparing `pytorch_rocm_gtt-0.1.1.tar` & `pytorch_rocm_gtt-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2024-04-02 00:41:38.081826 pytorch_rocm_gtt-0.1.1/LICENSE
--rw-r--r--   0        0        0     1464 2024-04-02 00:41:38.081826 pytorch_rocm_gtt-0.1.1/README.md
--rw-r--r--   0        0        0      557 2024-04-02 00:41:38.085826 pytorch_rocm_gtt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-02 00:41:38.085826 pytorch_rocm_gtt-0.1.1/pytorch_rocm_gtt/VERSION
--rw-r--r--   0        0        0      709 2024-04-02 00:41:38.085826 pytorch_rocm_gtt-0.1.1/pytorch_rocm_gtt/__init__.py
--rw-r--r--   0        0        0      510 2024-04-02 00:41:38.085826 pytorch_rocm_gtt-0.1.1/pytorch_rocm_gtt/gttalloc.c
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 pytorch_rocm_gtt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-02 01:08:51.648657 pytorch_rocm_gtt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2820 2024-04-02 01:08:51.648657 pytorch_rocm_gtt-0.1.2/README.md
+-rw-r--r--   0        0        0      720 2024-04-02 01:08:51.652657 pytorch_rocm_gtt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-02 01:08:51.652657 pytorch_rocm_gtt-0.1.2/pytorch_rocm_gtt/VERSION
+-rw-r--r--   0        0        0      709 2024-04-02 01:08:51.652657 pytorch_rocm_gtt-0.1.2/pytorch_rocm_gtt/__init__.py
+-rw-r--r--   0        0        0      510 2024-04-02 01:08:51.652657 pytorch_rocm_gtt-0.1.2/pytorch_rocm_gtt/gttalloc.c
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 pytorch_rocm_gtt-0.1.2/PKG-INFO
```

### Comparing `pytorch_rocm_gtt-0.1.1/LICENSE` & `pytorch_rocm_gtt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_rocm_gtt-0.1.1/pyproject.toml` & `pytorch_rocm_gtt-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "pytorch-rocm-gtt"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "A memory allocator for PyTorch to allow using more memory than the iGPU reserved"
 authors = ["rochacbruno"]
 readme = "README.md"
 
+[tool.poetry.urls]
+"repository" = "https://github.com/pappacena/pytorch-rocm-gtt"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.4.4"
```

### Comparing `pytorch_rocm_gtt-0.1.1/pytorch_rocm_gtt/__init__.py` & `pytorch_rocm_gtt-0.1.2/pytorch_rocm_gtt/__init__.py`

 * *Files identical despite different names*

