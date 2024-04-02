# Comparing `tmp/krabby-0.1.8.tar.gz` & `tmp/krabby-0.1.9.tar.gz`

## Comparing `krabby-0.1.8.tar` & `krabby-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 krabby-0.1.8/Cargo.toml
--rw-r--r--   0      501       20     3526 2024-03-31 08:30:15.000000 krabby-0.1.8/.github/workflows/CI.yml
--rw-r--r--   0      501       20      702 2024-03-31 10:19:15.000000 krabby-0.1.8/.gitignore
--rw-r--r--   0      501       20      323 2024-03-31 09:57:07.000000 krabby-0.1.8/README.md
--rw-r--r--   0      501       20     1105 2024-03-31 15:40:10.000000 krabby-0.1.8/krabby.pyi
--rw-r--r--   0      501       20     4627 2024-03-31 16:30:19.000000 krabby-0.1.8/src/flashtext/keyword_processor.rs
--rw-r--r--   0      501       20       95 2024-03-31 09:31:20.000000 krabby-0.1.8/src/flashtext/mod.rs
--rw-r--r--   0      501       20     3281 2024-03-31 15:17:48.000000 krabby-0.1.8/src/lib.rs
--rw-r--r--   0      501       20      118 2024-03-31 08:34:49.000000 krabby-0.1.8/src/trie/mod.rs
--rw-r--r--   0      501       20      916 2024-03-31 09:31:07.000000 krabby-0.1.8/src/trie/node.rs
--rw-r--r--   0      501       20      319 2024-03-31 08:34:49.000000 krabby-0.1.8/src/trie/span.rs
--rw-r--r--   0      501       20     8035 2024-03-31 15:00:41.000000 krabby-0.1.8/src/trie/trie.rs
--rw-r--r--   0      501       20     7857 2024-03-31 16:31:28.000000 krabby-0.1.8/Cargo.lock
--rw-r--r--   0      501       20      442 2024-03-31 10:01:38.000000 krabby-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 krabby-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 krabby-0.1.9/Cargo.toml
+-rw-r--r--   0      501       20     3526 2024-03-31 08:30:15.000000 krabby-0.1.9/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      702 2024-03-31 10:19:15.000000 krabby-0.1.9/.gitignore
+-rw-r--r--   0      501       20      323 2024-03-31 09:57:07.000000 krabby-0.1.9/README.md
+-rw-r--r--   0      501       20     1105 2024-03-31 15:40:10.000000 krabby-0.1.9/krabby.pyi
+-rw-r--r--   0      501       20     4052 2024-04-01 00:27:56.000000 krabby-0.1.9/src/flashtext/keyword_processor.rs
+-rw-r--r--   0      501       20       95 2024-03-31 09:31:20.000000 krabby-0.1.9/src/flashtext/mod.rs
+-rw-r--r--   0      501       20     3309 2024-04-01 04:49:58.000000 krabby-0.1.9/src/lib.rs
+-rw-r--r--   0      501       20      118 2024-03-31 08:34:49.000000 krabby-0.1.9/src/trie/mod.rs
+-rw-r--r--   0      501       20      916 2024-03-31 09:31:07.000000 krabby-0.1.9/src/trie/node.rs
+-rw-r--r--   0      501       20      319 2024-03-31 08:34:49.000000 krabby-0.1.9/src/trie/span.rs
+-rw-r--r--   0      501       20     8035 2024-03-31 15:00:41.000000 krabby-0.1.9/src/trie/trie.rs
+-rw-r--r--   0      501       20     7857 2024-04-01 04:50:33.000000 krabby-0.1.9/Cargo.lock
+-rw-r--r--   0      501       20      442 2024-03-31 10:01:38.000000 krabby-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 krabby-0.1.9/PKG-INFO
```

### Comparing `krabby-0.1.8/.github/workflows/CI.yml` & `krabby-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `krabby-0.1.8/.gitignore` & `krabby-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `krabby-0.1.8/krabby.pyi` & `krabby-0.1.9/krabby.pyi`

 * *Files identical despite different names*

### Comparing `krabby-0.1.8/src/flashtext/keyword_processor.rs` & `krabby-0.1.9/src/flashtext/keyword_processor.rs`

 * *Files 17% similar despite different names*

```diff
@@ -24,40 +24,34 @@
             boundary: match boundary {
                 "" => None,
                 _ => Some(boundary.chars().collect()),
             },
         }
     }
 
+    fn normalize(&self, keyword: &str) -> String {
+        if self.case_sensitive {
+            return keyword.to_string();
+        }
+        return keyword.to_lowercase();
+    }
+
     pub fn put(&mut self, keyword: &str) {
-        let key = if !self.case_sensitive {
-            keyword.to_lowercase()
-        } else {
-            keyword.to_string()
-        };
-        // let mut key: Vec<char> = keyword.chars().collect();
-        // if !self.case_sensitive {
-        //     key = key.iter().map(|c| c.to_lowercase()).collect();
-        // }
+        let key = self.normalize(keyword);
 
-        // let key_str: String = key.iter().collect();
         if self.keywords.contains_key(&key) {
             return;
         }
 
         self.trie.put(&key.chars().collect(), true);
         self.keywords.insert(key, keyword.to_string());
     }
 
     pub fn pop(&mut self, keyword: &str) {
-        let key = if !self.case_sensitive {
-            keyword.to_lowercase()
-        } else {
-            keyword.to_string()
-        };
+        let key = self.normalize(keyword);
 
         if !self.keywords.contains_key(&key) {
             return;
         }
 
         self.keywords.remove(&key);
         self.trie.pop(&key.chars().collect(), true);
@@ -65,19 +59,15 @@
 
     pub fn get_keywords(&self) -> Vec<String> {
         self.keywords.values().map(|v| v.clone()).collect()
     }
 
     pub fn extract(&self, text: &str) -> Vec<Span<usize, String>> {
         let spans: Vec<Span<usize, Vec<char>>>;
-        let target: Vec<char> = if !self.case_sensitive {
-            text.to_lowercase().chars().collect()
-        } else {
-            text.chars().collect()
-        };
+        let target: Vec<char> = self.normalize(text).chars().collect();
 
         match self.boundary {
             Some(ref b) => {
                 spans = self.trie.extract(&target, true, Some(b));
             }
             None => {
                 spans = self.trie.extract(&target, true, None);
@@ -97,24 +87,20 @@
             .collect();
     }
 
     pub fn replace(&self, text: &str, repl: &HashMap<&str, &str>, default: Option<&str>) -> String {
         let repl: HashMap<String, String> = {
             let mut r = HashMap::new();
             for (k, v) in repl.iter() {
-                let k: String = if !self.case_sensitive {
-                    k.to_lowercase()
-                } else {
-                    k.to_string()
-                };
+                let k: String = self.normalize(k);
                 r.insert(k, v.to_string());
             }
             r
         };
-        
+
         let spans = self.extract(text);
         let mut result = String::new();
         let mut last_end = 0;
         let indices: Vec<usize> = text.char_indices().map(|(i, _)| i).collect();
 
         for span in spans {
             let start = indices[span.start];
@@ -149,16 +135,11 @@
             result.push_str(&text[last_end..]);
         }
 
         return result;
     }
 
     pub fn has(&self, keyword: &str) -> bool {
-        let target: String = if !self.case_sensitive {
-            keyword.to_lowercase()
-        } else {
-            keyword.to_string()
-        };
-
+        let target: String = self.normalize(keyword);
         self.keywords.contains_key(&target)
     }
 }
```

### Comparing `krabby-0.1.8/src/lib.rs` & `krabby-0.1.9/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -134,10 +134,11 @@
         self.core.has(keyword)
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn krabby(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add_class::<Span>()?;
     m.add_class::<KeywordProcessor>()?;
     Ok(())
 }
```

### Comparing `krabby-0.1.8/src/trie/node.rs` & `krabby-0.1.9/src/trie/node.rs`

 * *Files identical despite different names*

### Comparing `krabby-0.1.8/src/trie/trie.rs` & `krabby-0.1.9/src/trie/trie.rs`

 * *Files identical despite different names*

### Comparing `krabby-0.1.8/Cargo.lock` & `krabby-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "krabby"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.153"
```

### Comparing `krabby-0.1.8/PKG-INFO` & `krabby-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: krabby
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A Flashtext library for Python by Rust
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

