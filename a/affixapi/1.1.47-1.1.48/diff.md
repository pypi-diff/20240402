# Comparing `tmp/affixapi-1.1.47.tar.gz` & `tmp/affixapi-1.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.47.tar", last modified: Mon Apr  1 22:37:44 2024, max compression
+gzip compressed data, was "affixapi-1.1.48.tar", last modified: Mon Apr  1 22:43:15 2024, max compression
```

## Comparing `affixapi-1.1.47.tar` & `affixapi-1.1.48.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.458694 affixapi-1.1.47/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-01 22:37:36.000000 affixapi-1.1.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-01 22:37:44.458694 affixapi-1.1.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21550 2024-04-01 22:37:36.000000 affixapi-1.1.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.458694 affixapi-1.1.47/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-01 22:37:44.000000 affixapi-1.1.47/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-01 22:37:44.000000 affixapi-1.1.47/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:37:44.000000 affixapi-1.1.47/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 22:37:44.000000 affixapi-1.1.47/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 22:37:44.000000 affixapi-1.1.47/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.438694 affixapi-1.1.47/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.438694 affixapi-1.1.47/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    57193 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    57208 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.438694 affixapi-1.1.47/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.450694 affixapi-1.1.47/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17933 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/currency_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-01 22:37:36.000000 affixapi-1.1.47/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.450694 affixapi-1.1.47/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-01 22:37:37.000000 affixapi-1.1.47/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:37:44.458694 affixapi-1.1.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 22:37:37.000000 affixapi-1.1.47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:37:44.458694 affixapi-1.1.47/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_currency_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-01 22:37:37.000000 affixapi-1.1.47/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.673390 affixapi-1.1.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-01 22:43:12.000000 affixapi-1.1.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-01 22:43:15.673390 affixapi-1.1.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-04-01 22:43:12.000000 affixapi-1.1.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.673390 affixapi-1.1.48/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-01 22:43:15.000000 affixapi-1.1.48/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-01 22:43:15.000000 affixapi-1.1.48/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:43:15.000000 affixapi-1.1.48/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 22:43:15.000000 affixapi-1.1.48/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 22:43:15.000000 affixapi-1.1.48/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.653390 affixapi-1.1.48/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.653390 affixapi-1.1.48/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52498 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.653390 affixapi-1.1.48/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.665390 affixapi-1.1.48/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17933 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/currency_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.665390 affixapi-1.1.48/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-01 22:43:12.000000 affixapi-1.1.48/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:43:15.677390 affixapi-1.1.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 22:43:12.000000 affixapi-1.1.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:15.673390 affixapi-1.1.48/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_currency_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-01 22:43:12.000000 affixapi-1.1.48/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.47/LICENSE` & `affixapi-1.1.48/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/PKG-INFO` & `affixapi-1.1.48/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: affixapi
-Version: 1.1.47
-Summary: Affix API
-Home-page: 
-Author: OpenAPI Generator community
-Author-email: developers@affixapi.com
-Keywords: OpenAPI,OpenAPI-Generator,Affix API
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: urllib3>=1.25.3
-Requires-Dist: python-dateutil
-
 # openapi-client
 The affixapi.com API documentation.
 
 # Introduction
 Affix API is an OAuth 2.1 application that allows developers to access
 customer data, without developers needing to manage or maintain
 integrations; or collect login credentials or API keys from users for these
@@ -267,20 +253,17 @@
 ```python
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
-from openapi_client.model.create_employee_request import CreateEmployeeRequest
-from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
-from openapi_client.model.inline_response400 import InlineResponse400
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
 from openapi_client.model.time_off_entries20230301_response import TimeOffEntries20230301Response
 from openapi_client.model.timesheets20230301_response import Timesheets20230301Response
@@ -319,15 +302,14 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.affixapi.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *20230301Api* | [**xhr_companies20230301**](docs/20230301Api.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*20230301Api* | [**xhr_create_employee20230301**](docs/20230301Api.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *20230301Api* | [**xhr_employees20230301**](docs/20230301Api.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *20230301Api* | [**xhr_groups20230301**](docs/20230301Api.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *20230301Api* | [**xhr_identity20230301**](docs/20230301Api.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *20230301Api* | [**xhr_payruns20230301**](docs/20230301Api.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *20230301Api* | [**xhr_payslips20230301**](docs/20230301Api.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *20230301Api* | [**xhr_time_off_balances20230301**](docs/20230301Api.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *20230301Api* | [**xhr_time_off_entries20230301**](docs/20230301Api.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
@@ -337,15 +319,14 @@
 *ManagementApi* | [**client**](docs/ManagementApi.md#client) | **GET** /2023-03-01/management/client | Client
 *ManagementApi* | [**disconnect**](docs/ManagementApi.md#disconnect) | **POST** /2023-03-01/management/disconnect | Disconnect token
 *ManagementApi* | [**introspect**](docs/ManagementApi.md#introspect) | **GET** /2023-03-01/management/introspect | Inspect token
 *ManagementApi* | [**token**](docs/ManagementApi.md#token) | **POST** /2023-03-01/management/token | Create token
 *ManagementApi* | [**tokens**](docs/ManagementApi.md#tokens) | **GET** /2023-03-01/management/tokens | Tokens
 *ManagementApi* | [**update_client**](docs/ManagementApi.md#update_client) | **POST** /2023-03-01/management/client | Update client
 *XHRVerticallyIntegratedApi* | [**xhr_companies20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*XHRVerticallyIntegratedApi* | [**xhr_create_employee20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *XHRVerticallyIntegratedApi* | [**xhr_employees20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *XHRVerticallyIntegratedApi* | [**xhr_groups20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *XHRVerticallyIntegratedApi* | [**xhr_identity20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *XHRVerticallyIntegratedApi* | [**xhr_payruns20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *XHRVerticallyIntegratedApi* | [**xhr_payslips20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_balances20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_entries20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
```

### Comparing `affixapi-1.1.47/README.md` & `affixapi-1.1.48/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: affixapi
+Version: 1.1.48
+Summary: Affix API
+Home-page: 
+Author: OpenAPI Generator community
+Author-email: developers@affixapi.com
+Keywords: OpenAPI,OpenAPI-Generator,Affix API
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: urllib3>=1.25.3
+Requires-Dist: python-dateutil
+
 # openapi-client
 The affixapi.com API documentation.
 
 # Introduction
 Affix API is an OAuth 2.1 application that allows developers to access
 customer data, without developers needing to manage or maintain
 integrations; or collect login credentials or API keys from users for these
@@ -253,20 +267,17 @@
 ```python
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
-from openapi_client.model.create_employee_request import CreateEmployeeRequest
-from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
-from openapi_client.model.inline_response400 import InlineResponse400
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
 from openapi_client.model.time_off_entries20230301_response import TimeOffEntries20230301Response
 from openapi_client.model.timesheets20230301_response import Timesheets20230301Response
@@ -305,15 +316,14 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.affixapi.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *20230301Api* | [**xhr_companies20230301**](docs/20230301Api.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*20230301Api* | [**xhr_create_employee20230301**](docs/20230301Api.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *20230301Api* | [**xhr_employees20230301**](docs/20230301Api.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *20230301Api* | [**xhr_groups20230301**](docs/20230301Api.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *20230301Api* | [**xhr_identity20230301**](docs/20230301Api.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *20230301Api* | [**xhr_payruns20230301**](docs/20230301Api.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *20230301Api* | [**xhr_payslips20230301**](docs/20230301Api.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *20230301Api* | [**xhr_time_off_balances20230301**](docs/20230301Api.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *20230301Api* | [**xhr_time_off_entries20230301**](docs/20230301Api.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
@@ -323,15 +333,14 @@
 *ManagementApi* | [**client**](docs/ManagementApi.md#client) | **GET** /2023-03-01/management/client | Client
 *ManagementApi* | [**disconnect**](docs/ManagementApi.md#disconnect) | **POST** /2023-03-01/management/disconnect | Disconnect token
 *ManagementApi* | [**introspect**](docs/ManagementApi.md#introspect) | **GET** /2023-03-01/management/introspect | Inspect token
 *ManagementApi* | [**token**](docs/ManagementApi.md#token) | **POST** /2023-03-01/management/token | Create token
 *ManagementApi* | [**tokens**](docs/ManagementApi.md#tokens) | **GET** /2023-03-01/management/tokens | Tokens
 *ManagementApi* | [**update_client**](docs/ManagementApi.md#update_client) | **POST** /2023-03-01/management/client | Update client
 *XHRVerticallyIntegratedApi* | [**xhr_companies20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*XHRVerticallyIntegratedApi* | [**xhr_create_employee20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *XHRVerticallyIntegratedApi* | [**xhr_employees20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *XHRVerticallyIntegratedApi* | [**xhr_groups20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *XHRVerticallyIntegratedApi* | [**xhr_identity20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *XHRVerticallyIntegratedApi* | [**xhr_payruns20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *XHRVerticallyIntegratedApi* | [**xhr_payslips20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_balances20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_entries20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
```

### Comparing `affixapi-1.1.47/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.48/affixapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.47
+Version: 1.1.48
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -267,20 +267,17 @@
 ```python
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
-from openapi_client.model.create_employee_request import CreateEmployeeRequest
-from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
-from openapi_client.model.inline_response400 import InlineResponse400
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
 from openapi_client.model.time_off_entries20230301_response import TimeOffEntries20230301Response
 from openapi_client.model.timesheets20230301_response import Timesheets20230301Response
@@ -319,15 +316,14 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.affixapi.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *20230301Api* | [**xhr_companies20230301**](docs/20230301Api.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*20230301Api* | [**xhr_create_employee20230301**](docs/20230301Api.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *20230301Api* | [**xhr_employees20230301**](docs/20230301Api.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *20230301Api* | [**xhr_groups20230301**](docs/20230301Api.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *20230301Api* | [**xhr_identity20230301**](docs/20230301Api.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *20230301Api* | [**xhr_payruns20230301**](docs/20230301Api.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *20230301Api* | [**xhr_payslips20230301**](docs/20230301Api.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *20230301Api* | [**xhr_time_off_balances20230301**](docs/20230301Api.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *20230301Api* | [**xhr_time_off_entries20230301**](docs/20230301Api.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
@@ -337,15 +333,14 @@
 *ManagementApi* | [**client**](docs/ManagementApi.md#client) | **GET** /2023-03-01/management/client | Client
 *ManagementApi* | [**disconnect**](docs/ManagementApi.md#disconnect) | **POST** /2023-03-01/management/disconnect | Disconnect token
 *ManagementApi* | [**introspect**](docs/ManagementApi.md#introspect) | **GET** /2023-03-01/management/introspect | Inspect token
 *ManagementApi* | [**token**](docs/ManagementApi.md#token) | **POST** /2023-03-01/management/token | Create token
 *ManagementApi* | [**tokens**](docs/ManagementApi.md#tokens) | **GET** /2023-03-01/management/tokens | Tokens
 *ManagementApi* | [**update_client**](docs/ManagementApi.md#update_client) | **POST** /2023-03-01/management/client | Update client
 *XHRVerticallyIntegratedApi* | [**xhr_companies20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_companies20230301) | **GET** /2023-03-01/xhr/company | Company
-*XHRVerticallyIntegratedApi* | [**xhr_create_employee20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_create_employee20230301) | **POST** /2023-03-01/xhr/employee | Create employee
 *XHRVerticallyIntegratedApi* | [**xhr_employees20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_employees20230301) | **GET** /2023-03-01/xhr/employees | Employees
 *XHRVerticallyIntegratedApi* | [**xhr_groups20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_groups20230301) | **GET** /2023-03-01/xhr/groups | Groups
 *XHRVerticallyIntegratedApi* | [**xhr_identity20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_identity20230301) | **GET** /2023-03-01/xhr/identity | Identity
 *XHRVerticallyIntegratedApi* | [**xhr_payruns20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payruns20230301) | **GET** /2023-03-01/xhr/payruns | Payruns
 *XHRVerticallyIntegratedApi* | [**xhr_payslips20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_payslips20230301) | **GET** /2023-03-01/xhr/payruns/{payrun_id} | Payslips
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_balances20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_balances20230301) | **GET** /2023-03-01/xhr/time-off-balances | Time off balances
 *XHRVerticallyIntegratedApi* | [**xhr_time_off_entries20230301**](docs/XHRVerticallyIntegratedApi.md#xhr_time_off_entries20230301) | **GET** /2023-03-01/xhr/time-off-entries | Time off entries
```

### Comparing `affixapi-1.1.47/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.48/affixapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/__init__.py` & `affixapi-1.1.48/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.48/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,28 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
-from openapi_client.model.create_employee_request import CreateEmployeeRequest
-from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
-from openapi_client.model.inline_response400 import InlineResponse400
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
 from openapi_client.model.time_off_entries20230301_response import TimeOffEntries20230301Response
 from openapi_client.model.timesheets20230301_response import Timesheets20230301Response
 from openapi_client.model.work_locations20230301_response import WorkLocations20230301Response
 
 
-class 20230301Api(object):
+class XHRVerticallyIntegratedApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
@@ -154,134 +151,14 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__xhr_companies20230301
         )
 
-        def __xhr_create_employee20230301(
-            self,
-            create_employee_request,
-            **kwargs
-        ):
-            """Create employee  # noqa: E501
-
-            Creates a new Employee   # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.xhr_create_employee20230301(create_employee_request, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                create_employee_request (CreateEmployeeRequest):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (float/tuple): timeout setting for this request. If one
-                    number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                EmployeeResponse
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['create_employee_request'] = \
-                create_employee_request
-            return self.call_with_http_info(**kwargs)
-
-        self.xhr_create_employee20230301 = _Endpoint(
-            settings={
-                'response_type': (EmployeeResponse,),
-                'auth': [
-                    'access-token'
-                ],
-                'endpoint_path': '/2023-03-01/xhr/employee',
-                'operation_id': 'xhr_create_employee20230301',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_employee_request',
-                ],
-                'required': [
-                    'create_employee_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_employee_request':
-                        (CreateEmployeeRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'create_employee_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client,
-            callable=__xhr_create_employee20230301
-        )
-
         def __xhr_employees20230301(
             self,
             **kwargs
         ):
             """Employees  # noqa: E501
 
             List the individuals (employees, contractors, accountants, and others) listed in the HRIS/Payroll software   # noqa: E501
```

### Comparing `affixapi-1.1.47/openapi_client/api/core_api.py` & `affixapi-1.1.48/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/api/management_api.py` & `affixapi-1.1.48/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.48/openapi_client/api/2023_03_01_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,28 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
-from openapi_client.model.create_employee_request import CreateEmployeeRequest
-from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
-from openapi_client.model.inline_response400 import InlineResponse400
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
 from openapi_client.model.time_off_entries20230301_response import TimeOffEntries20230301Response
 from openapi_client.model.timesheets20230301_response import Timesheets20230301Response
 from openapi_client.model.work_locations20230301_response import WorkLocations20230301Response
 
 
-class XHRVerticallyIntegratedApi(object):
+class 20230301Api(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
@@ -154,134 +151,14 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__xhr_companies20230301
         )
 
-        def __xhr_create_employee20230301(
-            self,
-            create_employee_request,
-            **kwargs
-        ):
-            """Create employee  # noqa: E501
-
-            Creates a new Employee   # noqa: E501
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.xhr_create_employee20230301(create_employee_request, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                create_employee_request (CreateEmployeeRequest):
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (float/tuple): timeout setting for this request. If one
-                    number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                EmployeeResponse
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['create_employee_request'] = \
-                create_employee_request
-            return self.call_with_http_info(**kwargs)
-
-        self.xhr_create_employee20230301 = _Endpoint(
-            settings={
-                'response_type': (EmployeeResponse,),
-                'auth': [
-                    'access-token'
-                ],
-                'endpoint_path': '/2023-03-01/xhr/employee',
-                'operation_id': 'xhr_create_employee20230301',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_employee_request',
-                ],
-                'required': [
-                    'create_employee_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_employee_request':
-                        (CreateEmployeeRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'create_employee_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client,
-            callable=__xhr_create_employee20230301
-        )
-
         def __xhr_employees20230301(
             self,
             **kwargs
         ):
             """Employees  # noqa: E501
 
             List the individuals (employees, contractors, accountants, and others) listed in the HRIS/Payroll software   # noqa: E501
```

### Comparing `affixapi-1.1.47/openapi_client/api_client.py` & `affixapi-1.1.48/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/apis/__init__.py` & `affixapi-1.1.48/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/configuration.py` & `affixapi-1.1.48/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/exceptions.py` & `affixapi-1.1.48/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.48/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/address_response.py` & `affixapi-1.1.48/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/client_request.py` & `affixapi-1.1.48/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/client_response.py` & `affixapi-1.1.48/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.48/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/company_response.py` & `affixapi-1.1.48/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/create_employee_request.py` & `affixapi-1.1.48/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.48/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.48/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/currency_request.py` & `affixapi-1.1.48/openapi_client/model/currency_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/currency_response.py` & `affixapi-1.1.48/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/disconnect_response.py` & `affixapi-1.1.48/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/employee_response.py` & `affixapi-1.1.48/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.48/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.48/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/employment_response.py` & `affixapi-1.1.48/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.48/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/group_response.py` & `affixapi-1.1.48/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.48/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.48/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.48/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/identity_response.py` & `affixapi-1.1.48/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/inline_response400.py` & `affixapi-1.1.48/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/inline_response401.py` & `affixapi-1.1.48/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/inline_response409.py` & `affixapi-1.1.48/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/introspect_response.py` & `affixapi-1.1.48/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.48/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/location_response.py` & `affixapi-1.1.48/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/message_response.py` & `affixapi-1.1.48/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/mode_request.py` & `affixapi-1.1.48/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/mode_response.py` & `affixapi-1.1.48/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payrun_response.py` & `affixapi-1.1.48/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.48/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslip_response.py` & `affixapi-1.1.48/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.48/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.48/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.48/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.48/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.48/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/provider_request.py` & `affixapi-1.1.48/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/provider_response.py` & `affixapi-1.1.48/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/providers_response.py` & `affixapi-1.1.48/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/scopes_request.py` & `affixapi-1.1.48/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/scopes_response.py` & `affixapi-1.1.48/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.48/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.48/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.48/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.48/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/timesheet_response.py` & `affixapi-1.1.48/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.48/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/token_request.py` & `affixapi-1.1.48/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/token_response.py` & `affixapi-1.1.48/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/tokens_response.py` & `affixapi-1.1.48/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.48/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/model_utils.py` & `affixapi-1.1.48/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/models/__init__.py` & `affixapi-1.1.48/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/openapi_client/rest.py` & `affixapi-1.1.48/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/setup.py` & `affixapi-1.1.48/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.47"
+VERSION = "1.1.48"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.47/test/test_2023_03_01_api.py` & `affixapi-1.1.48/test/test_2023_03_01_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,14 @@
     def test_xhr_companies20230301(self):
         """Test case for xhr_companies20230301
 
         Company  # noqa: E501
         """
         pass
 
-    def test_xhr_create_employee20230301(self):
-        """Test case for xhr_create_employee20230301
-
-        Create employee  # noqa: E501
-        """
-        pass
-
     def test_xhr_employees20230301(self):
         """Test case for xhr_employees20230301
 
         Employees  # noqa: E501
         """
         pass
```

### Comparing `affixapi-1.1.47/test/test_address_no_non_null_request.py` & `affixapi-1.1.48/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_address_response.py` & `affixapi-1.1.48/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_client_request.py` & `affixapi-1.1.48/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_client_response.py` & `affixapi-1.1.48/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_companies20230301_response.py` & `affixapi-1.1.48/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_company_response.py` & `affixapi-1.1.48/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_core_api.py` & `affixapi-1.1.48/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_create_employee_request.py` & `affixapi-1.1.48/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.48/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_create_employee_request_manager.py` & `affixapi-1.1.48/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_currency_request.py` & `affixapi-1.1.48/test/test_currency_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_currency_response.py` & `affixapi-1.1.48/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_disconnect_response.py` & `affixapi-1.1.48/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_employee_response.py` & `affixapi-1.1.48/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_employees20230301_response.py` & `affixapi-1.1.48/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.48/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_employment_response.py` & `affixapi-1.1.48/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_group_no_null_enum_request.py` & `affixapi-1.1.48/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_group_response.py` & `affixapi-1.1.48/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_groups20230301_response.py` & `affixapi-1.1.48/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.48/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_id_and_message_response.py` & `affixapi-1.1.48/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_identity_response.py` & `affixapi-1.1.48/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_inline_response400.py` & `affixapi-1.1.48/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_inline_response401.py` & `affixapi-1.1.48/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_inline_response409.py` & `affixapi-1.1.48/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_introspect_response.py` & `affixapi-1.1.48/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_location_no_non_null_request.py` & `affixapi-1.1.48/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_location_response.py` & `affixapi-1.1.48/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_management_api.py` & `affixapi-1.1.48/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_message_response.py` & `affixapi-1.1.48/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_mode_request.py` & `affixapi-1.1.48/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_mode_response.py` & `affixapi-1.1.48/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payrun_response.py` & `affixapi-1.1.48/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payruns20230301_response.py` & `affixapi-1.1.48/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslip_response.py` & `affixapi-1.1.48/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslip_response_contributions.py` & `affixapi-1.1.48/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslip_response_deductions.py` & `affixapi-1.1.48/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslip_response_earnings.py` & `affixapi-1.1.48/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslip_response_taxes.py` & `affixapi-1.1.48/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_payslips20230301_response.py` & `affixapi-1.1.48/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_provider_request.py` & `affixapi-1.1.48/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_provider_response.py` & `affixapi-1.1.48/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_providers_response.py` & `affixapi-1.1.48/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_scopes_request.py` & `affixapi-1.1.48/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_scopes_response.py` & `affixapi-1.1.48/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_time_off_balance_response.py` & `affixapi-1.1.48/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.48/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.48/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_time_off_entry_response.py` & `affixapi-1.1.48/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_timesheet_response.py` & `affixapi-1.1.48/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_timesheets20230301_response.py` & `affixapi-1.1.48/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_token_request.py` & `affixapi-1.1.48/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_token_response.py` & `affixapi-1.1.48/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_tokens_response.py` & `affixapi-1.1.48/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_work_locations20230301_response.py` & `affixapi-1.1.48/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.47/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.48/test/test_xhr__vertically_integrated_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,21 +27,14 @@
     def test_xhr_companies20230301(self):
         """Test case for xhr_companies20230301
 
         Company  # noqa: E501
         """
         pass
 
-    def test_xhr_create_employee20230301(self):
-        """Test case for xhr_create_employee20230301
-
-        Create employee  # noqa: E501
-        """
-        pass
-
     def test_xhr_employees20230301(self):
         """Test case for xhr_employees20230301
 
         Employees  # noqa: E501
         """
         pass
```

