# Comparing `tmp/ewatercycle_da-0.0.2.tar.gz` & `tmp/ewatercycle_da-0.0.3.tar.gz`

## Comparing `ewatercycle_da-0.0.2.tar` & `ewatercycle_da-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/Makefile
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/conf.py
--rw-r--r--   0        0        0  1891278 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/example_HBV_model_EnKF.ipynb
--rw-r--r--   0        0        0  1006765 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/example_HBV_model_PF_1.ipynb
--rw-r--r--   0        0        0   886757 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/example_HBV_model_PF_2.ipynb
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/make.bat
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/requirements.txt
--rw-r--r--   0        0        0   754797 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/Forcing/01620500_lump_cida_forcing_leap.txt
--rw-r--r--   0        0        0   211468 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/Observations/01620500_streamflow_qc.nc
--rw-r--r--   0        0        0   399700 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/Observations/01620500_streamflow_qc.txt
--rw-r--r--   0        0        0   376480 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/_images/method1_define_upfront.png
--rw-r--r--   0        0        0   376634 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/_images/method2_define_on_the_go.png
--rw-r--r--   0        0        0   603584 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/_images/method3_no_DA.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/autoapi/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/docs/autoapi/init/index.rst
--rw-r--r--   0        0        0    38621 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/src/ewatercycle_DA/DA.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/src/ewatercycle_DA/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/.gitignore
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/README.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0  1891278 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/example_HBV_model_EnKF.ipynb
+-rw-r--r--   0        0        0  1006765 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/example_HBV_model_PF_1.ipynb
+-rw-r--r--   0        0        0   886757 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/example_HBV_model_PF_2.ipynb
+-rw-r--r--   0        0        0    61678 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/example_Marrmot_Ensemble.ipynb
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0   754797 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Forcing/01620500_lump_cida_forcing_leap.txt
+-rw-r--r--   0        0        0    19400 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Forcing/BMI_testcase_m01_BuffaloRiver_TN_USA.mat
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Forcing/BMI_testcase_m01_BuffaloRiver_TN_USA.matZone.Identifier
+-rw-r--r--   0        0        0   211468 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Observations/01620500_streamflow_qc.nc
+-rw-r--r--   0        0        0   399700 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/Observations/01620500_streamflow_qc.txt
+-rw-r--r--   0        0        0   376480 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/_images/method1_define_upfront.png
+-rw-r--r--   0        0        0   376634 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/_images/method2_define_on_the_go.png
+-rw-r--r--   0        0        0   603584 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/_images/method3_no_DA.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/autoapi/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/docs/autoapi/init/index.rst
+-rw-r--r--   0        0        0    39501 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/src/ewatercycle_DA/DA.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/src/ewatercycle_DA/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/.gitignore
+-rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/README.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 ewatercycle_da-0.0.3/PKG-INFO
```

### Comparing `ewatercycle_da-0.0.2/.readthedocs.yaml` & `ewatercycle_da-0.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/.github/workflows/python-publish.yml` & `ewatercycle_da-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/Makefile` & `ewatercycle_da-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/conf.py` & `ewatercycle_da-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/example_HBV_model_EnKF.ipynb` & `ewatercycle_da-0.0.3/docs/example_HBV_model_EnKF.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/example_HBV_model_PF_1.ipynb` & `ewatercycle_da-0.0.3/docs/example_HBV_model_PF_1.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/example_HBV_model_PF_2.ipynb` & `ewatercycle_da-0.0.3/docs/example_HBV_model_PF_2.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/index.rst` & `ewatercycle_da-0.0.3/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
              
    example_HBV_model_PF_1
    example_HBV_model_PF_2
    example_HBV_model_EnKF
+   example_Marrmot_Ensemble
```

### Comparing `ewatercycle_da-0.0.2/docs/make.bat` & `ewatercycle_da-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/Forcing/01620500_lump_cida_forcing_leap.txt` & `ewatercycle_da-0.0.3/docs/Forcing/01620500_lump_cida_forcing_leap.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/Observations/01620500_streamflow_qc.nc` & `ewatercycle_da-0.0.3/docs/Observations/01620500_streamflow_qc.nc`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/Observations/01620500_streamflow_qc.txt` & `ewatercycle_da-0.0.3/docs/Observations/01620500_streamflow_qc.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/_images/method1_define_upfront.png` & `ewatercycle_da-0.0.3/docs/_images/method1_define_upfront.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/_images/method2_define_on_the_go.png` & `ewatercycle_da-0.0.3/docs/_images/method2_define_on_the_go.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/docs/_images/method3_no_DA.png` & `ewatercycle_da-0.0.3/docs/_images/method3_no_DA.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/src/ewatercycle_DA/DA.py` & `ewatercycle_da-0.0.3/src/ewatercycle_DA/DA.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,31 @@
 
 import types
 from typing import Any, Optional
 from pathlib import Path
 from pydantic import BaseModel
 
 import ewatercycle
+import ewatercycle.models
+import ewatercycle.forcing
 from ewatercycle.base.forcing import DefaultForcing
-from ewatercycle.models import HBV, Lorenz
 
-LOADED_MODELS: dict[str, Any] = dict(
-                                        HBV=ewatercycle.models.HBV,
-                                        Lorenz = ewatercycle.models.Lorenz,
-                                        ParallelisationSleep = ewatercycle.models.ParallelisationSleep,
-                                     )
-LOADED_HYDROLOGY_MODELS: dict[str, Any] = dict(
-                                        HBV=ewatercycle.models.HBV)
+# saves users from encountering errors - change this to config file later?
+KNOWN_WORKING_MODELS_DA: list[str] = ["HBV", "Lorenz", "ParallelisationSleep"]
+KNOWN_WORKING_MODELS_DA_HYDROLOGY: list[str] = ["HBV"]
 TLAG_MAX = 100 # sets maximum lag possible (d)
 
+
+def load_models(loaded_models) -> dict[str, Any]:
+    """Loads models found in user install"""
+    for model in ewatercycle.models.sources:
+        loaded_models.update({model: ewatercycle.models.sources[model]})
+    
+    return loaded_models
+
 class Ensemble(BaseModel):
     """Class for running data assimilation in eWaterCycle
 
     Args:
         N : Number of ensemble members
 
         location : Where the model is run, by default local - change to remote later
@@ -58,14 +63,18 @@
         measurement_operator: Function or list of Functions which maps the state vector to the measurement space:
             i.e. extracts the wanted value for comparison by the DA scheme from the state vector.   (Also known as H)
 
         observations: NetCDF file containing observations
 
         lst_models_name: list containing a set of all the model names: i.e. to run checks
 
+        logger: list to debug issues, this isn't the best way to debug/log but works for me
+
+        config_specific_storage: used by the config_specific_actions
+
 
     Note:
         Run ``setup`` and ``initialize`` before using other functions
 
     """
 
     N: int
@@ -77,14 +86,18 @@
     ensemble_method: Any | None = None
     ensemble_method_name: str | None = None
     observed_variable_name: str | None = None
     measurement_operator: Any | list | None = None
     observations: Any | None = None
     lst_models_name: list = []
     logger: list = [] # logging proved too complex for now so just append to list XD
+    config_specific_storage: Any | None = None
+
+    loaded_models: dict[str, Any] = dict()
+    loaded_models = load_models(loaded_models)
 
     def setup(self) -> None:
         """Creates a set of empty Ensemble member instances
         This allows further customisation: i.e. different models in one ensemble
         """
         if len(self.ensemble_list) != 0:
             self.ensemble_list = []
@@ -111,22 +124,24 @@
 
         # same for all members (to start with)
         if type(model_name) == str:
             for ensemble_member in self.ensemble_list:
                 ensemble_member.model_name = model_name
                 ensemble_member.forcing = forcing
                 ensemble_member.setup_kwargs = setup_kwargs
+                ensemble_member.loaded_models = self.loaded_models
 
         # more flexibility - could change in the future?
         elif type(model_name) == list and len(model_name) == self.N:
             validity_initialize_input(model_name, forcing, setup_kwargs)
             for index_m, ensemble_member in enumerate(self.ensemble_list):
                 ensemble_member.model_name = model_name[index_m]
                 ensemble_member.forcing = forcing[index_m]
                 ensemble_member.setup_kwargs = setup_kwargs[index_m]
+                ensemble_member.loaded_models = self.loaded_models
         else:
             raise SyntaxWarning(f"model should either string or list of string of length {self.N}")
 
         # setup & initialize - same in both cases - in parallel
         gathered_initialize = self.gather(*[self.initialize_parallel(self, i) for i in range(self.N)])
 
         with dask.config.set(self.dask_config):
@@ -192,14 +207,15 @@
 
             measurement_operator (:obj:`function`| :obj:`list[functions]`) = None: if not specified: by default 'all' known parameters,
                 can be a subset of all by passing a list containing strings of variable to include in the state vector.
                 Should you want to vary initial parameters, again all should be a list
 
         Note:
             Assumed memory is large enough to hold observations in memory/lazy open with xarray
+            Assumed memory is large enough to hold observations in memory/lazy open with xarray
         """
         validate_method(ensemble_method_name)
 
         self.ensemble_method = LOADED_METHODS[ensemble_method_name](N=self.N)
         self.ensemble_method_name = ensemble_method_name
 
         for hyper_param in hyper_parameters:
@@ -239,15 +255,15 @@
     # TODO: think if this is a good idea
     @staticmethod
     @delayed
     def finalize_parallel(ensemble, i):
         ensemble_member = ensemble.ensemble_list[i]
         ensemble_member.finalize()
 
-    def update(self, assimilate=True) -> None:
+    def update(self, assimilate=False) -> None:
         """Updates model for all members.
         Args:
             assimilate (bool): Whether to assimilate in a given timestep. True by default.
         Algorithm flow:
             Gets the state vector, modeled outcome and corresponding observation
 
             Computes new state vector using supplied method
@@ -265,24 +281,27 @@
 
         gathered_update = (self.gather(*[self.update_parallel(self, i) for i in range(self.N)]))
 
         with dask.config.set(self.dask_config):
             gathered_update.compute()
 
         if assimilate:
+            if not all(model_name in KNOWN_WORKING_MODELS_DA for model_name in self.lst_models_name):
+                raise RuntimeWarning(f'Not all models specified {self.lst_models_name} are known to work with' \
+                                    +'Data Assimilation. Either specify model that does work or submit a PR to add it.')
             # get observations
             current_time = np.datetime64(self.ensemble_list[0].model.time_as_datetime)
             current_obs = self.observations.sel(time=current_time, method="nearest").values
 
 
             self.assimilate(ensemble_method_name=self.ensemble_method_name,
                             obs=current_obs,
                             measurement_operator = self.measurement_operator,
                             hyper_parameters = self.ensemble_method.hyperparameters,
-                            state_vector_variables = None, # maybe fix later? - currently don't have acces
+                            state_vector_variables = None, # maybe fix later? - currently don't have access
                             )
 
 
     @staticmethod
     @delayed
     def update_parallel(ensemble, i):
         ensemble_member = ensemble.ensemble_list[i]
@@ -292,15 +311,15 @@
                    ensemble_method_name: str,
                    obs: np.ndarray,
                    measurement_operator,
                    hyper_parameters: dict,
                    state_vector_variables: str | list | None,
                    ):
 
-        """" Similar to calling .. py:function:: Ensemble.update(assimilate=True)
+        """ Similar to calling .. py:function:: Ensemble.update(assimilate=True)
         Intended for advanced users!
         The assimilate class aims to make on the fly data assimilation possible.
         You only need to define which method, observations and H operator you wish to use.
         This however requires more know-how of the situation,
 
         Args:
             ensemble_method_name (str): name of the data assimilation method for the ensemble
@@ -338,17 +357,19 @@
 
         self.ensemble_method.obs = obs
 
         self.ensemble_method.update()
 
         self.remove_negative()
 
+        self.config_specific_actions(pre_set_state=True)
+
         self.set_state_vector(self.ensemble_method.new_state_vectors)
 
-        self.config_specific_actions()
+        self.config_specific_actions(pre_set_state=False)
 
 
     def get_predicted_values(self, measurement_operator) -> np.ndarray:
         """"Loops over the state vectors and applies specified measurement operator to obtain predicted value"""
         predicted_values = []
         if type(measurement_operator) == list:
             # if a list is passed, it's a list of operators per ensemble member
@@ -363,21 +384,23 @@
             raise RuntimeError(f"Invalid type {measurement_operator}, should be either list of function but is ")
 
         return np.vstack(predicted_values)
 
     def remove_negative(self):
         """if only one model is loaded & hydrological: sets negative numbers to positive
            Other models such as the lorenz model can be negative"""
-        if len(self.lst_models_name) == 1 and self.lst_models_name[0] in LOADED_HYDROLOGY_MODELS:
+        # in future may be interesting to load multiple types of hydrological models in one ensemble
+        # for not not implemented
+        if len(self.lst_models_name) == 1 and self.lst_models_name[0] in KNOWN_WORKING_MODELS_DA_HYDROLOGY:
                 # set any values below 0 to small
                 self.ensemble_method.new_state_vectors[self.ensemble_method.new_state_vectors < 0] = 1e-6
         else:
-            warnings.warn("More than 1 model type loaded, no non zero values removes",category=UserWarning)
+            warnings.warn("More than 1 model type loaded, no non zero values removes",category=RuntimeWarning)
 
-    def config_specific_actions(self):
+    def config_specific_actions(self, pre_set_state):
         """Function for actions which are specific to a combination of model with method.
 
             Note:
                 Be specific when these are used to only occur when wanted
 
             *#1: PF & HBV*:
                 Particle filters replace the full particle: thus the lag function also needs to be copied.
@@ -393,27 +416,33 @@
 
         #1
         if self.ensemble_method_name == "PF":
             # in particle filter the whole particle needs to be copied
             # when dealing with lag this is difficult as we don't want it in the regular state vector
 
             if "HBV" in self.lst_models_name and len(self.lst_models_name) == 1:
-                # first get the memory vectors for all ensemble members
-                lag_vector_arr = np.zeros((len(self.ensemble_list),TLAG_MAX))
-                for index, ensemble_member in enumerate(self.ensemble_list):
-                    t_lag = int(ensemble_member.get_value("Tlag")[0])
-                    old_t_lag = np.array([ensemble_member.get_value(f"memory_vector{i}") for i in range(t_lag)]).flatten()
-                    lag_vector_arr[index,:t_lag] = old_t_lag
-                # resample so has the correct state
-                # TODO consider adding noise ?
-                new_lag_vector_lst = lag_vector_arr[self.ensemble_method.resample_indices]
-
-                for index, ensembleMember in enumerate(self.ensemble_list):
-                    new_t_lag = ensembleMember.get_value(f"Tlag")
-                    [ensembleMember.set_value(f"memory_vector{mem_index}", np.array([new_lag_vector_lst[index, mem_index]])) for mem_index in range(int(new_t_lag))]
+                if pre_set_state:
+                    # first get the memory vectors for all ensemble members
+                    lag_vector_arr = np.zeros((len(self.ensemble_list),TLAG_MAX))
+                    for index, ensemble_member in enumerate(self.ensemble_list):
+                        t_lag = int(ensemble_member.get_value("Tlag")[0])
+                        old_t_lag = np.array([ensemble_member.get_value(f"memory_vector{i}") for i in range(t_lag)]).flatten()
+                        lag_vector_arr[index,:t_lag] = old_t_lag
+
+                    self.config_specific_storage = lag_vector_arr
+
+                else:
+                    lag_vector_arr = self.config_specific_storage
+                    # resample so has the correct state
+                    # TODO consider adding noise ?
+                    new_lag_vector_lst = lag_vector_arr[self.ensemble_method.resample_indices]
+
+                    for index, ensembleMember in enumerate(self.ensemble_list):
+                        new_t_lag = ensembleMember.get_value(f"Tlag")
+                        [ensembleMember.set_value(f"memory_vector{mem_index}", np.array([new_lag_vector_lst[index, mem_index]])) for mem_index in range(int(new_t_lag))]
 
             elif "HBV" in self.lst_models_name:
                 warnings.warn(f"Models implemented:{self.lst_models_name}, could cause issues with particle filters"
                               'HBV needs to update the lag vector but cannot due to other model type(s)',
                               category=RuntimeWarning)
             else:
                 warnings.warn(f"Not running `config_specific_actions`",category=UserWarning)
@@ -421,23 +450,18 @@
         #2...
 
     def get_value(self, var_name: str) -> np.ndarray:
         """Gets current value of whole ensemble for given variable ### currently assumes 2d, fix for 1d:"""
         # infer shape of state vector:
         ref_model = self.ensemble_list[0]
         shape_data = ref_model.get_value(var_name).shape[0]
-        # shape_var = len(self.variable_names)
-
 
         output_array = np.zeros((self.N, shape_data))
 
         self.logger.append(f'{output_array.shape}')
-        # for i, ensemble_member in enumerate(self.ensemble_list):
-        #     output_array[i] = ensemble_member.model.get_value(var_name)
-        # return output_array
 
         gathered_get_value = (self.gather(*[self.get_value_parallel(self,var_name, i) for i in range(self.N)]))
 
         with dask.config.set(self.dask_config):
             get_value_lst = gathered_get_value.compute()
 
         output_array = np.vstack(get_value_lst)
@@ -451,19 +475,14 @@
         return ensemble_member.model.get_value(var_name)
 
     def get_state_vector(self) -> np.ndarray:
         """Gets current value of whole ensemble for specified state vector
             Note:
                 Assumes 1d array? although :obj:`np.vstack` does work for 2d arrays
         """
-        # collect state vector
-        # output_lst = []
-        # for ensemble_member in self.ensemble_list:
-        #     output_lst.append(ensemble_member.get_state_vector())
-
         gathered_get_state_vector = (self.gather(*[self.get_state_vector_parallel(self, i) for i in range(self.N)]))
 
         with dask.config.set(self.dask_config):
             output_lst = gathered_get_state_vector.compute()
 
         return np.vstack(output_lst) # N x len(z)
 
@@ -474,16 +493,14 @@
         return ensemble_member.get_state_vector()
 
     def set_value(self, var_name: str, src: np.ndarray) -> None:
         """Sets current value of whole ensemble for given variable
             args:
                 src (np.ndarray): size = number of ensemble members x 1 [N x 1]
         """
-        # for i, ensemble_member in enumerate(self.ensemble_list):
-        #     ensemble_member.model.set_value(var_name, src[i])
         gathered_set_value = (self.gather(*[self.set_value_parallel(self, var_name, src[i], i) for i in range(self.N)]))
 
         with dask.config.set(self.dask_config):
             gathered_set_value.compute()
 
     @staticmethod
     @delayed
@@ -494,16 +511,14 @@
     def set_state_vector(self, src: np.ndarray) -> None:
         """Sets current value of whole ensemble for specified state vector
 
             args:
                 src (np.ndarray): size = number of ensemble members x number of states in state vector [N x len(z)]
                     src[0] should return the state vector for the first value
         """
-        # for i, ensemble_member in enumerate(self.ensemble_list):
-        #     ensemble_member.set_state_vector(src[i])
         gathered_set_state_vector = (self.gather(*[self.set_state_vector_parallel(self,src[i], i) for i in range(self.N)]))
 
         with dask.config.set(self.dask_config):
             gathered_set_state_vector.compute()
 
 
     @staticmethod
@@ -559,30 +574,33 @@
 
         config (:obj:`Path`): path to config file for the model which the EnsembleMember contains.
 
         state_vector (:obj:`np.ndarray`): numpy array containing last states which were gotten
 
         variable_names (list[str]): list of string containing the variables in the state vector.
 
+        loaded_models (dict[str, Any]): dictionary containing model names and their corresponding instances
+
     """
 
     model_name: str | None = None
     forcing: DefaultForcing | None = None
     setup_kwargs: dict | None = None
 
     state_vector_variables: Optional[str | list] = None
 
     model: Any | None = None
     config: Path | None = None
     state_vector: Any | None = None
     variable_names: list[str] | None = None
+    loaded_models: dict[str, Any] = dict()
 
     def setup(self) -> None:
         """Setups the model provided with forcing and kwargs. Set the config file"""
-        self.model = LOADED_MODELS[self.model_name](forcing=self.forcing)
+        self.model = self.loaded_models[self.model_name](forcing=self.forcing)
         self.config, _ = self.model.setup(**self.setup_kwargs)
 
     def initialize(self) -> None:
         """Initializes the model with the config file generated in setup"""
         self.model.initialize(self.config)
 
     def set_state_vector_variable(self):
@@ -655,15 +673,15 @@
 
     def update(self) -> None:
         """Updates the model to the next timestep"""
         self.model.update()
 
     def verify_model_loaded(self) -> None:
         """Checks whether specified model is available."""
-        if self.model_name in LOADED_MODELS:
+        if self.model_name in self.loaded_models:
             pass
         else:
             raise UserWarning(f"Defined model: {self.model} not loaded")
 
 
 """
 Data assimilation methods
```

### Comparing `ewatercycle_da-0.0.2/LICENSE.txt` & `ewatercycle_da-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_da-0.0.2/pyproject.toml` & `ewatercycle_da-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 path = "src/ewatercycle_DA/__init__.py"
 
 [project]
 name = "ewatercycle-DA"
 description = "Implementation of data assimilation for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology", "data assimilation","parallelisation"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

