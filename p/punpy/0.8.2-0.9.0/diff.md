# Comparing `tmp/punpy-0.8.2.tar.gz` & `tmp/punpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\punpy-0.8.2.tar", last modified: Wed Oct 21 13:34:14 2020, max compression
+gzip compressed data, was "dist\punpy-0.9.0.tar", last modified: Wed Nov 18 12:17:35 2020, max compression
```

## Comparing `punpy-0.8.2.tar` & `punpy-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.895905 punpy-0.8.2/
--rw-rw-rw-   0        0        0       50 2020-09-04 14:53:18.000000 punpy-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2124 2020-10-21 13:34:14.896903 punpy-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1190 2020-09-04 14:53:18.000000 punpy-0.8.2/README.rst
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.834073 punpy-0.8.2/punpy/
--rw-rw-rw-   0        0        0      397 2020-10-05 16:36:29.000000 punpy-0.8.2/punpy/__init__.py
--rw-rw-rw-   0        0        0    18962 2020-09-04 16:32:19.000000 punpy-0.8.2/punpy/_version.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.860001 punpy-0.8.2/punpy/jacobian/
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/jacobian/__init__.py
--rw-rw-rw-   0        0        0    11249 2020-10-02 17:22:16.000000 punpy-0.8.2/punpy/jacobian/jacobian_propagation.py
--rw-rw-rw-   0        0        0     3557 2020-10-20 17:00:22.000000 punpy-0.8.2/punpy/jacobian/jacobian_retrieval.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.865986 punpy-0.8.2/punpy/jacobian/tests/
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/jacobian/tests/__init__.py
--rw-rw-rw-   0        0        0     9223 2020-10-05 17:42:43.000000 punpy-0.8.2/punpy/jacobian/tests/test_jacobian_propagation.py
--rw-rw-rw-   0        0        0        0 2020-07-01 12:19:25.000000 punpy-0.8.2/punpy/main.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.876038 punpy-0.8.2/punpy/mc/
--rw-rw-rw-   0        0        0     4292 2020-10-21 13:33:55.000000 punpy-0.8.2/punpy/mc/MCMC_retrieval.py
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/mc/__init__.py
--rw-rw-rw-   0        0        0    33532 2020-10-20 17:48:40.000000 punpy-0.8.2/punpy/mc/mc_propagation.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.882940 punpy-0.8.2/punpy/mc/tests/
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/mc/tests/__init__.py
--rw-rw-rw-   0        0        0    10299 2020-10-20 16:04:33.000000 punpy-0.8.2/punpy/mc/tests/test_mc_propagation.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.888924 punpy-0.8.2/punpy/utilities/
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.892916 punpy-0.8.2/punpy/utilities/tests/
--rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.8.2/punpy/utilities/tests/__init__.py
--rw-rw-rw-   0        0        0     1693 2020-09-28 15:01:59.000000 punpy-0.8.2/punpy/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2020-10-21 13:34:14.850029 punpy-0.8.2/punpy.egg-info/
--rw-rw-rw-   0        0        0     2124 2020-10-21 13:34:14.000000 punpy-0.8.2/punpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2020-10-21 13:34:14.000000 punpy-0.8.2/punpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-21 13:34:14.000000 punpy-0.8.2/punpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2020-10-21 13:34:14.000000 punpy-0.8.2/punpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-10-21 13:34:14.000000 punpy-0.8.2/punpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      463 2020-10-21 13:34:14.898897 punpy-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1253 2020-10-21 13:34:12.000000 punpy-0.8.2/setup.py
--rw-rw-rw-   0        0        0    68611 2020-09-04 16:32:19.000000 punpy-0.8.2/versioneer.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.425934 punpy-0.9.0/
+-rw-rw-rw-   0        0        0       50 2020-09-04 14:53:18.000000 punpy-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2124 2020-11-18 12:17:35.426931 punpy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1190 2020-09-04 14:53:18.000000 punpy-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.360115 punpy-0.9.0/punpy/
+-rw-rw-rw-   0        0        0      618 2020-11-18 12:09:29.000000 punpy-0.9.0/punpy/__init__.py
+-rw-rw-rw-   0        0        0    18962 2020-09-04 16:32:19.000000 punpy-0.9.0/punpy/_version.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.391666 punpy-0.9.0/punpy/jacobian/
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/jacobian/__init__.py
+-rw-rw-rw-   0        0        0    11249 2020-10-02 17:22:16.000000 punpy-0.9.0/punpy/jacobian/jacobian_propagation.py
+-rw-rw-rw-   0        0        0     3557 2020-10-20 17:00:22.000000 punpy-0.9.0/punpy/jacobian/jacobian_retrieval.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.397015 punpy-0.9.0/punpy/jacobian/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/jacobian/tests/__init__.py
+-rw-rw-rw-   0        0        0     9223 2020-10-05 17:42:43.000000 punpy-0.9.0/punpy/jacobian/tests/test_jacobian_propagation.py
+-rw-rw-rw-   0        0        0        0 2020-07-01 12:19:25.000000 punpy-0.9.0/punpy/main.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.407981 punpy-0.9.0/punpy/mc/
+-rw-rw-rw-   0        0        0     4292 2020-10-21 13:33:55.000000 punpy-0.9.0/punpy/mc/MCMC_retrieval.py
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/mc/__init__.py
+-rw-rw-rw-   0        0        0    38275 2020-11-18 12:12:16.000000 punpy-0.9.0/punpy/mc/mc_propagation.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.413966 punpy-0.9.0/punpy/mc/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/mc/tests/__init__.py
+-rw-rw-rw-   0        0        0    10299 2020-10-20 16:04:33.000000 punpy-0.9.0/punpy/mc/tests/test_mc_propagation.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.420947 punpy-0.9.0/punpy/utilities/
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.422941 punpy-0.9.0/punpy/utilities/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-15 19:12:35.000000 punpy-0.9.0/punpy/utilities/tests/__init__.py
+-rw-rw-rw-   0        0        0     1693 2020-09-28 15:01:59.000000 punpy-0.9.0/punpy/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2020-11-18 12:17:35.380059 punpy-0.9.0/punpy.egg-info/
+-rw-rw-rw-   0        0        0     2124 2020-11-18 12:17:34.000000 punpy-0.9.0/punpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2020-11-18 12:17:35.000000 punpy-0.9.0/punpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-11-18 12:17:34.000000 punpy-0.9.0/punpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2020-11-18 12:17:34.000000 punpy-0.9.0/punpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2020-11-18 12:17:34.000000 punpy-0.9.0/punpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      463 2020-11-18 12:17:35.428999 punpy-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2020-11-18 12:17:32.000000 punpy-0.9.0/setup.py
+-rw-rw-rw-   0        0        0    68611 2020-09-04 16:32:19.000000 punpy-0.9.0/versioneer.py
```

### Comparing `punpy-0.8.2/PKG-INFO` & `punpy-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punpy
-Version: 0.8.2
+Version: 0.9.0
 Summary: Propagating UNcertainties in PYthon
 Home-page: https://gitlab.npl.co.uk/eco/eo/punpy
 Author: Pieter De Vis
 Author-email: pieter.de.vis@npl.co.uk
 License: None
 Description: punpy
         =====
```

### Comparing `punpy-0.8.2/README.rst` & `punpy-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/_version.py` & `punpy-0.9.0/punpy/_version.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/jacobian/jacobian_propagation.py` & `punpy-0.9.0/punpy/jacobian/jacobian_propagation.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/jacobian/jacobian_retrieval.py` & `punpy-0.9.0/punpy/jacobian/jacobian_retrieval.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/jacobian/tests/test_jacobian_propagation.py` & `punpy-0.9.0/punpy/jacobian/tests/test_jacobian_propagation.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/mc/MCMC_retrieval.py` & `punpy-0.9.0/punpy/mc/MCMC_retrieval.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/mc/mc_propagation.py` & `punpy-0.9.0/punpy/mc/mc_propagation.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         """
 
         self.MCsteps = steps
         self.parallel_cores = parallel_cores
         if parallel_cores>1:
             self.pool=Pool(parallel_cores)
 
-    def propagate_random(self,func,x,u_x,cov_x=None,param_fixed=None,corr_between=None,return_corr=False,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1):
+    def propagate_random(self,func,x,u_x,cov_x=None,param_fixed=None,corr_between=None,return_corr=False,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1,PD_corr=True):
         """
         Propagate random uncertainties through measurement function with n input quantities.
         Input quantities can be floats, vectors (1d-array) or images (2d-array).
         Random uncertainties arise when there is no correlation between repeated measurements.
         It is possible (though rare) that there is a correlation in one of the dimensions that is not one of the repeat_dims.
 
         :param func: measurement function
@@ -61,34 +61,46 @@
                                                                            output_vars)
         if repeat_axis >= 0:
             n_repeats=yshape[repeat_axis]
             outs = np.empty(n_repeats,dtype=object)
             for i in range(n_repeats):
                 xb, u_xb = self.select_repeated_x(x,u_x,param_fixed,i,repeat_axis,n_repeats)
                 outs[i] = self.propagate_random(func,xb,u_xb,cov_x,param_fixed,corr_between,return_corr,
-                                                return_samples,repeat_dims,corr_axis=corr_axis,output_vars=output_vars)
+                                                return_samples,repeat_dims,corr_axis=corr_axis,output_vars=output_vars,PD_corr=False)
             return self.combine_repeated_outs(outs,yshape,n_repeats,len(x),repeat_axis,return_corr,return_samples,output_vars)
 
         else:
             MC_data = np.empty(len(x),dtype=np.ndarray)
             for i in range(len(x)):
                 if cov_x is None or cov_x[i]=="rand":
                     MC_data[i] = self.generate_samples_random(x[i],u_x[i])
                 elif cov_x[i]=="syst":
                     MC_data[i] = self.generate_samples_systematic(x[i],u_x[i])
+                elif param_fixed is not None:
+                    if param_fixed[i] and (len(x[i].shape) == 2):
+                        MC_data[i] = np.array([self.generate_samples_cov(
+                                        x[i][:,j].flatten(),cov_x[i]).reshape(
+                                        x[i][:,j].shape+(self.MCsteps,)) for j in
+                                            range(x[i].shape[1])]).T
+                        MC_data[i] = np.moveaxis(MC_data[i],0,1)
+
+                    else:
+                        MC_data[i] = self.generate_samples_cov(x[i].flatten(),cov_x[i]).reshape(x[i].shape+(self.MCsteps,))
                 else:
-                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),cov_x[i]).reshape(x[i].shape+(self.MCsteps,))
+                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),
+                                                           cov_x[i]).reshape(
+                        x[i].shape+(self.MCsteps,))
 
                 #print(MC_data[i].nbytes)
             if corr_between is not None:
-                print(len(MC_data),MC_data.shape)
+                #print(len(MC_data),MC_data.shape)
                 MC_data = self.correlate_samples_corr(MC_data,corr_between)
-            return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars)
+            return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars,PD_corr)
 
-    def propagate_systematic(self,func,x,u_x,cov_x=None,param_fixed=None,corr_between=None,return_corr=False,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1):
+    def propagate_systematic(self,func,x,u_x,cov_x=None,param_fixed=None,corr_between=None,return_corr=False,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1,PD_corr=True):
         """
         Propagate systematic uncertainties through measurement function with n input quantities.
         Input quantities can be floats, vectors (1d-array) or images (2d-array).
         Systematic uncertainties arise when there is full correlation between repeated measurements.
         There is a often also a correlation between measurements along the dimensions that is not one of the repeat_dims.
 
         :param func: measurement function
@@ -120,40 +132,53 @@
                                                                        output_vars)
 
         if repeat_axis >= 0:
             n_repeats=yshape[repeat_axis]
             outs = np.empty(n_repeats,dtype=object)
             for i in range(n_repeats):
                 xb,u_xb = self.select_repeated_x(x,u_x,param_fixed,i,repeat_axis,n_repeats)
+                # for ij in range(len(xb)):
+                #     print(ij,xb[ij],u_xb[ij])
                 outs[i] = self.propagate_systematic(func,xb,u_xb,cov_x,param_fixed,corr_between,
                                                 return_corr,return_samples,repeat_dims,
                                                 corr_axis=corr_axis,
-                                                output_vars=output_vars)
+                                                output_vars=output_vars,PD_corr=False)
             return self.combine_repeated_outs(outs,yshape,n_repeats,len(x),repeat_axis,
                                               return_corr,return_samples,output_vars)
 
         else:
             MC_data = np.empty(len(x),dtype=np.ndarray)
             for i in range(len(x)):
                 if u_x[i] is None:
                     u_x[i] = np.zeros_like(x[i])
-
-                if cov_x is None or cov_x[i] == "syst":
+                if cov_x[i] is None or cov_x[i] == "syst":
                     MC_data[i] = self.generate_samples_systematic(x[i],u_x[i])
                 elif cov_x[i] == "rand":
                     MC_data[i] = self.generate_samples_random(x[i],u_x[i])
+                elif param_fixed is not None:
+                    if param_fixed[i] and (len(x[i].shape) == 2):
+                        MC_data[i] = np.array([self.generate_samples_cov(
+                            x[i][:,j].flatten(),cov_x[i]).reshape
+                            (x[i][:,j].shape+(self.MCsteps,)) for j in
+                                               range(x[i].shape[1])])
+                        MC_data[i] = np.moveaxis(MC_data[i],0,1)
+                    else:
+                        MC_data[i] = self.generate_samples_cov(x[i].flatten()
+                                                               ,cov_x[i]).reshape\
+                            (x[i].shape+(self.MCsteps,))
                 else:
-                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),cov_x[i]).reshape(x[i].shape+(self.MCsteps,))
-
+                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),
+                                                           cov_x[i]).reshape(
+                        x[i].shape+(self.MCsteps,))
             if corr_between is not None:
                 MC_data = self.correlate_samples_corr(MC_data,corr_between)
 
-            return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars)
+            return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars,PD_corr)
 
-    def propagate_cov(self,func,x,cov_x,param_fixed=None,corr_between=None,return_corr=True,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1):
+    def propagate_cov(self,func,x,cov_x,param_fixed=None,corr_between=None,return_corr=True,return_samples=False,repeat_dims=-99,corr_axis=-99,output_vars=1,PD_corr=True):
         """
         Propagate uncertainties with given covariance matrix through measurement function with n input quantities.
         Input quantities can be floats, vectors (1d-array) or images (2d-array).
         The covariance matrix can represent the full covariance matrix between all measurements in all dimensions.
         Alternatively if there are repeated measurements specified in repeat_dims, the covariance matrix is given
         for the covariance along the dimension that is not one of the repeat_dims.
 
@@ -187,30 +212,43 @@
             n_repeats=yshape[repeat_axis]
             outs = np.empty(n_repeats,dtype=object)
             for i in range(n_repeats):
                 xb,_ = self.select_repeated_x(x,x,param_fixed,i,repeat_axis,n_repeats)
                 outs[i] = self.propagate_cov(func,xb,cov_x,param_fixed,corr_between,
                                                 return_corr,return_samples,repeat_dims,
                                                 corr_axis=corr_axis,
-                                                output_vars=output_vars)
+                                                output_vars=output_vars,PD_corr=False)
             return self.combine_repeated_outs(outs,yshape,n_repeats,len(x),repeat_axis,
                                               return_corr,return_samples,output_vars)
         else:
             MC_data = np.empty(len(x),dtype=np.ndarray)
             for i in range(len(x)):
                 if not hasattr(x[i],"__len__"):
                     MC_data[i] = self.generate_samples_systematic(x[i],cov_x[i])
                 elif (all((cov_x[i]==0).flatten())): #This is the case if one of the variables has no uncertainty
                     MC_data[i] = np.tile(x[i].flatten(),(self.MCsteps,1)).T
+                elif param_fixed is not None:
+                    if param_fixed[i] and (len(x[i].shape) == 2):
+                        MC_data[i] = np.array([self.generate_samples_cov(
+                            x[i][:,j].flatten(),cov_x[i]).reshape
+                            (x[i][:,j].shape+(self.MCsteps,)) for j in
+                                               range(x[i].shape[1])]).T
+                        MC_data[i] = np.moveaxis(MC_data[i],0,1)
+                    else:
+                        MC_data[i] = self.generate_samples_cov(x[i].flatten()
+                                                               ,cov_x[i]).reshape\
+                            (x[i].shape+(self.MCsteps,))
                 else:
-                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),cov_x[i]).reshape(x[i].shape+(self.MCsteps,))
+                    MC_data[i] = self.generate_samples_cov(x[i].flatten(),
+                                                           cov_x[i]).reshape(
+                        x[i].shape+(self.MCsteps,))
             if corr_between is not None:
                 MC_data = self.correlate_samples_corr(MC_data,corr_between)
 
-        return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars)
+        return self.process_samples(func,MC_data,return_corr,return_samples,corr_axis,output_vars,PD_corr)
 
     def perform_checks(self,func,x,u_x,repeat_dims,corr_axis,output_vars):
         if output_vars == 1:
             yshape = np.array(func(*x)).shape
         else:
             yshape = np.array(func(*x)[0]).shape
 
@@ -219,15 +257,15 @@
             if hasattr(x[i], "__len__"):
                 if x[i].shape != yshape and self.parallel_cores == 0:
                     shapewarning=True
             elif self.parallel_cores == 0:
                 shapewarning=True
 
         if shapewarning:
-            print(
+            warnings.warn(
                 "It looks like one of your input quantities is not an array or does not the same shape as the measurand."
                 "This is not a problem, but means you likely cannot use array operations in your measurement function."
                 "You might need to set parallel_cores to 1 or higher when creating your MCPropagation object.")
 
         for i in range(len(x)):
             if u_x[i] is None:
                 if hasattr(x[i],"__len__"):
@@ -253,45 +291,44 @@
 
         return yshape,u_x,repeat_axis,repeat_dims,corr_axis
 
     def select_repeated_x(self,x,u_x,param_fixed,i,repeat_axis,n_repeats):
         xb=np.zeros(len(x),dtype=object)
         u_xb=np.zeros(len(u_x),dtype=object)
         for j in range(len(x)):
-            if len(x[j].shape) > repeat_axis:
-                if (x[j].shape[repeat_axis]!=n_repeats):
+            selected=False
+            if param_fixed is not None:
+                if param_fixed[j] == True:
                     xb[j] = x[j]
                     u_xb[j] = u_x[j]
-                elif param_fixed is not None:
-                    if param_fixed[j]==True:
+                    selected=True
+            if not selected:
+                if len(x[j].shape) > repeat_axis:
+                    if (x[j].shape[repeat_axis]!=n_repeats):
                         xb[j] = x[j]
                         u_xb[j] = u_x[j]
-                elif repeat_axis == 0 :
-                    xb[j]=x[j][i]
-                    u_xb[j] = u_x[j][i]
-                elif repeat_axis == 1:
-                    xb[j] = x[j][:,i]
-                    u_xb[j] = u_x[j][:,i]
-                elif repeat_axis == 2:
-                    xb[j] = x[j][:,:,i]
-                    u_xb[j] = u_x[j][:,:,i]
-                else:
-                    warnings.warn("The repeat axis is too large to be dealt with by the"
-                                  "current version of punpy.")
-            else:
-                if (len(x[j])==n_repeats):
-                    xb[j] = x[j][i]
-                    u_xb[j] = u_x[j][i]
-                    if param_fixed is not None:
-                        if param_fixed[j]==True:
-                            xb[j] = x[j]
-                            u_xb[j] = u_x[j]
+                    elif repeat_axis == 0 :
+                        xb[j]=x[j][i]
+                        u_xb[j] = u_x[j][i]
+                    elif repeat_axis == 1:
+                        xb[j] = x[j][:,i]
+                        u_xb[j] = u_x[j][:,i]
+                    elif repeat_axis == 2:
+                        xb[j] = x[j][:,:,i]
+                        u_xb[j] = u_x[j][:,:,i]
+                    else:
+                        warnings.warn("The repeat axis is too large to be dealt with by the"
+                                      "current version of punpy.")
                 else:
-                    xb[j] = x[j]
-                    u_xb[j] = u_x[j]
+                    if (len(x[j])==n_repeats):
+                        xb[j] = x[j][i]
+                        u_xb[j] = u_x[j][i]
+                    else:
+                        xb[j] = x[j]
+                        u_xb[j] = u_x[j]
         return xb, u_xb
 
     def combine_repeated_outs(self,outs,yshape,n_repeats,lenx,repeat_axis,return_corr,return_samples,output_vars):
 
         if not return_corr and not return_samples:
             if output_vars == 1:
                 u_func = np.zeros(yshape)
@@ -341,28 +378,34 @@
                     for i in range(len(outs)):
                         u_func[:,:,:,i] = outs[i][0]
 
             returns = np.empty(len(outs[0]),dtype=object)
             returns[0]=u_func
             extra_index=0
             if return_corr:
-                returns[1]=np.mean([outs[i][1] for i in range(n_repeats)],axis=0)
+                corr=np.mean([outs[i][1] for i in range(n_repeats)],axis=0)
+                if not self.isPD(corr):
+                    corr=self.nearestPD_cholesky(corr,corr=True,return_cholesky=False)
+                returns[1]=corr
                 extra_index+=1
 
             if output_vars>1:
-                returns[1+extra_index]=np.mean([outs[i][1+extra_index] for i in range(n_repeats)],axis=0)
+                corr_out = np.mean([outs[i][1+extra_index] for i in range(n_repeats)],axis=0)
+                if not self.isPD(corr_out):
+                    corr_out=self.nearestPD_cholesky(corr_out,corr=True,return_cholesky=False)
+                returns[1+extra_index]=corr_out
                 extra_index+=1
 
             if return_samples:
                 returns[1+extra_index] = [np.vstack([outs[i][1+extra_index][k] for i in range(n_repeats)]) for k in range(lenx)]
                 returns[2+extra_index] = [np.vstack([outs[i][2+extra_index][k] for i in range(n_repeats)]) for k in range(lenx)]
 
             return returns
 
-    def process_samples(self,func,data,return_corr,return_samples,corr_axis=-99,output_vars=1):
+    def process_samples(self,func,data,return_corr,return_samples,corr_axis=-99,output_vars=1,PD_corr=True):
         """
         Run the MC-generated samples of input quantities through the measurement function and calculate
         correlation matrix if required.
 
         :param func: measurement function
         :type func: function
         :param data: MC-generated samples of input quantities
@@ -394,35 +437,47 @@
             # We again need to reorder the input quantities samples in order to be able to pass them to p.starmap
             # We here use lists to iterate over and order them slightly different as the case above.
             data2=[[data[j][...,i] for j in range(len(data))] for i in range(self.MCsteps)]
             MC_y2=np.array(self.pool.starmap(func,data2))
             MC_y = np.moveaxis(MC_y2,0,-1)
 
         u_func = np.std(MC_y,axis=-1)
+
         if not return_corr:
             if return_samples:
                 return u_func,MC_y,data
             else:
                 return u_func
         else:
             if output_vars==1:
-                corr_y = self.calculate_corr(MC_y,corr_axis)
+                corr_y = self.calculate_corr(MC_y,corr_axis).astype("float32")
+                if PD_corr:
+                    if not self.isPD(corr_y):
+                        corr_y = self.nearestPD_cholesky(corr_y,corr=True,
+                                                       return_cholesky=False)
                 if return_samples:
                     return u_func,corr_y,MC_y,data
                 else:
                     return u_func,corr_y
 
             else:
                 #create an empty arrays and then populate it with the correlation matrix for each output parameter individually
                 corr_ys=np.empty(output_vars,dtype=object)
                 for i in range(output_vars):
-                    corr_ys[i] = self.calculate_corr(MC_y[i],corr_axis)
-
+                    corr_ys[i] = self.calculate_corr(MC_y[i],corr_axis).astype("float32")
+                    if PD_corr:
+                        if not self.isPD(corr_ys[i]):
+                            corr_ys[i] = self.nearestPD_cholesky(corr_ys[i],corr=True,
+                                                             return_cholesky=False)
                 #calculate correlation matrix between the different outputs produced by the measurement function.
-                corr_out=np.corrcoef(MC_y.reshape((output_vars,-1)))
+                corr_out=np.corrcoef(MC_y.reshape((output_vars,-1))).astype("float32")
+                if PD_corr:
+                    if not self.isPD(corr_out):
+                        corr_out = self.nearestPD_cholesky(corr_out,corr=True,
+                                                         return_cholesky=False)
 
                 if return_samples:
                     return u_func,corr_ys,corr_out,MC_y,data
                 else:
                     return u_func,corr_ys,corr_out
 
     def calculate_corr(self,MC_y,corr_axis=-99):
@@ -588,15 +643,15 @@
             else:
                 samples_out=samples[:]
                 id_nonzero=np.where(stds!=0)
                 samples_out[id_nonzero]=np.dot(L[id_nonzero][:,id_nonzero],(samples[id_nonzero]-means[id_nonzero])/stds[id_nonzero])[:,0]*stds[id_nonzero]+means[id_nonzero]
                 return samples_out
 
     @staticmethod
-    def nearestPD_cholesky(A):
+    def nearestPD_cholesky(A,diff=0.001,corr=False,return_cholesky=True):
         """
         Find the nearest positive-definite matrix
 
         :param A: correlation matrix or covariance matrix
         :type A: array
         :return: nearest positive-definite matrix
         :rtype: array
@@ -628,22 +683,46 @@
             I = np.eye(A.shape[0])
             k = 1
             while not MCPropagation.isPD(A3):
                 mineig = np.min(np.real(np.linalg.eigvals(A3)))
                 A3 += I*(-mineig*k**2+spacing)
                 k += 1
 
-            if np.any(abs(A-A3)/(A+0.0001) > 0.0001):
-                raise ValueError(
-                    "One of the provided covariance matrix is not postive definite. Covariance matrices need to be at least positive semi-definite. Please check your covariance matrix.")
-            else:
-                warnings.warn(
-                    "One of the provided covariance matrix is not positive definite. It has been slightly changed (less than 0.01% in any element) to accomodate our method.")
-                return np.linalg.cholesky(A3)
+            maxdiff=np.max(np.abs(A-A3))
 
+            if corr == True:
+                if maxdiff>diff:
+                    raise ValueError(
+                        "One of the correlation matrices is not postive definite. "
+                        "Correlation matrices need to be at least positive "
+                        "semi-definite.")
+                else:
+                    print(
+                        "One of the provided covariance matrix is not positive "
+                        "definite. It has been slightly changed (less than %s in any "
+                        "element) to accomodate our method."%(diff))
+                    if return_cholesky:
+                        return np.linalg.cholesky(A3)
+                    else:
+                        return A3
+            else:
+                if maxdiff > diff:
+                    raise ValueError(
+                        "One of the provided covariance matrices is not postive "
+                        "definite. Covariance matrices need to be at least positive "
+                        "semi-definite. Please check your covariance matrix.")
+                else:
+                    print(
+                        "One of the provided covariance matrix is not positive "
+                        "definite. It has been slightly changed (less than %s \% in "
+                        "any element) to accomodate our method."%(diff/100))
+                    if return_cholesky:
+                        return np.linalg.cholesky(A3)
+                    else:
+                        return A3
     @staticmethod
     def isPD(B):
         """
         Returns true when input is positive-definite, via Cholesky
 
         :param B: matrix
         :type B: array
```

### Comparing `punpy-0.8.2/punpy/mc/tests/test_mc_propagation.py` & `punpy-0.9.0/punpy/mc/tests/test_mc_propagation.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy/utilities/utilities.py` & `punpy-0.9.0/punpy/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/punpy.egg-info/PKG-INFO` & `punpy-0.9.0/punpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punpy
-Version: 0.8.2
+Version: 0.9.0
 Summary: Propagating UNcertainties in PYthon
 Home-page: https://gitlab.npl.co.uk/eco/eo/punpy
 Author: Pieter De Vis
 Author-email: pieter.de.vis@npl.co.uk
 License: None
 Description: punpy
         =====
```

### Comparing `punpy-0.8.2/punpy.egg-info/SOURCES.txt` & `punpy-0.9.0/punpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `punpy-0.8.2/setup.py` & `punpy-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     #version=versioneer.get_version(),
     #cmdclass=versioneer.get_cmdclass(),
-    version='0.8.2',
+    version='0.9.0',
     name="punpy",
     url="https://gitlab.npl.co.uk/eco/eo/punpy",
     license="None",
     author="Pieter De Vis",
     author_email="pieter.de.vis@npl.co.uk",
     description="Propagating UNcertainties in PYthon",
     long_description=read("README.rst"),
```

### Comparing `punpy-0.8.2/versioneer.py` & `punpy-0.9.0/versioneer.py`

 * *Files identical despite different names*

