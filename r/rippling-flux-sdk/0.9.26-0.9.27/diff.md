# Comparing `tmp/rippling_flux_sdk-0.9.26.tar.gz` & `tmp/rippling_flux_sdk-0.9.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rippling_flux_sdk-0.9.26.tar", max compression
+gzip compressed data, was "rippling_flux_sdk-0.9.27.tar", max compression
```

## Comparing `rippling_flux_sdk-0.9.26.tar` & `rippling_flux_sdk-0.9.27.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1065 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/LICENSE
--rw-r--r--   0        0        0      793 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/README.md
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/__init__.py
--rw-r--r--   0        0        0       17 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/BUILD
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/__init__.py
--rw-r--r--   0        0        0      657 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/data_models.py
--rw-r--r--   0        0        0     1053 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/interface.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/__init__.py
--rw-r--r--   0        0        0       17 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/BUILD
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/__init__.py
--rw-r--r--   0        0        0      548 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/data_models.py
--rw-r--r--   0        0        0     1137 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/interface.py
--rw-r--r--   0        0        0       17 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/BUILD
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/__init__.py
--rw-r--r--   0        0        0     1820 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/data_models.py
--rw-r--r--   0        0        0     1115 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/interface.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.464240 rippling_flux_sdk-0.9.26/flux_sdk/flux_core/__init__.py
--rw-r--r--   0        0        0     5365 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/flux_core/data_models.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/report_payroll_contributions/__init__.py
--rw-r--r--   0        0        0     7415 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/report_payroll_contributions/data_models.py
--rw-r--r--   0        0        0     1165 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/report_payroll_contributions/interface.py
--rw-r--r--   0        0        0       17 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/update_deduction_elections/BUILD
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/update_deduction_elections/__init__.py
--rw-r--r--   0        0        0      487 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/update_deduction_elections/data_models.py
--rw-r--r--   0        0        0     1643 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/update_deduction_elections/interface.py
--rw-r--r--   0        0        0     1582 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/test_utils/contributions.csv
--rw-r--r--   0        0        0     8079 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/test_utils/test_pay_konnect.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/utils/ascensus.py
--rw-r--r--   0        0        0    22981 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/pension/utils/pay_konnect.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/user_management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/user_management/api/__init__.py
--rw-r--r--   0        0        0     1212 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/user_management/api/base_api.py
--rw-r--r--   0        0        0        0 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/user_management/data_models/__init__.py
--rw-r--r--   0        0        0      316 2023-12-18 09:21:10.468240 rippling_flux_sdk-0.9.26/flux_sdk/user_management/data_models/base_types.py
--rw-r--r--   0        0        0      536 2023-12-18 09:21:17.472261 rippling_flux_sdk-0.9.26/pyproject.toml
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 rippling_flux_sdk-0.9.26/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/LICENSE
+-rw-r--r--   0        0        0      793 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/README.md
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/__init__.py
+-rw-r--r--   0        0        0       17 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/BUILD
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/__init__.py
+-rw-r--r--   0        0        0      657 2023-12-19 16:46:44.436371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/data_models.py
+-rw-r--r--   0        0        0     1053 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/interface.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/__init__.py
+-rw-r--r--   0        0        0       17 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/BUILD
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/__init__.py
+-rw-r--r--   0        0        0      548 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/data_models.py
+-rw-r--r--   0        0        0     1137 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/interface.py
+-rw-r--r--   0        0        0       17 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/BUILD
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/__init__.py
+-rw-r--r--   0        0        0     1820 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/data_models.py
+-rw-r--r--   0        0        0     1115 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/interface.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flux_core/__init__.py
+-rw-r--r--   0        0        0     5618 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/flux_core/data_models.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/report_payroll_contributions/__init__.py
+-rw-r--r--   0        0        0     7415 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/report_payroll_contributions/data_models.py
+-rw-r--r--   0        0        0     1165 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/report_payroll_contributions/interface.py
+-rw-r--r--   0        0        0       17 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/update_deduction_elections/BUILD
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/update_deduction_elections/__init__.py
+-rw-r--r--   0        0        0      487 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/update_deduction_elections/data_models.py
+-rw-r--r--   0        0        0     1643 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/update_deduction_elections/interface.py
+-rw-r--r--   0        0        0     1582 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/test_utils/contributions.csv
+-rw-r--r--   0        0        0     8079 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/test_utils/test_pay_konnect.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/utils/ascensus.py
+-rw-r--r--   0        0        0    22981 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/pension/utils/pay_konnect.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/user_management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/user_management/api/__init__.py
+-rw-r--r--   0        0        0     1212 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/user_management/api/base_api.py
+-rw-r--r--   0        0        0        0 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/user_management/data_models/__init__.py
+-rw-r--r--   0        0        0      316 2023-12-19 16:46:44.440371 rippling_flux_sdk-0.9.27/flux_sdk/user_management/data_models/base_types.py
+-rw-r--r--   0        0        0      536 2023-12-19 16:46:50.616342 rippling_flux_sdk-0.9.27/pyproject.toml
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 rippling_flux_sdk-0.9.27/PKG-INFO
```

### Comparing `rippling_flux_sdk-0.9.26/LICENSE` & `rippling_flux_sdk-0.9.27/LICENSE`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/README.md` & `rippling_flux_sdk-0.9.27/README.md`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/data_models.py` & `rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/data_models.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/fertility/capabilities/report_eligibility_data/interface.py` & `rippling_flux_sdk-0.9.27/flux_sdk/fertility/capabilities/report_eligibility_data/interface.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/data_models.py` & `rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/data_models.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_contributions/interface.py` & `rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_contributions/interface.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/data_models.py` & `rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/data_models.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/flex/capabilities/update_enrollments/interface.py` & `rippling_flux_sdk-0.9.27/flux_sdk/flex/capabilities/update_enrollments/interface.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/flux_core/data_models.py` & `rippling_flux_sdk-0.9.27/flux_sdk/flux_core/data_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,14 +95,17 @@
     is_contractor: bool
     is_full_time: bool
     is_part_time: bool
     is_new_hire: bool
     is_rehire: bool
     is_international_employee: bool
     marital_status: Optional[MaritalStatus]
+    employement_type: Optional[str] # The employment type of the employee.
+    department: Optional[str]   # The department of the employee.
+    termination_reason: Optional[str]   # The termination reason of the employee if the employee is terminated.
 
 
 class ContributionType(Enum):
     """
     This enum is an exhaustive list of all 401k Contribution types supported by Rippling. Developers are expected
     to use this to fetch the Employee deduction contribution based on contribution type. If a contribution type your app
     requires is not present please reach out to apps@rippling.com to add support for that particular deduction.
```

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/report_payroll_contributions/data_models.py` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/report_payroll_contributions/data_models.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/report_payroll_contributions/interface.py` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/report_payroll_contributions/interface.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/capabilities/update_deduction_elections/interface.py` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/capabilities/update_deduction_elections/interface.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/test_utils/contributions.csv` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/test_utils/contributions.csv`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/test_utils/test_pay_konnect.py` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/test_utils/test_pay_konnect.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/pension/utils/pay_konnect.py` & `rippling_flux_sdk-0.9.27/flux_sdk/pension/utils/pay_konnect.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/flux_sdk/user_management/api/base_api.py` & `rippling_flux_sdk-0.9.27/flux_sdk/user_management/api/base_api.py`

 * *Files identical despite different names*

### Comparing `rippling_flux_sdk-0.9.26/pyproject.toml` & `rippling_flux_sdk-0.9.27/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rippling-flux-sdk"
-version = "0.9.26"
+version = "0.9.27"
 description = "Defines the interfaces and data-models used by Rippling Flux Apps."
 authors = ["Rippling Apps <apps@rippling.com>"]
 readme = "README.md"
 packages = [{include="flux_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rippling_flux_sdk-0.9.26/PKG-INFO` & `rippling_flux_sdk-0.9.27/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rippling-flux-sdk
-Version: 0.9.26
+Version: 0.9.27
 Summary: Defines the interfaces and data-models used by Rippling Flux Apps.
 Author: Rippling Apps
 Author-email: apps@rippling.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

