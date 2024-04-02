# Comparing `tmp/rython_calc-0.4.0.tar.gz` & `tmp/rython_calc-0.4.1.tar.gz`

## Comparing `rython_calc-0.4.0.tar` & `rython_calc-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.0/Cargo.toml
--rw-r--r--   0     1001      127     3584 2024-03-31 12:18:30.000000 rython_calc-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-03-31 12:18:30.000000 rython_calc-0.4.0/.gitignore
--rw-r--r--   0     1001      127     1075 2024-03-31 12:18:30.000000 rython_calc-0.4.0/LICENSE
--rw-r--r--   0     1001      127      603 2024-03-31 12:18:30.000000 rython_calc-0.4.0/README.md
--rw-r--r--   0     1001      127    10298 2024-03-31 12:18:30.000000 rython_calc-0.4.0/poetry.lock
--rw-r--r--   0     1001      127        0 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/cli/__init__.py
--rw-r--r--   0     1001      127     1735 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/rython/py.typed
--rw-r--r--   0     1001      127      666 2024-03-31 12:18:30.000000 rython_calc-0.4.0/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     2724 2024-03-31 12:18:30.000000 rython_calc-0.4.0/src/lib.rs
--rw-r--r--   0     1001      127     7857 2024-03-31 12:18:30.000000 rython_calc-0.4.0/Cargo.lock
--rw-r--r--   0     1001      127     1041 2024-03-31 12:18:30.000000 rython_calc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 rython_calc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.1/Cargo.toml
+-rw-r--r--   0     1001      127     3584 2024-04-02 19:58:30.000000 rython_calc-0.4.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-02 19:58:30.000000 rython_calc-0.4.1/.gitignore
+-rw-r--r--   0     1001      127     1075 2024-04-02 19:58:30.000000 rython_calc-0.4.1/LICENSE
+-rw-r--r--   0     1001      127      603 2024-04-02 19:58:30.000000 rython_calc-0.4.1/README.md
+-rw-r--r--   0     1001      127    10298 2024-04-02 19:58:30.000000 rython_calc-0.4.1/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1743 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/py.typed
+-rw-r--r--   0     1001      127      666 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     2924 2024-04-02 19:58:30.000000 rython_calc-0.4.1/src/lib.rs
+-rw-r--r--   0     1001      127      347 2024-04-02 19:58:30.000000 rython_calc-0.4.1/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127     7857 2024-04-02 19:58:30.000000 rython_calc-0.4.1/Cargo.lock
+-rw-r--r--   0     1001      127     1041 2024-04-02 19:58:30.000000 rython_calc-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 rython_calc-0.4.1/PKG-INFO
```

### Comparing `rython_calc-0.4.0/.github/workflows/CI.yml` & `rython_calc-0.4.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/.gitignore` & `rython_calc-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/LICENSE` & `rython_calc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/README.md` & `rython_calc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/poetry.lock` & `rython_calc-0.4.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/python/cli/main.py` & `rython_calc-0.4.1/python/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     for i in range(NUMBER_OF_LOOPS):
         base_int += 0
         base_int *= 1
     t2_stop = perf_counter()
     print(f"Loop time for python int basic methods add and mul: {t2_stop - t2_start}")
 
     t3_start = perf_counter()
-    new_int: rython_calc.NewInt = rython_calc.NewInt(1)
-    new_int.loop_add_mul_seq(NUMBER_OF_LOOPS, 0, 1)
+    new_int_2: rython_calc.NewInt = rython_calc.NewInt(1)
+    new_int_2.loop_add_mul_seq(NUMBER_OF_LOOPS, 0, 1)
     t3_stop = perf_counter()
     print(f"Loop time for NewInt method with loop in rust: {t3_stop - t3_start}")
 
     t4_start = perf_counter()
     new_float: rython_calc.NewFloat = rython_calc.NewFloat(1.0)
     for i in range(NUMBER_OF_LOOPS):
         new_float.add(0.0)
@@ -39,11 +39,11 @@
     for i in range(NUMBER_OF_LOOPS):
         base_float += 0.0
         base_float *= 1.0
     t5_stop = perf_counter()
     print(f"Loop time for python float basic methods add and mul: {t5_stop - t5_start}")
 
     t6_start = perf_counter()
-    new_float: rython_calc.NewFloat = rython_calc.NewFloat(1.0)
-    new_float.loop_add_mul_seq(NUMBER_OF_LOOPS, 0.0, 1.0)
+    new_float_2: rython_calc.NewFloat = rython_calc.NewFloat(1.0)
+    new_float_2.loop_add_mul_seq(NUMBER_OF_LOOPS, 0.0, 1.0)
     t6_stop = perf_counter()
     print(f"Loop time for NewFloat method with loop in rust: {t6_stop - t6_start}")
```

### Comparing `rython_calc-0.4.0/python/rython/rython_calc.pyi` & `rython_calc-0.4.1/python/rython/rython_calc.pyi`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.0/src/lib.rs` & `rython_calc-0.4.1/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 use pyo3::prelude::*;
 
 #[pyclass(module = "calc")]
 struct NewInt {
     number: i32,
 }
 
+fn wrap(obj: &Bound<'_, PyAny>) -> PyResult<i32> {
+    let val = obj.call_method1("__and__", (0xFFFFFFFF_u32,))?;
+    let val: u32 = val.extract()?;
+    Ok(val as i32)
+}
+
 #[pymethods]
 impl NewInt {
     #[new]
     #[pyo3(text_signature = "(number: int) -> None")]
-    fn new(number: i32) -> Self {
+    fn new(#[pyo3(from_py_with = "wrap")] number: i32) -> Self {
         Self { number }
     }
 
     #[pyo3(text_signature = "($self, second_number: int) -> int")]
     fn mul(&mut self, second_number: i32) -> PyResult<i32> {
         self.number = self.number.wrapping_mul(second_number);
         Ok(self.number)
@@ -83,13 +89,13 @@
 #[pyfunction]
 #[pyo3(text_signature = "(a: int, b: int) -> str")]
 fn sum_as_string(a: usize, b: usize) -> PyResult<String> {
     Ok((a + b).to_string())
 }
 
 #[pymodule]
-fn rython_calc(_py: Python, m: &PyModule) -> PyResult<()> {
+fn rython_calc(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<NewInt>()?;
     m.add_class::<NewFloat>()?;
     m.add_function(wrap_pyfunction!(sum_as_string, m)?)?;
     Ok(())
 }
```

### Comparing `rython_calc-0.4.0/Cargo.lock` & `rython_calc-0.4.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -99,17 +99,17 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -117,49 +117,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -180,15 +180,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rython"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
```

### Comparing `rython_calc-0.4.0/pyproject.toml` & `rython_calc-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rython-calc"
-version = "0.4.0"
+version = "0.4.1"
 description = "Rython package to test python and rust compatibility"
 authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 mypy = "^1.9.0"
```

### Comparing `rython_calc-0.4.0/PKG-INFO` & `rython_calc-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

