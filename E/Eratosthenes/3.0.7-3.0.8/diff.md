# Comparing `tmp/Eratosthenes-3.0.7.tar.gz` & `tmp/Eratosthenes-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eratosthenes-3.0.7.tar", last modified: Mon Apr  1 14:08:01 2024, max compression
+gzip compressed data, was "Eratosthenes-3.0.8.tar", last modified: Mon Apr  1 15:33:19 2024, max compression
```

## Comparing `Eratosthenes-3.0.7.tar` & `Eratosthenes-3.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/Eratosthenes.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-04-01 14:08:01.000000 Eratosthenes-3.0.7/Eratosthenes.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.7/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.7/MANIFEST.in
--rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.7/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-04-01 14:07:19.000000 Eratosthenes-3.0.7/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/src/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-04-01 14:02:53.000000 Eratosthenes-3.0.7/src/dispatchqueue.cpp
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 14:08:01.949711 Eratosthenes-3.0.7/src/include/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.7/src/include/config.h
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.7/src/include/dispatchqueue.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3651 2024-03-30 20:24:43.000000 Eratosthenes-3.0.7/src/include/prime_generator.hpp
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    14917 2024-04-01 14:06:17.000000 Eratosthenes-3.0.7/src/prime_gen.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/Eratosthenes.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      305 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       13 2024-04-01 15:33:19.000000 Eratosthenes-3.0.8/Eratosthenes.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2024-03-26 16:40:08.000000 Eratosthenes-3.0.8/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       19 2024-03-26 17:27:20.000000 Eratosthenes-3.0.8/MANIFEST.in
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     1550 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      814 2024-03-29 23:46:05.000000 Eratosthenes-3.0.8/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1318 2024-04-01 15:32:22.000000 Eratosthenes-3.0.8/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/src/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2895 2024-04-01 14:02:53.000000 Eratosthenes-3.0.8/src/dispatchqueue.cpp
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-04-01 15:33:19.440287 Eratosthenes-3.0.8/src/include/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      767 2024-03-26 15:47:52.000000 Eratosthenes-3.0.8/src/include/config.h
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1941 2024-03-30 14:18:47.000000 Eratosthenes-3.0.8/src/include/dispatchqueue.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3460 2024-04-01 15:30:54.000000 Eratosthenes-3.0.8/src/include/prime_generator.hpp
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    15188 2024-04-01 15:29:56.000000 Eratosthenes-3.0.8/src/prime_gen.cpp
```

### Comparing `Eratosthenes-3.0.7/Eratosthenes.egg-info/PKG-INFO` & `Eratosthenes-3.0.8/Eratosthenes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.7
+Version: 3.0.8
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.7/LICENSE` & `Eratosthenes-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.7/PKG-INFO` & `Eratosthenes-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eratosthenes
-Version: 3.0.7
+Version: 3.0.8
 Summary: Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division
 Home-page: https://github.com/vm6502q/Eratosthenes
 Author: Dan Strano
 Author-email: dan@unitary.fund
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `Eratosthenes-3.0.7/README.md` & `Eratosthenes-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.7/setup.py` & `Eratosthenes-3.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         language='c++',
         extra_compile_args = cpp_args,
     ),
 ]
 
 setup(
     name='Eratosthenes',
-    version='3.0.7',
+    version='3.0.8',
     author='Dan Strano',
     author_email='dan@unitary.fund',
     description='Fast prime generation for Python based on Sieve of Eratosthenes and Trial Division',
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/vm6502q/Eratosthenes",
     license="MIT",
```

### Comparing `Eratosthenes-3.0.7/src/dispatchqueue.cpp` & `Eratosthenes-3.0.8/src/dispatchqueue.cpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.7/src/include/config.h` & `Eratosthenes-3.0.8/src/include/config.h`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.7/src/include/dispatchqueue.hpp` & `Eratosthenes-3.0.8/src/include/dispatchqueue.hpp`

 * *Files identical despite different names*

### Comparing `Eratosthenes-3.0.7/src/include/prime_generator.hpp` & `Eratosthenes-3.0.8/src/include/prime_generator.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -53,28 +53,19 @@
             end = mid - 1U;
         }
     } while (start <= end);
 
     return ans;
 }
 
-inline BigInteger forward2(const size_t& p) {
-    // Make this NOT a multiple of 2.
-    return (p << 1U) - 1U;
-}
-
 inline BigInteger forward(const size_t& p) {
     // Make this NOT a multiple of 2 or 3.
     return (p << 1U) + (~(~p | 1U)) - 1U;
 }
 
-inline size_t backward2(const BigInteger& p) {
-    return (p + 1U) >> 1U;
-}
-
 inline size_t backward(const BigInteger& n) {
     return ((~(~n | 1U)) / 3U) + 1U;
 }
 
 inline size_t backward5(const BigInteger& n) {
     return (((((n + 1U) << 2U) / 5U + 1U) << 1U) / 3U + 1U) >> 1U;
 }
```

### Comparing `Eratosthenes-3.0.7/src/prime_gen.cpp` & `Eratosthenes-3.0.8/src/prime_gen.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -272,48 +272,51 @@
     // Assume the L1/L2 cache limit is 2048 KB.
     // We save half our necessary bytes by
     // removing multiples of 2.
     // The simple sieve removes multiples of 2, 3, and 5.
     // limit = 2048 KB = 2097152 B,
     // limit_segmented = limit * 2
     // limit_simple = ((((limit * 2) * 3) / 2) * 5) / 4
-    constexpr size_t limit = 4194304ULL;
+    constexpr size_t limit = 6291456ULL;
     constexpr size_t limit_simple = 31457281ULL;
 
     if (!(n & 1U)) {
         --n;
     }
+    if ((n % 3U) == 0) {
+        n -= 2U;
+    }
     if (limit_simple >= n) {
         return SieveOfEratosthenes(n);
     }
     std::vector<BigInteger> knownPrimes = SieveOfEratosthenes(limit_simple);
     knownPrimes.reserve(std::expint(log(n)) - std::expint(log(2)));
 
     // Divide the range in different segments
-    const size_t nCardinality = backward2(n);
-    size_t low = backward2(limit_simple);
+    const size_t nCardinality = backward(n);
+    size_t low = backward(limit_simple);
     size_t high = low + limit;
 
     // Process one segment at a time till we pass n.
     while (low < nCardinality)
     {
         if (high > nCardinality) {
            high = nCardinality;
         }
 
-        const BigInteger fLo = forward2(low);
+        const BigInteger fLo = forward(low);
         const size_t sqrtIndex = std::distance(
             knownPrimes.begin(),
-            std::upper_bound(knownPrimes.begin(), knownPrimes.end(), sqrt(forward2(high)) + 1U)
+            std::upper_bound(knownPrimes.begin(), knownPrimes.end(), sqrt(forward(high)) + 1U)
         );
 
         const size_t cardinality = high - low;
         bool notPrime[cardinality + 1U] = { false };
 
-        for (size_t k = 1U; k < sqrtIndex; ++k) {
+        for (size_t k = 2U; k < sqrtIndex; ++k) {
             const BigInteger& p = knownPrimes[k];
             dispatch.dispatch([&fLo, &low, &cardinality, p, &notPrime]() {
                 // We are skipping multiples of 2.
                 const BigInteger p2 = p << 1U;
 
                 // Find the minimum number in [low..high] that is
                 // a multiple of prime[i] (divisible by prime[i])
@@ -324,31 +327,33 @@
                     i += p;
                 }
                 if ((i & 1U) == 0U) {
                     i += p;
                 }
 
                 for (;;) {
-                    const size_t o = backward2(i) - low;
+                    const size_t o = backward(i) - low;
                     if (o > cardinality) {
                         return false;
                     }
-                    notPrime[o] = true;
+                    if (i % 3U) {
+                        notPrime[o] = true;
+                    }
                     i += p2;
                 }
 
                 return false;
             });
         }
         dispatch.finish();
 
         // Numbers which are not marked are prime
         for (size_t o = 1U; o <= cardinality; ++o) {
             if (!notPrime[o]) {
-                knownPrimes.push_back(forward2(o + low));
+                knownPrimes.push_back(forward(o + low));
             }
         }
 
         // Update low and high for next segment
         low = low + limit;
         high = low + limit;
     }
@@ -360,56 +365,62 @@
 {
     // TODO: This should scale to the system.
     // Assume the L1/L2 cache limit is 2048 KB.
     // We save half our necessary bytes by
     // removing multiples of 2.
     // The simple sieve removes multiples of 2, 3, and 5.
     // limit = 2048 KB = 2097152 B,
-    // limit_segmented = limit * 2
+    // limit_segmented = ((limit * 2) * 3) / 2
     // limit_simple = ((((limit * 2) * 3) / 2) * 5) / 4
-    constexpr size_t limit = 4194304ULL;
+    constexpr size_t limit = 6291456ULL;
     constexpr size_t limit_simple = 31457281ULL;
 
     if (!(n & 1U)) {
         --n;
     }
+    if ((n % 3U) == 0) {
+        n -= 2U;
+    }
     if (limit_simple >= n) {
         return CountPrimesTo(n);
     }
-    const BigInteger sqrtnp1 = sqrt(n) + 1U;
-    const BigInteger practicalLimit = ((sqrtnp1 < limit_simple) ? sqrtnp1 : limit_simple) | 1U;
+    BigInteger sqrtnp1 = (sqrt(n) + 1U) | 1U;
+    if ((sqrtnp1 % 3U) == 0U) {
+        sqrtnp1 += 2U;
+    }
+    const BigInteger practicalLimit = (sqrtnp1 < limit_simple) ? sqrtnp1 : limit_simple;
     std::vector<BigInteger> knownPrimes = SieveOfEratosthenes(practicalLimit);
     if (practicalLimit < sqrtnp1) {
         knownPrimes.reserve(std::expint(log(sqrtnp1)) - std::expint(log(2)));
     }
     size_t count = knownPrimes.size();
 
     // Divide the range in different segments
-    const size_t nCardinality = backward2(n);
-    size_t low = backward2(practicalLimit);
+    const size_t nCardinality = backward(n);
+    size_t low = backward(practicalLimit);
     size_t high = low + limit;
 
     // Process one segment at a time till we pass n.
     while (low < nCardinality)
     {
         if (high > nCardinality) {
            high = nCardinality;
         }
-        const BigInteger fLo = forward2(low);
+        const BigInteger fLo = forward(low);
         const size_t sqrtIndex = std::distance(
             knownPrimes.begin(),
-            std::upper_bound(knownPrimes.begin(), knownPrimes.end(), sqrt(forward2(high)) + 1U)
+            std::upper_bound(knownPrimes.begin(), knownPrimes.end(), sqrt(forward(high)) + 1U)
         );
 
         const size_t cardinality = high - low;
         bool notPrime[cardinality + 1U] = { false };
 
         // Use the primes found by the simple sieve
         // to find primes in current range
-        for (size_t k = 1U; k < sqrtIndex; ++k) {
+        for (size_t k = 2U; k < sqrtIndex; ++k) {
             const BigInteger& p = knownPrimes[k];
             dispatch.dispatch([&fLo, &low, &cardinality, p, &notPrime]() {
                 // We are skipping multiples of 2.
                 const BigInteger p2 = p << 1U;
 
                 // Find the minimum number in [low..high] that is
                 // a multiple of prime[i] (divisible by prime[i])
@@ -420,19 +431,21 @@
                     i += p;
                 }
                 if ((i & 1U) == 0U) {
                     i += p;
                 }
 
                 for (;;) {
-                    const size_t o = backward2(i) - low;
+                    const size_t o = backward(i) - low;
                     if (o > cardinality) {
                         return false;
                     }
-                    notPrime[o] = true;
+                    if (i % 3U) {
+                        notPrime[o] = true;
+                    }
                     i += p2;
                 }
 
                 return false;
             });
         }
         dispatch.finish();
@@ -442,15 +455,15 @@
                 if (!notPrime[o]) {
                     ++count;
                 }
             }
         } else {
             for (size_t o = 1U; o <= cardinality; ++o) {
                 if (!notPrime[o]) {
-                    const BigInteger p = forward2(o + low);
+                    const BigInteger p = forward(o + low);
                     if (p <= sqrtnp1) {
                         knownPrimes.push_back(p);
                     }
                     ++count;
                 }
             }
         }
```

