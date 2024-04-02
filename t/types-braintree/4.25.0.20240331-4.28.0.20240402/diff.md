# Comparing `tmp/types-braintree-4.25.0.20240331.tar.gz` & `tmp/types-braintree-4.28.0.20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-braintree-4.25.0.20240331.tar", last modified: Sun Mar 31 02:18:13 2024, max compression
+gzip compressed data, was "types-braintree-4.28.0.20240402.tar", last modified: Tue Apr  2 02:17:28 2024, max compression
```

## Comparing `types-braintree-4.25.0.20240331.tar` & `types-braintree-4.28.0.20240402.tar`

### file list

```diff
@@ -1,173 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.751471 types-braintree-4.25.0.20240331/braintree-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/braintree-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/account_updater_daily_report.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/ach_mandate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/add_on.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/add_on_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/address.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/address_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/amex_express_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/android_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/apple_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/apple_pay_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/apple_pay_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/attribute_getter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/authorization_adjustment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/bin_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/braintree_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/client_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/client_token_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/connected_merchant_paypal_status_changed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/connected_merchant_status_transitioned.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credentials_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credit_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credit_card_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credit_card_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credit_card_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/credit_card_verification_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/customer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/customer_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/customer_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/disbursement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/disbursement_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/discount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/discount_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.751471 types-braintree-4.25.0.20240331/braintree-stubs/dispute_details/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_details/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_details/evidence.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_details/paypal_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_details/status_history.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/dispute_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/document_upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/document_upload_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29247 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/error_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/error_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/europe_bank_account.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/authentication_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/authorization_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/braintree_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/configuration_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/gateway_timeout_error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/http/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/http/connection_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/http/invalid_response_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/http/timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/invalid_challenge_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/invalid_signature_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/not_found_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/request_timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/service_unavailable_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/too_many_requests_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/unexpected_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/exceptions/upgrade_required_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/facilitated_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/facilitator_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/granted_payment_instrument_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/iban_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/ids_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/local_payment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/local_payment_completed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/local_payment_reversed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/masterpass_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/address_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/business_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/funding_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/individual_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account/merchant_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/merchant_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/modification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/oauth_access_revocation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/oauth_credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/oauth_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/paginated_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/paginated_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/partner_merchant.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_instrument_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_method_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_method_nonce.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_method_nonce_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/payment_method_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/paypal_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/paypal_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/paypal_here.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/plan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/plan_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/processor_response_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/braintree-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/resource_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/revoked_payment_method_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/risk_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/samsung_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/settlement_batch_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/settlement_batch_summary_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/signature_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/subscription.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/subscription_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/subscription_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/subscription_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/subscription_status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/successful_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/three_d_secure_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_amounts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_line_item_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/transaction_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/unknown_payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/us_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/us_bank_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/us_bank_account_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/us_bank_account_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/us_bank_account_verification_search.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/braintree-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/datetime_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/generator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/graphql_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/util/xml_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/validation_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/validation_error_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/venmo_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/visa_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/webhook_notification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/webhook_notification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/webhook_testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 02:17:27.000000 types-braintree-4.25.0.20240331/braintree-stubs/webhook_testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:13.755471 types-braintree-4.25.0.20240331/types_braintree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/types_braintree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/types_braintree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/types_braintree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 02:18:13.000000 types-braintree-4.25.0.20240331/types_braintree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.540281 types-braintree-4.28.0.20240402/braintree-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/braintree-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/account_updater_daily_report.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/ach_mandate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/add_on.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/add_on_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/address.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/address_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/amex_express_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/android_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/attribute_getter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/authorization_adjustment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/bin_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/braintree_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/client_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/client_token_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/connected_merchant_paypal_status_changed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/connected_merchant_status_transitioned.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credentials_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/disbursement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/disbursement_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/discount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/discount_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.540281 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/evidence.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/paypal_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/status_history.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/document_upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/document_upload_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/enriched_customer_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38081 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/error_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/error_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/europe_bank_account.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/authentication_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/authorization_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/braintree_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/configuration_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/gateway_timeout_error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/connection_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/invalid_response_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/invalid_challenge_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/invalid_signature_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/not_found_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/request_timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/service_unavailable_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/test_operation_performed_in_production_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/too_many_requests_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/unexpected_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/upgrade_required_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_input.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_payload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/facilitated_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/facilitator_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/granted_payment_instrument_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/iban_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/ids_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/liability_shift.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_completed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_expired.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_funded.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_reversed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/masterpass_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/address_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/business_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/funding_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/individual_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/merchant_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/meta_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/meta_checkout_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/modification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/montary_amount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_access_revocation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/package_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paginated_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paginated_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/partner_merchant.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_instrument_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_customer_data_updated_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_nonce.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_nonce_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_here.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/plan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/plan_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/processor_response_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/braintree-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/resource_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/revoked_payment_method_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/risk_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/samsung_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/sepa_direct_debit_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/sepa_direct_debit_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/settlement_batch_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/settlement_batch_summary_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/signature_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/successful_result.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/authentication_ids.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/credit_card_defaults.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/credit_card_numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/merchant_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/nonces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/venmo_sdk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/three_d_secure_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_amounts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_line_item_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_review.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/unknown_payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification_search.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/braintree-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/datetime_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/graphql_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/xml_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/validation_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/validation_error_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/venmo_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/venmo_profile_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/visa_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_notification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_notification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/types_braintree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/top_level.txt
```

### Comparing `types-braintree-4.25.0.20240331/CHANGELOG.md` & `types-braintree-4.28.0.20240402/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 4.28.0.20240402 (2024-04-02)
+
+braintree: Cleanup overzealous reexports from non `__init__` modules (#11692)
+
+braintree: Use `Final` for string constants (#11680)
+
+braintree: Replace usages of `Any` (#11679)
+
+stubtest-complete & Bump braintree to 4.28.* (#11678)
+
 ## 4.25.0.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
 
 ## 4.25.0.20240205 (2024-02-05)
 
 A new shade of Black (#11362)
```

### Comparing `types-braintree-4.25.0.20240331/PKG-INFO` & `types-braintree-4.28.0.20240402/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.25.0.20240331
+Version: 4.28.0.20240402
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`.
 
 This version of `types-braintree` aims to provide accurate annotations
-for `braintree==4.25.*`.
+for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/__init__.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/address.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/address.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from _typeshed import Incomplete
+from typing import Final
 
-from braintree.configuration import Configuration as Configuration
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.resource import Resource as Resource
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
+from braintree.resource import Resource
 
 class Address(Resource):
     class ShippingMethod:
-        SameDay: str
-        NextDay: str
-        Priority: str
-        Ground: str
-        Electronic: str
-        ShipToStore: str
+        SameDay: Final = "same_day"
+        NextDay: Final = "next_day"
+        Priority: Final = "priority"
+        Ground: Final = "ground"
+        Electronic: Final = "electronic"
+        ShipToStore: Final = "ship_to_store"
+        PickupInStore: Final = "pickup_in_store"
 
     @staticmethod
     def create(params: Incomplete | None = None): ...
     @staticmethod
     def delete(customer_id, address_id): ...
     @staticmethod
     def find(customer_id, address_id): ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/address_gateway.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/util/http.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from _typeshed import Incomplete
-from typing import Any
+from typing import Final
 
-from braintree.address import Address as Address
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.exceptions.not_found_error import NotFoundError as NotFoundError
-from braintree.resource import Resource as Resource
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
+class Http:
+    class ContentType:
+        Xml: Final = "application/xml"
+        Multipart: Final = "multipart/form-data"
+        Json: Final = "application/json"
 
-class AddressGateway:
-    gateway: Any
-    config: Any
-    def __init__(self, gateway) -> None: ...
-    def create(self, params: Incomplete | None = None): ...
-    def delete(self, customer_id, address_id): ...
-    def find(self, customer_id, address_id): ...
-    def update(self, customer_id, address_id, params: Incomplete | None = None): ...
+    @staticmethod
+    def is_error_status(status): ...
+    @staticmethod
+    def raise_exception_from_status(status, message: Incomplete | None = None) -> None: ...
+    config: Incomplete
+    environment: Incomplete
+    def __init__(self, config, environment: Incomplete | None = None) -> None: ...
+    def post(self, path, params: Incomplete | None = None): ...
+    def delete(self, path): ...
+    def get(self, path): ...
+    def put(self, path, params: Incomplete | None = None): ...
+    def post_multipart(self, path, files, params: Incomplete | None = None): ...
+    def http_do(self, http_verb, path, headers, request_body): ...
+    def handle_exception(self, exception) -> None: ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/braintree_gateway.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/braintree_gateway.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 from _typeshed import Incomplete
-from typing import Any
 
-from braintree.add_on_gateway import AddOnGateway as AddOnGateway
-from braintree.address_gateway import AddressGateway as AddressGateway
-from braintree.apple_pay_gateway import ApplePayGateway as ApplePayGateway
-from braintree.client_token_gateway import ClientTokenGateway as ClientTokenGateway
-from braintree.configuration import Configuration as Configuration
-from braintree.credit_card_gateway import CreditCardGateway as CreditCardGateway
-from braintree.credit_card_verification_gateway import CreditCardVerificationGateway as CreditCardVerificationGateway
-from braintree.customer_gateway import CustomerGateway as CustomerGateway
-from braintree.discount_gateway import DiscountGateway as DiscountGateway
-from braintree.dispute_gateway import DisputeGateway as DisputeGateway
-from braintree.document_upload_gateway import DocumentUploadGateway as DocumentUploadGateway
-from braintree.merchant_account_gateway import MerchantAccountGateway as MerchantAccountGateway
-from braintree.merchant_gateway import MerchantGateway as MerchantGateway
-from braintree.oauth_gateway import OAuthGateway as OAuthGateway
-from braintree.payment_method_gateway import PaymentMethodGateway as PaymentMethodGateway
-from braintree.payment_method_nonce_gateway import PaymentMethodNonceGateway as PaymentMethodNonceGateway
-from braintree.paypal_account_gateway import PayPalAccountGateway as PayPalAccountGateway
-from braintree.plan_gateway import PlanGateway as PlanGateway
-from braintree.settlement_batch_summary_gateway import SettlementBatchSummaryGateway as SettlementBatchSummaryGateway
-from braintree.subscription_gateway import SubscriptionGateway as SubscriptionGateway
-from braintree.testing_gateway import TestingGateway as TestingGateway
-from braintree.transaction_gateway import TransactionGateway as TransactionGateway
-from braintree.transaction_line_item_gateway import TransactionLineItemGateway as TransactionLineItemGateway
-from braintree.us_bank_account_gateway import UsBankAccountGateway as UsBankAccountGateway
-from braintree.us_bank_account_verification_gateway import UsBankAccountVerificationGateway as UsBankAccountVerificationGateway
-from braintree.webhook_notification_gateway import WebhookNotificationGateway as WebhookNotificationGateway
-from braintree.webhook_testing_gateway import WebhookTestingGateway as WebhookTestingGateway
+from braintree.add_on_gateway import AddOnGateway
+from braintree.address_gateway import AddressGateway
+from braintree.apple_pay_gateway import ApplePayGateway
+from braintree.client_token_gateway import ClientTokenGateway
+from braintree.configuration import Configuration
+from braintree.credit_card_gateway import CreditCardGateway
+from braintree.credit_card_verification_gateway import CreditCardVerificationGateway
+from braintree.customer_gateway import CustomerGateway
+from braintree.discount_gateway import DiscountGateway
+from braintree.dispute_gateway import DisputeGateway
+from braintree.document_upload_gateway import DocumentUploadGateway
+from braintree.exchange_rate_quote_gateway import ExchangeRateQuoteGateway
+from braintree.merchant_account_gateway import MerchantAccountGateway
+from braintree.merchant_gateway import MerchantGateway
+from braintree.oauth_gateway import OAuthGateway
+from braintree.payment_method_gateway import PaymentMethodGateway
+from braintree.payment_method_nonce_gateway import PaymentMethodNonceGateway
+from braintree.paypal_account_gateway import PayPalAccountGateway
+from braintree.plan_gateway import PlanGateway
+from braintree.sepa_direct_debit_account_gateway import SepaDirectDebitAccountGateway
+from braintree.settlement_batch_summary_gateway import SettlementBatchSummaryGateway
+from braintree.subscription_gateway import SubscriptionGateway
+from braintree.testing_gateway import TestingGateway
+from braintree.transaction_gateway import TransactionGateway
+from braintree.transaction_line_item_gateway import TransactionLineItemGateway
+from braintree.us_bank_account_gateway import UsBankAccountGateway
+from braintree.us_bank_account_verification_gateway import UsBankAccountVerificationGateway
+from braintree.webhook_notification_gateway import WebhookNotificationGateway
+from braintree.webhook_testing_gateway import WebhookTestingGateway
 
 class BraintreeGateway:
-    config: Any
-    add_on: Any
-    address: Any
-    apple_pay: Any
-    client_token: Any
-    credit_card: Any
-    customer: Any
-    discount: Any
-    dispute: Any
-    document_upload: Any
-    graphql_client: Any
-    merchant: Any
-    merchant_account: Any
-    oauth: Any
-    payment_method: Any
-    payment_method_nonce: Any
-    paypal_account: Any
-    plan: Any
-    settlement_batch_summary: Any
-    subscription: Any
-    testing: Any
-    transaction: Any
-    transaction_line_item: Any
-    us_bank_account: Any
-    us_bank_account_verification: Any
-    verification: Any
-    webhook_notification: Any
-    webhook_testing: Any
+    config: Configuration
+    add_on: AddOnGateway
+    address: AddressGateway
+    apple_pay: ApplePayGateway
+    client_token: ClientTokenGateway
+    credit_card: CreditCardGateway
+    customer: CustomerGateway
+    discount: DiscountGateway
+    dispute: DisputeGateway
+    document_upload: DocumentUploadGateway
+    exchange_rate_quote: ExchangeRateQuoteGateway
+    graphql_client: Incomplete
+    merchant: MerchantGateway
+    merchant_account: MerchantAccountGateway
+    oauth: OAuthGateway
+    payment_method: PaymentMethodGateway
+    payment_method_nonce: PaymentMethodNonceGateway
+    paypal_account: PayPalAccountGateway
+    plan: PlanGateway
+    sepa_direct_debit_account: SepaDirectDebitAccountGateway
+    settlement_batch_summary: SettlementBatchSummaryGateway
+    subscription: SubscriptionGateway
+    testing: TestingGateway
+    transaction: TransactionGateway
+    transaction_line_item: TransactionLineItemGateway
+    us_bank_account: UsBankAccountGateway
+    us_bank_account_verification: UsBankAccountVerificationGateway
+    verification: CreditCardVerificationGateway
+    webhook_notification: WebhookNotificationGateway
+    webhook_testing: WebhookTestingGateway
     def __init__(self, config: Incomplete | None = None, **kwargs) -> None: ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/credit_card_verification.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any
+from _typeshed import Incomplete
+from decimal import Decimal
+from typing import Final
 
-from braintree.attribute_getter import AttributeGetter as AttributeGetter
-from braintree.configuration import Configuration as Configuration
-from braintree.resource import Resource as Resource
-from braintree.risk_data import RiskData as RiskData
-from braintree.three_d_secure_info import ThreeDSecureInfo as ThreeDSecureInfo
+from braintree.attribute_getter import AttributeGetter
+from braintree.risk_data import RiskData
+from braintree.three_d_secure_info import ThreeDSecureInfo
 
 class CreditCardVerification(AttributeGetter):
     class Status:
-        Failed: str
-        GatewayRejected: str
-        ProcessorDeclined: str
-        Verified: str
+        Failed: Final = "failed"
+        GatewayRejected: Final = "gateway_rejected"
+        ProcessorDeclined: Final = "processor_declined"
+        Verified: Final = "verified"
 
-    amount: Any
-    currency_iso_code: Any
-    processor_response_code: Any
-    processor_response_text: Any
-    network_response_code: Any
-    network_response_text: Any
-    risk_data: Any
-    three_d_secure_info: Any
+    amount: Decimal | None
+    currency_iso_code: Incomplete
+    processor_response_code: Incomplete
+    processor_response_text: Incomplete
+    network_response_code: Incomplete
+    network_response_text: Incomplete
+    risk_data: RiskData | None
+    three_d_secure_info: ThreeDSecureInfo | None
     def __init__(self, gateway, attributes) -> None: ...
     @staticmethod
     def find(verification_id): ...
     @staticmethod
     def search(*query): ...
     @staticmethod
     def create(params): ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/environment.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/environment.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from _typeshed import Incomplete
 from typing import ClassVar
 
-from braintree.exceptions.configuration_error import ConfigurationError as ConfigurationError
-
 class Environment:
     Development: ClassVar[Environment]
     QA: ClassVar[Environment]
     Sandbox: ClassVar[Environment]
     Production: ClassVar[Environment]
     All: ClassVar[dict[str, Environment]]
     __name__: str
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/exceptions/__init__.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/exceptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/payment_method.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/payment_method.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from _typeshed import Incomplete
 
-from braintree.address import Address as Address
-from braintree.configuration import Configuration as Configuration
-from braintree.resource import Resource as Resource
+from braintree.resource import Resource
 
 class PaymentMethod(Resource):
     @staticmethod
     def create(params: Incomplete | None = None): ...
     @staticmethod
     def find(payment_method_token): ...
     @staticmethod
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/payment_method_gateway.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/customer.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 from _typeshed import Incomplete
-from typing import Any
 
-from braintree.amex_express_checkout_card import AmexExpressCheckoutCard as AmexExpressCheckoutCard
-from braintree.android_pay_card import AndroidPayCard as AndroidPayCard
-from braintree.apple_pay_card import ApplePayCard as ApplePayCard
-from braintree.credit_card import CreditCard as CreditCard
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.europe_bank_account import EuropeBankAccount as EuropeBankAccount
-from braintree.exceptions.not_found_error import NotFoundError as NotFoundError
-from braintree.ids_search import IdsSearch as IdsSearch
-from braintree.masterpass_card import MasterpassCard as MasterpassCard
-from braintree.payment_method import PaymentMethod as PaymentMethod
-from braintree.payment_method_nonce import PaymentMethodNonce as PaymentMethodNonce
-from braintree.payment_method_parser import parse_payment_method as parse_payment_method
-from braintree.paypal_account import PayPalAccount as PayPalAccount
-from braintree.resource import Resource as Resource
-from braintree.resource_collection import ResourceCollection as ResourceCollection
-from braintree.samsung_pay_card import SamsungPayCard as SamsungPayCard
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
-from braintree.unknown_payment_method import UnknownPaymentMethod as UnknownPaymentMethod
-from braintree.us_bank_account import UsBankAccount as UsBankAccount
-from braintree.venmo_account import VenmoAccount as VenmoAccount
-from braintree.visa_checkout_card import VisaCheckoutCard as VisaCheckoutCard
+from braintree.address import Address
+from braintree.amex_express_checkout_card import AmexExpressCheckoutCard
+from braintree.android_pay_card import AndroidPayCard
+from braintree.apple_pay_card import ApplePayCard
+from braintree.credit_card import CreditCard
+from braintree.europe_bank_account import EuropeBankAccount
+from braintree.masterpass_card import MasterpassCard
+from braintree.paypal_account import PayPalAccount
+from braintree.resource import Resource
+from braintree.samsung_pay_card import SamsungPayCard
+from braintree.us_bank_account import UsBankAccount
+from braintree.venmo_account import VenmoAccount
+from braintree.visa_checkout_card import VisaCheckoutCard
 
-class PaymentMethodGateway:
-    gateway: Any
-    config: Any
-    def __init__(self, gateway) -> None: ...
-    def create(self, params: Incomplete | None = None): ...
-    def find(self, payment_method_token): ...
-    def update(self, payment_method_token, params): ...
-    def delete(self, payment_method_token, options: Incomplete | None = None): ...
-    options: Any
-    def grant(self, payment_method_token, options: Incomplete | None = None): ...
-    def revoke(self, payment_method_token): ...
+class Customer(Resource):
+    @staticmethod
+    def all(): ...
+    @staticmethod
+    def create(params: Incomplete | None = None): ...
+    @staticmethod
+    def delete(customer_id): ...
+    @staticmethod
+    def find(customer_id, association_filter_id: Incomplete | None = None): ...
+    @staticmethod
+    def search(*query): ...
+    @staticmethod
+    def update(customer_id, params: Incomplete | None = None): ...
+    @staticmethod
+    def create_signature(): ...
+    @staticmethod
+    def update_signature(): ...
+    payment_methods: list[Resource]
+    credit_cards: list[CreditCard]
+    addresses: list[Address]
+    paypal_accounts: list[PayPalAccount]
+    apple_pay_cards: list[ApplePayCard]
+    android_pay_cards: list[AndroidPayCard]
+    amex_express_checkout_cards: list[AmexExpressCheckoutCard]
+    europe_bank_accounts: list[EuropeBankAccount]
+    venmo_accounts: list[VenmoAccount]
+    us_bank_accounts: list[UsBankAccount]
+    visa_checkout_cards: list[VisaCheckoutCard]
+    masterpass_cards: list[MasterpassCard]
+    samsung_pay_cards: list[SamsungPayCard]
+    def __init__(self, gateway, attributes) -> None: ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/paypal_account.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_card.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from _typeshed import Incomplete
-from typing import Any
+from typing import Final
 
-from braintree.configuration import Configuration as Configuration
-from braintree.resource import Resource as Resource
+from braintree.resource import Resource
+from braintree.subscription import Subscription
 
-class PayPalAccount(Resource):
-    @staticmethod
-    def find(paypal_account_token): ...
-    @staticmethod
-    def delete(paypal_account_token): ...
-    @staticmethod
-    def update(paypal_account_token, params: Incomplete | None = None): ...
+class ApplePayCard(Resource):
+    class CardType:
+        AmEx: Final = "Apple Pay - American Express"
+        MasterCard: Final = "Apple Pay - MasterCard"
+        Visa: Final = "Apple Pay - Visa"
+
+    is_expired: Incomplete
+    subscriptions: list[Subscription]
+    def __init__(self, gateway, attributes) -> None: ...
+    @property
+    def expiration_date(self): ...
     @staticmethod
     def signature(): ...
-    subscriptions: Any
-    def __init__(self, gateway, attributes) -> None: ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/search.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/search.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from typing import Any
+from _typeshed import Incomplete
 
 class Search:
     class IsNodeBuilder:
-        name: Any
+        name: Incomplete
         def __init__(self, name) -> None: ...
         def __eq__(self, value): ...
         def is_equal(self, value): ...
 
     class EqualityNodeBuilder(IsNodeBuilder):
         def __ne__(self, value): ...
         def is_not_equal(self, value): ...
 
     class KeyValueNodeBuilder:
-        name: Any
+        name: Incomplete
         def __init__(self, name) -> None: ...
         def __eq__(self, value): ...
         def is_equal(self, value): ...
         def __ne__(self, value): ...
         def is_not_equal(self, value): ...
 
     class PartialMatchNodeBuilder(EqualityNodeBuilder):
         def starts_with(self, value): ...
         def ends_with(self, value): ...
 
     class EndsWithNodeBuilder:
-        name: Any
+        name: Incomplete
         def __init__(self, name) -> None: ...
         def ends_with(self, value): ...
 
     class TextNodeBuilder(PartialMatchNodeBuilder):
         def contains(self, value): ...
 
     class Node:
-        name: Any
-        dict: Any
+        name: Incomplete
+        dict: Incomplete
         def __init__(self, name, dict) -> None: ...
         def to_param(self): ...
 
     class MultipleValueNodeBuilder:
-        name: Any
-        whitelist: Any
+        name: Incomplete
+        whitelist: Incomplete
         def __init__(self, name, whitelist=[]) -> None: ...
         def in_list(self, *values): ...
         def __eq__(self, value): ...
 
     class MultipleValueOrTextNodeBuilder(TextNodeBuilder, MultipleValueNodeBuilder):
         def __init__(self, name, whitelist=[]) -> None: ...
 
     class RangeNodeBuilder:
-        name: Any
+        name: Incomplete
         def __init__(self, name) -> None: ...
         def __eq__(self, value): ...
         def is_equal(self, value): ...
         def __ge__(self, min): ...
         def greater_than_or_equal_to(self, min): ...
         def __le__(self, max): ...
         def less_than_or_equal_to(self, max): ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/testing_gateway.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/testing_gateway.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from typing import Any
-
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
-from braintree.transaction import Transaction as Transaction
+from _typeshed import Incomplete
 
 class TestingGateway:
-    gateway: Any
-    config: Any
+    gateway: Incomplete
+    config: Incomplete
     def __init__(self, gateway) -> None: ...
     def make_past_due(self, subscription_id, number_of_days_past_due: int = 1) -> None: ...
     def escrow_transaction(self, transaction_id) -> None: ...
     def settle_transaction(self, transaction_id): ...
     def settlement_confirm_transaction(self, transaction_id): ...
     def settlement_decline_transaction(self, transaction_id): ...
     def settlement_pending_transaction(self, transaction_id): ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/transaction.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/transaction.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,108 @@
 from _typeshed import Incomplete
-from typing import Any
+from decimal import Decimal
+from typing import Final
 
-from braintree.add_on import AddOn as AddOn
-from braintree.address import Address as Address
-from braintree.amex_express_checkout_card import AmexExpressCheckoutCard as AmexExpressCheckoutCard
-from braintree.android_pay_card import AndroidPayCard as AndroidPayCard
-from braintree.apple_pay_card import ApplePayCard as ApplePayCard
-from braintree.authorization_adjustment import AuthorizationAdjustment as AuthorizationAdjustment
-from braintree.configuration import Configuration as Configuration
-from braintree.credit_card import CreditCard as CreditCard
-from braintree.customer import Customer as Customer
-from braintree.descriptor import Descriptor as Descriptor
-from braintree.disbursement_detail import DisbursementDetail as DisbursementDetail
-from braintree.discount import Discount as Discount
-from braintree.dispute import Dispute as Dispute
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.europe_bank_account import EuropeBankAccount as EuropeBankAccount
-from braintree.exceptions.not_found_error import NotFoundError as NotFoundError
-from braintree.facilitated_details import FacilitatedDetails as FacilitatedDetails
-from braintree.facilitator_details import FacilitatorDetails as FacilitatorDetails
-from braintree.local_payment import LocalPayment as LocalPayment
-from braintree.masterpass_card import MasterpassCard as MasterpassCard
-from braintree.payment_instrument_type import PaymentInstrumentType as PaymentInstrumentType
-from braintree.paypal_account import PayPalAccount as PayPalAccount
-from braintree.paypal_here import PayPalHere as PayPalHere
-from braintree.resource import Resource as Resource
-from braintree.resource_collection import ResourceCollection as ResourceCollection
-from braintree.risk_data import RiskData as RiskData
-from braintree.samsung_pay_card import SamsungPayCard as SamsungPayCard
-from braintree.status_event import StatusEvent as StatusEvent
-from braintree.subscription_details import SubscriptionDetails as SubscriptionDetails
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
-from braintree.three_d_secure_info import ThreeDSecureInfo as ThreeDSecureInfo
-from braintree.transaction_line_item import TransactionLineItem as TransactionLineItem
-from braintree.us_bank_account import UsBankAccount as UsBankAccount
-from braintree.venmo_account import VenmoAccount as VenmoAccount
-from braintree.visa_checkout_card import VisaCheckoutCard as VisaCheckoutCard
+from braintree.add_on import AddOn
+from braintree.address import Address
+from braintree.amex_express_checkout_card import AmexExpressCheckoutCard
+from braintree.android_pay_card import AndroidPayCard
+from braintree.apple_pay_card import ApplePayCard
+from braintree.authorization_adjustment import AuthorizationAdjustment
+from braintree.credit_card import CreditCard
+from braintree.customer import Customer
+from braintree.descriptor import Descriptor
+from braintree.disbursement_detail import DisbursementDetail
+from braintree.discount import Discount
+from braintree.dispute import Dispute
+from braintree.europe_bank_account import EuropeBankAccount
+from braintree.facilitated_details import FacilitatedDetails
+from braintree.facilitator_details import FacilitatorDetails
+from braintree.local_payment import LocalPayment
+from braintree.masterpass_card import MasterpassCard
+from braintree.meta_checkout_card import MetaCheckoutCard
+from braintree.meta_checkout_token import MetaCheckoutToken
+from braintree.package_details import PackageDetails
+from braintree.paypal_account import PayPalAccount
+from braintree.paypal_here import PayPalHere
+from braintree.resource import Resource
+from braintree.risk_data import RiskData
+from braintree.samsung_pay_card import SamsungPayCard
+from braintree.sepa_direct_debit_account import SepaDirectDebitAccount
+from braintree.status_event import StatusEvent
+from braintree.subscription_details import SubscriptionDetails
+from braintree.three_d_secure_info import ThreeDSecureInfo
+from braintree.us_bank_account import UsBankAccount
+from braintree.venmo_account import VenmoAccount
+from braintree.visa_checkout_card import VisaCheckoutCard
 
 class Transaction(Resource):
     class CreatedUsing:
-        FullInformation: str
-        Token: str
+        FullInformation: Final = "full_information"
+        Token: Final = "token"
 
     class GatewayRejectionReason:
-        ApplicationIncomplete: str
-        Avs: str
-        AvsAndCvv: str
-        Cvv: str
-        Duplicate: str
-        Fraud: str
-        RiskThreshold: str
-        ThreeDSecure: str
-        TokenIssuance: str
+        ApplicationIncomplete: Final = "application_incomplete"
+        Avs: Final = "avs"
+        AvsAndCvv: Final = "avs_and_cvv"
+        Cvv: Final = "cvv"
+        Duplicate: Final = "duplicate"
+        ExcessiveRetry: Final = "excessive_retry"
+        Fraud: Final = "fraud"
+        RiskThreshold: Final = "risk_threshold"
+        ThreeDSecure: Final = "three_d_secure"
+        TokenIssuance: Final = "token_issuance"
+
+    class ReasonCode:
+        ANY_REASON_CODE: Final = "any_reason_code"
 
     class Source:
-        Api: str
-        ControlPanel: str
-        Recurring: str
+        Api: Final = "api"
+        ControlPanel: Final = "control_panel"
+        Recurring: Final = "recurring"
 
     class EscrowStatus:
-        HoldPending: str
-        Held: str
-        ReleasePending: str
-        Released: str
-        Refunded: str
+        HoldPending: Final = "hold_pending"
+        Held: Final = "held"
+        ReleasePending: Final = "release_pending"
+        Released: Final = "released"
+        Refunded: Final = "refunded"
 
     class Status:
-        AuthorizationExpired: str
-        Authorized: str
-        Authorizing: str
-        Failed: str
-        GatewayRejected: str
-        ProcessorDeclined: str
-        Settled: str
-        SettlementConfirmed: str
-        SettlementDeclined: str
-        SettlementFailed: str
-        SettlementPending: str
-        Settling: str
-        SubmittedForSettlement: str
-        Voided: str
+        AuthorizationExpired: Final = "authorization_expired"
+        Authorized: Final = "authorized"
+        Authorizing: Final = "authorizing"
+        Failed: Final = "failed"
+        GatewayRejected: Final = "gateway_rejected"
+        ProcessorDeclined: Final = "processor_declined"
+        Settled: Final = "settled"
+        SettlementConfirmed: Final = "settlement_confirmed"
+        SettlementDeclined: Final = "settlement_declined"
+        SettlementFailed: Final = "settlement_failed"
+        SettlementPending: Final = "settlement_pending"
+        Settling: Final = "settling"
+        SubmittedForSettlement: Final = "submitted_for_settlement"
+        Voided: Final = "voided"
 
     class Type:
-        Credit: str
-        Sale: str
+        Credit: Final = "credit"
+        Sale: Final = "sale"
 
     class IndustryType:
-        Lodging: str
-        TravelAndCruise: str
-        TravelAndFlight: str
+        Lodging: Final = "lodging"
+        TravelAndCruise: Final = "travel_cruise"
+        TravelAndFlight: Final = "travel_flight"
 
     class AdditionalCharge:
-        Restaurant: str
-        GiftShop: str
-        MiniBar: str
-        Telephone: str
-        Laundry: str
-        Other: str
+        Restaurant: Final = "restaurant"
+        GiftShop: Final = "gift_shop"
+        MiniBar: Final = "mini_bar"
+        Telephone: Final = "telephone"
+        Laundry: Final = "laundry"
+        Other: Final = "other"
 
     @staticmethod
     def adjust_authorization(transaction_id, amount): ...
     @staticmethod
     def clone_transaction(transaction_id, params): ...
     @staticmethod
     def cancel_release(transaction_id): ...
@@ -129,54 +131,62 @@
     @staticmethod
     def clone_signature(): ...
     @staticmethod
     def create_signature(): ...
     @staticmethod
     def submit_for_settlement_signature(): ...
     @staticmethod
+    def package_tracking_signature(): ...
+    @staticmethod
+    def package_tracking(transaction_id, params: Incomplete | None = None): ...
+    @staticmethod
     def update_details_signature(): ...
     @staticmethod
     def refund_signature(): ...
     @staticmethod
     def submit_for_partial_settlement(transaction_id, amount, params: Incomplete | None = None): ...
-    amount: Any
-    tax_amount: Any
-    discount_amount: Any
-    shipping_amount: Any
-    billing_details: Any
-    credit_card_details: Any
-    paypal_details: Any
-    paypal_here_details: Any
-    local_payment_details: Any
-    europe_bank_account_details: Any
-    us_bank_account: Any
-    apple_pay_details: Any
-    android_pay_card_details: Any
-    amex_express_checkout_card_details: Any
-    venmo_account_details: Any
-    visa_checkout_card_details: Any
-    masterpass_card_details: Any
-    samsung_pay_card_details: Any
-    sca_exemption_requested: Any
-    customer_details: Any
-    shipping_details: Any
-    add_ons: Any
-    discounts: Any
-    status_history: Any
-    subscription_details: Any
-    descriptor: Any
-    disbursement_details: Any
-    disputes: Any
-    authorization_adjustments: Any
-    payment_instrument_type: Any
-    risk_data: Any
-    three_d_secure_info: Any
-    facilitated_details: Any
-    facilitator_details: Any
-    network_transaction_id: Any
+    amount: Decimal
+    tax_amount: Decimal | None
+    discount_amount: Decimal | None
+    shipping_amount: Decimal | None
+    billing_details: Address
+    credit_card_details: CreditCard
+    packages: list[PackageDetails]
+    paypal_details: PayPalAccount
+    paypal_here_details: PayPalHere
+    local_payment_details: LocalPayment
+    sepa_direct_debit_account_details: SepaDirectDebitAccount
+    europe_bank_account_details: EuropeBankAccount
+    us_bank_account: UsBankAccount
+    apple_pay_details: ApplePayCard
+    android_pay_card_details: AndroidPayCard
+    amex_express_checkout_card_details: AmexExpressCheckoutCard
+    venmo_account_details: VenmoAccount
+    visa_checkout_card_details: VisaCheckoutCard
+    masterpass_card_details: MasterpassCard
+    samsung_pay_card_details: SamsungPayCard
+    meta_checkout_card_details: MetaCheckoutCard
+    meta_checkout_token_details: MetaCheckoutToken
+    sca_exemption_requested: Incomplete
+    customer_details: Customer
+    shipping_details: Address
+    add_ons: list[AddOn]
+    discounts: list[Discount]
+    status_history: list[StatusEvent]
+    subscription_details: SubscriptionDetails
+    descriptor: Descriptor
+    disbursement_details: DisbursementDetail
+    disputes: list[Dispute]
+    authorization_adjustments: list[AuthorizationAdjustment]
+    payment_instrument_type: Incomplete
+    risk_data: RiskData | None
+    three_d_secure_info: ThreeDSecureInfo | None
+    facilitated_details: FacilitatedDetails
+    facilitator_details: FacilitatorDetails
+    network_transaction_id: Incomplete
     def __init__(self, gateway, attributes) -> None: ...
     @property
     def vault_billing_address(self): ...
     @property
     def vault_credit_card(self): ...
     @property
     def vault_customer(self): ...
```

### Comparing `types-braintree-4.25.0.20240331/braintree-stubs/transaction_gateway.pyi` & `types-braintree-4.28.0.20240402/braintree-stubs/transaction_gateway.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 from _typeshed import Incomplete
-from typing import Any
-
-from braintree.error_result import ErrorResult as ErrorResult
-from braintree.exceptions.not_found_error import NotFoundError as NotFoundError
-from braintree.exceptions.request_timeout_error import RequestTimeoutError as RequestTimeoutError
-from braintree.resource import Resource as Resource
-from braintree.resource_collection import ResourceCollection as ResourceCollection
-from braintree.successful_result import SuccessfulResult as SuccessfulResult
-from braintree.transaction import Transaction as Transaction
 
 class TransactionGateway:
-    gateway: Any
-    config: Any
+    gateway: Incomplete
+    config: Incomplete
     def __init__(self, gateway) -> None: ...
     def adjust_authorization(self, transaction_id, amount): ...
     def clone_transaction(self, transaction_id, params): ...
     def cancel_release(self, transaction_id): ...
     def create(self, params): ...
     def credit(self, params): ...
     def find(self, transaction_id): ...
@@ -23,8 +14,9 @@
     def refund(self, transaction_id, amount_or_options: Incomplete | None = None): ...
     def sale(self, params): ...
     def search(self, *query): ...
     def release_from_escrow(self, transaction_id): ...
     def submit_for_settlement(self, transaction_id, amount: Incomplete | None = None, params: Incomplete | None = None): ...
     def update_details(self, transaction_id, params: Incomplete | None = None): ...
     def submit_for_partial_settlement(self, transaction_id, amount, params: Incomplete | None = None): ...
+    def package_tracking(self, transaction_id, params: Incomplete | None = None): ...
     def void(self, transaction_id): ...
```

### Comparing `types-braintree-4.25.0.20240331/setup.py` & `types-braintree-4.28.0.20240402/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,44 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`.
 
 This version of `types-braintree` aims to provide accurate annotations
-for `braintree==4.25.*`.
+for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="4.25.0.20240331",
+      version="4.28.0.20240402",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['braintree-stubs'],
-      package_data={'braintree-stubs': ['__init__.pyi', 'account_updater_daily_report.pyi', 'ach_mandate.pyi', 'add_on.pyi', 'add_on_gateway.pyi', 'address.pyi', 'address_gateway.pyi', 'amex_express_checkout_card.pyi', 'android_pay_card.pyi', 'apple_pay_card.pyi', 'apple_pay_gateway.pyi', 'apple_pay_options.pyi', 'attribute_getter.pyi', 'authorization_adjustment.pyi', 'bin_data.pyi', 'braintree_gateway.pyi', 'client_token.pyi', 'client_token_gateway.pyi', 'configuration.pyi', 'connected_merchant_paypal_status_changed.pyi', 'connected_merchant_status_transitioned.pyi', 'credentials_parser.pyi', 'credit_card.pyi', 'credit_card_gateway.pyi', 'credit_card_verification.pyi', 'credit_card_verification_gateway.pyi', 'credit_card_verification_search.pyi', 'customer.pyi', 'customer_gateway.pyi', 'customer_search.pyi', 'descriptor.pyi', 'disbursement.pyi', 'disbursement_detail.pyi', 'discount.pyi', 'discount_gateway.pyi', 'dispute.pyi', 'dispute_details/__init__.pyi', 'dispute_details/evidence.pyi', 'dispute_details/paypal_message.pyi', 'dispute_details/status_history.pyi', 'dispute_gateway.pyi', 'dispute_search.pyi', 'document_upload.pyi', 'document_upload_gateway.pyi', 'environment.pyi', 'error_codes.pyi', 'error_result.pyi', 'errors.pyi', 'europe_bank_account.pyi', 'exceptions/__init__.pyi', 'exceptions/authentication_error.pyi', 'exceptions/authorization_error.pyi', 'exceptions/braintree_error.pyi', 'exceptions/configuration_error.pyi', 'exceptions/gateway_timeout_error.pyi', 'exceptions/http/__init__.pyi', 'exceptions/http/connection_error.pyi', 'exceptions/http/invalid_response_error.pyi', 'exceptions/http/timeout_error.pyi', 'exceptions/invalid_challenge_error.pyi', 'exceptions/invalid_signature_error.pyi', 'exceptions/not_found_error.pyi', 'exceptions/request_timeout_error.pyi', 'exceptions/server_error.pyi', 'exceptions/service_unavailable_error.pyi', 'exceptions/too_many_requests_error.pyi', 'exceptions/unexpected_error.pyi', 'exceptions/upgrade_required_error.pyi', 'facilitated_details.pyi', 'facilitator_details.pyi', 'granted_payment_instrument_update.pyi', 'iban_bank_account.pyi', 'ids_search.pyi', 'local_payment.pyi', 'local_payment_completed.pyi', 'local_payment_reversed.pyi', 'masterpass_card.pyi', 'merchant.pyi', 'merchant_account/__init__.pyi', 'merchant_account/address_details.pyi', 'merchant_account/business_details.pyi', 'merchant_account/funding_details.pyi', 'merchant_account/individual_details.pyi', 'merchant_account/merchant_account.pyi', 'merchant_account_gateway.pyi', 'merchant_gateway.pyi', 'modification.pyi', 'oauth_access_revocation.pyi', 'oauth_credentials.pyi', 'oauth_gateway.pyi', 'paginated_collection.pyi', 'paginated_result.pyi', 'partner_merchant.pyi', 'payment_instrument_type.pyi', 'payment_method.pyi', 'payment_method_gateway.pyi', 'payment_method_nonce.pyi', 'payment_method_nonce_gateway.pyi', 'payment_method_parser.pyi', 'paypal_account.pyi', 'paypal_account_gateway.pyi', 'paypal_here.pyi', 'plan.pyi', 'plan_gateway.pyi', 'processor_response_types.pyi', 'resource.pyi', 'resource_collection.pyi', 'revoked_payment_method_metadata.pyi', 'risk_data.pyi', 'samsung_pay_card.pyi', 'search.pyi', 'settlement_batch_summary.pyi', 'settlement_batch_summary_gateway.pyi', 'signature_service.pyi', 'status_event.pyi', 'subscription.pyi', 'subscription_details.pyi', 'subscription_gateway.pyi', 'subscription_search.pyi', 'subscription_status_event.pyi', 'successful_result.pyi', 'testing_gateway.pyi', 'three_d_secure_info.pyi', 'transaction.pyi', 'transaction_amounts.pyi', 'transaction_details.pyi', 'transaction_gateway.pyi', 'transaction_line_item.pyi', 'transaction_line_item_gateway.pyi', 'transaction_search.pyi', 'unknown_payment_method.pyi', 'us_bank_account.pyi', 'us_bank_account_gateway.pyi', 'us_bank_account_verification.pyi', 'us_bank_account_verification_gateway.pyi', 'us_bank_account_verification_search.pyi', 'util/__init__.pyi', 'util/constants.pyi', 'util/crypto.pyi', 'util/datetime_parser.pyi', 'util/generator.pyi', 'util/graphql_client.pyi', 'util/http.pyi', 'util/parser.pyi', 'util/xml_util.pyi', 'validation_error.pyi', 'validation_error_collection.pyi', 'venmo_account.pyi', 'version.pyi', 'visa_checkout_card.pyi', 'webhook_notification.pyi', 'webhook_notification_gateway.pyi', 'webhook_testing.pyi', 'webhook_testing_gateway.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'braintree-stubs': ['__init__.pyi', 'account_updater_daily_report.pyi', 'ach_mandate.pyi', 'add_on.pyi', 'add_on_gateway.pyi', 'address.pyi', 'address_gateway.pyi', 'amex_express_checkout_card.pyi', 'android_pay_card.pyi', 'apple_pay_card.pyi', 'apple_pay_gateway.pyi', 'apple_pay_options.pyi', 'attribute_getter.pyi', 'authorization_adjustment.pyi', 'bin_data.pyi', 'braintree_gateway.pyi', 'client_token.pyi', 'client_token_gateway.pyi', 'configuration.pyi', 'connected_merchant_paypal_status_changed.pyi', 'connected_merchant_status_transitioned.pyi', 'credentials_parser.pyi', 'credit_card.pyi', 'credit_card_gateway.pyi', 'credit_card_verification.pyi', 'credit_card_verification_gateway.pyi', 'credit_card_verification_search.pyi', 'customer.pyi', 'customer_gateway.pyi', 'customer_search.pyi', 'descriptor.pyi', 'disbursement.pyi', 'disbursement_detail.pyi', 'discount.pyi', 'discount_gateway.pyi', 'dispute.pyi', 'dispute_details/__init__.pyi', 'dispute_details/evidence.pyi', 'dispute_details/paypal_message.pyi', 'dispute_details/status_history.pyi', 'dispute_gateway.pyi', 'dispute_search.pyi', 'document_upload.pyi', 'document_upload_gateway.pyi', 'enriched_customer_data.pyi', 'environment.pyi', 'error_codes.pyi', 'error_result.pyi', 'errors.pyi', 'europe_bank_account.pyi', 'exceptions/__init__.pyi', 'exceptions/authentication_error.pyi', 'exceptions/authorization_error.pyi', 'exceptions/braintree_error.pyi', 'exceptions/configuration_error.pyi', 'exceptions/gateway_timeout_error.pyi', 'exceptions/http/__init__.pyi', 'exceptions/http/connection_error.pyi', 'exceptions/http/invalid_response_error.pyi', 'exceptions/http/timeout_error.pyi', 'exceptions/invalid_challenge_error.pyi', 'exceptions/invalid_signature_error.pyi', 'exceptions/not_found_error.pyi', 'exceptions/request_timeout_error.pyi', 'exceptions/server_error.pyi', 'exceptions/service_unavailable_error.pyi', 'exceptions/test_operation_performed_in_production_error.pyi', 'exceptions/too_many_requests_error.pyi', 'exceptions/unexpected_error.pyi', 'exceptions/upgrade_required_error.pyi', 'exchange_rate_quote.pyi', 'exchange_rate_quote_gateway.pyi', 'exchange_rate_quote_input.pyi', 'exchange_rate_quote_payload.pyi', 'exchange_rate_quote_request.pyi', 'facilitated_details.pyi', 'facilitator_details.pyi', 'granted_payment_instrument_update.pyi', 'iban_bank_account.pyi', 'ids_search.pyi', 'liability_shift.pyi', 'local_payment.pyi', 'local_payment_completed.pyi', 'local_payment_expired.pyi', 'local_payment_funded.pyi', 'local_payment_reversed.pyi', 'masterpass_card.pyi', 'merchant.pyi', 'merchant_account/__init__.pyi', 'merchant_account/address_details.pyi', 'merchant_account/business_details.pyi', 'merchant_account/funding_details.pyi', 'merchant_account/individual_details.pyi', 'merchant_account/merchant_account.pyi', 'merchant_account_gateway.pyi', 'merchant_gateway.pyi', 'meta_checkout_card.pyi', 'meta_checkout_token.pyi', 'modification.pyi', 'montary_amount.pyi', 'oauth_access_revocation.pyi', 'oauth_credentials.pyi', 'oauth_gateway.pyi', 'package_details.pyi', 'paginated_collection.pyi', 'paginated_result.pyi', 'partner_merchant.pyi', 'payment_instrument_type.pyi', 'payment_method.pyi', 'payment_method_customer_data_updated_metadata.pyi', 'payment_method_gateway.pyi', 'payment_method_nonce.pyi', 'payment_method_nonce_gateway.pyi', 'payment_method_parser.pyi', 'paypal_account.pyi', 'paypal_account_gateway.pyi', 'paypal_here.pyi', 'plan.pyi', 'plan_gateway.pyi', 'processor_response_types.pyi', 'resource.pyi', 'resource_collection.pyi', 'revoked_payment_method_metadata.pyi', 'risk_data.pyi', 'samsung_pay_card.pyi', 'search.pyi', 'sepa_direct_debit_account.pyi', 'sepa_direct_debit_account_gateway.pyi', 'settlement_batch_summary.pyi', 'settlement_batch_summary_gateway.pyi', 'signature_service.pyi', 'status_event.pyi', 'subscription.pyi', 'subscription_details.pyi', 'subscription_gateway.pyi', 'subscription_search.pyi', 'subscription_status_event.pyi', 'successful_result.pyi', 'test/__init__.pyi', 'test/authentication_ids.pyi', 'test/credit_card_defaults.pyi', 'test/credit_card_numbers.pyi', 'test/merchant_account.pyi', 'test/nonces.pyi', 'test/venmo_sdk.pyi', 'testing_gateway.pyi', 'three_d_secure_info.pyi', 'transaction.pyi', 'transaction_amounts.pyi', 'transaction_details.pyi', 'transaction_gateway.pyi', 'transaction_line_item.pyi', 'transaction_line_item_gateway.pyi', 'transaction_review.pyi', 'transaction_search.pyi', 'unknown_payment_method.pyi', 'us_bank_account.pyi', 'us_bank_account_gateway.pyi', 'us_bank_account_verification.pyi', 'us_bank_account_verification_gateway.pyi', 'us_bank_account_verification_search.pyi', 'util/__init__.pyi', 'util/constants.pyi', 'util/crypto.pyi', 'util/datetime_parser.pyi', 'util/generator.pyi', 'util/graphql_client.pyi', 'util/http.pyi', 'util/parser.pyi', 'util/xml_util.pyi', 'validation_error.pyi', 'validation_error_collection.pyi', 'venmo_account.pyi', 'venmo_profile_data.pyi', 'version.pyi', 'visa_checkout_card.pyi', 'webhook_notification.pyi', 'webhook_notification_gateway.pyi', 'webhook_testing.pyi', 'webhook_testing_gateway.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-braintree-4.25.0.20240331/types_braintree.egg-info/PKG-INFO` & `types-braintree-4.28.0.20240402/types_braintree.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.25.0.20240331
+Version: 4.28.0.20240402
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`.
 
 This version of `types-braintree` aims to provide accurate annotations
-for `braintree==4.25.*`.
+for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

### Comparing `types-braintree-4.25.0.20240331/types_braintree.egg-info/SOURCES.txt` & `types-braintree-4.28.0.20240402/types_braintree.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -38,40 +38,54 @@
 braintree-stubs/discount.pyi
 braintree-stubs/discount_gateway.pyi
 braintree-stubs/dispute.pyi
 braintree-stubs/dispute_gateway.pyi
 braintree-stubs/dispute_search.pyi
 braintree-stubs/document_upload.pyi
 braintree-stubs/document_upload_gateway.pyi
+braintree-stubs/enriched_customer_data.pyi
 braintree-stubs/environment.pyi
 braintree-stubs/error_codes.pyi
 braintree-stubs/error_result.pyi
 braintree-stubs/errors.pyi
 braintree-stubs/europe_bank_account.pyi
+braintree-stubs/exchange_rate_quote.pyi
+braintree-stubs/exchange_rate_quote_gateway.pyi
+braintree-stubs/exchange_rate_quote_input.pyi
+braintree-stubs/exchange_rate_quote_payload.pyi
+braintree-stubs/exchange_rate_quote_request.pyi
 braintree-stubs/facilitated_details.pyi
 braintree-stubs/facilitator_details.pyi
 braintree-stubs/granted_payment_instrument_update.pyi
 braintree-stubs/iban_bank_account.pyi
 braintree-stubs/ids_search.pyi
+braintree-stubs/liability_shift.pyi
 braintree-stubs/local_payment.pyi
 braintree-stubs/local_payment_completed.pyi
+braintree-stubs/local_payment_expired.pyi
+braintree-stubs/local_payment_funded.pyi
 braintree-stubs/local_payment_reversed.pyi
 braintree-stubs/masterpass_card.pyi
 braintree-stubs/merchant.pyi
 braintree-stubs/merchant_account_gateway.pyi
 braintree-stubs/merchant_gateway.pyi
+braintree-stubs/meta_checkout_card.pyi
+braintree-stubs/meta_checkout_token.pyi
 braintree-stubs/modification.pyi
+braintree-stubs/montary_amount.pyi
 braintree-stubs/oauth_access_revocation.pyi
 braintree-stubs/oauth_credentials.pyi
 braintree-stubs/oauth_gateway.pyi
+braintree-stubs/package_details.pyi
 braintree-stubs/paginated_collection.pyi
 braintree-stubs/paginated_result.pyi
 braintree-stubs/partner_merchant.pyi
 braintree-stubs/payment_instrument_type.pyi
 braintree-stubs/payment_method.pyi
+braintree-stubs/payment_method_customer_data_updated_metadata.pyi
 braintree-stubs/payment_method_gateway.pyi
 braintree-stubs/payment_method_nonce.pyi
 braintree-stubs/payment_method_nonce_gateway.pyi
 braintree-stubs/payment_method_parser.pyi
 braintree-stubs/paypal_account.pyi
 braintree-stubs/paypal_account_gateway.pyi
 braintree-stubs/paypal_here.pyi
@@ -81,14 +95,16 @@
 braintree-stubs/py.typed
 braintree-stubs/resource.pyi
 braintree-stubs/resource_collection.pyi
 braintree-stubs/revoked_payment_method_metadata.pyi
 braintree-stubs/risk_data.pyi
 braintree-stubs/samsung_pay_card.pyi
 braintree-stubs/search.pyi
+braintree-stubs/sepa_direct_debit_account.pyi
+braintree-stubs/sepa_direct_debit_account_gateway.pyi
 braintree-stubs/settlement_batch_summary.pyi
 braintree-stubs/settlement_batch_summary_gateway.pyi
 braintree-stubs/signature_service.pyi
 braintree-stubs/status_event.pyi
 braintree-stubs/subscription.pyi
 braintree-stubs/subscription_details.pyi
 braintree-stubs/subscription_gateway.pyi
@@ -99,24 +115,26 @@
 braintree-stubs/three_d_secure_info.pyi
 braintree-stubs/transaction.pyi
 braintree-stubs/transaction_amounts.pyi
 braintree-stubs/transaction_details.pyi
 braintree-stubs/transaction_gateway.pyi
 braintree-stubs/transaction_line_item.pyi
 braintree-stubs/transaction_line_item_gateway.pyi
+braintree-stubs/transaction_review.pyi
 braintree-stubs/transaction_search.pyi
 braintree-stubs/unknown_payment_method.pyi
 braintree-stubs/us_bank_account.pyi
 braintree-stubs/us_bank_account_gateway.pyi
 braintree-stubs/us_bank_account_verification.pyi
 braintree-stubs/us_bank_account_verification_gateway.pyi
 braintree-stubs/us_bank_account_verification_search.pyi
 braintree-stubs/validation_error.pyi
 braintree-stubs/validation_error_collection.pyi
 braintree-stubs/venmo_account.pyi
+braintree-stubs/venmo_profile_data.pyi
 braintree-stubs/version.pyi
 braintree-stubs/visa_checkout_card.pyi
 braintree-stubs/webhook_notification.pyi
 braintree-stubs/webhook_notification_gateway.pyi
 braintree-stubs/webhook_testing.pyi
 braintree-stubs/webhook_testing_gateway.pyi
 braintree-stubs/dispute_details/__init__.pyi
@@ -131,27 +149,35 @@
 braintree-stubs/exceptions/gateway_timeout_error.pyi
 braintree-stubs/exceptions/invalid_challenge_error.pyi
 braintree-stubs/exceptions/invalid_signature_error.pyi
 braintree-stubs/exceptions/not_found_error.pyi
 braintree-stubs/exceptions/request_timeout_error.pyi
 braintree-stubs/exceptions/server_error.pyi
 braintree-stubs/exceptions/service_unavailable_error.pyi
+braintree-stubs/exceptions/test_operation_performed_in_production_error.pyi
 braintree-stubs/exceptions/too_many_requests_error.pyi
 braintree-stubs/exceptions/unexpected_error.pyi
 braintree-stubs/exceptions/upgrade_required_error.pyi
 braintree-stubs/exceptions/http/__init__.pyi
 braintree-stubs/exceptions/http/connection_error.pyi
 braintree-stubs/exceptions/http/invalid_response_error.pyi
 braintree-stubs/exceptions/http/timeout_error.pyi
 braintree-stubs/merchant_account/__init__.pyi
 braintree-stubs/merchant_account/address_details.pyi
 braintree-stubs/merchant_account/business_details.pyi
 braintree-stubs/merchant_account/funding_details.pyi
 braintree-stubs/merchant_account/individual_details.pyi
 braintree-stubs/merchant_account/merchant_account.pyi
+braintree-stubs/test/__init__.pyi
+braintree-stubs/test/authentication_ids.pyi
+braintree-stubs/test/credit_card_defaults.pyi
+braintree-stubs/test/credit_card_numbers.pyi
+braintree-stubs/test/merchant_account.pyi
+braintree-stubs/test/nonces.pyi
+braintree-stubs/test/venmo_sdk.pyi
 braintree-stubs/util/__init__.pyi
 braintree-stubs/util/constants.pyi
 braintree-stubs/util/crypto.pyi
 braintree-stubs/util/datetime_parser.pyi
 braintree-stubs/util/generator.pyi
 braintree-stubs/util/graphql_client.pyi
 braintree-stubs/util/http.pyi
```

