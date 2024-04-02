# Comparing `tmp/candidhealth-0.8.0.tar.gz` & `tmp/candidhealth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.8.0.tar", max compression
+gzip compressed data, was "candidhealth-0.9.0.tar", max compression
```

## Comparing `candidhealth-0.8.0.tar` & `candidhealth-0.9.0.tar`

### file list

```diff
@@ -1,371 +1,393 @@
--rw-r--r--   0        0        0      257 2023-10-30 17:13:09.785293 candidhealth-0.8.0/README.md
--rw-r--r--   0        0        0      393 2023-10-30 17:13:09.785293 candidhealth-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6865 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/__init__.py
--rw-r--r--   0        0        0     2650 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/candid_api_client.py
--rw-r--r--   0        0        0     5783 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/client.py
--rw-r--r--   0        0        0      519 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1620 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-10-30 17:13:09.785293 candidhealth-0.8.0/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      227 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/py.typed
--rw-r--r--   0        0        0     6965 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/__init__.py
--rw-r--r--   0        0        0      593 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/__init__.py
--rw-r--r--   0        0        0      304 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/__init__.py
--rw-r--r--   0        0        0     5343 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/client.py
--rw-r--r--   0        0        0      159 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      333 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      940 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
--rw-r--r--   0        0        0      882 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
--rw-r--r--   0        0        0      792 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0      609 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/__init__.py
--rw-r--r--   0        0        0      191 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/__init__.py
--rw-r--r--   0        0        0     2710 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/client.py
--rw-r--r--   0        0        0      256 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1370 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note.py
--rw-r--r--   0        0        0      838 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/__init__.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/__init__.py
--rw-r--r--   0        0        0      269 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/__init__.py
--rw-r--r--   0        0        0      377 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0      827 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/claim_frequency_type_code.py
--rw-r--r--   0        0        0     1230 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/claim_submission_record_create.py
--rw-r--r--   0        0        0     1369 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/external_claim_submission_create.py
--rw-r--r--   0        0        0      139 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1192 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     2609 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0      745 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      333 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/entity_not_found_error.py
--rw-r--r--   0        0        0      326 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/http_request_validation_error.py
--rw-r--r--   0        0        0      355 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/http_request_validations_error.py
--rw-r--r--   0        0        0      365 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/http_service_unavailable_error.py
--rw-r--r--   0        0        0      323 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      470 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/errors/updates_disabled_due_to_external_system_integration_error.py
--rw-r--r--   0        0        0     3265 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1400 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/claim_adjustment_group_codes.py
--rw-r--r--   0        0        0       98 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0      558 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/claim_submission_payer_responsibility_type.py
--rw-r--r--   0        0        0       76 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0      849 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/date_range_optional_end.py
--rw-r--r--   0        0        0       79 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/decimal.py
--rw-r--r--   0        0        0       77 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/email.py
--rw-r--r--   0        0        0      485 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/emr_payer_crosswalk.py
--rw-r--r--   0        0        0       91 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0      787 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/entity_not_found_error_message.py
--rw-r--r--   0        0        0       84 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/error_message.py
--rw-r--r--   0        0        0    13536 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0      817 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/http_service_unavailable_error_message.py
--rw-r--r--   0        0        0    15447 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0      100 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/invoice_id.py
--rw-r--r--   0        0        0       79 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     5534 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0      849 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      620 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/phone_number_type.py
--rw-r--r--   0        0        0    80253 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      101 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/provider_id.py
--rw-r--r--   0        0        0      763 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/removable_date_range_optional_end.py
--rw-r--r--   0        0        0      969 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/request_validation_error.py
--rw-r--r--   0        0        0      891 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     7036 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1060 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0     1008 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1026 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0      807 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/unauthorized_error_message.py
--rw-r--r--   0        0        0      840 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/updates_disabled_due_to_external_system_integration_error_message.py
--rw-r--r--   0        0        0       83 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/commons/types/work_queue_id.py
--rw-r--r--   0        0        0      121 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      127 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      101 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      279 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      985 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1927 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      930 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/eligibility/__init__.py
--rw-r--r--   0        0        0      607 2023-10-30 17:13:09.789294 candidhealth-0.8.0/src/candid/resources/eligibility/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/eligibility/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/eligibility/resources/v_2/__init__.py
--rw-r--r--   0        0        0     7297 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/eligibility/resources/v_2/client.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     2015 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1119 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1287 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1271 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1271 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      605 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     1896 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/__init__.py
--rw-r--r--   0        0        0    67469 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/client.py
--rw-r--r--   0        0        0      422 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
--rw-r--r--   0        0        0      327 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/errors/cash_pay_payer_error.py
--rw-r--r--   0        0        0      387 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
--rw-r--r--   0        0        0      416 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/errors/encounter_guarantor_missing_contact_info_error.py
--rw-r--r--   0        0        0     2543 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0      518 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/billable_status_type.py
--rw-r--r--   0        0        0      792 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/cash_pay_payer_error_message.py
--rw-r--r--   0        0        0      901 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
--rw-r--r--   0        0        0      971 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
--rw-r--r--   0        0        0      921 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      790 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
--rw-r--r--   0        0        0     7478 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
--rw-r--r--   0        0        0     5239 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
--rw-r--r--   0        0        0      916 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
--rw-r--r--   0        0        0      833 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py
--rw-r--r--   0        0        0      850 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_owner_of_next_action_type.py
--rw-r--r--   0        0        0      912 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
--rw-r--r--   0        0        0      889 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      996 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
--rw-r--r--   0        0        0      918 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1324 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
--rw-r--r--   0        0        0      865 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
--rw-r--r--   0        0        0      882 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/lab.py
--rw-r--r--   0        0        0      457 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
--rw-r--r--   0        0        0      980 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/medication.py
--rw-r--r--   0        0        0     2615 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
--rw-r--r--   0        0        0     1035 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
--rw-r--r--   0        0        0      710 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/responsible_party_type.py
--rw-r--r--   0        0        0       77 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
--rw-r--r--   0        0        0      544 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
--rw-r--r--   0        0        0      920 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
--rw-r--r--   0        0        0      143 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      844 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      838 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0      627 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/__init__.py
--rw-r--r--   0        0        0      207 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/__init__.py
--rw-r--r--   0        0        0     7531 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/client.py
--rw-r--r--   0        0        0      270 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0      729 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status.py
--rw-r--r--   0        0        0     1151 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status_response.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/__init__.py
--rw-r--r--   0        0        0      599 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/__init__.py
--rw-r--r--   0        0        0      452 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/__init__.py
--rw-r--r--   0        0        0     9170 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/client.py
--rw-r--r--   0        0        0      530 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/__init__.py
--rw-r--r--   0        0        0      305 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/export_date_too_early_error.py
--rw-r--r--   0        0        0      309 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/export_files_unavailable_error.py
--rw-r--r--   0        0        0      308 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/export_not_yet_available_error.py
--rw-r--r--   0        0        0      320 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/missing_daily_incremental_export_file_error.py
--rw-r--r--   0        0        0      152 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     1263 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/types/get_exports_response.py
--rw-r--r--   0        0        0      953 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/__init__.py
--rw-r--r--   0        0        0     1139 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/__init__.py
--rw-r--r--   0        0        0      870 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/allocation.py
--rw-r--r--   0        0        0      895 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/allocation_create.py
--rw-r--r--   0        0        0     1066 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/allocation_recipient.py
--rw-r--r--   0        0        0     1152 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/allocation_recipient_create.py
--rw-r--r--   0        0        0      916 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/refund_allocation.py
--rw-r--r--   0        0        0      941 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/refund_allocation_create.py
--rw-r--r--   0        0        0      356 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/financials/types/refund_reason.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/__init__.py
--rw-r--r--   0        0        0      603 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/__init__.py
--rw-r--r--   0        0        0      417 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/__init__.py
--rw-r--r--   0        0        0    11693 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/client.py
--rw-r--r--   0        0        0      202 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/errors/__init__.py
--rw-r--r--   0        0        0      387 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/errors/encounter_has_existing_guarantor_error.py
--rw-r--r--   0        0        0      438 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0      806 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py
--rw-r--r--   0        0        0     1119 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
--rw-r--r--   0        0        0      998 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
--rw-r--r--   0        0        0     1225 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
--rw-r--r--   0        0        0      967 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/__init__.py
--rw-r--r--   0        0        0     1231 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/__init__.py
--rw-r--r--   0        0        0      900 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier.py
--rw-r--r--   0        0        0     1051 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_base.py
--rw-r--r--   0        0        0      436 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_code.py
--rw-r--r--   0        0        0      833 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_create.py
--rw-r--r--   0        0        0      103 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_id.py
--rw-r--r--   0        0        0     1187 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_update.py
--rw-r--r--   0        0        0      925 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_value.py
--rw-r--r--   0        0        0      858 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/medicaid_provider_identifier.py
--rw-r--r--   0        0        0      858 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/medicare_provider_identifier.py
--rw-r--r--   0        0        0     1028 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/identifiers/types/updatable_identifier.py
--rw-r--r--   0        0        0      435 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      602 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      848 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-10-30 17:13:09.793294 candidhealth-0.8.0/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0     1109 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1510 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/patient_base.py
--rw-r--r--   0        0        0     1211 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      999 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1227 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      952 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/__init__.py
--rw-r--r--   0        0        0      627 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/__init__.py
--rw-r--r--   0        0        0      721 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/__init__.py
--rw-r--r--   0        0        0     7223 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/client.py
--rw-r--r--   0        0        0     1049 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1192 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjudication.py
--rw-r--r--   0        0        0     1217 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjudication_create.py
--rw-r--r--   0        0        0     1000 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjustment_reason_code.py
--rw-r--r--   0        0        0     1312 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/insurance_adjudication.py
--rw-r--r--   0        0        0     1219 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/insurance_adjudication_create.py
--rw-r--r--   0        0        0      114 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/insurance_adjudication_id.py
--rw-r--r--   0        0        0      851 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/remittance_advice_remark_code.py
--rw-r--r--   0        0        0     1632 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/service_line_adjudication.py
--rw-r--r--   0        0        0     1510 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/service_line_adjudication_create.py
--rw-r--r--   0        0        0      116 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/service_line_adjudication_id.py
--rw-r--r--   0        0        0      247 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1133 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1222 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1180 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/__init__.py
--rw-r--r--   0        0        0      617 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/__init__.py
--rw-r--r--   0        0        0      219 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/__init__.py
--rw-r--r--   0        0        0     7641 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/client.py
--rw-r--r--   0        0        0      298 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1094 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund.py
--rw-r--r--   0        0        0     1025 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_create.py
--rw-r--r--   0        0        0      108 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_id.py
--rw-r--r--   0        0        0      175 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      229 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1440 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      876 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      123 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      627 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/client.py
--rw-r--r--   0        0        0      114 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      415 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      570 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0     8568 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1081 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0      113 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      990 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_sort_options.py
--rw-r--r--   0        0        0      510 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      367 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/__init__.py
--rw-r--r--   0        0        0    15852 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/client.py
--rw-r--r--   0        0        0      499 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     3137 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_create_v_2.py
--rw-r--r--   0        0        0      967 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_page_v_2.py
--rw-r--r--   0        0        0     3327 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_update_v_2.py
--rw-r--r--   0        0        0     3305 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_v_2.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/__init__.py
--rw-r--r--   0        0        0      643 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/__init__.py
--rw-r--r--   0        0        0      785 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/__init__.py
--rw-r--r--   0        0        0    15313 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/client.py
--rw-r--r--   0        0        0     1149 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     2508 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility.py
--rw-r--r--   0        0        0     2370 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_create.py
--rw-r--r--   0        0        0      120 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_id.py
--rw-r--r--   0        0        0      986 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_page.py
--rw-r--r--   0        0        0     2466 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_update.py
--rw-r--r--   0        0        0      831 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_mode.py
--rw-r--r--   0        0        0     1709 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_operational_status.py
--rw-r--r--   0        0        0     3970 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_physical_type.py
--rw-r--r--   0        0        0      849 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_status.py
--rw-r--r--   0        0        0    36899 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_type.py
--rw-r--r--   0        0        0      123 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      615 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/client.py
--rw-r--r--   0        0        0      114 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
--rw-r--r--   0        0        0      370 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     1709 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
--rw-r--r--   0        0        0      167 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/__init__.py
--rw-r--r--   0        0        0     9388 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/client.py
--rw-r--r--   0        0        0      208 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0     1283 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment.py
--rw-r--r--   0        0        0      107 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/__init__.py
--rw-r--r--   0        0        0      613 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/__init__.py
--rw-r--r--   0        0        0      163 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/__init__.py
--rw-r--r--   0        0        0     9353 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/client.py
--rw-r--r--   0        0        0      202 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1276 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund.py
--rw-r--r--   0        0        0      106 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0      597 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/__init__.py
--rw-r--r--   0        0        0      159 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/__init__.py
--rw-r--r--   0        0        0     4814 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/client.py
--rw-r--r--   0        0        0      205 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/payer.py
--rw-r--r--   0        0        0      896 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/payer_page.py
--rw-r--r--   0        0        0      100 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/payer_uuid.py
--rw-r--r--   0        0        0      251 2023-10-30 17:13:09.797294 candidhealth-0.8.0/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0     1002 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1601 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/__init__.py
--rw-r--r--   0        0        0      557 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/__init__.py
--rw-r--r--   0        0        0      797 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/denial_reason_content.py
--rw-r--r--   0        0        0     1133 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_id_qualifier.py
--rw-r--r--   0        0        0     3045 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line.py
--rw-r--r--   0        0        0      989 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_adjustment.py
--rw-r--r--   0        0        0     2150 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_create.py
--rw-r--r--   0        0        0     1124 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      946 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      826 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      888 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/__init__.py
--rw-r--r--   0        0        0      603 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/client.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/__init__.py
--rw-r--r--   0        0        0      211 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/__init__.py
--rw-r--r--   0        0        0     6895 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/client.py
--rw-r--r--   0        0        0      298 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off.py
--rw-r--r--   0        0        0     1008 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off_create.py
--rw-r--r--   0        0        0      101 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off_id.py
--rw-r--r--   0        0        0      850 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off_reason.py
--rw-r--r--   0        0        0      111 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/__init__.py
--rw-r--r--   0        0        0      102 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/resources/__init__.py
--rw-r--r--   0        0        0      123 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/__init__.py
--rw-r--r--   0        0        0      139 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0    35570 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/types/carc.py
--rw-r--r--   0        0        0   129764 2023-10-30 17:13:09.801294 candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/types/rarc.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2023-11-09 20:41:29.726154 candidhealth-0.9.0/README.md
+-rw-r--r--   0        0        0      393 2023-11-09 20:41:29.726154 candidhealth-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6877 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/__init__.py
+-rw-r--r--   0        0        0     2650 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/candid_api_client.py
+-rw-r--r--   0        0        0     5790 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/client.py
+-rw-r--r--   0        0        0      519 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1620 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      227 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-11-09 20:41:29.726154 candidhealth-0.9.0/src/candid/py.typed
+-rw-r--r--   0        0        0     6977 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      593 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     5343 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      882 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      792 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0      609 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/__init__.py
+-rw-r--r--   0        0        0      191 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     2710 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/client.py
+-rw-r--r--   0        0        0      256 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1370 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note.py
+-rw-r--r--   0        0        0      838 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/__init__.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/__init__.py
+-rw-r--r--   0        0        0      269 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      377 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      827 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/claim_frequency_type_code.py
+-rw-r--r--   0        0        0     1264 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/claim_submission_record_create.py
+-rw-r--r--   0        0        0     1369 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/external_claim_submission_create.py
+-rw-r--r--   0        0        0      139 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1192 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     2771 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0      861 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      333 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/entity_not_found_error.py
+-rw-r--r--   0        0        0      326 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/http_request_validation_error.py
+-rw-r--r--   0        0        0      355 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/http_request_validations_error.py
+-rw-r--r--   0        0        0      365 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/http_service_unavailable_error.py
+-rw-r--r--   0        0        0      377 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/organization_not_authorized_error.py
+-rw-r--r--   0        0        0      323 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      470 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/errors/updates_disabled_due_to_external_system_integration_error.py
+-rw-r--r--   0        0        0     3403 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1400 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/claim_adjustment_group_codes.py
+-rw-r--r--   0        0        0       98 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0      558 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/claim_submission_payer_responsibility_type.py
+-rw-r--r--   0        0        0       76 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0      849 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/date_range_optional_end.py
+-rw-r--r--   0        0        0       79 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/decimal.py
+-rw-r--r--   0        0        0       77 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/email.py
+-rw-r--r--   0        0        0      485 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/emr_payer_crosswalk.py
+-rw-r--r--   0        0        0       91 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0      787 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/entity_not_found_error_message.py
+-rw-r--r--   0        0        0       84 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/error_message.py
+-rw-r--r--   0        0        0    13536 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0      817 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/http_service_unavailable_error_message.py
+-rw-r--r--   0        0        0    15447 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0      100 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/invoice_id.py
+-rw-r--r--   0        0        0       79 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0      803 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/organization_not_authorized_error_message.py
+-rw-r--r--   0        0        0       81 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     5534 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0      849 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      620 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/phone_number_type.py
+-rw-r--r--   0        0        0    80253 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      101 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/provider_id.py
+-rw-r--r--   0        0        0      763 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/removable_date_range_optional_end.py
+-rw-r--r--   0        0        0      969 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/request_validation_error.py
+-rw-r--r--   0        0        0      891 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     7036 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1060 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0     1008 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1026 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0      807 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/unauthorized_error_message.py
+-rw-r--r--   0        0        0      840 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/updates_disabled_due_to_external_system_integration_error_message.py
+-rw-r--r--   0        0        0       83 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      121 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      127 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      101 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      279 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      985 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1927 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      930 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/eligibility/__init__.py
+-rw-r--r--   0        0        0      607 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/eligibility/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/eligibility/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/eligibility/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     7297 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/eligibility/resources/v_2/client.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     2015 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1119 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1287 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1271 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1271 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      605 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     1968 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    67469 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0      422 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
+-rw-r--r--   0        0        0      327 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/errors/cash_pay_payer_error.py
+-rw-r--r--   0        0        0      387 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
+-rw-r--r--   0        0        0      416 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/errors/encounter_guarantor_missing_contact_info_error.py
+-rw-r--r--   0        0        0     2656 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      518 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/billable_status_type.py
+-rw-r--r--   0        0        0      792 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/cash_pay_payer_error_message.py
+-rw-r--r--   0        0        0      901 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      971 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      921 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      790 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0     7960 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0     5239 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      916 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
+-rw-r--r--   0        0        0      833 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py
+-rw-r--r--   0        0        0      850 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_owner_of_next_action_type.py
+-rw-r--r--   0        0        0      912 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      521 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_submission_origin_type.py
+-rw-r--r--   0        0        0      889 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      996 2023-11-09 20:41:29.730154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      918 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1324 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      882 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      980 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0     2615 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0     1035 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0      710 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/responsible_party_type.py
+-rw-r--r--   0        0        0       77 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      544 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      920 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      838 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      123 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0      820 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      114 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     7531 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/client.py
+-rw-r--r--   0        0        0      270 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status.py
+-rw-r--r--   0        0        0     1151 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status_response.py
+-rw-r--r--   0        0        0     1920 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     9486 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/client.py
+-rw-r--r--   0        0        0      193 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      384 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/errors/expected_network_status_check_error.py
+-rw-r--r--   0        0        0     2453 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     2787 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/compute_all_in_network_providers_request.py
+-rw-r--r--   0        0        0     1169 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/compute_all_in_network_providers_response.py
+-rw-r--r--   0        0        0     1403 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/compute_all_in_network_rendering_providers_result.py
+-rw-r--r--   0        0        0      806 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/expected_network_status_check_error_message.py
+-rw-r--r--   0        0        0     2782 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/expected_network_status_request_v_2.py
+-rw-r--r--   0        0        0      999 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/expected_network_status_response_v_2.py
+-rw-r--r--   0        0        0     1284 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/expected_network_status_subscriber_information.py
+-rw-r--r--   0        0        0     1171 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/expected_network_status_v_2.py
+-rw-r--r--   0        0        0     1106 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/in_network_rendering_providers_detail.py
+-rw-r--r--   0        0        0     1027 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/in_network_status.py
+-rw-r--r--   0        0        0     1093 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/indeterminate_network_status.py
+-rw-r--r--   0        0        0     1199 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/insurance_type.py
+-rw-r--r--   0        0        0      676 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/line_of_business.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/network_status_check_id.py
+-rw-r--r--   0        0        0     1051 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/out_of_network_status.py
+-rw-r--r--   0        0        0     8627 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/service_type.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/__init__.py
+-rw-r--r--   0        0        0      599 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/__init__.py
+-rw-r--r--   0        0        0      452 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/__init__.py
+-rw-r--r--   0        0        0     9170 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/client.py
+-rw-r--r--   0        0        0      530 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/__init__.py
+-rw-r--r--   0        0        0      305 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/export_date_too_early_error.py
+-rw-r--r--   0        0        0      309 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/export_files_unavailable_error.py
+-rw-r--r--   0        0        0      308 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/export_not_yet_available_error.py
+-rw-r--r--   0        0        0      320 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/missing_daily_incremental_export_file_error.py
+-rw-r--r--   0        0        0      152 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1263 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/types/get_exports_response.py
+-rw-r--r--   0        0        0      801 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/__init__.py
+-rw-r--r--   0        0        0      922 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/__init__.py
+-rw-r--r--   0        0        0      858 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/allocation.py
+-rw-r--r--   0        0        0      883 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/allocation_create.py
+-rw-r--r--   0        0        0     1045 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/allocation_target.py
+-rw-r--r--   0        0        0     1122 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/allocation_target_create.py
+-rw-r--r--   0        0        0      356 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/financials/types/refund_reason.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/__init__.py
+-rw-r--r--   0        0        0      603 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/__init__.py
+-rw-r--r--   0        0        0      417 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/__init__.py
+-rw-r--r--   0        0        0    11693 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/client.py
+-rw-r--r--   0        0        0      202 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/errors/__init__.py
+-rw-r--r--   0        0        0      387 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/errors/encounter_has_existing_guarantor_error.py
+-rw-r--r--   0        0        0      438 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      806 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py
+-rw-r--r--   0        0        0     1119 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
+-rw-r--r--   0        0        0      998 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
+-rw-r--r--   0        0        0     1225 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
+-rw-r--r--   0        0        0      967 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/__init__.py
+-rw-r--r--   0        0        0     1231 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier.py
+-rw-r--r--   0        0        0     1051 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_base.py
+-rw-r--r--   0        0        0      436 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_code.py
+-rw-r--r--   0        0        0      833 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_create.py
+-rw-r--r--   0        0        0      103 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_id.py
+-rw-r--r--   0        0        0     1187 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_update.py
+-rw-r--r--   0        0        0      925 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_value.py
+-rw-r--r--   0        0        0      858 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/medicaid_provider_identifier.py
+-rw-r--r--   0        0        0      858 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/medicare_provider_identifier.py
+-rw-r--r--   0        0        0     1028 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/identifiers/types/updatable_identifier.py
+-rw-r--r--   0        0        0      435 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      602 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      848 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0     1109 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1510 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/patient_base.py
+-rw-r--r--   0        0        0     1211 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      999 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1227 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      952 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/__init__.py
+-rw-r--r--   0        0        0      629 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/__init__.py
+-rw-r--r--   0        0        0      721 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     7223 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/client.py
+-rw-r--r--   0        0        0     1049 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1192 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjudication.py
+-rw-r--r--   0        0        0     1217 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjudication_create.py
+-rw-r--r--   0        0        0     1000 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjustment_reason_code.py
+-rw-r--r--   0        0        0     1312 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/insurance_adjudication.py
+-rw-r--r--   0        0        0     1219 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/insurance_adjudication_create.py
+-rw-r--r--   0        0        0      114 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/insurance_adjudication_id.py
+-rw-r--r--   0        0        0      851 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/remittance_advice_remark_code.py
+-rw-r--r--   0        0        0     1632 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/service_line_adjudication.py
+-rw-r--r--   0        0        0     1510 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/service_line_adjudication_create.py
+-rw-r--r--   0        0        0      116 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/service_line_adjudication_id.py
+-rw-r--r--   0        0        0      247 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1133 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1222 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1180 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/__init__.py
+-rw-r--r--   0        0        0      617 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/__init__.py
+-rw-r--r--   0        0        0      219 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     7641 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/client.py
+-rw-r--r--   0        0        0      298 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1178 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund.py
+-rw-r--r--   0        0        0     1109 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_create.py
+-rw-r--r--   0        0        0      108 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_id.py
+-rw-r--r--   0        0        0      175 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      229 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1440 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      876 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      123 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      627 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/client.py
+-rw-r--r--   0        0        0      114 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      415 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      570 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0     8568 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1081 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0      113 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      990 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_sort_options.py
+-rw-r--r--   0        0        0      510 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      367 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/__init__.py
+-rw-r--r--   0        0        0    15852 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/client.py
+-rw-r--r--   0        0        0      499 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     3137 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_create_v_2.py
+-rw-r--r--   0        0        0      967 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_page_v_2.py
+-rw-r--r--   0        0        0     3327 2023-11-09 20:41:29.734154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_update_v_2.py
+-rw-r--r--   0        0        0     3305 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_v_2.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/__init__.py
+-rw-r--r--   0        0        0      643 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/__init__.py
+-rw-r--r--   0        0        0      785 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/__init__.py
+-rw-r--r--   0        0        0    15313 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/client.py
+-rw-r--r--   0        0        0     1149 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     2508 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility.py
+-rw-r--r--   0        0        0     2370 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_create.py
+-rw-r--r--   0        0        0      120 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_id.py
+-rw-r--r--   0        0        0      986 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_page.py
+-rw-r--r--   0        0        0     2466 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_update.py
+-rw-r--r--   0        0        0      831 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_mode.py
+-rw-r--r--   0        0        0     1709 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_operational_status.py
+-rw-r--r--   0        0        0     3970 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_physical_type.py
+-rw-r--r--   0        0        0      849 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_status.py
+-rw-r--r--   0        0        0    36899 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_type.py
+-rw-r--r--   0        0        0      123 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      615 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/client.py
+-rw-r--r--   0        0        0      114 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
+-rw-r--r--   0        0        0      370 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1709 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
+-rw-r--r--   0        0        0      167 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/__init__.py
+-rw-r--r--   0        0        0     9305 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/client.py
+-rw-r--r--   0        0        0      208 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0     1395 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment.py
+-rw-r--r--   0        0        0      107 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/__init__.py
+-rw-r--r--   0        0        0      613 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/__init__.py
+-rw-r--r--   0        0        0      163 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     9721 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/client.py
+-rw-r--r--   0        0        0      202 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1498 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund.py
+-rw-r--r--   0        0        0      106 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0      597 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/__init__.py
+-rw-r--r--   0        0        0      159 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/__init__.py
+-rw-r--r--   0        0        0     4814 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/client.py
+-rw-r--r--   0        0        0      205 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/payer.py
+-rw-r--r--   0        0        0      896 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/payer_page.py
+-rw-r--r--   0        0        0      100 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/payer_uuid.py
+-rw-r--r--   0        0        0      251 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0     1002 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1601 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/__init__.py
+-rw-r--r--   0        0        0      557 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      797 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1133 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     3045 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line.py
+-rw-r--r--   0        0        0      989 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_adjustment.py
+-rw-r--r--   0        0        0     2150 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_create.py
+-rw-r--r--   0        0        0     1124 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      946 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      826 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      888 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/__init__.py
+-rw-r--r--   0        0        0      603 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/client.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/__init__.py
+-rw-r--r--   0        0        0      211 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     6895 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/client.py
+-rw-r--r--   0        0        0      298 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off.py
+-rw-r--r--   0        0        0     1027 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off_create.py
+-rw-r--r--   0        0        0      101 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off_id.py
+-rw-r--r--   0        0        0      850 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off_reason.py
+-rw-r--r--   0        0        0      111 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/__init__.py
+-rw-r--r--   0        0        0      102 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/resources/__init__.py
+-rw-r--r--   0        0        0      123 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      139 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0    39373 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/types/carc.py
+-rw-r--r--   0        0        0   129764 2023-11-09 20:41:29.738154 candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/types/rarc.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.9.0/PKG-INFO
```

### Comparing `candidhealth-0.8.0/src/candid/__init__.py` & `candidhealth-0.9.0/src/candid/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,165 +1,154 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .resources import (
-    Allocation,
-    AllocationCreate,
-    AllocationRecipient,
-    AllocationRecipientCreate,
-    AllocationRecipientCreate_BillingProviderById,
-    AllocationRecipientCreate_ClaimById,
-    AllocationRecipientCreate_ServiceLineById,
-    AllocationRecipient_BillingProviderId,
-    AllocationRecipient_Claim,
-    AllocationRecipient_ServiceLine,
-    Claim,
+from . import (
+    auth,
+    billing_notes,
+    claim_submission,
+    claims,
+    commons,
+    contracts,
+    diagnoses,
+    eligibility,
+    encounter_providers,
+    encounters,
+    era,
+    expected_network_status,
+    exports,
+    financials,
+    guarantor,
+    identifiers,
+    individual,
+    insurance_adjudications,
+    insurance_card,
+    insurance_refunds,
+    invoices,
+    organization_providers,
+    organization_service_facilities,
+    patient_payments,
+    patient_refunds,
+    payers,
+    service_facility,
+    service_lines,
+    tags,
+    write_offs,
+    x_12,
+)
+from .claims import Claim, ClaimStatus
+from .commons import (
     ClaimAdjustmentGroupCodes,
     ClaimId,
-    ClaimStatus,
     ClaimSubmissionPayerResponsibilityType,
-    ContractId,
     Date,
     DateRangeOptionalEnd,
     Decimal,
-    Diagnosis,
-    DiagnosisCreate,
-    DiagnosisId,
-    DiagnosisTypeCode,
     Email,
     EmrPayerCrosswalk,
     EncounterExternalId,
     EncounterId,
-    EncounterServiceFacility,
-    EncounterServiceFacilityBase,
     EntityNotFoundError,
     EntityNotFoundErrorMessage,
-    Era,
-    EraBase,
-    EraId,
     ErrorMessage,
     FacilityTypeCode,
-    Gender,
     HttpRequestValidationError,
     HttpRequestValidationsError,
     HttpServiceUnavailableError,
     HttpServiceUnavailableErrorMessage,
-    Identifier,
-    IdentifierBase,
-    IdentifierCode,
-    IdentifierCreate,
-    IdentifierId,
-    IdentifierUpdate,
-    IdentifierValue,
-    IdentifierValue_MedicaidProviderIdentifier,
-    IdentifierValue_MedicareProviderIdentifier,
-    IndividualBase,
-    IndividualId,
-    InsuranceCard,
-    InsuranceCardBase,
-    InsuranceCardCreate,
-    InsuranceCardId,
     InsuranceTypeCode,
-    Invoice,
     InvoiceId,
-    InvoiceItem,
-    InvoiceStatus,
     LinkUrl,
-    MedicaidProviderIdentifier,
-    MedicareProviderIdentifier,
     Npi,
     OrganizationId,
+    OrganizationNotAuthorizedError,
+    OrganizationNotAuthorizedErrorMessage,
     PageToken,
-    Patient,
-    PatientBase,
-    PatientCreate,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
     PhoneNumber,
     PhoneNumberType,
     ProcedureModifier,
     ProviderId,
-    RefundAllocation,
-    RefundAllocationCreate,
-    RefundReason,
     RemovableDateRangeOptionalEnd,
     RemovableDateRangeOptionalEnd_DateRange,
     RemovableDateRangeOptionalEnd_Remove,
     RequestValidationError,
     ResourcePage,
-    ServiceFacilityId,
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
-    StandaloneDiagnosisCreate,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
-    Subscriber,
-    SubscriberBase,
-    SubscriberCreate,
-    Tag,
-    TagColorEnum,
-    TagCreate,
-    TagId,
     UnauthorizedError,
     UnauthorizedErrorMessage,
+    UpdatesDisabledDueToExternalSystemIntegrationError,
+    UpdatesDisabledDueToExternalSystemIntegrationErrorMessage,
+    WorkQueueId,
+)
+from .contracts import ContractId
+from .diagnoses import Diagnosis, DiagnosisCreate, DiagnosisId, DiagnosisTypeCode, StandaloneDiagnosisCreate
+from .era import Era, EraBase, EraId
+from .financials import (
+    Allocation,
+    AllocationCreate,
+    AllocationTarget,
+    AllocationTargetCreate,
+    AllocationTargetCreate_BillingProviderById,
+    AllocationTargetCreate_ClaimById,
+    AllocationTargetCreate_ServiceLineById,
+    AllocationTarget_BillingProviderId,
+    AllocationTarget_Claim,
+    AllocationTarget_ServiceLine,
+    RefundReason,
+)
+from .identifiers import (
+    Identifier,
+    IdentifierBase,
+    IdentifierCode,
+    IdentifierCreate,
+    IdentifierId,
+    IdentifierUpdate,
+    IdentifierValue,
+    IdentifierValue_MedicaidProviderIdentifier,
+    IdentifierValue_MedicareProviderIdentifier,
+    MedicaidProviderIdentifier,
+    MedicareProviderIdentifier,
     UpdatableIdentifier,
     UpdatableIdentifier_Add,
     UpdatableIdentifier_Remove,
     UpdatableIdentifier_Update,
-    UpdatesDisabledDueToExternalSystemIntegrationError,
-    UpdatesDisabledDueToExternalSystemIntegrationErrorMessage,
-    WorkQueueId,
-    auth,
-    billing_notes,
-    claim_submission,
-    claims,
-    commons,
-    contracts,
-    diagnoses,
-    eligibility,
-    encounter_providers,
-    encounters,
-    era,
-    expected_network_status,
-    exports,
-    financials,
-    guarantor,
-    identifiers,
-    individual,
-    insurance_adjudication,
-    insurance_card,
-    insurance_refunds,
-    invoices,
-    organization_providers,
-    organization_service_facilities,
-    patient_payments,
-    patient_refunds,
-    payers,
-    service_facility,
-    service_lines,
-    tags,
-    write_offs,
-    x_12,
 )
-from .environment import CandidApiEnvironment
+from .individual import (
+    Gender,
+    IndividualBase,
+    IndividualId,
+    Patient,
+    PatientBase,
+    PatientCreate,
+    Subscriber,
+    SubscriberBase,
+    SubscriberCreate,
+)
+from .insurance_card import InsuranceCard, InsuranceCardBase, InsuranceCardCreate, InsuranceCardId
+from .invoices import Invoice, InvoiceItem, InvoiceStatus
+from .service_facility import EncounterServiceFacility, EncounterServiceFacilityBase, ServiceFacilityId
+from .tags import Tag, TagColorEnum, TagCreate, TagId
 
 __all__ = [
     "Allocation",
     "AllocationCreate",
-    "AllocationRecipient",
-    "AllocationRecipientCreate",
-    "AllocationRecipientCreate_BillingProviderById",
-    "AllocationRecipientCreate_ClaimById",
-    "AllocationRecipientCreate_ServiceLineById",
-    "AllocationRecipient_BillingProviderId",
-    "AllocationRecipient_Claim",
-    "AllocationRecipient_ServiceLine",
-    "CandidApiEnvironment",
+    "AllocationTarget",
+    "AllocationTargetCreate",
+    "AllocationTargetCreate_BillingProviderById",
+    "AllocationTargetCreate_ClaimById",
+    "AllocationTargetCreate_ServiceLineById",
+    "AllocationTarget_BillingProviderId",
+    "AllocationTarget_Claim",
+    "AllocationTarget_ServiceLine",
     "Claim",
     "ClaimAdjustmentGroupCodes",
     "ClaimId",
     "ClaimStatus",
     "ClaimSubmissionPayerResponsibilityType",
     "ContractId",
     "Date",
@@ -208,26 +197,26 @@
     "InvoiceItem",
     "InvoiceStatus",
     "LinkUrl",
     "MedicaidProviderIdentifier",
     "MedicareProviderIdentifier",
     "Npi",
     "OrganizationId",
+    "OrganizationNotAuthorizedError",
+    "OrganizationNotAuthorizedErrorMessage",
     "PageToken",
     "Patient",
     "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderId",
-    "RefundAllocation",
-    "RefundAllocationCreate",
     "RefundReason",
     "RemovableDateRangeOptionalEnd",
     "RemovableDateRangeOptionalEnd_DateRange",
     "RemovableDateRangeOptionalEnd_Remove",
     "RequestValidationError",
     "ResourcePage",
     "ServiceFacilityId",
@@ -268,15 +257,15 @@
     "era",
     "expected_network_status",
     "exports",
     "financials",
     "guarantor",
     "identifiers",
     "individual",
-    "insurance_adjudication",
+    "insurance_adjudications",
     "insurance_card",
     "insurance_refunds",
     "invoices",
     "organization_providers",
     "organization_service_facilities",
     "patient_payments",
     "patient_refunds",
```

### Comparing `candidhealth-0.8.0/src/candid/candid_api_client.py` & `candidhealth-0.9.0/src/candid/candid_api_client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/client.py` & `candidhealth-0.9.0/src/candid/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.billing_notes.client import AsyncBillingNotesClient, BillingNotesClient
 from .resources.eligibility.client import AsyncEligibilityClient, EligibilityClient
 from .resources.encounters.client import AsyncEncountersClient, EncountersClient
 from .resources.expected_network_status.client import AsyncExpectedNetworkStatusClient, ExpectedNetworkStatusClient
 from .resources.exports.client import AsyncExportsClient, ExportsClient
 from .resources.guarantor.client import AsyncGuarantorClient, GuarantorClient
-from .resources.insurance_adjudication.client import AsyncInsuranceAdjudicationClient, InsuranceAdjudicationClient
+from .resources.insurance_adjudications.client import AsyncInsuranceAdjudicationsClient, InsuranceAdjudicationsClient
 from .resources.insurance_refunds.client import AsyncInsuranceRefundsClient, InsuranceRefundsClient
 from .resources.organization_providers.client import AsyncOrganizationProvidersClient, OrganizationProvidersClient
 from .resources.organization_service_facilities.client import (
     AsyncOrganizationServiceFacilitiesClient,
     OrganizationServiceFacilitiesClient,
 )
 from .resources.patient_payments.client import AsyncPatientPaymentsClient, PatientPaymentsClient
@@ -43,15 +43,15 @@
         self.auth = AuthClient(client_wrapper=self._client_wrapper)
         self.billing_notes = BillingNotesClient(client_wrapper=self._client_wrapper)
         self.eligibility = EligibilityClient(client_wrapper=self._client_wrapper)
         self.encounters = EncountersClient(client_wrapper=self._client_wrapper)
         self.expected_network_status = ExpectedNetworkStatusClient(client_wrapper=self._client_wrapper)
         self.exports = ExportsClient(client_wrapper=self._client_wrapper)
         self.guarantor = GuarantorClient(client_wrapper=self._client_wrapper)
-        self.insurance_adjudication = InsuranceAdjudicationClient(client_wrapper=self._client_wrapper)
+        self.insurance_adjudications = InsuranceAdjudicationsClient(client_wrapper=self._client_wrapper)
         self.insurance_refunds = InsuranceRefundsClient(client_wrapper=self._client_wrapper)
         self.organization_service_facilities = OrganizationServiceFacilitiesClient(client_wrapper=self._client_wrapper)
         self.organization_providers = OrganizationProvidersClient(client_wrapper=self._client_wrapper)
         self.patient_payments = PatientPaymentsClient(client_wrapper=self._client_wrapper)
         self.patient_refunds = PatientRefundsClient(client_wrapper=self._client_wrapper)
         self.payers = PayersClient(client_wrapper=self._client_wrapper)
         self.write_offs = WriteOffsClient(client_wrapper=self._client_wrapper)
@@ -74,15 +74,15 @@
         self.auth = AsyncAuthClient(client_wrapper=self._client_wrapper)
         self.billing_notes = AsyncBillingNotesClient(client_wrapper=self._client_wrapper)
         self.eligibility = AsyncEligibilityClient(client_wrapper=self._client_wrapper)
         self.encounters = AsyncEncountersClient(client_wrapper=self._client_wrapper)
         self.expected_network_status = AsyncExpectedNetworkStatusClient(client_wrapper=self._client_wrapper)
         self.exports = AsyncExportsClient(client_wrapper=self._client_wrapper)
         self.guarantor = AsyncGuarantorClient(client_wrapper=self._client_wrapper)
-        self.insurance_adjudication = AsyncInsuranceAdjudicationClient(client_wrapper=self._client_wrapper)
+        self.insurance_adjudications = AsyncInsuranceAdjudicationsClient(client_wrapper=self._client_wrapper)
         self.insurance_refunds = AsyncInsuranceRefundsClient(client_wrapper=self._client_wrapper)
         self.organization_service_facilities = AsyncOrganizationServiceFacilitiesClient(
             client_wrapper=self._client_wrapper
         )
         self.organization_providers = AsyncOrganizationProvidersClient(client_wrapper=self._client_wrapper)
         self.patient_payments = AsyncPatientPaymentsClient(client_wrapper=self._client_wrapper)
         self.patient_refunds = AsyncPatientRefundsClient(client_wrapper=self._client_wrapper)
```

### Comparing `candidhealth-0.8.0/src/candid/core/__init__.py` & `candidhealth-0.9.0/src/candid/core/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/core/client_wrapper.py` & `candidhealth-0.9.0/src/candid/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "candidhealth",
-            "X-Fern-SDK-Version": "0.8.0",
+            "X-Fern-SDK-Version": "0.9.0",
         }
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
 
     def _get_token(self) -> typing.Optional[str]:
```

### Comparing `candidhealth-0.8.0/src/candid/core/datetime_utils.py` & `candidhealth-0.9.0/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/core/jsonable_encoder.py` & `candidhealth-0.9.0/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/__init__.py` & `candidhealth-0.9.0/src/candid/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,165 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import (
-    auth,
-    billing_notes,
-    claim_submission,
-    claims,
-    commons,
-    contracts,
-    diagnoses,
-    eligibility,
-    encounter_providers,
-    encounters,
-    era,
-    expected_network_status,
-    exports,
-    financials,
-    guarantor,
-    identifiers,
-    individual,
-    insurance_adjudication,
-    insurance_card,
-    insurance_refunds,
-    invoices,
-    organization_providers,
-    organization_service_facilities,
-    patient_payments,
-    patient_refunds,
-    payers,
-    service_facility,
-    service_lines,
-    tags,
-    write_offs,
-    x_12,
-)
-from .claims import Claim, ClaimStatus
-from .commons import (
+from .resources import (
+    Allocation,
+    AllocationCreate,
+    AllocationTarget,
+    AllocationTargetCreate,
+    AllocationTargetCreate_BillingProviderById,
+    AllocationTargetCreate_ClaimById,
+    AllocationTargetCreate_ServiceLineById,
+    AllocationTarget_BillingProviderId,
+    AllocationTarget_Claim,
+    AllocationTarget_ServiceLine,
+    Claim,
     ClaimAdjustmentGroupCodes,
     ClaimId,
+    ClaimStatus,
     ClaimSubmissionPayerResponsibilityType,
+    ContractId,
     Date,
     DateRangeOptionalEnd,
     Decimal,
+    Diagnosis,
+    DiagnosisCreate,
+    DiagnosisId,
+    DiagnosisTypeCode,
     Email,
     EmrPayerCrosswalk,
     EncounterExternalId,
     EncounterId,
+    EncounterServiceFacility,
+    EncounterServiceFacilityBase,
     EntityNotFoundError,
     EntityNotFoundErrorMessage,
+    Era,
+    EraBase,
+    EraId,
     ErrorMessage,
     FacilityTypeCode,
+    Gender,
     HttpRequestValidationError,
     HttpRequestValidationsError,
     HttpServiceUnavailableError,
     HttpServiceUnavailableErrorMessage,
+    Identifier,
+    IdentifierBase,
+    IdentifierCode,
+    IdentifierCreate,
+    IdentifierId,
+    IdentifierUpdate,
+    IdentifierValue,
+    IdentifierValue_MedicaidProviderIdentifier,
+    IdentifierValue_MedicareProviderIdentifier,
+    IndividualBase,
+    IndividualId,
+    InsuranceCard,
+    InsuranceCardBase,
+    InsuranceCardCreate,
+    InsuranceCardId,
     InsuranceTypeCode,
+    Invoice,
     InvoiceId,
+    InvoiceItem,
+    InvoiceStatus,
     LinkUrl,
+    MedicaidProviderIdentifier,
+    MedicareProviderIdentifier,
     Npi,
     OrganizationId,
+    OrganizationNotAuthorizedError,
+    OrganizationNotAuthorizedErrorMessage,
     PageToken,
+    Patient,
+    PatientBase,
+    PatientCreate,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
     PhoneNumber,
     PhoneNumberType,
     ProcedureModifier,
     ProviderId,
+    RefundReason,
     RemovableDateRangeOptionalEnd,
     RemovableDateRangeOptionalEnd_DateRange,
     RemovableDateRangeOptionalEnd_Remove,
     RequestValidationError,
     ResourcePage,
+    ServiceFacilityId,
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
+    StandaloneDiagnosisCreate,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
+    Subscriber,
+    SubscriberBase,
+    SubscriberCreate,
+    Tag,
+    TagColorEnum,
+    TagCreate,
+    TagId,
     UnauthorizedError,
     UnauthorizedErrorMessage,
-    UpdatesDisabledDueToExternalSystemIntegrationError,
-    UpdatesDisabledDueToExternalSystemIntegrationErrorMessage,
-    WorkQueueId,
-)
-from .contracts import ContractId
-from .diagnoses import Diagnosis, DiagnosisCreate, DiagnosisId, DiagnosisTypeCode, StandaloneDiagnosisCreate
-from .era import Era, EraBase, EraId
-from .financials import (
-    Allocation,
-    AllocationCreate,
-    AllocationRecipient,
-    AllocationRecipientCreate,
-    AllocationRecipientCreate_BillingProviderById,
-    AllocationRecipientCreate_ClaimById,
-    AllocationRecipientCreate_ServiceLineById,
-    AllocationRecipient_BillingProviderId,
-    AllocationRecipient_Claim,
-    AllocationRecipient_ServiceLine,
-    RefundAllocation,
-    RefundAllocationCreate,
-    RefundReason,
-)
-from .identifiers import (
-    Identifier,
-    IdentifierBase,
-    IdentifierCode,
-    IdentifierCreate,
-    IdentifierId,
-    IdentifierUpdate,
-    IdentifierValue,
-    IdentifierValue_MedicaidProviderIdentifier,
-    IdentifierValue_MedicareProviderIdentifier,
-    MedicaidProviderIdentifier,
-    MedicareProviderIdentifier,
     UpdatableIdentifier,
     UpdatableIdentifier_Add,
     UpdatableIdentifier_Remove,
     UpdatableIdentifier_Update,
+    UpdatesDisabledDueToExternalSystemIntegrationError,
+    UpdatesDisabledDueToExternalSystemIntegrationErrorMessage,
+    WorkQueueId,
+    auth,
+    billing_notes,
+    claim_submission,
+    claims,
+    commons,
+    contracts,
+    diagnoses,
+    eligibility,
+    encounter_providers,
+    encounters,
+    era,
+    expected_network_status,
+    exports,
+    financials,
+    guarantor,
+    identifiers,
+    individual,
+    insurance_adjudications,
+    insurance_card,
+    insurance_refunds,
+    invoices,
+    organization_providers,
+    organization_service_facilities,
+    patient_payments,
+    patient_refunds,
+    payers,
+    service_facility,
+    service_lines,
+    tags,
+    write_offs,
+    x_12,
 )
-from .individual import (
-    Gender,
-    IndividualBase,
-    IndividualId,
-    Patient,
-    PatientBase,
-    PatientCreate,
-    Subscriber,
-    SubscriberBase,
-    SubscriberCreate,
-)
-from .insurance_card import InsuranceCard, InsuranceCardBase, InsuranceCardCreate, InsuranceCardId
-from .invoices import Invoice, InvoiceItem, InvoiceStatus
-from .service_facility import EncounterServiceFacility, EncounterServiceFacilityBase, ServiceFacilityId
-from .tags import Tag, TagColorEnum, TagCreate, TagId
+from .environment import CandidApiEnvironment
 
 __all__ = [
     "Allocation",
     "AllocationCreate",
-    "AllocationRecipient",
-    "AllocationRecipientCreate",
-    "AllocationRecipientCreate_BillingProviderById",
-    "AllocationRecipientCreate_ClaimById",
-    "AllocationRecipientCreate_ServiceLineById",
-    "AllocationRecipient_BillingProviderId",
-    "AllocationRecipient_Claim",
-    "AllocationRecipient_ServiceLine",
+    "AllocationTarget",
+    "AllocationTargetCreate",
+    "AllocationTargetCreate_BillingProviderById",
+    "AllocationTargetCreate_ClaimById",
+    "AllocationTargetCreate_ServiceLineById",
+    "AllocationTarget_BillingProviderId",
+    "AllocationTarget_Claim",
+    "AllocationTarget_ServiceLine",
+    "CandidApiEnvironment",
     "Claim",
     "ClaimAdjustmentGroupCodes",
     "ClaimId",
     "ClaimStatus",
     "ClaimSubmissionPayerResponsibilityType",
     "ContractId",
     "Date",
@@ -197,26 +208,26 @@
     "InvoiceItem",
     "InvoiceStatus",
     "LinkUrl",
     "MedicaidProviderIdentifier",
     "MedicareProviderIdentifier",
     "Npi",
     "OrganizationId",
+    "OrganizationNotAuthorizedError",
+    "OrganizationNotAuthorizedErrorMessage",
     "PageToken",
     "Patient",
     "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderId",
-    "RefundAllocation",
-    "RefundAllocationCreate",
     "RefundReason",
     "RemovableDateRangeOptionalEnd",
     "RemovableDateRangeOptionalEnd_DateRange",
     "RemovableDateRangeOptionalEnd_Remove",
     "RequestValidationError",
     "ResourcePage",
     "ServiceFacilityId",
@@ -257,15 +268,15 @@
     "era",
     "expected_network_status",
     "exports",
     "financials",
     "guarantor",
     "identifiers",
     "individual",
-    "insurance_adjudication",
+    "insurance_adjudications",
     "insurance_card",
     "insurance_refunds",
     "invoices",
     "organization_providers",
     "organization_service_facilities",
     "patient_payments",
     "patient_refunds",
```

### Comparing `candidhealth-0.8.0/src/candid/resources/auth/client.py` & `candidhealth-0.9.0/src/candid/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/client.py` & `candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py` & `candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py` & `candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py` & `candidhealth-0.9.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/billing_notes/client.py` & `candidhealth-0.9.0/src/candid/resources/billing_notes/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/client.py` & `candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note.py` & `candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_base.py` & `candidhealth-0.9.0/src/candid/resources/billing_notes/resources/v_2/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/claim_frequency_type_code.py` & `candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/claim_frequency_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/claim_submission_record_create.py` & `candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/claim_submission_record_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 class ClaimSubmissionRecordCreate(pydantic.BaseModel):
     """
     Data about each external submission.
     """
 
     submitted_at: dt.datetime = pydantic.Field(description="When the claim was submitted to the payer.")
-    claim_frequency_code: ClaimFrequencyTypeCode
-    payer_responsibility: ClaimSubmissionPayerResponsibilityType
+    claim_frequency_code: typing.Optional[ClaimFrequencyTypeCode]
+    payer_responsibility: typing.Optional[ClaimSubmissionPayerResponsibilityType]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/claim_submission/resources/v_1/types/external_claim_submission_create.py` & `candidhealth-0.9.0/src/candid/resources/claim_submission/resources/v_1/types/external_claim_submission_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/claims/types/claim.py` & `candidhealth-0.9.0/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.9.0/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/__init__.py` & `candidhealth-0.9.0/src/candid/resources/commons/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     FacilityTypeCode,
     HttpServiceUnavailableErrorMessage,
     InsuranceTypeCode,
     InvoiceId,
     LinkUrl,
     Npi,
     OrganizationId,
+    OrganizationNotAuthorizedErrorMessage,
     PageToken,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
     PhoneNumber,
     PhoneNumberType,
     ProcedureModifier,
     ProviderId,
@@ -44,14 +45,15 @@
     WorkQueueId,
 )
 from .errors import (
     EntityNotFoundError,
     HttpRequestValidationError,
     HttpRequestValidationsError,
     HttpServiceUnavailableError,
+    OrganizationNotAuthorizedError,
     UnauthorizedError,
     UpdatesDisabledDueToExternalSystemIntegrationError,
 )
 
 __all__ = [
     "ClaimAdjustmentGroupCodes",
     "ClaimId",
@@ -72,14 +74,16 @@
     "HttpServiceUnavailableError",
     "HttpServiceUnavailableErrorMessage",
     "InsuranceTypeCode",
     "InvoiceId",
     "LinkUrl",
     "Npi",
     "OrganizationId",
+    "OrganizationNotAuthorizedError",
+    "OrganizationNotAuthorizedErrorMessage",
     "PageToken",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderId",
```

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/errors/__init__.py` & `candidhealth-0.9.0/src/candid/resources/commons/errors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .entity_not_found_error import EntityNotFoundError
 from .http_request_validation_error import HttpRequestValidationError
 from .http_request_validations_error import HttpRequestValidationsError
 from .http_service_unavailable_error import HttpServiceUnavailableError
+from .organization_not_authorized_error import OrganizationNotAuthorizedError
 from .unauthorized_error import UnauthorizedError
 from .updates_disabled_due_to_external_system_integration_error import (
     UpdatesDisabledDueToExternalSystemIntegrationError,
 )
 
 __all__ = [
     "EntityNotFoundError",
     "HttpRequestValidationError",
     "HttpRequestValidationsError",
     "HttpServiceUnavailableError",
+    "OrganizationNotAuthorizedError",
     "UnauthorizedError",
     "UpdatesDisabledDueToExternalSystemIntegrationError",
 ]
```

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .facility_type_code import FacilityTypeCode
 from .http_service_unavailable_error_message import HttpServiceUnavailableErrorMessage
 from .insurance_type_code import InsuranceTypeCode
 from .invoice_id import InvoiceId
 from .link_url import LinkUrl
 from .npi import Npi
 from .organization_id import OrganizationId
+from .organization_not_authorized_error_message import OrganizationNotAuthorizedErrorMessage
 from .page_token import PageToken
 from .patient_external_id import PatientExternalId
 from .patient_relationship_to_insured_code_all import PatientRelationshipToInsuredCodeAll
 from .phone_number import PhoneNumber
 from .phone_number_type import PhoneNumberType
 from .procedure_modifier import ProcedureModifier
 from .provider_id import ProviderId
@@ -62,14 +63,15 @@
     "FacilityTypeCode",
     "HttpServiceUnavailableErrorMessage",
     "InsuranceTypeCode",
     "InvoiceId",
     "LinkUrl",
     "Npi",
     "OrganizationId",
+    "OrganizationNotAuthorizedErrorMessage",
     "PageToken",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "PhoneNumber",
     "PhoneNumberType",
     "ProcedureModifier",
     "ProviderId",
```

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/claim_adjustment_group_codes.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/claim_adjustment_group_codes.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/claim_submission_payer_responsibility_type.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/claim_submission_payer_responsibility_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/date_range_optional_end.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/date_range_optional_end.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/entity_not_found_error_message.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/entity_not_found_error_message.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/http_service_unavailable_error_message.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/http_service_unavailable_error_message.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/phone_number.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/phone_number_type.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/removable_date_range_optional_end.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/removable_date_range_optional_end.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/request_validation_error.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/request_validation_error.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/state.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/unauthorized_error_message.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/unauthorized_error_message.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/commons/types/updates_disabled_due_to_external_system_integration_error_message.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/updates_disabled_due_to_external_system_integration_error_message.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.9.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.9.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/eligibility/client.py` & `candidhealth-0.9.0/src/candid/resources/eligibility/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/eligibility/resources/v_2/client.py` & `candidhealth-0.9.0/src/candid/resources/eligibility/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.9.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/client.py` & `candidhealth-0.9.0/src/candid/resources/encounters/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/__init__.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Encounter,
     EncounterBase,
     EncounterExternalIdUniquenessErrorType,
     EncounterGuarantorMissingContactInfoErrorType,
     EncounterOwnerOfNextActionType,
     EncounterPage,
     EncounterSortOptions,
+    EncounterSubmissionOriginType,
     IntakeFollowUp,
     IntakeFollowUpId,
     IntakeQuestion,
     IntakeQuestionId,
     IntakeResponseAndFollowUps,
     Intervention,
     InterventionCategory,
@@ -48,14 +49,15 @@
     "EncounterExternalIdUniquenessError",
     "EncounterExternalIdUniquenessErrorType",
     "EncounterGuarantorMissingContactInfoError",
     "EncounterGuarantorMissingContactInfoErrorType",
     "EncounterOwnerOfNextActionType",
     "EncounterPage",
     "EncounterSortOptions",
+    "EncounterSubmissionOriginType",
     "IntakeFollowUp",
     "IntakeFollowUpId",
     "IntakeQuestion",
     "IntakeQuestionId",
     "IntakeResponseAndFollowUps",
     "Intervention",
     "InterventionCategory",
```

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/client.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .encounter import Encounter
 from .encounter_base import EncounterBase
 from .encounter_external_id_uniqueness_error_type import EncounterExternalIdUniquenessErrorType
 from .encounter_guarantor_missing_contact_info_error_type import EncounterGuarantorMissingContactInfoErrorType
 from .encounter_owner_of_next_action_type import EncounterOwnerOfNextActionType
 from .encounter_page import EncounterPage
 from .encounter_sort_options import EncounterSortOptions
+from .encounter_submission_origin_type import EncounterSubmissionOriginType
 from .intake_follow_up import IntakeFollowUp
 from .intake_follow_up_id import IntakeFollowUpId
 from .intake_question import IntakeQuestion
 from .intake_question_id import IntakeQuestionId
 from .intake_response_and_follow_ups import IntakeResponseAndFollowUps
 from .intervention import Intervention
 from .intervention_category import InterventionCategory
@@ -42,14 +43,15 @@
     "Encounter",
     "EncounterBase",
     "EncounterExternalIdUniquenessErrorType",
     "EncounterGuarantorMissingContactInfoErrorType",
     "EncounterOwnerOfNextActionType",
     "EncounterPage",
     "EncounterSortOptions",
+    "EncounterSubmissionOriginType",
     "IntakeFollowUp",
     "IntakeFollowUpId",
     "IntakeQuestion",
     "IntakeQuestionId",
     "IntakeResponseAndFollowUps",
     "Intervention",
     "InterventionCategory",
```

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/billable_status_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/billable_status_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/cash_pay_payer_error_message.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/cash_pay_payer_error_message.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .....patient_payments.resources.v_3.types.patient_payment import PatientPayment
 from .....service_facility.types.encounter_service_facility import EncounterServiceFacility
 from .....tags.types.tag import Tag
 from .clinical_note_category import ClinicalNoteCategory
 from .coding_attribution_type import CodingAttributionType
 from .encounter_base import EncounterBase
 from .encounter_owner_of_next_action_type import EncounterOwnerOfNextActionType
+from .encounter_submission_origin_type import EncounterSubmissionOriginType
 from .patient_history_category import PatientHistoryCategory
 
 
 class Encounter(EncounterBase):
     encounter_id: EncounterId
     claims: typing.List[Claim]
     patient: Patient = pydantic.Field(
@@ -95,14 +96,21 @@
         description="The entity that performed the coding of medical services for the claim."
     )
     work_queue_id: typing.Optional[WorkQueueId]
     work_queue_membership_activated_at: typing.Optional[dt.datetime]
     owner_of_next_action: EncounterOwnerOfNextActionType = pydantic.Field(
         description="The party who is responsible for taking the next action on an Encounter, as defined by ownership of open Tasks."
     )
+    submission_origin: EncounterSubmissionOriginType = pydantic.Field(
+        description=(
+            "The party who originally submitted the Claim.\n"
+            "For Claims originating in Candid, this will be EncounterSubmissionOriginType.CANDID.\n"
+            "For Encounters created with an external_claim_submission object, this will be EncounterSubmissionOriginType.EXTERNAL.\n"
+        )
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_owner_of_next_action_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_owner_of_next_action_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intervention.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/lab.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/medication.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/note_category.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/responsible_party_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/responsible_party_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/encounters/resources/v_4/types/vitals.py` & `candidhealth-0.9.0/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/era/types/era.py` & `candidhealth-0.9.0/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/era/types/era_base.py` & `candidhealth-0.9.0/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.9.0/src/candid/resources/expected_network_status/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .resources.v_1.client import AsyncV1Client, V1Client
+from .resources.v_2.client import AsyncV2Client, V2Client
 
 
 class ExpectedNetworkStatusClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.v_1 = V1Client(client_wrapper=self._client_wrapper)
+        self.v_2 = V2Client(client_wrapper=self._client_wrapper)
 
 
 class AsyncExpectedNetworkStatusClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.v_1 = AsyncV1Client(client_wrapper=self._client_wrapper)
+        self.v_2 = AsyncV2Client(client_wrapper=self._client_wrapper)
```

### Comparing `candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status.py` & `candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status_response.py` & `candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_1/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/exports/client.py` & `candidhealth-0.9.0/src/candid/resources/exports/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/client.py` & `candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/errors/__init__.py` & `candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/exports/resources/v_3/types/get_exports_response.py` & `candidhealth-0.9.0/src/candid/resources/exports/resources/v_3/types/get_exports_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/__init__.py` & `candidhealth-0.9.0/src/candid/resources/financials/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Allocation,
     AllocationCreate,
-    AllocationRecipient,
-    AllocationRecipientCreate,
-    AllocationRecipientCreate_BillingProviderById,
-    AllocationRecipientCreate_ClaimById,
-    AllocationRecipientCreate_ServiceLineById,
-    AllocationRecipient_BillingProviderId,
-    AllocationRecipient_Claim,
-    AllocationRecipient_ServiceLine,
-    RefundAllocation,
-    RefundAllocationCreate,
+    AllocationTarget,
+    AllocationTargetCreate,
+    AllocationTargetCreate_BillingProviderById,
+    AllocationTargetCreate_ClaimById,
+    AllocationTargetCreate_ServiceLineById,
+    AllocationTarget_BillingProviderId,
+    AllocationTarget_Claim,
+    AllocationTarget_ServiceLine,
     RefundReason,
 )
 
 __all__ = [
     "Allocation",
     "AllocationCreate",
-    "AllocationRecipient",
-    "AllocationRecipientCreate",
-    "AllocationRecipientCreate_BillingProviderById",
-    "AllocationRecipientCreate_ClaimById",
-    "AllocationRecipientCreate_ServiceLineById",
-    "AllocationRecipient_BillingProviderId",
-    "AllocationRecipient_Claim",
-    "AllocationRecipient_ServiceLine",
-    "RefundAllocation",
-    "RefundAllocationCreate",
+    "AllocationTarget",
+    "AllocationTargetCreate",
+    "AllocationTargetCreate_BillingProviderById",
+    "AllocationTargetCreate_ClaimById",
+    "AllocationTargetCreate_ServiceLineById",
+    "AllocationTarget_BillingProviderId",
+    "AllocationTarget_Claim",
+    "AllocationTarget_ServiceLine",
     "RefundReason",
 ]
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/allocation.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_create.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ....core.datetime_utils import serialize_datetime
-from .allocation_recipient import AllocationRecipient
-
+from .identifier_base import IdentifierBase
 
-class Allocation(pydantic.BaseModel):
-    amount_cents: int
-    recipient: AllocationRecipient
 
+class IdentifierCreate(IdentifierBase):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/allocation_create.py` & `candidhealth-0.9.0/src/candid/resources/financials/types/allocation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .allocation_recipient_create import AllocationRecipientCreate
+from .allocation_target import AllocationTarget
 
 
-class AllocationCreate(pydantic.BaseModel):
+class Allocation(pydantic.BaseModel):
     amount_cents: int
-    recipient: AllocationRecipientCreate
+    target: AllocationTarget
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/allocation_recipient.py` & `candidhealth-0.9.0/src/candid/resources/financials/types/allocation_target.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 import typing_extensions
 
 from ...commons.types.claim_id import ClaimId
 from ...commons.types.provider_id import ProviderId
 from ...commons.types.service_line_id import ServiceLineId
 
 
-class AllocationRecipient_ServiceLine(pydantic.BaseModel):
+class AllocationTarget_ServiceLine(pydantic.BaseModel):
     type: typing_extensions.Literal["service_line"]
     value: ServiceLineId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-class AllocationRecipient_Claim(pydantic.BaseModel):
+class AllocationTarget_Claim(pydantic.BaseModel):
     type: typing_extensions.Literal["claim"]
     value: ClaimId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-class AllocationRecipient_BillingProviderId(pydantic.BaseModel):
+class AllocationTarget_BillingProviderId(pydantic.BaseModel):
     type: typing_extensions.Literal["billing_provider_id"]
     value: ProviderId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-AllocationRecipient = typing.Union[
-    AllocationRecipient_ServiceLine, AllocationRecipient_Claim, AllocationRecipient_BillingProviderId
+AllocationTarget = typing.Union[
+    AllocationTarget_ServiceLine, AllocationTarget_Claim, AllocationTarget_BillingProviderId
 ]
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/allocation_recipient_create.py` & `candidhealth-0.9.0/src/candid/resources/financials/types/allocation_target_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,37 @@
 import typing_extensions
 
 from ...commons.types.claim_id import ClaimId
 from ...commons.types.provider_id import ProviderId
 from ...commons.types.service_line_id import ServiceLineId
 
 
-class AllocationRecipientCreate_ServiceLineById(pydantic.BaseModel):
+class AllocationTargetCreate_ServiceLineById(pydantic.BaseModel):
     type: typing_extensions.Literal["service_line_by_id"]
     value: ServiceLineId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-class AllocationRecipientCreate_ClaimById(pydantic.BaseModel):
+class AllocationTargetCreate_ClaimById(pydantic.BaseModel):
     type: typing_extensions.Literal["claim_by_id"]
     value: ClaimId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-class AllocationRecipientCreate_BillingProviderById(pydantic.BaseModel):
+class AllocationTargetCreate_BillingProviderById(pydantic.BaseModel):
     type: typing_extensions.Literal["billing_provider_by_id"]
     value: ProviderId
 
     class Config:
         frozen = True
         smart_union = True
 
 
-AllocationRecipientCreate = typing.Union[
-    AllocationRecipientCreate_ServiceLineById,
-    AllocationRecipientCreate_ClaimById,
-    AllocationRecipientCreate_BillingProviderById,
+AllocationTargetCreate = typing.Union[
+    AllocationTargetCreate_ServiceLineById, AllocationTargetCreate_ClaimById, AllocationTargetCreate_BillingProviderById
 ]
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/refund_allocation.py` & `candidhealth-0.9.0/src/candid/resources/financials/types/allocation_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .allocation import Allocation
-from .refund_reason import RefundReason
+from .allocation_target_create import AllocationTargetCreate
 
 
-class RefundAllocation(pydantic.BaseModel):
-    allocation: Allocation
-    refund_reason: typing.Optional[RefundReason]
+class AllocationCreate(pydantic.BaseModel):
+    amount_cents: int
+    target: AllocationTargetCreate
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/financials/types/refund_allocation_create.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/medicaid_provider_identifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .allocation_create import AllocationCreate
-from .refund_reason import RefundReason
+from ...commons.types.state import State
 
 
-class RefundAllocationCreate(pydantic.BaseModel):
-    allocation: AllocationCreate
-    refund_reason: typing.Optional[RefundReason]
+class MedicaidProviderIdentifier(pydantic.BaseModel):
+    state: State
+    provider_number: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/client.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py` & `candidhealth-0.9.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/__init__.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_base.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_create.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/subscriber_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .identifier_base import IdentifierBase
+from ...insurance_card.types.insurance_card_create import InsuranceCardCreate
+from .subscriber_base import SubscriberBase
 
 
-class IdentifierCreate(IdentifierBase):
+class SubscriberCreate(SubscriberBase):
+    insurance_card: InsuranceCardCreate
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_update.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_update.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/identifier_value.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/identifier_value.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/medicaid_provider_identifier.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/medicare_provider_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...commons.types.state import State
 
 
-class MedicaidProviderIdentifier(pydantic.BaseModel):
+class MedicareProviderIdentifier(pydantic.BaseModel):
     state: State
     provider_number: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/medicare_provider_identifier.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/remittance_advice_remark_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.state import State
+from ......core.datetime_utils import serialize_datetime
+from .....x_12.resources.v_1.types.rarc import Rarc
 
 
-class MedicareProviderIdentifier(pydantic.BaseModel):
-    state: State
-    provider_number: str
+class RemittanceAdviceRemarkCode(pydantic.BaseModel):
+    reason_code: Rarc
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/identifiers/types/updatable_identifier.py` & `candidhealth-0.9.0/src/candid/resources/identifiers/types/updatable_identifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/gender.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/patient.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/patient.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/patient_base.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/patient_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/patient_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.9.0/src/candid/resources/individual/types/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_page_v_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...insurance_card.types.insurance_card_create import InsuranceCardCreate
-from .subscriber_base import SubscriberBase
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.resource_page import ResourcePage
+from .organization_provider_v_2 import OrganizationProviderV2
 
 
-class SubscriberCreate(SubscriberBase):
-    insurance_card: InsuranceCardCreate
+class OrganizationProviderPageV2(ResourcePage):
+    items: typing.List[OrganizationProviderV2]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/client.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .resources.v_1.client import AsyncV1Client, V1Client
 
 
-class InsuranceAdjudicationClient:
+class InsuranceAdjudicationsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.v_1 = V1Client(client_wrapper=self._client_wrapper)
 
 
-class AsyncInsuranceAdjudicationClient:
+class AsyncInsuranceAdjudicationsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.v_1 = AsyncV1Client(client_wrapper=self._client_wrapper)
```

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/__init__.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         Parameters:
             - insurance_adjudication_id: InsuranceAdjudicationId.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v4/{insurance_adjudication_id}"
+                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v1/{insurance_adjudication_id}"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -51,15 +51,15 @@
         Creates a new insurance adjudication record and returns the newly created InsuranceAdjudication object.
 
         Parameters:
             - request: InsuranceAdjudicationCreate.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/insurance-adjudications/v4"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/insurance-adjudications/v1"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -75,15 +75,15 @@
 
         Parameters:
             - insurance_adjudication_id: InsuranceAdjudicationId.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v4/{insurance_adjudication_id}"
+                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v1/{insurance_adjudication_id}"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -104,15 +104,15 @@
 
         Parameters:
             - insurance_adjudication_id: InsuranceAdjudicationId.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v4/{insurance_adjudication_id}"
+                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v1/{insurance_adjudication_id}"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -127,15 +127,15 @@
         Creates a new insurance adjudication record and returns the newly created InsuranceAdjudication object.
 
         Parameters:
             - request: InsuranceAdjudicationCreate.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/insurance-adjudications/v4"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/insurance-adjudications/v1"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -151,15 +151,15 @@
 
         Parameters:
             - insurance_adjudication_id: InsuranceAdjudicationId.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v4/{insurance_adjudication_id}"
+                f"{self._client_wrapper.get_base_url()}/", f"api/insurance-adjudications/v1/{insurance_adjudication_id}"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
```

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjudication.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjudication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjudication_create.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjudication_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/claim_adjustment_reason_code.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/claim_adjustment_reason_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/insurance_adjudication.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/insurance_adjudication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/insurance_adjudication_create.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/insurance_adjudication_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/remittance_advice_remark_code.py` & `candidhealth-0.9.0/src/candid/resources/commons/types/organization_not_authorized_error_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....x_12.resources.v_1.types.rarc import Rarc
+from ....core.datetime_utils import serialize_datetime
 
 
-class RemittanceAdviceRemarkCode(pydantic.BaseModel):
-    reason_code: Rarc
+class OrganizationNotAuthorizedErrorMessage(pydantic.BaseModel):
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/service_line_adjudication.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/service_line_adjudication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_adjudication/resources/v_1/types/service_line_adjudication_create.py` & `candidhealth-0.9.0/src/candid/resources/insurance_adjudications/resources/v_1/types/service_line_adjudication_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.9.0/src/candid/resources/insurance_card/types/insurance_card_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_refunds/client.py` & `candidhealth-0.9.0/src/candid/resources/insurance_refunds/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund.py` & `candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....financials.types.refund_allocation import RefundAllocation
+from .....financials.types.allocation import Allocation
+from .....financials.types.refund_reason import RefundReason
 from .insurance_refund_id import InsuranceRefundId
 
 
 class InsuranceRefund(pydantic.BaseModel):
     insurance_refund_id: InsuranceRefundId
     amount_cents: int
     refund_timestamp: typing.Optional[dt.datetime]
     refund_note: typing.Optional[str]
-    refund_allocations: typing.List[RefundAllocation]
+    allocations: typing.List[Allocation]
+    refund_reason: typing.Optional[RefundReason]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_create.py` & `candidhealth-0.9.0/src/candid/resources/insurance_refunds/resources/v_1/types/insurance_refund_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....financials.types.refund_allocation_create import RefundAllocationCreate
+from .....financials.types.allocation_create import AllocationCreate
+from .....financials.types.refund_reason import RefundReason
 
 
 class InsuranceRefundCreate(pydantic.BaseModel):
     amount_cents: int
     refund_timestamp: typing.Optional[dt.datetime]
     refund_note: typing.Optional[str]
-    refund_allocations: typing.List[RefundAllocationCreate]
+    allocations: typing.List[AllocationCreate]
+    refund_reason: typing.Optional[RefundReason]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.9.0/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.9.0/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.9.0/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/client.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_sort_options.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/client.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_create_v_2.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_create_v_2.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_page_v_2.py` & `candidhealth-0.9.0/src/candid/resources/expected_network_status/resources/v_2/types/out_of_network_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ......core.datetime_utils import serialize_datetime
-from .....commons.types.resource_page import ResourcePage
-from .organization_provider_v_2 import OrganizationProviderV2
+from .....organization_providers.resources.v_2.types.organization_provider_id import OrganizationProviderId
+from .....payers.resources.v_3.types.payer_uuid import PayerUuid
 
 
-class OrganizationProviderPageV2(ResourcePage):
-    items: typing.List[OrganizationProviderV2]
+class OutOfNetworkStatus(pydantic.BaseModel):
+    explanation: str
+    routed_payer_uuid: PayerUuid
+    routed_billing_provider_id: OrganizationProviderId
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_update_v_2.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_update_v_2.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_v_2.py` & `candidhealth-0.9.0/src/candid/resources/organization_providers/resources/v_3/types/organization_provider_v_2.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/client.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/__init__.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/client.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_create.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_page.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_update.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/organization_service_facility_update.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_mode.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_mode.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_operational_status.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_operational_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_physical_type.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_physical_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_status.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_type.py` & `candidhealth-0.9.0/src/candid/resources/organization_service_facilities/resources/v_2/types/service_facility_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/client.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/client.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from ....commons.types.invoice_id import InvoiceId
 from ....commons.types.patient_external_id import PatientExternalId
-from ....financials.types.allocation import Allocation
+from ....financials.types.allocation_create import AllocationCreate
 from .types.patient_payment import PatientPayment
 from .types.patient_payment_id import PatientPaymentId
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -50,16 +50,16 @@
 
     def create(
         self,
         *,
         amount_cents: int,
         payment_timestamp: typing.Optional[dt.datetime] = OMIT,
         payment_note: typing.Optional[str] = OMIT,
-        patient_external_id: typing.Optional[PatientExternalId] = OMIT,
-        allocations: typing.List[Allocation],
+        patient_external_id: PatientExternalId,
+        allocations: typing.List[AllocationCreate],
         invoice: typing.Optional[InvoiceId] = OMIT,
     ) -> PatientPayment:
         """
         **This endpoint is incubating.**
         Creates a new patient payment record and returns the newly created PatientPayment object.
         The allocations can describe whether the payment is being applied toward a specific service line,
         claim, or billing provider.
@@ -67,27 +67,29 @@
         Parameters:
             - amount_cents: int.
 
             - payment_timestamp: typing.Optional[dt.datetime].
 
             - payment_note: typing.Optional[str].
 
-            - patient_external_id: typing.Optional[PatientExternalId].
+            - patient_external_id: PatientExternalId.
 
-            - allocations: typing.List[Allocation].
+            - allocations: typing.List[AllocationCreate].
 
             - invoice: typing.Optional[InvoiceId].
         """
-        _request: typing.Dict[str, typing.Any] = {"amount_cents": amount_cents, "allocations": allocations}
+        _request: typing.Dict[str, typing.Any] = {
+            "amount_cents": amount_cents,
+            "patient_external_id": patient_external_id,
+            "allocations": allocations,
+        }
         if payment_timestamp is not OMIT:
             _request["payment_timestamp"] = payment_timestamp
         if payment_note is not OMIT:
             _request["payment_note"] = payment_note
-        if patient_external_id is not OMIT:
-            _request["patient_external_id"] = patient_external_id
         if invoice is not OMIT:
             _request["invoice"] = invoice
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/patient-payments/v4"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -156,16 +158,16 @@
 
     async def create(
         self,
         *,
         amount_cents: int,
         payment_timestamp: typing.Optional[dt.datetime] = OMIT,
         payment_note: typing.Optional[str] = OMIT,
-        patient_external_id: typing.Optional[PatientExternalId] = OMIT,
-        allocations: typing.List[Allocation],
+        patient_external_id: PatientExternalId,
+        allocations: typing.List[AllocationCreate],
         invoice: typing.Optional[InvoiceId] = OMIT,
     ) -> PatientPayment:
         """
         **This endpoint is incubating.**
         Creates a new patient payment record and returns the newly created PatientPayment object.
         The allocations can describe whether the payment is being applied toward a specific service line,
         claim, or billing provider.
@@ -173,27 +175,29 @@
         Parameters:
             - amount_cents: int.
 
             - payment_timestamp: typing.Optional[dt.datetime].
 
             - payment_note: typing.Optional[str].
 
-            - patient_external_id: typing.Optional[PatientExternalId].
+            - patient_external_id: PatientExternalId.
 
-            - allocations: typing.List[Allocation].
+            - allocations: typing.List[AllocationCreate].
 
             - invoice: typing.Optional[InvoiceId].
         """
-        _request: typing.Dict[str, typing.Any] = {"amount_cents": amount_cents, "allocations": allocations}
+        _request: typing.Dict[str, typing.Any] = {
+            "amount_cents": amount_cents,
+            "patient_external_id": patient_external_id,
+            "allocations": allocations,
+        }
         if payment_timestamp is not OMIT:
             _request["payment_timestamp"] = payment_timestamp
         if payment_note is not OMIT:
             _request["payment_note"] = payment_note
-        if patient_external_id is not OMIT:
-            _request["patient_external_id"] = patient_external_id
         if invoice is not OMIT:
             _request["invoice"] = invoice
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/patient-payments/v4"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment.py` & `candidhealth-0.9.0/src/candid/resources/patient_payments/resources/v_4/types/patient_payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
 from .....commons.types.invoice_id import InvoiceId
 from .....commons.types.organization_id import OrganizationId
+from .....commons.types.patient_external_id import PatientExternalId
 from .....financials.types.allocation import Allocation
 from .patient_payment_id import PatientPaymentId
 
 
 class PatientPayment(pydantic.BaseModel):
     patient_payment_id: PatientPaymentId
     organization_id: OrganizationId
     source_internal_id: str
     amount_cents: int
+    patient_external_id: PatientExternalId
     payment_timestamp: typing.Optional[dt.datetime]
     payment_note: typing.Optional[str]
     allocations: typing.List[Allocation]
     invoice: typing.Optional[InvoiceId]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_refunds/client.py` & `candidhealth-0.9.0/src/candid/resources/patient_refunds/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from ....commons.types.invoice_id import InvoiceId
 from ....commons.types.patient_external_id import PatientExternalId
-from ....financials.types.refund_allocation import RefundAllocation
+from ....financials.types.allocation_create import AllocationCreate
+from ....financials.types.refund_reason import RefundReason
 from .types.patient_refund import PatientRefund
 from .types.patient_refund_id import PatientRefundId
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -50,46 +51,53 @@
 
     def create(
         self,
         *,
         amount_cents: int,
         refund_timestamp: typing.Optional[dt.datetime] = OMIT,
         refund_note: typing.Optional[str] = OMIT,
-        patient_external_id: typing.Optional[PatientExternalId] = OMIT,
-        allocations: typing.List[RefundAllocation],
+        patient_external_id: PatientExternalId,
+        allocations: typing.List[AllocationCreate],
         invoice: typing.Optional[InvoiceId] = OMIT,
+        refund_reason: typing.Optional[RefundReason] = OMIT,
     ) -> PatientRefund:
         """
         **This endpoint is incubating.**
         Creates a new patient refund record and returns the newly created PatientRefund object.
         The allocations can describe whether the refund is being applied toward a specific service line,
         claim, or billing provider.
 
         Parameters:
             - amount_cents: int.
 
             - refund_timestamp: typing.Optional[dt.datetime].
 
             - refund_note: typing.Optional[str].
 
-            - patient_external_id: typing.Optional[PatientExternalId].
+            - patient_external_id: PatientExternalId.
 
-            - allocations: typing.List[RefundAllocation].
+            - allocations: typing.List[AllocationCreate].
 
             - invoice: typing.Optional[InvoiceId].
+
+            - refund_reason: typing.Optional[RefundReason].
         """
-        _request: typing.Dict[str, typing.Any] = {"amount_cents": amount_cents, "allocations": allocations}
+        _request: typing.Dict[str, typing.Any] = {
+            "amount_cents": amount_cents,
+            "patient_external_id": patient_external_id,
+            "allocations": allocations,
+        }
         if refund_timestamp is not OMIT:
             _request["refund_timestamp"] = refund_timestamp
         if refund_note is not OMIT:
             _request["refund_note"] = refund_note
-        if patient_external_id is not OMIT:
-            _request["patient_external_id"] = patient_external_id
         if invoice is not OMIT:
             _request["invoice"] = invoice
+        if refund_reason is not OMIT:
+            _request["refund_reason"] = refund_reason
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/patient-refunds/v1"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -156,46 +164,53 @@
 
     async def create(
         self,
         *,
         amount_cents: int,
         refund_timestamp: typing.Optional[dt.datetime] = OMIT,
         refund_note: typing.Optional[str] = OMIT,
-        patient_external_id: typing.Optional[PatientExternalId] = OMIT,
-        allocations: typing.List[RefundAllocation],
+        patient_external_id: PatientExternalId,
+        allocations: typing.List[AllocationCreate],
         invoice: typing.Optional[InvoiceId] = OMIT,
+        refund_reason: typing.Optional[RefundReason] = OMIT,
     ) -> PatientRefund:
         """
         **This endpoint is incubating.**
         Creates a new patient refund record and returns the newly created PatientRefund object.
         The allocations can describe whether the refund is being applied toward a specific service line,
         claim, or billing provider.
 
         Parameters:
             - amount_cents: int.
 
             - refund_timestamp: typing.Optional[dt.datetime].
 
             - refund_note: typing.Optional[str].
 
-            - patient_external_id: typing.Optional[PatientExternalId].
+            - patient_external_id: PatientExternalId.
 
-            - allocations: typing.List[RefundAllocation].
+            - allocations: typing.List[AllocationCreate].
 
             - invoice: typing.Optional[InvoiceId].
+
+            - refund_reason: typing.Optional[RefundReason].
         """
-        _request: typing.Dict[str, typing.Any] = {"amount_cents": amount_cents, "allocations": allocations}
+        _request: typing.Dict[str, typing.Any] = {
+            "amount_cents": amount_cents,
+            "patient_external_id": patient_external_id,
+            "allocations": allocations,
+        }
         if refund_timestamp is not OMIT:
             _request["refund_timestamp"] = refund_timestamp
         if refund_note is not OMIT:
             _request["refund_note"] = refund_note
-        if patient_external_id is not OMIT:
-            _request["patient_external_id"] = patient_external_id
         if invoice is not OMIT:
             _request["invoice"] = invoice
+        if refund_reason is not OMIT:
+            _request["refund_reason"] = refund_reason
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/patient-refunds/v1"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
```

### Comparing `candidhealth-0.8.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund.py` & `candidhealth-0.9.0/src/candid/resources/patient_refunds/resources/v_1/types/patient_refund.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
 from .....commons.types.invoice_id import InvoiceId
 from .....commons.types.organization_id import OrganizationId
+from .....commons.types.patient_external_id import PatientExternalId
 from .....financials.types.allocation import Allocation
+from .....financials.types.refund_reason import RefundReason
 from .patient_refund_id import PatientRefundId
 
 
 class PatientRefund(pydantic.BaseModel):
     patient_refund_id: PatientRefundId
     organization_id: OrganizationId
     source_internal_id: str
     amount_cents: int
+    patient_external_id: PatientExternalId
     refund_timestamp: typing.Optional[dt.datetime]
     refund_note: typing.Optional[str]
     allocations: typing.List[Allocation]
     invoice: typing.Optional[InvoiceId]
+    refund_reason: typing.Optional[RefundReason]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/payers/client.py` & `candidhealth-0.9.0/src/candid/resources/payers/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/client.py` & `candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/payer.py` & `candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/payer.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/payers/resources/v_3/types/payer_page.py` & `candidhealth-0.9.0/src/candid/resources/payers/resources/v_3/types/payer_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.9.0/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.9.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/__init__.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/__init__.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/denial_reason_content.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/drug_identification.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/drug_identification.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/measurement_unit_code.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_id_qualifier.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_adjustment.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_create.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_denial_reason.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_denial_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/service_lines/resources/v_2/types/service_line_era_data.py` & `candidhealth-0.9.0/src/candid/resources/service_lines/resources/v_2/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/tags/types/tag.py` & `candidhealth-0.9.0/src/candid/resources/tags/types/tag.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.9.0/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.9.0/src/candid/resources/tags/types/tag_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/write_offs/client.py` & `candidhealth-0.9.0/src/candid/resources/write_offs/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/client.py` & `candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off.py` & `candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off_create.py` & `candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....financials.types.allocation import Allocation
+from .....financials.types.allocation_create import AllocationCreate
 from .write_off_reason import WriteOffReason
 
 
 class WriteOffCreate(pydantic.BaseModel):
     write_off_timestamp: dt.datetime
     write_off_note: typing.Optional[str]
     write_off_reason: WriteOffReason
-    allocation: Allocation
+    allocation: AllocationCreate
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.8.0/src/candid/resources/write_offs/resources/v_1/types/write_off_reason.py` & `candidhealth-0.9.0/src/candid/resources/write_offs/resources/v_1/types/write_off_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/types/carc.py` & `candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/types/carc.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,16 @@
     CARC_235 = "235"
     CARC_236 = "236"
     CARC_237 = "237"
     CARC_238 = "238"
     CARC_239 = "239"
     CARC_240 = "240"
     CARC_241 = "241"
+    CARC_242 = "242"
+    CARC_243 = "243"
     CARC_245 = "245"
     CARC_246 = "246"
     CARC_247 = "247"
     CARC_248 = "248"
     CARC_249 = "249"
     CARC_250 = "250"
     CARC_251 = "251"
@@ -241,14 +243,16 @@
     CARC_297 = "297"
     CARC_298 = "298"
     CARC_299 = "299"
     CARC_300 = "300"
     CARC_301 = "301"
     CARC_302 = "302"
     CARC_303 = "303"
+    CARC_304 = "304"
+    CARC_305 = "305"
     CARC_A_0 = "A0"
     CARC_A_1 = "A1"
     CARC_A_5 = "A5"
     CARC_A_6 = "A6"
     CARC_A_8 = "A8"
     CARC_B_1 = "B1"
     CARC_B_4 = "B4"
@@ -261,22 +265,46 @@
     CARC_B_13 = "B13"
     CARC_B_14 = "B14"
     CARC_B_15 = "B15"
     CARC_B_16 = "B16"
     CARC_B_20 = "B20"
     CARC_B_22 = "B22"
     CARC_B_23 = "B23"
+    CARC_P_1 = "P1"
+    CARC_P_2 = "P2"
+    CARC_P_3 = "P3"
+    CARC_P_4 = "P4"
+    CARC_P_5 = "P5"
+    CARC_P_6 = "P6"
+    CARC_P_7 = "P7"
+    CARC_P_8 = "P8"
+    CARC_P_9 = "P9"
+    CARC_P_10 = "P10"
+    CARC_P_11 = "P11"
+    CARC_P_12 = "P12"
+    CARC_P_13 = "P13"
+    CARC_P_14 = "P14"
+    CARC_P_15 = "P15"
+    CARC_P_16 = "P16"
+    CARC_P_17 = "P17"
+    CARC_P_18 = "P18"
+    CARC_P_19 = "P19"
+    CARC_P_20 = "P20"
+    CARC_P_21 = "P21"
+    CARC_P_22 = "P22"
+    CARC_P_23 = "P23"
     CARC_P_24 = "P24"
     CARC_P_25 = "P25"
     CARC_P_26 = "P26"
     CARC_P_27 = "P27"
     CARC_P_28 = "P28"
     CARC_P_29 = "P29"
     CARC_P_30 = "P30"
     CARC_P_31 = "P31"
+    CARC_P_32 = "P32"
 
     def visit(
         self,
         carc_1: typing.Callable[[], T_Result],
         carc_2: typing.Callable[[], T_Result],
         carc_3: typing.Callable[[], T_Result],
         carc_4: typing.Callable[[], T_Result],
@@ -452,14 +480,16 @@
         carc_235: typing.Callable[[], T_Result],
         carc_236: typing.Callable[[], T_Result],
         carc_237: typing.Callable[[], T_Result],
         carc_238: typing.Callable[[], T_Result],
         carc_239: typing.Callable[[], T_Result],
         carc_240: typing.Callable[[], T_Result],
         carc_241: typing.Callable[[], T_Result],
+        carc_242: typing.Callable[[], T_Result],
+        carc_243: typing.Callable[[], T_Result],
         carc_245: typing.Callable[[], T_Result],
         carc_246: typing.Callable[[], T_Result],
         carc_247: typing.Callable[[], T_Result],
         carc_248: typing.Callable[[], T_Result],
         carc_249: typing.Callable[[], T_Result],
         carc_250: typing.Callable[[], T_Result],
         carc_251: typing.Callable[[], T_Result],
@@ -510,14 +540,16 @@
         carc_297: typing.Callable[[], T_Result],
         carc_298: typing.Callable[[], T_Result],
         carc_299: typing.Callable[[], T_Result],
         carc_300: typing.Callable[[], T_Result],
         carc_301: typing.Callable[[], T_Result],
         carc_302: typing.Callable[[], T_Result],
         carc_303: typing.Callable[[], T_Result],
+        carc_304: typing.Callable[[], T_Result],
+        carc_305: typing.Callable[[], T_Result],
         carc_a_0: typing.Callable[[], T_Result],
         carc_a_1: typing.Callable[[], T_Result],
         carc_a_5: typing.Callable[[], T_Result],
         carc_a_6: typing.Callable[[], T_Result],
         carc_a_8: typing.Callable[[], T_Result],
         carc_b_1: typing.Callable[[], T_Result],
         carc_b_4: typing.Callable[[], T_Result],
@@ -530,22 +562,46 @@
         carc_b_13: typing.Callable[[], T_Result],
         carc_b_14: typing.Callable[[], T_Result],
         carc_b_15: typing.Callable[[], T_Result],
         carc_b_16: typing.Callable[[], T_Result],
         carc_b_20: typing.Callable[[], T_Result],
         carc_b_22: typing.Callable[[], T_Result],
         carc_b_23: typing.Callable[[], T_Result],
+        carc_p_1: typing.Callable[[], T_Result],
+        carc_p_2: typing.Callable[[], T_Result],
+        carc_p_3: typing.Callable[[], T_Result],
+        carc_p_4: typing.Callable[[], T_Result],
+        carc_p_5: typing.Callable[[], T_Result],
+        carc_p_6: typing.Callable[[], T_Result],
+        carc_p_7: typing.Callable[[], T_Result],
+        carc_p_8: typing.Callable[[], T_Result],
+        carc_p_9: typing.Callable[[], T_Result],
+        carc_p_10: typing.Callable[[], T_Result],
+        carc_p_11: typing.Callable[[], T_Result],
+        carc_p_12: typing.Callable[[], T_Result],
+        carc_p_13: typing.Callable[[], T_Result],
+        carc_p_14: typing.Callable[[], T_Result],
+        carc_p_15: typing.Callable[[], T_Result],
+        carc_p_16: typing.Callable[[], T_Result],
+        carc_p_17: typing.Callable[[], T_Result],
+        carc_p_18: typing.Callable[[], T_Result],
+        carc_p_19: typing.Callable[[], T_Result],
+        carc_p_20: typing.Callable[[], T_Result],
+        carc_p_21: typing.Callable[[], T_Result],
+        carc_p_22: typing.Callable[[], T_Result],
+        carc_p_23: typing.Callable[[], T_Result],
         carc_p_24: typing.Callable[[], T_Result],
         carc_p_25: typing.Callable[[], T_Result],
         carc_p_26: typing.Callable[[], T_Result],
         carc_p_27: typing.Callable[[], T_Result],
         carc_p_28: typing.Callable[[], T_Result],
         carc_p_29: typing.Callable[[], T_Result],
         carc_p_30: typing.Callable[[], T_Result],
         carc_p_31: typing.Callable[[], T_Result],
+        carc_p_32: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is Carc.CARC_1:
             return carc_1()
         if self is Carc.CARC_2:
             return carc_2()
         if self is Carc.CARC_3:
             return carc_3()
@@ -899,14 +955,18 @@
             return carc_238()
         if self is Carc.CARC_239:
             return carc_239()
         if self is Carc.CARC_240:
             return carc_240()
         if self is Carc.CARC_241:
             return carc_241()
+        if self is Carc.CARC_242:
+            return carc_242()
+        if self is Carc.CARC_243:
+            return carc_243()
         if self is Carc.CARC_245:
             return carc_245()
         if self is Carc.CARC_246:
             return carc_246()
         if self is Carc.CARC_247:
             return carc_247()
         if self is Carc.CARC_248:
@@ -1015,14 +1075,18 @@
             return carc_300()
         if self is Carc.CARC_301:
             return carc_301()
         if self is Carc.CARC_302:
             return carc_302()
         if self is Carc.CARC_303:
             return carc_303()
+        if self is Carc.CARC_304:
+            return carc_304()
+        if self is Carc.CARC_305:
+            return carc_305()
         if self is Carc.CARC_A_0:
             return carc_a_0()
         if self is Carc.CARC_A_1:
             return carc_a_1()
         if self is Carc.CARC_A_5:
             return carc_a_5()
         if self is Carc.CARC_A_6:
@@ -1055,14 +1119,60 @@
             return carc_b_16()
         if self is Carc.CARC_B_20:
             return carc_b_20()
         if self is Carc.CARC_B_22:
             return carc_b_22()
         if self is Carc.CARC_B_23:
             return carc_b_23()
+        if self is Carc.CARC_P_1:
+            return carc_p_1()
+        if self is Carc.CARC_P_2:
+            return carc_p_2()
+        if self is Carc.CARC_P_3:
+            return carc_p_3()
+        if self is Carc.CARC_P_4:
+            return carc_p_4()
+        if self is Carc.CARC_P_5:
+            return carc_p_5()
+        if self is Carc.CARC_P_6:
+            return carc_p_6()
+        if self is Carc.CARC_P_7:
+            return carc_p_7()
+        if self is Carc.CARC_P_8:
+            return carc_p_8()
+        if self is Carc.CARC_P_9:
+            return carc_p_9()
+        if self is Carc.CARC_P_10:
+            return carc_p_10()
+        if self is Carc.CARC_P_11:
+            return carc_p_11()
+        if self is Carc.CARC_P_12:
+            return carc_p_12()
+        if self is Carc.CARC_P_13:
+            return carc_p_13()
+        if self is Carc.CARC_P_14:
+            return carc_p_14()
+        if self is Carc.CARC_P_15:
+            return carc_p_15()
+        if self is Carc.CARC_P_16:
+            return carc_p_16()
+        if self is Carc.CARC_P_17:
+            return carc_p_17()
+        if self is Carc.CARC_P_18:
+            return carc_p_18()
+        if self is Carc.CARC_P_19:
+            return carc_p_19()
+        if self is Carc.CARC_P_20:
+            return carc_p_20()
+        if self is Carc.CARC_P_21:
+            return carc_p_21()
+        if self is Carc.CARC_P_22:
+            return carc_p_22()
+        if self is Carc.CARC_P_23:
+            return carc_p_23()
         if self is Carc.CARC_P_24:
             return carc_p_24()
         if self is Carc.CARC_P_25:
             return carc_p_25()
         if self is Carc.CARC_P_26:
             return carc_p_26()
         if self is Carc.CARC_P_27:
@@ -1071,7 +1181,9 @@
             return carc_p_28()
         if self is Carc.CARC_P_29:
             return carc_p_29()
         if self is Carc.CARC_P_30:
             return carc_p_30()
         if self is Carc.CARC_P_31:
             return carc_p_31()
+        if self is Carc.CARC_P_32:
+            return carc_p_32()
```

### Comparing `candidhealth-0.8.0/src/candid/resources/x_12/resources/v_1/types/rarc.py` & `candidhealth-0.9.0/src/candid/resources/x_12/resources/v_1/types/rarc.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.8.0/PKG-INFO` & `candidhealth-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candidhealth
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

