# Comparing `tmp/coola-0.5.1.tar.gz` & `tmp/coola-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.5.1.tar", max compression
+gzip compressed data, was "coola-0.6.0.tar", max compression
```

## Comparing `coola-0.5.1.tar` & `coola-0.6.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0     1501 2024-03-23 00:51:08.907697 coola-0.5.1/LICENSE
--rw-r--r--   0        0        0    11161 2024-03-23 00:51:08.907697 coola-0.5.1/README.md
--rw-r--r--   0        0        0     6864 2024-03-23 00:51:08.911697 coola-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      553 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/__init__.py
--rw-r--r--   0        0        0     3618 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/comparison.py
--rw-r--r--   0        0        0      266 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/__init__.py
--rw-r--r--   0        0        0     1935 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/__init__.py
--rw-r--r--   0        0        0     2426 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/base.py
--rw-r--r--   0        0        0     4122 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/collection.py
--rw-r--r--   0        0        0     2123 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/default.py
--rw-r--r--   0        0        0     2998 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/jax_.py
--rw-r--r--   0        0        0     4481 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/numpy_.py
--rw-r--r--   0        0        0     4208 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/pandas_.py
--rw-r--r--   0        0        0     4262 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/polars_.py
--rw-r--r--   0        0        0     2130 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/scalar.py
--rw-r--r--   0        0        0     4631 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/torch_.py
--rw-r--r--   0        0        0     1493 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/utils.py
--rw-r--r--   0        0        0     6502 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/comparators/xarray_.py
--rw-r--r--   0        0        0      488 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/config.py
--rw-r--r--   0        0        0     2074 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/__init__.py
--rw-r--r--   0        0        0     4973 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/base.py
--rw-r--r--   0        0        0     2098 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/data.py
--rw-r--r--   0        0        0     2256 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/dtype.py
--rw-r--r--   0        0        0     2849 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/equal.py
--rw-r--r--   0        0        0     2827 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/jax_.py
--rw-r--r--   0        0        0     3820 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/mapping.py
--rw-r--r--   0        0        0     9512 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/native.py
--rw-r--r--   0        0        0     2790 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/numpy_.py
--rw-r--r--   0        0        0     5624 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/pandas_.py
--rw-r--r--   0        0        0     6173 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/polars_.py
--rw-r--r--   0        0        0     3630 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/scalar.py
--rw-r--r--   0        0        0     2129 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/sequence.py
--rw-r--r--   0        0        0     2306 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/shape.py
--rw-r--r--   0        0        0     4186 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/handlers/torch_.py
--rw-r--r--   0        0        0      319 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/testers/__init__.py
--rw-r--r--   0        0        0     1348 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/testers/base.py
--rw-r--r--   0        0        0     9794 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/equality/testers/default.py
--rw-r--r--   0        0        0      502 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/formatters/__init__.py
--rw-r--r--   0        0        0     3485 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/formatters/base.py
--rw-r--r--   0        0        0    11668 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/formatters/default.py
--rw-r--r--   0        0        0     3543 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/formatters/numpy_.py
--rw-r--r--   0        0        0     3577 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/formatters/torch_.py
--rw-r--r--   0        0        0      875 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/__init__.py
--rw-r--r--   0        0        0     1822 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/base.py
--rw-r--r--   0        0        0     5605 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/default.py
--rw-r--r--   0        0        0     1397 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/functional.py
--rw-r--r--   0        0        0     2858 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/numpy_.py
--rw-r--r--   0        0        0     1363 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/random_.py
--rw-r--r--   0        0        0     2953 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/torch_.py
--rw-r--r--   0        0        0      826 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/random/utils.py
--rw-r--r--   0        0        0      552 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/__init__.py
--rw-r--r--   0        0        0     8056 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/base.py
--rw-r--r--   0        0        0     1600 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/basic.py
--rw-r--r--   0        0        0     2381 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/numpy_.py
--rw-r--r--   0        0        0     2793 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/registry.py
--rw-r--r--   0        0        0     2441 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/torch_.py
--rw-r--r--   0        0        0      907 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reducers/utils.py
--rw-r--r--   0        0        0     1722 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/reduction.py
--rw-r--r--   0        0        0     1535 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/summarization.py
--rw-r--r--   0        0        0      322 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/summarizers/__init__.py
--rw-r--r--   0        0        0     2983 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/summarizers/base.py
--rw-r--r--   0        0        0    12758 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/summarizers/summarizer.py
--rw-r--r--   0        0        0     1302 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/testing.py
--rw-r--r--   0        0        0      573 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/types.py
--rw-r--r--   0        0        0      871 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/__init__.py
--rw-r--r--   0        0        0     1189 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/array.py
--rw-r--r--   0        0        0     5837 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/format.py
--rw-r--r--   0        0        0    11275 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/imports.py
--rw-r--r--   0        0        0     1070 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/stats.py
--rw-r--r--   0        0        0     2632 2024-03-23 00:51:08.911697 coola-0.5.1/src/coola/utils/tensor.py
--rw-r--r--   0        0        0    12656 1970-01-01 00:00:00.000000 coola-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-04-02 04:09:13.904312 coola-0.6.0/LICENSE
+-rw-r--r--   0        0        0    11161 2024-04-02 04:09:13.904312 coola-0.6.0/README.md
+-rw-r--r--   0        0        0     6864 2024-04-02 04:09:13.904312 coola-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/__init__.py
+-rw-r--r--   0        0        0     3628 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/comparison.py
+-rw-r--r--   0        0        0      266 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/__init__.py
+-rw-r--r--   0        0        0     1935 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/__init__.py
+-rw-r--r--   0        0        0     2426 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/base.py
+-rw-r--r--   0        0        0     4122 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/collection.py
+-rw-r--r--   0        0        0     2123 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/default.py
+-rw-r--r--   0        0        0     2998 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/jax_.py
+-rw-r--r--   0        0        0     4481 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/numpy_.py
+-rw-r--r--   0        0        0     4208 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/pandas_.py
+-rw-r--r--   0        0        0     4262 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/polars_.py
+-rw-r--r--   0        0        0     2130 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/scalar.py
+-rw-r--r--   0        0        0     4631 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/torch_.py
+-rw-r--r--   0        0        0     1493 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/utils.py
+-rw-r--r--   0        0        0     6502 2024-04-02 04:09:13.904312 coola-0.6.0/src/coola/equality/comparators/xarray_.py
+-rw-r--r--   0        0        0      488 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/config.py
+-rw-r--r--   0        0        0     2074 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/__init__.py
+-rw-r--r--   0        0        0     4973 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/base.py
+-rw-r--r--   0        0        0     2098 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/data.py
+-rw-r--r--   0        0        0     2256 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/dtype.py
+-rw-r--r--   0        0        0     2849 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/equal.py
+-rw-r--r--   0        0        0     2827 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/jax_.py
+-rw-r--r--   0        0        0     3820 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/mapping.py
+-rw-r--r--   0        0        0     9512 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/native.py
+-rw-r--r--   0        0        0     2790 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/numpy_.py
+-rw-r--r--   0        0        0     5624 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/pandas_.py
+-rw-r--r--   0        0        0     6173 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/polars_.py
+-rw-r--r--   0        0        0     3630 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/scalar.py
+-rw-r--r--   0        0        0     2129 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/sequence.py
+-rw-r--r--   0        0        0     2306 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/shape.py
+-rw-r--r--   0        0        0     4186 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/handlers/torch_.py
+-rw-r--r--   0        0        0      319 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/base.py
+-rw-r--r--   0        0        0     9794 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/equality/testers/default.py
+-rw-r--r--   0        0        0      502 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/__init__.py
+-rw-r--r--   0        0        0     3485 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/base.py
+-rw-r--r--   0        0        0    11668 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/default.py
+-rw-r--r--   0        0        0     3543 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/numpy_.py
+-rw-r--r--   0        0        0     3577 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/formatters/torch_.py
+-rw-r--r--   0        0        0      445 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/__init__.py
+-rw-r--r--   0        0        0     1780 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/conversion.py
+-rw-r--r--   0        0        0     4100 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/nested/mapping.py
+-rw-r--r--   0        0        0      875 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/__init__.py
+-rw-r--r--   0        0        0     1822 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/base.py
+-rw-r--r--   0        0        0     5605 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/default.py
+-rw-r--r--   0        0        0     1397 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/functional.py
+-rw-r--r--   0        0        0     2858 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/numpy_.py
+-rw-r--r--   0        0        0     1363 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/random_.py
+-rw-r--r--   0        0        0     2953 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/torch_.py
+-rw-r--r--   0        0        0      826 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/random/utils.py
+-rw-r--r--   0        0        0      555 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/__init__.py
+-rw-r--r--   0        0        0     8056 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/base.py
+-rw-r--r--   0        0        0     1605 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/native.py
+-rw-r--r--   0        0        0     2381 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/numpy_.py
+-rw-r--r--   0        0        0     2802 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/registry.py
+-rw-r--r--   0        0        0     2441 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/torch_.py
+-rw-r--r--   0        0        0      909 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reducers/utils.py
+-rw-r--r--   0        0        0     1722 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/reduction.py
+-rw-r--r--   0        0        0     1535 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarization.py
+-rw-r--r--   0        0        0      322 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/__init__.py
+-rw-r--r--   0        0        0     2983 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/base.py
+-rw-r--r--   0        0        0    12758 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/summarizers/summarizer.py
+-rw-r--r--   0        0        0     1302 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/testing.py
+-rw-r--r--   0        0        0      573 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/types.py
+-rw-r--r--   0        0        0      871 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/__init__.py
+-rw-r--r--   0        0        0     1189 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/array.py
+-rw-r--r--   0        0        0     5837 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/format.py
+-rw-r--r--   0        0        0    11275 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/imports.py
+-rw-r--r--   0        0        0     1070 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/stats.py
+-rw-r--r--   0        0        0     2632 2024-04-02 04:09:13.908311 coola-0.6.0/src/coola/utils/tensor.py
+-rw-r--r--   0        0        0    12656 1970-01-01 00:00:00.000000 coola-0.6.0/PKG-INFO
```

### Comparing `coola-0.5.1/LICENSE` & `coola-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/README.md` & `coola-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/pyproject.toml` & `coola-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coola"
-version = "0.5.1"
+version = "0.6.0"
 description = "A library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = [
     "complex/nested objects",
@@ -62,19 +62,19 @@
 mkdocs-material = "^9.5"
 mkdocstrings = { extras = ["python"], version = "^0.24" }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=24.3"
 coverage = { extras = ["toml"], version = "^7.4" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
-pre-commit = "^3.6"
+pre-commit = "^3.7"
 pygments = "^2.17"
 pytest = "^8.1"
-pytest-cov = "^4.1"
-pytest-timeout = "^2.2"
+pytest-cov = "^5.0"
+pytest-timeout = "^2.3"
 ruff = ">=0.3.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coola-0.5.1/src/coola/__init__.py` & `coola-0.6.0/src/coola/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/comparison.py` & `coola-0.6.0/src/coola/comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from coola.equality.config import EqualityConfig
 from coola.equality.testers import EqualityTester
 
 if TYPE_CHECKING:
     from coola.equality.testers import BaseEqualityTester
 
+_tester = EqualityTester()
+
 
 def objects_are_allclose(
     actual: Any,
     expected: Any,
     *,
     rtol: float = 1e-5,
     atol: float = 1e-8,
@@ -63,15 +65,15 @@
     ...     rtol=0,
     ...     atol=1e-8,
     ... )
     False
 
     ```
     """
-    tester = tester or EqualityTester()
+    tester = tester or _tester
     config = EqualityConfig(
         tester=tester, show_difference=show_difference, equal_nan=equal_nan, atol=atol, rtol=rtol
     )
     return tester.equal(actual, expected, config)
 
 
 def objects_are_equal(
@@ -110,10 +112,10 @@
     ... )
     True
     >>> objects_are_equal([torch.ones(2, 3), torch.ones(2)], [torch.ones(2, 3), torch.zeros(2)])
     False
 
     ```
     """
-    tester = tester or EqualityTester()
+    tester = tester or _tester
     config = EqualityConfig(tester=tester, show_difference=show_difference, equal_nan=equal_nan)
     return tester.equal(actual, expected, config)
```

### Comparing `coola-0.5.1/src/coola/equality/comparators/__init__.py` & `coola-0.6.0/src/coola/equality/comparators/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/base.py` & `coola-0.6.0/src/coola/equality/comparators/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/collection.py` & `coola-0.6.0/src/coola/equality/comparators/collection.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/default.py` & `coola-0.6.0/src/coola/equality/comparators/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/jax_.py` & `coola-0.6.0/src/coola/equality/comparators/jax_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/numpy_.py` & `coola-0.6.0/src/coola/equality/comparators/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/pandas_.py` & `coola-0.6.0/src/coola/equality/comparators/pandas_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/polars_.py` & `coola-0.6.0/src/coola/equality/comparators/polars_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/scalar.py` & `coola-0.6.0/src/coola/equality/comparators/scalar.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/torch_.py` & `coola-0.6.0/src/coola/equality/comparators/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/utils.py` & `coola-0.6.0/src/coola/equality/comparators/utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/comparators/xarray_.py` & `coola-0.6.0/src/coola/equality/comparators/xarray_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/__init__.py` & `coola-0.6.0/src/coola/equality/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/base.py` & `coola-0.6.0/src/coola/equality/handlers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/data.py` & `coola-0.6.0/src/coola/equality/handlers/data.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/dtype.py` & `coola-0.6.0/src/coola/equality/handlers/dtype.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/equal.py` & `coola-0.6.0/src/coola/equality/handlers/equal.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/jax_.py` & `coola-0.6.0/src/coola/equality/handlers/jax_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/mapping.py` & `coola-0.6.0/src/coola/equality/handlers/mapping.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/native.py` & `coola-0.6.0/src/coola/equality/handlers/native.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/numpy_.py` & `coola-0.6.0/src/coola/equality/handlers/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/pandas_.py` & `coola-0.6.0/src/coola/equality/handlers/pandas_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/polars_.py` & `coola-0.6.0/src/coola/equality/handlers/polars_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/scalar.py` & `coola-0.6.0/src/coola/equality/handlers/scalar.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/sequence.py` & `coola-0.6.0/src/coola/equality/handlers/sequence.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/shape.py` & `coola-0.6.0/src/coola/equality/handlers/shape.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/handlers/torch_.py` & `coola-0.6.0/src/coola/equality/handlers/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/testers/base.py` & `coola-0.6.0/src/coola/equality/testers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/equality/testers/default.py` & `coola-0.6.0/src/coola/equality/testers/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/formatters/base.py` & `coola-0.6.0/src/coola/formatters/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/formatters/default.py` & `coola-0.6.0/src/coola/formatters/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/formatters/numpy_.py` & `coola-0.6.0/src/coola/formatters/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/formatters/torch_.py` & `coola-0.6.0/src/coola/formatters/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/__init__.py` & `coola-0.6.0/src/coola/random/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/base.py` & `coola-0.6.0/src/coola/random/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/default.py` & `coola-0.6.0/src/coola/random/default.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/functional.py` & `coola-0.6.0/src/coola/random/functional.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/numpy_.py` & `coola-0.6.0/src/coola/random/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/random_.py` & `coola-0.6.0/src/coola/random/random_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/torch_.py` & `coola-0.6.0/src/coola/random/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/random/utils.py` & `coola-0.6.0/src/coola/random/utils.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/reducers/__init__.py` & `coola-0.6.0/src/coola/reducers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 r"""Contain the reducer implementations."""
 
 __all__ = [
     "BaseBasicReducer",
     "BaseReducer",
-    "BasicReducer",
+    "NativeReducer",
     "EmptySequenceError",
     "NumpyReducer",
     "ReducerRegistry",
     "TorchReducer",
     "auto_reducer",
 ]
 
 from coola.reducers.base import BaseBasicReducer, BaseReducer, EmptySequenceError
-from coola.reducers.basic import BasicReducer
+from coola.reducers.native import NativeReducer
 from coola.reducers.numpy_ import NumpyReducer
 from coola.reducers.registry import ReducerRegistry
 from coola.reducers.torch_ import TorchReducer
 from coola.reducers.utils import auto_reducer
```

### Comparing `coola-0.5.1/src/coola/reducers/base.py` & `coola-0.6.0/src/coola/reducers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/reducers/basic.py` & `coola-0.6.0/src/coola/reducers/native.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 r"""Implement a simple reducer that uses only standard libray
 functions."""
 
 from __future__ import annotations
 
-__all__ = ["BasicReducer"]
+__all__ = ["NativeReducer"]
 
 from collections.abc import Sequence
 from statistics import mean, median, stdev
 from typing import TypeVar, Union
 
 from coola.reducers.base import BaseBasicReducer
 from coola.utils.stats import quantile
 
 T = TypeVar("T", bound=Sequence[Union[int, float]])
 
 
-class BasicReducer(BaseBasicReducer[T]):
-    r"""Implement a basic reducer.
+class NativeReducer(BaseBasicReducer[T]):
+    r"""Implement a native reducer.
 
     Example usage:
 
     ```pycon
-    >>> from coola.reducers import BasicReducer
-    >>> reducer = BasicReducer()
+    >>> from coola.reducers import NativeReducer
+    >>> reducer = NativeReducer()
     >>> reducer.max([-2, -1, 0, 1, 2])
     2
     >>> reducer.median([-2, -1, 0, 1, 2])
     0
     >>> reducer.sort([2, 1, -2, 3, 0])
     [-2, 0, 1, 2, 3]
```

### Comparing `coola-0.5.1/src/coola/reducers/numpy_.py` & `coola-0.6.0/src/coola/reducers/numpy_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/reducers/registry.py` & `coola-0.6.0/src/coola/reducers/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 r"""Implement a registry of reducers."""
 
 __all__ = ["ReducerRegistry"]
 
 from typing import ClassVar
 
 from coola.reducers.base import BaseReducer
-from coola.reducers.basic import BasicReducer
+from coola.reducers.native import NativeReducer
 from coola.utils.format import str_indent, str_mapping
 
 
 class ReducerRegistry:
     """Implement the reducer registry.
 
     The registry is a class variable, so it is shared with all the
     instances of this class.
     """
 
-    registry: ClassVar[dict[str, BaseReducer]] = {"basic": BasicReducer()}
+    registry: ClassVar[dict[str, BaseReducer]] = {"native": NativeReducer()}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}(\n  {str_indent(str_mapping(self.registry))}\n)"
 
     @classmethod
     def add_reducer(cls, name: str, reducer: BaseReducer, exist_ok: bool = False) -> None:
         r"""Add a reducer to the registry.
@@ -35,16 +35,16 @@
         Raises:
             RuntimeError: if a reducer is already registered for the
                 name and ``exist_ok=False``.
 
         Example usage:
 
         ```pycon
-        >>> from coola.reducers import ReducerRegistry, BasicReducer
-        >>> ReducerRegistry.add_reducer("basic", BasicReducer(), exist_ok=True)
+        >>> from coola.reducers import ReducerRegistry, NativeReducer
+        >>> ReducerRegistry.add_reducer("native", NativeReducer(), exist_ok=True)
 
         ```
         """
         if name in cls.registry and not exist_ok:
             msg = (
                 f"A reducer ({cls.registry[name]}) is already registered for the name "
                 f"{name}. Please use `exist_ok=True` if you want to overwrite the "
@@ -61,15 +61,15 @@
             The available reducers.
 
         Example usage:
 
         ```pycon
         >>> from coola.reducers import ReducerRegistry
         >>> ReducerRegistry.available_reducers()
-        ('basic', 'numpy', 'torch')
+        ('native', 'numpy', 'torch')
 
         ```
         """
         return tuple(cls.registry.keys())
 
     @classmethod
     def has_reducer(cls, name: str) -> bool:
@@ -82,15 +82,15 @@
             ``True`` if a reducer is registered,
                 otherwise ``False``.
 
         Example usage:
 
         ```pycon
         >>> from coola.reducers import ReducerRegistry
-        >>> ReducerRegistry.has_reducer("basic")
+        >>> ReducerRegistry.has_reducer("native")
         True
         >>> ReducerRegistry.has_reducer("missing")
         False
 
         ```
         """
         return name in cls.registry
```

### Comparing `coola-0.5.1/src/coola/reducers/torch_.py` & `coola-0.6.0/src/coola/reducers/torch_.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/reducers/utils.py` & `coola-0.6.0/src/coola/reducers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""Implement utility functions for reducers."""
 
 from __future__ import annotations
 
 __all__ = ["auto_reducer"]
 
-from coola.reducers import BaseReducer, BasicReducer, NumpyReducer, TorchReducer
+from coola.reducers import BaseReducer, NativeReducer, NumpyReducer, TorchReducer
 from coola.utils import is_numpy_available, is_torch_available
 
 
 def auto_reducer() -> BaseReducer:
     r"""Find the "best" reducer to used based on the installed packages.
 
     The "best" reducer is found by using the following rules:
@@ -27,8 +27,8 @@
 
     ```
     """
     if is_torch_available():
         return TorchReducer()
     if is_numpy_available():
         return NumpyReducer()
-    return BasicReducer()
+    return NativeReducer()
```

### Comparing `coola-0.5.1/src/coola/reduction.py` & `coola-0.6.0/src/coola/reduction.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/summarization.py` & `coola-0.6.0/src/coola/summarization.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/summarizers/base.py` & `coola-0.6.0/src/coola/summarizers/base.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/summarizers/summarizer.py` & `coola-0.6.0/src/coola/summarizers/summarizer.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/testing.py` & `coola-0.6.0/src/coola/testing.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/types.py` & `coola-0.6.0/src/coola/types.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/__init__.py` & `coola-0.6.0/src/coola/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/array.py` & `coola-0.6.0/src/coola/utils/array.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/format.py` & `coola-0.6.0/src/coola/utils/format.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/imports.py` & `coola-0.6.0/src/coola/utils/imports.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/stats.py` & `coola-0.6.0/src/coola/utils/stats.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/src/coola/utils/tensor.py` & `coola-0.6.0/src/coola/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `coola-0.5.1/PKG-INFO` & `coola-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.5.1
+Version: 0.6.0
 Summary: A library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: complex/nested objects,equality,jax,numpy,pandas,polars,pytorch,xarray
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coola Version: 0.5.1 Summary: A library to check if
+Metadata-Version: 2.1 Name: coola Version: 0.6.0 Summary: A library to check if
 two complex/nested objects are equal or not Home-page: https://github.com/
 durandtibo/coola License: BSD-3-Clause Keywords: complex/nested
 objects,equality,jax,numpy,pandas,polars,pytorch,xarray Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
```

