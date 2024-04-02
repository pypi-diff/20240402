# Comparing `tmp/geoindex_rs-0.1.0.tar.gz` & `tmp/geoindex_rs-0.2.0b1.tar.gz`

## Comparing `geoindex_rs-0.1.0.tar` & `geoindex_rs-0.2.0b1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0     1001      127      745 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/.github/workflows/python-wheels.yml
--rw-r--r--   0     1001      127      697 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127      486 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      127     9723 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/LICENSE_APACHE
--rw-r--r--   0     1001      127     1068 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/LICENSE_MIT
--rw-r--r--   0     1001      127     7165 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/README.md
--rw-r--r--   0     1001      127      147 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/benches/README.md
--rw-r--r--   0     1001      127      236 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/benches/generate_data.py
--rw-r--r--   0     1001      127     5443 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/benches/rtree.rs
--rw-r--r--   0     1001      127     3680 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/fixtures/data1_flatbush_js.raw
--rw-r--r--   0     1001      127     3200 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/fixtures/data1_input.raw
--rw-r--r--   0     1001      127      877 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/fixtures/flatbush_generate.js
--rw-r--r--   0     1001      127     2053 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/fixtures/generate_data.py
--rw-r--r--   0     1001      127     1185 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/package-lock.json
--rw-r--r--   0     1001      127      167 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/package.json
--rw-r--r--   0     1001      127      191 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/error.rs
--rw-r--r--   0     1001      127     3096 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/indices.rs
--rw-r--r--   0     1001      127     6819 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/builder.rs
--rw-r--r--   0     1001      127      161 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/constants.rs
--rw-r--r--   0     1001      127     3686 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/index.rs
--rw-r--r--   0     1001      127      248 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/mod.rs
--rw-r--r--   0     1001      127     6301 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/test.rs
--rw-r--r--   0     1001      127     5075 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/kdtree/trait.rs
--rw-r--r--   0     1001      127      220 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     7381 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/builder.rs
--rw-r--r--   0     1001      127       65 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/constants.rs
--rw-r--r--   0     1001      127     3741 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/index.rs
--rw-r--r--   0     1001      127      253 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/mod.rs
--rw-r--r--   0     1001      127     5487 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/sort/hilbert.rs
--rw-r--r--   0     1001      127      175 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/sort/mod.rs
--rw-r--r--   0     1001      127     4973 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/sort/str.rs
--rw-r--r--   0     1001      127      950 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/sort/trait.rs
--rw-r--r--   0     1001      127     7521 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/trait.rs
--rw-r--r--   0     1001      127     6273 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/traversal.rs
--rw-r--r--   0     1001      127     1636 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/rtree/util.rs
--rw-r--r--   0     1001      127     1859 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/test/integration.rs
--rw-r--r--   0     1001      127       95 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/test/mod.rs
--rw-r--r--   0     1001      127     3439 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/src/type.rs
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 geoindex_rs-0.1.0/python/Cargo.toml
--rw-r--r--   0     1001      127     3078 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/.gitignore
--rw-r--r--   0     1001      127       64 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/CHANGELOG.md
--rw-r--r--   0     1001      127     1977 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/README.md
--rw-r--r--   0     1001      127       84 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/python/geoindex_rs/__init__.py
--rw-r--r--   0     1001      127     1497 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/python/geoindex_rs/_rust.pyi
--rw-r--r--   0     1001      127      661 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/python/geoindex_rs/enums.py
--rw-r--r--   0     1001      127        0 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/python/geoindex_rs/py.typed
--rw-r--r--   0     1001      127     2892 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/src/kdtree.rs
--rw-r--r--   0     1001      127      373 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/src/lib.rs
--rw-r--r--   0     1001      127     4066 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/src/rtree.rs
--rw-r--r--   0     1001      127    12844 2024-03-29 02:54:21.000000 geoindex_rs-0.1.0/python/Cargo.lock
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 geoindex_rs-0.1.0/pyproject.toml
--rw-r--r--   0     1001      127      661 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/geoindex_rs/enums.py
--rw-r--r--   0     1001      127       84 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/geoindex_rs/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/geoindex_rs/py.typed
--rw-r--r--   0     1001      127     1497 2024-03-29 02:54:17.000000 geoindex_rs-0.1.0/python/geoindex_rs/_rust.pyi
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 geoindex_rs-0.1.0/PKG-INFO
+-rw-r--r--   0     1001      127      894 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/.github/workflows/python-wheels.yml
+-rw-r--r--   0     1001      127      697 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      506 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/.gitignore
+-rw-r--r--   0     1001      127     9723 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/LICENSE_APACHE
+-rw-r--r--   0     1001      127     1068 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/LICENSE_MIT
+-rw-r--r--   0     1001      127     7433 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/README.md
+-rw-r--r--   0     1001      127      147 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/benches/README.md
+-rw-r--r--   0     1001      127      236 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/benches/generate_data.py
+-rw-r--r--   0     1001      127     5443 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/benches/rtree.rs
+-rw-r--r--   0     1001      127     3680 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/fixtures/data1_flatbush_js.raw
+-rw-r--r--   0     1001      127     3200 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/fixtures/data1_input.raw
+-rw-r--r--   0     1001      127      877 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/fixtures/flatbush_generate.js
+-rw-r--r--   0     1001      127     2053 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/fixtures/generate_data.py
+-rw-r--r--   0     1001      127     1185 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/package-lock.json
+-rw-r--r--   0     1001      127      167 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/package.json
+-rw-r--r--   0     1001      127      252 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/error.rs
+-rw-r--r--   0     1001      127     3096 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/indices.rs
+-rw-r--r--   0     1001      127     6819 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/builder.rs
+-rw-r--r--   0     1001      127      161 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/constants.rs
+-rw-r--r--   0     1001      127     3686 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/index.rs
+-rw-r--r--   0     1001      127      248 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/mod.rs
+-rw-r--r--   0     1001      127     6301 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/test.rs
+-rw-r--r--   0     1001      127     5075 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/kdtree/trait.rs
+-rw-r--r--   0     1001      127      220 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/lib.rs
+-rw-r--r--   0     1001      127     7492 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/builder.rs
+-rw-r--r--   0     1001      127       65 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/constants.rs
+-rw-r--r--   0     1001      127     5338 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/index.rs
+-rw-r--r--   0     1001      127      253 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/mod.rs
+-rw-r--r--   0     1001      127     5487 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/sort/hilbert.rs
+-rw-r--r--   0     1001      127      175 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/sort/mod.rs
+-rw-r--r--   0     1001      127     4973 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/sort/str.rs
+-rw-r--r--   0     1001      127      950 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/sort/trait.rs
+-rw-r--r--   0     1001      127     8143 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/trait.rs
+-rw-r--r--   0     1001      127     6273 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/traversal.rs
+-rw-r--r--   0     1001      127     1636 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/rtree/util.rs
+-rw-r--r--   0     1001      127     1939 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/test/integration.rs
+-rw-r--r--   0     1001      127       95 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/test/mod.rs
+-rw-r--r--   0     1001      127     3439 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/src/type.rs
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 geoindex_rs-0.2.0b1/python/Cargo.toml
+-rw-r--r--   0     1001      127     3078 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/.gitignore
+-rw-r--r--   0     1001      127       64 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/CHANGELOG.md
+-rw-r--r--   0     1001      127     2118 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/README.md
+-rw-r--r--   0     1001      127     1106 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/bench.py
+-rw-r--r--   0     1001      127       84 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/python/geoindex_rs/__init__.py
+-rw-r--r--   0     1001      127     1884 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/python/geoindex_rs/_rust.pyi
+-rw-r--r--   0     1001      127      661 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/python/geoindex_rs/enums.py
+-rw-r--r--   0     1001      127        0 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/python/geoindex_rs/py.typed
+-rw-r--r--   0     1001      127     2892 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/src/kdtree.rs
+-rw-r--r--   0     1001      127      373 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/src/lib.rs
+-rw-r--r--   0     1001      127    11219 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/src/rtree.rs
+-rw-r--r--   0     1001      127    12851 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/Cargo.lock
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 geoindex_rs-0.2.0b1/pyproject.toml
+-rw-r--r--   0     1001      127      661 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/geoindex_rs/enums.py
+-rw-r--r--   0     1001      127       84 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/geoindex_rs/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/geoindex_rs/py.typed
+-rw-r--r--   0     1001      127     1884 2024-04-02 15:03:58.000000 geoindex_rs-0.2.0b1/python/geoindex_rs/_rust.pyi
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 geoindex_rs-0.2.0b1/PKG-INFO
```

### Comparing `geoindex_rs-0.1.0/Cargo.toml` & `geoindex_rs-0.2.0b1/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,26 +3,34 @@
 version = "0.1.1"
 authors = ["Kyle Barron <kylebarron2@gmail.com>"]
 edition = "2021"
 rust-version = "1.75"
 license = "MIT OR Apache-2.0"
 repository = "https://github.com/kylebarron/geo-index"
 description = "Fast, static, ABI-stable spatial indexes."
-categories = ["science::geo"]
+keywords = [
+    "rtree",
+    "r-tree",
+    "kdtree",
+    "spatial",
+    "spatial-index",
+    "nearest-neighbor",
+]
+categories = ["data-structures", "algorithms", "science::geo"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 bytemuck = "1"
 float_next_after = "1"
 num-traits = "0.2"
 rayon = { version = "1.8.0", optional = true }
 thiserror = "1"
 tinyvec = { version = "1", features = ["alloc", "rustc_1_40"] }
 
 [dev-dependencies]
 criterion = { version = "0.5", features = ["html_reports"] }
-rstar = "0.11"
+rstar = "0.12"
 
 [[bench]]
 name = "rtree"
 harness = false
```

### Comparing `geoindex_rs-0.1.0/.github/workflows/python-wheels.yml` & `geoindex_rs-0.2.0b1/.github/workflows/python-wheels.yml`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/.github/workflows/test.yml` & `geoindex_rs-0.2.0b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/LICENSE_APACHE` & `geoindex_rs-0.2.0b1/LICENSE_APACHE`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/LICENSE_MIT` & `geoindex_rs-0.2.0b1/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/README.md` & `geoindex_rs-0.2.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # geo-index
 
-[![crates.io version](https://img.shields.io/crates/v/geo-index.svg)](https://crates.io/crates/geo-index)
-[![docs.rs docs](https://docs.rs/geo-index/badge.svg)](https://docs.rs/geo-index)
+[![crates.io version][crates.io_badge]][crates.io_link]
+[![docs.rs docs][docs.rs_badge]][docs.rs_link]
+[![PyPI][pypi_badge]][pypi_link]
+
+[crates.io_badge]: https://img.shields.io/crates/v/geo-index.svg
+[crates.io_link]: https://crates.io/crates/geo-index
+[docs.rs_badge]: https://docs.rs/geo-index/badge.svg
+[docs.rs_link]: https://docs.rs/geo-index
+[pypi_badge]: https://badge.fury.io/py/geoindex-rs.svg
+[pypi_link]: https://pypi.org/project/geoindex-rs/
 
 A Rust crate for packed, static, zero-copy spatial indexes.
 
 ## Features
 
 - **An R-tree and k-d tree written in safe rust.**
 - **Fast.** Because of optimizations available by using static indexes, tends to be faster than dynamic implementations like [`rstar`](https://github.com/georust/rstar).
```

### Comparing `geoindex_rs-0.1.0/benches/rtree.rs` & `geoindex_rs-0.2.0b1/benches/rtree.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/fixtures/data1_flatbush_js.raw` & `geoindex_rs-0.2.0b1/fixtures/data1_flatbush_js.raw`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/fixtures/data1_input.raw` & `geoindex_rs-0.2.0b1/fixtures/data1_input.raw`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/fixtures/flatbush_generate.js` & `geoindex_rs-0.2.0b1/fixtures/flatbush_generate.js`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/fixtures/generate_data.py` & `geoindex_rs-0.2.0b1/fixtures/generate_data.py`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/package-lock.json` & `geoindex_rs-0.2.0b1/package-lock.json`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/indices.rs` & `geoindex_rs-0.2.0b1/src/indices.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/kdtree/builder.rs` & `geoindex_rs-0.2.0b1/src/kdtree/builder.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/kdtree/index.rs` & `geoindex_rs-0.2.0b1/src/kdtree/index.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/kdtree/test.rs` & `geoindex_rs-0.2.0b1/src/kdtree/test.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/kdtree/trait.rs` & `geoindex_rs-0.2.0b1/src/kdtree/trait.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/rtree/builder.rs` & `geoindex_rs-0.2.0b1/src/rtree/builder.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-use std::marker::PhantomData;
-
 use bytemuck::cast_slice_mut;
 
 use crate::indices::MutableIndices;
 use crate::r#type::IndexableNum;
 use crate::rtree::constants::VERSION;
-use crate::rtree::index::OwnedRTree;
+use crate::rtree::index::{OwnedRTree, TreeMetadata};
 use crate::rtree::sort::{Sort, SortParams};
 use crate::rtree::util::compute_num_nodes;
 
 /// A builder to create an [`OwnedRTree`].
 pub struct RTreeBuilder<N: IndexableNum> {
     /// data buffer
     data: Vec<u8>,
@@ -131,21 +129,25 @@
             boxes[self.pos] = self.min_y;
             self.pos += 1;
             boxes[self.pos] = self.max_x;
             self.pos += 1;
             boxes[self.pos] = self.max_y;
             self.pos += 1;
 
+            let metadata = unsafe {
+                TreeMetadata::new_unchecked(
+                    self.node_size,
+                    self.num_items,
+                    self.num_nodes,
+                    self.level_bounds,
+                )
+            };
             return OwnedRTree {
                 buffer: self.data,
-                node_size: self.node_size,
-                num_items: self.num_items,
-                num_nodes: self.num_nodes,
-                level_bounds: self.level_bounds,
-                phantom: PhantomData,
+                metadata,
             };
         }
 
         let mut sort_params = SortParams {
             num_items: self.num_items,
             node_size: self.node_size,
             min_x: self.min_x,
@@ -204,21 +206,25 @@
                     self.pos += 1;
                     boxes[self.pos] = node_max_y;
                     self.pos += 1;
                 }
             }
         }
 
+        let metadata = unsafe {
+            TreeMetadata::new_unchecked(
+                self.node_size,
+                self.num_items,
+                self.num_nodes,
+                self.level_bounds,
+            )
+        };
         OwnedRTree {
             buffer: self.data,
-            node_size: self.node_size,
-            num_items: self.num_items,
-            num_nodes: self.num_nodes,
-            level_bounds: self.level_bounds,
-            phantom: PhantomData,
+            metadata,
         }
     }
 }
 
 /// Mutable borrow of boxes and indices
 fn split_data_borrow<N: IndexableNum>(
     data: &mut [u8],
```

### Comparing `geoindex_rs-0.1.0/src/rtree/sort/hilbert.rs` & `geoindex_rs-0.2.0b1/src/rtree/sort/hilbert.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/rtree/sort/str.rs` & `geoindex_rs-0.2.0b1/src/rtree/sort/str.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/rtree/sort/trait.rs` & `geoindex_rs-0.2.0b1/src/rtree/sort/trait.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/rtree/trait.rs` & `geoindex_rs-0.2.0b1/src/rtree/trait.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,58 @@
-use std::borrow::Cow;
-
-use bytemuck::cast_slice;
-
+use crate::error::Result;
 use crate::indices::Indices;
 use crate::r#type::IndexableNum;
 use crate::rtree::index::{OwnedRTree, RTreeRef};
 use crate::rtree::traversal::{IntersectionIterator, Node};
+use crate::GeoIndexError;
 
 pub trait RTreeIndex<N: IndexableNum>: Sized {
     /// A slice representing all the bounding boxes of all elements contained within this tree,
     /// including the bounding boxes of each internal node.
     fn boxes(&self) -> &[N];
 
     /// A slice representing the indices within the `boxes` slice, including internal nodes.
-    fn indices(&self) -> Cow<'_, Indices>;
+    fn indices(&self) -> Indices;
 
     /// The total number of items contained in this RTree.
     fn num_items(&self) -> usize;
 
     /// The total number of nodes in this RTree, including both leaf and intermediate nodes.
     fn num_nodes(&self) -> usize;
 
     /// The maximum number of elements in each node.
     fn node_size(&self) -> usize;
+
+    /// The offsets into [RTreeIndex::boxes] where each level's boxes starts and ends. The tree is
+    /// laid out bottom-up, and there's an implicit initial 0. So the boxes of the lowest level of
+    /// the tree are located from `boxes[0..self.level_bounds()[0]]`.
     fn level_bounds(&self) -> &[usize];
 
+    /// The number of levels (height) of the tree.
+    fn num_levels(&self) -> usize {
+        self.level_bounds().len()
+    }
+
+    /// The tree is laid out from bottom to top. Level 0 is the _base_ of the tree. Each integer
+    /// higher is one level higher of the tree.
+    fn boxes_at_level(&self, level: usize) -> Result<&[N]> {
+        let level_bounds = self.level_bounds();
+        if level >= level_bounds.len() {
+            return Err(GeoIndexError::General("Level out of bounds".to_string()));
+        }
+        let result = if level == 0 {
+            &self.boxes()[0..level_bounds[0]]
+        } else if level == level_bounds.len() {
+            &self.boxes()[level_bounds[level]..]
+        } else {
+            &self.boxes()[level_bounds[level - 1]..level_bounds[level]]
+        };
+        Ok(result)
+    }
+
     /// Search an RTree given the provided bounding box.
     ///
     /// Results are the indexes of the inserted objects in insertion order.
     fn search(&self, min_x: N, min_y: N, max_x: N, max_y: N) -> Vec<usize> {
         let boxes = self.boxes();
         let indices = self.indices();
 
@@ -122,71 +146,61 @@
     fn root(&self) -> Node<'_, N, Self> {
         Node::from_root(self)
     }
 }
 
 impl<N: IndexableNum> RTreeIndex<N> for OwnedRTree<N> {
     fn boxes(&self) -> &[N] {
-        let data = &self.buffer;
-
-        let nodes_byte_length = self.num_nodes * 4 * N::BYTES_PER_ELEMENT;
-        cast_slice(&data[8..8 + nodes_byte_length])
+        self.metadata.boxes_slice(&self.buffer)
     }
 
-    fn indices(&self) -> Cow<'_, Indices> {
-        let data = &self.buffer;
-
-        let indices_bytes_per_element = if self.num_nodes < 16384 { 2 } else { 4 };
-        let nodes_byte_length = self.num_nodes * 4 * N::BYTES_PER_ELEMENT;
-        let indices_byte_length = self.num_nodes * indices_bytes_per_element;
-        let indices_buf = &data[8 + nodes_byte_length..8 + nodes_byte_length + indices_byte_length];
-
-        Cow::Owned(Indices::new(indices_buf, self.num_nodes()))
+    fn indices(&self) -> Indices {
+        self.metadata.indices_slice(&self.buffer)
     }
 
     fn num_nodes(&self) -> usize {
-        self.num_nodes
+        self.metadata.num_nodes
     }
 
     fn level_bounds(&self) -> &[usize] {
-        &self.level_bounds
+        &self.metadata.level_bounds
     }
 
     fn node_size(&self) -> usize {
-        self.node_size
+        self.metadata.node_size
     }
 
     fn num_items(&self) -> usize {
-        self.num_items
+        self.metadata.num_items
     }
 }
 
 impl<N: IndexableNum> RTreeIndex<N> for RTreeRef<'_, N> {
     fn boxes(&self) -> &[N] {
         self.boxes
     }
 
-    fn indices(&self) -> Cow<'_, Indices> {
-        Cow::Borrowed(&self.indices)
+    fn indices(&self) -> Indices {
+        self.indices
     }
 
     fn level_bounds(&self) -> &[usize] {
-        &self.level_bounds
+        &self.metadata.level_bounds
     }
 
     fn node_size(&self) -> usize {
-        self.node_size
+        self.metadata.node_size
     }
 
     fn num_items(&self) -> usize {
-        self.num_items
+        self.metadata.num_items
     }
 
     fn num_nodes(&self) -> usize {
-        self.num_nodes
+        self.metadata.num_nodes
     }
 }
 
 /// Binary search for the first value in the array bigger than the given.
 #[inline]
 fn upper_bound(value: usize, arr: &[usize]) -> usize {
     let mut i = 0;
```

### Comparing `geoindex_rs-0.1.0/src/rtree/traversal.rs` & `geoindex_rs-0.2.0b1/src/rtree/traversal.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/rtree/util.rs` & `geoindex_rs-0.2.0b1/src/rtree/util.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/src/test/integration.rs` & `geoindex_rs-0.2.0b1/src/test/integration.rs`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,22 @@
         rs_buf[0..header_byte_length],
         "should have same header bytes"
     );
 
     let js_flatbush = RTreeRef::<f64>::try_new(&js_buf).unwrap();
     let rs_flatbush = RTreeRef::<f64>::try_new(&rs_buf).unwrap();
 
-    assert_eq!(js_flatbush.num_items, rs_flatbush.num_items);
-    assert_eq!(js_flatbush.node_size, rs_flatbush.node_size);
+    assert_eq!(
+        js_flatbush.metadata.num_items,
+        rs_flatbush.metadata.num_items
+    );
+    assert_eq!(
+        js_flatbush.metadata.node_size,
+        rs_flatbush.metadata.node_size
+    );
 }
 
 pub(crate) fn flatbush_js_test_data() -> Vec<f64> {
     let buffer = read("fixtures/data1_input.raw").unwrap();
     let boxes_buf: &[f64] = cast_slice(&buffer);
     boxes_buf.to_vec()
 }
```

### Comparing `geoindex_rs-0.1.0/src/type.rs` & `geoindex_rs-0.2.0b1/src/type.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/python/Cargo.toml` & `geoindex_rs-0.2.0b1/python/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "geoindex-rs"
-version = "0.1.0"
+version = "0.2.0-beta.1"
 authors = ["Kyle Barron <kylebarron2@gmail.com>"]
 edition = "2021"
 description = "Fast, memory-efficient 2D spatial indexes for Python."
 readme = "README.md"
 repository = "https://github.com/kylebarron/geo-index"
 license = "MIT OR Apache-2.0"
 keywords = ["python", "geospatial"]
@@ -18,7 +18,11 @@
 
 [dependencies]
 bytes = "1"
 geo-index = { path = "../", features = ["rayon"] }
 numpy = "0.20"
 pyo3 = { version = "0.20", features = ["abi3-py38"] }
 thiserror = "1"
+
+[profile.release]
+lto = true
+codegen-units = 1
```

### Comparing `geoindex_rs-0.1.0/python/.gitignore` & `geoindex_rs-0.2.0b1/python/.gitignore`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/python/README.md` & `geoindex_rs-0.2.0b1/python/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # geoindex-rs
 
+[![PyPI][pypi_badge]][pypi_link]
+
+[pypi_badge]: https://badge.fury.io/py/geoindex-rs.svg
+[pypi_link]: https://pypi.org/project/geoindex-rs/
+
 Fast, memory-efficient 2D spatial indexes for Python.
 
 ## API
 
 ### `KDTree`
 
 #### `KDTree.from_interleaved`
```

### Comparing `geoindex_rs-0.1.0/python/python/geoindex_rs/enums.py` & `geoindex_rs-0.2.0b1/python/python/geoindex_rs/enums.py`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/python/src/kdtree.rs` & `geoindex_rs-0.2.0b1/python/src/kdtree.rs`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/python/Cargo.lock` & `geoindex_rs-0.2.0b1/python/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
  "rayon",
  "thiserror",
  "tinyvec",
 ]
 
 [[package]]
 name = "geoindex-rs"
-version = "0.1.0"
+version = "0.2.0-beta.1"
 dependencies = [
  "bytes",
  "geo-index",
  "numpy",
  "pyo3",
  "thiserror",
 ]
@@ -361,17 +361,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `geoindex_rs-0.1.0/python/geoindex_rs/enums.py` & `geoindex_rs-0.2.0b1/python/geoindex_rs/enums.py`

 * *Files identical despite different names*

### Comparing `geoindex_rs-0.1.0/PKG-INFO` & `geoindex_rs-0.2.0b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.3
 Name: geoindex-rs
-Version: 0.1.0
+Version: 0.2.0b1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Fast, memory-efficient 2D spatial indexes for Python.
 Keywords: python,geospatial
 Author: Kyle Barron <kylebarron2@gmail.com>
 Author-email: Kyle Barron <kylebarron2@gmail.com>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/kylebarron/geo-index
 
 # geoindex-rs
 
+[![PyPI][pypi_badge]][pypi_link]
+
+[pypi_badge]: https://badge.fury.io/py/geoindex-rs.svg
+[pypi_link]: https://pypi.org/project/geoindex-rs/
+
 Fast, memory-efficient 2D spatial indexes for Python.
 
 ## API
 
 ### `KDTree`
 
 #### `KDTree.from_interleaved`
```

