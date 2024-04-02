# Comparing `tmp/quantes-2.0.3.tar.gz` & `tmp/quantes-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantes-2.0.3.tar", last modified: Sun Mar 31 14:00:28 2024, max compression
+gzip compressed data, was "quantes-2.0.4.tar", last modified: Tue Apr  2 01:57:57 2024, max compression
```

## Comparing `quantes-2.0.3.tar` & `quantes-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-01 04:10:19.535872 quantes-2.0.3/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    35149 2024-03-31 02:51:56.000000 quantes-2.0.3/LICENSE
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12332 2024-04-01 04:10:19.534615 quantes-2.0.3/PKG-INFO
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    11815 2024-04-01 04:05:46.000000 quantes-2.0.3/README.md
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-01 04:10:19.449246 quantes-2.0.3/quantes/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-01 04:05:46.000000 quantes-2.0.3/quantes/__init__.py
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    49308 2024-04-01 04:05:46.000000 quantes-2.0.3/quantes/joint.py
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)   103339 2024-04-01 04:05:46.000000 quantes-2.0.3/quantes/linear.py
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-01 04:10:19.520740 quantes-2.0.3/quantes.egg-info/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12332 2024-04-01 04:10:19.000000 quantes-2.0.3/quantes.egg-info/PKG-INFO
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      235 2024-04-01 04:10:19.000000 quantes-2.0.3/quantes.egg-info/SOURCES.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        1 2024-04-01 04:10:19.000000 quantes-2.0.3/quantes.egg-info/dependency_links.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       59 2024-04-01 04:10:19.000000 quantes-2.0.3/quantes.egg-info/requires.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        8 2024-04-01 04:10:19.000000 quantes-2.0.3/quantes.egg-info/top_level.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       38 2024-04-01 04:10:19.536996 quantes-2.0.3/setup.cfg
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)     1002 2024-04-01 04:09:42.000000 quantes-2.0.3/setup.py
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.790560 quantes-2.0.4/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    35149 2024-03-31 02:51:56.000000 quantes-2.0.4/LICENSE
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12284 2024-04-02 01:57:57.788226 quantes-2.0.4/PKG-INFO
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    11815 2024-04-01 04:05:46.000000 quantes-2.0.4/README.md
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.684303 quantes-2.0.4/quantes/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/__init__.py
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    49712 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/joint.py
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)   103370 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/linear.py
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.773483 quantes-2.0.4/quantes.egg-info/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12284 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/PKG-INFO
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      235 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/SOURCES.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        1 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/dependency_links.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       59 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/requires.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        8 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/top_level.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       38 2024-04-02 01:57:57.791630 quantes-2.0.4/setup.cfg
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      958 2024-04-02 01:57:10.000000 quantes-2.0.4/setup.py
```

### Comparing `quantes-2.0.3/LICENSE` & `quantes-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quantes-2.0.3/PKG-INFO` & `quantes-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quantes
-Version: 2.0.3
+Version: 2.0.4
 Summary: Convolution Smoothed Quantile and Expected Shortfall Regression
 Home-page: https://github.com/WenxinZhou/conquer
-Author: ['Wenxin Zhou', 'Huaning Liu']
-Author-email: ['wenxinz@uic.edu', 'huaning3@illinois.edu']
+Author: Wenxin Zhou
+Author-email: wenxinz@uic.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quantes-2.0.3/README.md` & `quantes-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quantes-2.0.3/quantes/joint.py` & `quantes-2.0.4/quantes/joint.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,44 +29,14 @@
 ###############################################################################
 ######################### Linear QuantES Regression ###########################
 ###############################################################################
 class LR(low_dim):
     '''
         Joint Linear Quantile and Expected Shortfall Regression    
     '''
-    def _G2(self, G2_type=1):
-        '''
-            Specification Function G2 in Fissler and Ziegel's Joint Loss 
-        '''
-        if G2_type == 1:
-            f0 = lambda x : -np.sqrt(-x)
-            f1 = lambda x : 0.5 / np.sqrt(-x)
-            f2 = lambda x : 0.25 / np.sqrt((-x)**3)
-        elif G2_type == 2:
-            f0 = lambda x : -np.log(-x)
-            f1 = lambda x : -1 / x
-            f2 = lambda x : 1 / x ** 2
-        elif G2_type == 3:
-            f0 = lambda x : -1 / x
-            f1 = lambda x : 1 / x ** 2
-            f2 = lambda x : -2 / x ** 3
-        elif G2_type == 4:
-            f0 = lambda x : np.log( 1 + np.exp(x))
-            f1 = lambda x : np.exp(x) / (1 + np.exp(x))
-            f2 = lambda x : np.exp(x) / (1 + np.exp(x)) ** 2
-        elif G2_type == 5:
-            f0 = lambda x : np.exp(x)
-            f1 = lambda x : np.exp(x)
-            f2 = lambda x : np.exp(x) 
-        else:
-            raise ValueError("G2_type must be an integer between 1 and 5")
-
-        return f0, f1, f2 
-
-
     def _FZ_loss(self, x, tau, G1=False, G2_type=1):
         '''
             Fissler and Ziegel's Joint Loss Function
 
         Args:
             G1 : logical flag for the specification function G1 in FZ's loss;
                  G1(x)=0 if G1=False, and G1(x)=x and G1=True.
@@ -82,15 +52,15 @@
             Ymax = np.max(self.Y)
             Y = self.Y - Ymax
         else:
             Y = self.Y
         dim = X.shape[1]
         Yq = X @ x[:dim]
         Ye = X @ x[dim : 2*dim]
-        f0, f1, _ = self._G2(G2_type)
+        f0, f1, _ = G2(G2_type)
         loss = f1(Ye) * (Ye - Yq - (Y - Yq) * (Y<= Yq) / tau) - f0(Ye)
         if G1:
             return np.mean((tau - (Y<=Yq)) * (Y-Yq) + loss)
         else:
             return np.mean(loss)
 
 
@@ -99,21 +69,21 @@
                   options={'maxiter': None, 'maxfev': None, 'disp': False, 
                            'return_all': False, 'initial_simplex': None, 
                            'xatol': 0.0001, 'fatol': 0.0001, 'adaptive': False}):
         '''
             Joint Quantile & Expected Shortfall Regression via FZ Loss Minimization
 
         Refs:
-            Higher Order Elicitability and Osband's Principle (2016)
+            Higher Order Elicitability and Osband's Principle
             by Tobias Fissler and Johanna F. Ziegel
-            Ann. Statist. 44(4): 1680-1707
+            Ann. Statist. 44(4): 1680-1707, 2016
 
-            A Joint Quantile and Expected Shortfall Regression Framework (2019)
+            A Joint Quantile and Expected Shortfall Regression Framework
             by Timo Dimitriadis and Sebastian Bayer 
-            Electron. J. Stat. 13(1): 1823-1871
+            Electron. J. Stat. 13(1): 1823-1871, 2019
         
         Args:
             tau : quantile level; default is 0.5.
             G1 : logical flag for the specification function G1 in FZ's loss; 
                  G1(x)=0 if G1=False, and G1(x)=x and G1=True.
             G2_type : an integer (from 1 to 5) that indicates the type of the specification function G2 in FZ's loss.
             standardize : logical flag for x variable standardization prior to fitting the quantile model; 
@@ -134,26 +104,27 @@
 
         dim = self.X.shape[1]
         Ymax = np.max(self.Y)
         ### warm start with QR + truncated least squares
         qrfit = low_dim(self.X[:, self.itcp:], self.Y, intercept=True)\
                 .fit(tau=tau, standardize=standardize)
         coef_q = qrfit['beta']
-        tail = self.Y <= self.X.dot(coef_q)
+        tail = self.Y <= self.X @ coef_q
         tail_X = self.X[tail,:] 
         tail_Y = self.Y[tail]
-        coef_e = np.linalg.solve(tail_X.T.dot(tail_X), tail_X.T.dot(tail_Y))
+        coef_e = np.linalg.solve(tail_X.T @ tail_X, tail_X.T @ tail_Y)
         if G2_type in {1, 2, 3}:
             coef_q[0] -= Ymax
             coef_e[0] -= Ymax
         x0 = np.r_[(coef_q, coef_e)]
 
         ### joint quantile and ES fit
         fun  = lambda x : self._FZ_loss(x, tau, G1, G2_type)
-        esfit = minimize(fun, x0, method='Nelder-Mead', tol=tol, options=options)
+        esfit = minimize(fun, x0, method='Nelder-Mead', 
+                         tol=tol, options=options)
         nit, nfev = esfit['nit'], esfit['nfev']
 
         ### refit if convergence criterion is not met
         while refit and not esfit['success']:
             esfit = minimize(fun, esfit['x'], method='Nelder-Mead',
                              tol=tol, options=options)
             nit += esfit['nit']
@@ -171,33 +142,33 @@
 
 
     def twostep_fit(self, tau=0.5, h=None, kernel='Laplacian', 
                     loss='L2', robust=None, G2_type=1,
                     standardize=True, tol=None, options=None,
                     ci=False, level=0.95):
         '''
-            Two-Step Procedure for Joint Quantile & Expected Shortfall Regression
+            Two-Step Procedure for Joint QuantES Regression
 
         Refs:
-            Higher Order Elicitability and Osband's Principle (2016)
+            Higher Order Elicitability and Osband's Principle
             by Tobias Fissler and Johanna F. Ziegel
-            Ann. Statist. 44(4): 1680-1707
+            Ann. Statist. 44(4): 1680-1707, 2016
 
-            Effciently Weighted Estimation of Tail and Interquantile Expectations (2020)
+            Effciently Weighted Estimation of Tail and Interquantile Expectations
             by Sander Barendse 
-            SSRN Preprint
+            SSRN Preprint, 2020
         
             Robust Estimation and Inference 
-            for Expected Shortfall Regression with Many Regressors (2023)
+            for Expected Shortfall Regression with Many Regressors
             by Xuming He, Kean Ming Tan and Wen-Xin Zhou
-            J. R. Stat. Soc. B. 85(4): 1223-1246
+            J. R. Stat. Soc. B. 85(4): 1223-1246, 2023
 
-            Inference for Joint Quantile and Expected Shortfall Regression (2023)
-            by Xiang Peng and Judy Wang
-            Stat 12(1) e619
+            Inference for Joint Quantile and Expected Shortfall Regression
+            by Xiang Peng and Huixia Judy Wang
+            Stat 12(1) e619, 2023
 
         Args:
             tau : quantile level; default is 0.5.
             h : bandwidth; the default value is computed by self.bandwidth(tau).
             kernel : a character string representing one of the built-in smoothing kernels;
                      default is "Laplacian".
             loss : the loss function used in stage two. There are three options.
@@ -220,108 +191,111 @@
             'res_q' : a vector of fitted quantile regression residuals.
             'coef_e' : expected shortfall regression coefficient estimate.
             'robust' : robustification parameter in the Huber loss.
             'ci' : coordinates-wise (100*level)% confidence intervals.
         '''
   
         if loss in {'L2', 'Huber', 'TrunL2', 'TrunHuber'}:
-            qrfit = self.fit(tau=tau, h=h, kernel=kernel, standardize=standardize)
+            qrfit = self.fit(tau=tau, h=h, kernel=kernel, 
+                             standardize=standardize)
             nres_q = np.minimum(qrfit['res'], 0)
         
         if loss == 'L2':
-            adj = np.linalg.solve(self.X.T.dot(self.X), self.X.T.dot(nres_q) / tau)
+            adj = np.linalg.solve(self.X.T@self.X, self.X.T@nres_q / tau)
             coef_e = qrfit['beta'] + adj
             robust = None
         elif loss == 'Huber':
             Z = nres_q + tau*(self.Y - qrfit['res'])
             X0 = self.X[:, self.itcp:]
             if robust == None:
                 esfit = low_dim(tau*X0, Z, intercept=self.itcp).adaHuber()
                 coef_e = esfit['beta']
                 robust = esfit['robust']
                 if self.itcp: coef_e[0] /= tau
             elif robust > 0:
-                esfit = low_dim(tau*X0, Z, intercept=self.itcp).retire(robust=robust,
-                                                                       standardize=standardize,
-                                                                       scale=False)
+                esfit = low_dim(tau*X0, Z, intercept=self.itcp)\
+                    .als(robust=robust, standardize=standardize, scale=False)
                 coef_e = esfit['beta']
                 robust = esfit['robust']
                 if self.itcp: coef_e[0] /= tau
             else:
                 raise ValueError("robustification parameter must be positive")
         elif loss == 'FZ':
             if G2_type in np.arange(1,4):
                 Ymax = np.max(self.Y)
                 Y = self.Y - Ymax
             else:
                 Y = self.Y
             qrfit = low_dim(self.X[:, self.itcp:], Y, intercept=True)\
                     .fit(tau=tau, h=h, kernel=kernel, standardize=standardize)
             adj = np.minimum(qrfit['res'], 0)/tau + Y - qrfit['res']
-            f0, f1, f2 = self._G2(G2_type)
+            f0, f1, f2 = G2(G2_type)
 
-            fun  = lambda z : np.mean(f1(self.X.dot(z)) * (self.X.dot(z) - adj) \
-                                      - f0(self.X.dot(z)))
-            grad = lambda z : self.X.T.dot(f2(self.X.dot(z)) \
-                                           * (self.X.dot(z) - adj))/self.n
+            fun  = lambda z : np.mean(f1(self.X @ z) * (self.X @ z - adj) \
+                                      - f0(self.X @ z))
+            grad = lambda z : self.X.T@(f2(self.X@z)*(self.X@z - adj))/self.n
             esfit = minimize(fun, qrfit['beta'], method='BFGS', 
                              jac=grad, tol=tol, options=options)
             coef_e = esfit['x']
             robust = None
             if G2_type in np.arange(1,4):
                 coef_e[0] += Ymax
                 qrfit['beta'][0] += Ymax
         elif loss == 'TrunL2':
-            tail = self.Y <= self.X.dot(qrfit['beta'])
+            tail = self.Y <= self.X @ qrfit['beta']
             tail_X = self.X[tail,:] 
             tail_Y = self.Y[tail]
-            coef_e = np.linalg.solve(tail_X.T.dot(tail_X), 
-                                     tail_X.T.dot(tail_Y))
+            coef_e = np.linalg.solve(tail_X.T @ tail_X, 
+                                     tail_X.T @ tail_Y)
             robust = None
         elif loss == 'TrunHuber':
-            tail = self.Y <= self.X.dot(qrfit['beta'])
+            tail = self.Y <= self.X @ qrfit['beta']
             esfit = LR(self.X[tail, self.itcp:], self.Y[tail],\
                        intercept=self.itcp).adaHuber()
             coef_e = esfit['beta']
             robust = esfit['robust']
 
         if loss in {'L2', 'Huber'} and ci:
-            res_e = nres_q + tau * self.X.dot(qrfit['beta'] - coef_e)
+            res_e = nres_q + tau * self.X@(qrfit['beta'] - coef_e)
             n, p = self.X[:,self.itcp:].shape
             X0 = np.c_[np.ones(n,), self.X[:,self.itcp:] - self.mX]
             if loss == 'L2':
                 weight = res_e ** 2
             else:
                 weight = np.minimum(res_e ** 2, robust ** 2)
     
-            inv_sig = np.linalg.inv(X0.T.dot(X0) / n)   
-            acov = inv_sig.dot((X0.T * weight).dot(X0) / n).dot(inv_sig)
-            radius = norm.ppf(1/2 + level/2) * np.sqrt( np.diag(acov) / n) / tau
+            inv_sig = np.linalg.inv(X0.T @ X0 / n)   
+            acov = inv_sig @ ((X0.T * weight) @ X0 / n) @ inv_sig
+            radius = norm.ppf(1/2 + level/2) * np.sqrt(np.diag(acov)/n) / tau
             ci = np.c_[coef_e - radius, coef_e + radius]
 
         return {'coef_q': qrfit['beta'], 'res_q': qrfit['res'], 
                 'coef_e': coef_e,
                 'loss': loss, 'robust': robust,
                 'ci': ci, 'level': level}
 
 
     def boot_es(self, tau=0.5, h=None, kernel='Laplacian', 
                 loss='L2', robust=None, standardize=True, 
                 B=200, level=0.95):
 
-        fit = self.twostep_fit(tau, h, kernel, loss, robust, standardize=standardize)
+        fit = self.twostep_fit(tau, h, kernel, loss, 
+                               robust, standardize=standardize)
         boot_coef = np.zeros((self.X.shape[1], B))
         for b in range(B):
             idx = rgt.choice(np.arange(self.n), size=self.n)
-            boot = LR(self.X[idx,self.itcp:], self.Y[idx], intercept=self.itcp)
+            boot = LR(self.X[idx,self.itcp:], self.Y[idx], 
+                      intercept=self.itcp)
             if loss == 'L2':
-                bfit = boot.twostep_fit(tau, h, kernel, loss='L2', standardize=standardize)
+                bfit = boot.twostep_fit(tau, h, kernel, loss='L2', 
+                                        standardize=standardize)
             else:
-                bfit = boot.twostep_fit(tau, h, kernel, loss, \
-                                        robust=fit['robust'], standardize=standardize)
+                bfit = boot.twostep_fit(tau, h, kernel, loss,
+                                        robust=fit['robust'],
+                                        standardize=standardize)
             boot_coef[:,b] = bfit['coef_e']
         
         left  = np.quantile(boot_coef, 1/2-level/2, axis=1)
         right = np.quantile(boot_coef, 1/2+level/2, axis=1)
         piv_ci = np.c_[2*fit['coef_e'] - right, 2*fit['coef_e'] - left]
         per_ci = np.c_[left, right]
 
@@ -336,78 +310,80 @@
                loss='L2', robust=None, standardize=True, 
                ci=False, level=0.95):
         '''
             Non-Crossing Joint Quantile & Expected Shortfall Regression
 
         Refs:
             Robust Estimation and Inference  
-            for Expected Shortfall Regression with Many Regressors (2023)
+            for Expected Shortfall Regression with Many Regressors
             by Xuming He, Kean Ming Tan and Wen-Xin Zhou
-            J. R. Stat. Soc. B. 85(4): 1223-1246
+            J. R. Stat. Soc. B. 85(4): 1223-1246, 2023
         '''
 
         qrfit = self.fit(tau=tau, h=h, kernel=kernel, standardize=standardize)
         nres_q = np.minimum(qrfit['res'], 0)
         fitted_q = self.Y - qrfit['res']
         Z = nres_q/tau + fitted_q
  
-        P = matrix(self.X.T.dot(self.X) / self.n)
-        q = matrix(-self.X.T.dot(Z) / self.n)
+        P = matrix(self.X.T @ self.X / self.n)
+        q = matrix(-self.X.T @ Z / self.n)
         G = matrix(self.X)
         hh = matrix(fitted_q)
         l, c = 0, robust 
         
         if loss == 'L2':
-            esfit = solvers.qp(P, q, G, hh, initvals={'x': matrix(qrfit['beta'])})
+            esfit = solvers.qp(P, q, G, hh, 
+                               initvals={'x': matrix(qrfit['beta'])})
             coef_e = np.array(esfit['x']).reshape(self.X.shape[1],)
         else:
             rel = (self.X.shape[1] + np.log(self.n)) / self.n
-            esfit = self.twostep_fit(tau, h, kernel, loss, robust, standardize=standardize)
+            esfit = self.twostep_fit(tau, h, kernel, loss, 
+                                     robust, standardize=standardize)
             coef_e = esfit['coef_e']
-            res  = np.abs(Z - self.X.dot(coef_e))
+            res  = np.abs(Z - self.X @ coef_e)
             c = robust
             
             if robust == None:
                 c = find_root(lambda t : np.mean(np.minimum((res/t)**2, 1)) - rel,
                               np.min(res)+self.params['tol'], np.sqrt(res @ res))
 
             sol_diff = 1
             while l < self.params['max_iter'] \
                 and sol_diff > self.params['tol']:
                 wt = np.where(res > c, res/c, 1)
-                P = matrix( (self.X.T / wt ).dot(self.X) / self.n)
-                q = matrix( -self.X.T.dot(Z / wt) / self.n)
+                P = matrix( (self.X.T / wt ) @ self.X / self.n)
+                q = matrix( -self.X.T @ (Z / wt) / self.n)
                 esfit = solvers.qp(P, q, G, hh, initvals={'x': matrix(coef_e)})
                 tmp = np.array(esfit['x']).reshape(self.X.shape[1],)
                 sol_diff = np.max(np.abs(tmp - coef_e))
-                res = np.abs(Z - self.X.dot(tmp))
+                res = np.abs(Z - self.X @ tmp)
                 if robust == None:
                     c = find_root(lambda t : np.mean(np.minimum((res/t)**2, 1)) - rel,
                                   np.min(res)+self.params['tol'], np.sqrt(res @ res))
                 coef_e = tmp
                 l += 1
             c *= tau
 
         if ci:
-            res_e = nres_q + tau * (fitted_q - self.X.dot(coef_e))
+            res_e = nres_q + tau * (fitted_q - self.X @ coef_e)
             X0 = np.c_[np.ones(self.n,), self.X[:,self.itcp:] - self.mX]
             if loss == 'L2': weight = res_e ** 2
             else: weight = np.minimum(res_e ** 2, c ** 2)
     
-            inv_sig = np.linalg.inv(X0.T.dot(X0) / self.n)   
-            acov = inv_sig.dot((X0.T * weight).dot(X0) / self.n).dot(inv_sig)
-            radius = norm.ppf(1/2 + level/2) * np.sqrt( np.diag(acov) / self.n) / tau
+            inv_sig = np.linalg.inv(X0.T @ X0 / self.n)   
+            acov = inv_sig @ ((X0.T * weight) @ X0 / self.n) @ inv_sig
+            radius = norm.ppf(1/2 + level/2) * np.sqrt(np.diag(acov)/self.n) / tau
             ci = np.c_[coef_e - radius, coef_e + radius]
 
         return {'coef_q': qrfit['beta'], 
                 'res_q': qrfit['res'], 
                 'coef_e': coef_e, 'nit': l,
                 'loss': loss, 'robust': c,
                 'ci': ci, 'level': level}
-    
+
 
 
 ###############################################################################
 ########################## Kernel Ridge Regression ############################
 ###############################################################################
 class KRR:
     '''
@@ -753,21 +729,26 @@
             self.es_fit = self.K @ self.es_beta
         self.es_residual = Z - self.es_fit
         self.es_model = None
 
 
     def lses(self, tau=0.5, 
              alpha_q=1, alpha_e=1,
-             smooth=False, h=0., 
+             qt_fit=None, smooth=False, h=0.,
              method='L-BFGS-B', solver='clarabel',
              qt_tol=1e-7, options=None):
         
-        self.alpha_e, self.tau, self.itcp = alpha_e, tau, True
-        self.qt(tau, alpha_q, None, True,
-                smooth, h, method, solver, qt_tol, options) 
+        self.alpha_e, self.tau, self.itcp = alpha_e, tau, False
+        if qt_fit is None:
+            self.qt(tau, alpha_q, None, True, smooth, h, 
+                    method, solver, qt_tol, options)
+            qt_fit = self.qt_fit
+        else:
+            self.qt_fit = qt_fit
+
         Z = np.minimum(self.Y - self.qt_fit, 0)/tau + self.qt_fit
         if self.kernel == 'polynomial':
             self.params['gamma'] = None
         self.es_model = KR(alpha = alpha_e, kernel=self.kernel, 
                            gamma = self.params['gamma'],
                            degree = self.params['degree'],
                            coef0 = self.params['coef0'])
@@ -832,20 +813,30 @@
 
 ###############################################################################
 ######################### Neural Network Regression ###########################
 ###############################################################################
 class ANN:
     '''
     Artificial Neural Network Regression
+    
+    Methods:
+        __init__(): Initialize the ANN object
+        plot_losses(): Plot the training and validation losses
+        qt(): Fit (smoothed) quantile neural network regression
+        es(): Fit (robust) expected shortfall neural network regression
+        mean() : Fit mean neural network regression
+        predict(): Compute predicted  outcomes at test data
+        trainer(): Train the neural network model
     '''
     optimizers = ["sgd", "adam"]
     activations = ["sigmoid", "tanh", "relu", "leakyrelu"]
     params = {'batch_size' : 64, 'val_pct' : .25, 'step_size': 10,
               'activation' : 'relu', 'depth': 4, 'width': 256,  
-              'optimizer' : 'adam', 'lr': 1e-3, 'lr_decay': 1., 'n_epochs' : 200,
+              'optimizer' : 'adam', 'lr': 1e-3, 
+              'lr_decay': 1., 'n_epochs' : 200,
               'dropout_rate': 0.1, 'Lambda': .0, 'weight_decay': .0, 
               'momentum': 0.9, 'nesterov': True}
 
 
     def __init__(self, X, Y, normalization=None):
         '''
         Args:
@@ -1136,14 +1127,43 @@
         if f(tau) > 0:
             tmin = tau
         else: 
             tmax = tau
     return tau
 
 
+def G2(G2_type=1):
+    '''
+        Specification Function G2 in Fissler and Ziegel's Joint Loss 
+    '''
+    if G2_type == 1:
+        f0 = lambda x : -np.sqrt(-x)
+        f1 = lambda x : 0.5 / np.sqrt(-x)
+        f2 = lambda x : 0.25 / np.sqrt((-x)**3)
+    elif G2_type == 2:
+        f0 = lambda x : -np.log(-x)
+        f1 = lambda x : -1 / x
+        f2 = lambda x : 1 / x ** 2
+    elif G2_type == 3:
+        f0 = lambda x : -1 / x
+        f1 = lambda x : 1 / x ** 2
+        f2 = lambda x : -2 / x ** 3
+    elif G2_type == 4:
+        f0 = lambda x : np.log( 1 + np.exp(x))
+        f1 = lambda x : np.exp(x) / (1 + np.exp(x))
+        f2 = lambda x : np.exp(x) / (1 + np.exp(x)) ** 2
+    elif G2_type == 5:
+        f0 = lambda x : np.exp(x)
+        f1 = lambda x : np.exp(x)
+        f2 = lambda x : np.exp(x) 
+    else:
+        raise ValueError("G2_type must be an integer between 1 and 5")
+    return f0, f1, f2 
+
+
 def make_train_step_fn(model, loss_fn, optimizer):
     '''
     Builds function that performs a step in the training loop
     '''
     def perform_train_step_fn(x, y):
         model.train()
         yhat = model(x)
```

### Comparing `quantes-2.0.3/quantes/linear.py` & `quantes-2.0.4/quantes/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -924,15 +924,15 @@
         
         if standardize and adjust:
             beta0[self.itcp:] = beta0[self.itcp:]/self.sdX
             if self.itcp: beta0[0] -= self.mX.dot(beta0[1:])
         nit_seq = np.array(nit_seq)
             
         return {'beta': beta0, 'res': res, 'nstep': step, 'lambda': Lambda,
-                'niter': np.sum(nit_seq), 'nit_seq': nit_seq}
+                'niter': np.sum(nit_seq), 'nit_seq': nit_seq, 'bw': h}
 
 
     def irw_als(self, tau=0.5, Lambda=np.array([]), robust=3,
                 penalty="SCAD", a=3.7, nstep=3,
                 standardize=True, adjust=True):
         '''
             Iteratively Reweighted L1-Penalized Asymmetric Least Squares 
@@ -960,15 +960,16 @@
             beta0, res = model['beta'], model['res']
             step += 1
         
         if standardize and adjust:
             beta0[self.itcp:] = beta0[self.itcp:]/self.sdX
             if self.itcp: beta0[0] -= self.mX.dot(beta0[1:])
             
-        return {'beta': beta0, 'res': res, 'nstep': step, 'lambda': Lambda}
+        return {'beta': beta0, 'res': res, 'nstep': step, 
+                'lambda': Lambda, 'robust': robust}
     
 
     def l1_path(self, tau, 
                 lambda_seq=np.array([]), nlambda=50, order="descend",
                 h=None, kernel="Laplacian", 
                 standardize=True, adjust=True):
         '''
@@ -1025,16 +1026,17 @@
         if standardize and adjust:
             beta_seq[self.itcp:,] = beta_seq[self.itcp:,]/self.sdX[:,None]
             if self.itcp: beta_seq[0,:] -= self.mX.dot(beta_seq[1:,])
 
         return {'beta_seq': beta_seq, 
                 'res_seq': res_seq,
                 'size_seq': np.sum(beta_seq[self.itcp:,:] != 0, axis=0),
-                'lambda_seq': lambda_seq, \
-                'nit_seq': np.array(nit_seq), 'bw': h}
+                'lambda_seq': lambda_seq,
+                'nit_seq': np.array(nit_seq), 
+                'bw': h}
 
 
     def irw_path(self, tau, 
                  lambda_seq=np.array([]), nlambda=50, order="descend",
                  h=None, kernel="Laplacian",
                  penalty="SCAD", a=3.7, nstep=3, 
                  standardize=True, adjust=True):
@@ -1099,15 +1101,16 @@
             beta_seq[self.itcp:,] /= self.sdX[:,None]
             if self.itcp: beta_seq[0,:] -= self.mX.dot(beta_seq[1:,])
     
         return {'beta_seq': beta_seq, 
                 'res_seq': res_seq,
                 'size_seq': np.sum(beta_seq[self.itcp:,:] != 0, axis=0),
                 'lambda_seq': lambda_seq,
-                'nit_seq': np.array(nit_seq), 'bw': h}
+                'nit_seq': np.array(nit_seq),
+                'bw': h}
 
 
     def bic(self, tau=0.5, 
             lambda_seq=np.array([]), nlambda=100, order='descend',
             h=None, kernel="Laplacian", max_size=False, Cn=None,
             penalty="SCAD", a=3.7, nstep=3, 
             standardize=True, adjust=True):
@@ -1204,17 +1207,15 @@
                        default is FALSE.
             ncore : number of cores used for parallel computing.
         
         Returns:
             'boot_beta' : numpy array. 
                           1st column: penalized conquer estimate; 
                           2nd to last: bootstrap estimates.
-            
             'majority_vote' : selected model by majority vote.
-
             'intersection' : selected model by intersecting.
         '''
 
         if Lambda is None: 
             Lambda = 0.75*np.quantile(self.self_tuning(tau, standardize), 0.9)
         if h is None: h = self.bandwidth(tau) 
         if weight not in self.weights[:3]:
@@ -1262,16 +1263,16 @@
         
         ## Method 2: Intersection of all bootstrap models
         model2 = np.arange(self.p)
         for b in range(len(mb_beta[0,1:])):
             boot_model = np.where(mb_beta[self.itcp:,b+1] != 0)[0]
             model2 = np.intersect1d(model2, boot_model)
 
-        return {'boot_beta': mb_beta, \
-                'majority_vote': model1, \
+        return {'boot_beta': mb_beta,
+                'majority_vote': model1,
                 'intersection': model2}
 
 
     def boot_inference(self, tau=0.5, Lambda=None, 
                        h=None, kernel="Laplacian",
                        weight="Multinomial", alpha=0.05, 
                        penalty="SCAD", a=3.7, nstep=3,
@@ -1279,23 +1280,18 @@
         '''
             Post-Selection-Inference via Bootstrap
 
         Returns:
             'boot_beta' : numpy array. 
                           1st column: penalized conquer estimate; 
                           2nd to last: bootstrap estimates.
-            
             'majority_vote' : selected model by majority vote.
-
             'intersection' : selected model by intersecting.
-
             'percentile_ci' : numpy array. Percentile bootstrap CI.
-
             'pivotal_ci' : numpy array. Pivotal bootstrap CI.
-
             'normal_ci' : numpy array. Normal-based CI using bootstrap variance estimates.
         '''
 
         mb_model = self.boot_select(tau, Lambda, h, kernel, weight,
                                     penalty, a, nstep, standardize,
                                     parallel, ncore)
         
@@ -1543,15 +1539,14 @@
             else:
                 val_err[v,:] \
                     = np.array([smooth_check(Y_val - model['beta_seq'][0,l]*itcp
                                              - X_val@(model['beta_seq'][itcp:,l]),
                                              tau, h, kernel)
                                              for l in range(nlambda)])
 
-        
         cv_err = np.mean(val_err, axis=0)
         cv_min = min(cv_err)
         lambda_min = model['lambda_seq'][np.argmin(cv_err)]
 
         if penalty == "L1":
             if method == 'conquer':
                 cv_model = init.l1(tau, lambda_min, h, kernel,
@@ -1573,24 +1568,24 @@
                 'cv_res': cv_model['res'],
                 'lambda_min': lambda_min,
                 'lambda_seq': model['lambda_seq'],
                 'min_cv_err': cv_min,
                 'cv_err': cv_err}
 
 
+
 ##############################################################################
 ###### Use Validation Set to Choose the Regularization Parameter Lambda ######
 ##############################################################################
 class validate_lambda(cv_lambda):
     '''
         Train Penalized Conquer on a Validation Set
     '''
     penalties = ["L1", "SCAD", "MCP"]
     
-
     def __init__(self, X_train, Y_train, X_val, Y_val, 
                  intercept=True, options={}):
         self.n, self.p = X_train.shape
         self.X_train, self.Y_train = X_train, Y_train.reshape(self.n)
         self.X_val, self.Y_val = X_val, Y_val.reshape(len(Y_val))
         self.itcp = intercept
         self.params.update(options)
```

### Comparing `quantes-2.0.3/quantes.egg-info/PKG-INFO` & `quantes-2.0.4/quantes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quantes
-Version: 2.0.3
+Version: 2.0.4
 Summary: Convolution Smoothed Quantile and Expected Shortfall Regression
 Home-page: https://github.com/WenxinZhou/conquer
-Author: ['Wenxin Zhou', 'Huaning Liu']
-Author-email: ['wenxinz@uic.edu', 'huaning3@illinois.edu']
+Author: Wenxin Zhou
+Author-email: wenxinz@uic.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quantes-2.0.3/setup.py` & `quantes-2.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 install_requires = ['numpy', 'scipy', 'scikit-learn', 'qpsolvers', 'cvxopt', 'torch', 'matplotlib']
 
 setup(
     name='quantes',
-    version="2.0.3",
+    version="2.0.4",
     packages=find_packages(),
-    author=["Wenxin Zhou", "Huaning Liu"],
-    author_email=["wenxinz@uic.edu", "huaning3@illinois.edu"],
+    author="Wenxin Zhou",
+    author_email="wenxinz@uic.edu",
     description="Convolution Smoothed Quantile and Expected Shortfall Regression",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WenxinZhou/conquer",  # replace with the URL of your project
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

