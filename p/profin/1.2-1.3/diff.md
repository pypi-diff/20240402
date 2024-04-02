# Comparing `tmp/profin-1.2.tar.gz` & `tmp/profin-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profin-1.2.tar", last modified: Fri Mar 22 15:36:35 2024, max compression
+gzip compressed data, was "profin-1.3.tar", last modified: Tue Apr  2 09:23:14 2024, max compression
```

## Comparing `profin-1.2.tar` & `profin-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 15:36:35.089067 profin-1.2/
--rw-rw-rw-   0        0        0     1198 2024-02-27 08:45:46.000000 profin-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2024-02-27 08:50:55.000000 profin-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      211 2024-03-22 15:36:35.089067 profin-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-02-27 08:36:07.000000 profin-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 15:36:35.072169 profin-1.2/profin/
--rw-rw-rw-   0        0        0      183 2023-10-14 08:10:36.000000 profin-1.2/profin/__init__.py
--rw-rw-rw-   0        0        0    11687 2024-03-22 14:18:35.000000 profin-1.2/profin/indicators.py
--rw-rw-rw-   0        0        0    13476 2024-03-22 13:41:38.000000 profin-1.2/profin/project.py
--rw-rw-rw-   0        0        0     6395 2024-03-22 12:21:09.000000 profin-1.2/profin/risks.py
-drwxrwxrwx   0        0        0        0 2024-03-22 15:36:35.072169 profin-1.2/profin.egg-info/
--rw-rw-rw-   0        0        0      211 2024-03-22 15:36:34.000000 profin-1.2/profin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-03-22 15:36:34.000000 profin-1.2/profin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 15:36:34.000000 profin-1.2/profin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-27 09:01:14.000000 profin-1.2/profin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-03-22 15:36:34.000000 profin-1.2/profin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 15:36:35.089067 profin-1.2/setup.cfg
--rw-rw-rw-   0        0        0      421 2024-03-22 15:34:51.000000 profin-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:14.783059 profin-1.3/
+-rw-rw-rw-   0        0        0     1198 2024-02-27 08:45:46.000000 profin-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2024-02-27 08:50:55.000000 profin-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      211 2024-04-02 09:23:14.783059 profin-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-02-27 08:36:07.000000 profin-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:14.768528 profin-1.3/profin/
+-rw-rw-rw-   0        0        0      183 2023-10-14 08:10:36.000000 profin-1.3/profin/__init__.py
+-rw-rw-rw-   0        0        0    16180 2024-03-28 14:18:08.000000 profin-1.3/profin/indicators.py
+-rw-rw-rw-   0        0        0    13476 2024-03-22 13:41:38.000000 profin-1.3/profin/project.py
+-rw-rw-rw-   0        0        0     9002 2024-03-27 15:15:21.000000 profin-1.3/profin/risks.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:14.783059 profin-1.3/profin.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-04-02 09:23:14.000000 profin-1.3/profin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-02 09:23:14.000000 profin-1.3/profin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:23:14.000000 profin-1.3/profin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-27 09:01:14.000000 profin-1.3/profin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-04-02 09:23:14.000000 profin-1.3/profin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:23:14.783059 profin-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      421 2024-04-02 09:22:37.000000 profin-1.3/setup.py
```

### Comparing `profin-1.2/LICENSE.txt` & `profin-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `profin-1.2/profin/indicators.py` & `profin-1.3/profin/indicators.py`

 * *Files 21% similar despite different names*

```diff
@@ -117,26 +117,28 @@
 
         """
         EFFICIENCY = self.ATTR["E_out"] / self.ATTR["E_in"]
         
         return EFFICIENCY
 
 
-    def get_NPV(self, WACC):
+    def get_NPV(self, WACC, **kwargs):
         """
         This methods calculates the net present value of the energy project in US$,
         considering future developments of interest rates and country-specific
         developments.
 
         Returns
         -------
         NPV : int
 
         """
         
+        period_to_analyze = kwargs.get("PERIOD", self.ATTR["LIFETIME"])
+        
         #Calculate the matrix for all timesteps and random distributions.
         OPERATING_CASHFLOW = (
             self.ATTR["K_E_out"]*self.ATTR["E_out"] -
             self.ATTR["OPEX"] - 
             self.ATTR["K_E_in"]*self.ATTR["E_in"]
             ) * (1-self.ATTR["CORPORATE_TAX_RATE"])
          
@@ -151,15 +153,15 @@
             SUBSIDY + 
             TERMINAL_VALUE -
             K_INVEST
             )
         
         #Discounting of annual cashflows and investments
         NPV = 0
-        for t in range(self.ATTR["LIFETIME"]):
+        for t in range(period_to_analyze):
             NPV += RELEVANT_CASHFLOWS[t] / (1+WACC)**t
         
         return NPV
 
 
     def get_IRR(self):
         """
@@ -171,14 +173,15 @@
 
         """
         
         x_init = np.full(self.RANDOM_DRAWS, 0.05)
         IRR = so.fsolve(self.get_NPV, x_init)
         
         if IRR.mean() > 0.5:
+            print("IRR Mean: ", IRR.mean())
             raise Warning("Internal rate of return >50%. Please check your assumptions.")
         
         return IRR        
 
 
     def get_LCOE(self, WACC):
         """
@@ -297,8 +300,147 @@
         for t in range(self.ATTR["LIFETIME"]):
             NON_OPERATING_CASHFLOW_DISCOUNTED[t] = NON_OPERATING_CASHFLOW[t] / (1+WACC.mean())**t
             NON_OPERATING_CASHFLOW_STD_DISCOUNTED[t] = NON_OPERATING_CASHFLOW_STD[t] / (1+WACC.mean())**t        
         
         if DISCOUNT:
             return OPERATING_CASHFLOW_DISCOUNTED, OPERATING_CASHFLOW_STD_DISCOUNTED, NON_OPERATING_CASHFLOW_DISCOUNTED, NON_OPERATING_CASHFLOW_STD_DISCOUNTED
         else:
-            return OPERATING_CASHFLOW, OPERATING_CASHFLOW_STD, NON_OPERATING_CASHFLOW, NON_OPERATING_CASHFLOW_STD
+            return OPERATING_CASHFLOW, OPERATING_CASHFLOW_STD, NON_OPERATING_CASHFLOW, NON_OPERATING_CASHFLOW_STD
+        
+        
+    def get_NPV_Subsidy_Annually_Constant(self, ANNUAL_SUBSIDY, npv_target, WACC, PERIOD):
+        """
+        This methods calculates the net present value of the energy project in US$,
+        considering future developments of interest rates and country-specific
+        developments.
+
+        Returns
+        -------
+        NPV : int
+
+        """
+        
+        period_to_analyze = PERIOD
+        
+        #Calculate the matrix for all timesteps and random distributions.
+        OPERATING_CASHFLOW = (
+            self.ATTR["K_E_out"]*self.ATTR["E_out"] -
+            self.ATTR["OPEX"] - 
+            self.ATTR["K_E_in"]*self.ATTR["E_in"]
+            ) * (1-self.ATTR["CORPORATE_TAX_RATE"])
+         
+        TERMINAL_VALUE = self.ATTR["TERMINAL_VALUE"].copy()
+
+        K_INVEST = self.ATTR["K_INVEST"].copy()
+                
+        RELEVANT_CASHFLOWS = (
+            OPERATING_CASHFLOW + 
+            ANNUAL_SUBSIDY + 
+            TERMINAL_VALUE -
+            K_INVEST
+            )
+        
+        #Discounting of annual cashflows and investments
+        NPV = -npv_target
+        for t in range(period_to_analyze):
+            NPV += RELEVANT_CASHFLOWS[t] / (1+WACC)**t
+        
+        return NPV
+    
+    
+    def get_NPV_Subsidy_Fixed_Premium(self, FIXED_PREMIUM, npv_target, WACC, PERIOD):
+        """
+        This methods calculates the net present value of the energy project in US$,
+        considering future developments of interest rates and country-specific
+        developments.
+
+        Returns
+        -------
+        NPV : int
+
+        """
+        
+        period_to_analyze = PERIOD
+        
+        #Calculate the matrix for all timesteps and random distributions.
+        OPERATING_CASHFLOW = (
+            (self.ATTR["K_E_out"]+FIXED_PREMIUM)*self.ATTR["E_out"] -
+            self.ATTR["OPEX"] - 
+            self.ATTR["K_E_in"]*self.ATTR["E_in"]
+            ) * (1-self.ATTR["CORPORATE_TAX_RATE"])
+         
+        TERMINAL_VALUE = self.ATTR["TERMINAL_VALUE"].copy()
+
+        K_INVEST = self.ATTR["K_INVEST"].copy()
+                
+        RELEVANT_CASHFLOWS = (
+            OPERATING_CASHFLOW + 
+            TERMINAL_VALUE -
+            K_INVEST
+            )
+        
+        #Discounting of annual cashflows and investments
+        NPV = -npv_target
+        for t in range(period_to_analyze):
+            NPV += RELEVANT_CASHFLOWS[t] / (1+WACC)**t
+        
+        return NPV
+
+    
+    
+    def get_subsidy(self, npv_target, depreciation_target, subsidy_scheme, WACC):
+        """
+        This method returns the required subsidy to reach the defined
+        net present value target after a given depreciation period and
+        for a given subsidy scheme. 
+        Available subsidy schemes: 1) Initial subsidy (e.g. CAPEX), 
+        2) annually constant subsidy (e.g. H2Global), 3) CFD, 4) Fixed Premium
+
+        Parameters
+        ----------
+        npv_target : TYPE
+            DESCRIPTION.
+        depreciation_target : TYPE
+            DESCRIPTION.
+        subsidy_scheme : TYPE
+            DESCRIPTION.
+        WACC : TYPE
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        if subsidy_scheme == "INITIAL":
+            npv_temp = self.get_NPV(WACC, PERIOD=depreciation_target)
+            subsidy = npv_target - npv_temp
+            
+        elif subsidy_scheme == "ANNUALLY_CONSTANT":
+            x_init = np.full(self.RANDOM_DRAWS, 1e+6)
+            subsidy = so.fsolve(self.get_NPV_Subsidy_Annually_Constant, x_init, args=(npv_target,WACC,depreciation_target))
+
+        elif subsidy_scheme == "FIXED_PREMIUM":
+            x_init = np.full(self.RANDOM_DRAWS, 0.1)
+            subsidy = so.fsolve(self.get_NPV_Subsidy_Fixed_Premium, x_init, args=(npv_target,WACC,depreciation_target))
+
+        elif subsidy_scheme == "CFD":
+            OPERATING_CASHFLOW, OPERATING_CASHFLOW_STD, NON_OPERATING_CASHFLOW, NON_OPERATING_CASHFLOW_STD = self.get_cashflows(WACC)
+            subsidy = -(OPERATING_CASHFLOW + NON_OPERATING_CASHFLOW)
+        
+        else:
+            raise AttributeError("No such subsidy scheme defined.") 
+
+        return subsidy
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+
```

### Comparing `profin-1.2/profin/project.py` & `profin-1.3/profin/project.py`

 * *Files identical despite different names*

### Comparing `profin-1.2/profin/risks.py` & `profin-1.3/profin/risks.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,40 +57,58 @@
         NO_RISKS = len(self.RISK_PARAM)
                 
         if NO_RISKS == 1:
             SINGLE_RISK = list(self.RISK_PARAM)[0]
             #get distribution type
             distribution_temp = self.RISK_PARAM[SINGLE_RISK]["distribution"] 
             #get scale parameter (e.g. standard deviation)
-            if isinstance(self.RISK_PARAM[SINGLE_RISK]["scale"] , np.ndarray):
+            if isinstance(self.RISK_PARAM[SINGLE_RISK]["scale"] , np.ndarray) or isinstance(self.RISK_PARAM[SINGLE_RISK]["scale"] , list):
                 scale_temp = self.RISK_PARAM[SINGLE_RISK]["scale"][timestep]
             else:
                 #scale parameter is an int or float
                 scale_temp = self.RISK_PARAM[SINGLE_RISK]["scale"]
+                
+            if "limit" in list(self.RISK_PARAM[SINGLE_RISK]):
+                if isinstance(self.RISK_PARAM[SINGLE_RISK]["limit"]["max"] , np.ndarray) or isinstance(self.RISK_PARAM[SINGLE_RISK]["limit"]["max"] , list):
+                    max_trunc = self.RISK_PARAM[SINGLE_RISK]["limit"]["max"][timestep]
+                    min_trunc = self.RISK_PARAM[SINGLE_RISK]["limit"]["min"][timestep]
+                else:
+                    #scale parameter is an int or float
+                    max_trunc = self.RISK_PARAM[SINGLE_RISK]["limit"]["max"]
+                    min_trunc = self.RISK_PARAM[SINGLE_RISK]["limit"]["min"]
+                    
             #get mean
             mean_temp = self.ATTR[SINGLE_RISK][timestep].mean()
             
             if scale_temp == 0:
                 alpha = np.full(self.RANDOM_DRAWS, mean_temp)
             else:
                 if distribution_temp == "normal":
-                    #normal distribution
-                    normal_dist = stats.norm(
-                        loc=mean_temp, scale=scale_temp
-                        )
-                    alpha = normal_dist.rvs(size=self.RANDOM_DRAWS)
+                    if "limit" in list(self.RISK_PARAM[SINGLE_RISK]):
+                        max_scale = (max_trunc - mean_temp) / scale_temp
+                        min_scale = (min_trunc - mean_temp) / scale_temp
+                        
+                        #truncated normal distribution
+                        normal_dist = stats.truncnorm(
+                            a=min_scale, b=max_scale, loc=mean_temp, scale=scale_temp
+                            )
+                        alpha = normal_dist.rvs(size=self.RANDOM_DRAWS)
+                    else:
+                        #normal distribution
+                        normal_dist = stats.norm(loc=mean_temp, scale=scale_temp)
+                        alpha = normal_dist.rvs(size=self.RANDOM_DRAWS)
                 elif distribution_temp == "positive-normal":
                     #truncated normal distribution, all values above mean
-                    normal_dist = stats.norm(
+                    normal_dist = stats.truncnorm(
                         a=0, b=np.inf, loc=mean_temp, scale=scale_temp
                         )
                     alpha = normal_dist.rvs(size=self.RANDOM_DRAWS)
                 elif distribution_temp == "negative-normal":
                     #truncated normal distribution, all values below mean
-                    normal_dist = stats.norm(
+                    normal_dist = stats.truncnorm(
                         a=-np.inf, b=0, loc=mean_temp, scale=scale_temp
                         )
                     alpha = normal_dist.rvs(size=self.RANDOM_DRAWS)
                 else:
                     raise AttributeError("Unknown distribution.")
                 
             RISKS = {}
@@ -113,35 +131,55 @@
             for u in range(NO_RISKS):
                 UNIFORMS[u] = stats.norm.cdf(MARGINALS[u])
                 
             #DEFINE MARGINAL DISTRIBUTIONS
             ALPHA_ARRAY = {}
             for r, risk in enumerate(self.RISK_PARAM):
                 #get scale 
-                if isinstance(self.RISK_PARAM[risk]["scale"] , np.ndarray):
+                if isinstance(self.RISK_PARAM[risk]["scale"] , np.ndarray) or isinstance(self.RISK_PARAM[risk]["scale"] , list):
                     scale_temp = self.RISK_PARAM[risk]["scale"][timestep]
                 else:
                     #scale parameter is an int or float
                     scale_temp = self.RISK_PARAM[risk]["scale"]
                 #get loc/mean
-                loc_temp = self.ATTR[risk][timestep].mean()
+                mean_temp = self.ATTR[risk][timestep].mean()
+
+                #get limits for truncated distribution
+                if "limit" in list(self.RISK_PARAM[risk]):
+                    if isinstance(self.RISK_PARAM[risk]["limit"]["max"], np.ndarray) or isinstance(self.RISK_PARAM[risk]["limit"]["max"], list):
+                        max_trunc = self.RISK_PARAM[risk]["limit"]["max"][timestep]
+                        min_trunc = self.RISK_PARAM[risk]["limit"]["min"][timestep]
+                    else:
+
+                        #scale parameter is an int or float
+                        max_trunc = self.RISK_PARAM[risk]["limit"]["max"]
+                        min_trunc = self.RISK_PARAM[risk]["limit"]["min"]
 
                 if scale_temp == 0:
-                    ALPHA_ARRAY[r] = np.full(self.RANDOM_DRAWS, loc_temp)
+                    ALPHA_ARRAY[r] = np.full(self.RANDOM_DRAWS, mean_temp)
                 else:
                     if self.RISK_PARAM[risk]["distribution"] == "normal":
-                        DIST = stats.norm(loc=loc_temp, scale=scale_temp)
-                        ALPHA_ARRAY[r] = DIST.ppf(UNIFORMS[r])
+                        if "limit" in list(self.RISK_PARAM[risk]):
+                            max_scale = (max_trunc - mean_temp) / scale_temp
+                            min_scale = (min_trunc - mean_temp) / scale_temp                           
+                            #truncated normal distribution
+                            DIST = stats.truncnorm(
+                                a=min_scale, b=max_scale, loc=mean_temp, scale=scale_temp
+                                )
+                            ALPHA_ARRAY[r] = DIST.ppf(UNIFORMS[r])
+                        else:
+                            DIST = stats.norm(loc=mean_temp, scale=scale_temp)
+                            ALPHA_ARRAY[r] = DIST.ppf(UNIFORMS[r])
                     elif self.RISK_PARAM[risk]["distribution"] == "positive-normal":
                         #truncated normal distribution, with all values above the mean.
-                        DIST = stats.truncnorm(a=0, b=np.inf, loc=loc_temp, scale=scale_temp)
+                        DIST = stats.truncnorm(a=0, b=np.inf, loc=mean_temp, scale=scale_temp)
                         ALPHA_ARRAY[r] = DIST.ppf(UNIFORMS[r])
                     elif self.RISK_PARAM[risk]["distribution"] == "negative-normal":
                         #truncated normal distribution, with all values below the mean.
-                        DIST = stats.truncnorm(a=-np.inf, b=0, loc=loc_temp, scale=scale_temp)
+                        DIST = stats.truncnorm(a=-np.inf, b=0, loc=mean_temp, scale=scale_temp)
                         ALPHA_ARRAY[r] = DIST.ppf(UNIFORMS[r])
                     else:
                         raise AttributeError("Unknown distribution.")
                                               
             RISKS = {}
             for r, risk in enumerate(self.RISK_PARAM):
                 RISKS[risk] = ALPHA_ARRAY[r]
```

