# Comparing `tmp/climate_finance-0.1.29.tar.gz` & `tmp/climate_finance-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_finance-0.1.29.tar", max compression
+gzip compressed data, was "climate_finance-1.0.0.tar", max compression
```

## Comparing `climate_finance-0.1.29.tar` & `climate_finance-1.0.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1069 2024-04-02 16:32:14.257682 climate_finance-0.1.29/LICENSE
--rw-r--r--   0        0        0     1557 2024-04-02 16:32:14.257682 climate_finance-0.1.29/README.md
--rw-r--r--   0        0        0       11 2024-04-02 16:32:14.257682 climate_finance-0.1.29/climate_finance/.raw_data/README.md
--rw-r--r--   0        0        0       26 2024-04-02 16:32:14.257682 climate_finance-0.1.29/climate_finance/.raw_data/data_updates.json
--rw-r--r--   0        0        0       66 2024-04-02 16:32:14.257682 climate_finance-0.1.29/climate_finance/.raw_data/imputed_missing.csv
--rw-r--r--   0        0        0    16080 2024-04-02 16:32:14.257682 climate_finance-0.1.29/climate_finance/README.md
--rw-r--r--   0        0        0      500 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/common/__init__.py
--rw-r--r--   0        0        0     7222 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/common/analysis_tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/common/cleaning_tools.py
--rw-r--r--   0        0        0     9505 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/common/schema.py
--rw-r--r--   0        0        0     1128 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/config.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/__init__.py
--rw-r--r--   0        0        0    25778 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/data.py
--rw-r--r--   0        0        0     3817 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/deflators.py
--rw-r--r--   0        0        0     4466 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/dtypes.py
--rw-r--r--   0        0        0     3081 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/enums.py
--rw-r--r--   0        0        0     3366 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/loaders.py
--rw-r--r--   0        0        0    12444 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/tools.py
--rw-r--r--   0        0        0     2582 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/core/validation.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/bilateral/__init__.py
--rw-r--r--   0        0        0    10180 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/bilateral/bilateral_methodologies.py
--rw-r--r--   0        0        0     4589 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/bilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/__init__.py
--rw-r--r--   0        0        0    19795 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/crs_tools.py
--rw-r--r--   0        0        0    10482 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/multilateral_spending_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
--rw-r--r--   0        0        0     2606 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
--rw-r--r--   0        0        0     5781 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
--rw-r--r--   0        0        0     1037 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
--rw-r--r--   0        0        0      308 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/shares.py
--rw-r--r--   0        0        0     9869 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/multilateral/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/spending/__init__.py
--rw-r--r--   0        0        0     8157 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/spending/crdf.py
--rw-r--r--   0        0        0    13352 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/spending/crdf_crs.py
--rw-r--r--   0        0        0     5679 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/spending/crs.py
--rw-r--r--   0        0        0     6329 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/methodologies/spending/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/oecd/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/__init__.py
--rw-r--r--   0        0        0    19065 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
--rw-r--r--   0        0        0     7484 2024-04-02 16:32:14.261682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/names.py
--rw-r--r--   0        0        0    23354 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
--rw-r--r--   0        0        0     5570 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/provider_names.feather
--rw-r--r--   0        0        0     5370 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/recipient_names.feather
--rw-r--r--   0        0        0     1436 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/settings.py
--rw-r--r--   0        0        0    14959 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crdf/__init__.py
--rw-r--r--   0        0        0     4144 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crdf/provider_perspective.py
--rw-r--r--   0        0        0     4144 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crdf/recipient_perspective.py
--rw-r--r--   0        0        0     3579 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crdf/tools.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crs/__init__.py
--rw-r--r--   0        0        0    13300 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crs/add_crs_data.py
--rw-r--r--   0        0        0     9598 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/crs/get_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/multisystem/__init__.py
--rw-r--r--   0        0        0     4492 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/multisystem/crs_channel_mapping.csv
--rw-r--r--   0        0        0     2709 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/oecd/multisystem/get_data.py
--rw-r--r--   0        0        0    22597 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/README.md
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     7981 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/tools.py
--rw-r--r--   0        0        0     3705 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
--rw-r--r--   0        0        0     3439 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/validation.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/download/__init__.py
--rw-r--r--   0        0        0    17281 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/download/download_data.py
--rw-r--r--   0        0        0     9534 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/download/get_data.py
--rw-r--r--   0        0        0     3413 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/download/pre_process.py
--rw-r--r--   0        0        0     6309 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/get_unfccc_data.py
--rw-r--r--   0        0        0        0 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/manual/__init__.py
--rw-r--r--   0        0        0     2966 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/manual/get_data.py
--rw-r--r--   0        0        0    11767 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/manual/pre_process.py
--rw-r--r--   0        0        0     1164 2024-04-02 16:32:14.265682 climate_finance-0.1.29/climate_finance/unfccc/manual/read_files.py
--rw-r--r--   0        0        0      665 2024-04-02 16:32:14.269682 climate_finance-0.1.29/pyproject.toml
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 climate_finance-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-02 16:35:59.590178 climate_finance-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1557 2024-04-02 16:35:59.590178 climate_finance-1.0.0/README.md
+-rw-r--r--   0        0        0       11 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/README.md
+-rw-r--r--   0        0        0       26 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/data_updates.json
+-rw-r--r--   0        0        0       66 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/.raw_data/imputed_missing.csv
+-rw-r--r--   0        0        0    16080 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/README.md
+-rw-r--r--   0        0        0      499 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/__init__.py
+-rw-r--r--   0        0        0     7222 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/analysis_tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/cleaning_tools.py
+-rw-r--r--   0        0        0     9505 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/common/schema.py
+-rw-r--r--   0        0        0     1128 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/config.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/__init__.py
+-rw-r--r--   0        0        0    25778 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/data.py
+-rw-r--r--   0        0        0     3817 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/deflators.py
+-rw-r--r--   0        0        0     4466 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/dtypes.py
+-rw-r--r--   0        0        0     3081 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/enums.py
+-rw-r--r--   0        0        0     3366 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/loaders.py
+-rw-r--r--   0        0        0    12444 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/tools.py
+-rw-r--r--   0        0        0     2582 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/core/validation.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/__init__.py
+-rw-r--r--   0        0        0    10180 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py
+-rw-r--r--   0        0        0     4589 2024-04-02 16:35:59.590178 climate_finance-1.0.0/climate_finance/methodologies/bilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/__init__.py
+-rw-r--r--   0        0        0    19795 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/crs_tools.py
+-rw-r--r--   0        0        0    10482 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py
+-rw-r--r--   0        0        0     2606 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/__init__.py
+-rw-r--r--   0        0        0     5781 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py
+-rw-r--r--   0        0        0     1037 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py
+-rw-r--r--   0        0        0      308 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/shares.py
+-rw-r--r--   0        0        0     9869 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/multilateral/tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/__init__.py
+-rw-r--r--   0        0        0     8157 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crdf.py
+-rw-r--r--   0        0        0    13352 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crdf_crs.py
+-rw-r--r--   0        0        0     5679 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/crs.py
+-rw-r--r--   0        0        0     6329 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/methodologies/spending/tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0    19065 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     7484 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/names.py
+-rw-r--r--   0        0        0    23354 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather
+-rw-r--r--   0        0        0     5570 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_names.feather
+-rw-r--r--   0        0        0     5370 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/recipient_names.feather
+-rw-r--r--   0        0        0     1436 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/settings.py
+-rw-r--r--   0        0        0    14959 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/__init__.py
+-rw-r--r--   0        0        0     4144 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/provider_perspective.py
+-rw-r--r--   0        0        0     4144 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/recipient_perspective.py
+-rw-r--r--   0        0        0     3579 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crdf/tools.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/__init__.py
+-rw-r--r--   0        0        0    13300 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/add_crs_data.py
+-rw-r--r--   0        0        0     9598 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/crs/get_data.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/__init__.py
+-rw-r--r--   0        0        0     4492 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     2709 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/oecd/multisystem/get_data.py
+-rw-r--r--   0        0        0    22597 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     7981 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/tools.py
+-rw-r--r--   0        0        0     3705 2024-04-02 16:35:59.594178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json
+-rw-r--r--   0        0        0     3439 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/validation.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/__init__.py
+-rw-r--r--   0        0        0    17281 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/download_data.py
+-rw-r--r--   0        0        0     9534 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/get_data.py
+-rw-r--r--   0        0        0     3413 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/download/pre_process.py
+-rw-r--r--   0        0        0     6309 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/get_unfccc_data.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/__init__.py
+-rw-r--r--   0        0        0     2966 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/get_data.py
+-rw-r--r--   0        0        0    11767 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/pre_process.py
+-rw-r--r--   0        0        0     1164 2024-04-02 16:35:59.598178 climate_finance-1.0.0/climate_finance/unfccc/manual/read_files.py
+-rw-r--r--   0        0        0      664 2024-04-02 16:35:59.598178 climate_finance-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 climate_finance-1.0.0/PKG-INFO
```

### Comparing `climate_finance-0.1.29/LICENSE` & `climate_finance-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/README.md` & `climate_finance-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/README.md` & `climate_finance-1.0.0/climate_finance/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/common/analysis_tools.py` & `climate_finance-1.0.0/climate_finance/common/analysis_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/common/schema.py` & `climate_finance-1.0.0/climate_finance/common/schema.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/config.py` & `climate_finance-1.0.0/climate_finance/config.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/data.py` & `climate_finance-1.0.0/climate_finance/core/data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/deflators.py` & `climate_finance-1.0.0/climate_finance/core/deflators.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/dtypes.py` & `climate_finance-1.0.0/climate_finance/core/dtypes.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/enums.py` & `climate_finance-1.0.0/climate_finance/core/enums.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/loaders.py` & `climate_finance-1.0.0/climate_finance/core/loaders.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/tools.py` & `climate_finance-1.0.0/climate_finance/core/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/core/validation.py` & `climate_finance-1.0.0/climate_finance/core/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/bilateral/bilateral_methodologies.py` & `climate_finance-1.0.0/climate_finance/methodologies/bilateral/bilateral_methodologies.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/bilateral/tools.py` & `climate_finance-1.0.0/climate_finance/methodologies/bilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/crs_tools.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/crs_tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/multilateral_spending_data.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/multilateral_spending_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/get_oecd_imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/oecd_multilateral/shares.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/climate_components.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/one_multilateral/imputations.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/one_multilateral/imputations.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/multilateral/tools.py` & `climate_finance-1.0.0/climate_finance/methodologies/multilateral/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/spending/crdf.py` & `climate_finance-1.0.0/climate_finance/methodologies/spending/crdf.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/spending/crdf_crs.py` & `climate_finance-1.0.0/climate_finance/methodologies/spending/crdf_crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/spending/crs.py` & `climate_finance-1.0.0/climate_finance/methodologies/spending/crs.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/methodologies/spending/tools.py` & `climate_finance-1.0.0/climate_finance/methodologies/spending/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/names.py` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/names.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/provider_agency_names.feather` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_agency_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/provider_names.feather` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/provider_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/recipient_names.feather` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/recipient_names.feather`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/settings.py` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/settings.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/cleaning_tools/tools.py` & `climate_finance-1.0.0/climate_finance/oecd/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/crdf/provider_perspective.py` & `climate_finance-1.0.0/climate_finance/oecd/crdf/provider_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/crdf/recipient_perspective.py` & `climate_finance-1.0.0/climate_finance/oecd/crdf/recipient_perspective.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/crdf/tools.py` & `climate_finance-1.0.0/climate_finance/oecd/crdf/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/crs/add_crs_data.py` & `climate_finance-1.0.0/climate_finance/oecd/crs/add_crs_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/crs/get_data.py` & `climate_finance-1.0.0/climate_finance/oecd/crs/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/multisystem/crs_channel_mapping.csv` & `climate_finance-1.0.0/climate_finance/oecd/multisystem/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/oecd/multisystem/get_data.py` & `climate_finance-1.0.0/climate_finance/oecd/multisystem/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/README.md` & `climate_finance-1.0.0/climate_finance/unfccc/README.md`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/tools.py` & `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/tools.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json` & `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/unfccc_channel_mapping.json`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/cleaning_tools/validation.py` & `climate_finance-1.0.0/climate_finance/unfccc/cleaning_tools/validation.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/download/download_data.py` & `climate_finance-1.0.0/climate_finance/unfccc/download/download_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/download/get_data.py` & `climate_finance-1.0.0/climate_finance/unfccc/download/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/download/pre_process.py` & `climate_finance-1.0.0/climate_finance/unfccc/download/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/get_unfccc_data.py` & `climate_finance-1.0.0/climate_finance/unfccc/get_unfccc_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/manual/get_data.py` & `climate_finance-1.0.0/climate_finance/unfccc/manual/get_data.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/manual/pre_process.py` & `climate_finance-1.0.0/climate_finance/unfccc/manual/pre_process.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/climate_finance/unfccc/manual/read_files.py` & `climate_finance-1.0.0/climate_finance/unfccc/manual/read_files.py`

 * *Files identical despite different names*

### Comparing `climate_finance-0.1.29/pyproject.toml` & `climate_finance-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "climate-finance"
-version = "0.1.29"
+version = "1.0.0"
 description = "Climate Finance data"
 authors = ["Jorge Rivera, The ONE Campaign"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "climate_finance"}]
 
 [tool.poetry.dependencies]
```

### Comparing `climate_finance-0.1.29/PKG-INFO` & `climate_finance-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate-finance
-Version: 0.1.29
+Version: 1.0.0
 Summary: Climate Finance data
 License: MIT
 Author: Jorge Rivera, The ONE Campaign
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

