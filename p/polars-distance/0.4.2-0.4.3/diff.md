# Comparing `tmp/polars_distance-0.4.2.tar.gz` & `tmp/polars_distance-0.4.3.tar.gz`

## Comparing `polars_distance-0.4.2.tar` & `polars_distance-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 polars_distance-0.4.2/Cargo.toml
--rw-r--r--   0     1001      127      945 2024-03-24 00:04:35.000000 polars_distance-0.4.2/Makefile
--rw-r--r--   0     1001      127     1221 2024-03-24 00:04:35.000000 polars_distance-0.4.2/README.md
--rw-r--r--   0     1001      127    13935 2024-03-24 00:04:35.000000 polars_distance-0.4.2/polars_distance/__init__.py
--rw-r--r--   0     1001      127       17 2024-03-24 00:04:35.000000 polars_distance-0.4.2/polars_distance/_internal.pyi
--rw-r--r--   0     1001      127        0 2024-03-24 00:04:35.000000 polars_distance-0.4.2/polars_distance/py.typed
--rw-r--r--   0     1001      127      158 2024-03-24 00:04:35.000000 polars_distance-0.4.2/requirements.txt
--rw-r--r--   0     1001      127     7066 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/array.rs
--rw-r--r--   0     1001      127    17822 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/expressions.rs
--rw-r--r--   0     1001      127      412 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/lib.rs
--rw-r--r--   0     1001      127     8993 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/list.rs
--rw-r--r--   0     1001      127     1656 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/other_dist.rs
--rw-r--r--   0     1001      127     2317 2024-03-24 00:04:35.000000 polars_distance-0.4.2/src/string.rs
--rw-r--r--   0     1001      127     6382 2024-03-24 00:04:35.000000 polars_distance-0.4.2/tests/test_distance_arr.py
--rw-r--r--   0     1001      127    47565 2024-03-24 00:04:40.000000 polars_distance-0.4.2/Cargo.lock
--rw-r--r--   0     1001      127      887 2024-03-24 00:04:35.000000 polars_distance-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 polars_distance-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 polars_distance-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      127      945 2024-04-02 09:23:31.000000 polars_distance-0.4.3/Makefile
+-rw-r--r--   0     1001      127     1221 2024-04-02 09:23:31.000000 polars_distance-0.4.3/README.md
+-rw-r--r--   0     1001      127    14269 2024-04-02 09:23:31.000000 polars_distance-0.4.3/polars_distance/__init__.py
+-rw-r--r--   0     1001      127       17 2024-04-02 09:23:31.000000 polars_distance-0.4.3/polars_distance/_internal.pyi
+-rw-r--r--   0     1001      127        0 2024-04-02 09:23:31.000000 polars_distance-0.4.3/polars_distance/py.typed
+-rw-r--r--   0     1001      127      158 2024-04-02 09:23:31.000000 polars_distance-0.4.3/requirements.txt
+-rw-r--r--   0     1001      127     7066 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/array.rs
+-rw-r--r--   0     1001      127    18327 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/expressions.rs
+-rw-r--r--   0     1001      127      412 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      127     8993 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/list.rs
+-rw-r--r--   0     1001      127     1656 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/other_dist.rs
+-rw-r--r--   0     1001      127     2444 2024-04-02 09:23:31.000000 polars_distance-0.4.3/src/string.rs
+-rw-r--r--   0     1001      127     6690 2024-04-02 09:23:31.000000 polars_distance-0.4.3/tests/test_distance_arr.py
+-rw-r--r--   0     1001      127    47826 2024-04-02 09:23:38.000000 polars_distance-0.4.3/Cargo.lock
+-rw-r--r--   0     1001      127      887 2024-04-02 09:23:31.000000 polars_distance-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 polars_distance-0.4.3/PKG-INFO
```

### Comparing `polars_distance-0.4.2/Cargo.toml` & `polars_distance-0.4.3/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_distance"
-version = "0.4.2"
+version = "0.4.3"
 edition = "2021"
 
 [lib]
 name = "polars_distance"
 crate-type = ["cdylib"]
 
 [dependencies]
@@ -12,14 +12,15 @@
 polars-core = {version = "0.38.3"}
 polars-arrow = {version = "0.38.3"}
 pyo3 = { version = "0.20.3", features = ["extension-module", "abi3-py38"] }
 pyo3-polars = { version = "0.12", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
 distances = { version = "1.6.3"}
 rapidfuzz = { version = "0.5.0"}
+gestalt_ratio = { version = "0.2.1"}
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"] }
 
 [profile.release]
 opt-level = 3
 codegen-units = 1
```

### Comparing `polars_distance-0.4.2/Makefile` & `polars_distance-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/README.md` & `polars_distance-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/polars_distance/__init__.py` & `polars_distance-0.4.3/polars_distance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,23 @@
             return register_plugin_function(
                 plugin_path=Path(__file__).parent,
                 args=[self._expr, other],
                 function_name="prefix_str",
                 is_elementwise=True,
             )
 
+    def gestalt_ratio(self, other: IntoExpr) -> pl.Expr:
+        """Returns gestalt ratio between two expressions"""
+        return register_plugin_function(
+            plugin_path=Path(__file__).parent,
+            args=[self._expr, other],
+            function_name="gestalt_ratio_str",
+            is_elementwise=True,
+        )
+
 
 @pl.api.register_expr_namespace("dist_list")
 class DistancePairWiseList:
     def __init__(self, expr: pl.Expr):
         self._expr = expr
 
     def jaccard_index(self, other: IntoExpr) -> pl.Expr:
```

### Comparing `polars_distance-0.4.2/src/array.rs` & `polars_distance-0.4.3/src/array.rs`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/src/expressions.rs` & `polars_distance-0.4.3/src/expressions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 };
 use crate::other_dist::haversine_dist;
 use crate::string::{
     dam_levenshtein_dist, dam_levenshtein_normalized_dist, hamming_dist, hamming_normalized_dist,
     indel_dist, indel_normalized_dist, jaro_dist, jaro_winkler_dist, lcs_seq_dist,
     lcs_seq_normalized_dist, levenshtein_dist, levenshtein_normalized_dist, osa_dist,
     osa_normalized_dist, postfix_dist, postfix_normalized_dist, prefix_dist,
-    prefix_normalized_dist,
+    prefix_normalized_dist, gestalt_ratio
 };
 use distances::vectors::{bray_curtis, canberra, chebyshev, l3_norm, l4_norm, manhattan};
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
 
 #[derive(Deserialize)]
@@ -459,7 +459,19 @@
             let y_lat = y_lat.f64().unwrap();
             let y_long = y_long.f64().unwrap();
             haversine_dist(x_lat, x_long, y_lat, y_long, kwargs.unit)?.into_series()
         }
         _ => unimplemented!(),
     })
 }
+
+#[polars_expr(output_type=Float64)]
+fn gestalt_ratio_str(inputs: &[Series]) -> PolarsResult<Series> {
+    if inputs[0].dtype() != &DataType::String || inputs[1].dtype() != &DataType::String {
+        polars_bail!(InvalidOperation: "Gestalt ratio distance works only on Utf8 types. Please cast to Utf8 first.");
+    }
+    let x = inputs[0].str()?;
+    let y = inputs[1].str()?;
+
+    let out: Float64Chunked = arity::binary_elementwise_values(x, y, gestalt_ratio);
+    Ok(out.into_series())
+}
```

### Comparing `polars_distance-0.4.2/src/list.rs` & `polars_distance-0.4.3/src/list.rs`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/src/other_dist.rs` & `polars_distance-0.4.3/src/other_dist.rs`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/src/string.rs` & `polars_distance-0.4.3/src/string.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use rapidfuzz::distance::*;
+use gestalt_ratio::gestalt_ratio as _gestalt_ratio;
 
 // HAMMING
 pub fn hamming_dist(x: &str, y: &str) -> u32 {
     let result =
         hamming::distance_with_args(x.chars(), y.chars(), &hamming::Args::default().pad(true))
             as u32;
     dbg!(result.clone());
@@ -85,7 +86,11 @@
 pub fn prefix_dist(x: &str, y: &str) -> u32 {
     prefix::distance(x.chars(), y.chars()) as u32
 }
 
 pub fn prefix_normalized_dist(x: &str, y: &str) -> f64 {
     prefix::normalized_distance(x.chars(), y.chars())
 }
+
+pub fn gestalt_ratio(x: &str, y: &str) -> f64 {
+    _gestalt_ratio(x, y)
+}
```

### Comparing `polars_distance-0.4.2/tests/test_distance_arr.py` & `polars_distance-0.4.3/tests/test_distance_arr.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,7 +263,21 @@
     expected = pl.DataFrame(
         [
             pl.Series("haversine", [value], dtype=pl.Float64),
         ]
     )
 
     assert_frame_equal(result, expected)
+
+
+def test_gestalt(data):
+    result = data.select(
+        pld.col("str_l").dist_str.gestalt_ratio(pld.col("str_r")).alias("dist_gestalt")
+    )
+
+    expected = pl.DataFrame(
+        [
+            pl.Series("dist_gestalt", [0.8], dtype=pl.Float64),
+        ]
+    )
+
+    assert_frame_equal(result, expected)
```

### Comparing `polars_distance-0.4.2/Cargo.lock` & `polars_distance-0.4.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -118,15 +118,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -151,17 +151,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "windows-targets 0.52.4",
 ]
 
@@ -289,22 +289,22 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -330,14 +330,23 @@
 [[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
+name = "gestalt_ratio"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6b3c399c9a90b4de1792c277efc74b451ddeb4c2cfc11ac0b2f0503918f48ed"
+dependencies = [
+ "unicode-segmentation",
+]
+
+[[package]]
 name = "getrandom"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "js-sys",
@@ -427,17 +436,17 @@
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "itoap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9028f49264629065d057f340a86acb84867925865f73bbf8d47b4d149a7e88b8"
 
@@ -525,32 +534,32 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.4"
@@ -1078,17 +1087,18 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_distance"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "distances",
+ "gestalt_ratio",
  "jemallocator",
  "polars",
  "polars-arrow",
  "polars-core",
  "pyo3",
  "pyo3-polars",
  "rapidfuzz",
@@ -1159,28 +1169,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pyo3-polars"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
@@ -1203,15 +1213,15 @@
 checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -1272,17 +1282,17 @@
 checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1324,17 +1334,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
@@ -1382,22 +1392,22 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1477,15 +1487,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1493,17 +1503,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1545,15 +1555,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -1623,15 +1633,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1645,15 +1655,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1843,37 +1853,37 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `polars_distance-0.4.2/pyproject.toml` & `polars_distance-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_distance-0.4.2/PKG-INFO` & `polars_distance-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-distance
-Version: 0.4.2
+Version: 0.4.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Summary: Polars plugin for pairwise distance functions
 Author-email: Ion Koutsours <15728914+ion-elgreco@users.noreply.github.com>
 Requires-Python: >=3.8
```

