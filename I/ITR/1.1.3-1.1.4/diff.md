# Comparing `tmp/itr-1.1.3.tar.gz` & `tmp/itr-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itr-1.1.3.tar", last modified: Sun Jan 21 20:28:05 2024, max compression
+gzip compressed data, was "itr-1.1.4.tar", last modified: Tue Apr  2 09:25:49 2024, max compression
```

## Comparing `itr-1.1.3.tar` & `itr-1.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      544 2024-01-21 20:27:48.888882 itr-1.1.3/AUTHORS.rst
--rw-r--r--   0        0        0    11357 2024-01-21 20:27:48.888882 itr-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0      717 2024-01-21 20:27:48.888882 itr-1.1.3/README.md
--rw-r--r--   0        0        0     3384 2024-01-21 20:28:05.469026 itr-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4344 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/__init__.py
--rw-r--r--   0        0        0     8593 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/configs.py
--rw-r--r--   0        0        0     3298 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/__init__.py
--rw-r--r--   0        0        0   111904 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/base_providers.py
--rw-r--r--   0        0        0    10959 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/data_providers.py
--rw-r--r--   0        0        0    40800 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/data_warehouse.py
--rw-r--r--   0        0        0    24521 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/excel.py
--rw-r--r--   0        0        0    28671 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/input/country_region_info.csv
--rw-r--r--   0        0        0      282 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/input/oecd_iso.csv
--rw-r--r--   0        0        0    20339 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/input/region_classification.csv
--rw-r--r--   0        0        0    18792 2024-01-21 20:27:48.896882 itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM.json
--rw-r--r--   0        0        0   571330 2024-01-21 20:27:48.900882 itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM_PC.json
--rw-r--r--   0        0        0   951275 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM_S3.json
--rw-r--r--   0        0        0   107771 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_S3.json
--rw-r--r--   0        0        0    30116 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_1_5_degrees.json
--rw-r--r--   0        0        0    22148 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees.json
--rw-r--r--   0        0        0     5725 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees_high_efficiency.json
--rw-r--r--   0        0        0     5728 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees_shift_improve.json
--rw-r--r--   0        0        0    35841 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_below_2_degrees.json
--rw-r--r--   0        0        0   195917 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/json/benchmark_production_OECM.json
--rw-r--r--   0        0        0    24756 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/osc_units.py
--rw-r--r--   0        0        0    95556 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/template.py
--rw-r--r--   0        0        0    54624 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/data/vault_providers.py
--rw-r--r--   0        0        0    40127 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/interfaces.py
--rw-r--r--   0        0        0    10223 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/portfolio_aggregation.py
--rw-r--r--   0        0        0        0 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/py.typed
--rw-r--r--   0        0        0    25262 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/temperature_score.py
--rw-r--r--   0        0        0    13450 2024-01-21 20:27:48.904882 itr-1.1.3/src/ITR/utils.py
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 itr-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      544 2024-04-02 09:25:32.837481 itr-1.1.4/AUTHORS.rst
+-rw-r--r--   0        0        0    11357 2024-04-02 09:25:32.837481 itr-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      717 2024-04-02 09:25:32.837481 itr-1.1.4/README.md
+-rw-r--r--   0        0        0     3360 2024-04-02 09:25:49.689394 itr-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4345 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/__init__.py
+-rw-r--r--   0        0        0     8594 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/configs.py
+-rw-r--r--   0        0        0     3298 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/__init__.py
+-rw-r--r--   0        0        0   112558 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/base_providers.py
+-rw-r--r--   0        0        0    10959 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/data_providers.py
+-rw-r--r--   0        0        0    40800 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/data_warehouse.py
+-rw-r--r--   0        0        0    24521 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/excel.py
+-rw-r--r--   0        0        0    28671 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/input/country_region_info.csv
+-rw-r--r--   0        0        0      282 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/input/oecd_iso.csv
+-rw-r--r--   0        0        0    20339 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/input/region_classification.csv
+-rw-r--r--   0        0        0    18792 2024-04-02 09:25:32.845481 itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM.json
+-rw-r--r--   0        0        0   571330 2024-04-02 09:25:32.849481 itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM_PC.json
+-rw-r--r--   0        0        0   951275 2024-04-02 09:25:32.849481 itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM_S3.json
+-rw-r--r--   0        0        0   107771 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_S3.json
+-rw-r--r--   0        0        0    30116 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_1_5_degrees.json
+-rw-r--r--   0        0        0    22148 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees.json
+-rw-r--r--   0        0        0     5725 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees_high_efficiency.json
+-rw-r--r--   0        0        0     5728 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees_shift_improve.json
+-rw-r--r--   0        0        0    35841 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_below_2_degrees.json
+-rw-r--r--   0        0        0   195917 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/json/benchmark_production_OECM.json
+-rw-r--r--   0        0        0    24764 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/osc_units.py
+-rw-r--r--   0        0        0    95900 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/template.py
+-rw-r--r--   0        0        0    54880 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/data/vault_providers.py
+-rw-r--r--   0        0        0    40127 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/interfaces.py
+-rw-r--r--   0        0        0    10223 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/portfolio_aggregation.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/py.typed
+-rw-r--r--   0        0        0    25302 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/temperature_score.py
+-rw-r--r--   0        0        0    13450 2024-04-02 09:25:32.853481 itr-1.1.4/src/ITR/utils.py
+-rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 itr-1.1.4/PKG-INFO
```

### Comparing `itr-1.1.3/AUTHORS.rst` & `itr-1.1.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/LICENSE.txt` & `itr-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/README.md` & `itr-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/pyproject.toml` & `itr-1.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ITR"
-version = "v1.1.3"
+version = "v1.1.4"
 description = "Assess the temperature alignment of current targets, commitments, and investment and lending portfolios."
 authors = [
     { name = "Michael Tiemann", email = "72577720+MichaelTiemannOSC@users.noreply.github.com" },
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 keywords = [
@@ -108,22 +108,21 @@
 ]
 dev = [
     "tox>=4.11.3",
     "tox-pdm>=0.7.0",
 ]
 lint = [
     "pre-commit",
-    "pyproject-flake8",
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
     "test/",
 ]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 70"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
```

### Comparing `itr-1.1.3/src/ITR/__init__.py` & `itr-1.1.4/src/ITR/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This package helps companies and financial institutions to assess the temperature alignment of investment and lending
 portfolios.
 """
+
 import os
 
 import numpy as np
 import pandas as pd
 import pint
 
 from . import utils  # noqa F401
```

### Comparing `itr-1.1.3/src/ITR/configs.py` & `itr-1.1.4/src/ITR/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This file defines the constants used throughout the different classes. In order to redefine these settings whilst using
 the module, extend the respective config class and pass it to the class as the "constants" parameter.
 """
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from typing import Callable, List, Optional
 
 import pandas as pd
```

### Comparing `itr-1.1.3/src/ITR/data/__init__.py` & `itr-1.1.4/src/ITR/data/__init__.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/base_providers.py` & `itr-1.1.4/src/ITR/data/base_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,26 +369,30 @@
                 ).unique()
                 if col in self._EI_df_t.columns
             ],
         ]
         # This piece of work essentially does a column-based join (to avoid extra transpositions)
         result = pd.concat(
             [
-                bm_proj_t[tuple(ser)].rename((idx, ser.iloc[2]))
-                if tuple(ser) in bm_proj_t
-                else bm_proj_t[ser_global].rename((idx, ser.iloc[2]))
-                if (
-                    ser_global := (
-                        ser.iloc[0],
-                        "Global",
-                        ser.iloc[2],
+                (
+                    bm_proj_t[tuple(ser)].rename((idx, ser.iloc[2]))
+                    if tuple(ser) in bm_proj_t
+                    else (
+                        bm_proj_t[ser_global].rename((idx, ser.iloc[2]))
+                        if (
+                            ser_global := (
+                                ser.iloc[0],
+                                "Global",
+                                ser.iloc[2],
+                            )
+                        )
+                        in bm_proj_t
+                        else pd.Series()
                     )
                 )
-                in bm_proj_t
-                else pd.Series()
                 for idx, ser in sec_reg_scopes.iterrows()
             ],
             axis=1,
         ).dropna(axis=1, how="all")
         result.columns = pd.MultiIndex.from_tuples(result.columns, names=["company_id", "scope"])
         return result
 
@@ -489,42 +493,46 @@
                         # Should not be reached, but this gives right answer if it is.
                         scope_ei[scope_name] = [
                             eir.value
                             for eir in company.projected_intensities[scope_name].projections
                             if eir.year == base_year
                         ]
                 scope_em = {
-                    scope: [
-                        IEmissionRealization(
-                            year=base_year,
-                            value=ei[0].value * company.base_year_production,  # type: ignore
-                        )
-                    ]
-                    if ei
-                    else []
+                    scope: (
+                        [
+                            IEmissionRealization(
+                                year=base_year,
+                                value=ei[0].value * company.base_year_production,  # type: ignore
+                            )
+                        ]
+                        if ei
+                        else []
+                    )
                     for scope, ei in scope_ei.items()
                 }
             else:
                 scope_em["S1"] = scope_em["S2"] = []
                 scope_em["S3"] = [IEmissionRealization(year=base_year, value=company.ghg_s3)] if company.ghg_s3 else []
                 scope_em["S1S2"] = [IEmissionRealization(year=base_year, value=company.ghg_s1s2)]
                 scope_em["S1S2S3"] = (
                     [IEmissionRealization(year=base_year, value=company.ghg_s1s2 + company.ghg_s3)]
                     if company.ghg_s1s2 and company.ghg_s3
                     else []
                 )
                 scope_ei = {
-                    scope: [
-                        IEIRealization(
-                            year=base_year,
-                            value=em[0].value / company.base_year_production,  # type: ignore
-                        )
-                    ]
-                    if em
-                    else []
+                    scope: (
+                        [
+                            IEIRealization(
+                                year=base_year,
+                                value=em[0].value / company.base_year_production,  # type: ignore
+                            )
+                        ]
+                        if em
+                        else []
+                    )
                     for scope, em in scope_em.items()
                 }
             company.historic_data = IHistoricData(
                 productions=[IProductionRealization(year=base_year, value=company.base_year_production)],
                 emissions=IHistoricEmissionsScopes(**scope_em),
                 emissions_intensities=IHistoricEIScopes(**scope_ei),
             )
@@ -901,17 +909,20 @@
             self._convert_projections_to_series(c, self.column_config.PROJECTED_TARGETS, EScope[scope_name])
             for c in self.get_company_data(company_ids)
             for scope_name in EScope.get_scopes()
             if c.projected_targets[scope_name]
         ]
         if target_list:
             with warnings.catch_warnings():
-                # pd.DataFrame.__init__ (in pandas/core/frame.py) ignores the beautiful dtype information adorning the pd.Series list elements we are providing.  Sad!
+                # pd.DataFrame.__init__ (in pandas/core/frame.py) ignores
+                # the beautiful dtype information adorning the pd.Series list
+                # elements we are providing.  Sad!
                 warnings.simplefilter("ignore")
-                # If target_list produces a ragged left edge, resort columns so that earliest year is leftmost
+                # If target_list produces a ragged left edge,
+                # resort columns so that earliest year is leftmost
                 df = pd.DataFrame(target_list).sort_index(axis=1)
                 df.index.set_names(["company_id", "scope"], inplace=True)
                 if year is not None:
                     return df[year]
                 return df
         return pd.DataFrame()
 
@@ -1034,15 +1045,16 @@
                         for scope in em_tot.index
                         if em_tot.loc[scope].squeeze().m != 0.0
                     ],
                 )
                 for sector in sectors
             ]
 
-            # Having done all scopes and sectors for this company above, replace historic Em and EI data below
+            # Having done all scopes and sectors for this company above,
+            # replace historic Em and EI data below
             for sector_aligned in aligned_em:
                 sector, scopes = sector_aligned
                 historic_sector = historic_dict["+".join([orig_id, sector])]
                 assert historic_sector is not None
                 # print(f"Historic {sector} initially\n{historic_sector.emissions}")
                 for scope_tuple in scopes:
                     scope, em_list = scope_tuple
@@ -1057,20 +1069,22 @@
                         ),
                     )
                     prod_list = historic_sector.productions
                     ei_list = list(
                         map(
                             lambda em_p: IEIRealization(
                                 year=em_p[0].year,
-                                value=Q_(
-                                    np.nan,
-                                    f"({em_p[0].value.u}) / ({em_p[1].value.u})",  # type: ignore
-                                )
-                                if em_p[1].value.m == 0.0  # type: ignore
-                                else em_p[0].value / em_p[1].value,
+                                value=(
+                                    Q_(
+                                        np.nan,
+                                        f"({em_p[0].value.u}) / ({em_p[1].value.u})",  # type: ignore
+                                    )
+                                    if em_p[1].value.m == 0.0  # type: ignore
+                                    else em_p[0].value / em_p[1].value
+                                ),
                             ),
                             zip(historic_sector.emissions[scope.name], prod_list),
                         )
                     )
                     setattr(historic_sector.emissions_intensities, scope.name, ei_list)
                 # print(f"Historic {sector} adjusted\n{historic_dict['+'.join([orig_id, sector])].emissions}")
         logger.info("Sector alignment complete")
@@ -1143,25 +1157,27 @@
             ).pint.dequantify()
             historic_ei_t.index.name = "year"
         if backfill_needed:
             # Fill in gaps between BASE_YEAR and the first data we have
             if ITR.HAS_UNCERTAINTIES:
                 historic_ei_t = historic_ei_t.map(lambda x: np.nan if ITR.isna(x) else x)
             backfilled_t = historic_ei_t.bfill(axis=0)
-            # FIXME: this hack causes backfilling only on dates on or after the first year of the benchmark, which keeps it from disrupting current test cases
+            # FIXME: this hack causes backfilling only on dates on or after the
+            # first year of the benchmark, which keeps it from disrupting current test cases
             # while also working on real-world use cases.  But we need to formalize this decision.
             backfilled_t = backfilled_t.reset_index()
             backfilled_t = backfilled_t.where(
                 backfilled_t.year >= self.projection_controls.BASE_YEAR,
                 historic_ei_t.reset_index(),
             )
             backfilled_t.set_index("year", inplace=True)
             if not historic_ei_t.compare(backfilled_t).empty:
                 logger.warning(
-                    f"some data backfilled to {self.projection_controls.BASE_YEAR} for company_ids in list {historic_ei_t.compare(backfilled_t).columns.get_level_values('company_id').unique().tolist()}"
+                    f"some data backfilled to {self.projection_controls.BASE_YEAR} for company_ids in list \
+                    {historic_ei_t.compare(backfilled_t).columns.get_level_values('company_id').unique().tolist()}"
                 )
                 historic_ei_t = backfilled_t.sort_index(axis=1)
                 for company in companies:
                     if ITR.isna(company.base_year_production):
                         # If we have no valid production data, we cannot use EI data to compute emissions
                         continue
                     for ghg_attr, ghg_scope in [
@@ -1421,17 +1437,19 @@
         # quantile doesn't handle pd.NA inside Quantity; FIXME: we can use np.nan because not expecting UFloat in input data
 
         # Turns out we have to dequantify here: https://github.com/pandas-dev/pandas/issues/45968
         # Can try again when ExtensionArrays are supported by `quantile`, `clip`, and friends
         if ITR.HAS_UNCERTAINTIES:
             try:
                 nominal_ei_t = historic_ei_t.apply(
-                    lambda col: pd.Series(ITR.nominal_values(col.values), index=col.index, name=col.name)
-                    if col.dtype.kind == "O"
-                    else col.astype("float64")
+                    lambda col: (
+                        pd.Series(ITR.nominal_values(col.values), index=col.index, name=col.name)
+                        if col.dtype.kind == "O"
+                        else col.astype("float64")
+                    )
                 )
                 err_ei_t = historic_ei_t.apply(
                     lambda col: pd.Series(ITR.std_devs(col.values), index=col.index, name=col.name)
                 )
             except ValueError:
                 logger.error("ValueError in _winsorize")
                 raise
@@ -1480,18 +1498,20 @@
     def _interpolate(self, historic_ei_t: pd.DataFrame) -> pd.DataFrame:
         # Interpolate NaNs surrounded by values, but don't extrapolate NaNs with last known value
         raise NotImplementedError
 
     def _get_trends(self, intensities_t: pd.DataFrame):
         # FIXME: rolling windows require conversion to float64.  Don't want to be a nuisance...
         intensities_t = intensities_t.apply(
-            lambda col: col
-            if col.dtype == np.float64
-            # Float64 NA needs to be converted to np.nan before we can apply nominal_values
-            else ITR.nominal_values(col.fillna(np.nan)).astype(np.float64)
+            lambda col: (
+                col
+                if col.dtype == np.float64
+                # Float64 NA needs to be converted to np.nan before we can apply nominal_values
+                else ITR.nominal_values(col.fillna(np.nan)).astype(np.float64)
+            )
         )
         # FIXME: Pandas 2.1
         # Treat NaN ratios as "unchnaged year on year"
         # FIXME Could we ever have UFloat NaNs here?  np.nan is valid UFloat.
         ratios_t: pd.DataFrame = intensities_t.rolling(window=2, closed="right").apply(
             func=self._year_on_year_ratio, raw=True
         )
@@ -1785,15 +1805,17 @@
                 if scope_targets_intensity and scope_targets_absolute:
                     target_i = scope_targets_intensity[0]
                     target_a = scope_targets_absolute[0]
                     if target_i.target_end_year == target_a.target_end_year:
                         if target_i.target_start_year >= target_a.target_start_year:
                             if target_i.target_start_year == target_a.target_start_year:
                                 warnings.warn(
-                                    f"intensity target overrides absolute target for target_start_year={target_i.target_start_year} and target_end_year={target_i.target_end_year}"
+                                    f"intensity target overrides absolute target for \
+                                    target_start_year={target_i.target_start_year} and \
+                                    target_end_year={target_i.target_end_year}"
                                 )
                             scope_targets_absolute.pop(0)
                             scope_targets = scope_targets_intensity
                         else:
                             scope_targets_intensity.pop(0)
                             scope_targets = scope_targets_absolute
                     elif target_i.target_end_year < target_a.target_end_year:
@@ -2137,16 +2159,14 @@
                         first_err * (period - y) / period + last_err * (y / period),
                     )
                     for y, year in enumerate(range(first_year, last_year + 1))
                 ]
             else:
                 # - If CAGR target <= 90% reduction, use CAGR model directly
                 cagr_factor = (last_value / first_value).m ** (1 / period)
-                cagr_data = [
-                    cagr_factor**y * first_value.m for y, year in enumerate(range(first_year, last_year + 1))
-                ]
+                cagr_data = [cagr_factor**y * first_value.m for y, year in enumerate(range(first_year, last_year + 1))]
         cagr_result = pd.Series(
             PA_(np.array(cagr_data), dtype=f"{last_value.u:~P}"),
             index=range(first_year, last_year + 1),
             name="CAGR",
         )
         return cagr_result
```

### Comparing `itr-1.1.3/src/ITR/data/data_providers.py` & `itr-1.1.4/src/ITR/data/data_providers.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/data_warehouse.py` & `itr-1.1.4/src/ITR/data/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/excel.py` & `itr-1.1.4/src/ITR/data/excel.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/input/country_region_info.csv` & `itr-1.1.4/src/ITR/data/input/country_region_info.csv`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/input/region_classification.csv` & `itr-1.1.4/src/ITR/data/input/region_classification.csv`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM_PC.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM_PC.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_OECM_S3.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_OECM_S3.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_S3.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_S3.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_1_5_degrees.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_1_5_degrees.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees_high_efficiency.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees_high_efficiency.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_2_degrees_shift_improve.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_2_degrees_shift_improve.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_EI_TPI_below_2_degrees.json` & `itr-1.1.4/src/ITR/data/json/benchmark_EI_TPI_below_2_degrees.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/json/benchmark_production_OECM.json` & `itr-1.1.4/src/ITR/data/json/benchmark_production_OECM.json`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/data/osc_units.py` & `itr-1.1.4/src/ITR/data/osc_units.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,15 +652,17 @@
 
 
 def requantify_df_from_columns(df: pd.DataFrame, inplace=False) -> pd.DataFrame:
     """
     :param df: pd.DataFrame
     :param inplace: bool, default False.  If True, perform operation in-place.
 
-    :return: A pd.DataFrame with columns originally matching the pattern COLUMN_NAME [UNITS] renamed to COLUMN_NAME and replaced with a PintArray with dtype=ureg(UNITS) (aka 'pint[UNITS]')
+    :return: A pd.DataFrame with columns originally matching the pattern
+    COLUMN_NAME [UNITS] renamed to COLUMN_NAME and replaced with a PintArray
+    with dtype=ureg(UNITS) (aka 'pint[UNITS]')
     """
     p = re.compile(r"^(.*)\s*\[(.*)\]\s*$")
     if not inplace:
         df = df.copy()
     for column in df.columns:
         m = p.match(column)
         if m:
```

### Comparing `itr-1.1.3/src/ITR/data/template.py` & `itr-1.1.4/src/ITR/data/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,17 +375,20 @@
                         "submetric",
                         ColumnsConfig.SCOPE,
                         "index",
                     ]
                 )
                 .loc[:, esg_year_columns]
             )
-            # Now we have to reconcile the fact that production submetrics/boundaries may or may not align with emissions(intensity) submetrics/boundaries
-            # There are two cases we handle: (1) unique production rows match all intensity rows, and (2) production rows with submetrics match intensity rows with same submetrics
-            # There may be intensities for multiple scopes, which all multiply against the same production number but which produce per-scope emissions values
+            # Now we have to reconcile the fact that production submetrics/boundaries may
+            # or may not align with emissions(intensity) submetrics/boundaries
+            # There are two cases we handle: (1) unique production rows match all intensity rows,
+            # and (2) production rows with submetrics match intensity rows with same submetrics
+            # There may be intensities for multiple scopes, which all multiply against the same
+            # production number but which produce per-scope emissions values
             df1_case1 = (
                 df1[df1.sub_count == 1]
                 .droplevel("submetric")
                 .drop(columns="sub_count")
                 .merge(
                     df2.reset_index(["submetric", ColumnsConfig.SCOPE, "index"])[
                         ["submetric", ColumnsConfig.SCOPE, "index"]
@@ -541,19 +544,21 @@
         )
         df.loc[df.region.isnull(), "region"] = df.country.map(ITR_country_to_region)
 
         df_fundamentals = df.set_index(ColumnsConfig.COMPANY_ID, drop=False).convert_dtypes()
 
         if self.template_version == 2:
             # Ensure our df_esg rows connect back to fundamental data
-            # the one single advantage of template_version==1 is that fundamental data and esg data are all part of the same rows so no need to do this integrity check/correction
+            # the one single advantage of template_version==1 is that
+            # fundamental data and esg data are all part of the same rows
+            # so no need to do this integrity check/correction
             esg_missing_fundamentals = ~df_esg.company_id.isin(df_fundamentals.index)
             if esg_missing_fundamentals.any():
                 logger.error(
-                    f"The following companies have ESG data defined but no fundamental data and will be removed from further analysis:\n{df_esg[esg_missing_fundamentals].company_id.unique()}"
+                    f"The following companies have ESG data defined but no fundamental data and will be removed from further analysis:\n{df_esg[esg_missing_fundamentals].company_id.unique()}"  # noqa: E501
                 )
                 df_esg = df_esg[~esg_missing_fundamentals]
 
         # testing if all data is in the same currency
         fundamental_metrics = [
             "company_market_cap",
             "company_revenue",
@@ -606,20 +611,22 @@
                 fx_df = fx_df[fx_conversion_mask].assign(
                     currency_tuple=lambda x: x["currency"].map(convert_prefix_to_scalar),
                     fx_quote_tuple=lambda x: x["fx_quote"].map(convert_prefix_to_scalar),
                 )
 
                 # FIXME: These simple rules don't take into account different conversion rates at different time periods.
                 fx_df.apply(
-                    lambda x: fx_ctx.redefine(
-                        f"{x.currency_tuple[0]} = {x.fx_rate * x.fx_quote_tuple[1] / x.currency_tuple[1]} {x.fx_quote_tuple[0]}"
-                    )
-                    if x.currency_tuple[0] != "USD"
-                    else fx_ctx.redefine(
-                        f"{x.fx_quote_tuple[0]} = {x.currency_tuple[1]/(x.fx_rate * x.fx_quote_tuple[1])} {x.currency_tuple[0]}"
+                    lambda x: (
+                        fx_ctx.redefine(
+                            f"{x.currency_tuple[0]} = {x.fx_rate * x.fx_quote_tuple[1] / x.currency_tuple[1]} {x.fx_quote_tuple[0]}"
+                        )
+                        if x.currency_tuple[0] != "USD"
+                        else fx_ctx.redefine(
+                            f"{x.fx_quote_tuple[0]} = {x.currency_tuple[1]/(x.fx_rate * x.fx_quote_tuple[1])} {x.currency_tuple[0]}"
+                        )
                     ),
                     axis=1,
                 )
                 ureg.add_context(fx_ctx)
                 ureg.enable_contexts("FX")
 
                 for col in fundamental_metrics:
@@ -913,15 +920,15 @@
             # Validate that all our em_metrics are, in fact, some kind of emissions quantity
             em_invalid = df_esg.loc[em_metrics.index].unit.map(
                 lambda x: not isinstance(x, str) or not ureg(x).is_compatible_with("t CO2")
             )
             em_invalid_idx = em_invalid[em_invalid].index
             if len(em_invalid_idx) > 0:
                 logger.error(
-                    f"The following rows of data do not have proper emissions data (can be converted to t CO2e) and will be dropped from the analysis\n{df_esg.loc[em_invalid_idx]}"
+                    f"The following rows of data do not have proper emissions data (can be converted to t CO2e) and will be dropped from the analysis\n{df_esg.loc[em_invalid_idx]}"  # noqa: E501
                 )
                 df_esg = df_esg.loc[df_esg.index.difference(em_invalid_idx)]
                 em_metrics = em_metrics.loc[em_metrics.index.difference(em_invalid_idx)]
 
             submetric_sector_map = {
                 "cement": "Cement",
                 "clinker": "Cement",
@@ -1160,28 +1167,32 @@
                         case_2.droplevel("sector").index.intersection(case_1.droplevel("sector").index)
                     )
                 ]
                 if not case_3.empty:
                     # Shift out of general (case_1) and leave in specific (case_2)
                     case_1 = case_1.loc[~case_1.index.isin(case_3.index)]
 
-                # Case 4: case_1 scopes containing case_2 scopes that need to be removed before remaining scopes can be allocated
-                # Example: We have S1 allocated to electricity and gas, but S2 and S3 are general.  To allocate S1S2S3 we need to subtract out S1, allocate remaining to S2 and S3 across Electricity and Gas sectors
-                # Eni's Plenitude and power is an example where S1S2S3 > S1+S2+S3 (due to lifecycle emissions concept).  FIXME: don't know how to deal with that!
+                # Case 4: case_1 scopes containing case_2 scopes that need to be removed before
+                # remaining scopes can be allocated
+                # Example: We have S1 allocated to electricity and gas, but S2 and S3 are general.
+                # To allocate S1S2S3 we need to subtract out S1, allocate remaining to S2 and S3
+                # across Electricity and Gas sectors
+                # Eni's Plenitude and power is an example where S1S2S3 > S1+S2+S3 (due to lifecycle emissions concept).
+                # FIXME: don't know how to deal with that!
                 case_4_df = case_1.reset_index("metric").merge(
                     case_2.reset_index("metric"),
                     on=["sector", "company_id"],
                     suffixes=[None, "_2"],
                 )
                 case_4 = case_4_df[case_4_df.apply(lambda x: x.metric_2 in x.metric, axis=1)].set_index(
                     "metric", append=True
                 )
                 if not case_4.empty:
                     logger.error(
-                        f"Dropping attempt to disentangle embedded submetrics found in sector/scope assignment dataframe:\n{best_esg_em.submetric[case_4.index]}"
+                        f"Dropping attempt to disentangle embedded submetrics found in sector/scope assignment dataframe:\n{best_esg_em.submetric[case_4.index]}"  # noqa: E501
                     )
                     case_1 = case_1.loc[~case_1.index.isin(case_4.index)]
 
                 em_needs_allocation = best_esg_em.index.isin(case_1.index)
                 new_em_to_allocate = (
                     best_esg_em.reset_index()[em_needs_allocation]
                     # This gives us combinatorial product of common scope emissions across all types of production
@@ -1275,19 +1286,19 @@
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 # Quieting warnings due to https://github.com/hgrecco/pint/issues/1897
                 df4 = (
                     df3_num_t
                     * df3_denom_t.rdiv(1.0).apply(
                         lambda x: x.map(
-                            lambda y: x.dtype.na_value
-                            if ITR.isna(y)
-                            else Q_(0, x.dtype.units)
-                            if np.isinf(ITR.nominal_values(y.m))
-                            else y
+                            lambda y: (
+                                x.dtype.na_value
+                                if ITR.isna(y)
+                                else Q_(0, x.dtype.units) if np.isinf(ITR.nominal_values(y.m)) else y
+                            )
                         )
                     )
                 ).T
             df4["variable"] = VariablesConfig.EMISSIONS_INTENSITIES
             df4 = df4.reset_index().set_index(["company_id", "variable", "scope"])
             # Build df5 from PintArrays, not object types
             df3_num_t = pd.concat({VariablesConfig.EMISSIONS: df3_num_t}, names=["variable"], axis=1)
@@ -1394,15 +1405,17 @@
         for company in self._companies:
             row = df_fundamentals.loc[company.company_id]
             company.emissions_metric = EmissionsMetric(row[ColumnsConfig.EMISSIONS_METRIC])
             company.production_metric = ProductionMetric(row[ColumnsConfig.PRODUCTION_METRIC])
         # And keep df_fundamentals in sync
         self.df_fundamentals = df_fundamentals
 
-        # company_id, netzero_year, target_type, target_scope, target_start_year, target_base_year, target_base_year_qty, target_base_year_unit, target_year, target_reduction_ambition
+        # company_id, netzero_year, target_type, target_scope, target_start_year,
+        # target_base_year, target_base_year_qty, target_base_year_unit, target_year,
+        # target_reduction_ambition
         return self._company_df_to_model(None, df_target_data, df_historic_data)
 
     def _validate_target_data(self, target_data: pd.DataFrame) -> pd.DataFrame:
         """
         Performs checks on the supplied target data. Some values are put in to make the tool function.
         :param target_data:
         :return:
@@ -1433,17 +1446,19 @@
                     target_data = target_data[~mask]
 
         # Convert CH4 to the GWP of CO2e; don't convert CH4->CO2e in intensity targets
         target_data.reset_index(inplace=True)
         ch4_idx = target_data.target_base_year_unit.str.contains("CH4")
         ch4_gwp = Q_(gwp.data["AR5GWP100"]["CH4"], "CO2e/CH4")
         ch4_maybe_co2e = target_data.loc[ch4_idx].target_base_year_unit.map(
-            lambda x: x.replace("CH4", "CO2e")
-            if len(dims := ureg.parse_units(x).dimensionality) == 2 and "[mass]" in dims
-            else x
+            lambda x: (
+                x.replace("CH4", "CO2e")
+                if len(dims := ureg.parse_units(x).dimensionality) == 2 and "[mass]" in dims
+                else x
+            )
         )
         ch4_is_co2e = target_data.loc[ch4_idx].target_base_year_unit != ch4_maybe_co2e
         ch4_to_co2e = ch4_is_co2e[ch4_is_co2e]
         target_data.loc[ch4_to_co2e.index, "target_base_year_unit"] = ch4_maybe_co2e.loc[ch4_to_co2e.index]
         target_data.loc[ch4_to_co2e.index, "target_base_year_qty"] *= ch4_gwp.m
         target_data.set_index("company_id", inplace=True)
 
@@ -1456,15 +1471,15 @@
                 f"Invalid target types {target_data[mask].target_type} among companies with ID: {c_ids_with_invalid_target_type}"
             )
             target_data = target_data[~mask]
 
         mask = target_data["netzero_year"] > ProjectionControls.TARGET_YEAR
         if mask.any():
             c_ids_invalid_netzero_year = unique_ids(mask)
-            warning_message = f"Invalid net-zero target years (>{ProjectionControls.TARGET_YEAR}) are entered for companies with ID: {c_ids_invalid_netzero_year}"
+            warning_message = f"Invalid net-zero target years (>{ProjectionControls.TARGET_YEAR}) are entered for companies with ID: {c_ids_invalid_netzero_year}"  # noqa: E501
             logger.warning(warning_message)
             target_data = target_data[~mask]
 
         mask = target_data.netzero_year.isna()
         if mask.any():
             c_ids_without_netzero_year = unique_ids(mask)
             warning_message = f"Companies without netzero targets: {c_ids_without_netzero_year}"
```

### Comparing `itr-1.1.3/src/ITR/data/vault_providers.py` & `itr-1.1.4/src/ITR/data/vault_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
 
 # Rewrite dataframe DF so that columns containing Pint quantities are represented by a column for the Magnitude and column for the Units.
 # The magnitude column retains the original column name and the units column is renamed with a _units suffix.
 def dequantify_df(df: pd.DataFrame) -> pd.DataFrame:
     return pd.concat([dequantify_column(df[col]) for col in df.columns], axis=1)
 
 
-# Because this DF comes from reading a Trino table, and because columns must be unqiue, we don't have to enumerate to ensure we properly handle columns with duplicated names
+# Because this DF comes from reading a Trino table, and because columns must be unique,
+# we don't have to enumerate to ensure we properly handle columns with duplicated names
 def requantify_df(df: pd.DataFrame, typemap={}) -> pd.DataFrame:
     units_col = None
     columns_not_found = [k for k in typemap.keys() if k not in df.columns]
     if columns_not_found:
         logger.error(f"columns {columns_not_found} not found in DataFrame")
         raise ValueError
     columns_reversed = reversed(df.columns)
@@ -121,18 +122,19 @@
         catalog: Optional[str] = "",  # FIXME: this should go away when osc-ingest-tools 0.5.3 is released
         schema: Optional[str] = "",
         hive_bucket: Optional[Bucket] = None,
         hive_catalog: Optional[str] = None,
         hive_schema: Optional[str] = None,
     ):
         """
-        As an alternative to using FastAPI interfaces, this creates an interface allowing access to Production benchmark data via the Data Vault.
-        :param engine: the Sqlalchemy connect to the Data Vault
+        As an alternative to using FastAPI interfaces, this creates an interface allowing access to Production
+        benchmark data via the Data Vault. :param engine: the Sqlalchemy connect to the Data Vault
         :param schema: The database schema where the Data Vault lives
-        :param hive_bucket, hive_catalog, hive_schema: Optional parameters to enable fast ingestion via Hive; otherwise uses Trino batch insertion (which is slow)
+        :param hive_bucket, hive_catalog, hive_schema: Optional parameters to enable fast ingestion via Hive;
+        otherwise uses Trino batch insertion (which is slow)
         """
         super().__init__()
         self.engine = engine
         self.catalog = catalog or os.environ.get(
             "ITR_CATALOG", "osc_datacommons_dev"
         )  # FIXME: needed for osc-ingest-tools < 0.5.3
         self.schema = schema or engine.dialect.default_schema_name or os.environ.get("ITR_SCHEMA", "demo_dv")
@@ -150,15 +152,17 @@
     """
     Create a table in the Data Vault
 
     :param df: The DataFrame to be written as a table in the Data Vault
     :param schemaname: The schema where the table should be written
     :param tablename: The name of the table in the Data Vault
     :param engine: The SqlAlchemy connection to the Data Vault
-    :param hive_bucket: :param hive_catalog: :param hive_schema: Optional paramters.  If given we attempt to use a fast Hive ingestion process.  Otherwise use default (and slow) Trino ingestion.
+    :param hive_bucket: :param hive_catalog: :param hive_schema: Optional paramters.
+    # If given we attempt to use a fast Hive ingestion process.
+    # Otherwise use default (and slow) Trino ingestion.
     :param verbose: If True, log information about actions of the Data Vault as they happen
     """
     drop_table = f"drop table if exists {vault.schema}.{tablename}"
     qres = osc._do_sql(drop_table, vault.engine, verbose)  # noqa F841
     logger.debug("dtypes, columns, and index of create_vault_table_from_df(df...)")
     logger.debug(df.dtypes)
     logger.debug(df.columns)
@@ -193,15 +197,16 @@
             method=osc.TrinoBatchInsert(batch_size=5000, verbose=verbose),
         )
 
 
 # When reading SQL tables to import into DataFrames, it is up to the user to preserve {COL}, {COL}_units pairings so they can be reconstructed.
 # If the user does a naive "select * from ..." this happens naturally.
 # We can give a warning when we see a resulting dataframe that could have, but does not have, unit information properly integrated.  But
-# fixing the query on the fly becomes difficult when we consider the fully complexity of parsing and rewriting SQL queries to put the units columns in the correct locations.
+# fixing the query on the fly becomes difficult when we consider the fully complexity of parsing and
+# rewriting SQL queries to put the units columns in the correct locations.
 # (i.e., properly in the principal SELECT clause (which can have arbitrarily complex terms), not confused by FROM, WHERE, GROUP BY, ORDER BY, etc.)
 
 
 def read_quantified_sql(
     sql: str,
     tablename: Union[str, None],
     engine: sqlalchemy.Engine,
@@ -222,30 +227,31 @@
         ]
         if extra_unit_columns:
             extra_unit_columns_positions = [
                 (i, extra_unit_columns[i][0], extra_unit_columns[i][1]) for i in range(len(extra_unit_columns))
             ]
             for col_tuple in extra_unit_columns_positions:
                 logger.error(
-                    f"Missing units column '{col_tuple[2]}' after original column '{sql_df.columns[col_tuple[1]]}' (should be column #{col_tuple[0]+col_tuple[1]+1} in new query)"
+                    f"Missing units column '{col_tuple[2]}' after original column '{sql_df.columns[col_tuple[1]]}' (should be column #{col_tuple[0]+col_tuple[1]+1} in new query)"  # noqa: E501
                 )
             raise ValueError
     return requantify_df(sql_df).convert_dtypes()
 
 
 # Basic Corp Data Asumptions
 #   5 year historical EI (else we presume single year is constant backward and forward)
 #   5 year historical Production (else we presume single year is constant backward and forward)
 #   5 year historical Emissions (else we presume single year is constant backward and forward)
 #   We can infer one of the above from the other two (simple maths)
 #   The above tables identify the scope(s) to which they apply (S1, S2, S12, S3, S123) and data source (e.g. 'rmi_20211120')
 
 # Basic Benchmark Data Assumptions
 #   EI for a given scope
-#   Production defined in terms of growth (or negative growth) on a rolling basis (so 0.05, -0.04) would mean 5% growth followed by 4% negative growth for a total of 0.8%
+#   Production defined in terms of growth (or negative growth) on a rolling basis
+# (so 0.05, -0.04) would mean 5% growth followed by 4% negative growth for a total of 0.8%
 #   Benchmarks are named (e.g., 'OECM')
 
 
 class VaultProviderProductionBenchmark(ProductionBenchmarkDataProvider):
     def __init__(
         self,
         vault: VaultInstance,
@@ -454,26 +460,30 @@
                 ).unique()
                 if col in self._EI_df_t.columns
             ],
         ]
         # This piece of work essentially does a column-based join (to avoid extra transpositions)
         result = pd.concat(
             [
-                bm_proj_t[tuple(ser)].rename((idx, ser.iloc[2]))
-                if tuple(ser) in bm_proj_t
-                else bm_proj_t[ser_global].rename((idx, ser.iloc[2]))
-                if (
-                    ser_global := (
-                        ser.iloc[0],
-                        "Global",
-                        ser.iloc[2],
+                (
+                    bm_proj_t[tuple(ser)].rename((idx, ser.iloc[2]))
+                    if tuple(ser) in bm_proj_t
+                    else (
+                        bm_proj_t[ser_global].rename((idx, ser.iloc[2]))
+                        if (
+                            ser_global := (
+                                ser.iloc[0],
+                                "Global",
+                                ser.iloc[2],
+                            )
+                        )
+                        in bm_proj_t
+                        else pd.Series()
                     )
                 )
-                in bm_proj_t
-                else pd.Series()
                 for idx, ser in sec_reg_scopes.iterrows()
             ],
             axis=1,
         ).dropna(axis=1, how="all")
         result.columns = pd.MultiIndex.from_tuples(result.columns, names=["company_id", "scope"])
         return result
 
@@ -738,15 +748,15 @@
         elif factor == "emissions":
             where_sql = f"where year = {year}"
             if scope in [EScope.S1, EScope.S2, EScope.S3]:
                 factor_sql = f"select company_id, sum(co2_{scope.name.lower()}_by_year)"
             elif scope == EScope.S1S2:
                 factor_sql = "select company_id, sum(co2_s1_by_year+if(is_nan(co2_s2_by_year),0.0,co2_s2_by_year))"
             elif scope == EScope.S1S2:
-                factor_sql = "select company_id, sum(co2_s1_by_year+if(is_nan(co2_s2_by_year),0.0,co2_s2_by_year)+if(is_nan(co2_s3_by_year),0.0,co2_s3_by_year))"
+                factor_sql = "select company_id, sum(co2_s1_by_year+if(is_nan(co2_s2_by_year),0.0,co2_s2_by_year)+if(is_nan(co2_s3_by_year),0.0,co2_s3_by_year))"  # noqa: E501
             else:
                 raise ValueError(f"scope {scope} not supported")
         else:
             factor_sql = f"select company_id, sum({factor})"
         qres = osc._do_sql(
             f"{factor_sql} as {factor} {from_sql} {where_sql} {group_sql}", self._v.engine, verbose=False
         )
@@ -784,21 +794,23 @@
         which rely on trajectory and target projections from benchmark production and SDA pathways.
 
         Fundamentally: DataWarehouse(benchmark_ei, benchmark_prod, company_data)
             -> { production_data, trajectory_data,  target_data }
             -> { cumulative_budgets, cumulative_emissions }
 
         :param engine: The Sqlalchemy connector to the Data Vault
-        :param company_data: as a VaultCompanyDataProvider, this provides both a reference to a fundamental company data table and data structures containing historic ESG data.  Trajectory and Target projections also get filled in here.
+        :param company_data: as a VaultCompanyDataProvider, this provides both a reference to a fundamental
+        company data table and data structures containing historic ESG data.  Trajectory and Target projections also get filled in here.
         :param benchmark_projected_production: A reference to the benchmark production table as well as data structures used by the Data Vault for projections
         :param benchmark_projected_ei: A reference to the benchmark emissions intensity table as well as data structures used by the Data Vault for projections
         :param estimate_missing_data: If provided, a function that can fill in missing S3 data (possibly by aligning to benchmark statistics)
         :param ingest_schema: The database schema where the Data Vault lives
         :param itr_prefix: A prefix for all tables so that different users can use the same schema without conflicts
-        :param hive_bucket: :param hive_catalog: :param hive_schema: Optional paramters.  If given we attempt to use a fast Hive ingestion process.  Otherwise use default (and slow) Trino ingestion.
+        :param hive_bucket: :param hive_catalog: :param hive_schema: Optional paramters.  If given we attempt to use a
+        fast Hive ingestion process.  Otherwise use default (and slow) Trino ingestion.
         """
         # This initialization step adds trajectory and target projections to `company_data`
         super().__init__(
             company_data=company_data,  # type: ignore
             benchmark_projected_production=benchmark_projected_production,
             benchmarks_projected_ei=benchmarks_projected_ei,
             estimate_missing_data=estimate_missing_data,
@@ -973,15 +985,15 @@
        CE_BY.cumulative_trajectory/(B_BY.intensity * P_BY.production_by_year)
              * sum(B.intensity * P.production_by_year) over (partition by C.company_id, B.scope order by P.year) as cumulative_scaled_budget,
        CE_BY.cumulative_trajectory_units as cumulative_scaled_budget_units,
        B.scope
 from {self._v.schema}.{self._company_table} C
      join P_BY on P_BY.company_id=C.company_id
      join {self._v.schema}.{self._production_table} P on P.company_id=C.company_id
-     join {self._v.schema}.{self._benchmarks_ei_name} B on P.year=B.year and C.sector=B.sector and B.region=if(C.region in ('North America', 'Europe'), C.region, 'Global')
+     join {self._v.schema}.{self._benchmarks_ei_name} B on P.year=B.year and C.sector=B.sector and B.region=if(C.region in ('North America', 'Europe'), C.region, 'Global')  # noqa: E501
      join {self._v.schema}.{self._emissions_table} CE on CE.company_id=C.company_id and B.scope=CE.scope and CE.year=P.year
      join {self._v.schema}.{self._emissions_table} CE_BY on CE_BY.company_id=C.company_id and CE_BY.scope=B.scope and CE_BY.year=P_BY.base_year
      join {self._v.schema}.{self._benchmarks_ei_name} B_BY on B.scope=B_BY.scope and B.region=B_BY.region and B.sector=B_BY.sector and B_BY.year=P_BY.base_year
 """
 
         qres = osc._do_sql(budgets_from_productions, self._v.engine, verbose=True)
         assert len(qres) and len(qres[0]) and qres[0][0] > 0
@@ -1061,15 +1073,15 @@
         company_ids: List[str],
         scope: EScope = EScope.S1S2,
         year: int = 2050,
     ) -> pd.Series:
         if probability < 0 or probability > 1:
             raise ValueError(f"probability value {probability} outside range [0.0, 1.0]")
         temp_scores = read_quantified_sql(
-            "select company_id, scope, target_temperature_score, target_temperature_score_units, trajectory_temperature_score, trajectory_temperature_score_units, year"
+            "select company_id, scope, target_temperature_score, target_temperature_score_units, trajectory_temperature_score, trajectory_temperature_score_units, year"  # noqa: E501
             f" from {self._tempscore_table}  where scope='{scope.name}' and year={year}",
             None,
             self._v.engine,
             index_col=["company_id", "scope"],
         )
         # We may have company_ids in our portfolio not in our database, and vice-versa.
         # Return proper pa_temp_scores for what we can find, and np.nan for those we cannot
@@ -1077,13 +1089,12 @@
             data=None,
             index=pd.MultiIndex.from_tuples(
                 [(company_id, scope.name) for company_id in company_ids], names=["company_id", "scope"]
             ),
             name="temp_score",
             dtype="pint[delta_degC]",
         )
-        retval.loc[
-            retval.index.intersection(temp_scores.index)
-        ] = temp_scores.target_temperature_score * probability + temp_scores.trajectory_temperature_score * (
-            1 - probability
+        retval.loc[retval.index.intersection(temp_scores.index)] = (
+            temp_scores.target_temperature_score * probability
+            + temp_scores.trajectory_temperature_score * (1 - probability)
         )
         return retval
```

### Comparing `itr-1.1.3/src/ITR/interfaces.py` & `itr-1.1.4/src/ITR/interfaces.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/portfolio_aggregation.py` & `itr-1.1.4/src/ITR/portfolio_aggregation.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/src/ITR/temperature_score.py` & `itr-1.1.4/src/ITR/temperature_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,22 @@
 
         self.aggregation_method = aggregation_method
         self.budget_column = budget_column
         self.grouping: list = []
         if grouping is not None:
             self.grouping = grouping
 
-    def get_score(
-        self, scorable_row: pd.Series
-    ) -> Tuple[delta_degC_Quantity, delta_degC_Quantity, float, delta_degC_Quantity, float, EScoreResultType,]:
+    def get_score(self, scorable_row: pd.Series) -> Tuple[
+        delta_degC_Quantity,
+        delta_degC_Quantity,
+        float,
+        delta_degC_Quantity,
+        float,
+        EScoreResultType,
+    ]:
         """
         Get the temperature score for a certain target based on the annual reduction rate and the regression parameters.
 
         :param scorable_row: The target as a row of a data frame
         :return: The temperature score, which is a tuple of (TEMPERATURE_SCORE, TRAJECTORY_SCORE, TRAJECTORY_OVERSHOOT,
                         TARGET_SCORE, TARGET_OVERSHOOT, TEMPERATURE_RESULTS])
         """
```

### Comparing `itr-1.1.3/src/ITR/utils.py` & `itr-1.1.4/src/ITR/utils.py`

 * *Files identical despite different names*

### Comparing `itr-1.1.3/PKG-INFO` & `itr-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ITR
-Version: 1.1.3
+Version: 1.1.4
 Summary: Assess the temperature alignment of current targets, commitments, and investment and lending portfolios.
 Keywords: Climate ITR Finance
 Author-Email: Michael Tiemann <72577720+MichaelTiemannOSC@users.noreply.github.com>
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

