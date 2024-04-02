# Comparing `tmp/ccsds-0.1.0b3.tar.gz` & `tmp/ccsds-0.1.0b4.tar.gz`

## Comparing `ccsds-0.1.0b3.tar` & `ccsds-0.1.0b4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 ccsds-0.1.0b3/Cargo.toml
--rw-rw----   0     1000     1000       79 2024-01-28 20:54:27.000000 ccsds-0.1.0b3/.gitattributes
--rw-rw-r--   0     1000     1000     2825 2024-01-27 02:47:54.000000 ccsds-0.1.0b3/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      705 2024-04-01 20:19:08.000000 ccsds-0.1.0b3/.gitignore
--rw-rw-r--   0     1000     1000    35149 2024-01-27 23:15:56.000000 ccsds-0.1.0b3/LICENSE.txt
--rw-rw-r--   0     1000     1000      671 2024-04-01 20:18:47.000000 ccsds-0.1.0b3/README.md
--rw-rw-r--   0     1000     1000     1340 2024-04-01 15:04:02.000000 ccsds-0.1.0b3/ccsds.pyi
--rw-rw-r--   0     1000     1000    19393 2024-04-01 19:42:56.000000 ccsds-0.1.0b3/src/lib.rs
--rw-rw-r--   0     1000     1000    66560 2024-01-28 20:53:44.000000 ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.dat
--rw-r--r--   0     1000     1000     1696 2024-01-29 15:20:40.000000 ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.txt
--rw-rw-r--   0     1000     1000      522 2024-01-29 19:03:20.000000 ccsds-0.1.0b3/tests/test.py
--rw-rw-r--   0     1000     1000    23562 2024-04-01 20:22:27.000000 ccsds-0.1.0b3/Cargo.lock
--rw-rw-r--   0     1000     1000      438 2024-01-29 19:12:16.000000 ccsds-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 ccsds-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 ccsds-0.1.0b4/Cargo.toml
+-rw-rw----   0     1000     1000       79 2024-01-28 20:54:27.000000 ccsds-0.1.0b4/.gitattributes
+-rw-rw-r--   0     1000     1000     2825 2024-01-27 02:47:54.000000 ccsds-0.1.0b4/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      705 2024-04-01 20:19:08.000000 ccsds-0.1.0b4/.gitignore
+-rw-rw-r--   0     1000     1000    35149 2024-01-27 23:15:56.000000 ccsds-0.1.0b4/LICENSE.txt
+-rw-rw-r--   0     1000     1000      671 2024-04-01 20:18:47.000000 ccsds-0.1.0b4/README.md
+-rw-rw-r--   0     1000     1000     1340 2024-04-01 15:04:02.000000 ccsds-0.1.0b4/ccsds.pyi
+-rw-rw-r--   0     1000     1000    20078 2024-04-02 16:52:25.000000 ccsds-0.1.0b4/src/lib.rs
+-rw-rw-r--   0     1000     1000    66560 2024-01-28 20:53:44.000000 ccsds-0.1.0b4/tests/fixtures/snpp_synchronized_cadus.dat
+-rw-r--r--   0     1000     1000     1696 2024-01-29 15:20:40.000000 ccsds-0.1.0b4/tests/fixtures/snpp_synchronized_cadus.txt
+-rw-rw-r--   0     1000     1000      522 2024-01-29 19:03:20.000000 ccsds-0.1.0b4/tests/test.py
+-rw-rw-r--   0     1000     1000    23524 2024-04-02 16:54:13.000000 ccsds-0.1.0b4/Cargo.lock
+-rw-rw-r--   0     1000     1000      438 2024-01-29 19:12:16.000000 ccsds-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 ccsds-0.1.0b4/PKG-INFO
```

### Comparing `ccsds-0.1.0b3/Cargo.toml` & `ccsds-0.1.0b4/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ccsds"
-version = "0.1.0-beta.3"
+version = "0.1.0-beta.4"
 authors = ["Bruce Flynn <brucef@ssec.wisc.edu>"]
 edition = "2021"
 description = "CCSDS spacecraft data stream decoding"
 keywords = ["ccsds", "spacepacket", "framing", "cadu"]
 categories = ["aerospace::space-protocols"]
 license-file = "LICENSE.txt"
 repository = "https://github.com/bmflynn/ccsdspy"
@@ -12,9 +12,9 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ccsds"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.19.2", features = ["extension-module", "abi3-py37"] }
-ccsds = "^0.1.0-beta.3"
+ccsds = "^0.1.0-beta.4"
 spacecrafts = "^0.1.0-beta.3"
```

### Comparing `ccsds-0.1.0b3/.github/workflows/CI.yml` & `ccsds-0.1.0b4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/.gitignore` & `ccsds-0.1.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/LICENSE.txt` & `ccsds-0.1.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/README.md` & `ccsds-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/ccsds.pyi` & `ccsds-0.1.0b4/ccsds.pyi`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/src/lib.rs` & `ccsds-0.1.0b4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,15 @@
     if let Some(interleave) = interleave {
         if !(2..=10).contains(&interleave) {
             return Err(PyValueError::new_err(format!(
                 "improbable interleave value; expected 2..10: got {interleave}"
             )));
         }
         let interleave: u8 = interleave.try_into().unwrap(); // checked above
-        builder = builder.reed_solomon_interleave(interleave);
+        builder = builder.reed_solomon(interleave);
     }
 
     let frames = builder.build().start(blocks).filter_map(Result::ok);
 
     Ok(FrameIterator {
         frames: Box::new(frames),
     })
@@ -473,15 +473,15 @@
     if let Some(interleave) = interleave {
         if !(2..=10).contains(&interleave) {
             return Err(PyValueError::new_err(
                 "invalid interleave value; expected 2..10: got {interleave}",
             ));
         }
         let interleave: u8 = interleave.try_into().unwrap(); // checked above
-        builder = builder.reed_solomon_interleave(interleave);
+        builder = builder.reed_solomon(interleave);
     }
     let frames = builder.build().start(blocks).filter_map(Result::ok);
 
     let packets: Box<dyn Iterator<Item = ccsds::DecodedPacket> + Send + 'static> = Box::new(
         ccsds::decode_framed_packets(scid, frames, izone_len, trailer_len),
     );
 
@@ -531,18 +531,17 @@
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct PnConfig;
 
 impl PnConfig {
     fn new(config: Option<spacecrafts::PnConfig>) -> Option<Self> {
-        match config {
-            Some(_) => Some(Self {}),
-            None => None,
-        }
+        config.map(|_| {
+            Self{}
+        })
     }
 }
 
 #[pymethods]
 impl PnConfig {
     fn __repr__(&self) -> String {
         self.__str__()
@@ -574,22 +573,21 @@
             self.interleave, self.virtual_fill_length, self.num_correctable
         )
     }
 }
 
 impl RSConfig {
     fn new(config: Option<spacecrafts::RSConfig>) -> Option<Self> {
-        match config {
-            Some(rs) => Some(Self {
+        config.map(|rs| {
+            RSConfig {
                 interleave: rs.interleave,
                 virtual_fill_length: rs.virtual_fill_length,
                 num_correctable: rs.num_correctable,
-            }),
-            None => None,
-        }
+            }
+        })
     }
 }
 
 #[pyclass]
 #[derive(Clone, Debug)]
 pub struct FramingConfig {
     #[pyo3(get)]
@@ -630,23 +628,43 @@
             Some(rs) => rs.__str__(),
             None => "None".to_string(),
         };
         format!("FramingConfig(length={}, insert_zone_length={}, trailer_length={}, pseudo_noise={}, reed_solomon={})",
         self.length, self.insert_zone_length, self.trailer_length, pn, rs).to_string()
     }
 
-    /// Length of the RS codeblock.
+    /// Return the computed length of a CADU block, i.e., CADU length - ASM length, from 
+    /// our config.
     pub fn codeblock_len(&self) -> usize {
         match &self.reed_solomon {
             Some(rs) => self.length + 2 * rs.num_correctable as usize * rs.interleave as usize,
             None => self.length,
         }
     }
 }
 
+/// Lookup the FramingConfig for a spacecraft.
+///
+/// This makes use of a spacecraftsdb formatted database file. See the releases at 
+/// https://github.com/bmflynn/spacecraftsdb to download a database file.
+///
+/// Parameters
+/// ----------
+/// scid : int
+///     The spacecraft identifier for a spacecraft.
+///
+/// path : str, optional
+///     Local path to a specific spacecraftsdb database file. If not provided this will 
+///     attempt to load the database from ./spacecraftsdb.json,
+///     $XDG_DATA_HOME/spacecraftsdb/spacecraftsdb.json, ~/.spacecraftsdb.json.
+///
+/// Returns
+/// -------
+/// FramingConfig or None
+///     The configuration for the specified spacecraft if available, otherwise `None`
 #[pyfunction]
 fn framing_config(scid: u16, path: Option<&str>) -> PyResult<Option<FramingConfig>> {
     match ccsds::framing_config(scid, path) {
         Ok(Some(framing)) => Ok(Some(FramingConfig::new(framing))),
         Ok(None) => Ok(None),
         Err(err) => Err(PyFileNotFoundError::new_err(format!("{err}"))),
     }
```

### Comparing `ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.dat` & `ccsds-0.1.0b4/tests/fixtures/snpp_synchronized_cadus.dat`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.txt` & `ccsds-0.1.0b4/tests/fixtures/snpp_synchronized_cadus.txt`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/tests/test.py` & `ccsds-0.1.0b4/tests/test.py`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0b3/Cargo.lock` & `ccsds-0.1.0b4/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 name = "anyhow"
 version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -39,41 +39,38 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "ccsds"
-version = "0.1.0-beta.3"
+version = "0.1.0-beta.4"
 dependencies = [
- "ccsds 0.1.0-beta.3 (registry+https://github.com/rust-lang/crates.io-index)",
+ "ccsds 0.1.0-beta.4 (registry+https://github.com/rust-lang/crates.io-index)",
  "pyo3",
  "spacecrafts",
 ]
 
 [[package]]
 name = "ccsds"
-version = "0.1.0-beta.3"
+version = "0.1.0-beta.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0c2f521790a26fed2945439b2cc67cb4f950f4b0f3293c0e1bdfce36d4a9a17"
+checksum = "18335d66745b42f8a5a3f2e8225986110c50ebe19b0ad503d05c237703f5fd78"
 dependencies = [
  "chrono",
  "crossbeam",
  "ndarray",
  "rayon",
  "rs2",
  "serde",
@@ -88,25 +85,25 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.33"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f13690e35a5e4ace198e7beea2895d29f3a9cc55015fcebe6336bd2010af9eb"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -186,40 +183,40 @@
  "option-ext",
  "redox_users",
  "windows-sys",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "getrandom"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.4"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.59"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6a67363e2aa4443928ce15e57ebae94fd8949958fd1223c4cfc0cd473ad7539"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -238,32 +235,32 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.67"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libredox"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
@@ -279,33 +276,33 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "matrixmultiply"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
 dependencies = [
  "autocfg",
  "rawpointer",
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
 name = "ndarray"
 version = "0.15.6"
@@ -317,36 +314,35 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -396,17 +392,17 @@
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.2"
@@ -480,17 +476,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -526,60 +522,60 @@
 name = "rs2"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44b2e9b1a862d7e012298e5f24642050cc205e973bce20a656befe95d8c4a0d3"
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "spacecrafts"
 version = "0.1.0-beta.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e58f5eaffcab38b70cdd65f05b3bf0e781d3947ba0fae71fd1e934fd00366a8a"
 dependencies = [
@@ -598,47 +594,47 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
@@ -662,15 +658,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -694,73 +690,73 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -781,103 +777,103 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
```

### Comparing `ccsds-0.1.0b3/PKG-INFO` & `ccsds-0.1.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ccsds
-Version: 0.1.0b3
+Version: 0.1.0b4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pytest ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE.txt
```

