# Comparing `tmp/quantes-2.0.4.tar.gz` & `tmp/quantes-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantes-2.0.4.tar", last modified: Tue Apr  2 01:57:57 2024, max compression
+gzip compressed data, was "quantes-2.0.5.tar", last modified: Tue Apr  2 02:06:27 2024, max compression
```

## Comparing `quantes-2.0.4.tar` & `quantes-2.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.790560 quantes-2.0.4/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    35149 2024-03-31 02:51:56.000000 quantes-2.0.4/LICENSE
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12284 2024-04-02 01:57:57.788226 quantes-2.0.4/PKG-INFO
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    11815 2024-04-01 04:05:46.000000 quantes-2.0.4/README.md
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.684303 quantes-2.0.4/quantes/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/__init__.py
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    49712 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/joint.py
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)   103370 2024-04-02 01:56:54.000000 quantes-2.0.4/quantes/linear.py
-drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:57:57.773483 quantes-2.0.4/quantes.egg-info/
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    12284 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/PKG-INFO
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      235 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/SOURCES.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        1 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/dependency_links.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       59 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/requires.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        8 2024-04-02 01:57:57.000000 quantes-2.0.4/quantes.egg-info/top_level.txt
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       38 2024-04-02 01:57:57.791630 quantes-2.0.4/setup.cfg
--rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      958 2024-04-02 01:57:10.000000 quantes-2.0.4/setup.py
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 02:06:27.107203 quantes-2.0.5/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    35149 2024-03-31 02:51:56.000000 quantes-2.0.5/LICENSE
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    15026 2024-04-02 02:06:27.106201 quantes-2.0.5/PKG-INFO
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    14557 2024-04-02 02:04:00.000000 quantes-2.0.5/README.md
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 02:06:27.037490 quantes-2.0.5/quantes/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 01:56:54.000000 quantes-2.0.5/quantes/__init__.py
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    49712 2024-04-02 01:56:54.000000 quantes-2.0.5/quantes/joint.py
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)   103370 2024-04-02 01:56:54.000000 quantes-2.0.5/quantes/linear.py
+drwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        0 2024-04-02 02:06:27.093843 quantes-2.0.5/quantes.egg-info/
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)    15026 2024-04-02 02:06:26.000000 quantes-2.0.5/quantes.egg-info/PKG-INFO
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      235 2024-04-02 02:06:26.000000 quantes-2.0.5/quantes.egg-info/SOURCES.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        1 2024-04-02 02:06:26.000000 quantes-2.0.5/quantes.egg-info/dependency_links.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       59 2024-04-02 02:06:26.000000 quantes-2.0.5/quantes.egg-info/requires.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)        8 2024-04-02 02:06:26.000000 quantes-2.0.5/quantes.egg-info/top_level.txt
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)       38 2024-04-02 02:06:27.108201 quantes-2.0.5/setup.cfg
+-rwxrwxrwx   0 h9liu     (1000) h9liu     (1000)      958 2024-04-02 02:06:13.000000 quantes-2.0.5/setup.py
```

### Comparing `quantes-2.0.4/LICENSE` & `quantes-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantes-2.0.4/PKG-INFO` & `quantes-2.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantes
-Version: 2.0.4
+Version: 2.0.5
 Summary: Convolution Smoothed Quantile and Expected Shortfall Regression
 Home-page: https://github.com/WenxinZhou/conquer
 Author: Wenxin Zhou
 Author-email: wenxinz@uic.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 This package contains two modules: the `linear` module, which implements convolution smoothed quantile regression in both low and high dimensions, and the `joint` module, designed for joint quantile and expected shortfall regression.
 
 The `low_dim` class in the `linear` module applies a convolution smoothing approach to fit linear quantile regression models, known as *conquer*. 
 It also constructs normal-based and (multiplier) bootstrap confidence intervals for all slope coefficients. The `high_dim` class fits sparse quantile regression models in high dimensions via *L<sub>1</sub>*-penalized and iteratively reweighted *L<sub>1</sub>*-penalized (IRW-*L<sub>1</sub>*) conquer methods. The IRW method is inspired by the local linear approximation (LLA) algorithm proposed by [Zou & Li (2008)](https://doi.org/10.1214/009053607000000802) for folded concave penalized estimation, exemplified by the SCAD penalty ([Fan & Li, 2001](https://fan.princeton.edu/papers/01/penlike.pdf)) and the minimax concave penalty (MCP) ([Zhang, 2010](https://doi.org/10.1214/09-AOS729)). Computationally, each weighted l<sub>1</sub>-penalized conquer estimator is solved using the local adaptive majorize-minimization algorithm ([LAMM](https://doi.org/10.1214/17-AOS1568)). For comparison, the proximal ADMM algorithm ([pADMM](https://doi.org/10.1080/00401706.2017.1345703)) is also implemented.
 
 The `LR` class in the `joint` module fits joint linear quantile and expected shortfall (ES) regression models ([Dimitriadis & Bayer, 2019](https://doi.org/10.1214/19-EJS1560); [Patton, Ziegel & Chen, 2019](https://doi.org/10.1016/j.jeconom.2018.10.008)) using either FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)) or two-step procedures ([Barendse, 2020](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2937665); [Peng & Wang, 2023](https://onlinelibrary.wiley.com/doi/10.1002/sta4.619); [He, Tan & Zhou, 2023](https://doi.org/10.1093/jrsssb/qkad063)). For the second step of ES estimation, setting ``robust=TRUE`` uses the Huber loss with an adaptively chosen robustification parameter to gain robustness against heavy-tailed error/response; see [He, Tan & Zhou (2023)](https://doi.org/10.1093/jrsssb/qkad063) for more details. Moreover, a combination of the iteratively reweighted least squares (IRLS) algorithm and quadratic programming is utilized to compute non-crossing ES estimates. This ensures that the fitted ES does not exceed the fitted quantile at each observation.
 
-The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al, 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
+The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
 
 
 ## Dependencies
 
 ```
 python >= 3.9, numpy, scipy, scikit-learn, cvxopt, qpsolvers, torch
 optional: matplotlib
@@ -136,15 +136,15 @@
 ## solution path of l1-penalized QR
 l1_admm_path = admm.l1_path(tau=tau, lambda_seq=lambda_seq)
 
 ## solution path of irw-l1-penalized QR
 irw_admm_path = admm.irw_path(tau=tau, lambda_seq=lambda_seq)
 ```
 
-The class `QuantES` in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
+The `LR` class in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
 
 ```
 import numpy as np
 import pandas as pd
 import numpy.random as rgt
 from quantes.joint import LR
 
@@ -183,14 +183,65 @@
 
 out = pd.DataFrame(np.c_[(m1['coef_e'], m2['coef_e'], m3['coef_e'], m4['coef_e'], 
                           m5['coef_e'], m6['coef_e'], m7['coef_e'], m8['coef_e'])], 
                    columns=['L2', 'TLS', 'FZ', 'AH', 'NC-L2', 'NC-AH', 'Joint0', 'Joint1'])
 out
 ```
 
+The `KRR` class in `conquer.joint` contains functions to compute quantile and expected shortfall kernel ridge regression (KRR) estimators, respectively. Recast as a quadratic program ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)), the `qt()` function computes quantile KRR using QP solvers from `qpsolvers` ([Caron et al., 2024](https://pypi.org/project/qpsolvers/)). Setting `smooth=TRUE`, a convolution-smoothed quantile KRR is computed by the BFGS algorithm using `scipy.optimize.minimize`. By plugging in estimated quantiles, the two-step ES KRR estimator and its robust counterpart (using the *Huber loss*) are computed by the `es()` function with `robust=FALSE` and `robust=TRUE`, respectively. The functions `mean()`, `qt()` and `es()` from the `ANN` class in `conquer.joint` compute nonparametric mean, quantile and expected shortfall regression estimators using feedforward neural networks, respectively. 
+
+```
+import numpy as np
+import numpy.random as rgt
+from scipy.stats import norm
+from quantes.joint import KRR, ANN
+
+mean_fn = lambda x: np.cos(2*np.pi*(x[:,0])) \
+                    + (1 + np.exp(-x[:,1]-x[:,2]))**(-1) + (1 + x[:,3] \
+                    + x[:,4])**(-3) + (x[:,5] + np.exp(x[:,6]*x[:,7]))**(-1)
+std_fn = lambda x: np.sin(np.pi*(x[:,0] + x[:,1])*0.5) \
+                   + np.log(1 + (x[:,2]*x[:,3]*x[:,4])**2) \
+                   + x[:,7]*(1 + np.exp(-x[:,5]-x[:,6]))**(-1)
+n, p = 2048, 8
+X = rgt.uniform(0, 1, (n, p))
+Y = mean_fn(X) + std_fn(X)*rgt.normal(0, 1, n)
+tau = 0.2
+qt = norm.ppf(tau)
+es = norm.expect(lambda x : (x if x < qt else 0))/tau
+
+X_test = rgt.uniform(0, 1, (4096, p))
+mean_test = mean_fn(X_test)
+qt_test = mean_test + std_fn(X_test)*qt
+es_test = mean_test + std_fn(X_test)*es
+
+kr = KRR(X, Y, kernel='polynomial', 
+         kernel_params={'degree': 3, 'gamma': 1, 'coef0': 1})
+kr.qt(tau=tau, alpha_q=1, solver='cvxopt')
+qt_pred = kr.qt_predict(X_test)
+print('Mean squared prediction error of quantile KRR:', np.mean((qt_test - qt_pred)**2))
+
+kr.lses(tau=tau, alpha_q=1, alpha_e=1, solver='cvxopt')
+es_pred = kr.es_predict(X_test)
+print('Mean squared prediction error of ES KRR:', np.mean((es_test - es_pred)**2))
+
+args = {'batch_size': 128, 'val_pct': .125, 
+        'activation': 'relu', 'depth': 4, 'width': 64,
+        'optimizer': 'adam', 'lr': .001, 
+        'n_epochs': 200, 'dropout_rate': .0}
+nn = ANN(X, Y)
+nn.qt(tau=tau, options=args, device='cpu')
+qt_pred = nn.predict(X_test)
+qt_fit = nn.fit
+print('Mean squared prediction error of quantile NN:', np.mean((qt_test - qt_pred)**2))
+
+nn.es(tau=tau, plot=True, qt_fit=qt_fit, options=args)
+es_pred = nn.predict(X_test)
+print('Mean squared prediction error of ES NN:', np.mean((es_test - es_pred)**2))
+```
+
 
 ## References
 
 Fernandes, M., Guerre, E. and Horta, E. (2021). Smoothing quantile regressions. *J. Bus. Econ. Statist.* **39**(1) 338–357. [Paper](https://doi.org/10.1080/07350015.2019.1660177)
 
 He, X., Tan, K. M. and Zhou, W.-X. (2023). Robust estimation and inference for expected shortfall regression with many regressors. *J. R. Stat. Soc. B.* **85**(4) 1223-1246. [Paper](https://doi.org/10.1093/jrsssb/qkad063)
```

### Comparing `quantes-2.0.4/README.md` & `quantes-2.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This package contains two modules: the `linear` module, which implements convolution smoothed quantile regression in both low and high dimensions, and the `joint` module, designed for joint quantile and expected shortfall regression.
 
 The `low_dim` class in the `linear` module applies a convolution smoothing approach to fit linear quantile regression models, known as *conquer*. 
 It also constructs normal-based and (multiplier) bootstrap confidence intervals for all slope coefficients. The `high_dim` class fits sparse quantile regression models in high dimensions via *L<sub>1</sub>*-penalized and iteratively reweighted *L<sub>1</sub>*-penalized (IRW-*L<sub>1</sub>*) conquer methods. The IRW method is inspired by the local linear approximation (LLA) algorithm proposed by [Zou & Li (2008)](https://doi.org/10.1214/009053607000000802) for folded concave penalized estimation, exemplified by the SCAD penalty ([Fan & Li, 2001](https://fan.princeton.edu/papers/01/penlike.pdf)) and the minimax concave penalty (MCP) ([Zhang, 2010](https://doi.org/10.1214/09-AOS729)). Computationally, each weighted l<sub>1</sub>-penalized conquer estimator is solved using the local adaptive majorize-minimization algorithm ([LAMM](https://doi.org/10.1214/17-AOS1568)). For comparison, the proximal ADMM algorithm ([pADMM](https://doi.org/10.1080/00401706.2017.1345703)) is also implemented.
 
 The `LR` class in the `joint` module fits joint linear quantile and expected shortfall (ES) regression models ([Dimitriadis & Bayer, 2019](https://doi.org/10.1214/19-EJS1560); [Patton, Ziegel & Chen, 2019](https://doi.org/10.1016/j.jeconom.2018.10.008)) using either FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)) or two-step procedures ([Barendse, 2020](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2937665); [Peng & Wang, 2023](https://onlinelibrary.wiley.com/doi/10.1002/sta4.619); [He, Tan & Zhou, 2023](https://doi.org/10.1093/jrsssb/qkad063)). For the second step of ES estimation, setting ``robust=TRUE`` uses the Huber loss with an adaptively chosen robustification parameter to gain robustness against heavy-tailed error/response; see [He, Tan & Zhou (2023)](https://doi.org/10.1093/jrsssb/qkad063) for more details. Moreover, a combination of the iteratively reweighted least squares (IRLS) algorithm and quadratic programming is utilized to compute non-crossing ES estimates. This ensures that the fitted ES does not exceed the fitted quantile at each observation.
 
-The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al, 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
+The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
 
 
 ## Dependencies
 
 ```
 python >= 3.9, numpy, scipy, scikit-learn, cvxopt, qpsolvers, torch
 optional: matplotlib
@@ -121,15 +121,15 @@
 ## solution path of l1-penalized QR
 l1_admm_path = admm.l1_path(tau=tau, lambda_seq=lambda_seq)
 
 ## solution path of irw-l1-penalized QR
 irw_admm_path = admm.irw_path(tau=tau, lambda_seq=lambda_seq)
 ```
 
-The class `QuantES` in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
+The `LR` class in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
 
 ```
 import numpy as np
 import pandas as pd
 import numpy.random as rgt
 from quantes.joint import LR
 
@@ -168,14 +168,65 @@
 
 out = pd.DataFrame(np.c_[(m1['coef_e'], m2['coef_e'], m3['coef_e'], m4['coef_e'], 
                           m5['coef_e'], m6['coef_e'], m7['coef_e'], m8['coef_e'])], 
                    columns=['L2', 'TLS', 'FZ', 'AH', 'NC-L2', 'NC-AH', 'Joint0', 'Joint1'])
 out
 ```
 
+The `KRR` class in `conquer.joint` contains functions to compute quantile and expected shortfall kernel ridge regression (KRR) estimators, respectively. Recast as a quadratic program ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)), the `qt()` function computes quantile KRR using QP solvers from `qpsolvers` ([Caron et al., 2024](https://pypi.org/project/qpsolvers/)). Setting `smooth=TRUE`, a convolution-smoothed quantile KRR is computed by the BFGS algorithm using `scipy.optimize.minimize`. By plugging in estimated quantiles, the two-step ES KRR estimator and its robust counterpart (using the *Huber loss*) are computed by the `es()` function with `robust=FALSE` and `robust=TRUE`, respectively. The functions `mean()`, `qt()` and `es()` from the `ANN` class in `conquer.joint` compute nonparametric mean, quantile and expected shortfall regression estimators using feedforward neural networks, respectively. 
+
+```
+import numpy as np
+import numpy.random as rgt
+from scipy.stats import norm
+from quantes.joint import KRR, ANN
+
+mean_fn = lambda x: np.cos(2*np.pi*(x[:,0])) \
+                    + (1 + np.exp(-x[:,1]-x[:,2]))**(-1) + (1 + x[:,3] \
+                    + x[:,4])**(-3) + (x[:,5] + np.exp(x[:,6]*x[:,7]))**(-1)
+std_fn = lambda x: np.sin(np.pi*(x[:,0] + x[:,1])*0.5) \
+                   + np.log(1 + (x[:,2]*x[:,3]*x[:,4])**2) \
+                   + x[:,7]*(1 + np.exp(-x[:,5]-x[:,6]))**(-1)
+n, p = 2048, 8
+X = rgt.uniform(0, 1, (n, p))
+Y = mean_fn(X) + std_fn(X)*rgt.normal(0, 1, n)
+tau = 0.2
+qt = norm.ppf(tau)
+es = norm.expect(lambda x : (x if x < qt else 0))/tau
+
+X_test = rgt.uniform(0, 1, (4096, p))
+mean_test = mean_fn(X_test)
+qt_test = mean_test + std_fn(X_test)*qt
+es_test = mean_test + std_fn(X_test)*es
+
+kr = KRR(X, Y, kernel='polynomial', 
+         kernel_params={'degree': 3, 'gamma': 1, 'coef0': 1})
+kr.qt(tau=tau, alpha_q=1, solver='cvxopt')
+qt_pred = kr.qt_predict(X_test)
+print('Mean squared prediction error of quantile KRR:', np.mean((qt_test - qt_pred)**2))
+
+kr.lses(tau=tau, alpha_q=1, alpha_e=1, solver='cvxopt')
+es_pred = kr.es_predict(X_test)
+print('Mean squared prediction error of ES KRR:', np.mean((es_test - es_pred)**2))
+
+args = {'batch_size': 128, 'val_pct': .125, 
+        'activation': 'relu', 'depth': 4, 'width': 64,
+        'optimizer': 'adam', 'lr': .001, 
+        'n_epochs': 200, 'dropout_rate': .0}
+nn = ANN(X, Y)
+nn.qt(tau=tau, options=args, device='cpu')
+qt_pred = nn.predict(X_test)
+qt_fit = nn.fit
+print('Mean squared prediction error of quantile NN:', np.mean((qt_test - qt_pred)**2))
+
+nn.es(tau=tau, plot=True, qt_fit=qt_fit, options=args)
+es_pred = nn.predict(X_test)
+print('Mean squared prediction error of ES NN:', np.mean((es_test - es_pred)**2))
+```
+
 
 ## References
 
 Fernandes, M., Guerre, E. and Horta, E. (2021). Smoothing quantile regressions. *J. Bus. Econ. Statist.* **39**(1) 338–357. [Paper](https://doi.org/10.1080/07350015.2019.1660177)
 
 He, X., Tan, K. M. and Zhou, W.-X. (2023). Robust estimation and inference for expected shortfall regression with many regressors. *J. R. Stat. Soc. B.* **85**(4) 1223-1246. [Paper](https://doi.org/10.1093/jrsssb/qkad063)
```

### Comparing `quantes-2.0.4/quantes/joint.py` & `quantes-2.0.5/quantes/joint.py`

 * *Files identical despite different names*

### Comparing `quantes-2.0.4/quantes/linear.py` & `quantes-2.0.5/quantes/linear.py`

 * *Files identical despite different names*

### Comparing `quantes-2.0.4/quantes.egg-info/PKG-INFO` & `quantes-2.0.5/quantes.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantes
-Version: 2.0.4
+Version: 2.0.5
 Summary: Convolution Smoothed Quantile and Expected Shortfall Regression
 Home-page: https://github.com/WenxinZhou/conquer
 Author: Wenxin Zhou
 Author-email: wenxinz@uic.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 This package contains two modules: the `linear` module, which implements convolution smoothed quantile regression in both low and high dimensions, and the `joint` module, designed for joint quantile and expected shortfall regression.
 
 The `low_dim` class in the `linear` module applies a convolution smoothing approach to fit linear quantile regression models, known as *conquer*. 
 It also constructs normal-based and (multiplier) bootstrap confidence intervals for all slope coefficients. The `high_dim` class fits sparse quantile regression models in high dimensions via *L<sub>1</sub>*-penalized and iteratively reweighted *L<sub>1</sub>*-penalized (IRW-*L<sub>1</sub>*) conquer methods. The IRW method is inspired by the local linear approximation (LLA) algorithm proposed by [Zou & Li (2008)](https://doi.org/10.1214/009053607000000802) for folded concave penalized estimation, exemplified by the SCAD penalty ([Fan & Li, 2001](https://fan.princeton.edu/papers/01/penlike.pdf)) and the minimax concave penalty (MCP) ([Zhang, 2010](https://doi.org/10.1214/09-AOS729)). Computationally, each weighted l<sub>1</sub>-penalized conquer estimator is solved using the local adaptive majorize-minimization algorithm ([LAMM](https://doi.org/10.1214/17-AOS1568)). For comparison, the proximal ADMM algorithm ([pADMM](https://doi.org/10.1080/00401706.2017.1345703)) is also implemented.
 
 The `LR` class in the `joint` module fits joint linear quantile and expected shortfall (ES) regression models ([Dimitriadis & Bayer, 2019](https://doi.org/10.1214/19-EJS1560); [Patton, Ziegel & Chen, 2019](https://doi.org/10.1016/j.jeconom.2018.10.008)) using either FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)) or two-step procedures ([Barendse, 2020](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2937665); [Peng & Wang, 2023](https://onlinelibrary.wiley.com/doi/10.1002/sta4.619); [He, Tan & Zhou, 2023](https://doi.org/10.1093/jrsssb/qkad063)). For the second step of ES estimation, setting ``robust=TRUE`` uses the Huber loss with an adaptively chosen robustification parameter to gain robustness against heavy-tailed error/response; see [He, Tan & Zhou (2023)](https://doi.org/10.1093/jrsssb/qkad063) for more details. Moreover, a combination of the iteratively reweighted least squares (IRLS) algorithm and quadratic programming is utilized to compute non-crossing ES estimates. This ensures that the fitted ES does not exceed the fitted quantile at each observation.
 
-The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al, 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
+The `KRR` and `ANN` classes in the `joint` module implement two nonparametric methods for joint quantile and expected shortfall regressions: kernel ridge regression ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)) and neural network regression. For fitting nonparametric QR through the `qt()` method in both `KRR` and `ANN`, there is a `smooth` option available. When set to `TRUE`, it uses the Gaussian kernel convoluted check loss. For fitting nonparametric ES regression using nonparametrically generated surrogate response variables, the `es()` function provides two options: *squared loss* (`robust=FALSE`) and the *Huber loss* (`robust=TRUE`).
 
 
 ## Dependencies
 
 ```
 python >= 3.9, numpy, scipy, scikit-learn, cvxopt, qpsolvers, torch
 optional: matplotlib
@@ -136,15 +136,15 @@
 ## solution path of l1-penalized QR
 l1_admm_path = admm.l1_path(tau=tau, lambda_seq=lambda_seq)
 
 ## solution path of irw-l1-penalized QR
 irw_admm_path = admm.irw_path(tau=tau, lambda_seq=lambda_seq)
 ```
 
-The class `QuantES` in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
+The `LR` class in `conquer.joint` contains functions that fit joint (linear) quantile and expected shortfall models. The `joint_fit` function computes joint quantile and ES regression estimates based on FZ loss minimization ([Fissler & Ziegel, 2016](https://doi.org/10.1214/16-AOS1439)). The `twostep_fit` function implements two-stage procesures to compute quantile and ES regression estimates, with the ES part depending on a user-specified `loss`. Options are ``L2``, ``TrunL2``, ``FZ`` and ``Huber``. The `nc_fit` function computes non-crossing counterparts of the ES estimates when `loss` = `L2` or `Huber`.
 
 ```
 import numpy as np
 import pandas as pd
 import numpy.random as rgt
 from quantes.joint import LR
 
@@ -183,14 +183,65 @@
 
 out = pd.DataFrame(np.c_[(m1['coef_e'], m2['coef_e'], m3['coef_e'], m4['coef_e'], 
                           m5['coef_e'], m6['coef_e'], m7['coef_e'], m8['coef_e'])], 
                    columns=['L2', 'TLS', 'FZ', 'AH', 'NC-L2', 'NC-AH', 'Joint0', 'Joint1'])
 out
 ```
 
+The `KRR` class in `conquer.joint` contains functions to compute quantile and expected shortfall kernel ridge regression (KRR) estimators, respectively. Recast as a quadratic program ([Takeuchi et al., 2006](https://www.jmlr.org/papers/v7/takeuchi06a.html)), the `qt()` function computes quantile KRR using QP solvers from `qpsolvers` ([Caron et al., 2024](https://pypi.org/project/qpsolvers/)). Setting `smooth=TRUE`, a convolution-smoothed quantile KRR is computed by the BFGS algorithm using `scipy.optimize.minimize`. By plugging in estimated quantiles, the two-step ES KRR estimator and its robust counterpart (using the *Huber loss*) are computed by the `es()` function with `robust=FALSE` and `robust=TRUE`, respectively. The functions `mean()`, `qt()` and `es()` from the `ANN` class in `conquer.joint` compute nonparametric mean, quantile and expected shortfall regression estimators using feedforward neural networks, respectively. 
+
+```
+import numpy as np
+import numpy.random as rgt
+from scipy.stats import norm
+from quantes.joint import KRR, ANN
+
+mean_fn = lambda x: np.cos(2*np.pi*(x[:,0])) \
+                    + (1 + np.exp(-x[:,1]-x[:,2]))**(-1) + (1 + x[:,3] \
+                    + x[:,4])**(-3) + (x[:,5] + np.exp(x[:,6]*x[:,7]))**(-1)
+std_fn = lambda x: np.sin(np.pi*(x[:,0] + x[:,1])*0.5) \
+                   + np.log(1 + (x[:,2]*x[:,3]*x[:,4])**2) \
+                   + x[:,7]*(1 + np.exp(-x[:,5]-x[:,6]))**(-1)
+n, p = 2048, 8
+X = rgt.uniform(0, 1, (n, p))
+Y = mean_fn(X) + std_fn(X)*rgt.normal(0, 1, n)
+tau = 0.2
+qt = norm.ppf(tau)
+es = norm.expect(lambda x : (x if x < qt else 0))/tau
+
+X_test = rgt.uniform(0, 1, (4096, p))
+mean_test = mean_fn(X_test)
+qt_test = mean_test + std_fn(X_test)*qt
+es_test = mean_test + std_fn(X_test)*es
+
+kr = KRR(X, Y, kernel='polynomial', 
+         kernel_params={'degree': 3, 'gamma': 1, 'coef0': 1})
+kr.qt(tau=tau, alpha_q=1, solver='cvxopt')
+qt_pred = kr.qt_predict(X_test)
+print('Mean squared prediction error of quantile KRR:', np.mean((qt_test - qt_pred)**2))
+
+kr.lses(tau=tau, alpha_q=1, alpha_e=1, solver='cvxopt')
+es_pred = kr.es_predict(X_test)
+print('Mean squared prediction error of ES KRR:', np.mean((es_test - es_pred)**2))
+
+args = {'batch_size': 128, 'val_pct': .125, 
+        'activation': 'relu', 'depth': 4, 'width': 64,
+        'optimizer': 'adam', 'lr': .001, 
+        'n_epochs': 200, 'dropout_rate': .0}
+nn = ANN(X, Y)
+nn.qt(tau=tau, options=args, device='cpu')
+qt_pred = nn.predict(X_test)
+qt_fit = nn.fit
+print('Mean squared prediction error of quantile NN:', np.mean((qt_test - qt_pred)**2))
+
+nn.es(tau=tau, plot=True, qt_fit=qt_fit, options=args)
+es_pred = nn.predict(X_test)
+print('Mean squared prediction error of ES NN:', np.mean((es_test - es_pred)**2))
+```
+
 
 ## References
 
 Fernandes, M., Guerre, E. and Horta, E. (2021). Smoothing quantile regressions. *J. Bus. Econ. Statist.* **39**(1) 338–357. [Paper](https://doi.org/10.1080/07350015.2019.1660177)
 
 He, X., Tan, K. M. and Zhou, W.-X. (2023). Robust estimation and inference for expected shortfall regression with many regressors. *J. R. Stat. Soc. B.* **85**(4) 1223-1246. [Paper](https://doi.org/10.1093/jrsssb/qkad063)
```

### Comparing `quantes-2.0.4/setup.py` & `quantes-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 install_requires = ['numpy', 'scipy', 'scikit-learn', 'qpsolvers', 'cvxopt', 'torch', 'matplotlib']
 
 setup(
     name='quantes',
-    version="2.0.4",
+    version="2.0.5",
     packages=find_packages(),
     author="Wenxin Zhou",
     author_email="wenxinz@uic.edu",
     description="Convolution Smoothed Quantile and Expected Shortfall Regression",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WenxinZhou/conquer",  # replace with the URL of your project
```

