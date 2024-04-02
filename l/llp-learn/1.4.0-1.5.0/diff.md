# Comparing `tmp/llp_learn-1.4.0.tar.gz` & `tmp/llp_learn-1.5.0.tar.gz`

## Comparing `llp_learn-1.4.0.tar` & `llp_learn-1.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.4.0/mkdocs.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.4.0/docs/index.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.4.0/docs/reference.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/__about__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/base.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/alter/__init__.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/alter/_base.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/alter/_classes.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/dllp/__init__.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/dllp/_classes.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/dllp/_loaders.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/em/__init__.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/em/_classes.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpfc/__init__.py
--rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpfc/_classes.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpfc/_loaders.py
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpfc/_make_groups.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpvat/__init__.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpvat/_classes.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpvat/_loaders.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/llpvat/_vat_loss.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/mixbag/__init__.py
--rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/mixbag/_classes.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/mixbag/_loaders.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/mixbag/_losses.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/model_selection/__init__.py
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/model_selection/_search.py
--rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/model_selection/_split.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/util/__init__.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 llp_learn-1.4.0/src/llp_learn/util/_util.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 llp_learn-1.4.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 llp_learn-1.4.0/README.md
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 llp_learn-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 llp_learn-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.5.0/docs/index.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.5.0/docs/reference.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/__about__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/base.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/alter/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/alter/_base.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/alter/_classes.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/dllp/__init__.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/dllp/_classes.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/dllp/_loaders.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/em/__init__.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/em/_classes.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpfc/__init__.py
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpfc/_classes.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpfc/_loaders.py
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpfc/_make_groups.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpvat/__init__.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpvat/_classes.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpvat/_loaders.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/llpvat/_vat_loss.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/mixbag/__init__.py
+-rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/mixbag/_classes.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/mixbag/_loaders.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/mixbag/_losses.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/model_selection/__init__.py
+-rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/model_selection/_search.py
+-rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/model_selection/_split.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/util/__init__.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 llp_learn-1.5.0/src/llp_learn/util/_util.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 llp_learn-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 llp_learn-1.5.0/README.md
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 llp_learn-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 llp_learn-1.5.0/PKG-INFO
```

### Comparing `llp_learn-1.4.0/src/llp_learn/base.py` & `llp_learn-1.5.0/src/llp_learn/base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/alter/_base.py` & `llp_learn-1.5.0/src/llp_learn/alter/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/alter/_classes.py` & `llp_learn-1.5.0/src/llp_learn/alter/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/dllp/_classes.py` & `llp_learn-1.5.0/src/llp_learn/dllp/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/dllp/_loaders.py` & `llp_learn-1.5.0/src/llp_learn/dllp/_loaders.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/em/_classes.py` & `llp_learn-1.5.0/src/llp_learn/em/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpfc/_classes.py` & `llp_learn-1.5.0/src/llp_learn/llpfc/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpfc/_loaders.py` & `llp_learn-1.5.0/src/llp_learn/llpfc/_loaders.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpfc/_make_groups.py` & `llp_learn-1.5.0/src/llp_learn/llpfc/_make_groups.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpvat/_classes.py` & `llp_learn-1.5.0/src/llp_learn/llpvat/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpvat/_loaders.py` & `llp_learn-1.5.0/src/llp_learn/llpvat/_loaders.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/llpvat/_vat_loss.py` & `llp_learn-1.5.0/src/llp_learn/llpvat/_vat_loss.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/mixbag/_classes.py` & `llp_learn-1.5.0/src/llp_learn/mixbag/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/mixbag/_loaders.py` & `llp_learn-1.5.0/src/llp_learn/mixbag/_loaders.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/mixbag/_losses.py` & `llp_learn-1.5.0/src/llp_learn/mixbag/_losses.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/model_selection/_search.py` & `llp_learn-1.5.0/src/llp_learn/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/src/llp_learn/model_selection/_split.py` & `llp_learn-1.5.0/src/llp_learn/model_selection/_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,15 +426,15 @@
             f_plus = np.zeros(self.n_splits, dtype=int)
             folds = defaultdict(set)
 
             # Creating the folds
             while len(assigned_bags) != num_bags:
                 f = np.argmin(f_sizes)
                 f_p = f_plus[f] / f_sizes[f] if f_sizes[f] != 0 else 0.0
-                if f_p >= p_plus:
+                if f_p <= p_plus:
                     c = (m_plus ** 2) / m_plus_squared_sum
                 else:
                     c = (m_minus ** 2) / m_minus_squared_sum
 
                 c[assigned_bags] = 0
 
                 b = random.choice(bag_list, size = 1, replace = False, p = c)[0]
@@ -454,20 +454,22 @@
             folds = defaultdict(set)
 
             # Creating the folds
             while len(assigned_bags) != num_bags:
                 f = np.argmin(np.sum(f_sizes, axis=1))
                 c = m + f_sizes[f]
                 c_prop = c / np.sum(c, axis=1).reshape(-1, 1)
-                c_norm = np.linalg.norm(c_prop - global_prop, axis=1)     
-                b = np.argsort(c_norm) # sort values by norm
-                b = b[~np.in1d(b, assigned_bags)][0] # filter assigned bags and select the bag
+                c_dist = np.linalg.norm(c_prop - global_prop, axis=1)
+                c_dist = np.exp(-c_dist)
+                c_probs = c_dist / np.sum(c_dist[np.setdiff1d(bag_list, assigned_bags)])
+                c_probs[assigned_bags] = 0
+                b = random.choice(bag_list, size = 1, replace = False, p = c_probs)[0]
                 folds[f].add(b)
                 assigned_bags.append(b)
-                f_sizes[f] += m[b]
+                f_sizes[f] += m[b]  
 
         # Generating the train/test indexes
         for i in range(self.n_splits):
             bags_test = list(folds[i])
             test_index = np.where(np.isin(bags, bags_test))[0]
             train_index = np.setdiff1d(np.array(range(len(bags))), test_index)
```

### Comparing `llp_learn-1.4.0/src/llp_learn/util/_util.py` & `llp_learn-1.5.0/src/llp_learn/util/_util.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/.gitignore` & `llp_learn-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/LICENSE.txt` & `llp_learn-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/README.md` & `llp_learn-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/pyproject.toml` & `llp_learn-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llp_learn-1.4.0/PKG-INFO` & `llp_learn-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llp-learn
-Version: 1.4.0
+Version: 1.5.0
 Summary: Learning from Label Proportions (LLP) methods in Python
 Project-URL: Documentation, https://github.com/gaabrielfranco/llp-learn#readme
 Project-URL: Issues, https://github.com/gaabrielfranco/llp-learn/issues
 Project-URL: Source, https://github.com/gaabrielfranco/llp-learn
 Author-email: Gabriel Franco <gvfranco@bu.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
```

