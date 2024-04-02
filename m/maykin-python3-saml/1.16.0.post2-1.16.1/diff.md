# Comparing `tmp/maykin_python3_saml-1.16.0.post2.tar.gz` & `tmp/maykin_python3_saml-1.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maykin_python3_saml-1.16.0.post2.tar", max compression
+gzip compressed data, was "maykin_python3_saml-1.16.1.tar", max compression
```

## Comparing `maykin_python3_saml-1.16.0.post2.tar` & `maykin_python3_saml-1.16.1.tar`

### file list

```diff
@@ -1,219 +1,219 @@
--rw-r--r--   0        0        0     1109 2024-02-15 10:00:22.620516 maykin_python3_saml-1.16.0.post2/LICENSE
--rw-r--r--   0        0        0    78329 2024-02-22 11:19:28.641669 maykin_python3_saml-1.16.0.post2/README.md
--rw-r--r--   0        0        0     4813 2024-02-23 08:59:58.401940 maykin_python3_saml-1.16.0.post2/pyproject.toml
--rw-r--r--   0        0        0      557 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/src/onelogin/__init__.py
--rw-r--r--   0        0        0      557 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/__init__.py
--rw-r--r--   0        0        0     4003 2024-02-22 11:19:28.641669 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/artifact_resolve.py
--rw-r--r--   0        0        0     6998 2024-02-22 11:19:28.641669 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/artifact_response.py
--rw-r--r--   0        0        0    34302 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/auth.py
--rw-r--r--   0        0        0     6782 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/authn_request.py
--rw-r--r--   0        0        0     1434 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/compat.py
--rw-r--r--   0        0        0     5215 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/constants.py
--rw-r--r--   0        0        0      330 2024-02-22 11:19:32.295022 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/crypto_utils.py
--rw-r--r--   0        0        0     3654 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/errors.py
--rw-r--r--   0        0        0    12654 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/idp_metadata_parser.py
--rw-r--r--   0        0        0    13667 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/logout_request.py
--rw-r--r--   0        0        0     8515 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/logout_response.py
--rw-r--r--   0        0        0    14328 2024-02-22 11:19:32.295022 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/metadata.py
--rw-r--r--   0        0        0    48117 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/response.py
--rw-r--r--   0        0        0     5776 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-context-schema-os.xsd
--rw-r--r--   0        0        0    15230 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-policy-schema-os.xsd
--rw-r--r--   0        0        0     2386 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-assertion-schema-os.xsd
--rw-r--r--   0        0        0     2774 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-protocol-schema-os.xsd
--rw-r--r--   0        0        0    12774 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-assertion-2.0.xsd
--rw-r--r--   0        0        0      762 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-authn-context-2.0.xsd
--rw-r--r--   0        0        0    29275 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-authn-context-types-2.0.xsd
--rw-r--r--   0        0        0    15895 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-metadata-2.0.xsd
--rw-r--r--   0        0        0    13466 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-protocol-2.0.xsd
--rw-r--r--   0        0        0     1139 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-metadata-attr.xsd
--rw-r--r--   0        0        0      732 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-attribute-ext.xsd
--rw-r--r--   0        0        0     1453 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-metadata-algsupport-v1.0.xsd
--rw-r--r--   0        0        0     3098 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-metadata-ui-v1.0.xsd
--rw-r--r--   0        0        0    13093 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-schema-assertion-2.0.xsd
--rw-r--r--   0        0        0    13867 2024-02-22 11:19:28.645002 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-schema-protocol-2.0.xsd
--rw-r--r--   0        0        0     4830 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xenc-schema.xsd
--rw-r--r--   0        0        0     8836 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xml.xsd
--rw-r--r--   0        0        0    10003 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xmldsig-core-schema.xsd
--rw-r--r--   0        0        0    32462 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/settings.py
--rw-r--r--   0        0        0     6501 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/soap_logout_request.py
--rw-r--r--   0        0        0     1127 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/ssl_adapter.py
--rw-r--r--   0        0        0    40077 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/utils.py
--rw-r--r--   0        0        0     6128 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xml_templates.py
--rw-r--r--   0        0        0     7053 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xml_utils.py
--rw-r--r--   0        0        0     5818 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xmlparser.py
--rw-r--r--   0        0        0        0 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/__init__.py
--rw-r--r--   0        0        0      644 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/certs/certificate1
--rw-r--r--   0        0        0      550 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/coverage.rc
--rw-r--r--   0        0        0     3317 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/artifact_response/artifact_response.xml
--rw-r--r--   0        0        0     3323 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/artifact_response/artifact_response_invalid.xml
--rw-r--r--   0        0        0      594 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/customPath/advanced_settings.json
--rw-r--r--   0        0        0      927 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/idp.crt
--rwxr-xr-x   0        0        0      928 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/metadata.crt
--rwxr-xr-x   0        0        0      891 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/metadata.key
--rwxr-xr-x   0        0        0      928 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/sp.crt
--rwxr-xr-x   0        0        0      891 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/sp.key
--rw-r--r--   0        0        0      821 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/invalid_issuer.xml
--rw-r--r--   0        0        0      509 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/invalid_issuer.xml.base64
--rw-r--r--   0        0        0      586 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/no_nameId.xml
--rw-r--r--   0        0        0      793 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/not_after_failed.xml
--rw-r--r--   0        0        0      488 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/not_after_failed.xml.base64
--rw-r--r--   0        0        0      736 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request.xml
--rw-r--r--   0        0        0      996 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request.xml.base64
--rw-r--r--   0        0        0      472 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_deflated.xml.base64
--rw-r--r--   0        0        0     1960 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_encrypted_nameid.xml
--rw-r--r--   0        0        0      753 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_with_encoding.xml
--rw-r--r--   0        0        0      823 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_with_sessionindex.xml
--rw-r--r--   0        0        0      389 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/invalids/no_status.xml.base64
--rw-r--r--   0        0        0      433 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/invalids/status_code_responder.xml.base64
--rw-r--r--   0        0        0      701 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response.xml
--rw-r--r--   0        0        0      953 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response.xml.base64
--rw-r--r--   0        0        0      437 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response_deflated.xml.base64
--rw-r--r--   0        0        0      740 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response_with_encoding.xml
--rw-r--r--   0        0        0      473 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response_with_encoding_deflated.xml.base64
--rw-r--r--   0        0        0     6649 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/entities_metadata.xml
--rw-r--r--   0        0        0     2925 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/expired_metadata_settings1.xml
--rw-r--r--   0        0        0     2675 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata.xml
--rw-r--r--   0        0        0     2554 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata2.xml
--rw-r--r--   0        0        0     4446 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_different_sign_and_encrypt_cert.xml
--rw-r--r--   0        0        0     5259 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_multi_certs.xml
--rw-r--r--   0        0        0     5257 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_multi_signing_certs.xml
--rw-r--r--   0        0        0     4349 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_same_sign_and_encrypt_cert.xml
--rw-r--r--   0        0        0    10914 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_multiple_descriptors.xml
--rw-r--r--   0        0        0      988 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/metadata_bad_order_settings1.xml
--rw-r--r--   0        0        0      988 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/metadata_settings1.xml
--rw-r--r--   0        0        0      882 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/no_expiration_mark_metadata.xml
--rw-r--r--   0        0        0     2927 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/noentity_metadata_settings1.xml
--rw-r--r--   0        0        0     5496 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/signed_metadata_settings1.xml
--rw-r--r--   0        0        0     5127 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/signed_metadata_settings2.xml
--rw-r--r--   0        0        0    20092 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/testshib-providers.xml
--rw-r--r--   0        0        0      989 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/metadata/unparsed_metadata.xml
--rw-r--r--   0        0        0      916 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/misc/sp2.key
--rw-r--r--   0        0        0      891 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/misc/sp3.key
--rw-r--r--   0        0        0     1704 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/misc/sp4.key
--rw-r--r--   0        0        0      986 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/requests/authn_request.xml
--rw-r--r--   0        0        0     1329 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/requests/authn_request.xml.base64
--rw-r--r--   0        0        0     5526 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/adfs_response.xml.base64
--rw-r--r--   0        0        0     2843 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/decrypted_valid_encrypted_assertion.xml
--rw-r--r--   0        0        0    11829 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_encrypted_assertion.xml.base64
--rw-r--r--   0        0        0    12056 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_encrypted_assertion2.xml.base64
--rw-r--r--   0        0        0     8849 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_response.xml.base64
--rw-r--r--   0        0        0     8796 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_response2.xml.base64
--rw-r--r--   0        0        0     3996 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/expired_response.xml.base64
--rw-r--r--   0        0        0     8821 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/bad_reference.xml.base64
--rw-r--r--   0        0        0     9125 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/duplicated_attributes.xml.base64
--rw-r--r--   0        0        0     8685 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/empty_destination.xml.base64
--rw-r--r--   0        0        0     8729 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/empty_nameid.xml.base64
--rw-r--r--   0        0        0     5132 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_attrs.xml.base64
--rw-r--r--   0        0        0    10101 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_nameID_without_EncMethod.xml.base64
--rw-r--r--   0        0        0     9617 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_nameID_without_keyinfo.xml.base64
--rw-r--r--   0        0        0     2949 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_audience.xml.base64
--rw-r--r--   0        0        0     2980 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_issuer_assertion.xml.base64
--rw-r--r--   0        0        0     2984 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_issuer_message.xml.base64
--rw-r--r--   0        0        0     2964 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_sessionindex.xml.base64
--rw-r--r--   0        0        0     2940 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_inresponse.xml.base64
--rw-r--r--   0        0        0     2961 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_nb.xml.base64
--rw-r--r--   0        0        0     2964 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_noa.xml.base64
--rw-r--r--   0        0        0     2952 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_recipient.xml.base64
--rw-r--r--   0        0        0     9918 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/multiple_assertions.xml.base64
--rw-r--r--   0        0        0     6037 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_authnstatement.xml.base64
--rw-r--r--   0        0        0     6140 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_conditions.xml.base64
--rw-r--r--   0        0        0     3753 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_id.xml.base64
--rw-r--r--   0        0        0     6348 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_issuer_assertion.xml.base64
--rw-r--r--   0        0        0     6320 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_issuer_response.xml.base64
--rw-r--r--   0        0        0     3357 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_key.xml.base64
--rw-r--r--   0        0        0     2772 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_nameid.xml.base64
--rw-r--r--   0        0        0     3725 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_saml2.xml.base64
--rw-r--r--   0        0        0     2577 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_signature.xml.base64
--rw-r--r--   0        0        0     5289 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_status.xml.base64
--rw-r--r--   0        0        0     5293 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_status_code.xml.base64
--rw-r--r--   0        0        0     2728 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_subjectconfirmation_data.xml.base64
--rw-r--r--   0        0        0     2976 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_subjectconfirmation_method.xml.base64
--rw-r--r--   0        0        0     3813 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/not_after_failed.xml.base64
--rw-r--r--   0        0        0     6277 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/not_before_failed.xml.base64
--rw-r--r--   0        0        0     5132 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/response_encrypted_attrs.xml.base64
--rw-r--r--   0        0        0    10484 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signature_wrapping_attack.xml.base64
--rw-r--r--   0        0        0    10492 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signature_wrapping_attack2.xml.base64
--rw-r--r--   0        0        0     7349 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signed_assertion_response.xml.base64
--rw-r--r--   0        0        0      777 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/status_code_responder.xml.base64
--rw-r--r--   0        0        0      853 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/status_code_responer_and_msg.xml.base64
--rw-r--r--   0        0        0     6380 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/wrong_spnamequalifier.xml.base64
--rw-r--r--   0        0        0     2768 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/no_audience.xml.base64
--rw-r--r--   0        0        0     3475 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/open_saml_response.xml
--rw-r--r--   0        0        0     2844 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/pretty_decrypted_valid_encrypted_assertion.xml
--rw-r--r--   0        0        0     5087 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/pretty_signed_message_response.xml
--rw-r--r--   0        0        0     5196 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response1.xml.base64
--rw-r--r--   0        0        0     6312 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response1_with_duplicate_attributes.xml.base64
--rw-r--r--   0        0        0     5352 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response1_with_friendlyname.xml.base64
--rw-r--r--   0        0        0     4786 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response2.xml.base64
--rw-r--r--   0        0        0     3982 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response3.xml.base64
--rw-r--r--   0        0        0     5668 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response4.xml.base64
--rw-r--r--   0        0        0     6218 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response5.xml.base64
--rw-r--r--   0        0        0     5301 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/responses/response6.xml.base64
--rw-r--r--   0        0        0    10072 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_encrypted_nameid.xml.base64
--rw-r--r--   0        0        0     7136 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_node_text_attack.xml.base64
--rw-r--r--   0        0        0     8467 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_ampersands.xml
--rw-r--r--   0        0        0     5668 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_ampersands.xml.base64
--rw-r--r--   0        0        0     5472 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_nested_nameid_values.xml.base64
--rw-r--r--   0        0        0     4981 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_without_assertion_reference_uri.xml.base64
--rw-r--r--   0        0        0     4981 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/response_without_reference_uri.xml.base64
--rw-r--r--   0        0        0     6429 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_assertion_response.xml.base64
--rw-r--r--   0        0        0     6396 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_assertion_response2.xml.base64
--rw-r--r--   0        0        0     9969 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_encrypted_assertion.xml.base64
--rw-r--r--   0        0        0     9656 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_encrypted_assertion2.xml.base64
--rw-r--r--   0        0        0     8613 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_encrypted_assertion.xml.base64
--rw-r--r--   0        0        0     8840 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_encrypted_assertion2.xml.base64
--rw-r--r--   0        0        0     6461 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_response.xml.base64
--rw-r--r--   0        0        0    10605 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_response2.xml.base64
--rw-r--r--   0        0        0     4171 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/simple_saml_php.xml
--rw-r--r--   0        0        0     2125 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_assertion.xml.base64
--rw-r--r--   0        0        0     2965 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_response.xml.base64
--rw-r--r--   0        0        0     2996 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_response_with_miliseconds.xm.base64
--rw-r--r--   0        0        0     6753 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_encrypted_assertion.xml.base64
--rw-r--r--   0        0        0     8208 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_encrypted_assertion_encrypted_nameid.xml.base64
--rw-r--r--   0        0        0     8760 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response.xml.base64
--rw-r--r--   0        0        0     8797 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response2.xml.base64
--rw-r--r--   0        0        0     8756 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response_with_namequalifier.xml.base64
--rw-r--r--   0        0        0     5585 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response_without_inresponseto.xml.base64
--rw-r--r--   0        0        0     3997 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_unsigned_response.xml
--rw-r--r--   0        0        0     3997 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_unsigned_response.xml.base64
--rw-r--r--   0        0        0     9722 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/data/responses/wrapped_response_2.xml.base64
--rw-r--r--   0        0        0     1899 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request.xml
--rw-r--r--   0        0        0     1888 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_empty_id.xml
--rw-r--r--   0        0        0     1850 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_empty_nameId.xml
--rw-r--r--   0        0        0     1905 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_invalid_issuer.xml
--rw-r--r--   0        0        0     1909 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_invalid_signature.xml
--rw-r--r--   0        0        0     2077 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/pylint.rc
--rw-r--r--   0        0        0     2246 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings1.json
--rw-r--r--   0        0        0     2159 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings10.json
--rw-r--r--   0        0        0     2718 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings11.json
--rw-r--r--   0        0        0     3916 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings12.json
--rw-r--r--   0        0        0     3842 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings13.json
--rw-r--r--   0        0        0     2575 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings14.json
--rw-r--r--   0        0        0     2488 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings15.json
--rw-r--r--   0        0        0     2252 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings2.json
--rw-r--r--   0        0        0     2226 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings3.json
--rw-r--r--   0        0        0     3764 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings4.json
--rw-r--r--   0        0        0     2969 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings5.json
--rw-r--r--   0        0        0     1495 2024-02-22 11:19:28.648336 maykin_python3_saml-1.16.0.post2/tests/settings/settings6.json
--rw-r--r--   0        0        0     4798 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/settings/settings7.json
--rw-r--r--   0        0        0     5841 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/settings/settings8.json
--rw-r--r--   0        0        0     1362 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/settings/settings9.json
--rw-r--r--   0        0        0        0 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/__init__.py
--rw-r--r--   0        0        0     2710 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/artifact_resolve_request_test.py
--rw-r--r--   0        0        0     3349 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/artifact_response_test.py
--rw-r--r--   0        0        0    83627 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/auth_test.py
--rw-r--r--   0        0        0    18878 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/authn_request_test.py
--rw-r--r--   0        0        0      337 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/error_test.py
--rw-r--r--   0        0        0    54952 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/idp_metadata_parser_test.py
--rw-r--r--   0        0        0    26614 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/logout_request_test.py
--rw-r--r--   0        0        0    19455 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/logout_response_test.py
--rw-r--r--   0        0        0    19057 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/metadata_test.py
--rw-r--r--   0        0        0   109294 2024-02-22 11:19:32.295022 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/response_test.py
--rw-r--r--   0        0        0    51685 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/settings_test.py
--rw-r--r--   0        0        0     1952 2024-02-15 10:00:22.647183 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/signed_response_test.py
--rw-r--r--   0        0        0     4175 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/soap_logout_request_test.py
--rw-r--r--   0        0        0    50647 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/utils_test.py
--rw-r--r--   0        0        0     8501 2024-02-22 11:19:28.651669 maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/xml_utils_test.py
--rw-r--r--   0        0        0        0 2022-10-31 15:34:11.726435 maykin_python3_saml-1.16.0.post2/tests/src/__init__.py
--rw-r--r--   0        0        0    80280 1970-01-01 00:00:00.000000 maykin_python3_saml-1.16.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-02-15 10:00:22.620516 maykin_python3_saml-1.16.1/LICENSE
+-rw-r--r--   0        0        0    78327 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/README.md
+-rw-r--r--   0        0        0     4807 2024-04-02 10:33:29.228131 maykin_python3_saml-1.16.1/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/src/onelogin/__init__.py
+-rw-r--r--   0        0        0      557 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/src/onelogin/saml2/__init__.py
+-rw-r--r--   0        0        0     4003 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/artifact_resolve.py
+-rw-r--r--   0        0        0     6998 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/artifact_response.py
+-rw-r--r--   0        0        0    34302 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/auth.py
+-rw-r--r--   0        0        0     6782 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/authn_request.py
+-rw-r--r--   0        0        0     1434 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/src/onelogin/saml2/compat.py
+-rw-r--r--   0        0        0     5215 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/constants.py
+-rw-r--r--   0        0        0      330 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/crypto_utils.py
+-rw-r--r--   0        0        0     3654 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/errors.py
+-rw-r--r--   0        0        0    12527 2024-04-02 10:33:02.844628 maykin_python3_saml-1.16.1/src/onelogin/saml2/idp_metadata_parser.py
+-rw-r--r--   0        0        0    13667 2024-04-02 09:26:47.789428 maykin_python3_saml-1.16.1/src/onelogin/saml2/logout_request.py
+-rw-r--r--   0        0        0     8515 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/logout_response.py
+-rw-r--r--   0        0        0    14328 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/metadata.py
+-rw-r--r--   0        0        0    48117 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/response.py
+-rw-r--r--   0        0        0     5776 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-context-schema-os.xsd
+-rw-r--r--   0        0        0    15230 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-policy-schema-os.xsd
+-rw-r--r--   0        0        0     2386 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-assertion-schema-os.xsd
+-rw-r--r--   0        0        0     2774 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-protocol-schema-os.xsd
+-rw-r--r--   0        0        0    12774 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0        0        0      762 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-authn-context-2.0.xsd
+-rw-r--r--   0        0        0    29275 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-authn-context-types-2.0.xsd
+-rw-r--r--   0        0        0    15895 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-metadata-2.0.xsd
+-rw-r--r--   0        0        0    13466 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-protocol-2.0.xsd
+-rw-r--r--   0        0        0     1139 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-metadata-attr.xsd
+-rw-r--r--   0        0        0      732 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-attribute-ext.xsd
+-rw-r--r--   0        0        0     1453 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-metadata-algsupport-v1.0.xsd
+-rw-r--r--   0        0        0     3098 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-metadata-ui-v1.0.xsd
+-rw-r--r--   0        0        0    13093 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-schema-assertion-2.0.xsd
+-rw-r--r--   0        0        0    13867 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-schema-protocol-2.0.xsd
+-rw-r--r--   0        0        0     4830 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xenc-schema.xsd
+-rw-r--r--   0        0        0     8836 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xml.xsd
+-rw-r--r--   0        0        0    10003 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xmldsig-core-schema.xsd
+-rw-r--r--   0        0        0    32462 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/settings.py
+-rw-r--r--   0        0        0     6501 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/soap_logout_request.py
+-rw-r--r--   0        0        0     1127 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/ssl_adapter.py
+-rw-r--r--   0        0        0    40077 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/utils.py
+-rw-r--r--   0        0        0     6128 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/xml_templates.py
+-rw-r--r--   0        0        0     7053 2024-04-02 09:26:47.792761 maykin_python3_saml-1.16.1/src/onelogin/saml2/xml_utils.py
+-rw-r--r--   0        0        0     5818 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/src/onelogin/saml2/xmlparser.py
+-rw-r--r--   0        0        0        0 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/__init__.py
+-rw-r--r--   0        0        0      644 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/certs/certificate1
+-rw-r--r--   0        0        0      550 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/coverage.rc
+-rw-r--r--   0        0        0     3317 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/artifact_response/artifact_response.xml
+-rw-r--r--   0        0        0     3323 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/artifact_response/artifact_response_invalid.xml
+-rw-r--r--   0        0        0      594 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/customPath/advanced_settings.json
+-rw-r--r--   0        0        0      927 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/customPath/certs/idp.crt
+-rwxr-xr-x   0        0        0      928 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/customPath/certs/metadata.crt
+-rwxr-xr-x   0        0        0      891 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/customPath/certs/metadata.key
+-rwxr-xr-x   0        0        0      928 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/customPath/certs/sp.crt
+-rwxr-xr-x   0        0        0      891 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/customPath/certs/sp.key
+-rw-r--r--   0        0        0      821 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/invalid_issuer.xml
+-rw-r--r--   0        0        0      509 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/invalid_issuer.xml.base64
+-rw-r--r--   0        0        0      586 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/no_nameId.xml
+-rw-r--r--   0        0        0      793 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/not_after_failed.xml
+-rw-r--r--   0        0        0      488 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/not_after_failed.xml.base64
+-rw-r--r--   0        0        0      736 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request.xml
+-rw-r--r--   0        0        0      996 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request.xml.base64
+-rw-r--r--   0        0        0      472 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_deflated.xml.base64
+-rw-r--r--   0        0        0     1960 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_encrypted_nameid.xml
+-rw-r--r--   0        0        0      753 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_with_encoding.xml
+-rw-r--r--   0        0        0      823 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_with_sessionindex.xml
+-rw-r--r--   0        0        0      389 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/invalids/no_status.xml.base64
+-rw-r--r--   0        0        0      433 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/invalids/status_code_responder.xml.base64
+-rw-r--r--   0        0        0      701 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response.xml
+-rw-r--r--   0        0        0      953 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response.xml.base64
+-rw-r--r--   0        0        0      437 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response_deflated.xml.base64
+-rw-r--r--   0        0        0      740 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response_with_encoding.xml
+-rw-r--r--   0        0        0      473 2022-10-31 15:34:11.716435 maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response_with_encoding_deflated.xml.base64
+-rw-r--r--   0        0        0     6649 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/entities_metadata.xml
+-rw-r--r--   0        0        0     2925 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/expired_metadata_settings1.xml
+-rw-r--r--   0        0        0     2675 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata.xml
+-rw-r--r--   0        0        0     2554 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata2.xml
+-rw-r--r--   0        0        0     4446 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_different_sign_and_encrypt_cert.xml
+-rw-r--r--   0        0        0     5259 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_multi_certs.xml
+-rw-r--r--   0        0        0     5257 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_multi_signing_certs.xml
+-rw-r--r--   0        0        0     4349 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_same_sign_and_encrypt_cert.xml
+-rw-r--r--   0        0        0    10914 2024-02-15 10:00:22.640516 maykin_python3_saml-1.16.1/tests/data/metadata/idp_multiple_descriptors.xml
+-rw-r--r--   0        0        0      988 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/metadata_bad_order_settings1.xml
+-rw-r--r--   0        0        0      988 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/metadata_settings1.xml
+-rw-r--r--   0        0        0      882 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/no_expiration_mark_metadata.xml
+-rw-r--r--   0        0        0     2927 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/noentity_metadata_settings1.xml
+-rw-r--r--   0        0        0     5496 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/signed_metadata_settings1.xml
+-rw-r--r--   0        0        0     5127 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/signed_metadata_settings2.xml
+-rw-r--r--   0        0        0    20092 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/testshib-providers.xml
+-rw-r--r--   0        0        0      989 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/metadata/unparsed_metadata.xml
+-rw-r--r--   0        0        0      916 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/misc/sp2.key
+-rw-r--r--   0        0        0      891 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/misc/sp3.key
+-rw-r--r--   0        0        0     1704 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/misc/sp4.key
+-rw-r--r--   0        0        0      986 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/requests/authn_request.xml
+-rw-r--r--   0        0        0     1329 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/requests/authn_request.xml.base64
+-rw-r--r--   0        0        0     5526 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/adfs_response.xml.base64
+-rw-r--r--   0        0        0     2843 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/decrypted_valid_encrypted_assertion.xml
+-rw-r--r--   0        0        0    11829 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/double_signed_encrypted_assertion.xml.base64
+-rw-r--r--   0        0        0    12056 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/double_signed_encrypted_assertion2.xml.base64
+-rw-r--r--   0        0        0     8849 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/double_signed_response.xml.base64
+-rw-r--r--   0        0        0     8796 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/double_signed_response2.xml.base64
+-rw-r--r--   0        0        0     3996 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/expired_response.xml.base64
+-rw-r--r--   0        0        0     8821 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/bad_reference.xml.base64
+-rw-r--r--   0        0        0     9125 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/duplicated_attributes.xml.base64
+-rw-r--r--   0        0        0     8685 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/empty_destination.xml.base64
+-rw-r--r--   0        0        0     8729 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/empty_nameid.xml.base64
+-rw-r--r--   0        0        0     5132 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_attrs.xml.base64
+-rw-r--r--   0        0        0    10101 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_nameID_without_EncMethod.xml.base64
+-rw-r--r--   0        0        0     9617 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_nameID_without_keyinfo.xml.base64
+-rw-r--r--   0        0        0     2949 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_audience.xml.base64
+-rw-r--r--   0        0        0     2980 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_issuer_assertion.xml.base64
+-rw-r--r--   0        0        0     2984 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_issuer_message.xml.base64
+-rw-r--r--   0        0        0     2964 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_sessionindex.xml.base64
+-rw-r--r--   0        0        0     2940 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_inresponse.xml.base64
+-rw-r--r--   0        0        0     2961 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_nb.xml.base64
+-rw-r--r--   0        0        0     2964 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_noa.xml.base64
+-rw-r--r--   0        0        0     2952 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_recipient.xml.base64
+-rw-r--r--   0        0        0     9918 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/multiple_assertions.xml.base64
+-rw-r--r--   0        0        0     6037 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_authnstatement.xml.base64
+-rw-r--r--   0        0        0     6140 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_conditions.xml.base64
+-rw-r--r--   0        0        0     3753 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_id.xml.base64
+-rw-r--r--   0        0        0     6348 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_issuer_assertion.xml.base64
+-rw-r--r--   0        0        0     6320 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_issuer_response.xml.base64
+-rw-r--r--   0        0        0     3357 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_key.xml.base64
+-rw-r--r--   0        0        0     2772 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_nameid.xml.base64
+-rw-r--r--   0        0        0     3725 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_saml2.xml.base64
+-rw-r--r--   0        0        0     2577 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_signature.xml.base64
+-rw-r--r--   0        0        0     5289 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_status.xml.base64
+-rw-r--r--   0        0        0     5293 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_status_code.xml.base64
+-rw-r--r--   0        0        0     2728 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_subjectconfirmation_data.xml.base64
+-rw-r--r--   0        0        0     2976 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_subjectconfirmation_method.xml.base64
+-rw-r--r--   0        0        0     3813 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/not_after_failed.xml.base64
+-rw-r--r--   0        0        0     6277 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/not_before_failed.xml.base64
+-rw-r--r--   0        0        0     5132 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/response_encrypted_attrs.xml.base64
+-rw-r--r--   0        0        0    10484 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/signature_wrapping_attack.xml.base64
+-rw-r--r--   0        0        0    10492 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/signature_wrapping_attack2.xml.base64
+-rw-r--r--   0        0        0     7349 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/invalids/signed_assertion_response.xml.base64
+-rw-r--r--   0        0        0      777 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/status_code_responder.xml.base64
+-rw-r--r--   0        0        0      853 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/status_code_responer_and_msg.xml.base64
+-rw-r--r--   0        0        0     6380 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/invalids/wrong_spnamequalifier.xml.base64
+-rw-r--r--   0        0        0     2768 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/no_audience.xml.base64
+-rw-r--r--   0        0        0     3475 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/open_saml_response.xml
+-rw-r--r--   0        0        0     2844 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/pretty_decrypted_valid_encrypted_assertion.xml
+-rw-r--r--   0        0        0     5087 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/pretty_signed_message_response.xml
+-rw-r--r--   0        0        0     5196 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response1.xml.base64
+-rw-r--r--   0        0        0     6312 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response1_with_duplicate_attributes.xml.base64
+-rw-r--r--   0        0        0     5352 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response1_with_friendlyname.xml.base64
+-rw-r--r--   0        0        0     4786 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response2.xml.base64
+-rw-r--r--   0        0        0     3982 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response3.xml.base64
+-rw-r--r--   0        0        0     5668 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response4.xml.base64
+-rw-r--r--   0        0        0     6218 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response5.xml.base64
+-rw-r--r--   0        0        0     5301 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/responses/response6.xml.base64
+-rw-r--r--   0        0        0    10072 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response_encrypted_nameid.xml.base64
+-rw-r--r--   0        0        0     7136 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response_node_text_attack.xml.base64
+-rw-r--r--   0        0        0     8467 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response_with_ampersands.xml
+-rw-r--r--   0        0        0     5668 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response_with_ampersands.xml.base64
+-rw-r--r--   0        0        0     5472 2022-10-31 15:34:11.719768 maykin_python3_saml-1.16.1/tests/data/responses/response_with_nested_nameid_values.xml.base64
+-rw-r--r--   0        0        0     4981 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/response_without_assertion_reference_uri.xml.base64
+-rw-r--r--   0        0        0     4981 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/response_without_reference_uri.xml.base64
+-rw-r--r--   0        0        0     6429 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/signed_assertion_response.xml.base64
+-rw-r--r--   0        0        0     6396 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_assertion_response2.xml.base64
+-rw-r--r--   0        0        0     9969 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_encrypted_assertion.xml.base64
+-rw-r--r--   0        0        0     9656 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_encrypted_assertion2.xml.base64
+-rw-r--r--   0        0        0     8613 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_message_encrypted_assertion.xml.base64
+-rw-r--r--   0        0        0     8840 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_message_encrypted_assertion2.xml.base64
+-rw-r--r--   0        0        0     6461 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/data/responses/signed_message_response.xml.base64
+-rw-r--r--   0        0        0    10605 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/signed_message_response2.xml.base64
+-rw-r--r--   0        0        0     4171 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/simple_saml_php.xml
+-rw-r--r--   0        0        0     2125 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/unsigned_assertion.xml.base64
+-rw-r--r--   0        0        0     2965 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/unsigned_response.xml.base64
+-rw-r--r--   0        0        0     2996 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/unsigned_response_with_miliseconds.xm.base64
+-rw-r--r--   0        0        0     6753 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_encrypted_assertion.xml.base64
+-rw-r--r--   0        0        0     8208 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_encrypted_assertion_encrypted_nameid.xml.base64
+-rw-r--r--   0        0        0     8760 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_response.xml.base64
+-rw-r--r--   0        0        0     8797 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_response2.xml.base64
+-rw-r--r--   0        0        0     8756 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_response_with_namequalifier.xml.base64
+-rw-r--r--   0        0        0     5585 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_response_without_inresponseto.xml.base64
+-rw-r--r--   0        0        0     3997 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_unsigned_response.xml
+-rw-r--r--   0        0        0     3997 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/valid_unsigned_response.xml.base64
+-rw-r--r--   0        0        0     9722 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/data/responses/wrapped_response_2.xml.base64
+-rw-r--r--   0        0        0     1899 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request.xml
+-rw-r--r--   0        0        0     1888 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_empty_id.xml
+-rw-r--r--   0        0        0     1850 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_empty_nameId.xml
+-rw-r--r--   0        0        0     1905 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_invalid_issuer.xml
+-rw-r--r--   0        0        0     1909 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_invalid_signature.xml
+-rw-r--r--   0        0        0     2077 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/pylint.rc
+-rw-r--r--   0        0        0     2246 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings1.json
+-rw-r--r--   0        0        0     2159 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings10.json
+-rw-r--r--   0        0        0     2718 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings11.json
+-rw-r--r--   0        0        0     3916 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings12.json
+-rw-r--r--   0        0        0     3842 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings13.json
+-rw-r--r--   0        0        0     2575 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings14.json
+-rw-r--r--   0        0        0     2488 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings15.json
+-rw-r--r--   0        0        0     2252 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings2.json
+-rw-r--r--   0        0        0     2226 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings3.json
+-rw-r--r--   0        0        0     3764 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings4.json
+-rw-r--r--   0        0        0     2969 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings5.json
+-rw-r--r--   0        0        0     1495 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings6.json
+-rw-r--r--   0        0        0     4798 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings7.json
+-rw-r--r--   0        0        0     5841 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings8.json
+-rw-r--r--   0        0        0     1362 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/settings/settings9.json
+-rw-r--r--   0        0        0        0 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/src/OneLogin/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-31 15:34:11.723101 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/__init__.py
+-rw-r--r--   0        0        0     2710 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/artifact_resolve_request_test.py
+-rw-r--r--   0        0        0     3349 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/artifact_response_test.py
+-rw-r--r--   0        0        0    83627 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/auth_test.py
+-rw-r--r--   0        0        0    18878 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/authn_request_test.py
+-rw-r--r--   0        0        0      337 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/error_test.py
+-rw-r--r--   0        0        0    54924 2024-04-02 10:33:02.844628 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/idp_metadata_parser_test.py
+-rw-r--r--   0        0        0    26614 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/logout_request_test.py
+-rw-r--r--   0        0        0    19455 2024-02-15 10:00:22.643850 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/logout_response_test.py
+-rw-r--r--   0        0        0    19057 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/metadata_test.py
+-rw-r--r--   0        0        0   109294 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/response_test.py
+-rw-r--r--   0        0        0    51685 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/settings_test.py
+-rw-r--r--   0        0        0     1952 2024-02-15 10:00:22.647183 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/signed_response_test.py
+-rw-r--r--   0        0        0     4175 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/soap_logout_request_test.py
+-rw-r--r--   0        0        0    50647 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/utils_test.py
+-rw-r--r--   0        0        0     8501 2024-04-02 09:26:47.796095 maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/xml_utils_test.py
+-rw-r--r--   0        0        0        0 2022-10-31 15:34:11.726435 maykin_python3_saml-1.16.1/tests/src/__init__.py
+-rw-r--r--   0        0        0    80272 1970-01-01 00:00:00.000000 maykin_python3_saml-1.16.1/PKG-INFO
```

### Comparing `maykin_python3_saml-1.16.0.post2/LICENSE` & `maykin_python3_saml-1.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/README.md` & `maykin_python3_saml-1.16.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -771,15 +771,15 @@
 * If ``RelayState`` is provided, a redirection takes place.
 
 Notice that we saved the user data in the session before the redirection to have the user data available at the ``RelayState`` view.
 
 In order to retrieve attributes we use:
 
 ```python
-attributes = auth.get_attributes();
+attributes = auth.get_attributes()
 ```
 
 With this method we get a dict with all the user data provided by the IdP in the assertion of the SAML response.
 
 If we execute print attributes we could get:
 
 ```python
@@ -792,15 +792,15 @@
 ```
 
 Each attribute name can be used as a key to obtain the value. Every attribute is a list of values. A single-valued attribute is a list of a single element.
 
 The following code is equivalent:
 
 ```python
-attributes = auth.get_attributes();
+attributes = auth.get_attributes()
 print(attributes['cn'])
 
 print(auth.get_attribute('cn'))
 ```
 
 Before trying to get an attribute, check that the user is authenticated. If the user isn't authenticated, an empty dict will be returned. For example, if we call to ``get_attributes`` before a ``auth.process_response``, the ``get_attributes()`` will return an empty dict.
```

### Comparing `maykin_python3_saml-1.16.0.post2/pyproject.toml` & `maykin_python3_saml-1.16.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maykin-python3-saml"
-version = "1.16.0.post2"
+version = "1.16.1"
 description = "Saml Python Toolkit. Add SAML support to your Python software using this library"
 license = "Apache-2.0"
 authors = [
     "SAML-Toolkits <contact@iamdigitalservices.com>",
     "Maykin Media <support@maykinmedia.nl>",
 ]
 maintainers = ["Sixto Martin <sixto.martin.garcia@gmail.com>"]
```

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/__init__.py` & `maykin_python3_saml-1.16.1/src/onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/__init__.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/__init__.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/artifact_resolve.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/artifact_resolve.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/artifact_response.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/artifact_response.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/auth.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/auth.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/authn_request.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/authn_request.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/compat.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/compat.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/constants.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/constants.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/errors.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/errors.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/idp_metadata_parser.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/idp_metadata_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 """ OneLogin_Saml2_IdPMetadataParser class
 Metadata class of SAML Python Toolkit.
 """
 
 
 from copy import deepcopy
 
-try:
-    import urllib.request as urllib2
-except ImportError:
-    import urllib2
-
-import ssl
+import requests
 
 from onelogin.saml2.constants import OneLogin_Saml2_Constants
 from onelogin.saml2.xml_utils import OneLogin_Saml2_XML
 
 
 class OneLogin_Saml2_IdPMetadataParser(object):
     """
@@ -42,24 +37,20 @@
         :type headers: dict
 
         :returns: metadata XML
         :rtype: string
         """
         valid = False
 
-        request = urllib2.Request(url, headers=headers or {})
-
-        if validate_cert:
-            response = urllib2.urlopen(request, timeout=timeout)
-        else:
-            ctx = ssl.create_default_context()
-            ctx.check_hostname = False
-            ctx.verify_mode = ssl.CERT_NONE
-            response = urllib2.urlopen(request, context=ctx, timeout=timeout)
-        xml = response.read()
+        # MAYKIN: use requests to retrieve the metadata, so the CA bundle configured for
+        # requests can be used and self-signed/private root certificates still continue
+        # to work.
+        response = requests.get(url, headers=headers, verify=validate_cert, timeout=timeout)
+        response.raise_for_status()
+        xml = response.content
 
         if xml:
             try:
                 dom = OneLogin_Saml2_XML.to_etree(xml)
                 idp_descriptor_nodes = OneLogin_Saml2_XML.query(dom, '//md:IDPSSODescriptor')
                 if idp_descriptor_nodes:
                     valid = True
```

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/logout_request.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/logout_request.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/logout_response.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/logout_response.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/metadata.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/metadata.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/response.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/response.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-context-schema-os.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-context-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-policy-schema-os.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-policy-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-assertion-schema-os.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-assertion-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-protocol-schema-os.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/access_control-xacml-2.0-saml-protocol-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-assertion-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-authn-context-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-authn-context-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-authn-context-types-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-authn-context-types-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-metadata-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-metadata-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/saml-schema-protocol-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-metadata-attr.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-metadata-attr.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-attribute-ext.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-attribute-ext.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-metadata-algsupport-v1.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-metadata-algsupport-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-metadata-ui-v1.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-metadata-ui-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-schema-assertion-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/sstc-saml-schema-protocol-2.0.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/sstc-saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xenc-schema.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xml.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/schemas/xmldsig-core-schema.xsd` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/schemas/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/settings.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/settings.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/soap_logout_request.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/soap_logout_request.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/ssl_adapter.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/ssl_adapter.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/utils.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xml_templates.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/xml_templates.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xml_utils.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/xml_utils.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/src/onelogin/saml2/xmlparser.py` & `maykin_python3_saml-1.16.1/src/onelogin/saml2/xmlparser.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/certs/certificate1` & `maykin_python3_saml-1.16.1/tests/certs/certificate1`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/coverage.rc` & `maykin_python3_saml-1.16.1/tests/coverage.rc`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/artifact_response/artifact_response.xml` & `maykin_python3_saml-1.16.1/tests/data/artifact_response/artifact_response.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/artifact_response/artifact_response_invalid.xml` & `maykin_python3_saml-1.16.1/tests/data/artifact_response/artifact_response_invalid.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/advanced_settings.json` & `maykin_python3_saml-1.16.1/tests/data/customPath/advanced_settings.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/idp.crt` & `maykin_python3_saml-1.16.1/tests/data/customPath/certs/idp.crt`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/metadata.crt` & `maykin_python3_saml-1.16.1/tests/data/customPath/certs/metadata.crt`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/metadata.key` & `maykin_python3_saml-1.16.1/tests/data/customPath/certs/metadata.key`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/sp.crt` & `maykin_python3_saml-1.16.1/tests/data/customPath/certs/sp.crt`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/customPath/certs/sp.key` & `maykin_python3_saml-1.16.1/tests/data/customPath/certs/sp.key`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/invalid_issuer.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/invalid_issuer.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/no_nameId.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/no_nameId.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/invalids/not_after_failed.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/invalids/not_after_failed.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_encrypted_nameid.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_encrypted_nameid.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_with_encoding.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_with_encoding.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_requests/logout_request_with_sessionindex.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_requests/logout_request_with_sessionindex.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/logout_responses/logout_response_with_encoding.xml` & `maykin_python3_saml-1.16.1/tests/data/logout_responses/logout_response_with_encoding.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/entities_metadata.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/entities_metadata.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/expired_metadata_settings1.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/expired_metadata_settings1.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata2.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata2.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_different_sign_and_encrypt_cert.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_different_sign_and_encrypt_cert.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_multi_certs.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_multi_certs.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_multi_signing_certs.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_multi_signing_certs.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_metadata_same_sign_and_encrypt_cert.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_metadata_same_sign_and_encrypt_cert.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/idp_multiple_descriptors.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/idp_multiple_descriptors.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/metadata_bad_order_settings1.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/metadata_bad_order_settings1.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/metadata_settings1.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/metadata_settings1.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/no_expiration_mark_metadata.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/no_expiration_mark_metadata.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/noentity_metadata_settings1.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/noentity_metadata_settings1.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/signed_metadata_settings1.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/signed_metadata_settings1.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/signed_metadata_settings2.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/signed_metadata_settings2.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/testshib-providers.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/testshib-providers.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/metadata/unparsed_metadata.xml` & `maykin_python3_saml-1.16.1/tests/data/metadata/unparsed_metadata.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/misc/sp2.key` & `maykin_python3_saml-1.16.1/tests/data/misc/sp2.key`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/misc/sp3.key` & `maykin_python3_saml-1.16.1/tests/data/misc/sp3.key`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/misc/sp4.key` & `maykin_python3_saml-1.16.1/tests/data/misc/sp4.key`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/requests/authn_request.xml` & `maykin_python3_saml-1.16.1/tests/data/requests/authn_request.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/requests/authn_request.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/requests/authn_request.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/adfs_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/adfs_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/decrypted_valid_encrypted_assertion.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/decrypted_valid_encrypted_assertion.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_encrypted_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/double_signed_encrypted_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_encrypted_assertion2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/double_signed_encrypted_assertion2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/double_signed_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/double_signed_response2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/double_signed_response2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/expired_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/expired_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/bad_reference.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/bad_reference.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/duplicated_attributes.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/duplicated_attributes.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/empty_destination.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/empty_destination.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/empty_nameid.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/empty_nameid.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_attrs.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_attrs.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_nameID_without_EncMethod.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_nameID_without_EncMethod.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/encrypted_nameID_without_keyinfo.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/encrypted_nameID_without_keyinfo.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_audience.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_audience.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_issuer_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_issuer_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_issuer_message.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_issuer_message.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_sessionindex.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_sessionindex.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_inresponse.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_inresponse.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_nb.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_nb.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_noa.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_noa.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/invalid_subjectconfirmation_recipient.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/invalid_subjectconfirmation_recipient.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/multiple_assertions.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/multiple_assertions.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_authnstatement.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_authnstatement.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_conditions.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_conditions.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_id.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_id.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_issuer_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_issuer_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_issuer_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_issuer_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_key.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_key.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_nameid.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_nameid.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_saml2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_saml2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_signature.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_signature.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_status.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_status.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_status_code.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_status_code.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_subjectconfirmation_data.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_subjectconfirmation_data.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/no_subjectconfirmation_method.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/no_subjectconfirmation_method.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/not_after_failed.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/not_after_failed.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/not_before_failed.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/not_before_failed.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/response_encrypted_attrs.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/response_encrypted_attrs.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signature_wrapping_attack.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/signature_wrapping_attack.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signature_wrapping_attack2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/signature_wrapping_attack2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/signed_assertion_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/signed_assertion_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/status_code_responder.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/status_code_responder.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/status_code_responer_and_msg.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/status_code_responer_and_msg.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/invalids/wrong_spnamequalifier.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/invalids/wrong_spnamequalifier.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/no_audience.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/no_audience.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/open_saml_response.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/open_saml_response.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/pretty_decrypted_valid_encrypted_assertion.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/pretty_decrypted_valid_encrypted_assertion.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/pretty_signed_message_response.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/pretty_signed_message_response.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response1.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response1.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response1_with_duplicate_attributes.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response1_with_duplicate_attributes.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response1_with_friendlyname.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response1_with_friendlyname.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response3.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response3.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response4.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response4.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response5.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response5.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response6.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response6.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_encrypted_nameid.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_encrypted_nameid.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_node_text_attack.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_node_text_attack.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_ampersands.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/response_with_ampersands.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_ampersands.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_with_ampersands.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_with_nested_nameid_values.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_with_nested_nameid_values.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_without_assertion_reference_uri.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_without_assertion_reference_uri.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/response_without_reference_uri.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/response_without_reference_uri.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_assertion_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_assertion_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_assertion_response2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_assertion_response2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_encrypted_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_encrypted_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_encrypted_assertion2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_encrypted_assertion2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_encrypted_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_message_encrypted_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_encrypted_assertion2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_message_encrypted_assertion2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_message_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/signed_message_response2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/signed_message_response2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/simple_saml_php.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/simple_saml_php.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/unsigned_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/unsigned_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/unsigned_response_with_miliseconds.xm.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/unsigned_response_with_miliseconds.xm.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_encrypted_assertion.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_encrypted_assertion.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_encrypted_assertion_encrypted_nameid.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_encrypted_assertion_encrypted_nameid.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_response2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response_with_namequalifier.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_response_with_namequalifier.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_response_without_inresponseto.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_response_without_inresponseto.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_unsigned_response.xml` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_unsigned_response.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/valid_unsigned_response.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/valid_unsigned_response.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/responses/wrapped_response_2.xml.base64` & `maykin_python3_saml-1.16.1/tests/data/responses/wrapped_response_2.xml.base64`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request.xml` & `maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_empty_id.xml` & `maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_empty_id.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_empty_nameId.xml` & `maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_empty_nameId.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_invalid_issuer.xml` & `maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_invalid_issuer.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/data/soap_logout_requests/soap_logout_request_invalid_signature.xml` & `maykin_python3_saml-1.16.1/tests/data/soap_logout_requests/soap_logout_request_invalid_signature.xml`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/pylint.rc` & `maykin_python3_saml-1.16.1/tests/pylint.rc`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings1.json` & `maykin_python3_saml-1.16.1/tests/settings/settings1.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings10.json` & `maykin_python3_saml-1.16.1/tests/settings/settings10.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings11.json` & `maykin_python3_saml-1.16.1/tests/settings/settings11.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings12.json` & `maykin_python3_saml-1.16.1/tests/settings/settings12.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings13.json` & `maykin_python3_saml-1.16.1/tests/settings/settings13.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings14.json` & `maykin_python3_saml-1.16.1/tests/settings/settings14.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings15.json` & `maykin_python3_saml-1.16.1/tests/settings/settings15.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings2.json` & `maykin_python3_saml-1.16.1/tests/settings/settings2.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings3.json` & `maykin_python3_saml-1.16.1/tests/settings/settings3.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings4.json` & `maykin_python3_saml-1.16.1/tests/settings/settings4.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings5.json` & `maykin_python3_saml-1.16.1/tests/settings/settings5.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings6.json` & `maykin_python3_saml-1.16.1/tests/settings/settings6.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings7.json` & `maykin_python3_saml-1.16.1/tests/settings/settings7.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings8.json` & `maykin_python3_saml-1.16.1/tests/settings/settings8.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/settings/settings9.json` & `maykin_python3_saml-1.16.1/tests/settings/settings9.json`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/artifact_resolve_request_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/artifact_resolve_request_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/artifact_response_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/artifact_response_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/auth_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/authn_request_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/authn_request_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/idp_metadata_parser_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/idp_metadata_parser_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # -*- coding: utf-8 -*-
 
-
-try:
-    from urllib.error import URLError
-except ImportError:
-    from urllib2 import URLError
-
 from copy import deepcopy
 import json
 from os.path import dirname, join, exists
 from lxml.etree import XMLSyntaxError
+from requests import RequestException
 import unittest
 
 from onelogin.saml2.idp_metadata_parser import OneLogin_Saml2_IdPMetadataParser
 from onelogin.saml2.constants import OneLogin_Saml2_Constants
 
 
 class OneLogin_Saml2_IdPMetadataParser_Test(unittest.TestCase):
@@ -47,15 +42,15 @@
         """
         with self.assertRaises(Exception):
             data = OneLogin_Saml2_IdPMetadataParser.get_metadata('http://google.es')
 
         try:
             data = OneLogin_Saml2_IdPMetadataParser.get_metadata('https://idp.testshib.org/idp/shibboleth')
             self.assertTrue(data is not None and data is not {})
-        except URLError:
+        except RequestException:
             pass
 
     def testGetMetadataWithHeaders(self):
         data = OneLogin_Saml2_IdPMetadataParser.get_metadata('https://samltest.id/saml/providers',
                                                              headers={'User-Agent': 'Mozilla/5.0'})
         self.assertIsNotNone(data)
         self.assertIn(b'entityID=', data)
@@ -65,15 +60,15 @@
         Tests the parse_remote method of the OneLogin_Saml2_IdPMetadataParser
         """
         with self.assertRaises(Exception):
             data = OneLogin_Saml2_IdPMetadataParser.parse_remote('http://google.es')
 
         try:
             data = OneLogin_Saml2_IdPMetadataParser.parse_remote('https://idp.testshib.org/idp/shibboleth')
-        except URLError:
+        except RequestException:
             xml = self.file_contents(join(self.data_path, 'metadata', 'testshib-providers.xml'))
             data = OneLogin_Saml2_IdPMetadataParser.parse(xml)
 
         self.assertTrue(data is not None and data is not {})
         expected_settings_json = """
         {
           "sp": {
@@ -168,15 +163,15 @@
             }]
           }
         }
         """
         try:
             xmldoc = OneLogin_Saml2_IdPMetadataParser.get_metadata(
                 'https://idp.testshib.org/idp/shibboleth')
-        except URLError:
+        except RequestException:
             xmldoc = self.file_contents(join(self.data_path, 'metadata', 'testshib-providers.xml'))
 
         # Parse, require SSO REDIRECT binding, implicitly.
         settings1 = OneLogin_Saml2_IdPMetadataParser.parse(xmldoc)
         # Parse, require SSO REDIRECT binding, explicitly.
         settings2 = OneLogin_Saml2_IdPMetadataParser.parse(
             xmldoc,
@@ -211,15 +206,15 @@
             }]
           }
         }
         """
         try:
             xmldoc = OneLogin_Saml2_IdPMetadataParser.get_metadata(
                 'https://idp.testshib.org/idp/shibboleth')
-        except URLError:
+        except RequestException:
             xmldoc = self.file_contents(join(self.data_path, 'metadata', 'testshib-providers.xml'))
 
         # Parse, require POST binding.
         settings = OneLogin_Saml2_IdPMetadataParser.parse(
             xmldoc,
             required_sso_binding=OneLogin_Saml2_Constants.BINDING_HTTP_POST
         )
```

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/logout_request_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/logout_request_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/logout_response_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/logout_response_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/metadata_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/response_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/response_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/settings_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/settings_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/signed_response_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/signed_response_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/soap_logout_request_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/soap_logout_request_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/utils_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/tests/src/OneLogin/saml2_tests/xml_utils_test.py` & `maykin_python3_saml-1.16.1/tests/src/OneLogin/saml2_tests/xml_utils_test.py`

 * *Files identical despite different names*

### Comparing `maykin_python3_saml-1.16.0.post2/PKG-INFO` & `maykin_python3_saml-1.16.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maykin-python3-saml
-Version: 1.16.0.post2
+Version: 1.16.1
 Summary: Saml Python Toolkit. Add SAML support to your Python software using this library
 Home-page: https://github.com/maykinmedia/python3-saml
 License: Apache-2.0
 Keywords: saml,saml2,sso,xmlsec,federation,identity
 Author: SAML-Toolkits
 Author-email: contact@iamdigitalservices.com
 Maintainer: Sixto Martin
@@ -813,15 +813,15 @@
 * If ``RelayState`` is provided, a redirection takes place.
 
 Notice that we saved the user data in the session before the redirection to have the user data available at the ``RelayState`` view.
 
 In order to retrieve attributes we use:
 
 ```python
-attributes = auth.get_attributes();
+attributes = auth.get_attributes()
 ```
 
 With this method we get a dict with all the user data provided by the IdP in the assertion of the SAML response.
 
 If we execute print attributes we could get:
 
 ```python
@@ -834,15 +834,15 @@
 ```
 
 Each attribute name can be used as a key to obtain the value. Every attribute is a list of values. A single-valued attribute is a list of a single element.
 
 The following code is equivalent:
 
 ```python
-attributes = auth.get_attributes();
+attributes = auth.get_attributes()
 print(attributes['cn'])
 
 print(auth.get_attribute('cn'))
 ```
 
 Before trying to get an attribute, check that the user is authenticated. If the user isn't authenticated, an empty dict will be returned. For example, if we call to ``get_attributes`` before a ``auth.process_response``, the ``get_attributes()`` will return an empty dict.
```

