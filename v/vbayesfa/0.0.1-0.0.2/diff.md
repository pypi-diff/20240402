# Comparing `tmp/vbayesfa-0.0.1.tar.gz` & `tmp/vbayesfa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbayesfa-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vbayesfa-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vbayesfa-0.0.1.tar` & `vbayesfa-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      233 2023-12-05 19:19:59.509576 vbayesfa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-12-05 19:21:23.883136 vbayesfa-0.0.1/src/vbayesfa/.DS_Store
--rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.1/src/vbayesfa/__init__.py
--rw-r--r--   0        0        0     5210 2023-11-08 19:35:39.865262 vbayesfa-0.0.1/src/vbayesfa/bayes_factors.py
--rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.1/src/vbayesfa/discrete_finite.py
--rw-r--r--   0        0        0    12636 2023-11-08 19:32:20.917698 vbayesfa-0.0.1/src/vbayesfa/exp_families.py
--rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.1/src/vbayesfa/fit_ibp.py
--rw-r--r--   0        0        0     4834 2023-11-07 21:00:14.535873 vbayesfa-0.0.1/src/vbayesfa/fit_lpa.py
--rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.1/src/vbayesfa/full_discrete_finite.py
--rw-r--r--   0        0        0      995 2023-08-28 16:38:09.224634 vbayesfa-0.0.1/src/vbayesfa/linear_regression.py
--rw-r--r--   0        0        0    30724 2023-12-01 16:21:31.441127 vbayesfa-0.0.1/src/vbayesfa/lpa.py
--rw-r--r--   0        0        0    15256 2023-12-01 16:11:38.061451 vbayesfa-0.0.1/src/vbayesfa/lpa_outcome_analysis.py
--rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.1/src/vbayesfa/make_sim_data.py
--rw-r--r--   0        0        0    11261 2023-07-05 16:08:39.229965 vbayesfa-0.0.1/src/vbayesfa/sparse_cont_finite.py
--rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.1/src/vbayesfa/sparse_pos_cont_finite.py
--rw-r--r--   0        0        0      179 1970-01-01 00:00:00.000000 vbayesfa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      233 2024-04-02 17:04:30.623992 vbayesfa-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-01-31 17:01:44.847879 vbayesfa-0.0.2/src/vbayesfa/.DS_Store
+-rw-r--r--   0        0        0       69 2023-12-05 19:18:02.101247 vbayesfa-0.0.2/src/vbayesfa/__init__.py
+-rw-r--r--   0        0        0    16507 2024-03-11 15:13:41.467877 vbayesfa-0.0.2/src/vbayesfa/bayes_factors.py
+-rw-r--r--   0        0        0    28671 2024-03-14 18:29:17.477573 vbayesfa-0.0.2/src/vbayesfa/exp_families.py
+-rw-r--r--   0        0        0     5207 2024-02-27 14:40:09.708047 vbayesfa-0.0.2/src/vbayesfa/fit_lpa.py
+-rw-r--r--   0        0        0     9420 2023-07-05 21:34:32.174051 vbayesfa-0.0.2/src/vbayesfa/ibp/discrete_finite.py
+-rw-r--r--   0        0        0     3726 2023-06-16 14:40:29.441517 vbayesfa-0.0.2/src/vbayesfa/ibp/fit_ibp.py
+-rw-r--r--   0        0        0     9770 2023-07-05 21:33:47.123462 vbayesfa-0.0.2/src/vbayesfa/ibp/full_discrete_finite.py
+-rw-r--r--   0        0        0     3164 2023-05-25 19:01:25.945355 vbayesfa-0.0.2/src/vbayesfa/ibp/make_sim_data.py
+-rw-r--r--   0        0        0    11261 2023-07-05 16:08:39.229965 vbayesfa-0.0.2/src/vbayesfa/ibp/sparse_cont_finite.py
+-rw-r--r--   0        0        0    16282 2023-07-05 21:31:30.740293 vbayesfa-0.0.2/src/vbayesfa/ibp/sparse_pos_cont_finite.py
+-rw-r--r--   0        0        0    35324 2024-02-01 16:54:29.814042 vbayesfa-0.0.2/src/vbayesfa/lpa.py
+-rw-r--r--   0        0        0    20925 2024-04-01 20:20:16.509148 vbayesfa-0.0.2/src/vbayesfa/lpa_outcome_analysis.py
+-rw-r--r--   0        0        0     8745 2024-04-01 16:49:52.674660 vbayesfa-0.0.2/src/vbayesfa/simulate_data.py
+-rw-r--r--   0        0        0     6148 2024-01-30 20:49:54.836172 vbayesfa-0.0.2/src/vbayesfa/tests/.DS_Store
+-rw-r--r--   0        0        0     5776 2024-02-29 18:02:24.703820 vbayesfa-0.0.2/src/vbayesfa/tests/test_exp_families.py
+-rw-r--r--   0        0        0     1625 2024-03-11 14:40:52.003495 vbayesfa-0.0.2/src/vbayesfa/tests/test_lpa.py
+-rw-r--r--   0        0        0     2147 2024-03-11 15:41:20.385592 vbayesfa-0.0.2/src/vbayesfa/tests/test_lpa_outcome_analysis.py
+-rw-r--r--   0        0        0      179 1970-01-01 00:00:00.000000 vbayesfa-0.0.2/PKG-INFO
```

### Comparing `vbayesfa-0.0.1/src/vbayesfa/.DS_Store` & `vbayesfa-0.0.2/src/vbayesfa/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -76,47 +76,47 @@
 000004b0: 0000 0008 4ec3 4fc4 1b17 c541 0000 0012  ....N.O....A....
 000004c0: 002e 0069 0070 0079 006e 0062 005f 0063  ...i.p.y.n.b._.c
 000004d0: 0068 0065 0063 006b 0070 006f 0069 006e  .h.e.c.k.p.o.i.n
 000004e0: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
 000004f0: 0000 0000 0000 000b 005f 005f 0069 006e  ........._._.i.n
 00000500: 0069 0074 005f 005f 002e 0070 0079 496c  .i.t._._...p.yIl
 00000510: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
-00000520: 002e ffff ffff ffff 0000 0000 0012 0064  ...............d
-00000530: 0069 0073 0063 0072 0065 0074 0065 005f  .i.s.c.r.e.t.e._
-00000540: 0066 0069 006e 0069 0074 0065 002e 0070  .f.i.n.i.t.e...p
-00000550: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
-00000560: 018b 0000 002e ffff ffff ffff 0000 0000  ................
-00000570: 000a 0066 0069 0074 005f 0069 0062 0070  ...f.i.t._.i.b.p
-00000580: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
-00000590: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
-000005a0: 0000 0000 000a 0066 0069 0074 005f 006c  .......f.i.t._.l
-000005b0: 0070 0061 002e 0070 0079 496c 6f63 626c  .p.a...p.yIlocbl
-000005c0: 6f62 0000 0010 0000 0267 0000 002e ffff  ob.......g......
-000005d0: ffff ffff 0000 0000 0017 0066 0075 006c  ...........f.u.l
-000005e0: 006c 005f 0064 0069 0073 0063 0072 0065  .l._.d.i.s.c.r.e
-000005f0: 0074 0065 005f 0066 0069 006e 0069 0074  .t.e._.f.i.n.i.t
-00000600: 0065 002e 0070 0079 496c 6f63 626c 6f62  .e...p.yIlocblob
-00000610: 0000 0010 0000 02d5 0000 002e ffff ffff  ................
-00000620: ffff 0000 0000 0006 006c 0070 0061 002e  .........l.p.a..
-00000630: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
-00000640: 0000 011d 0000 009e ffff ffff ffff 0000  ................
-00000650: 0000 0010 006d 0061 006b 0065 005f 0073  .....m.a.k.e._.s
-00000660: 0069 006d 005f 0064 0061 0074 0061 002e  .i.m._.d.a.t.a..
-00000670: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
-00000680: 0000 018b 0000 009e ffff ffff ffff 0000  ................
-00000690: 0000 0015 0073 0070 0061 0072 0073 0065  .....s.p.a.r.s.e
-000006a0: 005f 0063 006f 006e 0074 005f 0066 0069  ._.c.o.n.t._.f.i
-000006b0: 006e 0069 0074 0065 002e 0070 0079 496c  .n.i.t.e...p.yIl
-000006c0: 6f63 626c 6f62 0000 0010 0000 01f9 0000  ocblob..........
-000006d0: 009e ffff ffff ffff 0000 0000 0019 0073  ...............s
-000006e0: 0070 0061 0072 0073 0065 005f 0070 006f  .p.a.r.s.e._.p.o
-000006f0: 0073 005f 0063 006f 006e 0074 005f 0066  .s._.c.o.n.t._.f
-00000700: 0069 006e 0069 0074 0065 002e 0070 0079  .i.n.i.t.e...p.y
-00000710: 496c 6f63 626c 6f62 0000 0010 0000 0267  Ilocblob.......g
-00000720: 0000 009e ffff ffff ffff 0000 0000 0000  ................
+00000520: 002e ffff ffff ffff 0000 0000 000a 0066  ...............f
+00000530: 0069 0074 005f 006c 0070 0061 002e 0070  .i.t._.l.p.a...p
+00000540: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
+00000550: 0267 0000 002e ffff ffff ffff 0000 0000  .g..............
+00000560: 0006 006c 0070 0061 002e 0070 0079 496c  ...l.p.a...p.yIl
+00000570: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
+00000580: 009e ffff ffff ffff 0000 0000 0005 0074  ...............t
+00000590: 0065 0073 0074 0073 6277 7370 626c 6f62  .e.s.t.sbwspblob
+000005a0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000005b0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+000005c0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+000005d0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+000005e0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+000005f0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00000600: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00000610: 0908 095f 1018 7b7b 3635 2c20 3433 397d  ..._..{{65, 439}
+00000620: 2c20 7b31 3039 382c 2034 3336 7d7d 0908  , {1098, 436}}..
+00000630: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
+00000640: 0000 0101 0000 0000 0000 000d 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 008b 0000 0005  ................
+00000660: 0074 0065 0073 0074 0073 6c67 3153 636f  .t.e.s.t.slg1Sco
+00000670: 6d70 0000 0000 0000 3343 0000 0005 0074  mp......3C.....t
+00000680: 0065 0073 0074 0073 6d6f 4444 626c 6f62  .e.s.t.smoDDblob
+00000690: 0000 0008 94f8 6a39 ccb4 c541 0000 0005  ......j9...A....
+000006a0: 0074 0065 0073 0074 0073 6d6f 6444 626c  .t.e.s.t.smodDbl
+000006b0: 6f62 0000 0008 8ff2 b624 ccb4 c541 0000  ob.......$...A..
+000006c0: 0005 0074 0065 0073 0074 0073 7068 3153  ...t.e.s.t.sph1S
+000006d0: 636f 6d70 0000 0000 0000 5000 0000 0005  comp......P.....
+000006e0: 0074 0065 0073 0074 0073 7653 726e 6c6f  .t.e.s.t.svSrnlo
+000006f0: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
+00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `vbayesfa-0.0.1/src/vbayesfa/discrete_finite.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.1/src/vbayesfa/fit_ibp.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/fit_ibp.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.1/src/vbayesfa/fit_lpa.py` & `vbayesfa-0.0.2/src/vbayesfa/fit_lpa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import numpy as np
 import functools
 import multiprocessing
 from itertools import product
 from .lpa import lpa_model
 from scipy.special import digamma
+from time import perf_counter
 
 def fit_lpa(x, starting_hpar = None, n_workers = 4, restarts = 4, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234, tolerance = 1e-05, max_iter = 50, min_iter = 30):
     """
+    Fit a Dirichlet process latent profile analysis (DPM-LPA) model using mean field
+    variational Bayes.
+    
     Parameters
     ----------
     x: data frame or array
         Observed data (data frame or matrix).  If a matrix then rows are variables and columns
         are observations; if a data frame then rows are observations and columns are variables.
-    starting_hpar: tuple, optional
-        If None (default) then the initial hyperparameters will be sampled as normal.
+    starting_hpar: dict, optional
+        If None (default) then the initial hyperparameters will have their default values.
         If specified, then it should be in as a dict with keys (phi, w1, w2, gamma1, gamma2).
     n_workers: int, optional
         Number of workers in the pool for parallel processing; should be less than
         or equal to the number of available CPUs.
     restarts: int, optional
-        Number of random restarts per set of alpha and omega values.
+        Number of random restarts.
     T: integer, optional
         Truncation level of the variational approximation.
     prior_w1: float, optional
         First prior hyperparameter on alpha.
     prior_w2: float, optional
         Second prior hyperparameter on alpha.
     prior_lambda_mu: float, optional
@@ -40,16 +44,19 @@
     max_iter: integer, optional
         Maximum number of iterations to run the optimization.
     min_iter: integer, optional
         Minimum number of iterations to run the optimization.
         
     Notes
     -----
-    ***** ADD THESE *****
+    This creates multiple lpa_model objects from the lpa.py module and fits them with using parallel
+    processing. See the documentation for the lpa_model object for more details.
     """
+    tic = perf_counter()
+
     model_list = []
     final_elbo = []
     
     with multiprocessing.Pool(n_workers) as pool:
         fun = functools.partial(__model_fit_wrapper__, x = x, starting_hpar = starting_hpar, T = T, prior_w1 = prior_w1, prior_w2 = prior_w2, prior_lambda_mu = prior_lambda_mu, prior_strength_for_xi = prior_strength_for_xi, tolerance = tolerance, max_iter = max_iter, min_iter = min_iter)
         
         # generate random seeds for each model based on the seed parameter
@@ -60,15 +67,17 @@
         
         results = pool.map(fun, seed_list)
         for result in results:
             model_list += [result]
             final_elbo += [result.elbo_list[-1]]
         
     final_elbo = np.array(final_elbo)
-        
+    toc = perf_counter()
+    print(f"Fit the model in {toc - tic:0.4f} seconds.")
+    
     return {'final_elbo': final_elbo, 'model_list': model_list, 'best_model': model_list[final_elbo.argmax()]}
 
 def __model_fit_wrapper__(seed, x, starting_hpar, T, prior_w1, prior_w2, prior_lambda_mu, prior_strength_for_xi, tolerance, max_iter, min_iter):
     """
     Defines an LPA model and fits it to the data, returning the result.
     This function is only defined in order to get the parallelization to work.
     """
```

### Comparing `vbayesfa-0.0.1/src/vbayesfa/full_discrete_finite.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/full_discrete_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.1/src/vbayesfa/lpa.py` & `vbayesfa-0.0.2/src/vbayesfa/lpa.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,135 @@
     Latent profiles have different means for each variable but share a common precision (xi).
     These have a normal-gamma prior.
     
     The concentration parameter (alpha) is learned.
     
     Attributes
     ----------
-    #####
+    * Data and related *
+    
+    x: array
+        Matrix of observations (rows are variables and columns are participants/observations).
+    T: integer
+        Truncation level for the variational approximation. Represents the maximum number of
+        latent profiles that can be discovered.
+    index: array or None
+        Participant IDs.
+    x_names: ordered categorical series
+        Names of observed variables.
+    mask: array
+        Indicates missing observations (= 1 if not missing, = 0 if missing).
+    n: int
+        Number of observations.
+    n_per_var: array of int
+        Number of observations for each variable (accounting for missing data).
+    m: int
+        Number of observed variables.
+    seed: int
+        Random seed.
+    rng: random generator
+        Generator for random numbers.
+    
+    * Prior distribution hyperparameters *
+    
+    prior_alpha_xi: float
+        Prior conventional hyperparameter for xi.
+    prior_beta_xi: float
+        Prior conventional hyperparameter for xi.
+    prior_m_mu: float
+        Prior conventional hyperparameter for mu.
+    prior_lambda_mu: float
+        Prior conventional hyperparameter for mu.
+    prior_tau1: float
+        Prior natural hyperparameter for mu and xi.
+    prior_tau2: float
+        Prior natural hyperparameter for mu and xi.
+    prior_tau3: float
+        Prior natural hyperparameter for mu and xi.
+    prior_tau4: float
+        Prior natural hyperparameter for mu and xi.
+    h_prior_tau: float
+        Prior log-normalizer for each of the observed variables.
+    prior_w1: float
+        First prior hyperparameter on alpha.
+    prior_w2: float
+        Second prior hyperparameter on alpha.
+    
+    * Lists for storing the ELBO and its components at each iteration *
+    
+    E_log_lik_list: list
+        List of expected log-likelihood values across updates.
+    E_log_prior_list: list
+        List of expected log-prior values across updates.
+    entropy_list: list
+        List of variational distribution entropy values across updates.
+    elbo_list: list
+        List of ELBO (evidence lower bound) values across updates.
+    
+    * Variational hyperparameters and related quantities *
+    
+    phi: array
+        Latent profile membership probabilities.
+    v_mu: array
+        Variance of mu.
+    E_xi_mu: array
+        Expected value of xi*mu.
+    E_xi_mu2: array
+        Expected value of xi*mu^2.
+    E_xi: array
+        Expected value of xi.
+    E_log_xi: array
+        Expected value of log(xi).
+    w1: float
+        First hyperparameter of alpha.
+    w2: float
+        Second hyperparameter of alpha.
+    E_alpha: float
+        Expected value of alpha.
+    E_log_alpha: float
+        Expected value of log(alpha).
+    gamma1: array
+        First hyperparameter of V.
+    gamma2: array
+        Second hyperparameter of V.
+    E_log_V: array
+        Expected value of log(V).
+    E_log_1minusV: array
+        Expected value of log(1 - V).
+    E_pi: array
+        Sample means of phi for each profile.
+    
+    * Results arranged for interpretation and analysis *
+    
+    n_profiles: int
+        Number of non-empty profiles (based on hard profile assignment).
+    profile_order: array
+        Order of profiles by number of members, i.e. profile size (based on hard profile assignment).
+    sorted_phi: array
+        Version of phi (profile membership probabilities) sorted by profile size
+        and omitting empty profiles.
+    sorted_m_mu: array
+        Version of m_mu (posterior mean of mu) sorted by profile size and omitting empty profiles.
+    sorted_v_mu: array
+        Version of v_mu (posterior variance of mu) sorted by profile size and omitting empty profiles.
+    z_hat: array
+        Point estimates of z (profile membership) based on hard assignment, with profiles labeled in size order.
+    z_hat_1hot: array
+        The same information as z_hat, but in 1-hot encoding, i.e. z_hat_1hot[j,i] = 1 if person/observation i
+        is in profile j and = 0 otherwise.
+    n_per_profile: array
+        Profile size, i.e. the number of members of each profile based on hard assignment (ordered by profile size).
+    prop_per_profile: array
+        Similar to n_per_profile, but gives proportions rather than numbers.
     
     Methods
     -------
     
+    ** FINISH THIS **
+    
     Notes
     -----
     This is based on Blei and Jordan (2006).
     
     The concentration parameter is given a Gamma(3, 1) prior and learned via variational
     Bayes as described in Appendix B.
     '''
@@ -39,16 +155,18 @@
     def __init__(self, x, T = 20, prior_w1 = 3.0, prior_w2 = 1.0, prior_lambda_mu = 0.5, prior_strength_for_xi = 10.0, seed = 1234):
         """
         Parameters
         ----------
         x: data frame or array
             Observed data (data frame or matrix).  If a matrix then rows are variables and columns
             are observations; if a data frame then rows are observations and columns are variables.
+            Missing values are replaced with 0 for computational reasons.
         T: integer, optional
-            Truncation level for the variational approximation.
+            Truncation level for the variational approximation. Represents the maximum number of
+            latent profiles that can be discovered.
         prior_w1: float, optional,
             First prior hyperparameter on alpha.
         prior_w2: float, optional
             Second prior hyperparameter on alpha.
         prior_lambda_mu: float, optional
             Controls the width of the prior distribution on mu: 
             higher values -> tighter prior around 0.
@@ -265,15 +383,15 @@
         for t in range(self.T):
             self.v_mu[:,t] = self.beta_xi/(self.lambda_mu[:,t]*(self.alpha_xi - 1))
             self.E_xi_mu[:,t] = (self.alpha_xi/self.beta_xi)*self.m_mu[:,t]
             self.E_xi_mu2[:,t] = (self.alpha_xi/self.beta_xi)*self.m_mu[:,t]**2 + 1/self.lambda_mu[:,t]
     
     def compute_E_log_lik(self):
         # compute the variational expectation of the total log-likelihood (can make more efficient later)
-        E_log_lik = - 0.5**np.log(2*np.pi) + 0.5*np.sum(self.n_per_var*self.E_log_xi)
+        E_log_lik = -0.5*np.sum(self.n_per_var)*np.log(2*np.pi) + 0.5*np.sum(self.n_per_var*self.E_log_xi) # FIX THIS LINE
         for j in range(self.m):
             E_log_lik += np.sum( self.mask[j,:]*( np.inner(self.E_xi_mu[j,:], self.phi.T)*self.x[j,:] - 0.5*self.E_xi[j]*self.x[j,:]**2 - 0.5*np.inner(self.E_xi_mu2[j,:], self.phi.T) ) )
         return E_log_lik
     
     def compute_E_log_prior(self):
         # compute expected log-prior
         E_log_mu_xi_prior = np.sum(np.sum(self.prior_tau1*self.E_xi_mu, axis = 1) + self.prior_tau2*self.E_xi + 0.5*self.prior_tau3*self.E_log_xi - np.sum(self.prior_tau4*self.E_xi_mu2, axis = 1) - self.h_prior_tau)
@@ -338,15 +456,15 @@
         plot_df = pd.DataFrame({'mu': np.concatenate([self.sorted_m_mu[:, most_similar_pair[0]], self.sorted_m_mu[:, most_similar_pair[1]]]), 
                                 'profile': self.m*['profile ' + str(most_similar_pair[0] + start_profile_labels_from1)] + self.m*['profile ' + str(most_similar_pair[1] + start_profile_labels_from1)], 
                                 'variable': pd.Categorical(2*list(self.x_names), categories = self.x_names, ordered = True)})
         plot = p9.ggplot(plot_df, p9.aes(x = 'variable', y = 'mu')) + p9.geom_bar(stat = 'identity')
         plot += p9.theme_classic(base_size = font_size) + p9.theme(figure_size = figure_size, axis_text_x = p9.element_text(rotation = 90, hjust = 1))
         plot += p9.facet_wrap('profile', scales = 'free_x', ncol = 2)
         
-        return {'similarity': similarity, 'max_similarity': similarity_off_diag.max(), 'most_similar_pair': most_similar_pair, 'mean_similarity': np.mean(similarity_vector), 'plot': plot}            
+        return {'similarity': similarity, 'distance': np.sqrt(squareform(squared_distance)), 'max_similarity': similarity_off_diag.max(), 'most_similar_pair': most_similar_pair, 'mean_similarity': np.mean(similarity_vector), 'min_distance': np.min(np.sqrt(squared_distance)), 'mean_distance': np.mean(np.sqrt(squared_distance)), 'plot': plot}            
     
     def classify_new_data(self, x_new):
         '''
         Compute the (approximate) probability of new data points belonging to
         each profile given the model's current variational parameters.
         
         Notes
```

### Comparing `vbayesfa-0.0.1/src/vbayesfa/lpa_outcome_analysis.py` & `vbayesfa-0.0.2/src/vbayesfa/lpa_outcome_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,44 +33,114 @@
                  font_size = 11,
                  facet_var = 'variable',
                  ncol = 4):
     '''
     Analyze the relationship between dependent variables (y) -
     that are assumed to be normally distributed - and the profiles.
     This is done without changing the model's other variational parameters.
+    
+    Parameters
+    ----------
+    model: LPA model
+        The fitted LPA model.
+    y: dataframe
+        Outcome data.
+    x_new:
+        New LPA model data (from participants not used to fit the LPA model).
+    y_new: dataframe
+        New outcome data (from participants not used to fit the LPA model).
+    index: array-like, optional
+        Optional individual participant/observation labels.
+    profile_labels: array-like, optional
+        Optional labels for latent profiles.
+    start_profile_labels_from1: boolean, optional
+        Whether to label latent profiles starting from 0 (Python style)
+        or from 1 (R/Matlab/ordinary counting style). This only affects
+        output labeling, not any calculations.
+    prior_alpha: float, optional
+        Prior alpha parameter.
+    prior_beta: float, optional
+        Prior beta parameter.
+    prior_m: float, optional
+        Prior m parameter.
+    prior_lambda: float, optional
+        Prior lambda parameter.
+    figure_size: list of floats, optional
+        Size of plots.
+    font_size: integer, optional
+        Font size for plots.
+    facet_var: string, optional
+        Faceting variable for plots.
+    ncol: integer, optional
+        Number of columns to use in plots.
+        
+    Returns
+    -------
+    A dict with the following data:
+    
+    plot: plot
+        A plot displaying 95% posterior credible intervals of group means for each outcome variable.
+    plot_df: dataframe
+        Table of statistics used to create the plot.
+    bayes_factors: dataframe
+        Table of Bayesian 1-way ANOVA results.
+            bf10: Bayes factor for comparing H1 (all latent profiles have different means) to H0 (all latent profiles have the same mean).
+            log10_bf10: The base-10 logarithm of the above (this is easier to interpret).
+            post_hoc_result: The best partition of latent profiles into sets with equal means within each set and different means between sets. This is the result of post-hoc analysis, which is performed only when log10_bf10 > *ASDF* (indicating substantial evidence for H1 according to the criteria of *REF*).
+    r2: series
+        Coefficient of determination (r^2) for each outcome, based on LPA categorization of participants/
+        observations.
+    post_hpar: dataframe
+        Posterior hyperparameters of each outcome for each latent profile.
+        
+    Notes
+    -----
+    
+    Outcome means/variances are given a normal-gamma prior distribution with the specified hyperparameters (prior alpha,
+    prior_beta, prior_m, and prior_lambda).
+    
+    All calculations relating latent profiles to outcome variables (y) use hard assignment of participants/observations
+    to latent profiles, i.e. each participant is assigned to their most probable profile, which is then treated as known.
+    
+    Outcome variance is treated as shared across profiles in computing the Bayes factors, but not when computing posterior
+    hyperparameters or r^2. This does not seem to make much practical difference, but is an inconsistency that could be changed
+    later.
+    
+    Currently y_new and x_new are not used. In a previous version, they were used to compute r^2 values for observations/
+    participants that had not been used in fitting either the LPA model or the outcome variable relationship. This
+    provided a measure of out of sample generalization of outcome relationships. This should be added back into a future version.
+    
+    *UPDATE THIS LAST POINT*
+    In a future version, we should change the Bayes factors to perform Rouder et al Bayesian ANOVA calculations
+    rather than the somewhat naive versions I've used here. Also, the pairwise mean comparisons should be replaced with
+    a partition-based post-hoc analysis as described in our paper.
     '''
     ##### SET UP DATA ETC #####
     y_names = pd.Categorical(y.columns.values, categories = y.columns.values, ordered = True)
     if index is None:
         y = y.copy()
     else:
         y = y.iloc[index].copy().transpose()
     n_y = y.shape[1] # number of dependent variables
         
-    bayes_factor_df = pd.DataFrame(1.0,
-                                   columns = ['bf10', 'frac_bf10'],
+    bayes_factor_df = pd.DataFrame(columns = ['bf10', 'log10_bf10', 'conclusion', 'post_hoc_result'],
                                    index = y_names) # empty dataframe for results
-        
-    ##### COMPUTE REGULAR, FRACTIONAL, AND POSTERIOR BAYES FACTORS #####
+    
+    ##### COMPUTE BAYES FACTORS (BAYESIAN ANOVAS) #####
     for j in range(n_y):
         y_j = y[y_names[j]].values
-        bayes_factor_df.loc[y_names[j], 'bf10'] = bayes_factors.normal_shared_var(y_j, model.z_hat_1hot, prior_m, prior_lambda, prior_alpha, prior_beta)
-        bayes_factor_df.loc[y_names[j], 'frac_bf10'] = bayes_factors.frac_normal_shared_var(y_j, model.z_hat_1hot, prior_m, prior_lambda, prior_alpha, prior_beta)
-        bayes_factor_df.loc[y_names[j], 'post_bf10'] = bayes_factors.post_normal_shared_var(y_j, model.z_hat_1hot, prior_m, prior_lambda, prior_alpha, prior_beta)
-        
-    ##### PAIRWISE COMPARISONS (FRACTIONAL BAYES FACTORS) TO PROFILE 0 #####
-    pairwise_log10_frac_bf10 = pd.DataFrame(0.0,
-                                            columns = ['profile ' + str(t + start_profile_labels_from1) for t in range(1, model.n_profiles)],
-                                            index = y_names)
-    for j in range(n_y):
-        for t in range(1, model.n_profiles):
-            in_profiles = np.isin(model.z_hat, [0, t])
-            y_used = y.loc[in_profiles, y_names[j]].values # only include data from people in these profiles
-            z_hat_used = model.z_hat_1hot[:, in_profiles][[0, t], :]
-            pairwise_log10_frac_bf10.loc[y_names[j], 'profile ' + str(t + start_profile_labels_from1)] = np.log10(bayes_factors.frac_normal_shared_var(y_used, z_hat_used, prior_m, prior_lambda, prior_alpha, prior_beta))
+        bayes_factor_df.loc[y_names[j], 'bf10'] = bayes_factors.bf10_1way_anova(y = y_j, groups = model.z_hat, rscale = 0.5, epsrel = 1e-4, limit = 50)
+        bayes_factor_df.loc[y_names[j], 'log10_bf10'] = np.log10(bayes_factor_df.loc[y_names[j], 'bf10'])
+        if bayes_factor_df.loc[y_names[j], 'log10_bf10'] > 0.5:
+            bayes_factor_df.loc[y_names[j], 'conclusion'] = 'profile means differ'
+            bayes_factor_df.loc[y_names[j], 'post_hoc_result'] = bayes_factors.partition_posthoc(y = y_j, groups = model.z_hat, rscale = 0.5, epsrel = 1e-4, limit = 50)['best_partition'] # post-hoc analysis (partition-based)
+        elif bayes_factor_df.loc[y_names[j], 'log10_bf10'] < 0.5:
+            bayes_factor_df.loc[y_names[j], 'conclusion'] = 'profile means ='
+        else:
+            bayes_factor_df.loc[y_names[j], 'conclusion'] = 'indecisive'
     
     ##### POSTERIOR HYPERPARAMETERS #####
     post_hpar = {'m': np.zeros([n_y, model.n_profiles]), 'lambda': np.zeros([n_y, model.n_profiles]), 'alpha': np.zeros(n_y), 'beta': np.zeros(n_y)}
     v_mu = np.zeros([n_y, model.n_profiles])
     for j in range(n_y):
         (y_j, z_hat_j) = _remove_nan(y[y_names[j]].values, model.z_hat_1hot)
         dist = exp_families.multi_group_normal({'m': prior_m, 'lambda': prior_lambda, 'alpha': prior_alpha, 'beta': prior_beta}, model.n_profiles)
@@ -127,15 +197,16 @@
         
     if n_y > 1:
         if facet_var == 'profile':
             plot += p9.facet_wrap('profile', scales = 'free_x', ncol = ncol)
         elif facet_var == 'variable':
             plot += p9.facet_wrap('variable', scales = 'free', ncol = ncol)
     
-    output = {'plot': plot, 'plot_df': plot_df, 'bayes_factors': bayes_factor_df, 'log10_bayes_factors': np.log10(bayes_factor_df), 'pairwise_log10_frac_bf10': pairwise_log10_frac_bf10, 'r2': r2, 'post_hpar': post_hpar}
+    ##### OUTPUT #####
+    output = {'plot': plot, 'plot_df': plot_df, 'bayes_factors': bayes_factor_df, 'r2': r2, 'post_hpar': post_hpar}
     
 #    if not y_new is None:
         # TOTALLY REVISE THIS
         ##### GET THE APPROXIMATE LOG POSTERIOR PREDICTIVE (p(y | x)) AND PREDICTED MEAN FOR NEW DATA #####
 #        n_new = y_new.shape[0]
 #        log_post_pred = pd.DataFrame(0.0, index = y_new.index, columns = y_new.columns)
 #        post_pred_mean = pd.DataFrame(0.0, index = y_new.index, columns = y_new.columns)
@@ -176,17 +247,74 @@
                     facet_var = 'variable', 
                     ncol = 4):
     '''
     Analyze the relationship between dependent variables (y) -
     that are assumed to be Bernoulli distributed - and the profiles.
     This is done without changing the model's other variational parameters.
     
+    Parameters
+    ----------
+    model: LPA model
+        The fitted LPA model.
+    y: dataframe
+        Outcome data.
+    index: array-like, optional
+        Optional individual participant/observation labels.
+    profile_labels: array-like, optional
+        Optional labels for latent profiles.
+    start_profile_labels_from1: boolean, optional
+        Whether to label latent profiles starting from 0 (Python style)
+        or from 1 (R/Matlab/ordinary counting style). This only affects
+        output labeling, not any calculations.
+    prior_a: float, optional
+        Prior a parameter.
+    prior_b: float, optional
+        Prior b parameter.
+    figure_size: list of floats, optional
+        Size of plots.
+    font_size: integer, optional
+        Font size for plots.
+    facet_var: string, optional
+        Faceting variable for plots.
+    ncol: integer, optional
+        Number of columns to use in plots.
+    
+    Returns
+    -------
+    A dict with the following data:
+    
+    plot: plot
+        A plot displaying 95% posterior credible intervals of psi (outcome probability) for each outcome variable.
+    plot_df: dataframe
+        Table of statistics used to create the plot.
+    bayes_factors: dataframe
+        Table of Bayes factors, posterior Bayes factors, and fractional Bayes factors testing
+        equality of group outcome means.
+    log10_bayes_factors: dataframe
+        The Bayes factor table in base-10 logarithmic scale.
+    pairwise_log10_frac_bf10: dataframe
+        Table of pairwise Bayes factors testing equality of means between groups, in log-10 scale.
+    bss: series
+        Brier skill scores for each outcome (a measure of effect size similar to r^2), based on LPA categorization 
+        of participants/observations.
+    post_hpar: dataframe
+        Posterior hyperparameters of each outcome for each latent profile.
+    
     Notes
     -----
-    We assume y_i | z_i = t ~ Bernoulli(psi_t).
+    Statistical model:
+    y_i | z_i = t ~ Bernoulli(psi_t)
+    psi_t ~ Beta(prior_a, prior_b)
+    
+    All calculations relating latent profiles to outcome variables (y) use hard assignment of participants/observations
+    to latent profiles, i.e. each participant is assigned to their most probable profile, which is then treated as known.
+    
+    In a future version, the pairwise mean comparisons should be replaced with a partition-based post-hoc analysis as 
+    described in our paper. Also, it would be nice to add a generalization test using new data (x_new and y_new) as
+    in previous versions of the normal outcome analysis function.
     '''
     ##### SET UP DATA ETC #####
     y_names = pd.Categorical(y.columns.values, categories = y.columns.values, ordered = True)
     if index is None:
         y = y.copy()
     else:
         y = y.iloc[index].copy().transpose()
```

### Comparing `vbayesfa-0.0.1/src/vbayesfa/make_sim_data.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/make_sim_data.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.1/src/vbayesfa/sparse_cont_finite.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/sparse_cont_finite.py`

 * *Files identical despite different names*

### Comparing `vbayesfa-0.0.1/src/vbayesfa/sparse_pos_cont_finite.py` & `vbayesfa-0.0.2/src/vbayesfa/ibp/sparse_pos_cont_finite.py`

 * *Files identical despite different names*

